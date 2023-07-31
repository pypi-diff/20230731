# Comparing `tmp/storage-local-0.0.7.tar.gz` & `tmp/storage-local-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-local-0.0.7.tar", last modified: Mon Jul 31 10:43:42 2023, max compression
+gzip compressed data, was "storage-local-0.0.8.tar", last modified: Mon Jul 31 11:08:53 2023, max compression
```

## Comparing `storage-local-0.0.7.tar` & `storage-local-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:42.604775 storage-local-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 10:43:42.604775 storage-local-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-31 10:43:15.000000 storage-local-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:42.604775 storage-local-0.0.7/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:15.000000 storage-local-0.0.7/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 10:43:15.000000 storage-local-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:43:42.604775 storage-local-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-31 10:43:15.000000 storage-local-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:42.604775 storage-local-0.0.7/storage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 10:43:42.000000 storage-local-0.0.7/storage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-31 10:43:42.000000 storage-local-0.0.7/storage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:43:42.000000 storage-local-0.0.7/storage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 10:43:42.000000 storage-local-0.0.7/storage_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:42.604775 storage-local-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:43:15.000000 storage-local-0.0.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 10:43:15.000000 storage-local-0.0.7/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 10:43:15.000000 storage-local-0.0.7/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 11:08:53.535877 storage-local-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-31 11:08:31.000000 storage-local-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:31.000000 storage-local-0.0.8/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 11:08:31.000000 storage-local-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:08:53.535877 storage-local-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-31 11:08:31.000000 storage-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/storage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 11:08:53.000000 storage-local-0.0.8/storage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:53.535877 storage-local-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-31 11:08:31.000000 storage-local-0.0.8/tests/test_circles_storage.py
```

### Comparing `storage-local-0.0.7/README.md` & `storage-local-0.0.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,7 +42,9 @@
 "s3:PutObject"<br>
 
 # AWS Resouces
 storage.us-east-1.play1.circ.zone	arn:aws:s3:::storage.us-east-1.play1.circ.zone/*<br>
 
 # .env.play1
 Please make sure you have in your .env.play1 all the variables from .env.example<br>
+
+Please use ONLY CirclesStorage
```

### Comparing `storage-local-0.0.7/circles_local_aws_s3_storage_python/AWSStorage.py` & `storage-local-0.0.8/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/circles_local_aws_s3_storage_python/FileTypeDB.py` & `storage-local-0.0.8/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/circles_local_aws_s3_storage_python/StorageDB.py` & `storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/circles_local_aws_s3_storage_python/StorageInterface.py` & `storage-local-0.0.8/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/setup.py` & `storage-local-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='storage-local',
-    version='0.0.7',
+    version='0.0.8',
     author="Circles",
     author_email="info@circle.zone",
     description="PyPI Package for Circles S3 functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

### Comparing `storage-local-0.0.7/storage_local.egg-info/SOURCES.txt` & `storage-local-0.0.8/storage_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/tests/test_S3.py` & `storage-local-0.0.8/tests/test_S3.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.7/tests/test_circles_storage.py` & `storage-local-0.0.8/tests/test_circles_storage.py`

 * *Files identical despite different names*

