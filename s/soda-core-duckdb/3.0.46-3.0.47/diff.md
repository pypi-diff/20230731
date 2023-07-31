# Comparing `tmp/soda-core-duckdb-3.0.46.tar.gz` & `tmp/soda-core-duckdb-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-duckdb-3.0.46.tar", last modified: Wed Jul 19 15:16:08 2023, max compression
+gzip compressed data, was "soda-core-duckdb-3.0.47.tar", last modified: Mon Jul 31 08:36:24 2023, max compression
```

## Comparing `soda-core-duckdb-3.0.46.tar` & `soda-core-duckdb-3.0.47.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:08.339895 soda-core-duckdb-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:08.339567 soda-core-duckdb-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:08.340018 soda-core-duckdb-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      579 2023-07-19 13:37:16.000000 soda-core-duckdb-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:08.335758 soda-core-duckdb-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:08.336726 soda-core-duckdb-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)     5504 2023-06-08 07:54:26.000000 soda-core-duckdb-3.0.46/soda/data_sources/duckdb_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:08.338615 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:08.000000 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      268 2023-07-19 15:16:08.000000 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:08.000000 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       30 2023-07-19 15:16:08.000000 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:08.000000 soda-core-duckdb-3.0.46/soda_core_duckdb.egg-info/top_level.txt
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:08.338949 soda-core-duckdb-3.0.46/tests/
--rw-r--r--   0 vijay      (501) staff       (20)      690 2023-06-08 07:54:26.000000 soda-core-duckdb-3.0.46/tests/test_duckdb.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:24.658268 soda-core-duckdb-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:24.658025 soda-core-duckdb-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:36:24.658331 soda-core-duckdb-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      391 2023-07-28 11:01:31.000000 soda-core-duckdb-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:24.655978 soda-core-duckdb-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:24.656416 soda-core-duckdb-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     5504 2023-06-13 14:41:04.000000 soda-core-duckdb-3.0.47/soda/data_sources/duckdb_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:24.657718 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:24.000000 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-31 08:36:24.000000 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:36:24.000000 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       30 2023-07-31 08:36:24.000000 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:36:24.000000 soda-core-duckdb-3.0.47/soda_core_duckdb.egg-info/top_level.txt
```

### Comparing `soda-core-duckdb-3.0.46/soda/data_sources/duckdb_data_source.py` & `soda-core-duckdb-3.0.47/soda/data_sources/duckdb_data_source.py`

 * *Files identical despite different names*

