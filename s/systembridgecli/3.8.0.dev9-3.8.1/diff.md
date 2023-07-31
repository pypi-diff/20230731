# Comparing `tmp/systembridgecli-3.8.0.dev9.tar.gz` & `tmp/systembridgecli-3.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-3.8.0.dev9.tar", last modified: Tue Jul 18 14:37:05 2023, max compression
+gzip compressed data, was "systembridgecli-3.8.1.tar", last modified: Mon Jul 31 14:18:41 2023, max compression
```

## Comparing `systembridgecli-3.8.0.dev9.tar` & `systembridgecli-3.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:05.431375 systembridgecli-3.8.0.dev9/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:37:05.431375 systembridgecli-3.8.0.dev9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-18 14:36:29.000000 systembridgecli-3.8.0.dev9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:37:05.431375 systembridgecli-3.8.0.dev9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-18 14:36:29.000000 systembridgecli-3.8.0.dev9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:05.431375 systembridgecli-3.8.0.dev9/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 14:36:29.000000 systembridgecli-3.8.0.dev9/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-18 14:36:29.000000 systembridgecli-3.8.0.dev9/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-18 14:37:03.000000 systembridgecli-3.8.0.dev9/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:37:05.431375 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 14:37:05.000000 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-18 14:37:05.000000 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:37:05.000000 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-18 14:37:05.000000 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 14:37:05.000000 systembridgecli-3.8.0.dev9/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:41.914044 systembridgecli-3.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 14:18:41.914044 systembridgecli-3.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-31 14:18:02.000000 systembridgecli-3.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:18:41.914044 systembridgecli-3.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-31 14:18:02.000000 systembridgecli-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:41.914044 systembridgecli-3.8.1/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 14:18:02.000000 systembridgecli-3.8.1/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-07-31 14:18:02.000000 systembridgecli-3.8.1/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-31 14:18:02.000000 systembridgecli-3.8.1/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:18:41.914044 systembridgecli-3.8.1/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 14:18:41.000000 systembridgecli-3.8.1/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 14:18:41.000000 systembridgecli-3.8.1/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:18:41.000000 systembridgecli-3.8.1/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 14:18:41.000000 systembridgecli-3.8.1/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 14:18:41.000000 systembridgecli-3.8.1/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-3.8.0.dev9/pyproject.toml` & `systembridgecli-3.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.8.0.dev9/setup.py` & `systembridgecli-3.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-3.8.0.dev9/systembridgecli/__main__.py` & `systembridgecli-3.8.1/systembridgecli/__main__.py`

 * *Files identical despite different names*

