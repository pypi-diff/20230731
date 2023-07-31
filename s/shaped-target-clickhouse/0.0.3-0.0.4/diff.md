# Comparing `tmp/shaped_target_clickhouse-0.0.3.tar.gz` & `tmp/shaped_target_clickhouse-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaped_target_clickhouse-0.0.3.tar", max compression
+gzip compressed data, was "shaped_target_clickhouse-0.0.4.tar", max compression
```

## Comparing `shaped_target_clickhouse-0.0.3.tar` & `shaped_target_clickhouse-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/LICENSE
--rw-r--r--   0        0        0     4397 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/README.md
--rw-r--r--   0        0        0     1413 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/__init__.py
--rw-r--r--   0        0        0     4745 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/sinks.py
--rw-r--r--   0        0        0      775 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/target.py
--rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4397 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/README.md
+-rw-r--r--   0        0        0     1413 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/__init__.py
+-rw-r--r--   0        0        0     5422 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/sinks.py
+-rw-r--r--   0        0        0      775 2023-07-31 20:27:09.923095 shaped_target_clickhouse-0.0.4/target_clickhouse/target.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.4/PKG-INFO
```

### Comparing `shaped_target_clickhouse-0.0.3/LICENSE` & `shaped_target_clickhouse-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.3/README.md` & `shaped_target_clickhouse-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.3/pyproject.toml` & `shaped_target_clickhouse-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaped-target-clickhouse"
-version = "0.0.3"
+version = "0.0.4"
 description = "`target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Ben Theunissen"]
 keywords = [
     "ELT",
     "clickhouse",
 ]
```

### Comparing `shaped_target_clickhouse-0.0.3/target_clickhouse/sinks.py` & `shaped_target_clickhouse-0.0.4/target_clickhouse/sinks.py`

 * *Files 13% similar despite different names*

```diff
@@ -91,14 +91,19 @@
         if as_temp_table:
             msg = "Temporary tables are not supported."
             raise NotImplementedError(msg)
 
         _ = partition_keys  # Not supported in generic implementation.
 
         _, _, table_name = self.parse_full_table_name(full_table_name)
+
+        # If config table name is set, then use it instead of the table name.
+        if self.config.get("table_name"):
+            table_name = self.config.get("table_name")
+
         # Do not set schema, as it is not supported by Clickhouse.
         meta = MetaData(schema=None, bind=self._engine)
         columns: list[Column] = []
         primary_keys = primary_keys or []
         try:
             properties: dict = schema["properties"]
         except KeyError as e:
@@ -128,7 +133,24 @@
         """
         return
 
 class ClickhouseSink(SQLSink):
     """clickhouse target sink class."""
 
     connector_class = ClickhouseConnector
+
+    @property
+    def full_table_name(self) -> str:
+        """Return the fully qualified table name.
+
+        Returns
+            The fully qualified table name.
+        """
+        # Use the config table name if set.
+        if self.config.get("table_name"):
+            return self.config.get("table_name")
+
+        return self.connector.get_fully_qualified_name(
+            table_name=self.table_name,
+            schema_name=self.schema_name,
+            db_name=self.database_name,
+        )
```

### Comparing `shaped_target_clickhouse-0.0.3/target_clickhouse/target.py` & `shaped_target_clickhouse-0.0.4/target_clickhouse/target.py`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.3/PKG-INFO` & `shaped_target_clickhouse-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped-target-clickhouse
-Version: 0.0.3
+Version: 0.0.4
 Summary: `target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,clickhouse
 Author: Ben Theunissen
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

