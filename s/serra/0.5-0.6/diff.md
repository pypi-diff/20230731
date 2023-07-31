# Comparing `tmp/serra-0.5.tar.gz` & `tmp/serra-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serra-0.5.tar", last modified: Mon Jul 31 04:19:41 2023, max compression
+gzip compressed data, was "serra-0.6.tar", last modified: Mon Jul 31 04:59:18 2023, max compression
```

## Comparing `serra-0.5.tar` & `serra-0.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.057837 serra-0.5/
--rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-21 18:21:51.000000 serra-0.5/LICENSE.md
--rw-r--r--   0 alanwang   (501) staff       (20)      195 2023-07-31 04:19:41.057663 serra-0.5/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3852 2023-07-31 04:19:00.000000 serra-0.5/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.039728 serra-0.5/serra/
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.5/serra/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-07-31 04:18:53.000000 serra-0.5/serra/aws.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1862 2023-07-31 04:18:53.000000 serra-0.5/serra/cli.py
--rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-28 19:53:46.000000 serra-0.5/serra/config.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1782 2023-07-31 04:18:53.000000 serra-0.5/serra/config_parser.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.035488 serra-0.5/serra/data/
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.041330 serra-0.5/serra/data/autocomplete/
--rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/README.md
--rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/gen_schemas.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.041509 serra-0.5/serra/data/autocomplete/inputs/
--rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/inputs/specs.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.045511 serra-0.5/serra/data/autocomplete/output/
--rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AddColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AmazonS3Reader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/AmazonS3Writer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/CaseWhenTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/CastColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DatabricksReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DatabricksWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/DropColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/GetCountTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/JoinTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/LocalReader.json
--rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/LocalWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/MapTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/PivotTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/RenameColumnTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/SelectTransformer.json
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/SnowflakeWriter.json
--rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/output/serra_yaml_schema.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.046001 serra-0.5/serra/data/autocomplete/templates/
--rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/templates/schema_template.json
--rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-07-31 04:18:53.000000 serra-0.5/serra/data/autocomplete/templates/transformer_template.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.046461 serra-0.5/serra/data/workspace_example/
--rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/README.md
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.047141 serra-0.5/serra/data/workspace_example/examples/
--rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/ratings.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/sales.csv
--rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/examples/states_to_abbreviation.json
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.048496 serra-0.5/serra/data/workspace_example/jobs/
--rw-r--r--   0 alanwang   (501) staff       (20)     1984 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/Demo.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      415 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/LocalExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadExample.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadJoinWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadMapWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/jobs/ReadPivotWrite.yml
--rw-r--r--   0 alanwang   (501) staff       (20)      224 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/profiles.yml
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.048982 serra-0.5/serra/data/workspace_example/sql/
--rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/sql/easy_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-07-31 04:18:53.000000 serra-0.5/serra/data/workspace_example/sql/hard_demo.sql
--rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-07-31 04:18:53.000000 serra-0.5/serra/databricks.py
--rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-27 07:28:06.000000 serra-0.5/serra/exceptions.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-07-31 04:18:53.000000 serra-0.5/serra/profile.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.051236 serra-0.5/serra/readers/
--rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-30 22:45:03.000000 serra-0.5/serra/readers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/amazon_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-27 07:28:06.000000 serra-0.5/serra/readers/databricks_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/local_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-27 07:28:06.000000 serra-0.5/serra/readers/reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-21 18:21:51.000000 serra-0.5/serra/readers/s3_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-07-31 04:18:53.000000 serra-0.5/serra/readers/snowflaker_reader.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-07-31 04:18:53.000000 serra-0.5/serra/run.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.051799 serra-0.5/serra/runners/
--rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-21 18:21:51.000000 serra-0.5/serra/runners/ExecutionGraph.py
--rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-21 18:21:51.000000 serra-0.5/serra/runners/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3181 2023-07-31 04:18:53.000000 serra-0.5/serra/runners/graph_runner.py
--rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-07-31 04:18:53.000000 serra-0.5/serra/tests.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.055208 serra-0.5/serra/transformers/
--rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-25 20:52:34.000000 serra-0.5/serra/transformers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-27 07:28:06.000000 serra-0.5/serra/transformers/add_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/case_when_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 04:18:48.000000 serra-0.5/serra/transformers/cast_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/drop_columns_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/get_count_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/join_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1808 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/map_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-27 07:28:06.000000 serra-0.5/serra/transformers/pivot_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/rename_column_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-07-31 04:18:53.000000 serra-0.5/serra/transformers/select_transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-21 18:21:51.000000 serra-0.5/serra/transformers/transformer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-07-31 04:18:53.000000 serra-0.5/serra/translate_client.py
--rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-07-31 04:18:53.000000 serra-0.5/serra/utils.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.057308 serra-0.5/serra/writers/
--rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-30 22:44:29.000000 serra-0.5/serra/writers/__init__.py
--rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/amazon_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/databricks_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-27 07:28:06.000000 serra-0.5/serra/writers/local_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/s3_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-07-31 04:18:53.000000 serra-0.5/serra/writers/snowflake_writer.py
--rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-27 07:28:06.000000 serra-0.5/serra/writers/writer.py
-drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:19:41.040989 serra-0.5/serra.egg-info/
--rw-r--r--   0 alanwang   (501) staff       (20)      195 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/PKG-INFO
--rw-r--r--   0 alanwang   (501) staff       (20)     3277 2023-07-31 04:19:41.000000 serra-0.5/serra.egg-info/SOURCES.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/dependency_links.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       87 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/entry_points.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-21 20:20:18.000000 serra-0.5/serra.egg-info/not-zip-safe
--rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/requires.txt
--rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 04:19:40.000000 serra-0.5/serra.egg-info/top_level.txt
--rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 04:19:41.057882 serra-0.5/setup.cfg
--rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-07-31 04:19:39.000000 serra-0.5/setup.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.424116 serra-0.6/
+-rw-r--r--   0 alanwang   (501) staff       (20)     3860 2023-07-31 04:49:36.000000 serra-0.6/LICENSE.md
+-rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-07-31 04:59:18.423978 serra-0.6/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3852 2023-07-31 04:49:36.000000 serra-0.6/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.414281 serra-0.6/serra/
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 04:49:36.000000 serra-0.6/serra/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2006 2023-07-31 04:49:36.000000 serra-0.6/serra/aws.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1872 2023-07-31 04:49:36.000000 serra-0.6/serra/cli.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      222 2023-07-31 04:49:36.000000 serra-0.6/serra/config.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1782 2023-07-31 04:49:36.000000 serra-0.6/serra/config_parser.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.411594 serra-0.6/serra/data/
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415671 serra-0.6/serra/data/autocomplete/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1110 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/README.md
+-rw-r--r--   0 alanwang   (501) staff       (20)     1636 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/gen_schemas.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415783 serra-0.6/serra/data/autocomplete/inputs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2249 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/inputs/specs.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418356 serra-0.6/serra/data/autocomplete/output/
+-rw-r--r--   0 alanwang   (501) staff       (20)      391 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AddColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      276 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AmazonS3Reader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      341 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/AmazonS3Writer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      267 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/CaseWhenTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      216 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/CastColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      206 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DatabricksReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      389 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DatabricksWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/DropColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/GetCountTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      354 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/JoinTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      148 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/LocalReader.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      213 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/LocalWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      331 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/MapTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      408 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/PivotTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      274 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/RenameColumnTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      210 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/SelectTransformer.json
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/SnowflakeWriter.json
+-rw-r--r--   0 alanwang   (501) staff       (20)     7553 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/output/serra_yaml_schema.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418594 serra-0.6/serra/data/autocomplete/templates/
+-rw-r--r--   0 alanwang   (501) staff       (20)      326 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/templates/schema_template.json
+-rw-r--r--   0 alanwang   (501) staff       (20)       95 2023-07-31 04:49:36.000000 serra-0.6/serra/data/autocomplete/templates/transformer_template.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.418820 serra-0.6/serra/data/workspace_example/
+-rw-r--r--   0 alanwang   (501) staff       (20)      137 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/README.md
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.419206 serra-0.6/serra/data/workspace_example/examples/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1610 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/ratings.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     6706 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/sales.csv
+-rw-r--r--   0 alanwang   (501) staff       (20)     1124 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/examples/states_to_abbreviation.json
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.420030 serra-0.6/serra/data/workspace_example/jobs/
+-rw-r--r--   0 alanwang   (501) staff       (20)     1984 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/Demo.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      415 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/LocalExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      220 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadExample.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      456 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadJoinWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      393 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadMapWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      397 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/jobs/ReadPivotWrite.yml
+-rw-r--r--   0 alanwang   (501) staff       (20)      224 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/profiles.yml
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.420322 serra-0.6/serra/data/workspace_example/sql/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2603 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/sql/easy_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2909 2023-07-31 04:49:36.000000 serra-0.6/serra/data/workspace_example/sql/hard_demo.sql
+-rw-r--r--   0 alanwang   (501) staff       (20)     2964 2023-07-31 04:49:36.000000 serra-0.6/serra/databricks.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      106 2023-07-31 04:49:36.000000 serra-0.6/serra/exceptions.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1120 2023-07-31 04:49:36.000000 serra-0.6/serra/profile.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.421139 serra-0.6/serra/readers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      233 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1457 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/amazon_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      579 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/databricks_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      501 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/local_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      277 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      452 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/s3_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1380 2023-07-31 04:49:36.000000 serra-0.6/serra/readers/snowflaker_reader.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2977 2023-07-31 04:49:36.000000 serra-0.6/serra/run.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.421495 serra-0.6/serra/runners/
+-rw-r--r--   0 alanwang   (501) staff       (20)     2631 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/ExecutionGraph.py
+-rw-r--r--   0 alanwang   (501) staff       (20)        0 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3181 2023-07-31 04:49:36.000000 serra-0.6/serra/runners/graph_runner.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      443 2023-07-31 04:49:36.000000 serra-0.6/serra/tests.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.422957 serra-0.6/serra/transformers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      574 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      928 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/add_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      631 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/case_when_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      460 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/cast_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      601 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/drop_columns_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      637 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/get_count_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1288 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/join_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1808 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/map_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1178 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/pivot_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      700 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/rename_column_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1091 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/select_transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      310 2023-07-31 04:49:36.000000 serra-0.6/serra/transformers/transformer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1967 2023-07-31 04:49:36.000000 serra-0.6/serra/translate_client.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     2293 2023-07-31 04:49:36.000000 serra-0.6/serra/utils.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.423775 serra-0.6/serra/writers/
+-rw-r--r--   0 alanwang   (501) staff       (20)      232 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/__init__.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     1421 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/amazon_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      678 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/databricks_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      508 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/local_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      569 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/s3_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)     3048 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/snowflake_writer.py
+-rw-r--r--   0 alanwang   (501) staff       (20)      284 2023-07-31 04:49:36.000000 serra-0.6/serra/writers/writer.py
+drwxr-xr-x   0 alanwang   (501) staff       (20)        0 2023-07-31 04:59:18.415432 serra-0.6/serra.egg-info/
+-rw-r--r--   0 alanwang   (501) staff       (20)      240 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/PKG-INFO
+-rw-r--r--   0 alanwang   (501) staff       (20)     3277 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/SOURCES.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/dependency_links.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       88 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/entry_points.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        1 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/not-zip-safe
+-rw-r--r--   0 alanwang   (501) staff       (20)       83 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/requires.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)        6 2023-07-31 04:59:18.000000 serra-0.6/serra.egg-info/top_level.txt
+-rw-r--r--   0 alanwang   (501) staff       (20)       38 2023-07-31 04:59:18.424157 serra-0.6/setup.cfg
+-rw-r--r--   0 alanwang   (501) staff       (20)      918 2023-07-31 04:50:45.000000 serra-0.6/setup.py
```

### Comparing `serra-0.5/LICENSE.md` & `serra-0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `serra-0.5/README.md` & `serra-0.6/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/aws.py` & `serra-0.6/serra/aws.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/cli.py` & `serra-0.6/serra/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 def cli_create_job(job_name):
     """Create a databricks job
     """
     validate_workspace()
     create_job(job_name)
 
 @main.command(name="create")
-@click.argument("local_path", type=click.Path(), default=".")
+@click.argument("local_path", type=click.Path(), default="./workspace")
 def cli_create(local_path):
     """Copy workspace_example folder from S3 to local_path"""
     source_folder = f"{PACKAGE_PATH}/data/workspace_example"
     copy_folder(source_folder, local_path)
 
 @main.command(name="update_package")
 def cli_update_package():
```

### Comparing `serra-0.5/serra/config_parser.py` & `serra-0.6/serra/config_parser.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/autocomplete/README.md` & `serra-0.6/serra/data/autocomplete/README.md`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/autocomplete/gen_schemas.py` & `serra-0.6/serra/data/autocomplete/gen_schemas.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/autocomplete/inputs/specs.json` & `serra-0.6/serra/data/autocomplete/inputs/specs.json`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/autocomplete/output/serra_yaml_schema.json` & `serra-0.6/serra/data/autocomplete/output/serra_yaml_schema.json`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/examples/ratings.csv` & `serra-0.6/serra/data/workspace_example/examples/ratings.csv`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/examples/sales.csv` & `serra-0.6/serra/data/workspace_example/examples/sales.csv`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/examples/states_to_abbreviation.json` & `serra-0.6/serra/data/workspace_example/examples/states_to_abbreviation.json`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/jobs/Demo.yml` & `serra-0.6/serra/data/workspace_example/jobs/Demo.yml`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/sql/easy_demo.sql` & `serra-0.6/serra/data/workspace_example/sql/easy_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/data/workspace_example/sql/hard_demo.sql` & `serra-0.6/serra/data/workspace_example/sql/hard_demo.sql`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/databricks.py` & `serra-0.6/serra/databricks.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/profile.py` & `serra-0.6/serra/profile.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/readers/amazon_reader.py` & `serra-0.6/serra/readers/amazon_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/readers/databricks_reader.py` & `serra-0.6/serra/readers/databricks_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/readers/snowflaker_reader.py` & `serra-0.6/serra/readers/snowflaker_reader.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/run.py` & `serra-0.6/serra/run.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/runners/ExecutionGraph.py` & `serra-0.6/serra/runners/ExecutionGraph.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/runners/graph_runner.py` & `serra-0.6/serra/runners/graph_runner.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/__init__.py` & `serra-0.6/serra/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/add_column_transformer.py` & `serra-0.6/serra/transformers/add_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/case_when_transformer.py` & `serra-0.6/serra/transformers/case_when_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/drop_columns_transformer.py` & `serra-0.6/serra/transformers/drop_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/get_count_transformer.py` & `serra-0.6/serra/transformers/get_count_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/join_transformer.py` & `serra-0.6/serra/transformers/join_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/map_transformer.py` & `serra-0.6/serra/transformers/map_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/pivot_transformer.py` & `serra-0.6/serra/transformers/pivot_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/rename_column_transformer.py` & `serra-0.6/serra/transformers/rename_column_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/transformers/select_transformer.py` & `serra-0.6/serra/transformers/select_transformer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/translate_client.py` & `serra-0.6/serra/translate_client.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/utils.py` & `serra-0.6/serra/utils.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/writers/amazon_writer.py` & `serra-0.6/serra/writers/amazon_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/writers/databricks_writer.py` & `serra-0.6/serra/writers/databricks_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/writers/s3_writer.py` & `serra-0.6/serra/writers/s3_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra/writers/snowflake_writer.py` & `serra-0.6/serra/writers/snowflake_writer.py`

 * *Files identical despite different names*

### Comparing `serra-0.5/serra.egg-info/SOURCES.txt` & `serra-0.6/serra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serra-0.5/setup.py` & `serra-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='serra',
-      version='0.5',
+      version='0.6',
       description='Simplified Data Pipelines',
       url='http://github.com',
       author='Serra Technologies',
       author_email='founders@serra.io',
       packages=setuptools.find_packages(),
       package_data={"serra": ["data/workspace_example/*",
                               "data/workspace_example/*/*",
```

