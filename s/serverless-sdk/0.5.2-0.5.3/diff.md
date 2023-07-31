# Comparing `tmp/serverless-sdk-0.5.2.tar.gz` & `tmp/serverless-sdk-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-eigj_mpj/serverless-sdk-0.5.2.tar", last modified: Thu Jul  6 19:04:56 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-icisettl/serverless-sdk-0.5.3.tar", last modified: Mon Jul 31 21:12:52 2023, max compression
```

## Comparing `serverless-sdk-0.5.2.tar` & `serverless-sdk-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/tag_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/lib/warning_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/sls_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 19:04:56.000000 serverless-sdk-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-06 19:04:36.000000 serverless-sdk-0.5.2/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18061 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/tag_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:12:52.000000 serverless-sdk-0.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-07-31 21:12:27.000000 serverless-sdk-0.5.3/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.5.2/PKG-INFO` & `serverless-sdk-0.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.2
+Version: 0.5.3
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.2/README.md` & `serverless-sdk-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/pyproject.toml` & `serverless-sdk-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.5.3/serverless_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.5.2
+Version: 0.5.3
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `serverless-sdk-0.5.2/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.5.3/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/__init__.py` & `serverless-sdk-0.5.3/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/base.py` & `serverless-sdk-0.5.3/sls_sdk/base.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/exceptions.py` & `serverless-sdk-0.5.3/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.5.3/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/emitter.py` & `serverless-sdk-0.5.3/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/error.py` & `serverless-sdk-0.5.3/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.5.3/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/imports.py` & `serverless-sdk-0.5.3/sls_sdk/lib/imports.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with internally_imported():
     import time
     import contextvars
     import contextlib
     from urllib.parse import urlparse
     from urllib.parse import parse_qs
     import io
-    from typing import Iterable
+    from typing import Iterable, Optional, Any
 
 from ..error import report as report_error
 from .import_hook import ImportHook
 from .wrapper import replace_method
 
 
 SDK = sls_sdk.serverlessSdk
@@ -39,75 +39,89 @@
             return func(*args, **kwargs)
         except Exception:
             return None
 
     return wrapper
 
 
+def _decode_bytes(body: bytes, encoding: Optional[str], gzip: Any):
+    if encoding == "gzip":
+        return gzip.decompress(body).decode("utf-8")
+    return body.decode("utf-8")
+
+
 @safe_call
-def _decode_body(body):
+def _decode_body(body: Any, encoding: Optional[str] = None, gzip: Optional[Any] = None):
     if isinstance(body, bytes):
-        return body.decode("utf-8")
+        return _decode_bytes(body, encoding, gzip)
     elif isinstance(body, str):
         return body
     elif isinstance(body, io.IOBase):
         if body.seekable():
             current_position = body.tell()
             try:
-                return body.read().decode("utf-8")
+                return _decode_bytes(body.read(), encoding, gzip)
             finally:
                 body.seek(current_position)
+        elif hasattr(body, "peek"):
+            return _decode_bytes(body.peek(), encoding, gzip)
         else:
-            return body.peek().decode("utf-8")
+            return None
     elif isinstance(body, Iterable):
-        return b"".join(body).decode("utf-8")
+        return _decode_bytes(b"".join(body), encoding, gzip)
     else:
         return None
 
 
 class BaseInstrumenter:
     def __init__(self, target_module):
         self._import_hook = ImportHook(target_module)
         self._is_installed = False
         self._module = None
+        self._gzip = None
 
     def install(self, should_monitor_request_response):
         if self._is_installed:
             return
         self.should_monitor_request_response = should_monitor_request_response
 
         if self._import_hook.enabled:
             return
 
         self._import_hook.enable(self._install)
         self._is_installed = True
 
+        if should_monitor_request_response:
+            with internally_imported():
+                import gzip
+
+                self._gzip = gzip
+
     def uninstall(self):
         if not self._is_installed:
             return
 
         self._import_hook.disable(self._uninstall)
         self._is_installed = False
 
     def _install(self, module):
         raise NotImplementedError
 
     def _uninstall(self, module):
         raise NotImplementedError
 
-    def _capture_request_body(self, trace_span, body):
+    def _capture_request_body(
+        self, trace_span, body: Any, encoding: Optional[str] = None
+    ):
         if not body:
             return
         if not self.should_monitor_request_response:
             return
 
-        decoded = _decode_body(body)
-        # TODO: Temporary handling of `decoded` being `None` case
-        # Ideally we should invetsigate why `decoded` is `None`
-        # and ensure we handle it properly
+        decoded = _decode_body(body, encoding, self._gzip)
         if not decoded:
             return
         length = len(decoded)
 
         if length > SDK._maximum_body_byte_length:
             SDK._report_notice(
                 "Large body excluded",
@@ -147,16 +161,14 @@
             response.content.unread_data(response_body)
             if response_body:
                 trace_span.output = _decode_body(response_body)
         except Exception as ex:
             report_error(ex)
 
     async def _on_request_start(self, session, trace_config_ctx, params):
-        if hasattr(session, "_sls_ignore") and session._sls_ignore:
-            return
         trace_config_ctx.start_time = time.perf_counter_ns()
         SDK._debug_log("HTTP request")
         trace_config_ctx.trace_span = SDK._create_trace_span(
             f"python.{params.url.scheme}.request",
             start_time=trace_config_ctx.start_time,
         )
         trace_config_ctx.trace_span.tags.update(
@@ -192,15 +204,19 @@
         if trace_config_ctx.trace_span.end_time is None:
             trace_config_ctx.trace_span.close()
 
     async def _on_request_end(self, session, trace_config_ctx, params):
         if not hasattr(trace_config_ctx, "trace_span"):
             return
         self._capture_request_body(
-            trace_config_ctx.trace_span, trace_config_ctx.request_body
+            trace_config_ctx.trace_span,
+            trace_config_ctx.request_body,
+            params.headers.get("Content-Encoding")
+            if hasattr(params, "headers")
+            else None,
         )
         trace_config_ctx.trace_span.tags.update(
             {"status_code": params.response.status}, prefix="http"
         )
         await self._capture_response_body(trace_config_ctx.trace_span, params.response)
         if trace_config_ctx.trace_span.end_time is None:
             trace_config_ctx.trace_span.close()
@@ -247,19 +263,15 @@
         self._original_request = None
         self._original_getresponse = None
 
     def _instrumented_request(self):
         # See https://docs.python.org/3/library/http.client.html#http.client.HTTPConnection.request
         # for the signature of the request method
         def _func(_self, method, url, body=None, headers={}, *, encode_chunked=False):
-            _self._sls_ignore = (
-                _IGNORE_FOLLOWING_REQUEST.get() or _DISABLE_NATIVE_INSTRUMENTATION.get()
-            )
-
-            if _self._sls_ignore:
+            if _IGNORE_FOLLOWING_REQUEST.get() or _DISABLE_NATIVE_INSTRUMENTATION.get():
                 return self._original_request(
                     _self, method, url, body, headers, encode_chunked=encode_chunked
                 )
             start_time = time.perf_counter_ns()
 
             SDK._debug_log("HTTP request")
             protocol = (
@@ -282,15 +294,17 @@
                         "host": f"{_self.host}:{_self.port}",
                         "path": parsed_path.path,
                         "request_header_names": [h for h in headers.keys()],
                         "query_parameter_names": [q for q in query.keys()],
                     },
                     prefix="http",
                 )
-                self._capture_request_body(trace_span, body)
+                self._capture_request_body(
+                    trace_span, body, headers.get("Content-Encoding")
+                )
 
                 self._original_request(
                     _self, method, url, body, headers, encode_chunked=encode_chunked
                 )
             except Exception as ex:
                 trace_span = _HTTP_SPAN.get()
                 trace_span.tags["http.error_code"] = ex.__class__.__name__
@@ -301,15 +315,19 @@
         return _func
 
     def _instrumented_getresponse(self):
         # See https://docs.python.org/3/library/http.client.html#http.client.HTTPConnection.getresponse
         # for the signature of the getresponse method
         def _func(_self, *args, **kwargs):
             trace_span = _HTTP_SPAN.get()
-            if getattr(self, "_sls_ignore", False) or not trace_span:
+            if (
+                not trace_span
+                or _IGNORE_FOLLOWING_REQUEST.get()
+                or _DISABLE_NATIVE_INSTRUMENTATION.get()
+            ):
                 return self._original_getresponse(_self, *args, **kwargs)
 
             try:
                 response = self._original_getresponse(_self, *args, **kwargs)
                 trace_span.tags["http.status_code"] = response.status
                 self._capture_response_body(trace_span, response)
                 return response
@@ -401,15 +419,17 @@
                     "host": f"{instance.host}:{instance.port}",
                     "path": parsed_path.path,
                     "request_header_names": [h for h in headers.keys()],
                     "query_parameter_names": [q for q in query.keys()],
                 },
                 prefix="http",
             )
-            self._capture_request_body(trace_span, body)
+            self._capture_request_body(
+                trace_span, body, headers.get("Content-Encoding")
+            )
 
             with URLLib3Instrumenter._prevent_recursive_instrumentation():
                 response = actual_url_open(*args, **kwargs)
 
                 trace_span.tags["http.status_code"] = response.status
                 self._capture_response_body(trace_span, response)
                 return response
```

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,58 +14,59 @@
 
 
 _original_error = None
 _original_warning = None
 _original_warn = None
 
 
-def _resolve_message(*args) -> str:
-    return args[0] % args[1:]
+def _resolve_message(msg, *args) -> str:
+    msg = str(msg)
+    if args:
+        msg = msg % args
+    return msg
 
 
-def _error(self, *args, **kwargs):
+def _error(self, msg, *args, **kwargs):
     try:
-        if (
-            len(args) == 1
-            and type(args[0]) is dict
-            and args[0].get("source") == "serverlessSdk"
-        ):
-            args = (json.dumps(args[0], indent=2),) + args[1:]
+        if isinstance(msg, dict) and msg.get("source") == "serverlessSdk" and not args:
+            msg = json.dumps(msg, indent=2)
             return
-        if len(args) == 1 and isinstance(args[0], BaseException):
-            message = args[0]
+        elif not args and isinstance(msg, BaseException):
+            message = msg
         else:
-            message = _resolve_message(*args)
+            message = _resolve_message(msg, *args)
         create_error_captured_event(message, origin="pythonLogging")
     except Exception as ex:
         report_error(ex)
     finally:
-        _original_error(self, *args, **kwargs)
+        _original_error(self, msg, *args, **kwargs)
 
 
 def _warning(call_warn: bool = False):
-    def __warning(self, *args, **kwargs):
+    def __warning(self, msg, *args, **kwargs):
         try:
             if (
-                len(args) == 1
-                and type(args[0]) is dict
-                and args[0].get("source") == "serverlessSdk"
+                isinstance(msg, dict)
+                and msg.get("source") == "serverlessSdk"
+                and not args
             ):
-                args = (json.dumps(args[0], indent=2),) + args[1:]
+                msg = json.dumps(msg, indent=2)
                 return
-            create_warning_captured_event(
-                _resolve_message(*args), origin="pythonLogging"
-            )
+            elif not args and isinstance(msg, BaseException):
+                message = msg
+            else:
+                message = _resolve_message(msg, *args)
+            create_warning_captured_event(message, origin="pythonLogging")
         except Exception as ex:
             report_error(ex)
         finally:
             if call_warn:
-                _original_warn(self, *args, **kwargs)
+                _original_warn(self, msg, *args, **kwargs)
             else:
-                _original_warning(self, *args, **kwargs)
+                _original_warning(self, msg, *args, **kwargs)
 
     return __warning
 
 
 def install():
     global _is_installed
     if _is_installed:
```

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/instrumentation/wrapper.py` & `serverless-sdk-0.5.3/sls_sdk/lib/instrumentation/wrapper.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/name.py` & `serverless-sdk-0.5.3/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/notice.py` & `serverless-sdk-0.5.3/sls_sdk/lib/notice.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.5.3/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/tags.py` & `serverless-sdk-0.5.3/sls_sdk/lib/tags.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/trace.py` & `serverless-sdk-0.5.3/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/warning.py` & `serverless-sdk-0.5.3/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.5.3/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/tests/test_sdk.py` & `serverless-sdk-0.5.3/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.5.2/tests/test_thread_safety.py` & `serverless-sdk-0.5.3/tests/test_thread_safety.py`

 * *Files identical despite different names*

