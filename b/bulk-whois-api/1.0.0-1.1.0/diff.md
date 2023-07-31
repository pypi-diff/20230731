# Comparing `tmp/bulk-whois-api-1.0.0.tar.gz` & `tmp/bulk-whois-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/foobar/prj/whoisapi/bulk-whois-api-py/dist/tmp412iiw5j/bulk-whois-api-1.0.0.tar", last modified: Sat Jan 15 09:41:56 2022, max compression
+gzip compressed data, was "bulk-whois-api-1.1.0.tar", last modified: Mon Jul 31 10:35:23 2023, max compression
```

## Comparing `bulk-whois-api-1.0.0.tar` & `bulk-whois-api-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.515808 bulk-whois-api-1.0.0/
--rw-r--r--   0 foobar     (501) staff       (20)       81 2021-11-18 09:26:29.000000 bulk-whois-api-1.0.0/AUTHORS.rst
--rw-r--r--   0 foobar     (501) staff       (20)       76 2022-01-15 06:12:19.000000 bulk-whois-api-1.0.0/CHANGELOG.rst
--rw-r--r--   0 foobar     (501) staff       (20)     1058 2022-01-12 10:32:36.000000 bulk-whois-api-1.0.0/LICENSE
--rw-r--r--   0 foobar     (501) staff       (20)      150 2021-11-18 09:26:29.000000 bulk-whois-api-1.0.0/MANIFEST.in
--rw-r--r--   0 foobar     (501) staff       (20)     3531 2022-01-15 09:41:56.515467 bulk-whois-api-1.0.0/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)     2459 2022-01-15 09:37:06.000000 bulk-whois-api-1.0.0/README.rst
--rw-r--r--   0 foobar     (501) staff       (20)       38 2022-01-15 09:41:56.515932 bulk-whois-api-1.0.0/setup.cfg
--rw-r--r--   0 foobar     (501) staff       (20)     2184 2022-01-15 08:12:43.000000 bulk-whois-api-1.0.0/setup.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.494058 bulk-whois-api-1.0.0/src/
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.499133 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/
--rw-r--r--   0 foobar     (501) staff       (20)     3531 2022-01-15 09:41:56.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)      669 2022-01-15 09:41:56.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/SOURCES.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2022-01-15 09:41:56.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/dependency_links.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2022-01-15 09:08:46.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/not-zip-safe
--rw-r--r--   0 foobar     (501) staff       (20)       37 2022-01-15 09:41:56.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/requires.txt
--rw-r--r--   0 foobar     (501) staff       (20)       13 2022-01-15 09:41:56.000000 bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/top_level.txt
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.506161 bulk-whois-api-1.0.0/src/bulkwhoisapi/
--rw-r--r--   0 foobar     (501) staff       (20)      943 2022-01-14 14:29:04.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)    16599 2022-01-14 15:23:23.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/client.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.507952 bulk-whois-api-1.0.0/src/bulkwhoisapi/exceptions/
--rw-r--r--   0 foobar     (501) staff       (20)      385 2022-01-14 10:54:08.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/exceptions/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     1789 2022-01-15 06:08:20.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/exceptions/error.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.509621 bulk-whois-api-1.0.0/src/bulkwhoisapi/models/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/models/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     6804 2022-01-14 14:24:41.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/models/response.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.511642 bulk-whois-api-1.0.0/src/bulkwhoisapi/net/
--rw-r--r--   0 foobar     (501) staff       (20)       59 2021-11-18 09:26:29.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/net/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     2640 2022-01-14 15:23:23.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/net/http.py
--rw-r--r--   0 foobar     (501) staff       (20)       53 2022-01-12 10:32:36.000000 bulk-whois-api-1.0.0/src/bulkwhoisapi/version.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-01-15 09:41:56.514454 bulk-whois-api-1.0.0/tests/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.0.0/tests/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     5967 2022-01-15 08:08:47.000000 bulk-whois-api-1.0.0/tests/client_test.py
--rw-r--r--   0 foobar     (501) staff       (20)     7350 2022-01-15 08:08:47.000000 bulk-whois-api-1.0.0/tests/model_test.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.779666 bulk-whois-api-1.1.0/
+-rw-r--r--   0 foobar     (501) staff       (20)       81 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/AUTHORS.rst
+-rw-r--r--   0 foobar     (501) staff       (20)      170 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 foobar     (501) staff       (20)     1058 2022-01-12 10:32:36.000000 bulk-whois-api-1.1.0/LICENSE
+-rw-r--r--   0 foobar     (501) staff       (20)      150 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/MANIFEST.in
+-rw-r--r--   0 foobar     (501) staff       (20)     3658 2023-07-31 10:35:23.779352 bulk-whois-api-1.1.0/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)     2459 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/README.rst
+-rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 10:35:23.779773 bulk-whois-api-1.1.0/setup.cfg
+-rw-r--r--   0 foobar     (501) staff       (20)     2235 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/setup.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.763179 bulk-whois-api-1.1.0/src/
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.768929 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/
+-rw-r--r--   0 foobar     (501) staff       (20)     3658 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)      669 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/not-zip-safe
+-rw-r--r--   0 foobar     (501) staff       (20)       37 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/requires.txt
+-rw-r--r--   0 foobar     (501) staff       (20)       13 2023-07-31 10:35:23.000000 bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/top_level.txt
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.771922 bulk-whois-api-1.1.0/src/bulkwhoisapi/
+-rw-r--r--   0 foobar     (501) staff       (20)      943 2022-01-14 14:29:04.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)    16599 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/client.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.773100 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/
+-rw-r--r--   0 foobar     (501) staff       (20)      385 2022-01-14 10:54:08.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     1789 2022-01-15 06:08:20.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/error.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.774067 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     6804 2022-01-14 14:24:41.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/models/response.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.776293 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/
+-rw-r--r--   0 foobar     (501) staff       (20)       59 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     2640 2022-01-14 15:23:23.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/net/http.py
+-rw-r--r--   0 foobar     (501) staff       (20)       53 2023-07-31 10:23:47.000000 bulk-whois-api-1.1.0/src/bulkwhoisapi/version.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 10:35:23.778516 bulk-whois-api-1.1.0/tests/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-11-18 09:26:29.000000 bulk-whois-api-1.1.0/tests/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     5967 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.0/tests/client_test.py
+-rw-r--r--   0 foobar     (501) staff       (20)     7350 2022-01-15 08:08:47.000000 bulk-whois-api-1.1.0/tests/model_test.py
```

### Comparing `bulk-whois-api-1.0.0/LICENSE` & `bulk-whois-api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/PKG-INFO` & `bulk-whois-api-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: bulk-whois-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client library for Bulk Whois API.
 Home-page: https://github.com/whois-api-llc/bulk-whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: bulk,whois,api,whoisxmlapi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :alt: bulk-whois-api-py license
     :target: https://opensource.org/licenses/MIT
@@ -42,15 +42,15 @@
 Overview
 ========
 
 The client library for
 `Bulk Whois API <https://whois.whoisxmlapi.com/bulk-api>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install bulk-whois-api
@@ -146,12 +146,17 @@
         - user_requests: [BulkRequest]
 
 
 
 Changelog
 =========
 
+1.1.0 (2023-07-31)
+------------------
+
+* Bump requests & whois-api
+* Drop Python 3.6 support
+
 1.0.0 (2022-01-15)
 ------------------
 
 * First release
-
```

### Comparing `bulk-whois-api-1.0.0/README.rst` & `bulk-whois-api-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Overview
 ========
 
 The client library for
 `Bulk Whois API <https://whois.whoisxmlapi.com/bulk-api>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install bulk-whois-api
```

### Comparing `bulk-whois-api-1.0.0/setup.py` & `bulk-whois-api-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 version_content = {}
 exec(read('src/bulkwhoisapi/version.py'), version_content)
 
 setup(
     name='bulk-whois-api',
     version=version_content['VERSION'],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     license='MIT',
     description='Python client library for Bulk Whois API.',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='WHOIS API, Inc',
@@ -47,18 +47,19 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Unix',
         'Operating System :: POSIX',
         'Operating System :: Microsoft :: Windows',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Utilities',
     ],
     keywords=[
         'bulk',
         'whois',
         'api',
         'whoisxmlapi',
```

### Comparing `bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/PKG-INFO` & `bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: bulk-whois-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python client library for Bulk Whois API.
 Home-page: https://github.com/whois-api-llc/bulk-whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: bulk,whois,api,whoisxmlapi
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :alt: bulk-whois-api-py license
     :target: https://opensource.org/licenses/MIT
@@ -42,15 +42,15 @@
 Overview
 ========
 
 The client library for
 `Bulk Whois API <https://whois.whoisxmlapi.com/bulk-api>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 
 .. code-block:: shell
 
     pip install bulk-whois-api
@@ -146,12 +146,17 @@
         - user_requests: [BulkRequest]
 
 
 
 Changelog
 =========
 
+1.1.0 (2023-07-31)
+------------------
+
+* Bump requests & whois-api
+* Drop Python 3.6 support
+
 1.0.0 (2022-01-15)
 ------------------
 
 * First release
-
```

### Comparing `bulk-whois-api-1.0.0/src/bulk_whois_api.egg-info/SOURCES.txt` & `bulk-whois-api-1.1.0/src/bulk_whois_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/src/bulkwhoisapi/__init__.py` & `bulk-whois-api-1.1.0/src/bulkwhoisapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/src/bulkwhoisapi/client.py` & `bulk-whois-api-1.1.0/src/bulkwhoisapi/client.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/src/bulkwhoisapi/exceptions/error.py` & `bulk-whois-api-1.1.0/src/bulkwhoisapi/exceptions/error.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/src/bulkwhoisapi/models/response.py` & `bulk-whois-api-1.1.0/src/bulkwhoisapi/models/response.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/src/bulkwhoisapi/net/http.py` & `bulk-whois-api-1.1.0/src/bulkwhoisapi/net/http.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/tests/client_test.py` & `bulk-whois-api-1.1.0/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `bulk-whois-api-1.0.0/tests/model_test.py` & `bulk-whois-api-1.1.0/tests/model_test.py`

 * *Files identical despite different names*

