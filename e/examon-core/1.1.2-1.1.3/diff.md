# Comparing `tmp/examon_core-1.1.2.tar.gz` & `tmp/examon_core-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_core-1.1.2.tar", max compression
+gzip compressed data, was "examon_core-1.1.3.tar", max compression
```

## Comparing `examon_core-1.1.2.tar` & `examon_core-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      225 2023-07-28 15:55:25.250080 examon_core-1.1.2/examon_core/__init__.py
--rwxr-xr-x   0        0        0     1908 2023-07-30 15:28:57.756531 examon_core-1.1.2/examon_core/code_as_string_factory.py
--rw-r--r--   0        0        0     1301 2023-07-30 18:35:51.460062 examon_core-1.1.2/examon_core/code_execution_sandbox.py
--rw-r--r--   0        0        0     1671 2023-07-30 08:22:25.918054 examon_core-1.1.2/examon_core/code_metrics.py
--rwxr-xr-x   0        0        0      574 2023-07-17 15:50:11.694400 examon_core-1.1.2/examon_core/examon_item.py
--rwxr-xr-x   0        0        0     2085 2023-07-30 15:20:51.926942 examon_core-1.1.2/examon_core/examon_item_registry.py
--rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.1.2/examon_core/multi_choice_factory.py
--rwxr-xr-x   0        0        0      617 2023-07-30 15:10:40.198476 examon_core-1.1.2/examon_core/question.py
--rw-r--r--   0        0        0     3000 2023-07-30 18:20:40.962231 examon_core-1.1.2/examon_core/question_factory.py
--rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.1.2/examon_core/question_response.py
--rw-r--r--   0        0        0      476 2023-07-30 19:12:19.400783 examon_core-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 examon_core-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      225 2023-07-28 15:55:25.250080 examon_core-1.1.3/examon_core/__init__.py
+-rwxr-xr-x   0        0        0     1883 2023-07-30 22:32:24.432974 examon_core-1.1.3/examon_core/code_as_string_factory.py
+-rw-r--r--   0        0        0     1301 2023-07-30 18:35:51.460062 examon_core-1.1.3/examon_core/code_execution_sandbox.py
+-rw-r--r--   0        0        0     1671 2023-07-30 08:22:25.918054 examon_core-1.1.3/examon_core/code_metrics.py
+-rwxr-xr-x   0        0        0      574 2023-07-30 22:07:32.328202 examon_core-1.1.3/examon_core/examon_item.py
+-rwxr-xr-x   0        0        0     2085 2023-07-30 15:20:51.926942 examon_core-1.1.3/examon_core/examon_item_registry.py
+-rw-r--r--   0        0        0      408 2023-07-16 08:19:13.774401 examon_core-1.1.3/examon_core/multi_choice_factory.py
+-rwxr-xr-x   0        0        0      617 2023-07-30 15:10:40.198476 examon_core-1.1.3/examon_core/question.py
+-rw-r--r--   0        0        0     3000 2023-07-30 22:15:54.737355 examon_core-1.1.3/examon_core/question_factory.py
+-rwxr-xr-x   0        0        0      201 2023-07-15 15:48:50.722464 examon_core-1.1.3/examon_core/question_response.py
+-rw-r--r--   0        0        0      476 2023-07-30 22:33:49.077411 examon_core-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 examon_core-1.1.3/PKG-INFO
```

### Comparing `examon_core-1.1.2/examon_core/code_as_string_factory.py` & `examon_core-1.1.3/examon_core/code_as_string_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import re
 import logging
 
 
 class CodeAsStringFactory:
     @staticmethod
     def build(function, decorators=[]):
         src_code = CodeAsStringFactory.function_src(function)
@@ -34,15 +33,15 @@
                 all_hints += f'# {hint}\n'
         all_hints = f'# Hints:\n{all_hints}\n\n'
         return all_hints + src_code
 
 
 class RemoveQuizItemDecorator:
     def decorate(self, src_code):
-        return re.sub('@examon\\_item\\(.*\\)', '', src_code)
+        return src_code[src_code.find('def'):]
 
 
 class AppendPrintDecorator:
     def __init__(self, function_name, param=''):
         self.function_name = function_name
         self.param = param
```

### Comparing `examon_core-1.1.2/examon_core/code_execution_sandbox.py` & `examon_core-1.1.3/examon_core/code_execution_sandbox.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/examon_core/code_metrics.py` & `examon_core-1.1.3/examon_core/code_metrics.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/examon_core/examon_item.py` & `examon_core-1.1.3/examon_core/examon_item.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/examon_core/examon_item_registry.py` & `examon_core-1.1.3/examon_core/examon_item_registry.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/examon_core/question.py` & `examon_core-1.1.3/examon_core/question.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/examon_core/question_factory.py` & `examon_core-1.1.3/examon_core/question_factory.py`

 * *Files identical despite different names*

### Comparing `examon_core-1.1.2/PKG-INFO` & `examon_core-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: examon-core
-Version: 1.1.2
+Version: 1.1.3
 Summary: Examon Core Libs
 Author: Jarrod Folino
 Author-email: jdfolino@icloud.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

