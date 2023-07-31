# Comparing `tmp/shaped_target_clickhouse-0.0.1.tar.gz` & `tmp/shaped_target_clickhouse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaped_target_clickhouse-0.0.1.tar", max compression
+gzip compressed data, was "shaped_target_clickhouse-0.0.2.tar", max compression
```

## Comparing `shaped_target_clickhouse-0.0.1.tar` & `shaped_target_clickhouse-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/LICENSE
--rw-r--r--   0        0        0     4314 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/README.md
--rw-r--r--   0        0        0     1413 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/target_clickhouse/__init__.py
--rw-r--r--   0        0        0     4436 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/target_clickhouse/sinks.py
--rw-r--r--   0        0        0      645 2023-06-12 23:01:25.180175 shaped_target_clickhouse-0.0.1/target_clickhouse/target.py
--rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4314 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/README.md
+-rw-r--r--   0        0        0     1413 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/__init__.py
+-rw-r--r--   0        0        0     4695 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/sinks.py
+-rw-r--r--   0        0        0      645 2023-07-31 19:00:05.781473 shaped_target_clickhouse-0.0.2/target_clickhouse/target.py
+-rw-r--r--   0        0        0     5109 1970-01-01 00:00:00.000000 shaped_target_clickhouse-0.0.2/PKG-INFO
```

### Comparing `shaped_target_clickhouse-0.0.1/LICENSE` & `shaped_target_clickhouse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.1/README.md` & `shaped_target_clickhouse-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.1/pyproject.toml` & `shaped_target_clickhouse-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shaped-target-clickhouse"
-version = "0.0.1"
+version = "0.0.2"
 description = "`target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK."
 readme = "README.md"
 authors = ["Ben Theunissen"]
 keywords = [
     "ELT",
     "clickhouse",
 ]
@@ -18,15 +18,15 @@
 singer-sdk = { version="^0.28.0" }
 fs-s3fs = { version = "^1.1.1", optional = true }
 clickhouse-sqlalchemy = "^0.2.4"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 tox = "^3.25.0"
-ruff = "^0.0.272"
+ruff = "^0.0.278"
 singer-sdk = { version="^0.28.0", extras = ["testing"] }
 
 [tool.poetry.extras]
 s3 = ["fs-s3fs"]
 
 [tool.ruff]
 ignore = [
@@ -47,13 +47,13 @@
 [tool.ruff.isort]
 known-first-party = ["target_clickhouse"]
 
 [tool.ruff.pylint]
 max-args=6
 
 [build-system]
-requires = ["poetry-core>=1.0.8"]
+requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 # CLI declaration
 target-clickhouse = 'target_clickhouse.target:TargetClickhouse.cli'
```

### Comparing `shaped_target_clickhouse-0.0.1/target_clickhouse/sinks.py` & `shaped_target_clickhouse-0.0.2/target_clickhouse/sinks.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,11 +113,21 @@
                 ),
             )
 
         table_engine = engines.MergeTree(primary_key=primary_keys)
         _ = Table(table_name, meta, *columns, table_engine)
         meta.create_all(self._engine)
 
+    def prepare_schema(self, _: str) -> None:
+        """Create the target database schema.
+
+        In Clickhouse, a schema is a database, so this method is a no-op.
+
+        Args:
+            schema_name: The target schema name.
+        """
+        return
+
 class ClickhouseSink(SQLSink):
     """clickhouse target sink class."""
 
     connector_class = ClickhouseConnector
```

### Comparing `shaped_target_clickhouse-0.0.1/target_clickhouse/target.py` & `shaped_target_clickhouse-0.0.2/target_clickhouse/target.py`

 * *Files identical despite different names*

### Comparing `shaped_target_clickhouse-0.0.1/PKG-INFO` & `shaped_target_clickhouse-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shaped-target-clickhouse
-Version: 0.0.1
+Version: 0.0.2
 Summary: `target-clickhouse` is a Singer target for clickhouse, built with the Meltano Singer SDK.
 License: Apache-2.0
 Keywords: ELT,clickhouse
 Author: Ben Theunissen
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

