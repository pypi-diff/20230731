# Comparing `tmp/fateful-0.3.0.tar.gz` & `tmp/fateful-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fateful-0.3.0.tar", last modified: Tue Jul 18 16:16:56 2023, max compression
+gzip compressed data, was "fateful-0.4.0.tar", last modified: Mon Jul 31 13:16:39 2023, max compression
```

## Comparing `fateful-0.3.0.tar` & `fateful-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     6235 2023-07-18 16:16:36.761087 fateful-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/__init__.py
--rw-r--r--   0        0        0     2750 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/http.py
--rw-r--r--   0        0        0     2053 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/json.py
--rw-r--r--   0        0        0        0 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/__init__.py
--rw-r--r--   0        0        0    17438 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/async_result.py
--rw-r--r--   0        0        0     2148 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/container.py
--rw-r--r--   0        0        0      804 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/effect.py
--rw-r--r--   0        0        0     6632 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/func.py
--rw-r--r--   0        0        0    12595 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/option.py
--rw-r--r--   0        0        0     7157 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/monad/result.py
--rw-r--r--   0        0        0        0 2023-07-18 16:16:36.761087 fateful-0.3.0/fateful/py.typed.py
--rw-r--r--   0        0        0      679 2023-07-18 16:16:56.472957 fateful-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4752 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_async_try.py
--rw-r--r--   0        0        0     1833 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_http.py
--rw-r--r--   0        0        0      525 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_impure.py
--rw-r--r--   0        0        0     1829 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_json.py
--rw-r--r--   0        0        0     8198 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_option.py
--rw-r--r--   0        0        0     3035 2023-07-18 16:16:36.765087 fateful-0.3.0/tests/test_result.py
--rw-r--r--   0        0        0     6485 1970-01-01 00:00:00.000000 fateful-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     6893 2023-07-31 13:16:23.812910 fateful-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 13:16:23.812910 fateful-0.4.0/fateful/__init__.py
+-rw-r--r--   0        0        0     2669 2023-07-31 13:16:23.812910 fateful-0.4.0/fateful/container.py
+-rw-r--r--   0        0        0     2706 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/http.py
+-rw-r--r--   0        0        0     1008 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/json.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/__init__.py
+-rw-r--r--   0        0        0    17438 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/async_result.py
+-rw-r--r--   0        0        0     2148 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/container.py
+-rw-r--r--   0        0        0      804 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/effect.py
+-rw-r--r--   0        0        0     6632 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/func.py
+-rw-r--r--   0        0        0    12595 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/option.py
+-rw-r--r--   0        0        0     7157 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/monad/result.py
+-rw-r--r--   0        0        0        0 2023-07-31 13:16:23.816910 fateful-0.4.0/fateful/py.typed.py
+-rw-r--r--   0        0        0      859 2023-07-31 13:16:39.453092 fateful-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4752 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_async_try.py
+-rw-r--r--   0        0        0     1833 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_http.py
+-rw-r--r--   0        0        0      525 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_impure.py
+-rw-r--r--   0        0        0     2369 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_json.py
+-rw-r--r--   0        0        0     8269 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_option.py
+-rw-r--r--   0        0        0     3035 2023-07-31 13:16:23.816910 fateful-0.4.0/tests/test_result.py
+-rw-r--r--   0        0        0     7386 1970-01-01 00:00:00.000000 fateful-0.4.0/PKG-INFO
```

### Comparing `fateful-0.3.0/README.md` & `fateful-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 # fateful
 
-*Option* and *Result* container for python !
+*Option* and *Result* container for python
 
 ![fateful](./docs/img/fateful.png)
 
 documentation: https://jerkos.github.io/fateful/
 
 Python has some great functional features. The most notable ones are list / dict
 comprehensions. However, when you start to chain function calls (or predicate
  or whatever), it becomes rapidly a pain.
 
  In some famous languages, we have *Option* and *Result* monad helping user to handle
  optional values (i.e. None values) and possibly failing computation (Rust, Java, Kotlin...)
 
- So, this very small Python library implements those monads - Option and Result -
+ So, this very small Python library implements those monads - Option, Result or AsyncResult -
  providing a way to handle optional values / computation failures in a functional style.
 
  A focus has been made to typing (but can still be improved of course !)
 
 
+## Installation
+
+```bash
+pip install fateful
+
+pip install fateful[http] # install aiohttp to enable async api calls helper
+
+pip install fateful[orjson] # install orjson a fast json implementation
+
+pip install fateful[all] # install all optional dependencies
+```
+
 ## Option monad
 
-The Option Monad, also known as the Maybe Monad, is a concept from functional programming that provides a way to handle optional values in a more controlled and expressive manner. It helps avoid null or undefined errors by encapsulating a value that may or may not be present. The key idea behind the Option Monad is to provide a container that can either hold a value (Some) or indicate the absence of a value (None).
+The Option Monad, also known as the Maybe Monad, is a concept from functional programming that provides
+a way to handle optional values in a more controlled and expressive manner. It helps avoid null or
+undefined errors by encapsulating a value that may or may not be present. The key idea behind the
+Option Monad is to provide a container that can either hold a value (Some) or indicate the absence
+of a value (None).
 
 The Option Monad offers several benefits, including:
 
 - Safety: It helps prevent null or undefined errors that can occur when working with optional values.
 - Clarity: It makes the presence or absence of a value explicit, enhancing the readability of code.
-- Composability: It allows for chaining operations on optional values without explicitly checking for null or undefined values.
-- Functional style: It promotes functional programming principles by encouraging pure functions and immutability.
+- Composability: It allows for chaining operations on optional values without explicitly checking for
+  null or undefined values.
+- Functional style: It promotes functional programming principles by encouraging pure functions and
+  immutability.
 
 
 When you do not know if a value is None or is actually a real value / object, use **opt**
 to wrap it into an option
 
 ``` python
 from fateful import opt, Null, Some
@@ -49,15 +67,15 @@
 
 >>> opt(None).get() # same as none.get()
 Traceback (most recent call last):
 ...
 ValueError: Option is empty
 ```
 
-Option monad implements tu iteration protocl
+Option monad implements the iteration protocl
 
 ```python
 >>> o = opt([1, 2, 3]).for_each(print)
 [1, 2, 3]
 
 >>> a = opt('optional option value')
 >>> for i in a:
@@ -87,15 +105,15 @@
 from fateful.monad.option import option
 result = option("some").map(lambda x: len(x) * 2).or_(0)
 ```
 
 An option can contain another option type but can be flattened
 
 ```python
-x = option(option(option(1))).flatten() # x is Some[int]
+x = option(option(option(1))).flatten() # x is Some[Some[Some[int]]]
 
 y: Some[Some[Some[int]]] = Some(Some(Some(1)))
 x: Some[int] = Some(Some(Some(1))).flatten()
 ```
 
 We can lift an function to return an *option* type using a decorator
 
@@ -110,35 +128,41 @@
 
 x: Some[int] = maybe(2)
 x: Empty = maybe(0)
 ```
 
 ## Result monad
 
-The Result Monad is another concept from functional programming that is used to handle computations that may produce a successful result or a failure. It provides a way to encapsulate the outcome of an operation, allowing you to handle and propagate errors in a controlled manner.
-
-The Result Monad typically has two possible states: Ok (representing a successful result) and Err (representing a failure or an error condition). The Ok state contains the successful result value, while the Err state contains information about the failure, such as an error message or an error object.
+The Result Monad is another concept from functional programming that is used to handle computations
+that may produce a successful result or a failure. It provides a way to encapsulate the outcome of
+an operation, allowing you to handle and propagate errors in a controlled manner.
+
+The Result Monad typically has two possible states: Ok (representing a successful result) and Err
+(representing a failure or an error condition). The Ok state contains the successful result value,
+while the Err state contains information about the failure, such as an error message or an error object.
 
 The Result Monad offers several benefits:
 
 - Explicit error handling: It makes error handling explicit and separates the handling of successful results from error conditions.
 - Propagation of errors: It allows errors to be easily propagated through a chain of operations, avoiding the need for explicit error-checking at each step.
 - Composition: It enables the chaining and composition of operations on results in a concise and expressive manner.
 - Error recovery: It provides mechanisms to handle and recover from errors, such as by mapping to alternative values or applying fallback strategies.
 
 ```python
 def may_fail(x: int) -> float:
     return 1 / x
 
-from fateful.monad.try_ import Try
+from fateful.monad.resut import sync_try
+
+r: Ok[float] | Err[ZeroDivisionError] = sync_try(may_fail, ZeroDivisionError)(1)
+result = sync_try(may_fail, ZeroDivisionError)(1).or_(10.0)
 
-result = Try.of(may_fail).on_error((ZeroDivisionError,))(1).or_(10.0)
 assert result == 1.0
 
-result = Try.of(may_fail).on_error((ZeroDivisionError,))(0).or_(10.0)
+result = sync_try(may_fail, ZeroDivisonError)(0).or_(10.0)
 assert result == 10.0
 
 
 ```
 
 ## Async Result
 
@@ -146,49 +170,66 @@
 
 
 ```python
 async def divide_async(a, b):
     await asyncio.sleep(0.1)
     return a / b
 
-value = await async_try(add_async, 1, 1).or_else(lambda: 4)
-value = await async_try(add_async, 1, 1).or_(4)
-divide: AsyncResult[..., float, ZeroDivisionError] = async_try(add_async, 1, 1)
-divide.on_errors((ValueError,)) # mypy / pyright complains because ZeroDiisionError does not match ValueError
-result: Ok[float] | Err[ZeroDivisionError] = await divide.on_errors((ZeroDivisionError,)).execute()
+from fateful.monad import async_try
+
+value = await async_try(add_async)( 1, 1).or_else(lambda: 4)
+
+value = await async_try(add_async)(1, 1).or_(4)
+
+divide: AsyncResult[..., float, ZeroDivisionError] = async_try(add_async, ZeroDivisionError)(1, 1)
+
+result: Ok[float] | Err[ZeroDivisionError] = await divide..execute()
 
 # transforming value
 value = await divide.map(lambda r: r - 100).or_(0)
 
-match (await divide.on_errors((ZeroDivisionError,)).execute()):
+match (await divide.execute()):
     case Ok(val):
         return val
     case Err(err):
         raise err
     case _:
         raise TypeError("Never supposed to happen")
 ```
 
 ## Http module
 
 Miscellaneous functions dealing with http client functions
 
-Wraps aihttp for perform http call and parsing results optionnaly as json
+Wraps aiohttp for perform http call and parsing results optionnaly as json
 
-```python
+*aiohttp* is a library of choice for making http requests. A good alternative is *httpx*
+but various benchmarks show that it is slightly slower.
 
+```python
+page_content: str = await try_get("http://google.com").or_raise()
 ```
 
+## Container module
+
+Simple subclass to return option monad when getting values
+implementation of list and dict
+
+```python
+x = opt_list([1,2,3])
+v: Some[int] = x.at(0)
+v: Empty = x.at(12)
+```
 ## Json module
 
 Miscellaneous functions dealing with json (parsing, manipulating...)
 
 ``` python
->>> from fateful.json import obj
->>> i = obj({'z-index': 1000})
+>>> from fateful.json import opt_dict
+>>> i = opt_dict({'z-index': 1000})
 >>> i.toto = [4, 5, 6]
 >>> str(i)
 '{"z-index": 1000, "toto": [4, 5, 6]}'
 ```
 
 
 Notes: I found some python packages doing almost the same things. I did
```

### Comparing `fateful-0.3.0/fateful/http.py` & `fateful-0.4.0/fateful/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,95 +1,89 @@
 import logging
+import typing as t
 from enum import Enum
 from functools import partial
 from json import JSONDecodeError
-from typing import Any, Type
 
-from aiohttp import ClientError, ClientSession
+try:
+    from aiohttp import ClientError, ClientSession
+    from yarl import URL
+except ImportError:
+    logging.warning("aiohttp and yarl are not installed")
+    raise
 
-from fateful.json import JsArray, JsObject, try_parse
+from fateful.json import js_array, js_object, try_parse
 from fateful.monad.async_result import async_try
 from fateful.monad.result import Err, Ok
 
 
 class HttpMethods(str, Enum):
-    """ """
+    """A list of basic HTTP methods."""
 
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     PATCH = "PATCH"
     OPTIONS = "OPTIONS"
 
 
 class ContentType:
-    """ """
+    """Content-Type header values."""
 
     value = "Content-Type"
     APPLICATION_JSON = "application/json"
 
 
-class NetworkError(Exception):
-    """ """
-
-    ...
-
-
-class HttpException(NetworkError):
-    """ """
-
-    def __init__(self, code: int, detail: str):
-        self.code = code
-        self.detail = detail
-
-
-class NetworkException(NetworkError):
-    """ """
-
-    ...
+T = t.TypeVar("T")
 
 
 async def request(
     method: HttpMethods,
-    url,
+    url: str | URL,
     /,
     *,
     session: ClientSession,
-    response_class: Type[Any] | None = None,
-    **kwargs: Any,
-) -> Ok[str | JsArray | JsObject | Any] | Err[
-    NetworkError | ClientError | JSONDecodeError | Exception
-]:
+    object_hook: type[T] | None = None,
+    **kwargs: t.Any,
+) -> Ok[str | js_array | js_object | T | list[T]] | Err[ClientError | JSONDecodeError]:
     """
     Generic method for making a request
     """
     try:
         async with session.request(method.value, url, **kwargs) as resp:
             try:
                 content_type = resp.headers.getall(ContentType.value)
                 is_json = ContentType.APPLICATION_JSON in content_type
+                resp.raise_for_status()
                 resp_as_text = await resp.text()
-                if resp.status >= 400:
-                    return Err(HttpException(resp.status, resp_as_text))
                 if is_json:
-                    return try_parse(resp_as_text, response_class=response_class)
+                    return try_parse(resp_as_text, object_hook=object_hook)
                 return Ok(resp_as_text)
             except ClientError as e:  # pragma: no cover
                 logging.error(e)
                 return Err(e)
     except ClientError as e:
         logging.exception(e)
         return Err(e)
 
 
 get = partial(request, HttpMethods.GET)
 
 
-def try_get(url, **kwargs):
+def try_get(url: str | URL, **kwargs):
+    """
+    return an async try of get
+
+    Args:
+        url: url to get
+
+    Returns:
+        : async try
+    """
     return async_try(get)(url, **kwargs)
 
 
 post = partial(request, HttpMethods.POST)
 
 
 def try_post(url, **kwargs):  # pragma: no cover
```

### Comparing `fateful-0.3.0/fateful/monad/async_result.py` & `fateful-0.4.0/fateful/monad/async_result.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/fateful/monad/container.py` & `fateful-0.4.0/fateful/monad/container.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/fateful/monad/effect.py` & `fateful-0.4.0/fateful/monad/effect.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/fateful/monad/func.py` & `fateful-0.4.0/fateful/monad/func.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/fateful/monad/option.py` & `fateful-0.4.0/fateful/monad/option.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/fateful/monad/result.py` & `fateful-0.4.0/fateful/monad/result.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/pyproject.toml` & `fateful-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -19,21 +19,31 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "fateful"
-version = "0.3.0"
-description = "rusty container"
+version = "0.4.0"
+description = "rusty Option and Result container for python. Ready for pattern matching and asyncio"
 authors = [
     { name = "Marco", email = "cram@hotmail.fr" },
 ]
 dependencies = [
-    "aiohttp>=3.8.4",
     "pampy>=0.3.0",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
+
+[project.optional-dependencies]
+http = [
+    "aiohttp >= 3.8.4",
+]
+orjson = [
+    "orjson",
+]
+all = [
+    "fateful[http,orjson]",
+]
```

### Comparing `fateful-0.3.0/tests/test_async_try.py` & `fateful-0.4.0/tests/test_async_try.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/tests/test_http.py` & `fateful-0.4.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/tests/test_impure.py` & `fateful-0.4.0/tests/test_impure.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/tests/test_option.py` & `fateful-0.4.0/tests/test_option.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import typing
 import unittest
 from functools import partial
 
 import pytest
+from aiohttp import ClientResponseError
 from assertpy import assert_that
 
-from fateful.http import HttpException
 from fateful.monad.container import EmptyError
 from fateful.monad.func import (
     MatchError,
     _,
     default,
     identity,
     raise_err,
@@ -139,16 +139,18 @@
             case Some(x):
                 print(x)
             case Err(e):
                 raise e
             case Empty():
                 logging.debug("Empty")
 
-        match Err(HttpException(400, detail="toto")):
-            case Err(HttpException(code=x)):
+        match Err(
+            ClientResponseError(None, (), status=400, message="toto")  # type: ignore
+        ):
+            case Err(ClientResponseError(status=x)):
                 print(f"Got {x} code from error")
 
         value = opt("tata")
         x = when(Some(_)).then(lambda x: "match first")
         default >> (partial(raise_error, MatchError()))
         value.match(
             when(Some(_)).then(lambda x: "match first"),
```

### Comparing `fateful-0.3.0/tests/test_result.py` & `fateful-0.4.0/tests/test_result.py`

 * *Files identical despite different names*

### Comparing `fateful-0.3.0/PKG-INFO` & `fateful-0.4.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,72 @@
 Metadata-Version: 2.1
 Name: fateful
-Version: 0.3.0
-Summary: rusty container
+Version: 0.4.0
+Summary: rusty Option and Result container for python. Ready for pattern matching and asyncio
 Author-Email: Marco <cram@hotmail.fr>
 License: MIT
 Requires-Python: >=3.10
-Requires-Dist: aiohttp>=3.8.4
 Requires-Dist: pampy>=0.3.0
+Requires-Dist: aiohttp>=3.8.4; extra == "http"
+Requires-Dist: orjson; extra == "orjson"
+Requires-Dist: fateful[http,orjson]; extra == "all"
+Provides-Extra: http
+Provides-Extra: orjson
+Provides-Extra: all
 Description-Content-Type: text/markdown
 
 # fateful
 
-*Option* and *Result* container for python !
+*Option* and *Result* container for python
 
 ![fateful](./docs/img/fateful.png)
 
 documentation: https://jerkos.github.io/fateful/
 
 Python has some great functional features. The most notable ones are list / dict
 comprehensions. However, when you start to chain function calls (or predicate
  or whatever), it becomes rapidly a pain.
 
  In some famous languages, we have *Option* and *Result* monad helping user to handle
  optional values (i.e. None values) and possibly failing computation (Rust, Java, Kotlin...)
 
- So, this very small Python library implements those monads - Option and Result -
+ So, this very small Python library implements those monads - Option, Result or AsyncResult -
  providing a way to handle optional values / computation failures in a functional style.
 
  A focus has been made to typing (but can still be improved of course !)
 
 
+## Installation
+
+```bash
+pip install fateful
+
+pip install fateful[http] # install aiohttp to enable async api calls helper
+
+pip install fateful[orjson] # install orjson a fast json implementation
+
+pip install fateful[all] # install all optional dependencies
+```
+
 ## Option monad
 
-The Option Monad, also known as the Maybe Monad, is a concept from functional programming that provides a way to handle optional values in a more controlled and expressive manner. It helps avoid null or undefined errors by encapsulating a value that may or may not be present. The key idea behind the Option Monad is to provide a container that can either hold a value (Some) or indicate the absence of a value (None).
+The Option Monad, also known as the Maybe Monad, is a concept from functional programming that provides
+a way to handle optional values in a more controlled and expressive manner. It helps avoid null or
+undefined errors by encapsulating a value that may or may not be present. The key idea behind the
+Option Monad is to provide a container that can either hold a value (Some) or indicate the absence
+of a value (None).
 
 The Option Monad offers several benefits, including:
 
 - Safety: It helps prevent null or undefined errors that can occur when working with optional values.
 - Clarity: It makes the presence or absence of a value explicit, enhancing the readability of code.
-- Composability: It allows for chaining operations on optional values without explicitly checking for null or undefined values.
-- Functional style: It promotes functional programming principles by encouraging pure functions and immutability.
+- Composability: It allows for chaining operations on optional values without explicitly checking for
+  null or undefined values.
+- Functional style: It promotes functional programming principles by encouraging pure functions and
+  immutability.
 
 
 When you do not know if a value is None or is actually a real value / object, use **opt**
 to wrap it into an option
 
 ``` python
 from fateful import opt, Null, Some
@@ -60,15 +83,15 @@
 
 >>> opt(None).get() # same as none.get()
 Traceback (most recent call last):
 ...
 ValueError: Option is empty
 ```
 
-Option monad implements tu iteration protocl
+Option monad implements the iteration protocl
 
 ```python
 >>> o = opt([1, 2, 3]).for_each(print)
 [1, 2, 3]
 
 >>> a = opt('optional option value')
 >>> for i in a:
@@ -98,15 +121,15 @@
 from fateful.monad.option import option
 result = option("some").map(lambda x: len(x) * 2).or_(0)
 ```
 
 An option can contain another option type but can be flattened
 
 ```python
-x = option(option(option(1))).flatten() # x is Some[int]
+x = option(option(option(1))).flatten() # x is Some[Some[Some[int]]]
 
 y: Some[Some[Some[int]]] = Some(Some(Some(1)))
 x: Some[int] = Some(Some(Some(1))).flatten()
 ```
 
 We can lift an function to return an *option* type using a decorator
 
@@ -121,35 +144,41 @@
 
 x: Some[int] = maybe(2)
 x: Empty = maybe(0)
 ```
 
 ## Result monad
 
-The Result Monad is another concept from functional programming that is used to handle computations that may produce a successful result or a failure. It provides a way to encapsulate the outcome of an operation, allowing you to handle and propagate errors in a controlled manner.
-
-The Result Monad typically has two possible states: Ok (representing a successful result) and Err (representing a failure or an error condition). The Ok state contains the successful result value, while the Err state contains information about the failure, such as an error message or an error object.
+The Result Monad is another concept from functional programming that is used to handle computations
+that may produce a successful result or a failure. It provides a way to encapsulate the outcome of
+an operation, allowing you to handle and propagate errors in a controlled manner.
+
+The Result Monad typically has two possible states: Ok (representing a successful result) and Err
+(representing a failure or an error condition). The Ok state contains the successful result value,
+while the Err state contains information about the failure, such as an error message or an error object.
 
 The Result Monad offers several benefits:
 
 - Explicit error handling: It makes error handling explicit and separates the handling of successful results from error conditions.
 - Propagation of errors: It allows errors to be easily propagated through a chain of operations, avoiding the need for explicit error-checking at each step.
 - Composition: It enables the chaining and composition of operations on results in a concise and expressive manner.
 - Error recovery: It provides mechanisms to handle and recover from errors, such as by mapping to alternative values or applying fallback strategies.
 
 ```python
 def may_fail(x: int) -> float:
     return 1 / x
 
-from fateful.monad.try_ import Try
+from fateful.monad.resut import sync_try
+
+r: Ok[float] | Err[ZeroDivisionError] = sync_try(may_fail, ZeroDivisionError)(1)
+result = sync_try(may_fail, ZeroDivisionError)(1).or_(10.0)
 
-result = Try.of(may_fail).on_error((ZeroDivisionError,))(1).or_(10.0)
 assert result == 1.0
 
-result = Try.of(may_fail).on_error((ZeroDivisionError,))(0).or_(10.0)
+result = sync_try(may_fail, ZeroDivisonError)(0).or_(10.0)
 assert result == 10.0
 
 
 ```
 
 ## Async Result
 
@@ -157,49 +186,66 @@
 
 
 ```python
 async def divide_async(a, b):
     await asyncio.sleep(0.1)
     return a / b
 
-value = await async_try(add_async, 1, 1).or_else(lambda: 4)
-value = await async_try(add_async, 1, 1).or_(4)
-divide: AsyncResult[..., float, ZeroDivisionError] = async_try(add_async, 1, 1)
-divide.on_errors((ValueError,)) # mypy / pyright complains because ZeroDiisionError does not match ValueError
-result: Ok[float] | Err[ZeroDivisionError] = await divide.on_errors((ZeroDivisionError,)).execute()
+from fateful.monad import async_try
+
+value = await async_try(add_async)( 1, 1).or_else(lambda: 4)
+
+value = await async_try(add_async)(1, 1).or_(4)
+
+divide: AsyncResult[..., float, ZeroDivisionError] = async_try(add_async, ZeroDivisionError)(1, 1)
+
+result: Ok[float] | Err[ZeroDivisionError] = await divide..execute()
 
 # transforming value
 value = await divide.map(lambda r: r - 100).or_(0)
 
-match (await divide.on_errors((ZeroDivisionError,)).execute()):
+match (await divide.execute()):
     case Ok(val):
         return val
     case Err(err):
         raise err
     case _:
         raise TypeError("Never supposed to happen")
 ```
 
 ## Http module
 
 Miscellaneous functions dealing with http client functions
 
-Wraps aihttp for perform http call and parsing results optionnaly as json
+Wraps aiohttp for perform http call and parsing results optionnaly as json
 
-```python
+*aiohttp* is a library of choice for making http requests. A good alternative is *httpx*
+but various benchmarks show that it is slightly slower.
 
+```python
+page_content: str = await try_get("http://google.com").or_raise()
 ```
 
+## Container module
+
+Simple subclass to return option monad when getting values
+implementation of list and dict
+
+```python
+x = opt_list([1,2,3])
+v: Some[int] = x.at(0)
+v: Empty = x.at(12)
+```
 ## Json module
 
 Miscellaneous functions dealing with json (parsing, manipulating...)
 
 ``` python
->>> from fateful.json import obj
->>> i = obj({'z-index': 1000})
+>>> from fateful.json import opt_dict
+>>> i = opt_dict({'z-index': 1000})
 >>> i.toto = [4, 5, 6]
 >>> str(i)
 '{"z-index": 1000, "toto": [4, 5, 6]}'
 ```
 
 
 Notes: I found some python packages doing almost the same things. I did
```

