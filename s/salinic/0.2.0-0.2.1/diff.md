# Comparing `tmp/salinic-0.2.0.tar.gz` & `tmp/salinic-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.2.0.tar", max compression
+gzip compressed data, was "salinic-0.2.1.tar", max compression
```

## Comparing `salinic-0.2.0.tar` & `salinic-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10226 2023-07-31 05:34:39.706490 salinic-0.2.0/LICENSE
--rw-r--r--   0        0        0     1624 2023-07-31 05:34:39.706490 salinic-0.2.0/README.md
--rw-r--r--   0        0        0      464 2023-07-31 05:34:39.706490 salinic-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/__init__.py
--rw-r--r--   0        0        0      344 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/engine.py
--rw-r--r--   0        0        0      285 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/field.py
--rw-r--r--   0        0        0      534 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/schema.py
--rw-r--r--   0        0        0      228 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/search.py
--rw-r--r--   0        0        0      118 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/search_query.py
--rw-r--r--   0        0        0     3213 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/session.py
--rw-r--r--   0        0        0       67 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/utils.py
--rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 salinic-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-07-31 05:38:15.927182 salinic-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1624 2023-07-31 05:38:15.927182 salinic-0.2.1/README.md
+-rw-r--r--   0        0        0      464 2023-07-31 05:38:15.927182 salinic-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/__init__.py
+-rw-r--r--   0        0        0      344 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/engine.py
+-rw-r--r--   0        0        0      285 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/field.py
+-rw-r--r--   0        0        0      534 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/schema.py
+-rw-r--r--   0        0        0      228 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/search.py
+-rw-r--r--   0        0        0      118 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/search_query.py
+-rw-r--r--   0        0        0     3213 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/session.py
+-rw-r--r--   0        0        0       67 2023-07-31 05:38:15.927182 salinic-0.2.1/salinic/utils.py
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 salinic-0.2.1/PKG-INFO
```

### Comparing `salinic-0.2.0/LICENSE` & `salinic-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.2.0/README.md` & `salinic-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `salinic-0.2.0/salinic/schema.py` & `salinic-0.2.1/salinic/schema.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.0/salinic/session.py` & `salinic-0.2.1/salinic/session.py`

 * *Files identical despite different names*

### Comparing `salinic-0.2.0/PKG-INFO` & `salinic-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salinic
-Version: 0.2.0
+Version: 0.2.1
 Summary: Search abstraction layer
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

