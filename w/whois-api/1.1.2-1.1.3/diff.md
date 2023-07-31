# Comparing `tmp/whois-api-1.1.2.tar.gz` & `tmp/whois-api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-api-1.1.2.tar", last modified: Tue Nov  8 12:08:00 2022, max compression
+gzip compressed data, was "whois-api-1.1.3.tar", last modified: Mon Jul 31 09:35:05 2023, max compression
```

## Comparing `whois-api-1.1.2.tar` & `whois-api-1.1.3.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.127176 whois-api-1.1.2/
--rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.1.2/AUTHORS.rst
--rw-r--r--   0 foobar     (501) staff       (20)      345 2022-11-08 12:07:04.000000 whois-api-1.1.2/CHANGELOG.rst
--rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.1.2/LICENSE
--rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.1.2/MANIFEST.in
--rw-r--r--   0 foobar     (501) staff       (20)     2916 2022-11-08 12:08:00.126532 whois-api-1.1.2/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)     1614 2021-11-19 14:11:58.000000 whois-api-1.1.2/README.rst
--rw-r--r--   0 foobar     (501) staff       (20)       38 2022-11-08 12:08:00.127395 whois-api-1.1.2/setup.cfg
--rw-r--r--   0 foobar     (501) staff       (20)     2011 2022-11-08 12:07:04.000000 whois-api-1.1.2/setup.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.107346 whois-api-1.1.2/src/
--rw-r--r--   0 foobar     (501) staff       (20)     6148 2022-04-20 08:40:18.000000 whois-api-1.1.2/src/.DS_Store
--rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.1.2/src/__init__.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.111656 whois-api-1.1.2/src/whois_api.egg-info/
--rw-r--r--   0 foobar     (501) staff       (20)     2916 2022-11-08 12:08:00.000000 whois-api-1.1.2/src/whois_api.egg-info/PKG-INFO
--rw-r--r--   0 foobar     (501) staff       (20)      648 2022-11-08 12:08:00.000000 whois-api-1.1.2/src/whois_api.egg-info/SOURCES.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2022-11-08 12:08:00.000000 whois-api-1.1.2/src/whois_api.egg-info/dependency_links.txt
--rw-r--r--   0 foobar     (501) staff       (20)        1 2022-11-08 12:07:59.000000 whois-api-1.1.2/src/whois_api.egg-info/not-zip-safe
--rw-r--r--   0 foobar     (501) staff       (20)       20 2022-11-08 12:08:00.000000 whois-api-1.1.2/src/whois_api.egg-info/requires.txt
--rw-r--r--   0 foobar     (501) staff       (20)       18 2022-11-08 12:08:00.000000 whois-api-1.1.2/src/whois_api.egg-info/top_level.txt
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.113244 whois-api-1.1.2/src/whoisapi/
--rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/client.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.115580 whois-api-1.1.2/src/whoisapi/exceptions/
--rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/exceptions/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/exceptions/error.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.120379 whois-api-1.1.2/src/whoisapi/models/
--rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.1.2/src/whoisapi/models/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.1.2/src/whoisapi/models/base.py
--rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/models/request.py
--rw-r--r--   0 foobar     (501) staff       (20)    12429 2021-11-19 14:11:58.000000 whois-api-1.1.2/src/whoisapi/models/response.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.122853 whois-api-1.1.2/src/whoisapi/net/
--rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.1.2/src/whoisapi/net/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.1.2/src/whoisapi/net/http.py
-drwxr-xr-x   0 foobar     (501) staff       (20)        0 2022-11-08 12:08:00.124956 whois-api-1.1.2/tests/
--rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.1.2/tests/__init__.py
--rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.1.2/tests/client_test.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.031524 whois-api-1.1.3/
+-rw-r--r--   0 foobar     (501) staff       (20)       81 2021-04-14 07:33:27.000000 whois-api-1.1.3/AUTHORS.rst
+-rw-r--r--   0 foobar     (501) staff       (20)      427 2023-07-31 08:35:10.000000 whois-api-1.1.3/CHANGELOG.rst
+-rw-r--r--   0 foobar     (501) staff       (20)     1058 2021-04-14 07:33:27.000000 whois-api-1.1.3/LICENSE
+-rw-r--r--   0 foobar     (501) staff       (20)      150 2021-04-14 07:33:27.000000 whois-api-1.1.3/MANIFEST.in
+-rw-r--r--   0 foobar     (501) staff       (20)     3050 2023-07-31 09:35:05.031042 whois-api-1.1.3/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)     1614 2023-07-31 08:12:01.000000 whois-api-1.1.3/README.rst
+-rw-r--r--   0 foobar     (501) staff       (20)       38 2023-07-31 09:35:05.031715 whois-api-1.1.3/setup.cfg
+-rw-r--r--   0 foobar     (501) staff       (20)     2062 2023-07-31 08:35:10.000000 whois-api-1.1.3/setup.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.020141 whois-api-1.1.3/src/
+-rw-r--r--   0 foobar     (501) staff       (20)       23 2021-04-14 08:34:58.000000 whois-api-1.1.3/src/__init__.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.023158 whois-api-1.1.3/src/whois_api.egg-info/
+-rw-r--r--   0 foobar     (501) staff       (20)     3050 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/PKG-INFO
+-rw-r--r--   0 foobar     (501) staff       (20)      634 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/SOURCES.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/dependency_links.txt
+-rw-r--r--   0 foobar     (501) staff       (20)        1 2023-07-31 09:33:16.000000 whois-api-1.1.3/src/whois_api.egg-info/not-zip-safe
+-rw-r--r--   0 foobar     (501) staff       (20)       20 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/requires.txt
+-rw-r--r--   0 foobar     (501) staff       (20)       18 2023-07-31 09:35:05.000000 whois-api-1.1.3/src/whois_api.egg-info/top_level.txt
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.024061 whois-api-1.1.3/src/whoisapi/
+-rw-r--r--   0 foobar     (501) staff       (20)      712 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3177 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/client.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.024988 whois-api-1.1.3/src/whoisapi/exceptions/
+-rw-r--r--   0 foobar     (501) staff       (20)      312 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/exceptions/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     1186 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/exceptions/error.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.027477 whois-api-1.1.3/src/whoisapi/models/
+-rw-r--r--   0 foobar     (501) staff       (20)      262 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/models/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)      600 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/models/base.py
+-rw-r--r--   0 foobar     (501) staff       (20)     5618 2021-11-19 14:11:58.000000 whois-api-1.1.3/src/whoisapi/models/request.py
+-rw-r--r--   0 foobar     (501) staff       (20)    12429 2023-07-31 08:36:47.000000 whois-api-1.1.3/src/whoisapi/models/response.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.029199 whois-api-1.1.3/src/whoisapi/net/
+-rw-r--r--   0 foobar     (501) staff       (20)       59 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/net/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     3369 2021-04-14 07:33:27.000000 whois-api-1.1.3/src/whoisapi/net/http.py
+drwxr-xr-x   0 foobar     (501) staff       (20)        0 2023-07-31 09:35:05.030258 whois-api-1.1.3/tests/
+-rw-r--r--   0 foobar     (501) staff       (20)        0 2021-04-14 07:33:27.000000 whois-api-1.1.3/tests/__init__.py
+-rw-r--r--   0 foobar     (501) staff       (20)     2012 2021-04-14 10:02:07.000000 whois-api-1.1.3/tests/client_test.py
```

### Comparing `whois-api-1.1.2/LICENSE` & `whois-api-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/PKG-INFO` & `whois-api-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
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
-Requires-Python: ~=3.6
+Requires-Python: ~=3.7
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :alt: whois-api-py license
     :target: https://opensource.org/licenses/MIT
@@ -41,15 +42,15 @@
 Overview
 ========
 
 The client library for
 `Whois API <https://whois.whoisxmlapi.com/>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 ::
 
     pip install whois-api
 
@@ -96,14 +97,20 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.1.3 (2023-07-31)
+------------------
+
+* Bump requests
+* Drop Python 3.6 support
+
 1.1.2 (2022-11-08)
 ------------------
 
 * Bump urllib3
 
 1.1.1 (2021-11-19)
 ------------------
```

### Comparing `whois-api-1.1.2/README.rst` & `whois-api-1.1.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Overview
 ========
 
 The client library for
 `Whois API <https://whois.whoisxmlapi.com/>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 ::
 
     pip install whois-api
```

### Comparing `whois-api-1.1.2/setup.py` & `whois-api-1.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         join(dirname(__file__), *names),
         encoding=kwargs.get('encoding', 'utf8')
     ).read()
 
 
 setup(
     name='whois-api',
-    version='1.1.2',
-    python_requires='~=3.6',
+    version='1.1.3',
+    python_requires='~=3.7',
     license='MIT',
     description='Python client library for Whois API.',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('', read('README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
     ),
     author='WHOIS API, Inc',
@@ -44,18 +44,19 @@
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
         'whois',
         'api',
         'whoisxmlapi',
     ],
```

### Comparing `whois-api-1.1.2/src/whois_api.egg-info/PKG-INFO` & `whois-api-1.1.3/src/whois_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: whois-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: Python client library for Whois API.
 Home-page: https://github.com/whois-api-llc/whois-api-py
 Author: WHOIS API, Inc
 Author-email: support@whoisxmlapi.com
 License: MIT
 Keywords: whois,api,whoisxmlapi
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
-Requires-Python: ~=3.6
+Requires-Python: ~=3.7
 Provides-Extra: dev
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 .. image:: https://img.shields.io/badge/License-MIT-green.svg
     :alt: whois-api-py license
     :target: https://opensource.org/licenses/MIT
@@ -41,15 +42,15 @@
 Overview
 ========
 
 The client library for
 `Whois API <https://whois.whoisxmlapi.com/>`_
 in Python language.
 
-The minimum Python version is 3.6.
+The minimum Python version is 3.7.
 
 Installation
 ============
 ::
 
     pip install whois-api
 
@@ -96,14 +97,20 @@
     client.parameters.output_format = 'xml'
     print(client.raw_data('whoisxmlapi.com'))
 
 
 Changelog
 =========
 
+1.1.3 (2023-07-31)
+------------------
+
+* Bump requests
+* Drop Python 3.6 support
+
 1.1.2 (2022-11-08)
 ------------------
 
 * Bump urllib3
 
 1.1.1 (2021-11-19)
 ------------------
```

### Comparing `whois-api-1.1.2/src/whois_api.egg-info/SOURCES.txt` & `whois-api-1.1.3/src/whois_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
-src/.DS_Store
 src/__init__.py
 src/whois_api.egg-info/PKG-INFO
 src/whois_api.egg-info/SOURCES.txt
 src/whois_api.egg-info/dependency_links.txt
 src/whois_api.egg-info/not-zip-safe
 src/whois_api.egg-info/requires.txt
 src/whois_api.egg-info/top_level.txt
```

### Comparing `whois-api-1.1.2/src/whoisapi/__init__.py` & `whois-api-1.1.3/src/whoisapi/__init__.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/client.py` & `whois-api-1.1.3/src/whoisapi/client.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/exceptions/error.py` & `whois-api-1.1.3/src/whoisapi/exceptions/error.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/models/base.py` & `whois-api-1.1.3/src/whoisapi/models/base.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/models/request.py` & `whois-api-1.1.3/src/whoisapi/models/request.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/models/response.py` & `whois-api-1.1.3/src/whoisapi/models/response.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/src/whoisapi/net/http.py` & `whois-api-1.1.3/src/whoisapi/net/http.py`

 * *Files identical despite different names*

### Comparing `whois-api-1.1.2/tests/client_test.py` & `whois-api-1.1.3/tests/client_test.py`

 * *Files identical despite different names*

