# Comparing `tmp/bulk-whois-api-1.1.0.tar.gz` & `tmp/bulk-whois-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulk-whois-api-1.1.0.tar", last modified: Mon Jul 31 10:35:23 2023, max compression
+gzip compressed data, was "bulk-whois-api-1.1.1.tar", last modified: Mon Jul 31 11:52:15 2023, max compression
```

## Comparing `bulk-whois-api-1.1.0.tar` & `bulk-whois-api-1.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.779666 bulk-whois-api-1.1.0/
--rw-r--r--   0 foobar     (501) staff       (20)       81 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/AUTHORS.rst
--rw-r--r--   0 foobar     (501) staff       (20)      170 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/CHANGELOG.rst
--rw-r--r--   0 foobar     (501) staff       (20)     1058 2022-01-12 10:32:36.000000 bulk-whois-api-1.1.0/LICENSE
--rw-r--r--   0 foobar     (501) staff       (20)      150 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/MANIFEST.in
--rw-r--r--   0 foobar     (501) staff       (20)     3658 2023-07-31 10:35:23.779352 bulk-whois-api-1.1.0/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)     2459 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/README.rst
--rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 10:35:23.779773 bulk-whois-api-1.1.0/setup.cfg
--rw-r--r--   0 foobar     (501) staff       (20)     2235 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/setup.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.763179 bulk-whois-api-1.1.0/src/
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.768929 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/
--rw-r--r--   0 foobar     (501) staff       (20)     3658 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)      669 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/SOURCES.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/dependency_links.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/not-zip-safe
--rw-r--r--   0 foobar     (501) staff       (20)       37 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/requires.txt
--rw-r--r--   0 foobar     (501) staff       (20)       13 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/top_level.txt
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.771922 bulk-whois-api-1.1.0/src/bulkwhoisapi/
--rw-r--r--   0 foobar     (501) staff       (20)      943 2022-01-14 14:29:04.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)    16599 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/client.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.773100 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/
--rw-r--r--   0 foobar     (501) staff       (20)      385 2022-01-14 10:54:08.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     1789 2022-01-15 06:08:20.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/error.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.774067 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     6804 2022-01-14 14:24:41.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/response.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.776293 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/
--rw-r--r--   0 foobar     (501) staff       (20)       59 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     2640 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/http.py
--rw-r--r--   0 foobar     (501) staff       (20)       53 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/version.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.778516 bulk-whois-api-1.1.0/tests/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/tests/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     5967 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.0/tests/client_test.py
--rw-r--r--   0 foobar     (501) staff       (20)     7350 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.0/tests/model_test.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.138991 bulk-whois-api-1.1.1/
+-rw-r--r--   0 foobar     (501) staff       (20)       81 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.1/AUTHORS.rst
+-rw-r--r--   0 foobar     (501) staff       (20)      227 2023-07-31 11:51:37.000000 bulk-whois-api-1.1.1/CHANGELOG.rst
+-rw-r--r--   0 foobar     (501) staff       (20)     1058 2022-01-12 10:32:36.000000 bulk-whois-api-1.1.1/LICENSE
+-rw-r--r--   0 foobar     (501) staff       (20)      150 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.1/MANIFEST.in
+-rw-r--r--   0 foobar     (501) staff       (20)     3715 2023-07-31 11:52:15.135997 bulk-whois-api-1.1.1/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)     2459 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.1/README.rst
+-rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 11:52:15.139245 bulk-whois-api-1.1.1/setup.cfg
+-rw-r--r--   0 foobar     (501) staff       (20)     2235 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.1/setup.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.116955 bulk-whois-api-1.1.1/src/
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.123008 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/
+-rw-r--r--   0 foobar     (501) staff       (20)     3715 2023-07-31 11:52:15.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)      669 2023-07-31 11:52:15.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 11:52:15.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/not-zip-safe
+-rw-r--r--   0 foobar     (501) staff       (20)       37 2023-07-31 11:52:15.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/requires.txt
+-rw-r--r--   0 foobar     (501) staff       (20)       13 2023-07-31 11:52:15.000000 bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/top_level.txt
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.126531 bulk-whois-api-1.1.1/src/bulkwhoisapi/
+-rw-r--r--   0 foobar     (501) staff       (20)      943 2022-01-14 14:29:04.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)    16599 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/client.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.127730 bulk-whois-api-1.1.1/src/bulkwhoisapi/exceptions/
+-rw-r--r--   0 foobar     (501) staff       (20)      385 2022-01-14 10:54:08.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/exceptions/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     1789 2022-01-15 06:08:20.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/exceptions/error.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.129016 bulk-whois-api-1.1.1/src/bulkwhoisapi/models/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/models/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     6804 2022-01-14 14:24:41.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/models/response.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.132356 bulk-whois-api-1.1.1/src/bulkwhoisapi/net/
+-rw-r--r--   0 foobar     (501) staff       (20)       59 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/net/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     2640 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/net/http.py
+-rw-r--r--   0 foobar     (501) staff       (20)       53 2023-07-31 11:51:37.000000 bulk-whois-api-1.1.1/src/bulkwhoisapi/version.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 11:52:15.134477 bulk-whois-api-1.1.1/tests/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.1/tests/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     5967 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.1/tests/client_test.py
+-rw-r--r--   0 foobar     (501) staff       (20)     7350 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.1/tests/model_test.py
```

### Comparing `bulk-whois-api-1.1.0/LICENSE` & `bulk-whois-api-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/PKG-INFO` & `bulk-whois-api-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-whois-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client library for Bulk Whois API.
 Home-page: https://github.com/whois-api-llc/bulk-whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: bulk,whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -146,14 +146,19 @@
         - user_requests: [BulkRequest]
 
 
 
 Changelog
 =========
 
+1.1.1 (2023-07-31)
+------------------
+
+* Bump whois-api
+
 1.1.0 (2023-07-31)
 ------------------
 
 * Bump requests & whois-api
 * Drop Python 3.6 support
 
 1.0.0 (2022-01-15)
```

### Comparing `bulk-whois-api-1.1.0/README.rst` & `bulk-whois-api-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/setup.py` & `bulk-whois-api-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/PKG-INFO` & `bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulk-whois-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python client library for Bulk Whois API.
 Home-page: https://github.com/whois-api-llc/bulk-whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: bulk,whois,api,whoisxmlapi
 Classifier: Development Status :: 5 - Production/Stable
@@ -146,14 +146,19 @@
         - user_requests: [BulkRequest]
 
 
 
 Changelog
 =========
 
+1.1.1 (2023-07-31)
+------------------
+
+* Bump whois-api
+
 1.1.0 (2023-07-31)
 ------------------
 
 * Bump requests & whois-api
 * Drop Python 3.6 support
 
 1.0.0 (2022-01-15)
```

### Comparing `bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/SOURCES.txt` & `bulk-whois-api-1.1.1/src/bulk_whois_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulkwhoisapi/__init__.py` & `bulk-whois-api-1.1.1/src/bulkwhoisapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulkwhoisapi/client.py` & `bulk-whois-api-1.1.1/src/bulkwhoisapi/client.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/error.py` & `bulk-whois-api-1.1.1/src/bulkwhoisapi/exceptions/error.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulkwhoisapi/models/response.py` & `bulk-whois-api-1.1.1/src/bulkwhoisapi/models/response.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/src/bulkwhoisapi/net/http.py` & `bulk-whois-api-1.1.1/src/bulkwhoisapi/net/http.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/tests/client_test.py` & `bulk-whois-api-1.1.1/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.1.0/tests/model_test.py` & `bulk-whois-api-1.1.1/tests/model_test.py`

 * *Files identical despite different names*

