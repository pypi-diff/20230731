# Comparing `tmp/httpx_s3_client-0.0.3.tar.gz` & `tmp/httpx_s3_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_s3_client-0.0.3.tar", max compression
+gzip compressed data, was "httpx_s3_client-0.0.4.tar", max compression
```

## Comparing `httpx_s3_client-0.0.3.tar` & `httpx_s3_client-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-07-25 06:18:30.098333 httpx_s3_client-0.0.3/LICENSE
--rw-r--r--   0        0        0    10495 2023-07-25 06:18:30.098540 httpx_s3_client-0.0.3/LICENSE.md
--rw-r--r--   0        0        0     7440 2023-07-31 09:02:22.262036 httpx_s3_client-0.0.3/README.md
--rw-r--r--   0        0        0      200 2023-07-29 05:51:25.407397 httpx_s3_client-0.0.3/httpx_s3_client/__init__.py
--rw-r--r--   0        0        0     2574 2023-07-29 05:52:12.475227 httpx_s3_client-0.0.3/httpx_s3_client/_xml.py
--rw-r--r--   0        0        0    23854 2023-07-31 07:37:11.099379 httpx_s3_client-0.0.3/httpx_s3_client/client.py
--rw-r--r--   0        0        0     9649 2023-07-31 07:37:11.099583 httpx_s3_client-0.0.3/httpx_s3_client/credentials.py
--rw-r--r--   0        0        0        0 2023-07-25 06:18:30.099487 httpx_s3_client-0.0.3/httpx_s3_client/py.typed
--rw-r--r--   0        0        0      152 2023-07-25 07:06:11.360545 httpx_s3_client-0.0.3/httpx_s3_client/version.py
--rw-r--r--   0        0        0     2561 2023-07-31 08:53:26.497007 httpx_s3_client-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     9157 1970-01-01 00:00:00.000000 httpx_s3_client-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0    10495 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/LICENSE.md
+-rw-r--r--   0        0        0     7814 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/README.md
+-rw-r--r--   0        0        0      200 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/__init__.py
+-rw-r--r--   0        0        0     2574 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/_xml.py
+-rw-r--r--   0        0        0    23854 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/client.py
+-rw-r--r--   0        0        0     9649 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/credentials.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/py.typed
+-rw-r--r--   0        0        0      152 2023-07-31 09:31:26.180497 httpx_s3_client-0.0.4/httpx_s3_client/version.py
+-rw-r--r--   0        0        0     2561 2023-07-31 09:31:26.184496 httpx_s3_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9531 1970-01-01 00:00:00.000000 httpx_s3_client-0.0.4/PKG-INFO
```

### Comparing `httpx_s3_client-0.0.3/LICENSE` & `httpx_s3_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_s3_client-0.0.3/LICENSE.md` & `httpx_s3_client-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `httpx_s3_client-0.0.3/README.md` & `httpx_s3_client-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 httpx-s3-client
 ================
 
-[![Coverage Status](https://coveralls.io/repos/github/vmorugin/httpx-s3-client/badge.svg?branch=master)](https://coveralls.io/github/vmorugin/httpx-s3-client?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/vmorugin/httpx-s3-client/badge.svg?branch=master)](https://coveralls.io/github/vmorugin/httpx-s3-client?branch=master) [![PyPI - License](https://img.shields.io/pypi/l/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![PyPI](https://img.shields.io/pypi/v/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![PyPI](https://img.shields.io/pypi/pyversions/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)]()
 
 The simple module for putting and getting object from Amazon S3 compatible endpoints.
 
 ## Installation
 
 ```bash
-pip install aiohttp-s3-client
+pip install httpx-s3-client
 ```
 
 ## Usage
 
 ```python
 from http import HTTPStatus
```

### Comparing `httpx_s3_client-0.0.3/httpx_s3_client/_xml.py` & `httpx_s3_client-0.0.4/httpx_s3_client/_xml.py`

 * *Files identical despite different names*

### Comparing `httpx_s3_client-0.0.3/httpx_s3_client/client.py` & `httpx_s3_client-0.0.4/httpx_s3_client/client.py`

 * *Files identical despite different names*

### Comparing `httpx_s3_client-0.0.3/httpx_s3_client/credentials.py` & `httpx_s3_client-0.0.4/httpx_s3_client/credentials.py`

 * *Files identical despite different names*

### Comparing `httpx_s3_client-0.0.3/pyproject.toml` & `httpx_s3_client-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "httpx-s3-client"
 # Dummy version which will be rewritten with poem-plugins
-version = "0.0.3"
+version = "0.0.4"
 description = "The simple module for putting and getting object from Amazon S3 compatible endpoints"
 authors = [
     "Vladimir Morugin <vamorugin@gmail.com>",
     "Dmitry Orlov <me@mosquito.su>",
     "Yuri Shikanov <dizballanze@gmail.com>",
     "Alexander Vasin <hi@alvass.in>",
 ]
```

### Comparing `httpx_s3_client-0.0.3/PKG-INFO` & `httpx_s3_client-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-s3-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: The simple module for putting and getting object from Amazon S3 compatible endpoints
 Home-page: https://github.com/Folld/httpx-s3-client
 License: Apache Software License
 Author: Vladimir Morugin
 Author-email: vamorugin@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -35,22 +35,22 @@
 Project-URL: Source, https://github.com/Folld/httpx-s3-client
 Project-URL: Tracker, https://github.com/Folld/httpx-s3-client/issues
 Description-Content-Type: text/markdown
 
 httpx-s3-client
 ================
 
-[![Coverage Status](https://coveralls.io/repos/github/vmorugin/httpx-s3-client/badge.svg?branch=master)](https://coveralls.io/github/vmorugin/httpx-s3-client?branch=master)
+[![Coverage Status](https://coveralls.io/repos/github/vmorugin/httpx-s3-client/badge.svg?branch=master)](https://coveralls.io/github/vmorugin/httpx-s3-client?branch=master) [![PyPI - License](https://img.shields.io/pypi/l/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![PyPI](https://img.shields.io/pypi/v/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![PyPI](https://img.shields.io/pypi/pyversions/httpx-s3-client)](https://pypi.org/project/httpx-s3-client) [![Mypy](http://www.mypy-lang.org/static/mypy_badge.svg)]()
 
 The simple module for putting and getting object from Amazon S3 compatible endpoints.
 
 ## Installation
 
 ```bash
-pip install aiohttp-s3-client
+pip install httpx-s3-client
 ```
 
 ## Usage
 
 ```python
 from http import HTTPStatus
```

