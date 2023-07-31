# Comparing `tmp/soda-core-denodo-3.0.46.tar.gz` & `tmp/soda-core-denodo-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-denodo-3.0.46.tar", last modified: Wed Jul 19 15:16:00 2023, max compression
+gzip compressed data, was "soda-core-denodo-3.0.47.tar", last modified: Mon Jul 31 08:36:17 2023, max compression
```

## Comparing `soda-core-denodo-3.0.46.tar` & `soda-core-denodo-3.0.47.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.432125 soda-core-denodo-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:00.431691 soda-core-denodo-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:00.432259 soda-core-denodo-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      657 2023-07-19 13:37:16.000000 soda-core-denodo-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.426888 soda-core-denodo-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.428492 soda-core-denodo-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)     2479 2023-06-08 07:54:26.000000 soda-core-denodo-3.0.46/soda/data_sources/denodo_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:00.431185 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       45 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:00.000000 soda-core-denodo-3.0.46/soda_core_denodo.egg-info/top_level.txt
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:17.934364 soda-core-denodo-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:17.934165 soda-core-denodo-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:36:17.934435 soda-core-denodo-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      469 2023-07-28 11:01:31.000000 soda-core-denodo-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:17.932196 soda-core-denodo-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:17.932754 soda-core-denodo-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     2479 2023-06-13 14:41:04.000000 soda-core-denodo-3.0.47/soda/data_sources/denodo_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:17.933882 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:17.000000 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-31 08:36:17.000000 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:36:17.000000 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       45 2023-07-31 08:36:17.000000 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:36:17.000000 soda-core-denodo-3.0.47/soda_core_denodo.egg-info/top_level.txt
```

### Comparing `soda-core-denodo-3.0.46/soda/data_sources/denodo_data_source.py` & `soda-core-denodo-3.0.47/soda/data_sources/denodo_data_source.py`

 * *Files identical despite different names*

