# Comparing `tmp/gundi_client_v2-2.1.0.tar.gz` & `tmp/gundi_client_v2-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gundi_client_v2-2.1.0.tar", max compression
+gzip compressed data, was "gundi_client_v2-2.1.1.tar", max compression
```

## Comparing `gundi_client_v2-2.1.0.tar` & `gundi_client_v2-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1542 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/README.md
--rw-r--r--   0        0        0       53 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/gundi_client_v2/__init__.py
--rw-r--r--   0        0        0      684 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.0/gundi_client_v2/auth.py
--rw-r--r--   0        0        0     5343 2023-07-14 14:07:45.155266 gundi_client_v2-2.1.0/gundi_client_v2/client.py
--rw-r--r--   0        0        0        0 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.0/gundi_client_v2/errors.py
--rw-r--r--   0        0        0      657 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.0/gundi_client_v2/settings.py
--rw-r--r--   0        0        0      678 2023-07-14 12:42:41.019860 gundi_client_v2-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 gundi_client_v2-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1542 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.1/README.md
+-rw-r--r--   0        0        0       53 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.1/gundi_client_v2/__init__.py
+-rw-r--r--   0        0        0      684 2023-07-14 12:26:43.861804 gundi_client_v2-2.1.1/gundi_client_v2/auth.py
+-rw-r--r--   0        0        0     5343 2023-07-31 13:01:18.995535 gundi_client_v2-2.1.1/gundi_client_v2/client.py
+-rw-r--r--   0        0        0        0 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.1/gundi_client_v2/errors.py
+-rw-r--r--   0        0        0      657 2023-07-14 12:26:43.889805 gundi_client_v2-2.1.1/gundi_client_v2/settings.py
+-rw-r--r--   0        0        0      678 2023-07-31 13:18:07.096636 gundi_client_v2-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2355 1970-01-01 00:00:00.000000 gundi_client_v2-2.1.1/PKG-INFO
```

### Comparing `gundi_client_v2-2.1.0/README.md` & `gundi_client_v2-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.0/gundi_client_v2/auth.py` & `gundi_client_v2-2.1.1/gundi_client_v2/auth.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.0/gundi_client_v2/client.py` & `gundi_client_v2-2.1.1/gundi_client_v2/client.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.0/gundi_client_v2/settings.py` & `gundi_client_v2-2.1.1/gundi_client_v2/settings.py`

 * *Files identical despite different names*

### Comparing `gundi_client_v2-2.1.0/pyproject.toml` & `gundi_client_v2-2.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gundi-client-v2"
-version = "2.1.0"
+version = "2.1.1"
 description = "An async client for Gundi's API"
 authors = [
     "Chris Doehring <chrisdo@earthranger.com>",
     "Mariano M <marianom@earthranger.com>",
     "Victor Garcia <victorg@earthranger.com>"
 ]
 license = "Apache-2.0"
@@ -16,15 +16,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 environs = "^9.5"
 pydantic = "^1.10"
 httpx = "^0.24.0"
 respx = "^0.20.1"
-gundi-core = "^1.2.0"
+gundi-core = "^1.2.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pytest = "^7.2.1"
 pytest-asyncio = "^0.20.3"
 
 [build-system]
```

### Comparing `gundi_client_v2-2.1.0/PKG-INFO` & `gundi_client_v2-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: gundi-client-v2
-Version: 2.1.0
+Version: 2.1.1
 Summary: An async client for Gundi's API
 License: Apache-2.0
 Author: Chris Doehring
 Author-email: chrisdo@earthranger.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: environs (>=9.5,<10.0)
-Requires-Dist: gundi-core (>=1.2.0,<2.0.0)
+Requires-Dist: gundi-core (>=1.2.1,<2.0.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: pydantic (>=1.10,<2.0)
 Requires-Dist: respx (>=0.20.1,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Gundi Client
 ## Introduction
```

