# Comparing `tmp/tairHaystack-0.0.3.tar.gz` & `tmp/tairHaystack-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tairHaystack-0.0.3.tar", last modified: Mon Jul 31 05:51:29 2023, max compression
+gzip compressed data, was "tairHaystack-1.0.0.tar", last modified: Mon Jul 31 06:01:35 2023, max compression
```

## Comparing `tairHaystack-0.0.3.tar` & `tairHaystack-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.042030 tairHaystack-0.0.3/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 05:51:29.041880 tairHaystack-0.0.3/PKG-INFO
--rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 05:51:29.042075 tairHaystack-0.0.3/setup.cfg
--rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 05:50:58.000000 tairHaystack-0.0.3/setup.py
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.038418 tairHaystack-0.0.3/tairHaystack/
--rw-r--r--   0 tanzhidong   (502) staff       (20)       92 2023-07-31 02:04:29.000000 tairHaystack-0.0.3/tairHaystack/__init__.py
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.041189 tairHaystack-0.0.3/tairHaystack/document_stores/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 02:04:50.000000 tairHaystack-0.0.3/tairHaystack/document_stores/__init__.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairHaystack-0.0.3/tairHaystack/document_stores/errors.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairHaystack-0.0.3/tairHaystack/document_stores/filter_utils.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 04:47:47.000000 tairHaystack-0.0.3/tairHaystack/document_stores/tairvector.py
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.039564 tairHaystack-0.0.3/tairHaystack.egg-info/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/PKG-INFO
--rw-r--r--   0 tanzhidong   (502) staff       (20)      380 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/SOURCES.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/dependency_links.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/requires.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       13 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/top_level.txt
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 06:01:35.613170 tairHaystack-1.0.0/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 06:01:35.612998 tairHaystack-1.0.0/PKG-INFO
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 06:01:35.613227 tairHaystack-1.0.0/setup.cfg
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 06:01:24.000000 tairHaystack-1.0.0/setup.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 06:01:35.609592 tairHaystack-1.0.0/tairHaystack/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       92 2023-07-31 05:57:22.000000 tairHaystack-1.0.0/tairHaystack/__init__.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 06:01:35.612496 tairHaystack-1.0.0/tairHaystack/document_stores/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 05:57:22.000000 tairHaystack-1.0.0/tairHaystack/document_stores/__init__.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairHaystack-1.0.0/tairHaystack/document_stores/errors.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairHaystack-1.0.0/tairHaystack/document_stores/filter_utils.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 04:47:47.000000 tairHaystack-1.0.0/tairHaystack/document_stores/tairvector.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 06:01:35.610610 tairHaystack-1.0.0/tairHaystack.egg-info/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 06:01:35.000000 tairHaystack-1.0.0/tairHaystack.egg-info/PKG-INFO
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      380 2023-07-31 06:01:35.000000 tairHaystack-1.0.0/tairHaystack.egg-info/SOURCES.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 06:01:35.000000 tairHaystack-1.0.0/tairHaystack.egg-info/dependency_links.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 06:01:35.000000 tairHaystack-1.0.0/tairHaystack.egg-info/requires.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       13 2023-07-31 06:01:35.000000 tairHaystack-1.0.0/tairHaystack.egg-info/top_level.txt
```

### Comparing `tairHaystack-0.0.3/PKG-INFO` & `tairHaystack-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tairHaystack
-Version: 0.0.3
+Version: 1.0.0
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

### Comparing `tairHaystack-0.0.3/setup.py` & `tairHaystack-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '1.0.0'
 DESCRIPTION = 'Tair vector database with Haystack'
 LONG_DESCRIPTION = 'An new integration of Tair vector database TairVector with Haystack by deepset.'
 
 # 配置
 setup(
     # 名称必须匹配文件名 'tairHaystack'
     name="tairHaystack",
```

### Comparing `tairHaystack-0.0.3/tairHaystack/document_stores/errors.py` & `tairHaystack-1.0.0/tairHaystack/document_stores/errors.py`

 * *Files identical despite different names*

### Comparing `tairHaystack-0.0.3/tairHaystack/document_stores/filter_utils.py` & `tairHaystack-1.0.0/tairHaystack/document_stores/filter_utils.py`

 * *Files identical despite different names*

### Comparing `tairHaystack-0.0.3/tairHaystack/document_stores/tairvector.py` & `tairHaystack-1.0.0/tairHaystack/document_stores/tairvector.py`

 * *Files identical despite different names*

### Comparing `tairHaystack-0.0.3/tairHaystack.egg-info/PKG-INFO` & `tairHaystack-1.0.0/tairHaystack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tairHaystack
-Version: 0.0.3
+Version: 1.0.0
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

