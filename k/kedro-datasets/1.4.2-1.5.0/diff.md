# Comparing `tmp/kedro-datasets-1.4.2.tar.gz` & `tmp/kedro-datasets-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro-datasets-1.4.2.tar", last modified: Mon Jul  3 09:51:23 2023, max compression
+gzip compressed data, was "kedro-datasets-1.5.0.tar", last modified: Mon Jul 31 15:37:02 2023, max compression
```

## Comparing `kedro-datasets-1.4.2.tar` & `kedro-datasets-1.5.0.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/api/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/api/api_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/biosequence/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/biosequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/biosequence/biosequence_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/dask/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/dask/parquet_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/databricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/databricks/managed_table_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/email/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8009 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/email/message_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/geopandas/geojson_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/holoviews/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/holoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/holoviews/holoviews_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/json/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/json/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/matplotlib/matplotlib_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets/networkx/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/gml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/graphml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/networkx/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10731 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/feather_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/gbq_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/hdf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/parquet_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/sql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pandas/xml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10687 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pickle/pickle_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/pillow/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pillow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/pillow/image_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/plotly/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/plotly/plotly_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/polars/csv_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/redis/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/redis/redis_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/snowflake/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/snowflake/snowpark_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/deltatable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_hive_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7110 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_jdbc_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/spark/spark_streaming_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/svmlight/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/svmlight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/svmlight/svmlight_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.888485 kedro-datasets-1.4.2/kedro_datasets/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tensorflow/tensorflow_model_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/text/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/text/text_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/tracking/metrics_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/video/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/video/video_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/kedro_datasets/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/yaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/kedro_datasets/yaml/yaml_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 09:51:23.884484 kedro-datasets-1.4.2/kedro_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-03 09:51:23.000000 kedro-datasets-1.4.2/kedro_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 09:51:23.892485 kedro-datasets-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-03 09:51:12.000000 kedro-datasets-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/api/api_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/biosequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/biosequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/biosequence/biosequence_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/dask/parquet_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/databricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/databricks/managed_table_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/email/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/email/message_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/geopandas/geojson_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/holoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/holoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/holoviews/holoviews_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/json/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/matplotlib/matplotlib_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.839839 kedro-datasets-1.5.0/kedro_datasets/networkx/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/gml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/graphml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/networkx/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10802 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/feather_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/gbq_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9998 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/hdf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/parquet_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21158 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/sql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pandas/xml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10741 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pickle/pickle_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/pillow/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pillow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/pillow/image_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/plotly/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/plotly/plotly_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/polars/csv_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.843839 kedro-datasets-1.5.0/kedro_datasets/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/redis/redis_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/snowflake/snowpark_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/deltatable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16216 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_hive_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_jdbc_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/spark/spark_streaming_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/svmlight/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/svmlight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/svmlight/svmlight_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7755 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/text/text_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/tracking/metrics_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12475 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/video/video_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.847839 kedro-datasets-1.5.0/kedro_datasets/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/yaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/kedro_datasets/yaml/yaml_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.835839 kedro-datasets-1.5.0/kedro_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 15:37:02.000000 kedro-datasets-1.5.0/kedro_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:37:02.851839 kedro-datasets-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-31 15:36:49.000000 kedro-datasets-1.5.0/tests/test_io.py
```

### Comparing `kedro-datasets-1.4.2/README.md` & `kedro-datasets-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.2/kedro_datasets/api/api_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/api/api_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 It uses the python requests library: https://requests.readthedocs.io/en/latest/
 """
 import json as json_  # make pylint happy
 from copy import deepcopy
 from typing import Any, Dict, List, Tuple, Union
 
 import requests
-from kedro.io.core import AbstractDataSet, DataSetError
 from requests import Session, sessions
 from requests.auth import AuthBase
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 
 class APIDataSet(AbstractDataSet[None, requests.Response]):
     """``APIDataSet`` loads/saves data from/to HTTP(S) APIs.
     It uses the python requests library: https://requests.readthedocs.io/en/latest/
 
     Example usage for the `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/biosequence/biosequence_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/biosequence/biosequence_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict, List
 
 import fsspec
 from Bio import SeqIO
-from kedro.io.core import AbstractDataSet, get_filepath_str, get_protocol_and_path
+from kedro.io.core import get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractDataset as AbstractDataSet
 
 
 class BioSequenceDataSet(AbstractDataSet[List, List]):
     r"""``BioSequenceDataSet`` loads and saves data to a sequence file.
 
     Example:
     ::
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/dask/parquet_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/dask/parquet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 
 from copy import deepcopy
 from typing import Any, Dict
 
 import dask.dataframe as dd
 import fsspec
 import triad
-from kedro.io.core import AbstractDataSet, get_protocol_and_path
+from kedro.io.core import get_protocol_and_path
+
+from .._io import AbstractDataset as AbstractDataSet
 
 
 class ParquetDataSet(AbstractDataSet[dd.DataFrame, dd.DataFrame]):
     """``ParquetDataSet`` loads and saves data to parquet file(s). It uses Dask
     remote data services to handle the corresponding load and save operations:
     https://docs.dask.org/en/latest/how-to/connect-to-remote-data.html
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/databricks/managed_table_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/databricks/managed_table_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 """
 import logging
 import re
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    VersionNotFoundError,
-)
+from kedro.io.core import Version, VersionNotFoundError
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
 from pyspark.sql.utils import AnalysisException, ParseException
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 @dataclass(frozen=True)
 class ManagedTable:
     """Stores the definition of a managed table"""
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/email/message_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/email/message_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 from email.message import Message
 from email.parser import Parser
 from email.policy import default
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class EmailMessageDataSet(AbstractVersionedDataSet[Message, Message]):
     """``EmailMessageDataSet`` loads/saves an email message from/to a file
     using an underlying filesystem (e.g.: local, S3, GCS). It uses the
     ``email`` package in the standard library to manage email messages.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/geopandas/geojson_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/geopandas/geojson_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 """
 import copy
 from pathlib import PurePosixPath
 from typing import Any, Dict, Union
 
 import fsspec
 import geopandas as gpd
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class GeoJSONDataSet(
     AbstractVersionedDataSet[
         gpd.GeoDataFrame, Union[gpd.GeoDataFrame, Dict[str, gpd.GeoDataFrame]]
     ]
 ):
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/holoviews/holoviews_writer.py` & `kedro-datasets-1.5.0/kedro_datasets/holoviews/holoviews_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 import io
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict, NoReturn, TypeVar
 
 import fsspec
 import holoviews as hv
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 # HoloViews to be passed in `hv.save()`
 HoloViews = TypeVar("HoloViews")
 
 
 class HoloviewsWriter(AbstractVersionedDataSet[HoloViews, NoReturn]):
     """``HoloviewsWriter`` saves Holoviews objects to image file(s) in an underlying
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/json/json_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/json/json_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 """
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class JSONDataSet(AbstractVersionedDataSet[Any, Any]):
     """``JSONDataSet`` loads/saves data from/to a JSON file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 
     Example usage for the
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/matplotlib/matplotlib_writer.py` & `kedro-datasets-1.5.0/kedro_datasets/matplotlib/matplotlib_writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict, List, NoReturn, Union
 from warnings import warn
 
 import fsspec
 import matplotlib.pyplot as plt
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class MatplotlibWriter(
     AbstractVersionedDataSet[
         Union[plt.figure, List[plt.figure], Dict[str, plt.figure]], NoReturn
     ]
 ):
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/networkx/gml_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/networkx/graphml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-"""NetworkX ``GMLDataSet`` loads and saves graphs to a graph modelling language (GML)
-file using an underlying filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to
-create GML data.
+"""NetworkX ``GraphMLDataSet`` loads and saves graphs to a GraphML file using an underlying
+filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to create GraphML data.
 """
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import networkx
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
 
-class GMLDataSet(AbstractVersionedDataSet[networkx.Graph, networkx.Graph]):
-    """``GMLDataSet`` loads and saves graphs to a GML file using an
+
+class GraphMLDataSet(AbstractVersionedDataSet[networkx.Graph, networkx.Graph]):
+    """``GraphMLDataSet`` loads and saves graphs to a GraphML file using an
     underlying filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to
-    create GML data.
+    create GraphML data.
     See https://networkx.org/documentation/stable/tutorial.html for details.
 
     Example:
     ::
 
-        >>> from kedro_datasets.networkx import GMLDataSet
+        >>> from kedro_datasets.networkx import GraphMLDataSet
         >>> import networkx as nx
         >>> graph = nx.complete_graph(100)
-        >>> graph_dataset = GMLDataSet(filepath="test.gml")
+        >>> graph_dataset = GraphMLDataSet(filepath="test.graphml")
         >>> graph_dataset.save(graph)
         >>> reloaded = graph_dataset.load()
         >>> assert nx.is_isomorphic(graph, reloaded)
 
     """
 
     DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
@@ -46,39 +42,39 @@
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
         metadata: Dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``GMLDataSet``.
+        """Creates a new instance of ``GraphMLDataSet``.
 
         Args:
-            filepath: Filepath in POSIX format to the NetworkX GML file.
-            load_args: Arguments passed on to ``networkx.read_gml``.
+            filepath: Filepath in POSIX format to the NetworkX GraphML file.
+            load_args: Arguments passed on to ``networkx.read_graphml``.
                 See the details in
-                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gml.read_gml.html
-            save_args: Arguments passed on to ``networkx.write_gml``.
+                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.graphml.read_graphml.html
+            save_args: Arguments passed on to ``networkx.write_graphml``.
                 See the details in
-                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gml.write_gml.html
+                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.graphml.write_graphml.html
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
-            metadata: Any Any arbitrary metadata.
+            metadata: Any arbitrary Any arbitrary metadata.
                 This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
@@ -109,21 +105,20 @@
         _fs_open_args_save.setdefault("mode", "wb")
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
     def _load(self) -> networkx.Graph:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
-            data = networkx.read_gml(fs_file, **self._load_args)
-        return data
+            return networkx.read_graphml(fs_file, **self._load_args)
 
     def _save(self, data: networkx.Graph) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
         with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
-            networkx.write_gml(data, fs_file, **self._save_args)
+            networkx.write_graphml(data, fs_file, **self._save_args)
         self._invalidate_cache()
 
     def _exists(self) -> bool:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         return self._fs.exists(load_path)
 
     def _describe(self) -> Dict[str, Any]:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/networkx/graphml_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/networkx/gml_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
-"""NetworkX ``GraphMLDataSet`` loads and saves graphs to a GraphML file using an underlying
-filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to create GraphML data.
+"""NetworkX ``GMLDataSet`` loads and saves graphs to a graph modelling language (GML)
+file using an underlying filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to
+create GML data.
 """
 
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import networkx
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
 
-class GraphMLDataSet(AbstractVersionedDataSet[networkx.Graph, networkx.Graph]):
-    """``GraphMLDataSet`` loads and saves graphs to a GraphML file using an
+
+class GMLDataSet(AbstractVersionedDataSet[networkx.Graph, networkx.Graph]):
+    """``GMLDataSet`` loads and saves graphs to a GML file using an
     underlying filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to
-    create GraphML data.
+    create GML data.
     See https://networkx.org/documentation/stable/tutorial.html for details.
 
     Example:
     ::
 
-        >>> from kedro_datasets.networkx import GraphMLDataSet
+        >>> from kedro_datasets.networkx import GMLDataSet
         >>> import networkx as nx
         >>> graph = nx.complete_graph(100)
-        >>> graph_dataset = GraphMLDataSet(filepath="test.graphml")
+        >>> graph_dataset = GMLDataSet(filepath="test.gml")
         >>> graph_dataset.save(graph)
         >>> reloaded = graph_dataset.load()
         >>> assert nx.is_isomorphic(graph, reloaded)
 
     """
 
     DEFAULT_LOAD_ARGS: Dict[str, Any] = {}
@@ -45,39 +43,39 @@
         load_args: Dict[str, Any] = None,
         save_args: Dict[str, Any] = None,
         version: Version = None,
         credentials: Dict[str, Any] = None,
         fs_args: Dict[str, Any] = None,
         metadata: Dict[str, Any] = None,
     ) -> None:
-        """Creates a new instance of ``GraphMLDataSet``.
+        """Creates a new instance of ``GMLDataSet``.
 
         Args:
-            filepath: Filepath in POSIX format to the NetworkX GraphML file.
-            load_args: Arguments passed on to ``networkx.read_graphml``.
+            filepath: Filepath in POSIX format to the NetworkX GML file.
+            load_args: Arguments passed on to ``networkx.read_gml``.
                 See the details in
-                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.graphml.read_graphml.html
-            save_args: Arguments passed on to ``networkx.write_graphml``.
+                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gml.read_gml.html
+            save_args: Arguments passed on to ``networkx.write_gml``.
                 See the details in
-                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.graphml.write_graphml.html
+                https://networkx.org/documentation/stable/reference/readwrite/generated/networkx.readwrite.gml.write_gml.html
             version: If specified, should be an instance of
                 ``kedro.io.core.Version``. If its ``load`` attribute is
                 None, the latest version will be loaded. If its ``save``
                 attribute is None, save version will be autogenerated.
             credentials: Credentials required to get access to the underlying filesystem.
                 E.g. for ``GCSFileSystem`` it should look like `{"token": None}`.
             fs_args: Extra arguments to pass into underlying filesystem class constructor
                 (e.g. `{"project": "my-project"}` for ``GCSFileSystem``), as well as
                 to pass to the filesystem's `open` method through nested keys
                 `open_args_load` and `open_args_save`.
                 Here you can find all available arguments for `open`:
                 https://filesystem-spec.readthedocs.io/en/latest/api.html#fsspec.spec.AbstractFileSystem.open
                 All defaults are preserved, except `mode`, which is set to `r` when loading
                 and to `w` when saving.
-            metadata: Any arbitrary Any arbitrary metadata.
+            metadata: Any Any arbitrary metadata.
                 This is ignored by Kedro, but may be consumed by users or external plugins.
         """
         _fs_args = deepcopy(fs_args) or {}
         _fs_open_args_load = _fs_args.pop("open_args_load", {})
         _fs_open_args_save = _fs_args.pop("open_args_save", {})
         _credentials = deepcopy(credentials) or {}
 
@@ -108,20 +106,21 @@
         _fs_open_args_save.setdefault("mode", "wb")
         self._fs_open_args_load = _fs_open_args_load
         self._fs_open_args_save = _fs_open_args_save
 
     def _load(self) -> networkx.Graph:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
-            return networkx.read_graphml(fs_file, **self._load_args)
+            data = networkx.read_gml(fs_file, **self._load_args)
+        return data
 
     def _save(self, data: networkx.Graph) -> None:
         save_path = get_filepath_str(self._get_save_path(), self._protocol)
         with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
-            networkx.write_graphml(data, fs_file, **self._save_args)
+            networkx.write_gml(data, fs_file, **self._save_args)
         self._invalidate_cache()
 
     def _exists(self) -> bool:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
         return self._fs.exists(load_path)
 
     def _describe(self) -> Dict[str, Any]:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/networkx/json_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/networkx/json_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,17 @@
 import json
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import networkx
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
 
 
 class JSONDataSet(AbstractVersionedDataSet[networkx.Graph, networkx.Graph]):
     """NetworkX ``JSONDataSet`` loads and saves graphs to a JSON file using an
     underlying filesystem (e.g.: local, S3, GCS). ``NetworkX`` is used to
     create JSON data.
     See https://networkx.org/documentation/stable/tutorial.html for details.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/csv_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/csv_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class CSVDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``CSVDataSet`` loads/saves data from/to a CSV file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to handle the CSV file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/excel_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/excel_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict, Union
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class ExcelDataSet(
     AbstractVersionedDataSet[
         Union[pd.DataFrame, Dict[str, pd.DataFrame]],
         Union[pd.DataFrame, Dict[str, pd.DataFrame]],
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/feather_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/feather_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+
 logger = logging.getLogger(__name__)
 
 
 class FeatherDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``FeatherDataSet`` loads and saves data to a feather file using an
     underlying filesystem (e.g.: local, S3, GCS). The underlying functionality
     is supported by pandas, so it supports all allowed pandas options
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/gbq_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/gbq_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 
 import fsspec
 import pandas as pd
 from google.cloud import bigquery
 from google.cloud.exceptions import NotFound
 from google.oauth2.credentials import Credentials
 from kedro.io.core import (
-    AbstractDataSet,
-    DataSetError,
     get_filepath_str,
     get_protocol_and_path,
     validate_on_forbidden_chars,
 )
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 
 class GBQTableDataSet(AbstractDataSet[None, pd.DataFrame]):
     """``GBQTableDataSet`` loads and saves data from/to Google BigQuery.
     It uses pandas-gbq to read and write from/to BigQuery table.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
@@ -312,9 +313,9 @@
 
         return pd.read_gbq(
             project_id=self._project_id,
             credentials=self._credentials,
             **load_args,
         )
 
-    def _save(self, data: None) -> NoReturn:
+    def _save(self, data: None) -> NoReturn:  # pylint: disable=no-self-use
         raise DataSetError("'save' is not supported on GBQQueryDataSet")
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/generic_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/generic_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 NON_FILE_SYSTEM_TARGETS = [
     "clipboard",
     "numpy",
     "sql",
     "period",
     "records",
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/hdf_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/hdf_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 from copy import deepcopy
 from pathlib import PurePosixPath
 from threading import Lock
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 HDFSTORE_DRIVER = "H5FD_CORE"
 
 
 class HDFDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``HDFDataSet`` loads/saves data from/to a hdf file using an underlying
     filesystem (e.g. local, S3, GCS). It uses pandas.HDFStore to handle the hdf file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/json_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/json_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class JSONDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``JSONDataSet`` loads/saves data from/to a JSON file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to handle the json file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/parquet_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/parquet_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import Path, PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class ParquetDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``ParquetDataSet`` loads/saves data from/to a Parquet file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to handle the Parquet file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/sql_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/sql_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,21 @@
 import datetime as dt
 import re
 from pathlib import PurePosixPath
 from typing import Any, Dict, NoReturn, Optional
 
 import fsspec
 import pandas as pd
-from kedro.io.core import (
-    AbstractDataSet,
-    DataSetError,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import get_filepath_str, get_protocol_and_path
 from sqlalchemy import create_engine, inspect
 from sqlalchemy.exc import NoSuchModuleError
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 __all__ = ["SQLTableDataSet", "SQLQueryDataSet"]
 
 KNOWN_PIP_INSTALL = {
     "psycopg2": "psycopg2",
     "mysqldb": "mysqlclient",
     "cx_Oracle": "cx_Oracle",
     "mssql": "pyodbc",
@@ -507,15 +505,15 @@
         if self._filepath:
             load_path = get_filepath_str(PurePosixPath(self._filepath), self._protocol)
             with self._fs.open(load_path, mode="r") as fs_file:
                 load_args["sql"] = fs_file.read()
 
         return pd.read_sql_query(con=engine, **load_args)
 
-    def _save(self, data: None) -> NoReturn:
+    def _save(self, data: None) -> NoReturn:  # pylint: disable=no-self-use
         raise DataSetError("'save' is not supported on SQLQueryDataSet")
 
     # For mssql only
     def adapt_mssql_date_params(self) -> None:
         """We need to change the format of datetime parameters.
         MSSQL expects datetime in the exact format %y-%m-%dT%H:%M:%S.
         Here, we also accept plain dates.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pandas/xml_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pandas/xml_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import pandas as pd
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class XMLDataSet(AbstractVersionedDataSet[pd.DataFrame, pd.DataFrame]):
     """``XMLDataSet`` loads/saves data from/to a XML file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses pandas to handle the XML file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pickle/pickle_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pickle/pickle_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 """
 import importlib
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class PickleDataSet(AbstractVersionedDataSet[Any, Any]):
     """``PickleDataSet`` loads/saves data from/to a Pickle file using an underlying
     filesystem (e.g.: local, S3, GCS). The underlying functionality is supported by
     the specified backend library passed in (defaults to the ``pickle`` library), so it
     supports all allowed options for loading and saving pickle files.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/pillow/image_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/pillow/image_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,23 +2,20 @@
 filesystem (e.g.: local, S3, GCS). It uses Pillow to handle image file.
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 from PIL import Image
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 
 class ImageDataSet(AbstractVersionedDataSet[Image.Image, Image.Image]):
     """``ImageDataSet`` loads/saves image data as `numpy` from an underlying
     filesystem (e.g.: local, S3, GCS). It uses Pillow to handle image file.
 
     Example usage for the
     `Python API <https://kedro.readthedocs.io/en/stable/data/\
@@ -115,21 +112,30 @@
     def _load(self) -> Image.Image:
         load_path = get_filepath_str(self._get_load_path(), self._protocol)
 
         with self._fs.open(load_path, **self._fs_open_args_load) as fs_file:
             return Image.open(fs_file).copy()
 
     def _save(self, data: Image.Image) -> None:
-        save_path = get_filepath_str(self._get_save_path(), self._protocol)
+        save_path = self._get_save_path()
 
-        with self._fs.open(save_path, **self._fs_open_args_save) as fs_file:
-            data.save(fs_file, **self._save_args)
+        with self._fs.open(
+            get_filepath_str(save_path, self._protocol), **self._fs_open_args_save
+        ) as fs_file:
+            data.save(fs_file, format=self._get_format(save_path), **self._save_args)
 
         self._invalidate_cache()
 
+    @staticmethod
+    def _get_format(file_path: PurePosixPath):
+        ext = file_path.suffix.lower()
+        if ext not in Image.EXTENSION:
+            Image.init()
+        return Image.EXTENSION.get(ext)
+
     def _exists(self) -> bool:
         try:
             load_path = get_filepath_str(self._get_load_path(), self._protocol)
         except DataSetError:
             return False
 
         return self._fs.exists(load_path)
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/plotly/json_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/plotly/json_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,19 @@
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict, Union
 
 import fsspec
 import plotly.io as pio
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 from plotly import graph_objects as go
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+
 
 class JSONDataSet(
     AbstractVersionedDataSet[go.Figure, Union[go.Figure, go.FigureWidget]]
 ):
     """``JSONDataSet`` loads/saves a plotly figure from/to a JSON file using an
     underlying filesystem (e.g.: local, S3, GCS).
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/plotly/plotly_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/plotly/plotly_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro-datasets-1.4.2/kedro_datasets/polars/csv_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/polars/csv_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import polars as pl
 from kedro.io.core import (
     PROTOCOL_DELIMITER,
-    AbstractVersionedDataSet,
-    DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 class CSVDataSet(AbstractVersionedDataSet[pl.DataFrame, pl.DataFrame]):
     """``CSVDataSet`` loads/saves data from/to a CSV file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses polars to handle the CSV file.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/redis/redis_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/redis/redis_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 import importlib
 import os
 from copy import deepcopy
 from typing import Any, Dict
 
 import redis
-from kedro.io.core import AbstractDataSet, DataSetError
+
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
 
 
 class PickleDataSet(AbstractDataSet[Any, Any]):
     """``PickleDataSet`` loads/saves data from/to a Redis database. The
     underlying functionality is supported by the redis library, so it supports
     all allowed options for instantiating the redis app ``from_url`` and setting
     a value.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/snowflake/snowpark_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/snowflake/snowpark_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """``AbstractDataSet`` implementation to access Snowflake using Snowpark dataframes
 """
 import logging
 from copy import deepcopy
 from typing import Any, Dict
 
 import snowflake.snowpark as sp
-from kedro.io.core import AbstractDataSet, DataSetError
+
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
 
 logger = logging.getLogger(__name__)
 
 
 class SnowparkTableDataSet(AbstractDataSet):
     """``SnowparkTableDataSet`` loads and saves Snowpark dataframes.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/spark/deltatable_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/spark/deltatable_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """``AbstractDataSet`` implementation to access DeltaTables using
 ``delta-spark``
 """
 from pathlib import PurePosixPath
 from typing import Any, Dict, NoReturn
 
 from delta.tables import DeltaTable
-from kedro.io.core import AbstractDataSet, DataSetError
 from pyspark.sql import SparkSession
 from pyspark.sql.utils import AnalysisException
 
 from kedro_datasets.spark.spark_dataset import _split_filepath, _strip_dbfs_prefix
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 
 class DeltaTableDataSet(AbstractDataSet[None, DeltaTable]):
     """``DeltaTableDataSet`` loads data into DeltaTable objects.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/spark/spark_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/spark/spark_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,23 @@
 from functools import partial
 from pathlib import PurePosixPath
 from typing import Any, Dict, List, Optional, Tuple
 from warnings import warn
 
 import fsspec
 from hdfs import HdfsError, InsecureClient
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
 from pyspark.sql.utils import AnalysisException
 from s3fs import S3FileSystem
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 logger = logging.getLogger(__name__)
 
 
 def _parse_glob_pattern(pattern: str) -> str:
     special = ("*", "?", "[")
     clean = []
     for part in pattern.split("/"):
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/spark/spark_hive_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/spark/spark_hive_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """``AbstractDataSet`` implementation to access Spark dataframes using
 ``pyspark`` on Apache Hive.
 """
 import pickle
 from copy import deepcopy
 from typing import Any, Dict, List
 
-from kedro.io.core import AbstractDataSet, DataSetError
 from pyspark.sql import DataFrame, SparkSession, Window
 from pyspark.sql.functions import col, lit, row_number
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 
 # pylint:disable=too-many-instance-attributes
 class SparkHiveDataSet(AbstractDataSet[DataFrame, DataFrame]):
     """``SparkHiveDataSet`` loads and saves Spark dataframes stored on Hive.
     This data set also handles some incompatible file types such as using partitioned parquet on
     hive which will not normally allow upserts to existing data without a complete replacement
     of the existing file/partition.
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/spark/spark_jdbc_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/spark/spark_jdbc_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """SparkJDBCDataSet to load and save a PySpark DataFrame via JDBC."""
 
 from copy import deepcopy
 from typing import Any, Dict
 
-from kedro.io.core import AbstractDataSet, DataSetError
 from pyspark.sql import DataFrame, SparkSession
 
+from .._io import AbstractDataset as AbstractDataSet
+from .._io import DatasetError as DataSetError
+
 __all__ = ["SparkJDBCDataSet"]
 
 
 class SparkJDBCDataSet(AbstractDataSet[DataFrame, DataFrame]):
     """``SparkJDBCDataSet`` loads data from a database table accessible
     via JDBC URL url and connection properties and saves the content of
     a PySpark DataFrame to an external database table via JDBC.  It uses
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/spark/spark_streaming_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/spark/spark_streaming_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """SparkStreamingDataSet to load and save a PySpark Streaming DataFrame."""
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
-from kedro.io.core import AbstractDataSet
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.utils import AnalysisException
 
 from kedro_datasets.spark.spark_dataset import (
     SparkDataSet,
     _split_filepath,
     _strip_dbfs_prefix,
 )
 
+from .._io import AbstractDataset as AbstractDataSet
+
 
 class SparkStreamingDataSet(AbstractDataSet):
     """``SparkStreamingDataSet`` loads data to Spark Streaming Dataframe objects.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
     data_catalog.html#use-the-data-catalog-with-the-yaml-api>`_:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/svmlight/svmlight_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/svmlight/svmlight_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 ``dump_svmlight_file`` to save and ``load_svmlight_file`` to load a file.
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict, Optional, Tuple, Union
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
 from numpy import ndarray
 from scipy.sparse.csr import csr_matrix
 from sklearn.datasets import dump_svmlight_file, load_svmlight_file
 
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
+
 # NOTE: kedro.extras.datasets will be removed in Kedro 0.19.0.
 # Any contribution to datasets should be made in kedro-datasets
 # in kedro-plugins (https://github.com/kedro-org/kedro-plugins)
 
 # Type of data input
 _DI = Tuple[Union[ndarray, csr_matrix], ndarray]
 # Type of data output
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/tensorflow/tensorflow_model_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/tensorflow/tensorflow_model_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 import copy
 import tempfile
 from pathlib import PurePath, PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import tensorflow as tf
+
+# TODO: Replace these imports by the appropriate ones from kedro_datasets._io
+# to avoid deprecation warnings for users,
+# see https://github.com/kedro-org/kedro-plugins/pull/255
 from kedro.io.core import (
     AbstractVersionedDataSet,
     DataSetError,
     Version,
     get_filepath_str,
     get_protocol_and_path,
 )
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/text/text_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/text/text_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 filesystem (e.g.: local, S3, GCS).
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class TextDataSet(AbstractVersionedDataSet[str, str]):
     """``TextDataSet`` loads/saves data from/to a text file using an underlying
     filesystem (e.g.: local, S3, GCS)
 
     Example usage for the
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/tracking/json_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/tracking/json_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
 The ``JSONDataSet`` is part of Kedro Experiment Tracking. The dataset is versioned by default.
 """
 from typing import NoReturn
 
 from kedro.io.core import DataSetError
 
-from kedro_datasets.json import JSONDataSet as JDS
+from kedro_datasets.json import json_dataset
 
 
-class JSONDataSet(JDS):
+class JSONDataSet(json_dataset.JSONDataSet):
     """``JSONDataSet`` saves data to a JSON file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file.
     The ``JSONDataSet`` is part of Kedro Experiment Tracking.
     The dataset is write-only and it is versioned by default.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/tracking/metrics_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/tracking/metrics_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 and only takes metrics of numeric values.
 """
 import json
 from typing import Dict, NoReturn
 
 from kedro.io.core import DataSetError, get_filepath_str
 
-from kedro_datasets.json import JSONDataSet
+from kedro_datasets.json import json_dataset
 
 
-class MetricsDataSet(JSONDataSet):
+class MetricsDataSet(json_dataset.JSONDataSet):
     """``MetricsDataSet`` saves data to a JSON file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses native json to handle the JSON file. The
     ``MetricsDataSet`` is part of Kedro Experiment Tracking. The dataset is write-only,
     it is versioned by default and only takes metrics of numeric values.
 
     Example usage for the
     `YAML API <https://kedro.readthedocs.io/en/stable/data/\
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/video/video_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/video/video_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 from pathlib import Path, PurePosixPath
 from typing import Any, Dict, Generator, Optional, Sequence, Tuple, Union
 
 import cv2
 import fsspec
 import numpy as np
 import PIL.Image
-from kedro.io.core import AbstractDataSet, get_protocol_and_path
+from kedro.io.core import get_protocol_and_path
+
+from .._io import AbstractDataset as AbstractDataSet
 
 
 class SlicedVideo:
     """A representation of slices of other video types"""
 
     def __init__(self, video, slice_indexes):
         self.video = video
@@ -154,15 +156,14 @@
             return SlicedVideo(self, index)
         return self._frames[index]
 
 
 class GeneratorVideo(AbstractVideo):
     """A video object with frames yielded by a generator"""
 
-    # pylint: disable=too-many-arguments
     def __init__(
         self,
         frames: Generator[PIL.Image.Image, None, None],
         length,
         fps: float,
         fourcc: str = "mp4v",
     ) -> None:
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets/yaml/yaml_dataset.py` & `kedro-datasets-1.5.0/kedro_datasets/yaml/yaml_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 """
 from copy import deepcopy
 from pathlib import PurePosixPath
 from typing import Any, Dict
 
 import fsspec
 import yaml
-from kedro.io.core import (
-    AbstractVersionedDataSet,
-    DataSetError,
-    Version,
-    get_filepath_str,
-    get_protocol_and_path,
-)
+from kedro.io.core import Version, get_filepath_str, get_protocol_and_path
+
+from .._io import AbstractVersionedDataset as AbstractVersionedDataSet
+from .._io import DatasetError as DataSetError
 
 
 class YAMLDataSet(AbstractVersionedDataSet[Dict, Dict]):
     """``YAMLDataSet`` loads/saves data from/to a YAML file using an underlying
     filesystem (e.g.: local, S3, GCS). It uses PyYAML to handle the YAML file.
 
     Example usage for the
```

### Comparing `kedro-datasets-1.4.2/kedro_datasets.egg-info/SOURCES.txt` & `kedro-datasets-1.5.0/kedro_datasets.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 README.md
 pyproject.toml
-setup.py
 kedro_datasets/__init__.py
+kedro_datasets/_io.py
 kedro_datasets.egg-info/PKG-INFO
 kedro_datasets.egg-info/SOURCES.txt
 kedro_datasets.egg-info/dependency_links.txt
 kedro_datasets.egg-info/requires.txt
 kedro_datasets.egg-info/top_level.txt
 kedro_datasets/api/__init__.py
 kedro_datasets/api/api_dataset.py
@@ -27,14 +27,15 @@
 kedro_datasets/matplotlib/matplotlib_writer.py
 kedro_datasets/networkx/__init__.py
 kedro_datasets/networkx/gml_dataset.py
 kedro_datasets/networkx/graphml_dataset.py
 kedro_datasets/networkx/json_dataset.py
 kedro_datasets/pandas/__init__.py
 kedro_datasets/pandas/csv_dataset.py
+kedro_datasets/pandas/deltatable_dataset.py
 kedro_datasets/pandas/excel_dataset.py
 kedro_datasets/pandas/feather_dataset.py
 kedro_datasets/pandas/gbq_dataset.py
 kedro_datasets/pandas/generic_dataset.py
 kedro_datasets/pandas/hdf_dataset.py
 kedro_datasets/pandas/json_dataset.py
 kedro_datasets/pandas/parquet_dataset.py
@@ -67,8 +68,9 @@
 kedro_datasets/text/text_dataset.py
 kedro_datasets/tracking/__init__.py
 kedro_datasets/tracking/json_dataset.py
 kedro_datasets/tracking/metrics_dataset.py
 kedro_datasets/video/__init__.py
 kedro_datasets/video/video_dataset.py
 kedro_datasets/yaml/__init__.py
-kedro_datasets/yaml/yaml_dataset.py
+kedro_datasets/yaml/yaml_dataset.py
+tests/test_io.py
```

