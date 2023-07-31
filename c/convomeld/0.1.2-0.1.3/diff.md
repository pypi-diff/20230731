# Comparing `tmp/convomeld-0.1.2.tar.gz` & `tmp/convomeld-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convomeld-0.1.2.tar", max compression
+gzip compressed data, was "convomeld-0.1.3.tar", max compression
```

## Comparing `convomeld-0.1.2.tar` & `convomeld-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    34336 2023-07-31 16:58:18.192409 convomeld-0.1.2/LICENSE.md
--rw-r--r--   0        0        0      226 2023-07-31 16:58:18.196410 convomeld-0.1.2/README.md
--rw-r--r--   0        0        0      834 2023-07-31 17:01:53.731839 convomeld-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/__init__.py
--rw-r--r--   0        0        0       36 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/__main__.py
--rw-r--r--   0        0        0     5408 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/api.py
--rw-r--r--   0        0        0     1223 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/cli.py
--rw-r--r--   0        0        0      102 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/constants.py
--rw-r--r--   0        0        0     1761 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/convocat.py
--rw-r--r--   0        0        0     1575 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/convoparse.py
--rw-r--r--   0        0        0     6868 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/data_factory.py
--rw-r--r--   0        0        0     2602 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/df_to_convograph.py
--rw-r--r--   0        0        0    17528 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/graph.py
--rw-r--r--   0        0        0     1268 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/matchers.py
--rw-r--r--   0        0        0    10570 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/merge.py
--rw-r--r--   0        0        0     2512 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/parsers.py
--rw-r--r--   0        0        0     2905 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/sorters.py
--rw-r--r--   0        0        0     8061 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/state.py
--rw-r--r--   0        0        0     5182 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/states.py
--rw-r--r--   0        0        0     6960 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/thread.py
--rw-r--r--   0        0        0     1278 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/utils.py
--rw-r--r--   0        0        0     8730 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/validators.py
--rw-r--r--   0        0        0     4239 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/xlsx_csv_parsers.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 convomeld-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34336 2023-07-31 16:58:18.192409 convomeld-0.1.3/LICENSE.md
+-rw-r--r--   0        0        0      226 2023-07-31 16:58:18.196410 convomeld-0.1.3/README.md
+-rw-r--r--   0        0        0      834 2023-07-31 17:15:07.998709 convomeld-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/__init__.py
+-rw-r--r--   0        0        0       36 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/__main__.py
+-rw-r--r--   0        0        0     5408 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/api.py
+-rw-r--r--   0        0        0     1223 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/cli.py
+-rw-r--r--   0        0        0      102 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/constants.py
+-rw-r--r--   0        0        0     1761 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/convocat.py
+-rw-r--r--   0        0        0     1575 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/convoparse.py
+-rw-r--r--   0        0        0     6868 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/data_factory.py
+-rw-r--r--   0        0        0     2602 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/df_to_convograph.py
+-rw-r--r--   0        0        0    17528 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/graph.py
+-rw-r--r--   0        0        0     1268 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/matchers.py
+-rw-r--r--   0        0        0    10570 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/merge.py
+-rw-r--r--   0        0        0     2512 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/parsers.py
+-rw-r--r--   0        0        0     2905 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/sorters.py
+-rw-r--r--   0        0        0     8061 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/state.py
+-rw-r--r--   0        0        0     5182 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/states.py
+-rw-r--r--   0        0        0     6960 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/thread.py
+-rw-r--r--   0        0        0     1278 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/utils.py
+-rw-r--r--   0        0        0     8730 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/validators.py
+-rw-r--r--   0        0        0     4239 2023-07-31 16:58:18.212411 convomeld-0.1.3/src/convomeld/xlsx_csv_parsers.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 convomeld-0.1.3/PKG-INFO
```

### Comparing `convomeld-0.1.2/LICENSE.md` & `convomeld-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/pyproject.toml` & `convomeld-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "convomeld"
-version = "0.1.2"
+version = "0.1.3"
 description = "Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)"
 authors = [
     "Ruslan Borysov <borysov.ruslan98@gmail.com>",
     "Hobson Lane <hobson@tangibleai.com>",
     "Vlad Snisar <vlad@tangibleai.com>",
     "Cetin Czeckr <cetin@tangibleai.com>",
 ]
```

### Comparing `convomeld-0.1.2/src/convomeld/api.py` & `convomeld-0.1.3/src/convomeld/api.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/cli.py` & `convomeld-0.1.3/src/convomeld/cli.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/convocat.py` & `convomeld-0.1.3/src/convomeld/convocat.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/convoparse.py` & `convomeld-0.1.3/src/convomeld/convoparse.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/data_factory.py` & `convomeld-0.1.3/src/convomeld/data_factory.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/df_to_convograph.py` & `convomeld-0.1.3/src/convomeld/df_to_convograph.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/graph.py` & `convomeld-0.1.3/src/convomeld/graph.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/matchers.py` & `convomeld-0.1.3/src/convomeld/matchers.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/merge.py` & `convomeld-0.1.3/src/convomeld/merge.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/parsers.py` & `convomeld-0.1.3/src/convomeld/parsers.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/sorters.py` & `convomeld-0.1.3/src/convomeld/sorters.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/state.py` & `convomeld-0.1.3/src/convomeld/state.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/states.py` & `convomeld-0.1.3/src/convomeld/states.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/thread.py` & `convomeld-0.1.3/src/convomeld/thread.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/utils.py` & `convomeld-0.1.3/src/convomeld/utils.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/validators.py` & `convomeld-0.1.3/src/convomeld/validators.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/src/convomeld/xlsx_csv_parsers.py` & `convomeld-0.1.3/src/convomeld/xlsx_csv_parsers.py`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.2/PKG-INFO` & `convomeld-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convomeld
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)
 License: AGPL-3.0-or-later
 Author: Ruslan Borysov
 Author-email: borysov.ruslan98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

