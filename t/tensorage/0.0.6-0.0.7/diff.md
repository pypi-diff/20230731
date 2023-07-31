# Comparing `tmp/tensorage-0.0.6.tar.gz` & `tmp/tensorage-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorage-0.0.6.tar", last modified: Mon Jul 31 05:26:22 2023, max compression
+gzip compressed data, was "tensorage-0.0.7.tar", last modified: Mon Jul 31 09:54:07 2023, max compression
```

## Comparing `tensorage-0.0.6.tar` & `tensorage-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-31 05:26:07.000000 tensorage-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 05:26:07.000000 tensorage-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 05:26:22.053734 tensorage-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 05:26:07.000000 tensorage-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-31 05:26:07.000000 tensorage-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 05:26:22.053734 tensorage-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-31 05:26:07.000000 tensorage-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/tensorage/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/db_init.py
--rw-r--r--   0 runner    (1001) docker     (122)     2619 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/session.py
--rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/store.py
--rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-31 05:26:07.000000 tensorage-0.0.6/tensorage/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 05:26:22.053734 tensorage-0.0.6/tensorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-31 05:26:22.000000 tensorage-0.0.6/tensorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.562017 tensorage-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-07-31 09:53:57.000000 tensorage-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 09:53:57.000000 tensorage-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 09:54:07.562017 tensorage-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-31 09:53:57.000000 tensorage-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-31 09:53:57.000000 tensorage-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 09:54:07.562017 tensorage-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-07-31 09:53:57.000000 tensorage-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.558017 tensorage-0.0.7/tensorage/
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2388 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/db_init.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7351 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/store.py
+-rw-r--r--   0 runner    (1001) docker     (122)      155 2023-07-31 09:53:57.000000 tensorage-0.0.7/tensorage/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:54:07.562017 tensorage-0.0.7/tensorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      364 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-31 09:54:07.000000 tensorage-0.0.7/tensorage.egg-info/top_level.txt
```

### Comparing `tensorage-0.0.6/LICENSE` & `tensorage-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.6/setup.py` & `tensorage-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.6/tensorage/db_init.py` & `tensorage-0.0.7/tensorage/db_init.py`

 * *Files identical despite different names*

### Comparing `tensorage-0.0.6/tensorage/store.py` & `tensorage-0.0.7/tensorage/store.py`

 * *Files identical despite different names*

