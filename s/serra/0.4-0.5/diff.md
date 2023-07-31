# Comparing `tmp/serra-0.4.tar.gz` & `tmp/serra-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.4.tar", last modified: Mon Jul 31 00:03:11 2023, max compression
+gzip compressed data, was "serra-0.5.tar", last modified: Mon Jul 31 04:19:41 2023, max compression
```

## Comparing `serra-0.4.tar` & `serra-0.5.tar`

### file list

```diff
@@ -1,60 +1,105 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.998029 serra-0.4/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-31 00:01:40.000000 serra-0.4/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-31 00:03:11.997881 serra-0.4/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3846 2023-07-31 00:01:40.000000 serra-0.4/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.992487 serra-0.4/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 00:01:40.000000 serra-0.4/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2033 2023-07-31 00:01:40.000000 serra-0.4/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1859 2023-07-31 00:01:40.000000 serra-0.4/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-31 00:01:40.000000 serra-0.4/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1883 2023-07-31 00:01:40.000000 serra-0.4/serra/config_parser.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2963 2023-07-31 00:01:40.000000 serra-0.4/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-31 00:01:40.000000 serra-0.4/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1121 2023-07-31 00:01:40.000000 serra-0.4/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.994406 serra-0.4/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1456 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      487 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1378 2023-07-31 00:01:40.000000 serra-0.4/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2975 2023-07-31 00:01:40.000000 serra-0.4/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.994770 serra-0.4/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3180 2023-07-31 00:01:40.000000 serra-0.4/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      442 2023-07-31 00:01:40.000000 serra-0.4/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.996656 serra-0.4/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1385 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1820 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1090 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-31 00:01:40.000000 serra-0.4/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2005 2023-07-31 00:01:40.000000 serra-0.4/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2292 2023-07-31 00:01:40.000000 serra-0.4/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.997647 serra-0.4/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      677 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      568 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3047 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-31 00:01:40.000000 serra-0.4/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 00:03:11.993494 serra-0.4/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      223 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     1443 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 00:02:07.000000 serra-0.4/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       62 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 00:03:11.000000 serra-0.4/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 00:03:11.998119 serra-0.4/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      649 2023-07-31 00:03:01.000000 serra-0.4/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.057837 serra-0.5/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-21 18:21:51.000000 serra-0.5/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      195 2023-07-31 04:19:41.057663 serra-0.5/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3852 2023-07-31 04:19:00.000000 serra-0.5/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.039728 serra-0.5/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.5/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-07-31 04:18:53.000000 serra-0.5/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1862 2023-07-31 04:18:53.000000 serra-0.5/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-28 19:53:46.000000 serra-0.5/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1782 2023-07-31 04:18:53.000000 serra-0.5/serra/config_parser.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.035488 serra-0.5/serra/data/
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.041330 serra-0.5/serra/data/autocomplete/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/README.md
+-rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.041509 serra-0.5/serra/data/autocomplete/inputs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.045511 serra-0.5/serra/data/autocomplete/output/
+-rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.046001 serra-0.5/serra/data/autocomplete/templates/
+-rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.046461 serra-0.5/serra/data/workspace_example/
+-rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.047141 serra-0.5/serra/data/workspace_example/examples/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.048496 serra-0.5/serra/data/workspace_example/jobs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1984 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      415 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      224 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.048982 serra-0.5/serra/data/workspace_example/sql/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-07-31 04:18:53.000000 serra-0.5/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-27 07:28:06.000000 serra-0.5/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-07-31 04:18:53.000000 serra-0.5/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.051236 serra-0.5/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-30 22:45:03.000000 serra-0.5/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-27 07:28:06.000000 serra-0.5/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-27 07:28:06.000000 serra-0.5/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-21 18:21:51.000000 serra-0.5/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-07-31 04:18:53.000000 serra-0.5/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.051799 serra-0.5/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-21 18:21:51.000000 serra-0.5/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.5/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3181 2023-07-31 04:18:53.000000 serra-0.5/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-07-31 04:18:53.000000 serra-0.5/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.055208 serra-0.5/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-25 20:52:34.000000 serra-0.5/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-27 07:28:06.000000 serra-0.5/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 04:18:48.000000 serra-0.5/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1808 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-27 07:28:06.000000 serra-0.5/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-07-31 04:18:53.000000 serra-0.5/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-07-31 04:18:53.000000 serra-0.5/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.057308 serra-0.5/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-30 22:44:29.000000 serra-0.5/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-27 07:28:06.000000 serra-0.5/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-27 07:28:06.000000 serra-0.5/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.040989 serra-0.5/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      195 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3277 2023-07-31 04:19:41.000000 serra-0.5/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       87 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-21 20:20:18.000000 serra-0.5/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 04:19:41.057882 serra-0.5/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-07-31 04:19:39.000000 serra-0.5/setup.py
```

### Comparing `serra-0.4/LICENSE.md` & `serra-0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.4/README.md` & `serra-0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Project Header](serra.png)
+![Project Header](./etc/serra.png)
 
 Translate SQL to Object-Oriented Spark
 
 ## What is Serra?
 Developers can retool long-winded SQL scripts into simple, object-oriented Spark code with one command `serra translate`. 
 
 Serra is an end-to-end, ETL framework that simplifies complex SQL scripts to a few lines of PySpark code with transformer and in-house connector objects.
@@ -13,15 +13,15 @@
 
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install Serra.
 
 ```bash
-pip install serra==0.3
+pip install serra==0.5
 ```
 
 # Setup
 
 Setup your virtual environment below.
 
 ```bash
```

### Comparing `serra-0.4/serra/aws.py` & `serra-0.5/serra/aws.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import boto3
+import os
 import json
+
+import boto3
+
 from serra.profile import get_serra_profile
-import os
-import botocore
-from serra.config import PACKAGE_PATH
 
 def get_s3_client():
     user_profile = get_serra_profile()
     s3 = boto3.resource('s3',
             aws_access_key_id=user_profile.aws_access_key_id,
             aws_secret_access_key=user_profile.aws_secret_access_key)
     return s3
@@ -36,14 +36,15 @@
 def read_json_s3(file, bucket):
     s3 = get_s3_client()
     content_object = s3.Object(bucket, f'{file}.json')
     file_content = content_object.get()['Body'].read().decode('utf-8')
     return json.loads(file_content)
 
 def write_json_s3(obj, file, bucket):
+    s3 = get_s3_client()
     json_dump_s3 = lambda obj, f: s3.Object(bucket, key=f).put(Body=json.dumps(obj))
     json_dump_s3(obj, f'{file}.json')
 
 def copy_folder_to_s3(local_folder_path, bucket_name, s3_folder_key):
     """Copy a local folder and its contents to an S3 bucket."""
     s3_client = boto3.client("s3")
```

### Comparing `serra-0.4/serra/cli.py` & `serra-0.5/serra/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Entry point for serra command line tool
 import sys
 import click
+
 from serra.run import run_job_from_job_dir, update_package, create_job_yaml, run_job_from_aws, translate_job
 from serra.databricks import create_job
 from serra.utils import validate_workspace
 from serra.config import PACKAGE_PATH
 from serra.utils import copy_folder
 
 @click.group()
@@ -42,15 +43,15 @@
     validate_workspace()
     create_job(job_name)
 
 @main.command(name="create")
 @click.argument("local_path", type=click.Path(), default=".")
 def cli_create(local_path):
     """Copy workspace_example folder from S3 to local_path"""
-    source_folder = f"{PACKAGE_PATH}/../workspace_example"
+    source_folder = f"{PACKAGE_PATH}/data/workspace_example"
     copy_folder(source_folder, local_path)
 
 @main.command(name="update_package")
 def cli_update_package():
     """Uploads package to aws, and restarts databricks cluster
     """
     update_package()
```

### Comparing `serra-0.4/serra/config_parser.py` & `serra-0.5/serra/config_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# In case we ever want to change use of yaml file
 import yaml
-from serra.aws import retrieve_file_from_config_bucket
 
+from serra.aws import retrieve_file_from_config_bucket
 
 def convert_name_to_full(class_name):
     if "Reader" in class_name:
         return f"serra.readers.{class_name}"
     elif "Writer" in class_name:
         return f"serra.writers.{class_name}"
     else:
@@ -53,10 +52,7 @@
         return self.config.get(block_name).get(class_name)
     
     def get_tests_for_block(self, block_name):
         return self.config.get(block_name).get("tests")
     
     def get_test(self):
         return self.config.get('debug')
-
-if __name__=="__main__":
-    cp = ConfigParser("")
```

### Comparing `serra-0.4/serra/databricks.py` & `serra-0.5/serra/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Module to help connect to databricks
 from loguru import logger
 from databricks.sdk import WorkspaceClient
 from databricks.sdk.service.jobs import Task, PythonWheelTask
 from databricks.sdk.service.compute import Library, State
+
 from serra.aws import upload_file_to_config_bucket
 from serra.utils import get_path_to_user_configs_folder
 from serra.profile import get_serra_profile
 from serra.config import (
     WHEEL_FILE_NAME_IN_BUCKET,
     LOCAL_PATH_TO_WHEEL
 )
```

### Comparing `serra-0.4/serra/profile.py` & `serra-0.5/serra/profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import yaml
 
 class SerraProfile:
 
     def __init__(self, config):
         self.config = config
```

### Comparing `serra-0.4/serra/readers/amazon_reader.py` & `serra-0.5/serra/readers/amazon_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import boto3
 import pandas as pd
+
 from serra.utils import get_or_create_spark_session
 from serra.profile import get_serra_profile
 
 class AmazonS3Reader():
     def __init__(self, config):
         self.config = config
         self.serra_profile = get_serra_profile()
```

### Comparing `serra-0.4/serra/readers/databricks_reader.py` & `serra-0.5/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/readers/snowflaker_reader.py` & `serra-0.5/serra/readers/snowflaker_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import pandas as pd
 import snowflake.connector
+
 from serra.profile import get_serra_profile
 from serra.utils import get_or_create_spark_session
-import pandas as pd
+
 
 class SnowflakeReader():
     def __init__(self, config):
         self.config = config
         self.snowflake_account = get_serra_profile().snowflake_account
     
     @property
```

### Comparing `serra-0.4/serra/run.py` & `serra-0.5/serra/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Running a specific job
+import os
 import sys
 from sys import exit
-import os
-from serra.config_parser import ConfigParser
-from serra.utils import get_path_to_user_configs_folder, write_to_file
 from os.path import exists
+
 from loguru import logger
+
+from serra.config_parser import ConfigParser
+from serra.utils import get_path_to_user_configs_folder, write_to_file
 from serra.databricks import upload_wheel_to_bucket, restart_server
 from serra.runners.graph_runner import run_job_with_graph
 from serra.exceptions import SerraRunException
 from serra.translate_client import save_as_yaml, get_translated_yaml
 
 PACKAGE_PATH = os.path.dirname(os.path.dirname(__file__))
```

### Comparing `serra-0.4/serra/runners/ExecutionGraph.py` & `serra-0.5/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/runners/graph_runner.py` & `serra-0.5/serra/runners/graph_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from loguru import logger
+
 from serra.config_parser import ConfigParser, convert_name_to_full
 from serra.utils import import_class
 from serra.tests import duplicates_test, nulls_test
-from loguru import logger
 from serra.runners.ExecutionGraph import BlockGraph
 
 
 # Returns instatiated reader,writer,transformer class with config already passed in
 def get_configured_block_object(block_name, cf: ConfigParser):
     config = cf.get_config_for_block(block_name)
     class_name = cf.get_class_name_for_step(block_name)
```

### Comparing `serra-0.4/serra/transformers/__init__.py` & `serra-0.5/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/add_column_transformer.py` & `serra-0.5/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/case_when_transformer.py` & `serra-0.5/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/drop_columns_transformer.py` & `serra-0.5/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/get_count_transformer.py` & `serra-0.5/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/join_transformer.py` & `serra-0.5/serra/transformers/join_transformer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from pyspark.sql import functions as F
+
 from serra.exceptions import SerraRunException
 from serra.transformers.transformer import Transformer
-from serra.readers.s3_reader import S3Reader
-import logging
-
-logger = logging.getLogger(__name__)
 
 class JoinTransformer(Transformer):
     """
     Join tables together
     :param join_type: Type of join
     :param df1, df2: dataframes
     :param matching_col: column to join on
```

### Comparing `serra-0.4/serra/transformers/map_transformer.py` & `serra-0.5/serra/transformers/map_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pyspark.sql import functions as F
 
 from serra.transformers.transformer import Transformer
 from serra.exceptions import SerraRunException
-import json
 
 class MapTransformer(Transformer):
     """
     Test transformer to add a column to dataframe
     :param config: Holds column value
     """
```

### Comparing `serra-0.4/serra/transformers/pivot_transformer.py` & `serra-0.5/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/rename_column_transformer.py` & `serra-0.5/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.4/serra/transformers/select_transformer.py` & `serra-0.5/serra/transformers/select_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyspark.sql import DataFrame
 from pyspark.sql import functions as F
+
 from serra.transformers.transformer import Transformer
 from serra.exceptions import SerraRunException
 
 class SelectTransformer(Transformer):
     """
     Transformer to perform a SELECT operation on a DataFrame.
     :param config: Holds the list of columns to select from the DataFrame.
```

### Comparing `serra-0.4/serra/translate_client.py` & `serra-0.5/serra/translate_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import requests
+import time
+
 import yaml
 from loguru import logger
+
 from serra.config import TRANSLATE_URL
-import time
 
 def send_post_request(file_path, url):
     with open(file_path, 'r') as file:
         # Send the POST request with the file
         data = file.read()
         response = requests.post(url, data=data)
         return response
@@ -24,15 +26,15 @@
             with open(file_path, 'w') as file:
                 yaml.dump(yaml_content, file)
             logger.info(f"Content saved as YAML file: {os.path.abspath(file_path)}")
         except Exception as e:
             logger.info(f"Error saving content as YAML file: {str(e)}")
 
 def get_translated_yaml(file_path):
-    url = "https://serra-translate-59cfd3dacac9.herokuapp.com/"
+    url = TRANSLATE_URL
     create_job_url = url + "start_job"
     check_job_status_url = url + "get_job_status"
     get_job_result_url = url + "get_job_result"
 
     # Create the job
     job_id_response = send_post_request(file_path,create_job_url)
     if job_id_response.status_code != 200:
```

### Comparing `serra-0.4/serra/utils.py` & `serra-0.5/serra/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import os
+import shutil
+
 from pyspark.sql import SparkSession
 from os.path import exists
 from loguru import logger
-import os
-import shutil
 
 def write_to_file(filename, content):
     try:
         with open(filename, 'w') as file:
             file.write(content)
         logger.info(f"Successfully wrote to {filename}.")
     except IOError:
```

### Comparing `serra-0.4/serra/writers/amazon_writer.py` & `serra-0.5/serra/writers/amazon_writer.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import boto3
-from serra.profile import get_serra_profile
 
+from serra.profile import get_serra_profile
 
 class AmazonS3Writer():
     def __init__(self, config):
         self.config = config
         self.serra_profile = get_serra_profile()
     
     @property
```

### Comparing `serra-0.4/serra/writers/databricks_writer.py` & `serra-0.5/serra/writers/databricks_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from pyspark.sql import DataFrame
+
 from serra.writers import Writer
 from serra.utils import get_or_create_spark_session
-from pyspark.sql import DataFrame
 
 class DatabricksWriter(Writer):
     def __init__(self, config):
         self.spark = get_or_create_spark_session()
         self.config = config
         self.database = self.config.get('database')
         self.table = self.config.get('table')
```

### Comparing `serra-0.4/serra/writers/s3_writer.py` & `serra-0.5/serra/writers/s3_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from pyspark.sql import DataFrame
+
 from serra.writers import Writer
 from serra.utils import get_or_create_spark_session
-from pyspark.sql import DataFrame
 
 class S3Writer(Writer):
     def __init__(self, config):
         self.spark = get_or_create_spark_session()
         self.config = config
         self.path = self.config.get('path')
         self.format = self.config.get('format')
```

### Comparing `serra-0.4/serra/writers/snowflake_writer.py` & `serra-0.5/serra/writers/snowflake_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import snowflake.connector
-from serra.profile import get_serra_profile
 from loguru import logger
+
+from serra.profile import get_serra_profile
 from serra.exceptions import SerraRunException
 
 class SnowflakeWriter():
     def __init__(self, config):
         self.config = config
         self.type = self.config.get('type')
         self.snowflake_account = get_serra_profile().snowflake_account
```

