# Comparing `tmp/edx-rest-api-client-5.5.2.tar.gz` & `tmp/edx-rest-api-client-5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-rest-api-client-5.5.2.tar", last modified: Wed May 17 15:27:29 2023, max compression
+gzip compressed data, was "edx-rest-api-client-5.6.0.tar", last modified: Mon Jul 31 16:14:33 2023, max compression
```

## Comparing `edx-rest-api-client-5.5.2.tar` & `edx-rest-api-client-5.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4890 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.791263 edx-rest-api-client-5.5.2/edx_rest_api_client/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)    13918 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/edx_rest_api_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-17 15:27:29.000000 edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 15:27:29.795263 edx-rest-api-client-5.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-05-17 15:27:21.000000 edx-rest-api-client-5.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:14:33.782187 edx-rest-api-client-5.6.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5638 2023-07-31 16:14:33.778187 edx-rest-api-client-5.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4892 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:14:33.778187 edx-rest-api-client-5.6.0/edx_rest_api_client/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/edx_rest_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/edx_rest_api_client/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2784 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/edx_rest_api_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13918 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/edx_rest_api_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/edx_rest_api_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:14:33.778187 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5638 2023-07-31 16:14:33.000000 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-31 16:14:33.000000 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 16:14:33.000000 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-31 16:14:33.000000 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-31 16:14:33.000000 edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:14:33.778187 edx-rest-api-client-5.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 16:14:33.782187 edx-rest-api-client-5.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-07-31 16:14:22.000000 edx-rest-api-client-5.6.0/setup.py
```

### Comparing `edx-rest-api-client-5.5.2/LICENSE` & `edx-rest-api-client-5.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.2/PKG-INFO` & `edx-rest-api-client-5.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.5.2
+Version: 5.6.0
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
@@ -117,15 +117,15 @@
 All community members are expected to follow the `Open edX Code of Conduct`_.
 
 .. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 .. |CI| image:: https://github.com/openedx/edx-rest-api-client/workflows/Python%20CI/badge.svg?branch=master
     :target: https://github.com/openedx/edx-rest-api-client/actions?query=workflow%3A%22Python+CI%22
     :alt: Test suite status
 
 .. |Codecov| image:: https://codecov.io/github/openedx/edx-rest-api-client/coverage.svg?branch=master
```

### Comparing `edx-rest-api-client-5.5.2/README.rst` & `edx-rest-api-client-5.6.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 All community members are expected to follow the `Open edX Code of Conduct`_.
 
 .. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 .. |CI| image:: https://github.com/openedx/edx-rest-api-client/workflows/Python%20CI/badge.svg?branch=master
     :target: https://github.com/openedx/edx-rest-api-client/actions?query=workflow%3A%22Python+CI%22
     :alt: Test suite status
 
 .. |Codecov| image:: https://codecov.io/github/openedx/edx-rest-api-client/coverage.svg?branch=master
```

### Comparing `edx-rest-api-client-5.5.2/edx_rest_api_client/auth.py` & `edx-rest-api-client-5.6.0/edx_rest_api_client/auth.py`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.2/edx_rest_api_client/client.py` & `edx-rest-api-client-5.6.0/edx_rest_api_client/client.py`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.2/edx_rest_api_client.egg-info/PKG-INFO` & `edx-rest-api-client-5.6.0/edx_rest_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-rest-api-client
-Version: 5.5.2
+Version: 5.6.0
 Summary: Client utilities to access various Open edX Platform REST APIs.
 Home-page: https://github.com/openedx/edx-rest-api-client
 Author: edX
 Author-email: oscm@edx.org
 License: Apache
 Keywords: edx rest api client
 Classifier: Development Status :: 5 - Production/Stable
@@ -117,15 +117,15 @@
 All community members are expected to follow the `Open edX Code of Conduct`_.
 
 .. _Open edX Code of Conduct: https://openedx.org/code-of-conduct/
 
 Reporting Security Issues
 *************************
 
-Please do not report security issues in public. Please email security@tcril.org.
+Please do not report security issues in public. Please email security@openedx.org.
 
 
 .. |CI| image:: https://github.com/openedx/edx-rest-api-client/workflows/Python%20CI/badge.svg?branch=master
     :target: https://github.com/openedx/edx-rest-api-client/actions?query=workflow%3A%22Python+CI%22
     :alt: Test suite status
 
 .. |Codecov| image:: https://codecov.io/github/openedx/edx-rest-api-client/coverage.svg?branch=master
```

### Comparing `edx-rest-api-client-5.5.2/requirements/constraints.txt` & `edx-rest-api-client-5.6.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-rest-api-client-5.5.2/setup.py` & `edx-rest-api-client-5.6.0/setup.py`

 * *Files identical despite different names*

