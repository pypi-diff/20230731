# Comparing `tmp/model-connect-0.0.4.tar.gz` & `tmp/model-connect-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-connect-0.0.4.tar", last modified: Mon Jul 31 02:59:24 2023, max compression
+gzip compressed data, was "model-connect-0.0.5.tar", last modified: Mon Jul 31 04:57:53 2023, max compression
```

## Comparing `model-connect-0.0.4.tar` & `model-connect-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.167861 model-connect-0.0.4/
--rw-rw-rw-   0        0        0    10921 2023-07-31 02:59:24.167861 model-connect-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    10818 2023-07-31 00:53:30.000000 model-connect-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.032334 model-connect-0.0.4/model_connect/
--rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.4/model_connect/__init__.py
--rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.4/model_connect/connect.py
--rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.4/model_connect/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.075907 model-connect-0.0.4/model_connect/integrations/
--rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.4/model_connect/integrations/__init__.py
--rw-rw-rw-   0        0        0      651 2023-07-31 00:56:43.000000 model-connect-0.0.4/model_connect/integrations/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.092996 model-connect-0.0.4/model_connect/integrations/fastapi/
--rw-rw-rw-   0        0        0      401 2023-07-31 01:00:27.000000 model-connect-0.0.4/model_connect/integrations/fastapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.107411 model-connect-0.0.4/model_connect/integrations/fastapi/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/__init__.py
--rw-rw-rw-   0        0        0      961 2023-07-31 00:49:20.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/model.py
--rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/model_field.py
--rw-rw-rw-   0        0        0      504 2023-07-31 00:52:20.000000 model-connect-0.0.4/model_connect/integrations/fastapi/router.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.112916 model-connect-0.0.4/model_connect/integrations/psycopg2/
--rw-rw-rw-   0        0        0      846 2023-07-31 02:56:09.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.115915 model-connect-0.0.4/model_connect/integrations/psycopg2/common/
--rw-rw-rw-   0        0        0        0 2023-07-31 01:29:50.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/__init__.py
--rw-rw-rw-   0        0        0     3854 2023-07-31 02:03:39.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/processing.py
--rw-rw-rw-   0        0        0      577 2023-07-31 01:34:36.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/streaming.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/delete.py
--rw-rw-rw-   0        0        0     2811 2023-07-31 02:33:09.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/insert.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.125104 model-connect-0.0.4/model_connect/integrations/psycopg2/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/__init__.py
--rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/model.py
--rw-rw-rw-   0        0        0     1110 2023-07-31 02:27:12.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/model_field.py
--rw-rw-rw-   0        0        0     2993 2023-07-31 02:33:07.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/select.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/update.py
--rw-rw-rw-   0        0        0      840 2023-07-31 01:16:35.000000 model-connect-0.0.4/model_connect/integrations/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.132690 model-connect-0.0.4/model_connect/options/
--rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.4/model_connect/options/__init__.py
--rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.4/model_connect/options/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.145247 model-connect-0.0.4/model_connect/options/global/
--rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.4/model_connect/options/global/__init__.py
--rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.4/model_connect/options/global/global.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.149233 model-connect-0.0.4/model_connect/options/model/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.4/model_connect/options/model/__init__.py
--rw-rw-rw-   0        0        0     2017 2023-07-31 02:56:34.000000 model-connect-0.0.4/model_connect/options/model/model.py
--rw-rw-rw-   0        0        0     1508 2023-07-31 02:03:06.000000 model-connect-0.0.4/model_connect/options/model/query_params.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.151296 model-connect-0.0.4/model_connect/options/model_field/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.4/model_connect/options/model_field/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.166015 model-connect-0.0.4/model_connect/options/model_field/dtos/
--rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/request.py
--rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/response.py
--rw-rw-rw-   0        0        0     3446 2023-07-31 02:03:39.000000 model-connect-0.0.4/model_connect/options/model_field/model_field.py
--rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.4/model_connect/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.058434 model-connect-0.0.4/model_connect.egg-info/
--rw-rw-rw-   0        0        0    10921 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1723 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 02:59:24.167861 model-connect-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-07-31 02:59:11.000000 model-connect-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.551802 model-connect-0.0.5/
+-rw-rw-rw-   0        0        0    10921 2023-07-31 04:57:53.551802 model-connect-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10818 2023-07-31 00:53:30.000000 model-connect-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.488674 model-connect-0.0.5/model_connect/
+-rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.5/model_connect/__init__.py
+-rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.5/model_connect/connect.py
+-rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.5/model_connect/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.513450 model-connect-0.0.5/model_connect/integrations/
+-rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.5/model_connect/integrations/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-31 00:56:43.000000 model-connect-0.0.5/model_connect/integrations/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.515445 model-connect-0.0.5/model_connect/integrations/fastapi/
+-rw-rw-rw-   0        0        0      401 2023-07-31 01:00:27.000000 model-connect-0.0.5/model_connect/integrations/fastapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.519606 model-connect-0.0.5/model_connect/integrations/fastapi/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-07-31 00:49:20.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/model.py
+-rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.5/model_connect/integrations/fastapi/options/model_field.py
+-rw-rw-rw-   0        0        0      504 2023-07-31 00:52:20.000000 model-connect-0.0.5/model_connect/integrations/fastapi/router.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.521604 model-connect-0.0.5/model_connect/integrations/json/
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:32.000000 model-connect-0.0.5/model_connect/integrations/json/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:41.000000 model-connect-0.0.5/model_connect/integrations/json/decoder.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:45.000000 model-connect-0.0.5/model_connect/integrations/json/encoder.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.522605 model-connect-0.0.5/model_connect/integrations/json/options/
+-rw-rw-rw-   0        0        0        0 2023-07-31 03:58:36.000000 model-connect-0.0.5/model_connect/integrations/json/options/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.528786 model-connect-0.0.5/model_connect/integrations/psycopg2/
+-rw-rw-rw-   0        0        0      846 2023-07-31 02:56:09.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.531785 model-connect-0.0.5/model_connect/integrations/psycopg2/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:29:50.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/__init__.py
+-rw-rw-rw-   0        0        0     4034 2023-07-31 03:53:55.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/processing.py
+-rw-rw-rw-   0        0        0     1393 2023-07-31 04:42:27.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/common/streaming.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/delete.py
+-rw-rw-rw-   0        0        0     2960 2023-07-31 04:50:50.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/insert.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.534784 model-connect-0.0.5/model_connect/integrations/psycopg2/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/model.py
+-rw-rw-rw-   0        0        0     1157 2023-07-31 03:44:39.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/options/model_field.py
+-rw-rw-rw-   0        0        0     4135 2023-07-31 04:55:13.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/select.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.5/model_connect/integrations/psycopg2/update.py
+-rw-rw-rw-   0        0        0      840 2023-07-31 01:16:35.000000 model-connect-0.0.5/model_connect/integrations/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.537297 model-connect-0.0.5/model_connect/options/
+-rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.5/model_connect/options/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.5/model_connect/options/connect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.540296 model-connect-0.0.5/model_connect/options/global/
+-rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.5/model_connect/options/global/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.5/model_connect/options/global/global.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.544293 model-connect-0.0.5/model_connect/options/model/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.5/model_connect/options/model/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-07-31 02:56:34.000000 model-connect-0.0.5/model_connect/options/model/model.py
+-rw-rw-rw-   0        0        0     1508 2023-07-31 02:03:06.000000 model-connect-0.0.5/model_connect/options/model/query_params.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.546796 model-connect-0.0.5/model_connect/options/model_field/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.5/model_connect/options/model_field/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.549803 model-connect-0.0.5/model_connect/options/model_field/dtos/
+-rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/__init__.py
+-rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/request.py
+-rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.5/model_connect/options/model_field/dtos/response.py
+-rw-rw-rw-   0        0        0     3533 2023-07-31 03:43:04.000000 model-connect-0.0.5/model_connect/options/model_field/model_field.py
+-rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.5/model_connect/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:57:53.509456 model-connect-0.0.5/model_connect.egg-info/
+-rw-rw-rw-   0        0        0    10921 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1905 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 04:57:53.000000 model-connect-0.0.5/model_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:57:53.552802 model-connect-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-07-31 04:57:46.000000 model-connect-0.0.5/setup.py
```

### Comparing `model-connect-0.0.4/PKG-INFO` & `model-connect-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.4
+Version: 0.0.5
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
```

### Comparing `model-connect-0.0.4/README.md` & `model-connect-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/integrations/base.py` & `model-connect-0.0.5/model_connect/integrations/base.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/integrations/fastapi/options/model.py` & `model-connect-0.0.5/model_connect/integrations/fastapi/options/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/__init__.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/__init__.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/common/processing.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/common/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from dataclasses import dataclass
 from typing import TypeVar, Optional
 
+from model_connect.constants import is_undefined, UNDEFINED
 from model_connect.registry import get_model_field_options
 
 _T = TypeVar('_T')
 
 
 class ProcessedFilters(list['ProcessedFilter']):
-    def __init__(self, vars_: list, *args, **kwargs):
+    def __init__(self, vars_: list = UNDEFINED, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.vars = vars_ or []
+        if is_undefined(vars_):
+            vars_ = []
+
+        self.vars = vars_
 
 
 @dataclass
 class ProcessedFilter:
     column: str
     operator: str
     value: str
@@ -91,31 +95,35 @@
 
             for value_ in value:
                 if value_ is None and operator == '=':
                     operator = 'IS'
                 if value_ is None and operator in ('!=', '<>'):
                     operator = 'IS NOT'
 
-                result.vars.append(value)
+                result.vars.append(value_)
                 result.append(
                     ProcessedFilter(
                         column=field.name,
                         operator=operator,
                         value='%s'
                     )
                 )
 
     return result
 
+
 def process_sort_options(
         cls: type[_T],
         sort_options: dict
 ):
     result = ProcessedSortingOptions()
 
+    if not sort_options:
+        return result
+
     for field, direction in sort_options.items():
         field = get_model_field_options(cls, field)
 
         if not field:
             continue
 
         if not field.can_sort:
```

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/insert.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/insert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,55 +1,64 @@
 from dataclasses import dataclass, field, asdict
+from functools import cache
 from typing import Iterable, TypeVar
 
 from jinja2 import Template
 from psycopg2.extras import DictCursor
 
 from model_connect import registry
 from model_connect.integrations.psycopg2 import Psycopg2Model, Psycopg2ModelField
-from model_connect.integrations.psycopg2.common.streaming import stream_from_cursor, stream_results_to_model_type
+from model_connect.integrations.psycopg2.common.streaming import stream_from_cursor, stream_results_to_dataclass
 from model_connect.registry import get_model_options
 
 _T = TypeVar('_T')
 
 
 @dataclass
 class InsertSQL:
     sql: str
     vars: list = field(
         default_factory=list
     )
 
 
+@cache
+def generate_insert_columns(model_class: type[_T]) -> list[str]:
+    columns = []
+
+    model_fields = registry.get(model_class).model_fields.values()
+
+    for model_field in model_fields:
+        model_field = model_field.integrations.get(Psycopg2ModelField)
+
+        if not model_field.include_in_insert:
+            continue
+
+        columns.append(
+            model_field.column_name
+        )
+
+    return columns
+
+
 def create_insert_query(
         model_class: type[_T],
         data: _T | Iterable[_T],
         columns: list[str] = None
 ) -> InsertSQL:
     vars_ = []
 
     model = get_model_options(model_class)
     model = model.integrations.get(Psycopg2Model)
 
     if isinstance(data, model_class):
         data = [data]
 
     if not columns:
-        model_fields = registry.get(model_class).model_fields.values()
-
-        columns = []
-        for model_field in model_fields:
-            model_field = model_field.integrations.get(Psycopg2ModelField)
-
-            if not model_field.include_in_insert:
-                continue
-
-            columns.append(
-                model_field.column_name
-            )
+        columns = generate_insert_columns(model_class)
 
     values = []
 
     for item in data:
         if not isinstance(item, dict):
             # noinspection PyDataclass
             item = asdict(item)
@@ -109,11 +118,11 @@
 
     cursor.executemany(
         insert_query.sql,
         insert_query.vars
     )
 
     results = stream_from_cursor(cursor)
-    results = stream_results_to_model_type(results, model_class)
+    results = stream_results_to_dataclass(results, model_class)
 
     for result in results:
         yield result
```

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/options/model.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/options/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/options/model_field.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/options/model_field.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,9 +32,10 @@
         self.include_in_insert = coalesce(
             self.include_in_insert,
             not model_field.is_identifier
         )
 
         self.include_in_select = coalesce(
             self.include_in_select,
+            model_field.dataclass_field.init,
             True
         )
```

### Comparing `model-connect-0.0.4/model_connect/integrations/psycopg2/select.py` & `model-connect-0.0.5/model_connect/integrations/psycopg2/select.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,93 @@
 from dataclasses import dataclass, field as dataclass_field
+from functools import cache
 from typing import Any, TypeVar
 
 from jinja2 import Template
 from psycopg2.extras import DictCursor
 
+from model_connect import registry
+from model_connect.integrations.psycopg2 import Psycopg2ModelField
 from model_connect.integrations.psycopg2.common.processing import process_filter_options, process_sort_options, \
-    process_pagination_options
-from model_connect.integrations.psycopg2.common.streaming import stream_results_to_model_type, stream_from_cursor
+    process_pagination_options, ProcessedFilters
+from model_connect.integrations.psycopg2.common.streaming import stream_results_to_dataclass, stream_from_cursor
 from model_connect.integrations.psycopg2.options.model import Psycopg2Model
 from model_connect.registry import get_model_field_options, get_model_options
 
 _T = TypeVar('_T')
 
 
 @dataclass
 class SelectSQL:
     sql: str
     vars: list[Any] = dataclass_field(
         default_factory=list
     )
 
 
+@cache
+def generate_select_columns(model_class: type[_T]) -> list[str]:
+    columns = []
+
+    model_fields = registry.get(model_class).model_fields.values()
+
+    for model_field in model_fields:
+        model_field = model_field.integrations.get(Psycopg2ModelField)
+
+        if not model_field.include_in_select:
+            continue
+
+        columns.append(
+            model_field.column_name
+        )
+
+    return columns
+
+
 def create_select_query(
         model_class: type[_T],
+        columns: list[str] = None,
         filter_options: dict = None,
         sort_options: dict = None,
         pagination_options: dict = None
 ) -> SelectSQL:
     vars_ = []
 
     model = get_model_options(model_class)
     model = model.integrations.get(Psycopg2Model)
 
+    if columns is None:
+        columns = generate_select_columns(
+            model_class
+        )
+
     filter_options = process_filter_options(
         model_class,
         filter_options,
         vars_
     )
-    filter_options = list(filter_options)
 
     sort_options = process_sort_options(
         model_class,
         sort_options
     )
-    sort_options = list(sort_options)
 
     pagination_options = process_pagination_options(
         pagination_options,
         vars_
     )
 
     template = Template('''
         SELECT
-            *
+            {%- for column in columns %}
+            {{ column }}
+            {%- if not loop.last %}
+            ,
+            {%- endif %}
+            {%- endfor %}
 
         FROM
             {{ tablename }}
 
         {%- if filter_options %}
             WHERE
             {%- for filter in filter_options %}
@@ -83,14 +114,15 @@
 
         {%- if pagination_options.offset %}
             OFFSET %s
         {%- endif %}
         ''')
 
     sql = template.render(
+        columns=columns,
         tablename=model.tablename,
         filter_options=filter_options,
         sort_options=sort_options,
         pagination_options=pagination_options
     )
 
     sql = ' '.join(sql.split())
@@ -98,17 +130,31 @@
 
     return SelectSQL(
         sql,
         vars_
     )
 
 
-def stream_select(cursor: DictCursor, model_class: type[_T], chunk_size: int = 1000):
-    query = create_select_query(model_class)
+def stream_select(
+        cursor: DictCursor,
+        dataclass_type: type[_T],
+        columns: list[str] = None,
+        chunk_size: int = 1000,
+        filter_options: dict = None,
+        sort_options: dict = None,
+        pagination_options: dict = None
+):
+    query = create_select_query(
+        dataclass_type,
+        columns,
+        filter_options,
+        sort_options,
+        pagination_options
+    )
 
     cursor.execute(query.sql, query.vars)
 
     results = stream_from_cursor(cursor, chunk_size)
-    results = stream_results_to_model_type(results, model_class)
+    results = stream_results_to_dataclass(results, dataclass_type)
 
     for result in results:
         yield result
```

### Comparing `model-connect-0.0.4/model_connect/integrations/registry.py` & `model-connect-0.0.5/model_connect/integrations/registry.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/connect.py` & `model-connect-0.0.5/model_connect/options/connect.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/model/model.py` & `model-connect-0.0.5/model_connect/options/model/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/model/query_params.py` & `model-connect-0.0.5/model_connect/options/model/query_params.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/model_field/dtos/request.py` & `model-connect-0.0.5/model_connect/options/model_field/dtos/request.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/model_field/dtos/response.py` & `model-connect-0.0.5/model_connect/options/model_field/dtos/response.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect/options/model_field/model_field.py` & `model-connect-0.0.5/model_connect/options/model_field/model_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 
     _integrations: ModelFieldIntegrations = field(
         init=False,
         default_factory=dict
     )
 
     @property
+    def dataclass_field(self):
+        return self._dataclass_field
+
+    @property
     def type(self):
         return self._type
 
     @property
     def name(self):
         return self._name
```

### Comparing `model-connect-0.0.4/model_connect/registry.py` & `model-connect-0.0.5/model_connect/registry.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.4/model_connect.egg-info/PKG-INFO` & `model-connect-0.0.5/model_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.4
+Version: 0.0.5
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
```

### Comparing `model-connect-0.0.4/model_connect.egg-info/SOURCES.txt` & `model-connect-0.0.5/model_connect.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 model_connect/integrations/base.py
 model_connect/integrations/registry.py
 model_connect/integrations/fastapi/__init__.py
 model_connect/integrations/fastapi/router.py
 model_connect/integrations/fastapi/options/__init__.py
 model_connect/integrations/fastapi/options/model.py
 model_connect/integrations/fastapi/options/model_field.py
+model_connect/integrations/json/__init__.py
+model_connect/integrations/json/decoder.py
+model_connect/integrations/json/encoder.py
+model_connect/integrations/json/options/__init__.py
 model_connect/integrations/psycopg2/__init__.py
 model_connect/integrations/psycopg2/delete.py
 model_connect/integrations/psycopg2/insert.py
 model_connect/integrations/psycopg2/select.py
 model_connect/integrations/psycopg2/update.py
 model_connect/integrations/psycopg2/common/__init__.py
 model_connect/integrations/psycopg2/common/processing.py
```

### Comparing `model-connect-0.0.4/setup.py` & `model-connect-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 long_description = Path(__name__).parent / 'README.md'
 long_description = long_description.read_text()
 
 setup(
     name='model-connect',
-    version='0.0.4',
+    version='0.0.5',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(
         include=[
             'model_connect',
             'model_connect.*'
         ],
```

