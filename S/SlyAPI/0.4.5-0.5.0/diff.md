# Comparing `tmp/SlyAPI-0.4.5.tar.gz` & `tmp/SlyAPI-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SlyAPI-0.4.5.tar", last modified: Fri Mar  3 09:53:19 2023, max compression
+gzip compressed data, was "SlyAPI-0.5.0.tar", last modified: Mon Jul 31 05:42:20 2023, max compression
```

## Comparing `SlyAPI-0.4.5.tar` & `SlyAPI-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 09:53:19.869208 SlyAPI-0.4.5/
--rw-rw-rw-   0        0        0     1086 2023-02-24 11:46:30.000000 SlyAPI-0.4.5/LICENSE
--rw-rw-rw-   0        0        0     4487 2023-03-03 09:53:19.868211 SlyAPI-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0     2745 2023-02-27 06:45:16.000000 SlyAPI-0.4.5/README.md
--rw-rw-rw-   0        0        0     1043 2023-03-03 09:53:03.000000 SlyAPI-0.4.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-03 09:53:19.869208 SlyAPI-0.4.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-03 09:53:19.827692 SlyAPI-0.4.5/src/
-drwxrwxrwx   0        0        0        0 2023-03-03 09:53:19.846696 SlyAPI-0.4.5/src/SlyAPI/
--rw-rw-rw-   0        0        0      472 2023-02-26 03:23:21.000000 SlyAPI-0.4.5/src/SlyAPI/__init__.py
--rw-rw-rw-   0        0        0     1600 2023-02-27 00:42:21.000000 SlyAPI-0.4.5/src/SlyAPI/__main__.py
--rw-rw-rw-   0        0        0     4723 2023-02-27 05:55:35.000000 SlyAPI-0.4.5/src/SlyAPI/asyncy.py
--rw-rw-rw-   0        0        0     1191 2023-02-24 11:46:30.000000 SlyAPI-0.4.5/src/SlyAPI/auth.py
--rw-rw-rw-   0        0        0     6152 2023-02-27 02:55:37.000000 SlyAPI-0.4.5/src/SlyAPI/flow.py
--rw-rw-rw-   0        0        0     8151 2023-02-26 21:30:48.000000 SlyAPI-0.4.5/src/SlyAPI/oauth1.py
--rw-rw-rw-   0        0        0    11459 2023-03-03 09:48:32.000000 SlyAPI-0.4.5/src/SlyAPI/oauth2.py
--rw-rw-rw-   0        0        0     3760 2023-03-03 06:17:43.000000 SlyAPI-0.4.5/src/SlyAPI/web.py
--rw-rw-rw-   0        0        0    13282 2023-03-03 06:48:03.000000 SlyAPI-0.4.5/src/SlyAPI/webapi.py
-drwxrwxrwx   0        0        0        0 2023-03-03 09:53:19.863212 SlyAPI-0.4.5/src/SlyAPI.egg-info/
--rw-rw-rw-   0        0        0     4487 2023-03-03 09:53:19.000000 SlyAPI-0.4.5/src/SlyAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-03-03 09:53:19.000000 SlyAPI-0.4.5/src/SlyAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 09:53:19.000000 SlyAPI-0.4.5/src/SlyAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-03-03 09:53:19.000000 SlyAPI-0.4.5/src/SlyAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-03 09:53:19.000000 SlyAPI-0.4.5/src/SlyAPI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-03 09:53:19.867216 SlyAPI-0.4.5/test/
--rw-rw-rw-   0        0        0      924 2023-02-26 03:23:05.000000 SlyAPI-0.4.5/test/test_async_unmanage.py
--rw-rw-rw-   0        0        0     3371 2023-03-03 09:45:00.000000 SlyAPI-0.4.5/test/test_auth.py
--rw-rw-rw-   0        0        0     1879 2023-02-27 01:21:32.000000 SlyAPI-0.4.5/test/test_readme.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:42:20.991910 SlyAPI-0.5.0/
+-rw-rw-rw-   0        0        0     1086 2023-02-24 11:46:30.000000 SlyAPI-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0     4487 2023-07-31 05:42:20.991910 SlyAPI-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2745 2023-02-27 06:45:16.000000 SlyAPI-0.5.0/README.md
+-rw-rw-rw-   0        0        0     1043 2023-07-31 04:15:28.000000 SlyAPI-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:42:20.991910 SlyAPI-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 05:42:20.978898 SlyAPI-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:42:20.986905 SlyAPI-0.5.0/src/SlyAPI/
+-rw-rw-rw-   0        0        0      472 2023-02-26 03:23:21.000000 SlyAPI-0.5.0/src/SlyAPI/__init__.py
+-rw-rw-rw-   0        0        0     1600 2023-02-27 00:42:21.000000 SlyAPI-0.5.0/src/SlyAPI/__main__.py
+-rw-rw-rw-   0        0        0     3337 2023-07-31 02:21:09.000000 SlyAPI-0.5.0/src/SlyAPI/asyncy.py
+-rw-rw-rw-   0        0        0     1191 2023-02-24 11:46:30.000000 SlyAPI-0.5.0/src/SlyAPI/auth.py
+-rw-rw-rw-   0        0        0     6152 2023-02-27 02:55:37.000000 SlyAPI-0.5.0/src/SlyAPI/flow.py
+-rw-rw-rw-   0        0        0     8298 2023-03-04 02:36:42.000000 SlyAPI-0.5.0/src/SlyAPI/oauth1.py
+-rw-rw-rw-   0        0        0    11501 2023-03-12 02:07:16.000000 SlyAPI-0.5.0/src/SlyAPI/oauth2.py
+-rw-rw-rw-   0        0        0     3992 2023-03-12 02:08:53.000000 SlyAPI-0.5.0/src/SlyAPI/web.py
+-rw-rw-rw-   0        0        0    13784 2023-07-31 02:19:35.000000 SlyAPI-0.5.0/src/SlyAPI/webapi.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:42:20.988907 SlyAPI-0.5.0/src/SlyAPI.egg-info/
+-rw-rw-rw-   0        0        0     4487 2023-07-31 05:42:20.000000 SlyAPI-0.5.0/src/SlyAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-07-31 05:42:20.000000 SlyAPI-0.5.0/src/SlyAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:42:20.000000 SlyAPI-0.5.0/src/SlyAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2023-07-31 05:42:20.000000 SlyAPI-0.5.0/src/SlyAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 05:42:20.000000 SlyAPI-0.5.0/src/SlyAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 05:42:20.990909 SlyAPI-0.5.0/test/
+-rw-rw-rw-   0        0        0     1975 2023-07-31 03:37:09.000000 SlyAPI-0.5.0/test/test_api_readme.py
+-rw-rw-rw-   0        0        0     1094 2023-07-31 02:19:35.000000 SlyAPI-0.5.0/test/test_async_unmanage.py
+-rw-rw-rw-   0        0        0     3506 2023-07-31 03:27:14.000000 SlyAPI-0.5.0/test/test_auth.py
```

### Comparing `SlyAPI-0.4.5/LICENSE` & `SlyAPI-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SlyAPI-0.4.5/PKG-INFO` & `SlyAPI-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SlyAPI
-Version: 0.4.5
+Version: 0.5.0
 Summary: No-boilerplate, async and typed web api access with oauth1/2.
 Author: Dunkyl 🔣🔣
 License: The MIT License
         
         Copyright © 2021 Maroue Reus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `SlyAPI-0.4.5/README.md` & `SlyAPI-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `SlyAPI-0.4.5/pyproject.toml` & `SlyAPI-0.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SlyAPI"
-version = "0.4.5"
+version = "0.5.0"
 description = "No-boilerplate, async and typed web api access with oauth1/2."
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file="LICENSE" }
 authors = [{name="Dunkyl 🔣🔣"}]
 classifiers = [
     "Operating System :: OS Independent"
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI/__main__.py` & `SlyAPI-0.5.0/src/SlyAPI/__main__.py`

 * *Files identical despite different names*

### Comparing `SlyAPI-0.4.5/src/SlyAPI/asyncy.py` & `SlyAPI-0.5.0/src/SlyAPI/asyncy.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,73 +6,42 @@
 
 T = TypeVar('T')
 U = TypeVar('U')
 
 T_Params = ParamSpec("T_Params")
 U_Params = ParamSpec("U_Params")
 
-def run_sync_ensured(corofn: Callable[[], Coroutine[Any, None, None]]) -> None:
-    '''Run a coroutine, regardless of whether there is already an event loop.'''
-    try:
-        event_loop = asyncio.get_running_loop()
-        asyncio.create_task(corofn())
-    except RuntimeError:
-        event_loop = asyncio.get_event_loop_policy().get_event_loop()
-        event_loop.run_until_complete(corofn())
-
 unmanaged_tasks: set[Any] = set()
-async def unmanage_async_context(context: AbstractAsyncContextManager[T]) -> tuple[T, asyncio.Semaphore]:
+def unmanage_async_context(context: AbstractAsyncContextManager[T]) -> tuple[asyncio.Task[T], asyncio.Event]:
     '''
     Extract an async context manager's value without manually managing its lifetime.
-    The context manager is leaked and will only be cleaned up when the program exits.
-    '''
-    MISSING = object()
-    extracted = MISSING
-    extracted_semaphore = asyncio.Semaphore(0)
-    closed_semaphore = asyncio.Semaphore(0)
-    async def background():
-        nonlocal extracted
-        async with context as inner:
-            extracted = inner
-            extracted_semaphore.release()
-            print(f'Released semaphore for {context}')
-            await closed_semaphore.acquire()
-    task = asyncio.create_task(background())
-    unmanaged_tasks.add(task)
-    task.add_done_callback(unmanaged_tasks.remove)
-    await extracted_semaphore.acquire()
-    if extracted is MISSING:
-        raise RuntimeError('Async context manager did not return a value.')
-    else:
-        return (
-            extracted, # type: ignore
-            closed_semaphore )
+    The context manager is entered until `set()` is called on the returned event.
 
-def unmanage_async_context_sync(context: AbstractAsyncContextManager[T]) -> tuple[T, asyncio.Semaphore]:
+    thats it *unmanages your async context manager*
     '''
-    Extract an async context manager's value without manually managing its lifetime.
-    The context manager is leaked and will only be cleaned up when the program exits.
-    '''
-    MISSING = object()
-    extracted = context
-    closed_semaphore = asyncio.Semaphore(0)
+    close_context = asyncio.Event()
+    fut_T_ready = asyncio.Event()
+    fut_T = None
     async def background():
-        nonlocal extracted
-        async with context as _inner:
-            print(f'Released semaphore for {context}')
-            await closed_semaphore.acquire()
+        async with context as inner:
+            nonlocal fut_T
+            fut_T = inner
+            fut_T_ready.set()
+            # print(f'Released event for {context}')
+            await close_context.wait()
     task = asyncio.create_task(background())
     unmanaged_tasks.add(task)
     task.add_done_callback(unmanaged_tasks.remove)
-    if extracted is MISSING:
-        raise RuntimeError('Async context manager did not return a value.')
-    else:
-        return (
-            extracted, # type: ignore
-            closed_semaphore )
+    async def aenter_wait():
+        await fut_T_ready.wait()
+        assert fut_T is not None
+        return fut_T
+    return (
+        asyncio.create_task(aenter_wait()), # type: ignore
+        close_context )
 
 class AsyncLazy(Generic[T]):
     '''
     Async iterator which does not accumulate any results unless awaited.
     Awaiting instances will return a list of the results.
     '''
     gen: AsyncGenerator[T, None]
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI/auth.py` & `SlyAPI-0.5.0/src/SlyAPI/auth.py`

 * *Files identical despite different names*

### Comparing `SlyAPI-0.4.5/src/SlyAPI/flow.py` & `SlyAPI-0.5.0/src/SlyAPI/flow.py`

 * *Files identical despite different names*

### Comparing `SlyAPI-0.4.5/src/SlyAPI/oauth1.py` & `SlyAPI-0.5.0/src/SlyAPI/oauth1.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,18 @@
     for k, v in sorted(encoded.items()):
         results.append(F'{k}={v}')
     return '&'.join(results)
 
 # https://datatracker.ietf.org/doc/html/rfc5849#section-3.4.2
 def _hmac_sign(request: Request, signing_params: dict[str, Any], appSecret: str, userSecret: str|None = None) -> str:
         if not request.data_is_json:
-            all_params = { **request.data }
+            if isinstance(request.data, dict):
+                all_params = { **request.data }
+            else:
+                raise TypeError(F"Expected dict, got {type(request.data)}")
         else:
             all_params = {}
         all_params |= request.query_params | signing_params
         base = F"{request.method.value.upper()}&{percentEncode(request.url.lower())}&{percentEncode(paramString(all_params))}"
         # NOTE:
         #  2.  An "&" character (ASCII code 38), which MUST be included
         #        even when either secret is empty.
@@ -192,15 +195,15 @@
                 print(F"Response did not provide authorization:\n{content}")
                 print("\nThis is probably because the credentials for the app are invalid.")
                 exit(1)
                 # raise ValueError(F"Response did not provide authorization:\n{content}")
             oauth_token = resp_params['oauth_token'][0]
             # oauth_token_secret = resp_params['oauth_token_secret'][0]
             if resp_params['oauth_callback_confirmed'][0] != 'true':
-                raise ValueError(F"oauth_callback_confirmed was not true")
+                raise ValueError("oauth_callback_confirmed was not true")
 
     # step 2: get the user to authorize the application
     grant_link = F"{app.authorize_uri}?{urllib.parse.urlencode({'oauth_token': oauth_token})}"
 
     webbrowser.open(grant_link, new=1, autoraise=True)
 
     # step 2 (cont.): wait for the user to be redirected with the code
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI/oauth2.py` & `SlyAPI-0.5.0/src/SlyAPI/oauth2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import secrets
 from copy import copy
 from typing import Any, Callable, ParamSpec, TypeVar, cast
 
 from warnings import warn
 
 from .auth import Auth
-from .web import ApiError, Request, TomlMap, serve_once
+from .web import ApiError, JsonMap, Request, TomlMap, serve_once
 
 
 import aiohttp
 from aiohttp import ClientSession as Client
 
 import urllib.parse
 
@@ -111,28 +111,28 @@
 class OAuth2App:
     id: str
     secret: str
     auth_uri: str # flow step 1
     token_uri: str # flow step 3
 
     @classmethod
-    def from_json_obj(cls, obj: dict[str, str]) -> 'OAuth2App':
+    def from_json_obj(cls, obj: JsonMap) -> 'OAuth2App':
         '''Read an app from a JSON object, either from the Google Console JSON format or a set of kwargs'''
         match obj:
             case { # to_dict(self)
-                'id': id,
-                'secret': secret,
-                'auth_uri': auth_uri,
-                'token_uri': token_uri
+                'id': str(id),
+                'secret': str(secret),
+                'auth_uri': str(auth_uri),
+                'token_uri': str(token_uri)
             } | { # Google JSON
                 'web': {
-                    'client_id': id,
-                    'client_secret': secret,
-                    'auth_uri': auth_uri,
-                    'token_uri': token_uri
+                    'client_id': str(id),
+                    'client_secret': str(secret),
+                    'auth_uri': str(auth_uri),
+                    'token_uri': str(token_uri)
                 }
             }: 
                 return cls(id, secret, auth_uri, token_uri)
             case _:
                 raise ValueError(F"Unknown format for OAuth2App: {obj}")
 
     @classmethod
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI/web.py` & `SlyAPI-0.5.0/src/SlyAPI/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import asyncio
 from dataclasses import dataclass, field
 import datetime
 from enum import Enum
 import collections.abc
-from aiohttp import ClientSession as Client, ClientResponse as Response
+from typing import TypeAlias
+from aiohttp import ClientSession as Client, ClientResponse as Response, FormData
 
 ParamType = \
         int | str | Enum | None \
         | collections.abc.Set['ParamType'] \
         | collections.abc.Sequence['ParamType']
 # Mapping is covariant in the value type, allowing for subclasses of Enum as values.
 # dict is invariant in the value type, so we need to use Mapping instead.
 ParamsDict = collections.abc.Mapping[str, ParamType]
 
-JsonScalar = int | float | bool | str | None
-JsonType = JsonScalar | collections.abc.Sequence['JsonType'] | collections.abc.Mapping[str, 'JsonType']
-JsonMap = dict[str, JsonType]
+JsonScalar: TypeAlias = int | float | bool | str | None
+JsonType: TypeAlias = JsonScalar | list['JsonType'] | dict[str, 'JsonType']
+JsonMap: TypeAlias = dict[str, JsonType]
+
+JsonTypeCo: TypeAlias = JsonScalar | collections.abc.Sequence['JsonTypeCo'] | collections.abc.Mapping[str, 'JsonTypeCo']
+JsonMapCo: TypeAlias = collections.abc.Mapping[str, JsonTypeCo]
 
 TomlType = \
         JsonScalar \
         | datetime.datetime | datetime.date | datetime.time \
         | collections.abc.Sequence['TomlType'] \
         | collections.abc.Mapping[str, 'TomlType']
 TomlMap = collections.abc.Mapping[str, TomlType]
@@ -55,15 +59,15 @@
 
 @dataclass
 class Request:
     method: Method
     url: str
     query_params: dict[str, str|int]= field(default_factory=dict)
     headers: dict[str, str] = field(default_factory=dict)
-    data: JsonMap = field(default_factory=dict)
+    data: JsonMap|FormData = field(default_factory=dict)
     data_is_json: bool = False
 
     def send(self, client: Client):
         json = None
         data = None
         params = None
         headers = None
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI/webapi.py` & `SlyAPI-0.5.0/src/SlyAPI/webapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,56 @@
 '''
 Implementation for following classes:
 
 - WebAPI
 '''
 from dataclasses import asdict, is_dataclass
 from enum import Enum
-import asyncio
 import json
 from typing import Any, AsyncGenerator, cast, TypeVar, overload
 
 from aiohttp import ClientSession as Client
-from .asyncy import AsyncLazy, unmanage_async_context_sync
+from .asyncy import AsyncLazy, unmanage_async_context
 from .auth import Auth
 from .web import Request, Method, JsonMap, ParamsDict, ApiError
 
 T = TypeVar('T')
 
 class WebAPI:
     'Base class for web APIs'
-    _client: Client
-    _client_close_semaphone: asyncio.Semaphore
     _use_form_data: bool
 
     _parameter_list_delimiter: str = ','
 
     base_url: str
     auth: Auth
 
+    _maybe_client: Client | None
+    @property
+    def _client(self) -> Client:
+        if self._maybe_client is None:
+            self._maybe_client = Client()
+            # Client.__aenter__ returns Client
+            (_, self._client_close_context) = unmanage_async_context(self._maybe_client)
+        return self._maybe_client
+
     def __init__(self, auth: Auth, use_form_data: bool = False) -> None:
-        self._client, self._client_close_semaphone = unmanage_async_context_sync(Client())
+        self._maybe_client = None
         self.auth = auth
         self._use_form_data = use_form_data
 
     def __del__(self):
-        # free up the client session
-        try:
-            self._client_close_semaphone.release()
-        except RuntimeError: # event loop was closed
-            if self._client._connector is not None: # type: ignore
-                self._client._connector._close() # type: ignore
-                self._client._connector = None # type: ignore
+        # free up the client session if its been created
+        if hasattr(self, '_client_close_context'):
+            try:
+                self._client_close_context.set()
+            except RuntimeError: # event loop was closed
+                if self._client._connector is not None: # type: ignore
+                    self._client._connector._close() # type: ignore
+                    self._client._connector = None # type: ignore
 
     # delimit lists and sets, convert enums to their values, and exclude None values
     def _convert_parameters(self, params: ParamsDict) -> dict[str, str|int]:
         converted: dict[str, str|int] = {}
         for k, v in params.items():
             match v:
                 case set() if len(v) > 0: # non-empty set
@@ -58,15 +65,15 @@
                 case [Enum(), *_]: # list of enums
                     values = [e.value for e in v if e.value is not None]
                     if len(values) > 0:
                         converted[k] = self._parameter_list_delimiter.join(values)
                 case [_, *_]: # non-empty list
                     converted[k] = self._parameter_list_delimiter.join(map(str, v))
                 case Enum() if v.value is not None:
-                    print(F"Converting enum {v} to {v.value}")
+                    # print(F"Converting enum {v} to {v.value}")
                     converted[k] = v.value
                 case int() | str():
                     converted[k] = v
                 case _: pass # exclude None values
         return converted
 
     def get_full_url(self, path: str) -> str:
@@ -118,29 +125,32 @@
     @overload
     async def _request(self, method: Method, returns: None, path: str, params: ParamsDict|None=None, data: Any = None, headers: dict[str, str]|None=None) -> None:
         ...
 
     @overload
     async def _request(self, method: Method, returns: type[T], path: str, params: ParamsDict|None=None, data: Any = None, headers: dict[str, str]|None=None) -> T:
         ...
-    
-    async def _request(self, method: Method, returns: type[T]|None, path: str, params: ParamsDict|None=None, data: Any = None, headers: dict[str, str]|None=None) -> T|None:
+        
+
+    async def _request_context(self, method: Method, path: str, params: ParamsDict|None=None, data: Any = None, headers: dict[str, str]|None=None):
         if data and hasattr(data, 'to_json'):
             data = data.json()
         elif data and is_dataclass(data):
             data = asdict(data)
-        print(data)
-        
         req = await self.auth.sign(self._client,
             Request( method, self.get_full_url(path), 
                 self._convert_parameters(params) if params else {},
                 headers or {},
                 data, not self._use_form_data
             ))
-        async with req.send(self._client) as resp:
+        return req.send(self._client)
+
+    async def _request(self, method: Method, returns: type[T]|None, path: str, params: ParamsDict|None=None, data: Any = None, headers: dict[str, str]|None=None) -> T|None:
+        ctx = await self._request_context(method, path, params, data, headers)
+        async with ctx as resp:
             if resp.status >= 400:
                 raise await ApiError.from_resposnse(resp)
             if returns is None:
                 return None
             elif returns == str:
                 return await resp.text() # type: ignore ## T is str
             else:
@@ -276,15 +286,16 @@
         return AsyncLazy(self._paginated(path, params, limit))
 
     async def _paginated(self,
                         path: str,
                         params: ParamsDict,
                         limit: int | None) -> AsyncGenerator[JsonMap, None]:
         result_count = 0
-        params = dict(params) if params else {}
+
+        params = dict(params or {})
 
         while True:
             page = await self.get_json(path, params)
 
             items = page.get('items', page.get('data'))
 
             if not items: break
```

### Comparing `SlyAPI-0.4.5/src/SlyAPI.egg-info/PKG-INFO` & `SlyAPI-0.5.0/src/SlyAPI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SlyAPI
-Version: 0.4.5
+Version: 0.5.0
 Summary: No-boilerplate, async and typed web api access with oauth1/2.
 Author: Dunkyl 🔣🔣
 License: The MIT License
         
         Copyright © 2021 Maroue Reus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `SlyAPI-0.4.5/test/test_async_unmanage.py` & `SlyAPI-0.5.0/test/test_async_unmanage.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from SlyAPI.asyncy import unmanage_async_context
 
 async def test_unmanage_async_context():
 
     class FiveManager:
         was_entered = False
         was_exited = False
+        five_calculated = None
 
         async def __aenter__(self):
             self.was_entered = True
             return 5
 
         async def __aexit__(self, *_):
             self.was_exited = True
@@ -18,18 +19,20 @@
 
     async with five_factory_managed as five:
         assert five == 5
         assert five_factory_managed.was_entered
     assert five_factory_managed.was_exited
 
     five_factory_unmanaged = FiveManager()
-    five, release = await unmanage_async_context(five_factory_unmanaged)
+    five_once_entered, close_ctx = unmanage_async_context(five_factory_unmanaged)
+
+    five = await five_once_entered # yield to background context to run __aenter__
 
     assert five == 5
     assert five_factory_unmanaged.was_entered
     assert not five_factory_unmanaged.was_exited
 
-    release.release()
+    close_ctx.set()
 
-    await asyncio.sleep(0.1)
+    await asyncio.sleep(0) # yield to background context to run __aexit__
 
     assert five_factory_unmanaged.was_exited
```

### Comparing `SlyAPI-0.4.5/test/test_auth.py` & `SlyAPI-0.5.0/test/test_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+import os
 from datetime import datetime, timedelta
 from dataclasses import asdict
+
+from SlyAPI.web import JsonMap
 from SlyAPI import *
 
+test_dir = os.path.dirname(__file__)
+
 def test_oauth1_serialize():
 
     obj = {
         'key': 'example_key',
         'secret': 'example_secret'
     }
 
@@ -15,30 +20,31 @@
 
     user2 = OAuth1User.from_json_obj({
         'oauth_token': 'example_key',
         'oauth_token_secret': 'example_secret',
         'some_service_add_thing': 'example_thing'
     })
 
-    user3 = OAuth1User.from_json_file("test/ex_oauth1_user.json")
+    
+    user3 = OAuth1User.from_json_file(F"{test_dir}/ex_oauth1_user.json")
 
     assert user1 == user2 == user3
 
     err_invalid = None
     try:
         _err_user_inv = OAuth1User.from_json_obj({ "bad": "format" })
     except Exception as e :
         err_invalid = e
 
     assert err_invalid is not None
     assert isinstance(err_invalid, ValueError)
 
     err_not_found = None
     try:
-        _err_user_not_found = OAuth1User.from_json_file("test/not_exists.json")
+        _err_user_not_found = OAuth1User.from_json_file(F"{test_dir}/not_exists.json")
     except Exception as e:
         err_not_found = e
 
     assert err_not_found is not None
     assert isinstance(err_not_found, FileNotFoundError)
 
     obj = {
@@ -47,21 +53,21 @@
         'request_uri': 'https://example.com/request_token',
         'authorize_uri': 'https://example.com/authorize',
         'access_uri': 'https://example.com/access_token'
     }
 
     app1 = OAuth1App.from_json_obj(obj)
 
-    app2 = OAuth1App.from_json_file("test/ex_oauth1.json")
+    app2 = OAuth1App.from_json_file(F"{test_dir}/ex_oauth1.json")
 
     assert app1 == app2
 
     err_not_found = None
     try:
-        _err_user_not_found = OAuth1App.from_json_file("test/not_exists.json")
+        _err_user_not_found = OAuth1App.from_json_file(F"{test_dir}/not_exists.json")
     except FileNotFoundError as e:
         err_not_found = e
 
     assert err_not_found is not None
 
 def test_oauth2_serialize():
 
@@ -102,20 +108,20 @@
         _err_user_inv = OAuth2User.from_json_obj({ "bad": "format" })
     except ValueError as e :
         err_invalid = e
 
     assert err_invalid is not None
     assert isinstance(err_invalid, ValueError)
 
-    obj = {
+    obj: JsonMap = {
         'id': 'example_client_id',
         'secret': 'example_secret',
         'token_uri': 'https://example.com/request_token',
         'auth_uri': 'https://example.com/authorize',
     }
 
     app1 = OAuth2App.from_json_obj(obj)
 
-    app2 = OAuth2App.from_json_file("test/ex_oauth2.json")
+    app2 = OAuth2App.from_json_file(F"{test_dir}/ex_oauth2.json")
 
     assert app1 == app2
```

### Comparing `SlyAPI-0.4.5/test/test_readme.py` & `SlyAPI-0.5.0/test/test_api_readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from enum import Enum
-import sys
+import sys, os
 from typing import Any
 
 import pytest
 
 from SlyAPI import *
 
+test_dir = os.path.dirname(__file__)
+
 class Mode(Enum):
     XML  = 'xml'
     HTML = 'html'
     JSON = None
 
 class Units(Enum):
     STANDARD = 'standard' # Kelvin
@@ -47,18 +49,19 @@
     api = OpenWeather('example_key')
     assert api.base_url == 'https://api.openweathermap.org/data/2.5'
 
 # Preconditions:
 # - cwd is the project root
 # - internet connection
 # - API key for openweather.org is stored in test/apikey.txt
+# Skipped by default unless run in debugger
 @pytest.mark.skipif(sys.gettrace() is None, reason="Does side effects (web request)")
 async def test_readme():
 
-    key = open('test/apikey.txt', encoding='utf8').read().strip()
+    key = open(F'{test_dir}/apikey.txt', encoding='utf8').read().strip()
     weather = OpenWeather(key)
 
     city = await weather.city('New York,NY,US', units=Units.IMPERIAL)
 
     print(F"It's {city.temperature}°F in {city.name}, {city.description}.")
 
     assert city.name == 'New York'
```

