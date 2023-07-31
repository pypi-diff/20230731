# Comparing `tmp/catalystai-1.0.1.tar.gz` & `tmp/catalystai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystai-1.0.1.tar", last modified: Mon Jul 31 12:51:56 2023, max compression
+gzip compressed data, was "catalystai-1.0.2.tar", last modified: Mon Jul 31 12:54:36 2023, max compression
```

## Comparing `catalystai-1.0.1.tar` & `catalystai-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:51:56.584208 catalystai-1.0.1/
--rw-rw-rw-   0        0        0      106 2023-07-31 12:51:36.000000 catalystai-1.0.1/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.1/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-07-31 12:51:56.583199 catalystai-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 12:51:56.567886 catalystai-1.0.1/catalystai/
--rw-rw-rw-   0        0        0       26 2023-07-31 12:50:35.000000 catalystai-1.0.1/catalystai/__init__.py
--rw-rw-rw-   0        0        0     3316 2023-07-31 12:41:24.000000 catalystai-1.0.1/catalystai/minio.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:51:56.582210 catalystai-1.0.1/catalystai.egg-info/
--rw-rw-rw-   0        0        0      543 2023-07-31 12:51:56.000000 catalystai-1.0.1/catalystai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-31 12:51:56.000000 catalystai-1.0.1/catalystai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:51:56.000000 catalystai-1.0.1/catalystai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 12:51:56.000000 catalystai-1.0.1/catalystai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:51:56.584208 catalystai-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-31 12:51:40.000000 catalystai-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.491723 catalystai-1.0.2/
+-rw-rw-rw-   0        0        0      220 2023-07-31 12:54:28.000000 catalystai-1.0.2/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-07-31 12:54:36.490719 catalystai-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.470306 catalystai-1.0.2/catalystai/
+-rw-rw-rw-   0        0        0       31 2023-07-31 12:53:37.000000 catalystai-1.0.2/catalystai/__init__.py
+-rw-rw-rw-   0        0        0     3316 2023-07-31 12:53:42.000000 catalystai-1.0.2/catalystai/catalystai.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.489725 catalystai-1.0.2/catalystai.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:54:36.492725 catalystai-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-31 12:53:52.000000 catalystai-1.0.2/setup.py
```

### Comparing `catalystai-1.0.1/LICENCE.txt` & `catalystai-1.0.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.1/PKG-INFO` & `catalystai-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.1/catalystai/minio.py` & `catalystai-1.0.2/catalystai/catalystai.py`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.1/catalystai.egg-info/PKG-INFO` & `catalystai-1.0.2/catalystai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.1
+Version: 1.0.2
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.1/setup.py` & `catalystai-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 "Intended Audience :: Education",
 "Operating System :: MacOS :: MacOS X",
 "Operating System :: Microsoft :: Windows",
 "Programming Language :: Python :: 3",
 ]
 setup(
 name="catalystai",
-version="1.0.1",
+version="1.0.2",
 description="Catalyst AI package",
 long_description="Catalyst AI package to upload data to MinIO bucket",
 url="",
 author="Catalyst AI",
 author_email="catalystlabs.ai@gmail.com",
 license="Catalyst AI",
 classifiers=classifiers,
```

