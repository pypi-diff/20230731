# Comparing `tmp/surrealdb-beta-0.0.1.tar.gz` & `tmp/surrealdb-beta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealdb-beta-0.0.1.tar", last modified: Fri Jul 28 16:38:35 2023, max compression
+gzip compressed data, was "surrealdb-beta-0.0.2.tar", last modified: Mon Jul 31 09:38:20 2023, max compression
```

## Comparing `surrealdb-beta-0.0.1.tar` & `surrealdb-beta-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/connection_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/surrealdb/execution_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 16:38:09.000000 surrealdb-beta-0.0.1/surrealdb/execution_mixins/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:38:35.343861 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-28 16:38:35.000000 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-28 16:38:35.000000 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:38:35.000000 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:38:35.000000 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 16:38:35.000000 surrealdb-beta-0.0.1/surrealdb_beta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 09:37:47.000000 surrealdb-beta-0.0.2/surrealdb/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/connection_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb/execution_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/top_level.txt
```

### Comparing `surrealdb-beta-0.0.1/LICENSE` & `surrealdb-beta-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/README.md` & `surrealdb-beta-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/connection_interface.py` & `surrealdb-beta-0.0.2/surrealdb/connection_interface.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/execution_mixins/auth.py` & `surrealdb-beta-0.0.2/surrealdb/execution_mixins/auth.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/execution_mixins/create.py` & `surrealdb-beta-0.0.2/surrealdb/execution_mixins/create.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/execution_mixins/query.py` & `surrealdb-beta-0.0.2/surrealdb/execution_mixins/query.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/execution_mixins/set.py` & `surrealdb-beta-0.0.2/surrealdb/execution_mixins/set.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb/execution_mixins/update.py` & `surrealdb-beta-0.0.2/surrealdb/execution_mixins/update.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.1/surrealdb_beta.egg-info/SOURCES.txt` & `surrealdb-beta-0.0.2/surrealdb_beta.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
+surrealdb/VERSION.txt
 surrealdb/__init__.py
 surrealdb/connection_interface.py
 surrealdb/errors.py
 surrealdb/execution_mixins/__init__.py
 surrealdb/execution_mixins/auth.py
 surrealdb/execution_mixins/create.py
 surrealdb/execution_mixins/query.py
```

