# Comparing `tmp/open_source_sdk-0.0.1.tar.gz` & `tmp/open_source_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_source_sdk-0.0.1.tar", last modified: Mon Jul 31 09:56:08 2023, max compression
+gzip compressed data, was "open_source_sdk-0.0.2.tar", last modified: Mon Jul 31 11:38:42 2023, max compression
```

## Comparing `open_source_sdk-0.0.1.tar` & `open_source_sdk-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:56:08.624548 open_source_sdk-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-31 09:56:08.624548 open_source_sdk-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:56:08.620548 open_source_sdk-0.0.1/open_source_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/open_source_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/open_source_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/open_source_sdk/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:56:08.620548 open_source_sdk-0.0.1/open_source_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-31 09:56:08.000000 open_source_sdk-0.0.1/open_source_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 09:56:08.000000 open_source_sdk-0.0.1/open_source_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:56:08.000000 open_source_sdk-0.0.1/open_source_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 09:56:08.000000 open_source_sdk-0.0.1/open_source_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 09:56:08.000000 open_source_sdk-0.0.1/open_source_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/requirements_plot.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:56:08.624548 open_source_sdk-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:56:08.624548 open_source_sdk-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 09:55:17.000000 open_source_sdk-0.0.1/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/open_source_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/open_source_sdk/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/open_source_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 11:38:42.000000 open_source_sdk-0.0.2/open_source_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_plot.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:38:42.125261 open_source_sdk-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-31 11:38:12.000000 open_source_sdk-0.0.2/tests/test_demo.py
```

### Comparing `open_source_sdk-0.0.1/LICENSE` & `open_source_sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open_source_sdk-0.0.1/pyproject.toml` & `open_source_sdk-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 [project]
 name = "open_source_sdk"
 authors = [
     {name = "Open Civil Engineering"},
 ]
 maintainers= [
     {name = "Enrique García Méndez", email = "enriquegarcia@live.nl"},
-    {name = "Johan Tuls", email = "johan.tuls@bam.com"},
-    {name = "Wichard Bron", email = "wichard.bron@wsp.com"},
-    {name = "Sina Zel taat", email = "sina.zeltaat@wsp.com"},
+    # {name = "Johan Tuls", email = "johan.tuls@bam.com"},
+    # {name = "Wichard Bron", email = "wichard.bron@wsp.com"},
+    # {name = "Sina Zel taat", email = "sina.zeltaat@wsp.com"},
 ]
 description = "Template for the Python Civil Engineering library."
 requires-python = ">=3.10"
 keywords = ["Civil engineering", "Material properties", "Structural engineering", "Structural analysis", "Eurocodes", "Dutch building codes"]
 license = {text = "LGPL-2.1"}
 classifiers = [
     "Topic :: Scientific/Engineering",
```

