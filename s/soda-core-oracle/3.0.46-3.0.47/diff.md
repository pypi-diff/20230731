# Comparing `tmp/soda-core-oracle-3.0.46.tar.gz` & `tmp/soda-core-oracle-3.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-oracle-3.0.46.tar", last modified: Wed Jul 19 15:16:15 2023, max compression
+gzip compressed data, was "soda-core-oracle-3.0.47.tar", last modified: Mon Jul 31 08:36:31 2023, max compression
```

## Comparing `soda-core-oracle-3.0.46.tar` & `soda-core-oracle-3.0.47.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:15.690389 soda-core-oracle-3.0.46/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:15.690106 soda-core-oracle-3.0.46/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-19 15:16:15.690493 soda-core-oracle-3.0.46/setup.cfg
--rw-r--r--   0 vijay      (501) staff       (20)      634 2023-07-19 13:37:16.000000 soda-core-oracle-3.0.46/setup.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:15.687117 soda-core-oracle-3.0.46/soda/
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:15.687895 soda-core-oracle-3.0.46/soda/data_sources/
--rw-r--r--   0 vijay      (501) staff       (20)     9209 2023-06-08 07:54:26.000000 soda-core-oracle-3.0.46/soda/data_sources/oracle_data_source.py
-drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-19 15:16:15.689721 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/
--rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-19 15:16:15.000000 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/PKG-INFO
--rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-19 15:16:15.000000 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-19 15:16:15.000000 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 vijay      (501) staff       (20)       34 2023-07-19 15:16:15.000000 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/requires.txt
--rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-19 15:16:15.000000 soda-core-oracle-3.0.46/soda_core_oracle.egg-info/top_level.txt
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:31.489769 soda-core-oracle-3.0.47/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:31.489584 soda-core-oracle-3.0.47/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)       38 2023-07-31 08:36:31.489869 soda-core-oracle-3.0.47/setup.cfg
+-rw-r--r--   0 vijay      (501) staff       (20)      446 2023-07-28 11:01:31.000000 soda-core-oracle-3.0.47/setup.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:31.487887 soda-core-oracle-3.0.47/soda/
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:31.488290 soda-core-oracle-3.0.47/soda/data_sources/
+-rw-r--r--   0 vijay      (501) staff       (20)     9209 2023-06-13 14:41:04.000000 soda-core-oracle-3.0.47/soda/data_sources/oracle_data_source.py
+drwxr-xr-x   0 vijay      (501) staff       (20)        0 2023-07-31 08:36:31.489353 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/
+-rw-r--r--   0 vijay      (501) staff       (20)       61 2023-07-31 08:36:31.000000 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 vijay      (501) staff       (20)      247 2023-07-31 08:36:31.000000 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        1 2023-07-31 08:36:31.000000 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay      (501) staff       (20)       34 2023-07-31 08:36:31.000000 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/requires.txt
+-rw-r--r--   0 vijay      (501) staff       (20)        5 2023-07-31 08:36:31.000000 soda-core-oracle-3.0.47/soda_core_oracle.egg-info/top_level.txt
```

### Comparing `soda-core-oracle-3.0.46/soda/data_sources/oracle_data_source.py` & `soda-core-oracle-3.0.47/soda/data_sources/oracle_data_source.py`

 * *Files identical despite different names*

