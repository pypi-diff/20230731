# Comparing `tmp/serra-0.3.tar.gz` & `tmp/serra-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.3.tar", last modified: Fri Jul 28 19:54:00 2023, max compression
+gzip compressed data, was "serra-0.4.tar", last modified: Mon Jul 31 00:03:11 2023, max compression
```

## Comparing `serra-0.3.tar` & `serra-0.4.tar`

### file list

```diff
@@ -1,58 +1,60 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.697853 serra-0.3/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-21 18:21:51.000000 serra-0.3/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:54:00.697715 serra-0.3/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     1511 2023-07-28 19:53:46.000000 serra-0.3/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.693059 serra-0.3/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.3/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1315 2023-07-28 19:53:46.000000 serra-0.3/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1501 2023-07-28 01:15:14.000000 serra-0.3/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-28 19:53:46.000000 serra-0.3/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1883 2023-07-28 19:53:46.000000 serra-0.3/serra/config_parser.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2963 2023-07-28 19:53:46.000000 serra-0.3/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-27 07:28:06.000000 serra-0.3/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1025 2023-07-28 19:53:46.000000 serra-0.3/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.695026 serra-0.3/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      185 2023-07-21 18:21:51.000000 serra-0.3/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1456 2023-07-28 01:15:14.000000 serra-0.3/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      487 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-27 07:28:06.000000 serra-0.3/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-21 18:21:51.000000 serra-0.3/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2975 2023-07-28 19:53:46.000000 serra-0.3/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.695325 serra-0.3/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-21 18:21:51.000000 serra-0.3/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.3/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3183 2023-07-28 19:53:46.000000 serra-0.3/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      442 2023-07-28 01:15:14.000000 serra-0.3/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.696839 serra-0.3/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-25 20:52:34.000000 serra-0.3/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-28 19:53:46.000000 serra-0.3/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1385 2023-07-28 19:53:46.000000 serra-0.3/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1820 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1090 2023-07-27 07:28:06.000000 serra-0.3/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-21 18:21:51.000000 serra-0.3/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1189 2023-07-28 19:53:46.000000 serra-0.3/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1239 2023-07-28 01:15:14.000000 serra-0.3/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.697518 serra-0.3/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      186 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-28 01:15:14.000000 serra-0.3/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      677 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-27 07:28:06.000000 serra-0.3/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      568 2023-07-21 18:21:51.000000 serra-0.3/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-27 07:28:06.000000 serra-0.3/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-28 19:54:00.694301 serra-0.3/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     1374 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-21 20:20:18.000000 serra-0.3/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       62 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-28 19:54:00.000000 serra-0.3/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-28 19:54:00.697895 serra-0.3/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      649 2023-07-28 19:53:57.000000 serra-0.3/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.998029 serra-0.4/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-31 00:01:40.000000 serra-0.4/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-31 00:03:11.997881 serra-0.4/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3846 2023-07-31 00:01:40.000000 serra-0.4/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.992487 serra-0.4/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 00:01:40.000000 serra-0.4/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2033 2023-07-31 00:01:40.000000 serra-0.4/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1859 2023-07-31 00:01:40.000000 serra-0.4/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-31 00:01:40.000000 serra-0.4/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1883 2023-07-31 00:01:40.000000 serra-0.4/serra/config_parser.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2963 2023-07-31 00:01:40.000000 serra-0.4/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-31 00:01:40.000000 serra-0.4/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1121 2023-07-31 00:01:40.000000 serra-0.4/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.994406 serra-0.4/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1456 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      487 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1378 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2975 2023-07-31 00:01:40.000000 serra-0.4/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.994770 serra-0.4/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3180 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      442 2023-07-31 00:01:40.000000 serra-0.4/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.996656 serra-0.4/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1385 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1820 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1090 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2005 2023-07-31 00:01:40.000000 serra-0.4/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2292 2023-07-31 00:01:40.000000 serra-0.4/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.997647 serra-0.4/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      677 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      568 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3047 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.993494 serra-0.4/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     1443 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 00:02:07.000000 serra-0.4/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       62 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 00:03:11.998119 serra-0.4/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      649 2023-07-31 00:03:01.000000 serra-0.4/setup.py
```

### Comparing `serra-0.3/LICENSE.md` & `serra-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/cli.py` & `serra-0.4/serra/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Entry point for serra command line tool
 import sys
 import click
 from serra.run import run_job_from_job_dir, update_package, create_job_yaml, run_job_from_aws, translate_job
 from serra.databricks import create_job
 from serra.utils import validate_workspace
+from serra.config import PACKAGE_PATH
+from serra.utils import copy_folder
 
 @click.group()
 def main():
     pass
 
 @main.command(name="start")
 @click.argument("job_name")
@@ -36,14 +38,21 @@
 @click.argument("job_name")
 def cli_create_job(job_name):
     """Create a databricks job
     """
     validate_workspace()
     create_job(job_name)
 
+@main.command(name="create")
+@click.argument("local_path", type=click.Path(), default=".")
+def cli_create(local_path):
+    """Copy workspace_example folder from S3 to local_path"""
+    source_folder = f"{PACKAGE_PATH}/../workspace_example"
+    copy_folder(source_folder, local_path)
+
 @main.command(name="update_package")
 def cli_update_package():
     """Uploads package to aws, and restarts databricks cluster
     """
     update_package()
     
 # only for use by databricks cluster
```

### Comparing `serra-0.3/serra/config_parser.py` & `serra-0.4/serra/config_parser.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/databricks.py` & `serra-0.4/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/profile.py` & `serra-0.4/serra/profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,11 +31,15 @@
     @property
     def databricks_token(self):
         return self.config.get("DATABRICKS_TOKEN")
     
     @property
     def databricks_cluster_id(self):
         return self.config.get("DATABRICKS_CLUSTER_ID")
+    
+    @property
+    def snowflake_account(self):
+        return self.config.get("SNOWFLAKE")
 
 def get_serra_profile():
     serra_profile = SerraProfile.from_yaml_path("./profiles.yml")
     return serra_profile
```

### Comparing `serra-0.3/serra/readers/amazon_reader.py` & `serra-0.4/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/readers/databricks_reader.py` & `serra-0.4/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/run.py` & `serra-0.4/serra/run.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/runners/ExecutionGraph.py` & `serra-0.4/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/runners/graph_runner.py` & `serra-0.4/serra/runners/graph_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 
         if is_reader(block_name, cf):
             df = block_obj.read()
             df_map[block_name] = df
         elif is_writer(block_name, cf):
             assert len(block_obj.dependencies) == 1
             dependency = block_obj.dependencies[0]
-            df_map[dependency].show()
             block_obj.write(df_map[dependency]) # Get the 
         elif is_Transformer(block_name, cf):
             assert len(block_obj.dependencies) >= 1
             input_dfs = [df_map[dep] for dep in block_obj.dependencies]
             df = block_obj.transform(*input_dfs)
             df_map[block_name] = df
 
@@ -74,11 +73,13 @@
                 logger.info(f"\tRunning test {test_name}")
                 if test_name == 'nulls':
                     df = df_map[block_name]
                     nulls_test(df)
                 if test_name == 'duplicates':
                     df = df_map[block_name]
                     duplicates_test(df)
+    
+    df_map[dependency].show()
 
     if cf.get_test():
         logger.info("Debug is true—printing out rows.")
         df.show(500)
```

### Comparing `serra-0.3/serra/transformers/__init__.py` & `serra-0.4/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/add_column_transformer.py` & `serra-0.4/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/case_when_transformer.py` & `serra-0.4/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/drop_columns_transformer.py` & `serra-0.4/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/get_count_transformer.py` & `serra-0.4/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/join_transformer.py` & `serra-0.4/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/map_transformer.py` & `serra-0.4/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/pivot_transformer.py` & `serra-0.4/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/rename_column_transformer.py` & `serra-0.4/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/transformers/select_transformer.py` & `serra-0.4/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/writers/amazon_writer.py` & `serra-0.4/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/writers/databricks_writer.py` & `serra-0.4/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra/writers/s3_writer.py` & `serra-0.4/serra/writers/s3_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.3/serra.egg-info/SOURCES.txt` & `serra-0.4/serra.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 serra.egg-info/top_level.txt
 serra/readers/__init__.py
 serra/readers/amazon_reader.py
 serra/readers/databricks_reader.py
 serra/readers/local_reader.py
 serra/readers/reader.py
 serra/readers/s3_reader.py
+serra/readers/snowflaker_reader.py
 serra/runners/ExecutionGraph.py
 serra/runners/__init__.py
 serra/runners/graph_runner.py
 serra/transformers/__init__.py
 serra/transformers/add_column_transformer.py
 serra/transformers/case_when_transformer.py
 serra/transformers/cast_columns_transformer.py
@@ -42,8 +43,9 @@
 serra/transformers/select_transformer.py
 serra/transformers/transformer.py
 serra/writers/__init__.py
 serra/writers/amazon_writer.py
 serra/writers/databricks_writer.py
 serra/writers/local_writer.py
 serra/writers/s3_writer.py
+serra/writers/snowflake_writer.py
 serra/writers/writer.py
```

### Comparing `serra-0.3/setup.py` & `serra-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.3',
+      version='0.4',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Alan Wang',
       author_email='alan@serra.io',
       license='tbd',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/*.yml"]},
```

