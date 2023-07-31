# Comparing `tmp/soda-core-dremio-3.0.46.tar.gz` & `tmp/soda-core-dremio-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-dremio-3.0.46.tar", last modified: Wed Jul 19 15:16:04 2023, max compression
+gzip compressed data, was "soda-core-dremio-3.0.47.tar", last modified: Mon Jul 31 08:36:20 2023, max compression
```

## Comparing `soda-core-dremio-3.0.46.tar` & `soda-core-dremio-3.0.47.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:04.311900 soda-core-dremio-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:04.311433 soda-core-dremio-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:04.312044 soda-core-dremio-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      585 2023-07-19 13:37:16.000000 soda-core-dremio-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:04.306812 soda-core-dremio-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:04.307814 soda-core-dremio-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)     5458 2023-06-08 07:54:26.000000 soda-core-dremio-3.0.46/soda/data_sources/dremio_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:04.310037 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:04.000000 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      268 2023-07-19 15:16:04.000000 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:04.000000 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       33 2023-07-19 15:16:04.000000 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:04.000000 soda-core-dremio-3.0.46/soda_core_dremio.egg-info/top_level.txt
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:04.310374 soda-core-dremio-3.0.46/tests/
--rw-r--r--   0 vijay      (501) staff       (20)      141 2023-06-08 07:54:26.000000 soda-core-dremio-3.0.46/tests/test_dremio.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:20.951866 soda-core-dremio-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:20.951693 soda-core-dremio-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:36:20.951941 soda-core-dremio-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      397 2023-07-28 11:01:31.000000 soda-core-dremio-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:20.950055 soda-core-dremio-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:20.950494 soda-core-dremio-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     5458 2023-06-13 14:41:04.000000 soda-core-dremio-3.0.47/soda/data_sources/dremio_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:20.951452 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:20.000000 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-31 08:36:20.000000 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:36:20.000000 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       33 2023-07-31 08:36:20.000000 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:36:20.000000 soda-core-dremio-3.0.47/soda_core_dremio.egg-info/top_level.txt
```

### Comparing `soda-core-dremio-3.0.46/soda/data_sources/dremio_data_source.py` & `soda-core-dremio-3.0.47/soda/data_sources/dremio_data_source.py`

 * *Files identical despite different names*

