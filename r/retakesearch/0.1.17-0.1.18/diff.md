# Comparing `tmp/retakesearch-0.1.17.tar.gz` & `tmp/retakesearch-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.1.17.tar", max compression
+gzip compressed data, was "retakesearch-0.1.18.tar", max compression
```

## Comparing `retakesearch-0.1.17.tar` & `retakesearch-0.1.18.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-29 02:49:19.890655 retakesearch-0.1.17/README.md
--rw-r--r--   0        0        0      412 2023-07-29 02:49:37.451007 retakesearch-0.1.17/pyproject.toml
--rw-r--r--   0        0        0      174 2023-07-29 02:49:19.890655 retakesearch-0.1.17/retakesearch/__init__.py
--rw-r--r--   0        0        0     1277 2023-07-29 02:49:19.890655 retakesearch-0.1.17/retakesearch/client.py
--rw-r--r--   0        0        0     3204 2023-07-29 02:49:19.890655 retakesearch-0.1.17/retakesearch/index.py
--rw-r--r--   0        0        0      159 2023-07-29 02:49:19.890655 retakesearch-0.1.17/retakesearch/search.py
--rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.17/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 19:13:46.330360 retakesearch-0.1.18/README.md
+-rw-r--r--   0        0        0      412 2023-07-31 19:14:06.138453 retakesearch-0.1.18/pyproject.toml
+-rw-r--r--   0        0        0      174 2023-07-31 19:13:46.330360 retakesearch-0.1.18/retakesearch/__init__.py
+-rw-r--r--   0        0        0     1818 2023-07-31 19:13:46.330360 retakesearch-0.1.18/retakesearch/client.py
+-rw-r--r--   0        0        0     3536 2023-07-31 19:13:46.330360 retakesearch-0.1.18/retakesearch/index.py
+-rw-r--r--   0        0        0      159 2023-07-31 19:13:46.330360 retakesearch-0.1.18/retakesearch/search.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.18/PKG-INFO
```

### Comparing `retakesearch-0.1.17/PKG-INFO` & `retakesearch-0.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.1.17
+Version: 0.1.18
 Summary: Open Source Neural Search Engine Python Client
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

