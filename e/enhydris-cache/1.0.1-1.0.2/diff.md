# Comparing `tmp/enhydris-cache-1.0.1.tar.gz` & `tmp/enhydris-cache-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enhydris-cache-1.0.1.tar", last modified: Fri Mar 25 09:42:51 2022, max compression
+gzip compressed data, was "enhydris-cache-1.0.2.tar", last modified: Mon Jul 31 11:00:42 2023, max compression
```

## Comparing `enhydris-cache-1.0.1.tar` & `enhydris-cache-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      398 2022-03-25 09:40:54.000000 enhydris-cache-1.0.1/HISTORY.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      716 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/LICENSE
--rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/MANIFEST.in
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      795 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/README.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/docs/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      704 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/docs/api.rst
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1418 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/docs/conf.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/docs/history.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)      225 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/docs/index.rst
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4802 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/docs/usage.rst
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/enhydris_cache/
--rw-r--r--   0 anthony   (1000) anthony   (1000)      147 2022-03-25 09:41:40.000000 enhydris-cache-1.0.1/enhydris_cache/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4604 2022-03-25 09:40:54.000000 enhydris-cache-1.0.1/enhydris_cache/cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2220 2022-03-25 09:08:52.000000 enhydris-cache-1.0.1/enhydris_cache/enhydris_cache.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/enhydris_cache.egg-info/
--rw-r--r--   0 anthony   (1000) anthony   (1000)    12288 2022-03-25 09:41:54.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/.PKG-INFO.swp
--rw-r--r--   0 anthony   (1000) anthony   (1000)     2312 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/PKG-INFO
--rw-r--r--   0 anthony   (1000) anthony   (1000)      586 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/SOURCES.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/dependency_links.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       60 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/entry_points.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2022-03-25 08:49:59.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/not-zip-safe
--rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/requires.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       15 2022-03-25 09:42:51.000000 enhydris-cache-1.0.1/enhydris_cache.egg-info/top_level.txt
--rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/setup.cfg
--rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1706 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/setup.py
-drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2022-03-25 09:42:51.838995 enhydris-cache-1.0.1/tests/
--rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:16.000000 enhydris-cache-1.0.1/tests/__init__.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)    15960 2022-03-25 09:40:54.000000 enhydris-cache-1.0.1/tests/test_cli.py
--rw-r--r--   0 anthony   (1000) anthony   (1000)     4740 2022-03-25 09:28:10.000000 enhydris-cache-1.0.1/tests/test_enhydris_cache.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      483 2023-07-31 10:58:32.000000 enhydris-cache-1.0.2/HISTORY.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      716 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/LICENSE
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      199 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/MANIFEST.in
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2004 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      795 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/README.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/docs/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      704 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/api.rst
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1418 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/conf.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       28 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/history.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      225 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/index.rst
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4802 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/docs/usage.rst
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/enhydris_cache/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      147 2023-07-31 10:59:01.000000 enhydris-cache-1.0.2/enhydris_cache/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4604 2022-03-25 09:40:54.000000 enhydris-cache-1.0.2/enhydris_cache/cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2220 2022-03-25 09:08:52.000000 enhydris-cache-1.0.2/enhydris_cache/enhydris_cache.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/enhydris_cache.egg-info/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     2004 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/PKG-INFO
+-rw-r--r--   0 anthony   (1000) anthony   (1000)      548 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       59 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/entry_points.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        1 2023-07-31 10:48:14.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/not-zip-safe
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       41 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/requires.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       15 2023-07-31 11:00:42.000000 enhydris-cache-1.0.2/enhydris_cache.egg-info/top_level.txt
+-rw-r--r--   0 anthony   (1000) anthony   (1000)       92 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/setup.cfg
+-rwxr-xr-x   0 anthony   (1000) anthony   (1000)     1706 2023-07-31 10:58:32.000000 enhydris-cache-1.0.2/setup.py
+drwxr-xr-x   0 anthony   (1000) anthony   (1000)        0 2023-07-31 11:00:42.265578 enhydris-cache-1.0.2/tests/
+-rw-r--r--   0 anthony   (1000) anthony   (1000)        0 2022-03-05 20:41:16.000000 enhydris-cache-1.0.2/tests/__init__.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)    15960 2022-03-25 09:40:54.000000 enhydris-cache-1.0.2/tests/test_cli.py
+-rw-r--r--   0 anthony   (1000) anthony   (1000)     4740 2022-03-25 09:28:10.000000 enhydris-cache-1.0.2/tests/test_enhydris_cache.py
```

### Comparing `enhydris-cache-1.0.1/LICENSE` & `enhydris-cache-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/PKG-INFO` & `enhydris-cache-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 Metadata-Version: 2.1
 Name: enhydris-cache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/enhydris-cache
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
-Description: ==============
-        enhydris-cache
-        ==============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
-                :target: https://pypi.python.org/pypi/enhydris-cache
-        
-        .. image:: https://img.shields.io/travis/openmeteo/enhydris-cache.svg
-                :target: https://travis-ci.org/openmeteo/enhydris-cache
-        
-        .. image:: https://codecov.io/github/openmeteo/enhydris-cache/coverage.svg
-                :target: https://codecov.io/gh/openmeteo/enhydris-cache
-                :alt: Coverage
-        
-        .. image:: https://pyup.io/repos/github/openmeteo/enhydris-cache/shield.svg
-                 :target: https://pyup.io/repos/github/openmeteo/enhydris-cache/
-                 :alt: Updates
-        
-        Utilities for spatial integration of time series.
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://enhydris-cache.readthedocs.io.
-        
-        
-        =======
-        History
-        =======
-        
-        1.0.1 (2022-03-25)
-        ==================
-        
-        - Fixed error when attempting to connect to Enhydris unauthenticated.
-        
-        1.0.0 (2021-08-31)
-        ==================
-        
-        - The configuration file has changed; it now needs the timeseries_group_id
-          parameter.
-        - Needs Python 3.7 or later.
-        - Updated dependencies.
-        - Updated pypi metadata.
-        
-        0.1.1 (2019-06-13)
-        ==================
-        
-        - Initial release
-        
 Keywords: enhydris-cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==============
+enhydris-cache
+==============
+
+
+.. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
+        :target: https://pypi.python.org/pypi/enhydris-cache
+
+.. image:: https://img.shields.io/travis/openmeteo/enhydris-cache.svg
+        :target: https://travis-ci.org/openmeteo/enhydris-cache
+
+.. image:: https://codecov.io/github/openmeteo/enhydris-cache/coverage.svg
+        :target: https://codecov.io/gh/openmeteo/enhydris-cache
+        :alt: Coverage
+
+.. image:: https://pyup.io/repos/github/openmeteo/enhydris-cache/shield.svg
+         :target: https://pyup.io/repos/github/openmeteo/enhydris-cache/
+         :alt: Updates
+
+Utilities for spatial integration of time series.
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://enhydris-cache.readthedocs.io.
+
+
+=======
+History
+=======
+
+1.0.2 (2023-07-31)
+==================
+
+- Allow running with enhydris-api-client v.3
+
+1.0.1 (2022-03-25)
+==================
+
+- Fixed error when attempting to connect to Enhydris unauthenticated.
+
+1.0.0 (2021-08-31)
+==================
+
+- The configuration file has changed; it now needs the timeseries_group_id
+  parameter.
+- Needs Python 3.7 or later.
+- Updated dependencies.
+- Updated pypi metadata.
+
+0.1.1 (2019-06-13)
+==================
+
+- Initial release
```

### Comparing `enhydris-cache-1.0.1/README.rst` & `enhydris-cache-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/docs/api.rst` & `enhydris-cache-1.0.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/docs/conf.py` & `enhydris-cache-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/docs/usage.rst` & `enhydris-cache-1.0.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/enhydris_cache/cli.py` & `enhydris-cache-1.0.2/enhydris_cache/cli.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/enhydris_cache/enhydris_cache.py` & `enhydris-cache-1.0.2/enhydris_cache/enhydris_cache.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/enhydris_cache.egg-info/PKG-INFO` & `enhydris-cache-1.0.2/enhydris_cache.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 Metadata-Version: 2.1
 Name: enhydris-cache
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for spatial integration of time series
 Home-page: https://github.com/openmeteo/enhydris-cache
 Author: Antonis Christofides
 Author-email: antonis@antonischristofides.com
 License: GNU General Public License v3
-Description: ==============
-        enhydris-cache
-        ==============
-        
-        
-        .. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
-                :target: https://pypi.python.org/pypi/enhydris-cache
-        
-        .. image:: https://img.shields.io/travis/openmeteo/enhydris-cache.svg
-                :target: https://travis-ci.org/openmeteo/enhydris-cache
-        
-        .. image:: https://codecov.io/github/openmeteo/enhydris-cache/coverage.svg
-                :target: https://codecov.io/gh/openmeteo/enhydris-cache
-                :alt: Coverage
-        
-        .. image:: https://pyup.io/repos/github/openmeteo/enhydris-cache/shield.svg
-                 :target: https://pyup.io/repos/github/openmeteo/enhydris-cache/
-                 :alt: Updates
-        
-        Utilities for spatial integration of time series.
-        
-        
-        * Free software: GNU General Public License v3
-        * Documentation: https://enhydris-cache.readthedocs.io.
-        
-        
-        =======
-        History
-        =======
-        
-        1.0.1 (2022-03-25)
-        ==================
-        
-        - Fixed error when attempting to connect to Enhydris unauthenticated.
-        
-        1.0.0 (2021-08-31)
-        ==================
-        
-        - The configuration file has changed; it now needs the timeseries_group_id
-          parameter.
-        - Needs Python 3.7 or later.
-        - Updated dependencies.
-        - Updated pypi metadata.
-        
-        0.1.1 (2019-06-13)
-        ==================
-        
-        - Initial release
-        
 Keywords: enhydris-cache
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+==============
+enhydris-cache
+==============
+
+
+.. image:: https://img.shields.io/pypi/v/enhydris-cache.svg
+        :target: https://pypi.python.org/pypi/enhydris-cache
+
+.. image:: https://img.shields.io/travis/openmeteo/enhydris-cache.svg
+        :target: https://travis-ci.org/openmeteo/enhydris-cache
+
+.. image:: https://codecov.io/github/openmeteo/enhydris-cache/coverage.svg
+        :target: https://codecov.io/gh/openmeteo/enhydris-cache
+        :alt: Coverage
+
+.. image:: https://pyup.io/repos/github/openmeteo/enhydris-cache/shield.svg
+         :target: https://pyup.io/repos/github/openmeteo/enhydris-cache/
+         :alt: Updates
+
+Utilities for spatial integration of time series.
+
+
+* Free software: GNU General Public License v3
+* Documentation: https://enhydris-cache.readthedocs.io.
+
+
+=======
+History
+=======
+
+1.0.2 (2023-07-31)
+==================
+
+- Allow running with enhydris-api-client v.3
+
+1.0.1 (2022-03-25)
+==================
+
+- Fixed error when attempting to connect to Enhydris unauthenticated.
+
+1.0.0 (2021-08-31)
+==================
+
+- The configuration file has changed; it now needs the timeseries_group_id
+  parameter.
+- Needs Python 3.7 or later.
+- Updated dependencies.
+- Updated pypi metadata.
+
+0.1.1 (2019-06-13)
+==================
+
+- Initial release
```

### Comparing `enhydris-cache-1.0.1/enhydris_cache.egg-info/SOURCES.txt` & `enhydris-cache-1.0.2/enhydris_cache.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 docs/conf.py
 docs/history.rst
 docs/index.rst
 docs/usage.rst
 enhydris_cache/__init__.py
 enhydris_cache/cli.py
 enhydris_cache/enhydris_cache.py
-enhydris_cache.egg-info/.PKG-INFO.swp
 enhydris_cache.egg-info/PKG-INFO
 enhydris_cache.egg-info/SOURCES.txt
 enhydris_cache.egg-info/dependency_links.txt
 enhydris_cache.egg-info/entry_points.txt
 enhydris_cache.egg-info/not-zip-safe
 enhydris_cache.egg-info/requires.txt
 enhydris_cache.egg-info/top_level.txt
```

### Comparing `enhydris-cache-1.0.1/setup.py` & `enhydris-cache-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("README.rst") as readme_file:
     readme = readme_file.read()
 
 with open("HISTORY.rst") as history_file:
     history = history_file.read()
 
-requirements = ["Click>=7.0", "enhydris-api-client>=2.0.1,<3"]
+requirements = ["Click>=7.0", "enhydris-api-client>=2.0.1,<4"]
 
 test_requirements = []
 
 
 def get_version():
     scriptdir = os.path.dirname(os.path.abspath(__file__))
     init_py_path = os.path.join(scriptdir, "enhydris_cache", "__init__.py")
```

### Comparing `enhydris-cache-1.0.1/tests/test_cli.py` & `enhydris-cache-1.0.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `enhydris-cache-1.0.1/tests/test_enhydris_cache.py` & `enhydris-cache-1.0.2/tests/test_enhydris_cache.py`

 * *Files identical despite different names*

