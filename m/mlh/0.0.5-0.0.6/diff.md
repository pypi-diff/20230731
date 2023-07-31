# Comparing `tmp/mlh-0.0.5.tar.gz` & `tmp/mlh-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlh-0.0.5.tar", last modified: Mon Jul 31 18:03:53 2023, max compression
+gzip compressed data, was "mlh-0.0.6.tar", last modified: Mon Jul 31 18:18:54 2023, max compression
```

## Comparing `mlh-0.0.5.tar` & `mlh-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:03:53.733017 mlh-0.0.5/
--rw-rw-rw-   0        0        0     3157 2023-07-31 18:03:53.733017 mlh-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-07-31 16:46:11.000000 mlh-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 18:03:53.701815 mlh-0.0.5/mlh/
--rw-rw-rw-   0        0        0     1278 2023-07-31 17:20:46.000000 mlh-0.0.5/mlh/__init__.py
--rw-rw-rw-   0        0        0     5896 2023-07-31 17:59:45.000000 mlh-0.0.5/mlh/common_utils.py
--rw-rw-rw-   0        0        0     2747 2023-07-31 17:59:43.000000 mlh-0.0.5/mlh/data_from_parquet.py
--rw-rw-rw-   0        0        0     5936 2023-07-31 17:59:41.000000 mlh-0.0.5/mlh/s3_connect.py
--rw-rw-rw-   0        0        0    13560 2023-07-31 17:59:38.000000 mlh-0.0.5/mlh/snowflake_connect.py
--rw-rw-rw-   0        0        0     9666 2023-07-31 17:20:46.000000 mlh-0.0.5/mlh/sqlite_functions.py
--rw-rw-rw-   0        0        0    16876 2023-07-31 17:20:46.000000 mlh-0.0.5/mlh/support.py
--rw-rw-rw-   0        0        0    21008 2023-07-31 17:20:46.000000 mlh-0.0.5/mlh/woe.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:03:53.717395 mlh-0.0.5/mlh.egg-info/
--rw-rw-rw-   0        0        0     3157 2023-07-31 18:03:53.000000 mlh-0.0.5/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-31 18:03:53.000000 mlh-0.0.5/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:03:53.000000 mlh-0.0.5/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2023-07-31 18:03:53.000000 mlh-0.0.5/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 18:03:53.000000 mlh-0.0.5/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 18:03:53.733017 mlh-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      894 2023-07-31 17:31:41.000000 mlh-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.059581 mlh-0.0.6/
+-rw-rw-rw-   0        0        0     3157 2023-07-31 18:18:54.059581 mlh-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-07-31 16:46:11.000000 mlh-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.043564 mlh-0.0.6/mlh/
+-rw-rw-rw-   0        0        0     1278 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/__init__.py
+-rw-rw-rw-   0        0        0     5896 2023-07-31 17:59:45.000000 mlh-0.0.6/mlh/common_utils.py
+-rw-rw-rw-   0        0        0     2747 2023-07-31 17:59:43.000000 mlh-0.0.6/mlh/data_from_parquet.py
+-rw-rw-rw-   0        0        0     5936 2023-07-31 17:59:41.000000 mlh-0.0.6/mlh/s3_connect.py
+-rw-rw-rw-   0        0        0    13560 2023-07-31 17:59:38.000000 mlh-0.0.6/mlh/snowflake_connect.py
+-rw-rw-rw-   0        0        0     9666 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/sqlite_functions.py
+-rw-rw-rw-   0        0        0    16876 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/support.py
+-rw-rw-rw-   0        0        0    21008 2023-07-31 17:20:46.000000 mlh-0.0.6/mlh/woe.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:18:54.059581 mlh-0.0.6/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 18:18:53.000000 mlh-0.0.6/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 18:18:54.059581 mlh-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-07-31 18:17:09.000000 mlh-0.0.6/setup.py
```

### Comparing `mlh-0.0.5/PKG-INFO` & `mlh-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.5/README.md` & `mlh-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/__init__.py` & `mlh-0.0.6/mlh/__init__.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/common_utils.py` & `mlh-0.0.6/mlh/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/data_from_parquet.py` & `mlh-0.0.6/mlh/data_from_parquet.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/s3_connect.py` & `mlh-0.0.6/mlh/s3_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/snowflake_connect.py` & `mlh-0.0.6/mlh/snowflake_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/sqlite_functions.py` & `mlh-0.0.6/mlh/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/support.py` & `mlh-0.0.6/mlh/support.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh/woe.py` & `mlh-0.0.6/mlh/woe.py`

 * *Files identical despite different names*

### Comparing `mlh-0.0.5/mlh.egg-info/PKG-INFO` & `mlh-0.0.6/mlh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.0.5/setup.py` & `mlh-0.0.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlh",
-    version = '0.0.5',
+    version = '0.0.6',
     author="Devendra Kumar Sahu",
     author_email="devsahu99@gmail.com",
     description="This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/devsahu99/mlh",
     packages=['mlh'],
     install_requires=[
-        'pandas','scipy','IPython','matplotlib', 'snowflake-connector-python[pandas]', 's3fs', 'boto3', 'openpyxl', 'xlsxwriter', 'sagemaker', 'pyarrow', 'joblib', 'scikit-plot'
+        'pandas','scipy','IPython','matplotlib', 'snowflake-connector-python[pandas]', 's3fs', 'boto3', 'openpyxl', 'xlsxwriter'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

