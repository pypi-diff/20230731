# Comparing `tmp/datapipe_core-0.13.0a7.tar.gz` & `tmp/datapipe_core-0.13.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.13.0a7.tar", max compression
+gzip compressed data, was "datapipe_core-0.13.0a8.tar", max compression
```

## Comparing `datapipe_core-0.13.0a7.tar` & `datapipe_core-0.13.0a8.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a7/LICENSE
--rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0a7/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a7/datapipe/__init__.py
--rw-r--r--   0        0        0    18038 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/cli.py
--rw-r--r--   0        0        0     9520 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/compute.py
--rw-r--r--   0        0        0    37412 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/core_steps.py
--rw-r--r--   0        0        0     6780 2023-07-30 16:03:27.685421 datapipe_core-0.13.0a7/datapipe/datatable.py
--rw-r--r--   0        0        0     4649 2023-07-30 16:03:31.215421 datapipe_core-0.13.0a7/datapipe/event_logger.py
--rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/executor/__init__.py
--rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/executor/ray.py
--rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/lints.py
--rw-r--r--   0        0        0    22222 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/datapipe/metastore.py
--rw-r--r--   0        0        0      969 2023-07-30 16:08:00.215417 datapipe_core-0.13.0a7/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a7/datapipe/store/__init__.py
--rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/database.py
--rw-r--r--   0        0        0    18238 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/pandas.py
--rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/qdrant.py
--rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a7/datapipe/store/redis.py
--rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a7/datapipe/store/table_store.py
--rw-r--r--   0        0        0     9945 2023-07-30 16:08:03.355417 datapipe_core-0.13.0a7/datapipe/types.py
--rw-r--r--   0        0        0     2145 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a7/pyproject.toml
--rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a8/LICENSE
+-rw-r--r--   0        0        0      779 2023-07-30 16:02:08.285417 datapipe_core-0.13.0a8/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.13.0a8/datapipe/__init__.py
+-rw-r--r--   0        0        0    16161 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/cli.py
+-rw-r--r--   0        0        0     9520 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/compute.py
+-rw-r--r--   0        0        0    37565 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/core_steps.py
+-rw-r--r--   0        0        0     6780 2023-07-30 16:03:27.685421 datapipe_core-0.13.0a8/datapipe/datatable.py
+-rw-r--r--   0        0        0     4649 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/event_logger.py
+-rw-r--r--   0        0        0     1628 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/executor/__init__.py
+-rw-r--r--   0        0        0     2183 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/executor/ray.py
+-rw-r--r--   0        0        0     4236 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/lints.py
+-rw-r--r--   0        0        0    22222 2023-07-30 17:16:08.720825 datapipe_core-0.13.0a8/datapipe/metastore.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/migrations/__init__.py
+-rw-r--r--   0        0        0     3071 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/datapipe/migrations/v013.py
+-rw-r--r--   0        0        0      969 2023-07-30 16:08:00.215417 datapipe_core-0.13.0a8/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.13.0a8/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     8435 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/database.py
+-rw-r--r--   0        0        0    18238 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8674 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3209 2023-07-30 16:02:08.295417 datapipe_core-0.13.0a8/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.13.0a8/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     9945 2023-07-30 16:08:03.355417 datapipe_core-0.13.0a8/datapipe/types.py
+-rw-r--r--   0        0        0     2145 2023-07-31 17:04:18.495884 datapipe_core-0.13.0a8/pyproject.toml
+-rw-r--r--   0        0        0     3008 1970-01-01 00:00:00.000000 datapipe_core-0.13.0a8/PKG-INFO
```

### Comparing `datapipe_core-0.13.0a7/LICENSE` & `datapipe_core-0.13.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/README.md` & `datapipe_core-0.13.0a8/README.md`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/cli.py` & `datapipe_core-0.13.0a8/datapipe/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 import rich
 from opentelemetry import trace
 from opentelemetry.instrumentation.sqlalchemy import SQLAlchemyInstrumentor
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 from rich import print as rprint
-from sqlalchemy import insert, literal
-from sqlalchemy.sql import and_, func, select
 from tqdm_loggable.auto import tqdm
 
 from datapipe.compute import ComputeStep, DatapipeApp, run_steps, run_steps_changelist
 from datapipe.core_steps import BaseBatchTransformStep
 from datapipe.executor import Executor, SingleThreadExecutor
-from datapipe.types import ChangeList, IndexDF, Labels
+from datapipe.migrations import v013 as migrations_v013
+from datapipe.types import IndexDF, Labels
 
 tracer = trace.get_tracer("datapipe_app")
 
 rich.reconfigure(highlight=False)
 
 
 def load_pipeline(pipeline_name: str) -> DatapipeApp:
@@ -171,15 +170,15 @@
 
         cloud_trace_exporter = CloudTraceSpanExporter(
             resource_regex=r".*",
         )
         trace.get_tracer_provider().add_span_processor(BatchSpanProcessor(cloud_trace_exporter))  # type: ignore
 
     if executor == "SingleThreadExecutor":
-        ctx.obj["executor"] = SingleThreadExecutor
+        ctx.obj["executor"] = SingleThreadExecutor()
     elif executor == "RayExecutor":
         import ray
 
         from datapipe.executor.ray import RayExecutor
 
         ray_ctx = ray.init()
 
@@ -505,63 +504,16 @@
 @click.option("--labels", type=click.STRING, default="")
 def migrate_transform_tables(ctx: click.Context, labels: str, name: str) -> None:
     app: DatapipeApp = ctx.obj["pipeline"]
     labels_dict = parse_labels(labels)
     batch_transforms_steps = filter_steps_by_labels_and_name(
         app, labels=labels_dict, name_prefix=name
     )
-    for batch_transform in batch_transforms_steps:
-        if not isinstance(batch_transform, BaseBatchTransformStep):
-            continue
-        print(f"Checking '{batch_transform.get_name()}': ")
-        size = batch_transform.meta_table.get_metadata_size()
-        if size > 0:
-            print(f"Skipping -- size of metadata is greater 0: {size=}")
-            continue
-        if app.ds.meta_dbconn.con.driver in ("sqlite", "pysqlite"):
-            greatest_func = func.max
-        else:
-            greatest_func = func.greatest
-        output_tbls = [
-            output_dt.meta_table.sql_table for output_dt in batch_transform.output_dts
-        ]
-        sql = (
-            select(
-                *[output_tbls[0].c[k] for k in batch_transform.transform_keys],
-                greatest_func(*[tbl.c["process_ts"] for tbl in output_tbls]).label(
-                    "process_ts"
-                ),
-            )
-            .distinct()
-            .select_from(output_tbls[0])
-            .where(and_(*[tbl.c.delete_ts.is_(None) for tbl in output_tbls]))
-        )
-        prev_tbl = output_tbls[0]
-        for tbl in output_tbls[1:]:
-            sql = sql.outerjoin(
-                tbl,
-                and_(
-                    *[prev_tbl.c[k] == tbl.c[k] for k in batch_transform.transform_keys]
-                ),
-                full=True,
-            )
-            prev_tbl = tbl
-        insert_stmt = insert(batch_transform.meta_table.sql_table).from_select(
-            batch_transform.transform_keys
-            + ["process_ts", "is_success", "error", "priority"],
-            select(
-                *[sql.c[k] for k in batch_transform.transform_keys],
-                sql.c["process_ts"],
-                literal(True),
-                literal(None),
-                literal(0),
-            ),
-        )
-        app.ds.meta_dbconn.con.execute(insert_stmt)
-        rprint("  [green] ok[/green]")
+
+    return migrations_v013.migrate_transform_tables(app, batch_transforms_steps)
 
 
 for entry_point in metadata.entry_points().get("datapipe.cli", []):
     register_commands = entry_point.load()
     register_commands(cli)
```

### Comparing `datapipe_core-0.13.0a7/datapipe/compute.py` & `datapipe_core-0.13.0a8/datapipe/compute.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/core_steps.py` & `datapipe_core-0.13.0a8/datapipe/core_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1005,14 +1005,19 @@
     """
     Создание новой таблицы из результатов запуска `proc_func`.
     Функция может быть как обычной, так и генерирующейся
     """
 
     now = time.time()
     empty_generator = True
+    parameters = inspect.signature(func).parameters
+    kwargs = {
+        **({"ds": ds} if "ds" in parameters else {}),
+        **(kwargs or {}),
+    }
 
     assert inspect.isgeneratorfunction(
         func
     ), "Starting v0.8.0 proc_func should be a generator"
 
     with tracer.start_as_current_span("init generator"):
         try:
```

### Comparing `datapipe_core-0.13.0a7/datapipe/datatable.py` & `datapipe_core-0.13.0a8/datapipe/datatable.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/event_logger.py` & `datapipe_core-0.13.0a8/datapipe/event_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,23 +96,23 @@
         type,
         message,
         description,
         params,
         run_config: Optional[RunConfig] = None,
     ) -> None:
         if run_config is not None:
-            logger.debug(
+            logger.error(
                 f'Error in step {run_config.labels.get("step_name")}: {type} {message}\n{description}'
             )
             meta = {
                 "labels": run_config.labels,
                 "filters": run_config.filters,
             }
         else:
-            logger.debug(f"Error: {type} {message}\n{description}")
+            logger.error(f"Error: {type} {message}\n{description}")
             meta = {}
 
         ins = self.events_table.insert().values(
             type=EventTypes.ERROR.value,
             event={
                 "meta": meta,
                 "data": {
```

### Comparing `datapipe_core-0.13.0a7/datapipe/executor/__init__.py` & `datapipe_core-0.13.0a8/datapipe/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/executor/ray.py` & `datapipe_core-0.13.0a8/datapipe/executor/ray.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/lints.py` & `datapipe_core-0.13.0a8/datapipe/lints.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/metastore.py` & `datapipe_core-0.13.0a8/datapipe/metastore.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/run_config.py` & `datapipe_core-0.13.0a8/datapipe/run_config.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/database.py` & `datapipe_core-0.13.0a8/datapipe/store/database.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/filedir.py` & `datapipe_core-0.13.0a8/datapipe/store/filedir.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/milvus.py` & `datapipe_core-0.13.0a8/datapipe/store/milvus.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/pandas.py` & `datapipe_core-0.13.0a8/datapipe/store/pandas.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/qdrant.py` & `datapipe_core-0.13.0a8/datapipe/store/qdrant.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/redis.py` & `datapipe_core-0.13.0a8/datapipe/store/redis.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/store/table_store.py` & `datapipe_core-0.13.0a8/datapipe/store/table_store.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/datapipe/types.py` & `datapipe_core-0.13.0a8/datapipe/types.py`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.13.0a7/pyproject.toml` & `datapipe_core-0.13.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.13.0-alpha.7"
+version = "0.13.0-alpha.8"
 description = "`datapipe` is a realtime incremental ETL library for Python application"
 readme = "README.md"
 repository = "https://github.com/epoch8/datapipe"
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
```

### Comparing `datapipe_core-0.13.0a7/PKG-INFO` & `datapipe_core-0.13.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.13.0a7
+Version: 0.13.0a8
 Summary: `datapipe` is a realtime incremental ETL library for Python application
 Home-page: https://github.com/epoch8/datapipe
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

