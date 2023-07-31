# Comparing `tmp/forestadmin_datasource_sqlalchemy-1.0.0b3.tar.gz` & `tmp/forestadmin_datasource_sqlalchemy-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.0.0b3.tar", max compression
+gzip compressed data, was "forestadmin_datasource_sqlalchemy-1.0.0b4.tar", max compression
```

## Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3.tar` & `forestadmin_datasource_sqlalchemy-1.0.0b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/README.md
--rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11179 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/collections.py
--rw-r--r--   0        0        0     3045 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/datasource.py
--rw-r--r--   0        0        0      612 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/exceptions.py
--rw-r--r--   0        0        0     1923 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/interfaces.py
--rw-r--r--   0        0        0        0 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/__init__.py
--rw-r--r--   0        0        0     5956 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/aggregation.py
--rw-r--r--   0        0        0     6235 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/model_converter.py
--rw-r--r--   0        0        0    10207 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/query_factory.py
--rw-r--r--   0        0        0     2943 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
--rw-r--r--   0        0        0      519 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/relationships.py
--rw-r--r--   0        0        0     7029 2023-07-27 12:28:25.784370 forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/type_converter.py
--rw-r--r--   0        0        0     1808 2023-07-27 12:28:44.964527 forestadmin_datasource_sqlalchemy-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11179 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/collections.py
+-rw-r--r--   0        0        0     3045 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/datasource.py
+-rw-r--r--   0        0        0      612 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/exceptions.py
+-rw-r--r--   0        0        0     1923 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/interfaces.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/__init__.py
+-rw-r--r--   0        0        0     5956 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/aggregation.py
+-rw-r--r--   0        0        0     6235 2023-07-31 15:37:07.294435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/model_converter.py
+-rw-r--r--   0        0        0    10207 2023-07-31 15:37:07.298435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/query_factory.py
+-rw-r--r--   0        0        0     2943 2023-07-31 15:37:07.298435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/record_serializer.py
+-rw-r--r--   0        0        0      519 2023-07-31 15:37:07.298435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/relationships.py
+-rw-r--r--   0        0        0     7029 2023-07-31 15:37:07.298435 forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/type_converter.py
+-rw-r--r--   0        0        0     1808 2023-07-31 15:37:32.366605 forestadmin_datasource_sqlalchemy-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 forestadmin_datasource_sqlalchemy-1.0.0b4/PKG-INFO
```

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/collections.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/datasource.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/exceptions.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/interfaces.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/interfaces.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/aggregation.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/model_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/model_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/query_factory.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/query_factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/record_serializer.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/record_serializer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/relationships.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/relationships.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/forestadmin/datasource_sqlalchemy/utils/type_converter.py` & `forestadmin_datasource_sqlalchemy-1.0.0b4/forestadmin/datasource_sqlalchemy/utils/type_converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/pyproject.toml` & `forestadmin_datasource_sqlalchemy-1.0.0b4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-sqlalchemy"
-version = "1.0.0-beta.3"
+version = "1.0.0-beta.4"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
@@ -20,16 +20,16 @@
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 typing-extensions = "~=4.2"
 tzdata = "~=2022.6"
 sqlalchemy = "^1.4.44"
-forestadmin-datasource-toolkit = "^1.0.0-beta.3"
-forestadmin-agent-toolkit = "^1.0.0-beta.3"
+forestadmin-datasource-toolkit = "^1.0.0-beta.4"
+forestadmin-agent-toolkit = "^1.0.0-beta.4"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~=0.2.1"
 python = "<3.9"
 extras = [ "tzdata",]
 
 [tool.poetry.group.test]
```

### Comparing `forestadmin_datasource_sqlalchemy-1.0.0b3/PKG-INFO` & `forestadmin_datasource_sqlalchemy-1.0.0b4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-sqlalchemy
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
-Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.3,<2.0.0)
-Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.3,<2.0.0)
+Requires-Dist: forestadmin-agent-toolkit (>=1.0.0-beta.4,<2.0.0)
+Requires-Dist: forestadmin-datasource-toolkit (>=1.0.0-beta.4,<2.0.0)
 Requires-Dist: sqlalchemy (>=1.4.44,<2.0.0)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Requires-Dist: tzdata (>=2022.6,<2023.0)
 Description-Content-Type: text/markdown
```

