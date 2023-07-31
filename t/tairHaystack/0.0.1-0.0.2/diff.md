# Comparing `tmp/tairhaystack-0.0.1.tar.gz` & `tmp/tairhaystack-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tairhaystack-0.0.1.tar", last modified: Mon Jul 31 02:13:23 2023, max compression
+gzip compressed data, was "tairhaystack-0.0.2.tar", last modified: Mon Jul 31 03:35:14 2023, max compression
```

## Comparing `tairhaystack-0.0.1.tar` & `tairhaystack-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 02:13:23.772782 tairhaystack-0.0.1/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 02:13:23.772532 tairhaystack-0.0.1/PKG-INFO
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 02:13:23.770434 tairhaystack-0.0.1/document_stores/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 02:04:50.000000 tairhaystack-0.0.1/document_stores/__init__.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairhaystack-0.0.1/document_stores/errors.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairhaystack-0.0.1/document_stores/filter_utils.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 02:03:42.000000 tairhaystack-0.0.1/document_stores/tairvector.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 02:13:23.772889 tairhaystack-0.0.1/setup.cfg
--rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 02:10:17.000000 tairhaystack-0.0.1/setup.py
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 02:13:23.772051 tairhaystack-0.0.1/tairhaystack.egg-info/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 02:13:23.000000 tairhaystack-0.0.1/tairhaystack.egg-info/PKG-INFO
--rw-r--r--   0 tanzhidong   (502) staff       (20)      303 2023-07-31 02:13:23.000000 tairhaystack-0.0.1/tairhaystack.egg-info/SOURCES.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 02:13:23.000000 tairhaystack-0.0.1/tairhaystack.egg-info/dependency_links.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 02:13:23.000000 tairhaystack-0.0.1/tairhaystack.egg-info/requires.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       16 2023-07-31 02:13:23.000000 tairhaystack-0.0.1/tairhaystack.egg-info/top_level.txt
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.796313 tairhaystack-0.0.2/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 03:35:14.796151 tairhaystack-0.0.2/PKG-INFO
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.794482 tairhaystack-0.0.2/document_stores/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 02:04:50.000000 tairhaystack-0.0.2/document_stores/__init__.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairhaystack-0.0.2/document_stores/errors.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairhaystack-0.0.2/document_stores/filter_utils.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 02:03:42.000000 tairhaystack-0.0.2/document_stores/tairvector.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 03:35:14.796359 tairhaystack-0.0.2/setup.cfg
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 03:34:12.000000 tairhaystack-0.0.2/setup.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.795956 tairhaystack-0.0.2/tairhaystack.egg-info/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/PKG-INFO
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      303 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/SOURCES.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/dependency_links.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/requires.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       16 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/top_level.txt
```

### Comparing `tairhaystack-0.0.1/PKG-INFO` & `tairhaystack-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tairhaystack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

### Comparing `tairhaystack-0.0.1/document_stores/errors.py` & `tairhaystack-0.0.2/document_stores/errors.py`

 * *Files identical despite different names*

### Comparing `tairhaystack-0.0.1/document_stores/filter_utils.py` & `tairhaystack-0.0.2/document_stores/filter_utils.py`

 * *Files identical despite different names*

### Comparing `tairhaystack-0.0.1/document_stores/tairvector.py` & `tairhaystack-0.0.2/document_stores/tairvector.py`

 * *Files identical despite different names*

### Comparing `tairhaystack-0.0.1/setup.py` & `tairhaystack-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Tair vector database with Haystack'
 LONG_DESCRIPTION = 'An new integration of Tair vector database TairVector with Haystack by deepset.'
 
 # 配置
 setup(
     # 名称必须匹配文件名 'tairhaystack'
     name="tairhaystack",
```

### Comparing `tairhaystack-0.0.1/tairhaystack.egg-info/PKG-INFO` & `tairhaystack-0.0.2/tairhaystack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tairhaystack
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

