# Comparing `tmp/gooddata-fdw-1.3.1.dev5.tar.gz` & `tmp/gooddata-fdw-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooddata-fdw-1.3.1.dev5.tar", last modified: Fri Jun 23 15:18:32 2023, max compression
+gzip compressed data, was "gooddata-fdw-1.4.0.tar", last modified: Mon Jul 31 09:28:07 2023, max compression
```

## Comparing `gooddata-fdw-1.3.1.dev5.tar` & `gooddata-fdw-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:32.601807 gooddata-fdw-1.3.1.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-23 15:18:32.601807 gooddata-fdw-1.3.1.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:32.601807 gooddata-fdw-1.3.1.dev5/gooddata_fdw/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/column_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/column_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/fdw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/import_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/pg_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-06-23 15:18:15.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw/result_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:18:32.601807 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-23 15:18:32.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 15:18:32.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:18:32.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 15:18:32.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-23 15:18:32.000000 gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:18:32.601807 gooddata-fdw-1.3.1.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-23 15:18:24.000000 gooddata-fdw-1.3.1.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.742010 gooddata-fdw-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    40366 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-31 09:28:07.742010 gooddata-fdw-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.738010 gooddata-fdw-1.4.0/gooddata_fdw/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/column_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/column_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/fdw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/import_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/pg_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/gooddata_fdw/result_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:28:07.738010 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-07-31 09:28:07.000000 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-31 09:28:07.000000 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:28:07.000000 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 09:28:07.000000 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:28:07.000000 gooddata-fdw-1.4.0/gooddata_fdw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:28:07.742010 gooddata-fdw-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-31 09:27:55.000000 gooddata-fdw-1.4.0/setup.py
```

### Comparing `gooddata-fdw-1.3.1.dev5/LICENSE.txt` & `gooddata-fdw-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/PKG-INFO` & `gooddata-fdw-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.3.1.dev5
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Foreign Data Wrapper
 
 This project delivers PostgreSQL foreign data wrapper extension built on top of [multicorn](https://multicorn.org/).
 The extension makes [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) insights, computations and ad-hoc report data available in PostgreSQL as tables.
```

### Comparing `gooddata-fdw-1.3.1.dev5/README.md` & `gooddata-fdw-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/column_utils.py` & `gooddata-fdw-1.4.0/gooddata_fdw/column_utils.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/column_validation.py` & `gooddata-fdw-1.4.0/gooddata_fdw/column_validation.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/environment.py` & `gooddata-fdw-1.4.0/gooddata_fdw/environment.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/executor.py` & `gooddata-fdw-1.4.0/gooddata_fdw/executor.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/fdw.py` & `gooddata-fdw-1.4.0/gooddata_fdw/fdw.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/filter.py` & `gooddata-fdw-1.4.0/gooddata_fdw/filter.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/import_workspace.py` & `gooddata-fdw-1.4.0/gooddata_fdw/import_workspace.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/naming.py` & `gooddata-fdw-1.4.0/gooddata_fdw/naming.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/options.py` & `gooddata-fdw-1.4.0/gooddata_fdw/options.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/pg_logging.py` & `gooddata-fdw-1.4.0/gooddata_fdw/pg_logging.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw/result_reader.py` & `gooddata-fdw-1.4.0/gooddata_fdw/result_reader.py`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/PKG-INFO` & `gooddata-fdw-1.4.0/gooddata_fdw.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: gooddata-fdw
-Version: 1.3.1.dev5
+Version: 1.4.0
 Summary: GoodData.CN Foreign Data Wrapper For PostgreSQL
 Author: GoodData
 Author-email: support@gooddata.com
 License: MIT
-Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.3.1.dev5
+Project-URL: Documentation, https://gooddata-fdw.readthedocs.io/en/v1.4.0
 Project-URL: Source, https://github.com/gooddata/gooddata-python-sdk
 Keywords: gooddata,fdw,postgresql,analytics,headless,business,intelligence,headless-bi,cloud,native,semantic,layer,sql,metrics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # GoodData Foreign Data Wrapper
 
 This project delivers PostgreSQL foreign data wrapper extension built on top of [multicorn](https://multicorn.org/).
 The extension makes [GoodData.CN](https://www.gooddata.com/developers/cloud-native/) insights, computations and ad-hoc report data available in PostgreSQL as tables.
```

### Comparing `gooddata-fdw-1.3.1.dev5/gooddata_fdw.egg-info/SOURCES.txt` & `gooddata-fdw-1.4.0/gooddata_fdw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gooddata-fdw-1.3.1.dev5/setup.py` & `gooddata-fdw-1.4.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,46 +3,44 @@
 
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 REQUIRES = [
-    "gooddata-sdk~=1.3.1.dev5",
-    'importlib-metadata >= 1.0 ; python_version >= "3.7"',
+    "gooddata-sdk~=1.4.0",
     #    "multicorn>=1.4.0",
 ]
 
-
 setup(
     name="gooddata-fdw",
     description="GoodData.CN Foreign Data Wrapper For PostgreSQL",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="1.3.1.dev5",
+    version="1.4.0",
     author="GoodData",
     author_email="support@gooddata.com",
     license="MIT",
     license_file="LICENSE.txt",
     license_files=("LICENSE.txt",),
     install_requires=REQUIRES,
     packages=find_packages(exclude=["tests*"]),
-    python_requires=">=3.7.0",
+    python_requires=">=3.8.0",
     project_urls={
-        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.3.1.dev5",
+        "Documentation": "https://gooddata-fdw.readthedocs.io/en/v1.4.0",
         "Source": "https://github.com/gooddata/gooddata-python-sdk",
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Database",
         "Topic :: Scientific/Engineering",
         "Topic :: Software Development",
         "Typing :: Typed",
     ],
     keywords=[
         "gooddata",
```

