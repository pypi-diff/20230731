# Comparing `tmp/aiogram3_di-1.0.3.tar.gz` & `tmp/aiogram3_di-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_di-1.0.3.tar", last modified: Sun Jul 30 19:15:25 2023, max compression
+gzip compressed data, was "aiogram3_di-1.0.4.tar", last modified: Mon Jul 31 10:17:37 2023, max compression
```

## Comparing `aiogram3_di-1.0.3.tar` & `aiogram3_di-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.3/LICENSE
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1420 2023-07-30 18:50:20.000000 aiogram3_di-1.0.3/README.md
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/aiogram3_di/
--rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.3/aiogram3_di/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-30 19:15:01.000000 aiogram3_di-1.0.3/aiogram3_di/_version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)      289 2023-07-28 19:58:50.000000 aiogram3_di-1.0.3/aiogram3_di/depends.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1046 2023-07-30 15:37:12.000000 aiogram3_di-1.0.3/aiogram3_di/middleware.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)     5568 2023-07-30 15:37:12.000000 aiogram3_di-1.0.3/aiogram3_di/utils.py
-drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/aiogram3_di.egg-info/
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/PKG-INFO
--rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/SOURCES.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/dependency_links.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/requires.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-30 19:15:25.000000 aiogram3_di-1.0.3/aiogram3_di.egg-info/top_level.txt
--rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-30 19:15:25.177083 aiogram3_di-1.0.3/setup.cfg
--rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.3/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1075 2023-01-01 13:29:08.000000 aiogram3_di-1.0.4/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1420 2023-07-30 18:50:20.000000 aiogram3_di-1.0.4/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/aiogram3_di/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      142 2023-07-28 19:36:21.000000 aiogram3_di-1.0.4/aiogram3_di/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-07-31 10:16:49.000000 aiogram3_di-1.0.4/aiogram3_di/_version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      276 2023-07-31 08:28:38.000000 aiogram3_di-1.0.4/aiogram3_di/depends.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1046 2023-07-30 15:37:12.000000 aiogram3_di-1.0.4/aiogram3_di/middleware.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5546 2023-07-31 10:11:43.000000 aiogram3_di-1.0.4/aiogram3_di/utils.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/aiogram3_di.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     2050 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      318 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       17 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       12 2023-07-31 10:17:37.000000 aiogram3_di-1.0.4/aiogram3_di.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-07-31 10:17:37.301295 aiogram3_di-1.0.4/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1044 2023-07-30 19:11:38.000000 aiogram3_di-1.0.4/setup.py
```

### Comparing `aiogram3_di-1.0.3/LICENSE` & `aiogram3_di-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.3/PKG-INFO` & `aiogram3_di-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3_di
-Version: 1.0.3
+Version: 1.0.4
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
```

### Comparing `aiogram3_di-1.0.3/README.md` & `aiogram3_di-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.3/aiogram3_di/middleware.py` & `aiogram3_di-1.0.4/aiogram3_di/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram3_di-1.0.3/aiogram3_di/utils.py` & `aiogram3_di-1.0.4/aiogram3_di/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         stack: AsyncExitStack,
         data: dict[str, Any],
         param_data: dict[tuple[int, str], Any]
 ) -> Any:
     if (cached_value := cache.get(hash(call))) and dependency.use_cache:
         return cached_value
 
-    values = _get_valid_kwargs((data | _extract_params(inspect.getfullargspec(call).annotations, param_data)), call)
+    values = _get_valid_kwargs((data | _extract_params(inspect.get_annotations(call), param_data)), call)
 
     if _is_async_gen_callable(call):
         cm = asynccontextmanager(call)(**values)
         result = await stack.enter_async_context(cm)
     elif _is_gen_callable(call):
         cm = _contextmanager_in_threadpool(contextmanager(call)(**values))
         result = await stack.enter_async_context(cm)
@@ -111,15 +111,15 @@
 async def _process_global_dependency(
         cache: dict[int, Any],
         stack: AsyncExitStack,
         data: dict[str, Any],
         param_data: dict[tuple[int, str], Any],
         dependency: Depends
 ) -> None:
-    for param_name, sub_dependency, type_annotation in _get_dependencies(inspect.getfullargspec(dependency.func).annotations):
+    for param_name, sub_dependency, type_annotation in _get_dependencies(inspect.get_annotations(dependency.func)):
         await _process_dependency(cache, stack, data, param_data, sub_dependency, type_annotation, param_name)
 
     await __process_dependency(cache, dependency.func, dependency, stack, data, param_data)
 
 
 async def process_dependencies(
         stack: AsyncExitStack,
```

### Comparing `aiogram3_di-1.0.3/aiogram3_di.egg-info/PKG-INFO` & `aiogram3_di-1.0.4/aiogram3_di.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-di
-Version: 1.0.3
+Version: 1.0.4
 Summary: Dependency Injection implementation for aiogram 3.
 Home-page: https://github.com/Vladyslav49/aiogram3_di
 Author: Vladyslav49
 Author-email: 
 License: MIT
 Keywords: Aiogram,Telegram,Bots,DI,Dependency Injection
 Classifier: Intended Audience :: Developers
```

### Comparing `aiogram3_di-1.0.3/setup.py` & `aiogram3_di-1.0.4/setup.py`

 * *Files identical despite different names*

