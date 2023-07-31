# Comparing `tmp/hishel-0.0.7.tar.gz` & `tmp/hishel-0.0.8.tar.gz`

## Comparing `hishel-0.0.7.tar` & `hishel-0.0.8.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 hishel-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0     3813 2020-02-02 00:00:00.000000 hishel-0.0.7/README.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/__about__.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/__init__.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_controller.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_exceptions.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_files.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_headers.py
--rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_serializers.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_synchronization.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/py.typed
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/_client.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/_mock.py
--rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/_pool.py
--rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/_storages.py
--rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_async/_transports.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/__init__.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/_client.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/_mock.py
--rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/_pool.py
--rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/_storages.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 hishel-0.0.7/hishel/_sync/_transports.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.7/.gitignore
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.7/LICENSE
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 hishel-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 hishel-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 hishel-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 hishel-0.0.8/README.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/__init__.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_controller.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_exceptions.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_files.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_headers.py
+-rw-r--r--   0        0        0     7939 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_serializers.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_synchronization.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/py.typed
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_client.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_mock.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_pool.py
+-rw-r--r--   0        0        0     4317 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_storages.py
+-rw-r--r--   0        0        0     5811 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_async/_transports.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/__init__.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_client.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_mock.py
+-rw-r--r--   0        0        0     2902 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_pool.py
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_storages.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 hishel-0.0.8/hishel/_sync/_transports.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 hishel-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 hishel-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 hishel-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 hishel-0.0.8/PKG-INFO
```

### Comparing `hishel-0.0.7/CHANGELOG.md` & `hishel-0.0.8/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## 0.0.8 (7/31/2023)
+
+- Skip redis tests if the server was not found. (#16)
+- Decrease sleep time for the storage ttl tests. (#18)
+- Fail coverage under 100. (#19)
+
 ## 0.0.7 (7/30/2023)
 
 - Add support for `Heuristic Freshness`. (#11)
 - Change `Controller.cache_heuristically` to `Controller.allow_heuristics`. (#12)
 - Handle import errors. (#13)
 
 ## 0.0.6 (7/29/2023)
```

### Comparing `hishel-0.0.7/README.md` & `hishel-0.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 <p align="center">
   <a href=""><img width="350" height="250" src="https://raw.githubusercontent.com/karosis88/hishel/master/.github/logo.jpg" alt='HTTPX'></a>
 </p>
 
 
 <p align="center"><strong>Hishel</strong> <em>- An elegant HTTP Cache implementation for httpx and httpcore.</em></p>
 
+<p align="center">
+
+  <a href="https://pypi.org/project/hishel">
+      <img src="https://img.shields.io/pypi/v/hishel.svg" alt="pypi">
+  </a>
+
+  <a href="https://img.shields.io/pypi/l/hishel">
+      <img src="https://img.shields.io/pypi/l/hishel" alt="license">
+  </a>
+
+  <a href="https://img.shields.io/codecov/c/github/karosis88/hishel">
+      <img src="https://img.shields.io/codecov/c/github/karosis88/hishel" alt="license">
+  </a>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/project/hishel)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hishel.svg)](https://pypi.org/project/hishel)
-![PyPI - License](https://img.shields.io/pypi/l/hishel)
-![Codecov](https://img.shields.io/codecov/c/github/karosis88/hishel)
+</p>
 
 -----
 
 **Hishel (հիշել, remember)** is a library that implements HTTP Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most recent caching specification.
 
 ## Features
```

#### html2text {}

```diff
@@ -1,42 +1,38 @@
                                     [HTTPX]
      Hishel - An elegant HTTP Cache implementation for httpx and httpcore.
-[![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/
-project/hishel) [![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/hishel.svg)](https://pypi.org/project/hishel) ![PyPI - License]
-(https://img.shields.io/pypi/l/hishel) ![Codecov](https://img.shields.io/
-codecov/c/github/karosis88/hishel) ----- **Hishel (Õ°Õ«Õ·Õ¥Õ¬, remember)** is a
-library that implements HTTP Caching for [HTTPX](https://github.com/encode/
-httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in
-accordance with **RFC 9111**, the most recent caching specification. ##
-Features - ð¾ Persistence: Responses are cached in the [**persistent
-memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use. -
-ð¤² Compatibility: It is completely compatible with your existing transports
-or connection pools, **whether they are default, custom, or provided by third-
-party libraries.** - ð¤ Easy to use: You continue to use the httpx and
-httpcore interfaces. **Can be integrated with no changes to the code.** - ð§ 
-Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`,
-`Last-Modified`, `Cache-Control`, and `Expires` headers, and **handles response
-re-validation automatically**. - âï¸ Configurable: You have complete control
-over how the responses are stored and serialized, and there is built-in support
-for filesystem and redis backends. - ð Very fast: Your requests will be even
-faster if there are **no IO operations**. ## Documentation Go through the
-[Hishel documentation](https://karosis88.github.io/hishel/). ## QuickStart
-Install `Hishel` using pip: ``` shell $ pip install hishel ``` Let's begin with
-an example of a httpx client. ```python import hishel with hishel.CacheClient()
-as client: client.get("https://www.github.com") client.get("https://
-www.github.com") # takes from the cache (very fast!) ``` or in asynchronous
-context ```python import hishel async with hishel.AsyncCacheClient() as client:
-await client.get("https://www.github.com") await client.get("https://
-www.github.com") # takes from the cache ``` ## HTTPX and HTTP Core `Hishel`
-also supports the transports of `HTTPX` and the connection pools of `HTTP
-Core`. `Hishel` respects existing **transports** and **connection pools** and
-can therefore work **on top of them**, making hishel a very **compatible and
-flexible library**. **Transports** example: ``` python import httpx import
-hishel transport = httpx.HTTPTransport() cache_transport =
+                          [pypi] [license] [license]
+----- **Hishel (Õ°Õ«Õ·Õ¥Õ¬, remember)** is a library that implements HTTP
+Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://
+github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most
+recent caching specification. ## Features - ð¾ Persistence: Responses are
+cached in the [**persistent memory**](https://en.m.wikipedia.org/wiki/
+Persistent_memory) for later use. - ð¤² Compatibility: It is completely
+compatible with your existing transports or connection pools, **whether they
+are default, custom, or provided by third-party libraries.** - ð¤ Easy to
+use: You continue to use the httpx and httpcore interfaces. **Can be integrated
+with no changes to the code.** - ð§  Smart: Attempts to clearly implement RFC
+9111, understands `Vary`, `Etag`, `Last-Modified`, `Cache-Control`, and
+`Expires` headers, and **handles response re-validation automatically**. -
+âï¸ Configurable: You have complete control over how the responses are
+stored and serialized, and there is built-in support for filesystem and redis
+backends. - ð Very fast: Your requests will be even faster if there are **no
+IO operations**. ## Documentation Go through the [Hishel documentation](https:/
+/karosis88.github.io/hishel/). ## QuickStart Install `Hishel` using pip: ```
+shell $ pip install hishel ``` Let's begin with an example of a httpx client.
+```python import hishel with hishel.CacheClient() as client: client.get("https:
+//www.github.com") client.get("https://www.github.com") # takes from the cache
+(very fast!) ``` or in asynchronous context ```python import hishel async with
+hishel.AsyncCacheClient() as client: await client.get("https://www.github.com")
+await client.get("https://www.github.com") # takes from the cache ``` ## HTTPX
+and HTTP Core `Hishel` also supports the transports of `HTTPX` and the
+connection pools of `HTTP Core`. `Hishel` respects existing **transports** and
+**connection pools** and can therefore work **on top of them**, making hishel a
+very **compatible and flexible library**. **Transports** example: ``` python
+import httpx import hishel transport = httpx.HTTPTransport() cache_transport =
 hishel.CacheTransport(transport=transport) req = httpx.Request("GET", "https://
 www.github.com") cache_transport.handle_request(req)
 cache_transport.handle_request(req) # takes from the cache ``` **Connection
 Pool** example: ```python import httpcore import hishel pool =
 hishel.CacheConnectionPool(pool=httpcore.ConnectionPool()) pool.request("GET",
 "https://www.github.com") pool.request("GET", "https://www.github.com") # takes
 from the cache ``` ## How and where are the responses saved? The responses are
```

### Comparing `hishel-0.0.7/hishel/_controller.py` & `hishel-0.0.8/hishel/_controller.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_files.py` & `hishel-0.0.8/hishel/_files.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_headers.py` & `hishel-0.0.8/hishel/_headers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_serializers.py` & `hishel-0.0.8/hishel/_serializers.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_synchronization.py` & `hishel-0.0.8/hishel/_synchronization.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_utils.py` & `hishel-0.0.8/hishel/_utils.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_async/_client.py` & `hishel-0.0.8/hishel/_async/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_async/_mock.py` & `hishel-0.0.8/hishel/_async/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_async/_pool.py` & `hishel-0.0.8/hishel/_async/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_async/_storages.py` & `hishel-0.0.8/hishel/_async/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_async/_transports.py` & `hishel-0.0.8/hishel/_async/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_sync/_client.py` & `hishel-0.0.8/hishel/_sync/_client.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_sync/_mock.py` & `hishel-0.0.8/hishel/_sync/_mock.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_sync/_pool.py` & `hishel-0.0.8/hishel/_sync/_pool.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_sync/_storages.py` & `hishel-0.0.8/hishel/_sync/_storages.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/hishel/_sync/_transports.py` & `hishel-0.0.8/hishel/_sync/_transports.py`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/LICENSE` & `hishel-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/pyproject.toml` & `hishel-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hishel-0.0.7/PKG-INFO` & `hishel-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hishel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Persistant cache implementation for httpx and httpcore
 Project-URL: Homepage, https://github.com/karosis88/hishel
 Project-URL: Source, https://github.com/karosis88/hishel
 Author-email: Kar Petrosyan <kar.petrosyanpy@gmail.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
@@ -33,19 +33,29 @@
 <p align="center">
   <a href=""><img width="350" height="250" src="https://raw.githubusercontent.com/karosis88/hishel/master/.github/logo.jpg" alt='HTTPX'></a>
 </p>
 
 
 <p align="center"><strong>Hishel</strong> <em>- An elegant HTTP Cache implementation for httpx and httpcore.</em></p>
 
+<p align="center">
+
+  <a href="https://pypi.org/project/hishel">
+      <img src="https://img.shields.io/pypi/v/hishel.svg" alt="pypi">
+  </a>
+
+  <a href="https://img.shields.io/pypi/l/hishel">
+      <img src="https://img.shields.io/pypi/l/hishel" alt="license">
+  </a>
+
+  <a href="https://img.shields.io/codecov/c/github/karosis88/hishel">
+      <img src="https://img.shields.io/codecov/c/github/karosis88/hishel" alt="license">
+  </a>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/project/hishel)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hishel.svg)](https://pypi.org/project/hishel)
-![PyPI - License](https://img.shields.io/pypi/l/hishel)
-![Codecov](https://img.shields.io/codecov/c/github/karosis88/hishel)
+</p>
 
 -----
 
 **Hishel (հիշել, remember)** is a library that implements HTTP Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most recent caching specification.
 
 ## Features
 
@@ -136,14 +146,20 @@
 
 - Fork the project.
 - Make change.
 - Open the pull request.
 
 # Changelog
 
+## 0.0.8 (7/31/2023)
+
+- Skip redis tests if the server was not found. (#16)
+- Decrease sleep time for the storage ttl tests. (#18)
+- Fail coverage under 100. (#19)
+
 ## 0.0.7 (7/30/2023)
 
 - Add support for `Heuristic Freshness`. (#11)
 - Change `Controller.cache_heuristically` to `Controller.allow_heuristics`. (#12)
 - Handle import errors. (#13)
 
 ## 0.0.6 (7/29/2023)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hishel Version: 0.0.7 Summary: Persistant cache
+Metadata-Version: 2.1 Name: hishel Version: 0.0.8 Summary: Persistant cache
 implementation for httpx and httpcore Project-URL: Homepage, https://
 github.com/karosis88/hishel Project-URL: Source, https://github.com/karosis88/
 hishel Author-email: Kar Petrosyan
 petrosyanpy@gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: Environment :: Web
 Environment Classifier: Framework :: AsyncIO Classifier: Framework :: Trio
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
@@ -13,61 +13,59 @@
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Internet :: WWW/HTTP Requires-Python: >=3.8 Requires-Dist: httpcore
 Requires-Dist: httpx Provides-Extra: redis Requires-Dist: redis==4.6.0; extra
 == 'redis' Provides-Extra: yaml Requires-Dist: pyyaml==6.0.1; extra == 'yaml'
 Description-Content-Type: text/markdown
                                     [HTTPX]
      Hishel - An elegant HTTP Cache implementation for httpx and httpcore.
-[![PyPI - Version](https://img.shields.io/pypi/v/hishel.svg)](https://pypi.org/
-project/hishel) [![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/hishel.svg)](https://pypi.org/project/hishel) ![PyPI - License]
-(https://img.shields.io/pypi/l/hishel) ![Codecov](https://img.shields.io/
-codecov/c/github/karosis88/hishel) ----- **Hishel (Õ°Õ«Õ·Õ¥Õ¬, remember)** is a
-library that implements HTTP Caching for [HTTPX](https://github.com/encode/
-httpx) and [HTTP Core](https://github.com/encode/httpcore) libraries in
-accordance with **RFC 9111**, the most recent caching specification. ##
-Features - ð¾ Persistence: Responses are cached in the [**persistent
-memory**](https://en.m.wikipedia.org/wiki/Persistent_memory) for later use. -
-ð¤² Compatibility: It is completely compatible with your existing transports
-or connection pools, **whether they are default, custom, or provided by third-
-party libraries.** - ð¤ Easy to use: You continue to use the httpx and
-httpcore interfaces. **Can be integrated with no changes to the code.** - ð§ 
-Smart: Attempts to clearly implement RFC 9111, understands `Vary`, `Etag`,
-`Last-Modified`, `Cache-Control`, and `Expires` headers, and **handles response
-re-validation automatically**. - âï¸ Configurable: You have complete control
-over how the responses are stored and serialized, and there is built-in support
-for filesystem and redis backends. - ð Very fast: Your requests will be even
-faster if there are **no IO operations**. ## Documentation Go through the
-[Hishel documentation](https://karosis88.github.io/hishel/). ## QuickStart
-Install `Hishel` using pip: ``` shell $ pip install hishel ``` Let's begin with
-an example of a httpx client. ```python import hishel with hishel.CacheClient()
-as client: client.get("https://www.github.com") client.get("https://
-www.github.com") # takes from the cache (very fast!) ``` or in asynchronous
-context ```python import hishel async with hishel.AsyncCacheClient() as client:
-await client.get("https://www.github.com") await client.get("https://
-www.github.com") # takes from the cache ``` ## HTTPX and HTTP Core `Hishel`
-also supports the transports of `HTTPX` and the connection pools of `HTTP
-Core`. `Hishel` respects existing **transports** and **connection pools** and
-can therefore work **on top of them**, making hishel a very **compatible and
-flexible library**. **Transports** example: ``` python import httpx import
-hishel transport = httpx.HTTPTransport() cache_transport =
+                          [pypi] [license] [license]
+----- **Hishel (Õ°Õ«Õ·Õ¥Õ¬, remember)** is a library that implements HTTP
+Caching for [HTTPX](https://github.com/encode/httpx) and [HTTP Core](https://
+github.com/encode/httpcore) libraries in accordance with **RFC 9111**, the most
+recent caching specification. ## Features - ð¾ Persistence: Responses are
+cached in the [**persistent memory**](https://en.m.wikipedia.org/wiki/
+Persistent_memory) for later use. - ð¤² Compatibility: It is completely
+compatible with your existing transports or connection pools, **whether they
+are default, custom, or provided by third-party libraries.** - ð¤ Easy to
+use: You continue to use the httpx and httpcore interfaces. **Can be integrated
+with no changes to the code.** - ð§  Smart: Attempts to clearly implement RFC
+9111, understands `Vary`, `Etag`, `Last-Modified`, `Cache-Control`, and
+`Expires` headers, and **handles response re-validation automatically**. -
+âï¸ Configurable: You have complete control over how the responses are
+stored and serialized, and there is built-in support for filesystem and redis
+backends. - ð Very fast: Your requests will be even faster if there are **no
+IO operations**. ## Documentation Go through the [Hishel documentation](https:/
+/karosis88.github.io/hishel/). ## QuickStart Install `Hishel` using pip: ```
+shell $ pip install hishel ``` Let's begin with an example of a httpx client.
+```python import hishel with hishel.CacheClient() as client: client.get("https:
+//www.github.com") client.get("https://www.github.com") # takes from the cache
+(very fast!) ``` or in asynchronous context ```python import hishel async with
+hishel.AsyncCacheClient() as client: await client.get("https://www.github.com")
+await client.get("https://www.github.com") # takes from the cache ``` ## HTTPX
+and HTTP Core `Hishel` also supports the transports of `HTTPX` and the
+connection pools of `HTTP Core`. `Hishel` respects existing **transports** and
+**connection pools** and can therefore work **on top of them**, making hishel a
+very **compatible and flexible library**. **Transports** example: ``` python
+import httpx import hishel transport = httpx.HTTPTransport() cache_transport =
 hishel.CacheTransport(transport=transport) req = httpx.Request("GET", "https://
 www.github.com") cache_transport.handle_request(req)
 cache_transport.handle_request(req) # takes from the cache ``` **Connection
 Pool** example: ```python import httpcore import hishel pool =
 hishel.CacheConnectionPool(pool=httpcore.ConnectionPool()) pool.request("GET",
 "https://www.github.com") pool.request("GET", "https://www.github.com") # takes
 from the cache ``` ## How and where are the responses saved? The responses are
 stored by `Hishel` in [storages](https://karosis88.github.io/hishel/userguide/
 #storages). You have complete control over them; you can change storage or even
 write your own if necessary. ## Contributing `Hishel` is a powerful tool, but
 it is also a new project with potential flaws, so we welcome contributions! You
 can open the pull request by following these instructions if you want to
 improve `Hishel`. ð - Fork the project. - Make change. - Open the pull
-request. # Changelog ## 0.0.7 (7/30/2023) - Add support for `Heuristic
+request. # Changelog ## 0.0.8 (7/31/2023) - Skip redis tests if the server was
+not found. (#16) - Decrease sleep time for the storage ttl tests. (#18) - Fail
+coverage under 100. (#19) ## 0.0.7 (7/30/2023) - Add support for `Heuristic
 Freshness`. (#11) - Change `Controller.cache_heuristically` to
 `Controller.allow_heuristics`. (#12) - Handle import errors. (#13) ## 0.0.6 (7/
 29/2023) - Fix `Vary` header validation. (#8) - Dump original requests with the
 responses. (#7) ## 0.0.5 (7/29/2023) - Fix httpx response streaming. ## 0.0.4
 (7/29/2023) - Change `YamlSerializer` name to `YAMLSerializer`. ## 0.0.3 (7/28/
 2023) - Add `from_cache` response extension. - Add `typing_extensions` into the
 requirements. ## 0.0.2 (7/25/2023) - Add [redis](https://redis.io/) support. -
```

