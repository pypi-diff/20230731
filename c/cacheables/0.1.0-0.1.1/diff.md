# Comparing `tmp/cacheables-0.1.0.tar.gz` & `tmp/cacheables-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cacheables-0.1.0.tar", max compression
+gzip compressed data, was "cacheables-0.1.1.tar", max compression
```

## Comparing `cacheables-0.1.0.tar` & `cacheables-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     5481 2023-07-31 17:17:08.298558 cacheables-0.1.0/README.md
--rw-r--r--   0        0        0       29 2023-07-31 17:13:55.578270 cacheables-0.1.0/cacheables/__init__.py
--rw-r--r--   0        0        0    11594 2023-07-26 14:12:06.906854 cacheables-0.1.0/cacheables/core.py
--rw-r--r--   0        0        0      343 2023-07-31 17:17:03.058614 cacheables-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5808 1970-01-01 00:00:00.000000 cacheables-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5481 2023-07-31 17:17:08.298558 cacheables-0.1.1/README.md
+-rw-r--r--   0        0        0       29 2023-07-31 17:13:55.578270 cacheables-0.1.1/cacheables/__init__.py
+-rw-r--r--   0        0        0    11594 2023-07-26 14:12:06.906854 cacheables-0.1.1/cacheables/core.py
+-rw-r--r--   0        0        0      398 2023-07-31 18:13:54.384429 cacheables-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 cacheables-0.1.1/PKG-INFO
```

### Comparing `cacheables-0.1.0/README.md` & `cacheables-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cacheables-0.1.0/cacheables/core.py` & `cacheables-0.1.1/cacheables/core.py`

 * *Files identical despite different names*

### Comparing `cacheables-0.1.0/PKG-INFO` & `cacheables-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: cacheables
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
+Home-page: https://github.com/thomelane/cacheables
 Author: Thom Lane
 Author-email: thom.e.lane@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Project-URL: Repository, https://github.com/thomelane/cacheables
 Description-Content-Type: text/markdown
 
 # Cacheables
 
 Cacheables is a module that make it easy to cache function results. You'll be
 able to experiment faster (by avoiding repeated work) and keep track of your
 experiments with out-of-the-box versioning.
```

