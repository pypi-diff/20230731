# Comparing `tmp/salinic-0.1.0.tar.gz` & `tmp/salinic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "salinic-0.1.0.tar", max compression
+gzip compressed data, was "salinic-0.2.0.tar", max compression
```

## Comparing `salinic-0.1.0.tar` & `salinic-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10226 2023-07-30 07:45:25.743050 salinic-0.1.0/LICENSE
--rw-r--r--   0        0        0     1468 2023-07-30 07:45:25.743050 salinic-0.1.0/README.md
--rw-r--r--   0        0        0      367 2023-07-30 07:45:25.743050 salinic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      176 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/__init__.py
--rw-r--r--   0        0        0      438 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/engine.py
--rw-r--r--   0        0        0      285 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/field.py
--rw-r--r--   0        0        0      554 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/schema.py
--rw-r--r--   0        0        0      228 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/search.py
--rw-r--r--   0        0        0      118 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/search_query.py
--rw-r--r--   0        0        0     3213 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/session.py
--rw-r--r--   0        0        0       67 2023-07-30 07:45:25.743050 salinic-0.1.0/salinic/utils.py
--rw-r--r--   0        0        0     1818 1970-01-01 00:00:00.000000 salinic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10226 2023-07-31 05:34:39.706490 salinic-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1624 2023-07-31 05:34:39.706490 salinic-0.2.0/README.md
+-rw-r--r--   0        0        0      464 2023-07-31 05:34:39.706490 salinic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/__init__.py
+-rw-r--r--   0        0        0      344 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/engine.py
+-rw-r--r--   0        0        0      285 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/field.py
+-rw-r--r--   0        0        0      534 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/schema.py
+-rw-r--r--   0        0        0      228 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/search.py
+-rw-r--r--   0        0        0      118 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/search_query.py
+-rw-r--r--   0        0        0     3213 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/session.py
+-rw-r--r--   0        0        0       67 2023-07-31 05:34:39.706490 salinic-0.2.0/salinic/utils.py
+-rw-r--r--   0        0        0     2082 1970-01-01 00:00:00.000000 salinic-0.2.0/PKG-INFO
```

### Comparing `salinic-0.1.0/LICENSE` & `salinic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salinic-0.1.0/README.md` & `salinic-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: salinic
+Version: 0.2.0
+Summary: Search abstraction layer
+Author: Eugen Ciur
+Author-email: eugen@papermerge.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=2.1.1,<3.0.0)
+Requires-Dist: xapianpy (>=1.4.22.post2305071405,<2.0.0)
+Description-Content-Type: text/markdown
+
+[![Tests](https://github.com/papermerge/salinic/actions/workflows/tests.yml/badge.svg)](https://github.com/papermerge/salinic/actions/workflows/tests.yml)
+
 # Salinic
 
 Salinic - provides modular search. It features a unified, familiar API that
 allows you to plug in different search backends.
 Currently it supports only Xapian backend.
 
 
@@ -51,7 +67,8 @@
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
         sq = Search(IndexEntity).query(" your query string ")
 
         for found in session.exec(sq):
             print(found)  # found is instance of IndexEntity
+
```

### Comparing `salinic-0.1.0/salinic/schema.py` & `salinic-0.2.0/salinic/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from pydantic import BaseModel, model_serializer
-from pydantic import ConfigDict
+from pydantic import BaseModel, ConfigDict, model_serializer
 
 from .field import Field
 
 
 class Schema(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
```

### Comparing `salinic-0.1.0/salinic/session.py` & `salinic-0.2.0/salinic/session.py`

 * *Files identical despite different names*

### Comparing `salinic-0.1.0/PKG-INFO` & `salinic-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,8 @@
-Metadata-Version: 2.1
-Name: salinic
-Version: 0.1.0
-Summary: Search abstraction layer
-Author: Eugen Ciur
-Author-email: eugen@papermerge.com
-Requires-Python: >=3.11,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=2.1.1,<3.0.0)
-Description-Content-Type: text/markdown
+[![Tests](https://github.com/papermerge/salinic/actions/workflows/tests.yml/badge.svg)](https://github.com/papermerge/salinic/actions/workflows/tests.yml)
 
 # Salinic
 
 Salinic - provides modular search. It features a unified, familiar API that
 allows you to plug in different search backends.
 Currently it supports only Xapian backend.
 
@@ -63,8 +53,7 @@
         engine = create_engine("xapian:////search_index")
         session = Session(engine)
 
         sq = Search(IndexEntity).query(" your query string ")
 
         for found in session.exec(sq):
             print(found)  # found is instance of IndexEntity
-
```

