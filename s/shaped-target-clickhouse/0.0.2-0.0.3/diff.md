# Comparing `tmp/shaped_target_clickhouse-0.0.2.tar.gz` & `tmp/shaped_target_clickhouse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaped_target_clickhouse-0.0.2.tar", max compression
+gzip compressed data, was "shaped_target_clickhouse-0.0.3.tar", max compression
```

## Comparing `shaped_target_clickhouse-0.0.2.tar` & `shaped_target_clickhouse-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/LICENSE
--rw-r--r--   0        0        0     4314 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/README.md
--rw-r--r--   0        0        0     1413 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       29 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/__init__.py
--rw-r--r--   0        0        0     4695 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/sinks.py
--rw-r--r--   0        0        0      645 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/target.py
--rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4397 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/README.md
+-rw-r--r--   0        0        0     1413 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/__init__.py
+-rw-r--r--   0        0        0     4745 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/sinks.py
+-rw-r--r--   0        0        0      775 2023-07-31 20:03:33.670220 shaped_target_clickhouse-0.0.3/target_clickhouse/target.py
+-rw-r--r--   0        0        0     5192 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.3/PKG-INFO
```

### Comparing `shaped_target_clickhouse-0.0.2/LICENSE` & `shaped_target_clickhouse-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.2/README.md` & `shaped_target_clickhouse-0.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 target-clickhouse --about --format=markdown
 ```
 -->
 
 | Setting              | Required | Default | Description |
 |:---------------------|:--------:|:-------:|:------------|
 | sqlalchemy_url       | False    | None    | SQLAlchemy connection string |
+| table_name           | False    | None    | The name of the table to write to. |
 | default_target_schema| False    | None    | The default target database schema name to use for all streams. |
 | stream_maps          | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config    | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled   | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-clickhouse --about`
```

### Comparing `shaped_target_clickhouse-0.0.2/pyproject.toml` & `shaped_target_clickhouse-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaped-target-clickhouse"
-version = "0.0.2"
+version = "0.0.3"
 description = "`target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Ben Theunissen"]
 keywords = [
     "ELT",
     "clickhouse",
 ]
```

### Comparing `shaped_target_clickhouse-0.0.2/target_clickhouse/sinks.py` & `shaped_target_clickhouse-0.0.3/target_clickhouse/sinks.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,17 @@
         """
         if as_temp_table:
             msg = "Temporary tables are not supported."
             raise NotImplementedError(msg)
 
         _ = partition_keys  # Not supported in generic implementation.
 
-        _, schema_name, table_name = self.parse_full_table_name(full_table_name)
-        meta = MetaData(schema=schema_name, bind=self._engine)
+        _, _, table_name = self.parse_full_table_name(full_table_name)
+        # Do not set schema, as it is not supported by Clickhouse.
+        meta = MetaData(schema=None, bind=self._engine)
         columns: list[Column] = []
         primary_keys = primary_keys or []
         try:
             properties: dict = schema["properties"]
         except KeyError as e:
             msg = f"Schema for '{full_table_name}' does not define properties: {schema}"
             raise RuntimeError(msg) from e
```

### Comparing `shaped_target_clickhouse-0.0.2/target_clickhouse/target.py` & `shaped_target_clickhouse-0.0.3/target_clickhouse/target.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,18 @@
     config_jsonschema = th.PropertiesList(
         th.Property(
             "sqlalchemy_url",
             th.StringType,
             secret=True,  # Flag config as protected.
             description="SQLAlchemy connection string",
         ),
+        th.Property(
+            "table_name",
+            th.StringType,
+            description="Target table name",
+        ),
     ).to_dict()
 
     default_sink_class = ClickhouseSink
 
 if __name__ == "__main__":
     TargetClickhouse.cli()
```

### Comparing `shaped_target_clickhouse-0.0.2/PKG-INFO` & `shaped_target_clickhouse-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped-target-clickhouse
-Version: 0.0.2
+Version: 0.0.3
 Summary: `target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,clickhouse
 Author: Ben Theunissen
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -57,14 +57,15 @@
 target-clickhouse --about --format=markdown
 ```
 -->
 
 | Setting              | Required | Default | Description |
 |:---------------------|:--------:|:-------:|:------------|
 | sqlalchemy_url       | False    | None    | SQLAlchemy connection string |
+| table_name           | False    | None    | The name of the table to write to. |
 | default_target_schema| False    | None    | The default target database schema name to use for all streams. |
 | stream_maps          | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config    | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled   | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-clickhouse --about`
```

