# Comparing `tmp/soda-core-vertica-3.0.46.tar.gz` & `tmp/soda-core-vertica-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-vertica-3.0.46.tar", last modified: Wed Jul 19 15:16:41 2023, max compression
+gzip compressed data, was "soda-core-vertica-3.0.47.tar", last modified: Mon Jul 31 08:37:00 2023, max compression
```

## Comparing `soda-core-vertica-3.0.46.tar` & `soda-core-vertica-3.0.47.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:41.513647 soda-core-vertica-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       62 2023-07-19 15:16:41.513221 soda-core-vertica-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:41.513820 soda-core-vertica-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      597 2023-07-19 13:37:16.000000 soda-core-vertica-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:41.508162 soda-core-vertica-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:41.509509 soda-core-vertica-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)     7672 2023-06-08 07:54:26.000000 soda-core-vertica-3.0.46/soda/data_sources/vertica_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:41.511992 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       62 2023-07-19 15:16:41.000000 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      275 2023-07-19 15:16:41.000000 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:41.000000 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       45 2023-07-19 15:16:41.000000 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:41.000000 soda-core-vertica-3.0.46/soda_core_vertica.egg-info/top_level.txt
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:41.512390 soda-core-vertica-3.0.46/tests/
--rw-r--r--   0 vijay      (501) staff       (20)       29 2023-06-08 07:54:26.000000 soda-core-vertica-3.0.46/tests/test_vertica.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:37:00.778998 soda-core-vertica-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       62 2023-07-31 08:37:00.778833 soda-core-vertica-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:37:00.779066 soda-core-vertica-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      409 2023-07-28 11:01:31.000000 soda-core-vertica-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:37:00.776842 soda-core-vertica-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:37:00.777310 soda-core-vertica-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     7672 2023-06-13 14:41:04.000000 soda-core-vertica-3.0.47/soda/data_sources/vertica_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:37:00.778410 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       62 2023-07-31 08:37:00.000000 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      253 2023-07-31 08:37:00.000000 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:37:00.000000 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       45 2023-07-31 08:37:00.000000 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:37:00.000000 soda-core-vertica-3.0.47/soda_core_vertica.egg-info/top_level.txt
```

### Comparing `soda-core-vertica-3.0.46/soda/data_sources/vertica_data_source.py` & `soda-core-vertica-3.0.47/soda/data_sources/vertica_data_source.py`

 * *Files identical despite different names*

