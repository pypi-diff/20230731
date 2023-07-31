# Comparing `tmp/formal-sdk-0.9.0.tar.gz` & `tmp/formal-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-0.9.0.tar", last modified: Thu Jun  8 23:00:11 2023, max compression
+gzip compressed data, was "formal-sdk-1.0.0.tar", last modified: Mon Jul 31 16:07:49 2023, max compression
```

## Comparing `formal-sdk-0.9.0.tar` & `formal-sdk-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/src/formal_sdk/datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 22:59:53.000000 formal-sdk-0.9.0/src/formal_sdk/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:00:11.769542 formal-sdk-0.9.0/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-08 23:00:11.000000 formal-sdk-0.9.0/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-08 23:00:11.000000 formal-sdk-0.9.0/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:00:11.000000 formal-sdk-0.9.0/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 23:00:11.000000 formal-sdk-0.9.0/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 23:00:11.000000 formal-sdk-0.9.0/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-31 16:07:33.000000 formal-sdk-1.0.0/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:07:49.177026 formal-sdk-1.0.0/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 16:07:49.000000 formal-sdk-1.0.0/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-0.9.0/LICENSE` & `formal-sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.9.0/pyproject.toml` & `formal-sdk-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "0.9.0"
+version = "1.0.0"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
@@ -21,8 +21,8 @@
   'requests >= 2.26.0',
 ]
 
 # [tool.setuptools.packages.find]
 # where = ["src"]
 
 [project.urls]
-"Homepage" = "https://github.com/formalco"
+"Homepage" = "https://github.com/formalco"
```

