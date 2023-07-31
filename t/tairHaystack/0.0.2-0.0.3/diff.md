# Comparing `tmp/tairhaystack-0.0.2.tar.gz` & `tmp/tairHaystack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tairhaystack-0.0.2.tar", last modified: Mon Jul 31 03:35:14 2023, max compression
+gzip compressed data, was "tairHaystack-0.0.3.tar", last modified: Mon Jul 31 05:51:29 2023, max compression
```

## Comparing `tairhaystack-0.0.2.tar` & `tairHaystack-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.796313 tairhaystack-0.0.2/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 03:35:14.796151 tairhaystack-0.0.2/PKG-INFO
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.794482 tairhaystack-0.0.2/document_stores/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 02:04:50.000000 tairhaystack-0.0.2/document_stores/__init__.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairhaystack-0.0.2/document_stores/errors.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairhaystack-0.0.2/document_stores/filter_utils.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 02:03:42.000000 tairhaystack-0.0.2/document_stores/tairvector.py
--rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 03:35:14.796359 tairhaystack-0.0.2/setup.cfg
--rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 03:34:12.000000 tairhaystack-0.0.2/setup.py
-drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 03:35:14.795956 tairhaystack-0.0.2/tairhaystack.egg-info/
--rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/PKG-INFO
--rw-r--r--   0 tanzhidong   (502) staff       (20)      303 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/SOURCES.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/dependency_links.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/requires.txt
--rw-r--r--   0 tanzhidong   (502) staff       (20)       16 2023-07-31 03:35:14.000000 tairhaystack-0.0.2/tairhaystack.egg-info/top_level.txt
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.042030 tairHaystack-0.0.3/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 05:51:29.041880 tairHaystack-0.0.3/PKG-INFO
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       38 2023-07-31 05:51:29.042075 tairHaystack-0.0.3/setup.cfg
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      969 2023-07-31 05:50:58.000000 tairHaystack-0.0.3/setup.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.038418 tairHaystack-0.0.3/tairHaystack/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       92 2023-07-31 02:04:29.000000 tairHaystack-0.0.3/tairHaystack/__init__.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.041189 tairHaystack-0.0.3/tairHaystack/document_stores/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      103 2023-07-31 02:04:50.000000 tairHaystack-0.0.3/tairHaystack/document_stores/__init__.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)     9925 2023-06-25 12:03:04.000000 tairHaystack-0.0.3/tairHaystack/document_stores/errors.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    36615 2023-07-12 02:42:17.000000 tairHaystack-0.0.3/tairHaystack/document_stores/filter_utils.py
+-rw-r--r--   0 tanzhidong   (502) staff       (20)    59708 2023-07-31 04:47:47.000000 tairHaystack-0.0.3/tairHaystack/document_stores/tairvector.py
+drwxr-xr-x   0 tanzhidong   (502) staff       (20)        0 2023-07-31 05:51:29.039564 tairHaystack-0.0.3/tairHaystack.egg-info/
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      548 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/PKG-INFO
+-rw-r--r--   0 tanzhidong   (502) staff       (20)      380 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/SOURCES.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)        1 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/dependency_links.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       14 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/requires.txt
+-rw-r--r--   0 tanzhidong   (502) staff       (20)       13 2023-07-31 05:51:29.000000 tairHaystack-0.0.3/tairHaystack.egg-info/top_level.txt
```

### Comparing `tairhaystack-0.0.2/PKG-INFO` & `tairHaystack-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tairhaystack
-Version: 0.0.2
+Name: tairHaystack
+Version: 0.0.3
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

### Comparing `tairhaystack-0.0.2/document_stores/errors.py` & `tairHaystack-0.0.3/tairHaystack/document_stores/errors.py`

 * *Files identical despite different names*

### Comparing `tairhaystack-0.0.2/document_stores/filter_utils.py` & `tairHaystack-0.0.3/tairHaystack/document_stores/filter_utils.py`

 * *Files identical despite different names*

### Comparing `tairhaystack-0.0.2/document_stores/tairvector.py` & `tairHaystack-0.0.3/tairHaystack/document_stores/tairvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import tair
 import numpy as np
 from tqdm.auto import tqdm
 
 from haystack.schema import Document, FilterType, Label, Answer, Span
 from haystack.document_stores import BaseDocumentStore
 
-from tairhaystack.document_stores.filter_utils import LogicalFilterClause
-from tairhaystack.document_stores.errors import TairDocumentStoreError, DuplicateDocumentError
+from tairHaystack.document_stores.filter_utils import LogicalFilterClause
+from tairHaystack.document_stores.errors import TairDocumentStoreError, DuplicateDocumentError
 from haystack.nodes.retriever import DenseRetriever
 
 
 logger = logging.getLogger(__name__)
 
 
 def _sanitize_index_name(index: Optional[str]) -> Optional[str]:
```

### Comparing `tairhaystack-0.0.2/setup.py` & `tairHaystack-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Tair vector database with Haystack'
 LONG_DESCRIPTION = 'An new integration of Tair vector database TairVector with Haystack by deepset.'
 
 # 配置
 setup(
-    # 名称必须匹配文件名 'tairhaystack'
-    name="tairhaystack",
+    # 名称必须匹配文件名 'tairHaystack'
+    name="tairHaystack",
     version=VERSION,
     author="Zhidong Tan",
     author_email="<2741986499@email.com>",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['haystack', 'tair'], # add any additional packages that
```

### Comparing `tairhaystack-0.0.2/tairhaystack.egg-info/PKG-INFO` & `tairHaystack-0.0.3/tairHaystack.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tairhaystack
-Version: 0.0.2
+Name: tairHaystack
+Version: 0.0.3
 Summary: Tair vector database with Haystack
 Author: Zhidong Tan
 Author-email: <2741986499@email.com>
 Keywords: tair,haystack
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 2
```

