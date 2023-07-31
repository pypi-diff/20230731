# Comparing `tmp/model-connect-0.0.2.tar.gz` & `tmp/model-connect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-connect-0.0.2.tar", last modified: Mon Jul 31 00:36:41 2023, max compression
+gzip compressed data, was "model-connect-0.0.3.tar", last modified: Mon Jul 31 00:38:37 2023, max compression
```

## Comparing `model-connect-0.0.2.tar` & `model-connect-0.0.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.812777 model-connect-0.0.2/
--rw-rw-rw-   0        0        0    11393 2023-07-31 00:36:41.811271 model-connect-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    11290 2023-07-31 00:18:55.000000 model-connect-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.762739 model-connect-0.0.2/model_connect/
--rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.2/model_connect/__init__.py
--rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.2/model_connect/connect.py
--rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.2/model_connect/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.787980 model-connect-0.0.2/model_connect/integrations/
--rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.2/model_connect/integrations/__init__.py
--rw-rw-rw-   0        0        0      807 2023-07-30 22:28:32.000000 model-connect-0.0.2/model_connect/integrations/base.py
--rw-rw-rw-   0        0        0      476 2023-07-30 21:04:25.000000 model-connect-0.0.2/model_connect/integrations/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.788982 model-connect-0.0.2/model_connect/integrations/fastapi/
--rw-rw-rw-   0        0        0      345 2023-07-30 18:45:18.000000 model-connect-0.0.2/model_connect/integrations/fastapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.791981 model-connect-0.0.2/model_connect/integrations/fastapi/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.2/model_connect/integrations/fastapi/options/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-07-30 18:52:41.000000 model-connect-0.0.2/model_connect/integrations/fastapi/options/model.py
--rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.2/model_connect/integrations/fastapi/options/model_field.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.796496 model-connect-0.0.2/model_connect/integrations/psycopg2/
--rw-rw-rw-   0        0        0      478 2023-07-30 19:40:57.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/__init__.py
--rw-rw-rw-   0        0        0      577 2023-07-28 02:51:40.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/commons.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/delete.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:34.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/insert.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.799757 model-connect-0.0.2/model_connect/integrations/psycopg2/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/options/__init__.py
--rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/options/model.py
--rw-rw-rw-   0        0        0      633 2023-07-30 21:31:14.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/options/model_field.py
--rw-rw-rw-   0        0        0     6001 2023-07-30 23:55:10.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/select.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.2/model_connect/integrations/psycopg2/update.py
--rw-rw-rw-   0        0        0      533 2023-07-30 21:05:26.000000 model-connect-0.0.2/model_connect/integrations/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.801756 model-connect-0.0.2/model_connect/options/
--rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.2/model_connect/options/__init__.py
--rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.2/model_connect/options/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.804272 model-connect-0.0.2/model_connect/options/global/
--rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.2/model_connect/options/global/__init__.py
--rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.2/model_connect/options/global/global.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.807273 model-connect-0.0.2/model_connect/options/model/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.2/model_connect/options/model/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-07-30 22:31:01.000000 model-connect-0.0.2/model_connect/options/model/model.py
--rw-rw-rw-   0        0        0     1508 2023-07-30 20:33:29.000000 model-connect-0.0.2/model_connect/options/model/query_params.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.808275 model-connect-0.0.2/model_connect/options/model_field/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.2/model_connect/options/model_field/__init__.py
--rw-rw-rw-   0        0        0     3492 2023-07-30 22:35:02.000000 model-connect-0.0.2/model_connect/options/model_field/model_field.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.811271 model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/
--rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/request.py
--rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/response.py
--rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.2/model_connect/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:36:41.782925 model-connect-0.0.2/model_connect.egg-info/
--rw-rw-rw-   0        0        0    11393 2023-07-31 00:36:41.000000 model-connect-0.0.2/model_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2023-07-31 00:36:41.000000 model-connect-0.0.2/model_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 00:36:41.000000 model-connect-0.0.2/model_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 00:36:41.000000 model-connect-0.0.2/model_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 00:36:41.000000 model-connect-0.0.2/model_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 00:36:41.812777 model-connect-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      598 2023-07-31 00:35:19.000000 model-connect-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.607752 model-connect-0.0.3/
+-rw-rw-rw-   0        0        0    11395 2023-07-31 00:38:37.607752 model-connect-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11292 2023-07-31 00:38:26.000000 model-connect-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.556849 model-connect-0.0.3/model_connect/
+-rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.3/model_connect/__init__.py
+-rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.3/model_connect/connect.py
+-rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.3/model_connect/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.581160 model-connect-0.0.3/model_connect/integrations/
+-rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.3/model_connect/integrations/__init__.py
+-rw-rw-rw-   0        0        0      807 2023-07-30 22:28:32.000000 model-connect-0.0.3/model_connect/integrations/base.py
+-rw-rw-rw-   0        0        0      476 2023-07-30 21:04:25.000000 model-connect-0.0.3/model_connect/integrations/connect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.581160 model-connect-0.0.3/model_connect/integrations/fastapi/
+-rw-rw-rw-   0        0        0      345 2023-07-30 18:45:18.000000 model-connect-0.0.3/model_connect/integrations/fastapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.584709 model-connect-0.0.3/model_connect/integrations/fastapi/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/__init__.py
+-rw-rw-rw-   0        0        0     1024 2023-07-30 18:52:41.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/model.py
+-rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/model_field.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.590726 model-connect-0.0.3/model_connect/integrations/psycopg2/
+-rw-rw-rw-   0        0        0      478 2023-07-30 19:40:57.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-07-28 02:51:40.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/commons.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/delete.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:34.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/insert.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.594084 model-connect-0.0.3/model_connect/integrations/psycopg2/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/model.py
+-rw-rw-rw-   0        0        0      633 2023-07-30 21:31:14.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/model_field.py
+-rw-rw-rw-   0        0        0     6001 2023-07-30 23:55:10.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/select.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/update.py
+-rw-rw-rw-   0        0        0      533 2023-07-30 21:05:26.000000 model-connect-0.0.3/model_connect/integrations/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.596074 model-connect-0.0.3/model_connect/options/
+-rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.3/model_connect/options/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.3/model_connect/options/connect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.598073 model-connect-0.0.3/model_connect/options/global/
+-rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.3/model_connect/options/global/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.3/model_connect/options/global/global.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.601074 model-connect-0.0.3/model_connect/options/model/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.3/model_connect/options/model/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-07-30 22:31:01.000000 model-connect-0.0.3/model_connect/options/model/model.py
+-rw-rw-rw-   0        0        0     1508 2023-07-30 20:33:29.000000 model-connect-0.0.3/model_connect/options/model/query_params.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.602592 model-connect-0.0.3/model_connect/options/model_field/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.3/model_connect/options/model_field/__init__.py
+-rw-rw-rw-   0        0        0     3492 2023-07-30 22:35:02.000000 model-connect-0.0.3/model_connect/options/model_field/model_field.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.605611 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/
+-rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/__init__.py
+-rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/request.py
+-rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/response.py
+-rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.3/model_connect/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.576593 model-connect-0.0.3/model_connect.egg-info/
+-rw-rw-rw-   0        0        0    11395 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1667 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 00:38:37.607752 model-connect-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      598 2023-07-31 00:38:35.000000 model-connect-0.0.3/setup.py
```

### Comparing `model-connect-0.0.2/PKG-INFO` & `model-connect-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
-Our goals and how we plan to achieve them:
+ModelConnect goals and how it achieves them:
 
 - Simplicity
     - Fluent API
     - Minimal Setup to Start
 
 
 - Reliability
```

### Comparing `model-connect-0.0.2/README.md` & `model-connect-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
-Our goals and how we plan to achieve them:
+ModelConnect goals and how it achieves them:
 
 - Simplicity
     - Fluent API
     - Minimal Setup to Start
 
 
 - Reliability
```

### Comparing `model-connect-0.0.2/model_connect/integrations/base.py` & `model-connect-0.0.3/model_connect/integrations/base.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/fastapi/options/model.py` & `model-connect-0.0.3/model_connect/integrations/fastapi/options/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/psycopg2/commons.py` & `model-connect-0.0.3/model_connect/integrations/psycopg2/commons.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/psycopg2/options/model.py` & `model-connect-0.0.3/model_connect/integrations/psycopg2/options/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/psycopg2/options/model_field.py` & `model-connect-0.0.3/model_connect/integrations/psycopg2/options/model_field.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/psycopg2/select.py` & `model-connect-0.0.3/model_connect/integrations/psycopg2/select.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/integrations/registry.py` & `model-connect-0.0.3/model_connect/integrations/registry.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/connect.py` & `model-connect-0.0.3/model_connect/options/connect.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/model/model.py` & `model-connect-0.0.3/model_connect/options/model/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/model/query_params.py` & `model-connect-0.0.3/model_connect/options/model/query_params.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/model_field/model_field.py` & `model-connect-0.0.3/model_connect/options/model_field/model_field.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/request.py` & `model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/request.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/options/model_field/model_field_dtos/response.py` & `model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/response.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect/registry.py` & `model-connect-0.0.3/model_connect/registry.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/model_connect.egg-info/PKG-INFO` & `model-connect-0.0.3/model_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
-Our goals and how we plan to achieve them:
+ModelConnect goals and how it achieves them:
 
 - Simplicity
     - Fluent API
     - Minimal Setup to Start
 
 
 - Reliability
```

### Comparing `model-connect-0.0.2/model_connect.egg-info/SOURCES.txt` & `model-connect-0.0.3/model_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.2/setup.py` & `model-connect-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 long_description = Path(__name__).parent / 'README.md'
 long_description = long_description.read_text()
 
 setup(
     name='model-connect',
-    version='0.0.2',
+    version='0.0.3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(
         include=[
             'model_connect',
             'model_connect.*'
         ],
```

