# Comparing `tmp/aequitas-core-1.0.0.tar.gz` & `tmp/aequitas-core-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aequitas-core-1.0.0.tar", last modified: Fri Jul 28 10:20:24 2023, max compression
+gzip compressed data, was "aequitas-core-1.1.0.tar", last modified: Mon Jul 31 14:13:37 2023, max compression
```

## Comparing `aequitas-core-1.0.0.tar` & `aequitas-core-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:20:24.894214 aequitas-core-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-28 10:20:24.894214 aequitas-core-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:20:24.890214 aequitas-core-1.0.0/aequitas/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-28 10:20:01.000000 aequitas-core-1.0.0/aequitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/aequitas/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:20:24.890214 aequitas-core-1.0.0/aequitas/core/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/aequitas/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:20:24.894214 aequitas-core-1.0.0/aequitas_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-28 10:20:24.000000 aequitas-core-1.0.0/aequitas_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:20:24.894214 aequitas-core-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-28 10:19:42.000000 aequitas-core-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/aequitas/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-31 14:13:14.000000 aequitas-core-1.1.0/aequitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/aequitas/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/aequitas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/aequitas/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/aequitas/core/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/aequitas_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/aequitas_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/aequitas_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/aequitas_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:13:36.000000 aequitas-core-1.1.0/aequitas_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/aequitas_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 14:13:37.000000 aequitas-core-1.1.0/aequitas_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.120054 aequitas-core-1.1.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:13:37.124054 aequitas-core-1.1.0/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-31 14:12:47.000000 aequitas-core-1.1.0/test/core/test_metrics.py
```

### Comparing `aequitas-core-1.0.0/LICENSE` & `aequitas-core-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aequitas-core-1.0.0/PKG-INFO` & `aequitas-core-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aequitas-core
-Version: 1.0.0
+Version: 1.1.0
 Summary: Aequitas core library
 Home-page: https://github.com/aequitas-aod/core-lib
 Author: Giovanni Ciatto
 Author-email: giovanni.ciatto@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/aequitas-aod/core-lib/issues
 Project-URL: Source, https://github.com/aequitas-aod/core-lib
```

### Comparing `aequitas-core-1.0.0/aequitas_core.egg-info/PKG-INFO` & `aequitas-core-1.1.0/aequitas_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aequitas-core
-Version: 1.0.0
+Version: 1.1.0
 Summary: Aequitas core library
 Home-page: https://github.com/aequitas-aod/core-lib
 Author: Giovanni Ciatto
 Author-email: giovanni.ciatto@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/aequitas-aod/core-lib/issues
 Project-URL: Source, https://github.com/aequitas-aod/core-lib
```

### Comparing `aequitas-core-1.0.0/setup.py` & `aequitas-core-1.1.0/setup.py`

 * *Files identical despite different names*

