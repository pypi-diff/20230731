# Comparing `tmp/catalystai-1.0.2.tar.gz` & `tmp/catalystai-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystai-1.0.2.tar", last modified: Mon Jul 31 12:54:36 2023, max compression
+gzip compressed data, was "catalystai-1.0.3.tar", last modified: Mon Jul 31 13:50:41 2023, max compression
```

## Comparing `catalystai-1.0.2.tar` & `catalystai-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.491723 catalystai-1.0.2/
--rw-rw-rw-   0        0        0      220 2023-07-31 12:54:28.000000 catalystai-1.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      543 2023-07-31 12:54:36.490719 catalystai-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.470306 catalystai-1.0.2/catalystai/
--rw-rw-rw-   0        0        0       31 2023-07-31 12:53:37.000000 catalystai-1.0.2/catalystai/__init__.py
--rw-rw-rw-   0        0        0     3316 2023-07-31 12:53:42.000000 catalystai-1.0.2/catalystai/catalystai.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:54:36.489725 catalystai-1.0.2/catalystai.egg-info/
--rw-rw-rw-   0        0        0      543 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 12:54:36.000000 catalystai-1.0.2/catalystai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:54:36.492725 catalystai-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-31 12:53:52.000000 catalystai-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.984546 catalystai-1.0.3/
+-rw-rw-rw-   0        0        0      336 2023-07-31 13:50:31.000000 catalystai-1.0.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1058 2023-07-31 10:18:20.000000 catalystai-1.0.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 10:18:20.000000 catalystai-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      543 2023-07-31 13:50:41.983546 catalystai-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      184 2023-07-31 10:18:20.000000 catalystai-1.0.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.967496 catalystai-1.0.3/catalystai/
+-rw-rw-rw-   0        0        0       32 2023-07-31 13:49:37.000000 catalystai-1.0.3/catalystai/__init__.py
+-rw-rw-rw-   0        0        0     3316 2023-07-31 13:49:30.000000 catalystai-1.0.3/catalystai/catalystai.py
+drwxrwxrwx   0        0        0        0 2023-07-31 13:50:41.982549 catalystai-1.0.3/catalystai.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 13:50:41.000000 catalystai-1.0.3/catalystai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 13:50:41.985542 catalystai-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-31 13:50:21.000000 catalystai-1.0.3/setup.py
```

### Comparing `catalystai-1.0.2/LICENCE.txt` & `catalystai-1.0.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.2/PKG-INFO` & `catalystai-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.2/catalystai/catalystai.py` & `catalystai-1.0.3/catalystai/catalystai.py`

 * *Files identical despite different names*

### Comparing `catalystai-1.0.2/catalystai.egg-info/PKG-INFO` & `catalystai-1.0.3/catalystai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystai
-Version: 1.0.2
+Version: 1.0.3
 Summary: Catalyst AI package
 Home-page: 
 Author: Catalyst AI
 Author-email: catalystlabs.ai@gmail.com
 License: Catalyst AI
 Keywords: python,first package
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `catalystai-1.0.2/setup.py` & `catalystai-1.0.3/setup.py`

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
-version="1.0.2",
+version="1.0.3",
 description="Catalyst AI package",
 long_description="Catalyst AI package to upload data to MinIO bucket",
 url="",
 author="Catalyst AI",
 author_email="catalystlabs.ai@gmail.com",
 license="Catalyst AI",
 classifiers=classifiers,
```

