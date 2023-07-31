# Comparing `tmp/acmanager-0.0.2.tar.gz` & `tmp/acmanager-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acmanager-0.0.2.tar", max compression
+gzip compressed data, was "acmanager-0.2.3.tar", max compression
```

## Comparing `acmanager-0.0.2.tar` & `acmanager-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       42 2023-07-31 19:30:29.430008 acmanager-0.0.2/acmanager/__init__.py
--rw-r--r--   0        0        0     4378 2023-07-31 19:26:05.940924 acmanager-0.0.2/acmanager/acmanager.py
--rw-r--r--   0        0        0     1862 2023-07-31 19:12:50.643024 acmanager-0.0.2/acmanager/remove.py
--rw-r--r--   0        0        0     1088 2023-07-12 15:30:30.441607 acmanager-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      616 2023-07-31 19:30:37.830338 acmanager-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       98 2023-07-31 19:11:23.048452 acmanager-0.0.2/README.md
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 acmanager-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-07-31 19:11:41.310679 acmanager-0.2.3/acmanager/__init__.py
+-rw-r--r--   0        0        0     2533 2023-07-31 19:12:24.458292 acmanager-0.2.3/acmanager/acmanager.py
+-rw-r--r--   0        0        0     1862 2023-07-31 19:12:50.643024 acmanager-0.2.3/acmanager/remove.py
+-rw-r--r--   0        0        0     1088 2023-07-12 15:30:30.441607 acmanager-0.2.3/LICENSE.txt
+-rw-r--r--   0        0        0      616 2023-07-31 19:16:13.763185 acmanager-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-07-31 19:11:23.048452 acmanager-0.2.3/README.md
+-rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 acmanager-0.2.3/PKG-INFO
```

### Comparing `acmanager-0.0.2/acmanager/remove.py` & `acmanager-0.2.3/acmanager/remove.py`

 * *Files identical despite different names*

### Comparing `acmanager-0.0.2/LICENSE.txt` & `acmanager-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acmanager-0.0.2/pyproject.toml` & `acmanager-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "acmanager"
-version = "0.0.2"
+version = "0.2.3"
 authors = ["Caio Souza <caios@blip.ai>"]
 
 description = "Manipulação das combinações do Assistente de Conteudo."
 readme = "README.md"
 
 
 classifiers = [
```

### Comparing `acmanager-0.0.2/PKG-INFO` & `acmanager-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acmanager
-Version: 0.0.2
+Version: 0.2.3
 Summary: Manipulação das combinações do Assistente de Conteudo.
 Author: Caio Souza
 Author-email: caios@blip.ai
 Requires-Python: >=3.6
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

