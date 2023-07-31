# Comparing `tmp/anthropic-0.3.6.tar.gz` & `tmp/anthropic-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.3.6.tar", max compression
+gzip compressed data, was "anthropic-0.3.7.tar", max compression
```

## Comparing `anthropic-0.3.6.tar` & `anthropic-0.3.7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.6/LICENSE
--rw-r--r--   0        0        0     9649 2023-07-22 02:16:31.626443 anthropic-0.3.6/README.md
--rw-r--r--   0        0        0     1925 2023-07-22 02:16:31.626782 anthropic-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.6/src/anthropic/__init__.py
--rw-r--r--   0        0        0    46809 2023-06-26 21:50:36.628016 anthropic-0.3.6/src/anthropic/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.6/src/anthropic/_base_exceptions.py
--rw-r--r--   0        0        0    15329 2023-06-26 21:50:36.628587 anthropic-0.3.6/src/anthropic/_client.py
--rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.6/src/anthropic/_constants.py
--rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.6/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.6/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.6/src/anthropic/_qs.py
--rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.6/src/anthropic/_resource.py
--rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.6/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.6/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.6/src/anthropic/_types.py
--rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.6/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.6/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.6/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0      128 2023-07-22 02:16:31.627239 anthropic-0.3.6/src/anthropic/_version.py
--rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.6/src/anthropic/pagination.py
--rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.6/src/anthropic/py.typed
--rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.6/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.6/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.6/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.6/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.6/src/anthropic/types/completion.py
--rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.6/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0    10602 1970-01-01 00:00:00.000000 anthropic-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.7/LICENSE
+-rw-r--r--   0        0        0     9994 2023-07-31 16:20:19.817632 anthropic-0.3.7/README.md
+-rw-r--r--   0        0        0     1925 2023-07-31 16:20:19.817881 anthropic-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.7/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    47846 2023-07-31 16:20:19.818281 anthropic-0.3.7/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.7/src/anthropic/_base_exceptions.py
+-rw-r--r--   0        0        0    15554 2023-07-31 16:20:19.818545 anthropic-0.3.7/src/anthropic/_client.py
+-rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.7/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.7/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.7/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.7/src/anthropic/_qs.py
+-rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.7/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.7/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.7/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.7/src/anthropic/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.7/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.7/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.7/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      128 2023-07-31 16:20:19.818825 anthropic-0.3.7/src/anthropic/_version.py
+-rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.7/src/anthropic/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.7/src/anthropic/py.typed
+-rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.7/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.7/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.7/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.7/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.7/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.7/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0    10947 1970-01-01 00:00:00.000000 anthropic-0.3.7/PKG-INFO
```

### Comparing `anthropic-0.3.6/LICENSE` & `anthropic-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/README.md` & `anthropic-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -277,37 +277,41 @@
 If you need to, you can override it by setting default headers per-request or on the client object.
 
 Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
 
 ```python
 from anthropic import Anthropic
 
-anthropic = Anthropic(
+client = Anthropic(
     default_headers={"anthropic-version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
 ```python
 import httpx
 from anthropic import Anthropic
 
-anthropic = Anthropic(
+client = Anthropic(
     # Use a custom base URL
     base_url="http://my.test.server.example.com:8083",
     proxies="http://my.test.proxy.example.com",
     transport=httpx.HTTPTransport(local_address="0.0.0.0"),
 )
 ```
 
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
+## Advanced: Managing HTTP resources
+
+By default we will close the underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__) is called but you can also manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/anthropics/anthropic-sdk-python/issues) with questions, bugs, or suggestions.
```

### Comparing `anthropic-0.3.6/pyproject.toml` & `anthropic-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic"
-version = "0.3.6"
+version = "0.3.7"
 description = "Client library for the anthropic API"
 readme = "README.md"
 authors = ["Anthropic <support@anthropic.com>"]
 license = "MIT"
 repository = "https://github.com/anthropics/anthropic-sdk-python"
 packages = [
   { include = "anthropic", from = "src" }
```

### Comparing `anthropic-0.3.6/src/anthropic/__init__.py` & `anthropic-0.3.7/src/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_base_client.py` & `anthropic-0.3.7/src/anthropic/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import json
 import time
 import uuid
 import inspect
 import platform
+from types import TracebackType
 from random import random
 from typing import (
     Any,
     Dict,
     Type,
     Union,
     Generic,
@@ -673,14 +674,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        self._client.close()
+
+    def __enter__(self: _T) -> _T:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        self.close()
+
     @overload
     def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         remaining_retries: Optional[int] = None,
         *,
@@ -1005,14 +1027,35 @@
             timeout=timeout,
             proxies=proxies,  # type: ignore
             transport=transport,  # type: ignore
             limits=limits,
             headers={"Accept": "application/json"},
         )
 
+    def is_closed(self) -> bool:
+        return self._client.is_closed
+
+    async def close(self) -> None:
+        """Close the underlying HTTPX client.
+
+        The client will *not* be usable after this.
+        """
+        await self._client.aclose()
+
+    async def __aenter__(self: _T) -> _T:
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> None:
+        await self.close()
+
     @overload
     async def request(
         self,
         cast_to: Type[ResponseT],
         options: FinalRequestOptions,
         *,
         stream: Literal[False] = False,
```

### Comparing `anthropic-0.3.6/src/anthropic/_base_exceptions.py` & `anthropic-0.3.7/src/anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_client.py` & `anthropic-0.3.7/src/anthropic/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import os
+import asyncio
 from typing import Union, Mapping, Optional
 
 import httpx
 from tokenizers import Tokenizer  # type: ignore[import]
 
 from . import resources
 from ._qs import Querystring
@@ -77,40 +78,39 @@
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new synchronous anthropic client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
-        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         - `api_key` from `ANTHROPIC_API_KEY`
+        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         """
-        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", "")
+        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", None)
+        self.api_key = api_key
+
+        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
+        self.auth_token = auth_token or auth_token_envvar or None
 
         if base_url is None:
-            base_url = "https://api.anthropic.com"
+            base_url = f"https://api.anthropic.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.api_key = api_key
-
-        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
-        self.auth_token = auth_token or auth_token_envvar or None
-
         self._default_stream_cls = Stream
 
         self.completions = resources.Completions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -212,14 +212,17 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        self.close()
+
     def count_tokens(
         self,
         text: str,
     ) -> int:
         """Count the number of tokens in a given string"""
         # Note: tokenizer is untyped
         tokenizer = self.get_tokenizer()
@@ -262,40 +265,39 @@
         # outlining your use-case to help us decide if it should be
         # part of our public interface in the future.
         _strict_response_validation: bool = False,
     ) -> None:
         """Construct a new async anthropic client instance.
 
         This automatically infers the following arguments from their corresponding environment variables if they are not provided:
-        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         - `api_key` from `ANTHROPIC_API_KEY`
+        - `auth_token` from `ANTHROPIC_AUTH_TOKEN`
         """
-        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", "")
+        api_key = api_key or os.environ.get("ANTHROPIC_API_KEY", None)
+        self.api_key = api_key
+
+        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
+        self.auth_token = auth_token or auth_token_envvar or None
 
         if base_url is None:
-            base_url = "https://api.anthropic.com"
+            base_url = f"https://api.anthropic.com"
 
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             transport=transport,
             proxies=proxies,
             limits=connection_pool_limits,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.api_key = api_key
-
-        auth_token_envvar = os.environ.get("ANTHROPIC_AUTH_TOKEN", None)
-        self.auth_token = auth_token or auth_token_envvar or None
-
         self._default_stream_cls = AsyncStream
 
         self.completions = resources.AsyncCompletions(self)
 
     @property
     def qs(self) -> Querystring:
         return Querystring(array_format="comma")
@@ -397,14 +399,20 @@
             default_query=params,
         )
 
     # Alias for `copy` for nicer inline usage, e.g.
     # client.with_options(timeout=10).foo.create(...)
     with_options = copy
 
+    def __del__(self) -> None:
+        try:
+            asyncio.get_running_loop().create_task(self.close())
+        except Exception:
+            pass
+
     async def count_tokens(
         self,
         text: str,
     ) -> int:
         """Count the number of tokens in a given string"""
         # Note: tokenizer is untyped
         tokenizer = await self.get_tokenizer()
```

### Comparing `anthropic-0.3.6/src/anthropic/_exceptions.py` & `anthropic-0.3.7/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_models.py` & `anthropic-0.3.7/src/anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_qs.py` & `anthropic-0.3.7/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_resource.py` & `anthropic-0.3.7/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_streaming.py` & `anthropic-0.3.7/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_tokenizers.py` & `anthropic-0.3.7/src/anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_types.py` & `anthropic-0.3.7/src/anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_utils/__init__.py` & `anthropic-0.3.7/src/anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_utils/_transform.py` & `anthropic-0.3.7/src/anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/_utils/_utils.py` & `anthropic-0.3.7/src/anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/resources/completions.py` & `anthropic-0.3.7/src/anthropic/resources/completions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/tokenizer.json` & `anthropic-0.3.7/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/types/completion.py` & `anthropic-0.3.7/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/src/anthropic/types/completion_create_params.py` & `anthropic-0.3.7/src/anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.6/PKG-INFO` & `anthropic-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.3.6
+Version: 0.3.7
 Summary: Client library for the anthropic API
 Home-page: https://github.com/anthropics/anthropic-sdk-python
 License: MIT
 Author: Anthropic
 Author-email: support@anthropic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -302,37 +302,41 @@
 If you need to, you can override it by setting default headers per-request or on the client object.
 
 Be aware that doing so may result in incorrect types and other unexpected or undefined behavior in the SDK.
 
 ```python
 from anthropic import Anthropic
 
-anthropic = Anthropic(
+client = Anthropic(
     default_headers={"anthropic-version": "My-Custom-Value"},
 )
 ```
 
 ## Advanced: Configuring custom URLs, proxies, and transports
 
 You can configure the following keyword arguments when instantiating the client:
 
 ```python
 import httpx
 from anthropic import Anthropic
 
-anthropic = Anthropic(
+client = Anthropic(
     # Use a custom base URL
     base_url="http://my.test.server.example.com:8083",
     proxies="http://my.test.proxy.example.com",
     transport=httpx.HTTPTransport(local_address="0.0.0.0"),
 )
 ```
 
 See the httpx documentation for information about the [`proxies`](https://www.python-httpx.org/advanced/#http-proxying) and [`transport`](https://www.python-httpx.org/advanced/#custom-transports) keyword arguments.
 
+## Advanced: Managing HTTP resources
+
+By default we will close the underlying HTTP connections whenever the client is [garbage collected](https://docs.python.org/3/reference/datamodel.html#object.__del__) is called but you can also manually close the client using the `.close()` method if desired, or with a context manager that closes when exiting.
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please open an [issue](https://www.github.com/anthropics/anthropic-sdk-python/issues) with questions, bugs, or suggestions.
```

