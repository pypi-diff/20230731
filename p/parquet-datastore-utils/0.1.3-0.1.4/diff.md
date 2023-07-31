# Comparing `tmp/parquet_datastore_utils-0.1.3-py3-none-any.whl.zip` & `tmp/parquet_datastore_utils-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4072 bytes, number of entries: 6
+Zip file size: 4698 bytes, number of entries: 6
 -rw-r--r--  2.0 fat       37 b- defN 80-Jan-01 00:00 parquet_datastore_utils/__init__.py
 -rw-r--r--  2.0 fat      570 b- defN 80-Jan-01 00:00 parquet_datastore_utils/cleaner.py
--rw-r--r--  2.0 fat     6026 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
--rw-r--r--  2.0 fat      626 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/WHEEL
-?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.3.dist-info/RECORD
-6 files, 7874 bytes uncompressed, 3104 bytes compressed:  60.6%
+-rw-r--r--  2.0 fat     8125 b- defN 80-Jan-01 00:00 parquet_datastore_utils/read_write.py
+-rw-r--r--  2.0 fat      712 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 parquet_datastore_utils-0.1.4.dist-info/WHEEL
+?rw-r--r--  2.0 fat      527 b- defN 16-Jan-01 00:00 parquet_datastore_utils-0.1.4.dist-info/RECORD
+6 files, 10059 bytes uncompressed, 3730 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: parquet_datastore_utils/cleaner.py
 Comment: 
 
 Filename: parquet_datastore_utils/read_write.py
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.3.dist-info/METADATA
+Filename: parquet_datastore_utils-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.3.dist-info/WHEEL
+Filename: parquet_datastore_utils-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: parquet_datastore_utils-0.1.3.dist-info/RECORD
+Filename: parquet_datastore_utils-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## parquet_datastore_utils/read_write.py

```diff
@@ -98,42 +98,102 @@
     overwrite_period: bool
         Only applicable to timeseries data where there is existing data in the destination. If True, any chunks that
         overlap with the new data will be loaded, existing data in the interval covered by the new data will be removed,
         and the new data will be merged with any remaining data from those chunks. The result will then be written to
         `uri`. Only once the write is successful, all but the newest file in each partition directory will be removed,
         avoiding duplicate data in any given time period.
     """
-
-    # Simple case, new dataset or relying on default behaviour
-    if not fsspec.get_mapper(uri).fs.exists(uri) or not overwrite_period:
-        data.to_parquet(uri, partition_cols=partition_cols)
-        return
-
-    current_ds = pq.ParquetDataset(uri)
-
-    update_tables = []
-    for fragment in current_ds.fragments:
-        parts = ds._get_partition_keys(fragment.partition_expression)
-        if all([(data[key]==value).any() for key, value in parts.items()]):
-            update_tables.append(fragment.to_table())
-
-    new_table = pa.table(data)
-
-    if len(update_tables) > 0:
-    # Data overlaps data in exsiting fragments
-        ind = data.index.name
-        filtered_table = pa.concat_tables(update_tables, promote=True).filter(
-            (pc.field(ind) < data.index.min()), (pc.field(ind) > data.index.max()))
-
-        filtered_table = filtered_table.set_column(filtered_table.column_names.index(ind), ind, filtered_table[ind].cast(new_table[ind].type))
-
-        out = pa.concat_tables([filtered_table, new_table], promote=True)  # Promote=True to allow for mismatched schemas
-    else:
-        out = new_table
-
-    pq.write_to_dataset(out, uri, partition_cols=partition_cols, use_legacy_dataset=False)
-
-    dirs = set([os.path.dirname(fragment.path) for fragment in current_ds.fragments])
-
-    for dir in dirs:
-        delete_all_except_newest(dir)
+    keys = get_partition_keys(data, partition_cols)
+    wait_until_released(keys)
+    try:
+        # Simple case, new dataset or relying on default behaviour
+        if not fsspec.get_mapper(uri).fs.exists(uri) or not overwrite_period:
+            data.to_parquet(uri, partition_cols=partition_cols)
+            return
+
+        new_table = pa.table(data)
+        current_ds = pq.ParquetDataset(uri)
+
+        update_tables = []
+        for fragment in current_ds.fragments:
+            parts = ds._get_partition_keys(fragment.partition_expression)
+            if all([(data[key]==value).any() for key, value in parts.items()]):
+                fragment_data = fragment.to_table()
+                # append with partition values
+                for key, value in parts.items():
+                    value_array = pa.array(fragment_data.num_rows * [value], type=new_table[key].type)
+                    fragment_data = fragment_data.append_column(key, value_array)
+                update_tables.append(fragment_data)
+
+        if len(update_tables) > 0:
+            # Data overlaps data in exsiting fragments
+            index_name = data.index.name
+            existing_table = pa.concat_tables(update_tables, promote=True)
+            existing_table = existing_table.set_column(existing_table.column_names.index(index_name), index_name, existing_table[index_name].cast(new_table[index_name].type))
+            data_before = existing_table.filter((pc.field(index_name) < data.index.min()))
+            data__after = existing_table.filter((pc.field(index_name) > data.index.max()))
+            out = pa.concat_tables([data_before, new_table, data__after], promote=True)  # Promote=True to allow for mismatched schemas
+        else:
+            out = new_table
+
+        pq.write_to_dataset(out, uri, partition_cols=partition_cols, use_legacy_dataset=False)
+        dirs = set([os.path.dirname(fragment.path) for fragment in current_ds.fragments])
+        for dir in dirs:
+            delete_all_except_newest(dir)
+    finally:
+        release_lock(keys)
+    return
+
+
+import time
+MAX_CHECKS = 100
+SLEEP_SECONDS = 0.2
+global LOCKS
+LOCKS = []
+
+
+def wait_until_released(partition_keys):
+    """waits until all locks for the partition are dealt with, then locks partition keys"""
+    for i in range(MAX_CHECKS):
+        isLocked = check_is_locked(partition_keys)
+        if not isLocked:
+            break
+        time.sleep(SLEEP_SECONDS)
+    return do_lock(partition_keys)
+
+
+def check_is_locked(partition_keys):
+    """queries if any of the partion keys is locked"""
+    for key in partition_keys:
+        if key in LOCKS:
+            return True
+    return False
+
+
+def do_lock(partition_keys):
+    """registers the partition key as locked"""
+    global LOCKS
+    for key in partition_keys:
+        LOCKS.append(key)
+    return
+
+
+def release_lock(partition_keys):
+    """removes the partition from the lock"""
+    global LOCKS
+    for key in partition_keys:
+        try:
+            LOCKS.remove(key)
+        except:
+            pass
+    return
+
+
+def get_partition_keys(data, partition_cols):
+    """extracts unique names based on the partition-related values in the data"""
+    series = pd.Series(name="tmp", index=data.index, dtype=str)
+    series = series.fillna("")
+    for column in partition_cols:
+        series =  series + "-" + data[column].astype(str)
+    keys = list(np.unique(series))
+    return keys
```

## Comparing `parquet_datastore_utils-0.1.3.dist-info/RECORD` & `parquet_datastore_utils-0.1.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 parquet_datastore_utils/__init__.py,sha256=XxoVYuFy3yGwKLNGU2tMsNEzP4gvKgE_cQmzcjmzthY,37
 parquet_datastore_utils/cleaner.py,sha256=nBjY8IYPN9hGTUbgwVsi0iCb3EC42dE6HRojcfHfZdg,570
-parquet_datastore_utils/read_write.py,sha256=p5UMmZcfV1CRnBMYALTa_NfWUhnnVmXL7xJ7pH9PUc8,6026
-parquet_datastore_utils-0.1.3.dist-info/METADATA,sha256=YRk8GOD3DZMc4pnEZnR7Qb9XJBXcQLCIfBl_NkCCiuM,626
-parquet_datastore_utils-0.1.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-parquet_datastore_utils-0.1.3.dist-info/RECORD,,
+parquet_datastore_utils/read_write.py,sha256=R1uYcgPkgPuRh-DhZkH0MHcWMsv41YgBMUZMsWG6BgM,8125
+parquet_datastore_utils-0.1.4.dist-info/METADATA,sha256=1ghb6Ja3AbdQS3mqmoCwaVmuuMBhnViuomFsGNLSDH8,712
+parquet_datastore_utils-0.1.4.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+parquet_datastore_utils-0.1.4.dist-info/RECORD,,
```

