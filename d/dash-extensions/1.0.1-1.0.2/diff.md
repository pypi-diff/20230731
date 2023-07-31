# Comparing `tmp/dash_extensions-1.0.1.tar.gz` & `tmp/dash_extensions-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_extensions-1.0.1.tar", max compression
+gzip compressed data, was "dash_extensions-1.0.2.tar", max compression
```

## Comparing `dash_extensions-1.0.1.tar` & `dash_extensions-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,11 @@
--rw-r--r--   0        0        0     1077 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/LICENSE
--rw-r--r--   0        0        0     1877 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/README.md
--rw-r--r--   0        0        0     2243 2023-05-22 15:15:31.807984 dash_extensions-1.0.1/dash_extensions/BeforeAfter.py
--rw-r--r--   0        0        0     1388 2023-05-22 15:15:31.807984 dash_extensions-1.0.1/dash_extensions/CycleBreaker.py
--rw-r--r--   0        0        0     1282 2023-05-22 15:15:31.807984 dash_extensions-1.0.1/dash_extensions/DeferScript.py
--rw-r--r--   0        0        0     2596 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/EventListener.py
--rw-r--r--   0        0        0     2043 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/EventSource.py
--rw-r--r--   0        0        0     2665 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/Lottie.py
--rw-r--r--   0        0        0     1542 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/Mermaid.py
--rw-r--r--   0        0        0     1377 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/Purify.py
--rw-r--r--   0        0        0     1809 2023-05-22 15:15:31.811984 dash_extensions-1.0.1/dash_extensions/Ticker.py
--rw-r--r--   0        0        0     1885 2023-05-22 15:15:31.815984 dash_extensions-1.0.1/dash_extensions/WebSocket.py
--rw-r--r--   0        0        0     2492 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/dash_extensions/__init__.py
--rw-r--r--   0        0        0      519 2023-05-22 15:15:31.815984 dash_extensions-1.0.1/dash_extensions/_imports_.py
--rw-r--r--   0        0        0   292596 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/async-lottie.js
--rw-r--r--   0        0        0  1063846 2023-05-22 15:15:29.799974 dash_extensions-1.0.1/dash_extensions/async-lottie.js.map
--rw-r--r--   0        0        0   838722 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/async-mermaid.js
--rw-r--r--   0        0        0      108 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/async-mermaid.js.LICENSE.txt
--rw-r--r--   0        0        0  2940311 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/async-mermaid.js.map
--rw-r--r--   0        0        0   125714 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/dash_extensions.min.js
--rw-r--r--   0        0        0      342 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/dash_extensions.min.js.LICENSE.txt
--rw-r--r--   0        0        0   429994 2023-05-22 15:15:29.795974 dash_extensions-1.0.1/dash_extensions/dash_extensions.min.js.map
--rw-r--r--   0        0        0     2232 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/dash_extensions/dataiku.py
--rw-r--r--   0        0        0    45572 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/dash_extensions/enrich.py
--rw-r--r--   0        0        0     1520 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/dash_extensions/javascript.py
--rw-r--r--   0        0        0    20497 2023-05-22 15:15:31.815984 dash_extensions-1.0.1/dash_extensions/metadata.json
--rw-r--r--   0        0        0     2357 2023-05-22 15:15:30.987980 dash_extensions-1.0.1/dash_extensions/package-info.json
--rw-r--r--   0        0        0     3468 2023-05-22 15:14:01.747503 dash_extensions-1.0.1/dash_extensions/snippets.py
--rw-r--r--   0        0        0      957 2023-05-22 15:14:01.751503 dash_extensions-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2744 1970-01-01 00:00:00.000000 dash_extensions-1.0.1/setup.py
--rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 dash_extensions-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1877 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/README.md
+-rw-r--r--   0        0        0     2492 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/dash_extensions/__init__.py
+-rw-r--r--   0        0        0      478 2023-07-31 12:48:23.152889 dash_extensions-1.0.2/dash_extensions/_imports_.py
+-rw-r--r--   0        0        0     2232 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/dash_extensions/dataiku.py
+-rw-r--r--   0        0        0    46600 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/dash_extensions/enrich.py
+-rw-r--r--   0        0        0     1520 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/dash_extensions/javascript.py
+-rw-r--r--   0        0        0     3468 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/dash_extensions/snippets.py
+-rw-r--r--   0        0        0     1031 2023-07-31 12:46:14.943163 dash_extensions-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2781 1970-01-01 00:00:00.000000 dash_extensions-1.0.2/setup.py
+-rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 dash_extensions-1.0.2/PKG-INFO
```

### Comparing `dash_extensions-1.0.1/LICENSE` & `dash_extensions-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/README.md` & `dash_extensions-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/dash_extensions/__init__.py` & `dash_extensions-1.0.2/dash_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/dash_extensions/dataiku.py` & `dash_extensions-1.0.2/dash_extensions/dataiku.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/dash_extensions/enrich.py` & `dash_extensions-1.0.2/dash_extensions/enrich.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+import dataclasses
 import functools
 import hashlib
+import inspect
 import json
 import logging
 import secrets
 import struct
 import sys
 import threading
 import uuid
@@ -41,17 +43,20 @@
 from dash._utils import patch_collections_abc
 from dash.dependencies import _Wildcard, DashDependency  # lgtm [py/unused-import]
 from dash.development.base_component import Component
 from flask import session
 from flask_caching.backends import FileSystemCache, RedisCache
 from more_itertools import flatten
 from collections import defaultdict
-from typing import Dict, Callable, List, Union, Any, Tuple, Optional
+from typing import Dict, Callable, List, Union, Any, Tuple, Optional, Generic, TypeVar
 from datetime import datetime
 from dash_extensions import CycleBreaker
+from dataclass_wizard import fromdict, asdict
+
+T = TypeVar("T")
 
 _wildcard_mappings = {ALL: "<ALL>", MATCH: "<MATCH>", ALLSMALLER: "<ALLSMALLER>"}
 _wildcard_values = list(_wildcard_mappings.values())
 
 DEPENDENCY_APPEND_PREFIX = "dash_extensions_"
 
 
@@ -1012,14 +1017,85 @@
     if isinstance(i, dict):
         i = json.dumps({k: i[k] for k in sorted(i) if i[k] not in [ALL, MATCH, ALLSMALLER]})
     return f"{i}_{p}"
 
 
 # endregion
 
+# region SerializationTransform
+
+class SerializationTransform(DashTransform):
+
+    def apply_serverside(self, callbacks):
+        for callback in callbacks:
+            f = callback.f
+            callback.f = self._unpack_pack_callback(callback)(f)
+        return callbacks
+
+    def _try_load(self, data: Any, ann=None):
+        raise NotImplementedError
+
+    def _try_dump(self, obj: Any):
+        raise NotImplementedError
+
+    def _unpack_pack_callback(self, callback):
+        full_arg_spec = inspect.getfullargspec(callback.f)
+
+        def unpack_pack_args(f):
+            @functools.wraps(f)
+            def decorated_function(*args, **kwargs):
+                args = list(args)
+                # Replace args and kwargs. # TODO: Is recursion needed?
+                for i, arg in enumerate(args):
+                    an = full_arg_spec.annotations.get(full_arg_spec.args[i])
+                    value = [self._try_load(a, an) for a in arg] if isinstance(arg, list) else self._try_load(arg, an)
+                    args[i] = value
+                for key in kwargs:
+                    arg = kwargs[key]
+                    an = full_arg_spec.annotations.get(key)
+                    value = [self._try_load(a, an) for a in arg] if isinstance(arg, list) else self._try_load(arg, an)
+                    kwargs[key] = value
+                # Evaluate function.
+                data = f(*args, **kwargs)
+                # Capture outputs.
+                data = self._try_dump(data)
+                if isinstance(data, list):
+                    data = [self._try_dump(element) for element in data]
+                if isinstance(data, tuple):
+                    data = tuple([self._try_dump(element) for element in data])
+                if isinstance(data, dict):
+                    data = {key: self._try_dump(data[key]) for key in data}
+                return data
+
+            return decorated_function
+
+        return unpack_pack_args
+
+    def sort_key(self):
+        return 0
+
+# endregion
+
+# region DataclassTransform
+
+class DataclassTransform(SerializationTransform):
+
+    def _try_load(self, data: Any, ann=None) -> Any:
+        if not dataclasses.is_dataclass(ann):
+            return data
+        return fromdict(ann, data)
+
+    def _try_dump(self, obj: Any) -> Any:
+        if not dataclasses.is_dataclass(obj):
+            return obj
+        return asdict(obj)
+
+
+# endregion
+
 # region Server side output transform
 
 
 class ServersideBackend:
     def get(self, key, ignore_expired=False):
         raise NotImplementedError()
 
@@ -1093,42 +1169,36 @@
                  arg_check=True):
         super().__init__(component_id, component_property, allow_duplicate)
         self.backend = backend
         self.session_check = session_check
         self.arg_check = arg_check
 
 
-class ServersideOutputTransform(DashTransform):
+class ServersideOutputTransform(SerializationTransform):
     prefix: str = "SERVERSIDE_"
 
     def __init__(self,
                  backends: Optional[List[ServersideBackend]] = None,
                  default_backend: Optional[ServersideBackend] = None):
         super().__init__()
         # Per default, use file system backend.
         if backends is None:
             backends = [FileSystemBackend()]
         self._default_backend: ServersideBackend = backends[0] if default_backend is None else default_backend
         # Setup registry for easy/fast access.
         self._backend_registry: Dict[str, ServersideBackend] = {backend.uid: backend for backend in backends}
 
-    def apply_serverside(self, callbacks):
-        for callback in callbacks:
-            f = callback.f
-            callback.f = self._unpack_pack_callback(callback)(f)
-        return callbacks
-
-    def _try_load(self, obj: Any) -> Any:
-        if not isinstance(obj, str):
-            return obj
-        if not obj.startswith(self.prefix):
-            return obj
-        data = json.loads(obj[len(self.prefix):])
-        backend = self._backend_registry[data["backend_uid"]]
-        value = backend.get(data["key"], ignore_expired=True)
+    def _try_load(self, data: Any, ann=None) -> Any:
+        if not isinstance(data, str):
+            return data
+        if not data.startswith(self.prefix):
+            return data
+        obj = json.loads(data[len(self.prefix):])
+        backend = self._backend_registry[obj["backend_uid"]]
+        value = backend.get(obj["key"], ignore_expired=True)
         return value
 
     def _try_dump(self, obj: Any) -> Any:
         if not isinstance(obj, Serverside):
             return obj
         backend_uid = obj.backend_uid
         # If not backend it set, use the default.
@@ -1137,47 +1207,18 @@
         # Dump the data.
         backend = self._backend_registry[backend_uid]
         backend.set(obj.key, obj.value)
         # Return lookup structure.
         data = dict(backend_uid=backend_uid, key=obj.key)
         return f"{self.prefix}{json.dumps(data)}"
 
-    def _unpack_pack_callback(self, callback):
-        def unpack_pack_args(f):
-            @functools.wraps(f)
-            def decorated_function(*args, **kwargs):
-                args = list(args)
-                # Replace args and kwargs. # TODO: Is recursion needed?
-                for i, arg in enumerate(args):
-                    value = [self._try_load(a) for a in arg] if isinstance(arg, list) else self._try_load(arg)
-                    args[i] = value
-                for key in kwargs:
-                    arg = kwargs[key]
-                    value = [self._try_load(a) for a in arg] if isinstance(arg, list) else self._try_load(arg)
-                    kwargs[key] = value
-                # Evaluate function.
-                data = f(*args, **kwargs)
-                # Capture serverside outputs.
-                data = self._try_dump(data)
-                if isinstance(data, list):
-                    data = [self._try_dump(element) for element in data]
-                if isinstance(data, tuple):
-                    data = tuple([self._try_dump(element) for element in data])
-                if isinstance(data, dict):
-                    data = {key: self._try_dump(data[key]) for key in data}
-                return data
-
-            return decorated_function
-
-        return unpack_pack_args
-
 
-class Serverside:
+class Serverside(Generic[T]):
 
-    def __init__(self, value: Any, key: str = None, backend: Union[ServersideBackend, str, None] = None):
+    def __init__(self, value: T, key: str = None, backend: Union[ServersideBackend, str, None] = None):
         self.value = value
         self.key: str = str(uuid.uuid4()) if key is None else key
         self.backend_uid: str = backend.uid if isinstance(backend, ServersideBackend) else backend
 
 
 # endregion
```

### Comparing `dash_extensions-1.0.1/dash_extensions/javascript.py` & `dash_extensions-1.0.2/dash_extensions/javascript.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/dash_extensions/snippets.py` & `dash_extensions-1.0.2/dash_extensions/snippets.py`

 * *Files identical despite different names*

### Comparing `dash_extensions-1.0.1/pyproject.toml` & `dash_extensions-1.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 [tool.poetry]
 name = "dash-extensions"
-version = "1.0.1"
+version = "1.0.2"
 description = "Extensions for Plotly Dash."
 authors = ["emher <emil.h.eriksen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://dash-extensions.com"
 repository = "https://github.com/thedirtyfew/dash-extensions"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 dash = ">=2.9.3"
 more-itertools = "^9.0.0"
 jsbeautifier = "^1.14.3"
 Flask-Caching = "2.0.2"
 dash-mantine-components = {version = "^0.11.1", optional = true}
+dataclass-wizard = "^0.22.2"
 
 [tool.poetry.extras]
 mantine = ["dash-mantine-components"]
 
 [tool.poetry.dev-dependencies]
 dash = {extras = ["dev", "testing"], version = "^2.8.1"}
 pytest-cov = "^4.0.0"
 black = "^22.12.0"
 pandas = ">=1.5.3"
 quart = "^0.18.3"
-starlette = "^0.25.0"
+starlette = "^0.27.0"
+requests = "^2.31.0"
+certifi = "^2023.07.22"
 uvicorn = "^0.20.0"
 sse-starlette = "^1.2.1"
 urllib3 = "^1.26.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dash_extensions-1.0.1/setup.py` & `dash_extensions-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,24 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Flask-Caching==2.0.2',
  'dash>=2.9.3',
+ 'dataclass-wizard>=0.22.2,<0.23.0',
  'jsbeautifier>=1.14.3,<2.0.0',
  'more-itertools>=9.0.0,<10.0.0']
 
 extras_require = \
 {'mantine': ['dash-mantine-components>=0.11.1,<0.12.0']}
 
 setup_kwargs = {
     'name': 'dash-extensions',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'Extensions for Plotly Dash.',
     'long_description': '[![PyPI Latest Release](https://img.shields.io/pypi/v/dash-extensions.svg)](https://pypi.org/project/dash-extensions/)\n[![codecov](https://img.shields.io/codecov/c/github/thedirtyfew/dash-extensions?logo=codecov)](https://codecov.io/gh/thedirtyfew/dash-extensions)\n[![Testing](https://github.com/thedirtyfew/dash-extensions/actions/workflows/python-test.yml/badge.svg)](https://github.com/thedirtyfew/dash-extensions/actions/workflows/python-test.yml)\n[![CodeQL](https://github.com/thedirtyfew/dash-extensions/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/thedirtyfew/dash-extensions/actions/workflows/codeql-analysis.yml)\n\nThe `dash-extensions` package is a collection of utility functions, syntax extensions, and Dash components that aim to improve the Dash development experience. It can be divided in four main pillars,\n\n* The `enrich` module, which contains various enriched versions of Dash components\n* A number of custom components, e.g. the `Websocket` component, which enables real-time communication and push notifications\n* The `javascript` module, which contains functionality to ease the interplay between Dash and JavaScript\n* The `snippets` module, which contains a collection of utility functions (documentation limited to source code comments)\n\nThe `enrich` module enables a number of _transforms_ that add functionality and/or syntactic sugar to Dash. Examples include\n\n* Making it possible to avoid invoking a callback _if it is already running_ via the `BlockingCallbackTransform`\n* Enabling logging from within Dash callbacks via the `LogTransform`\n* Improving app performance via the `ServersideOutputTransform`\n\nto name a few. To enable interactivity, the documentation has been moved to a [separate page](http://dash-extensions.com).\n\nNB: The 1.0.0 version introduces a number of breaking changes, see documentation for details.\n',
     'author': 'emher',
     'author_email': 'emil.h.eriksen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dash-extensions.com',
```

### Comparing `dash_extensions-1.0.1/PKG-INFO` & `dash_extensions-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-extensions
-Version: 1.0.1
+Version: 1.0.2
 Summary: Extensions for Plotly Dash.
 Home-page: https://dash-extensions.com
 License: MIT
 Author: emher
 Author-email: emil.h.eriksen@gmail.com
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mantine
 Requires-Dist: Flask-Caching (==2.0.2)
 Requires-Dist: dash (>=2.9.3)
 Requires-Dist: dash-mantine-components (>=0.11.1,<0.12.0) ; extra == "mantine"
+Requires-Dist: dataclass-wizard (>=0.22.2,<0.23.0)
 Requires-Dist: jsbeautifier (>=1.14.3,<2.0.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Project-URL: Repository, https://github.com/thedirtyfew/dash-extensions
 Description-Content-Type: text/markdown
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/dash-extensions.svg)](https://pypi.org/project/dash-extensions/)
 [![codecov](https://img.shields.io/codecov/c/github/thedirtyfew/dash-extensions?logo=codecov)](https://codecov.io/gh/thedirtyfew/dash-extensions)
```

