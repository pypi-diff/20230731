# Comparing `tmp/robotchain_sdk-1.0.1.tar.gz` & `tmp/robotchain_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotchain_sdk-1.0.1.tar", last modified: Mon Jul 31 16:10:28 2023, max compression
+gzip compressed data, was "robotchain_sdk-1.0.3.tar", last modified: Mon Jul 31 16:26:06 2023, max compression
```

## Comparing `robotchain_sdk-1.0.1.tar` & `robotchain_sdk-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.863266 robotchain_sdk-1.0.1/
--rw-rw-rw-   0        0        0       45 2023-07-31 16:09:08.000000 robotchain_sdk-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1948 2023-07-31 16:10:28.862267 robotchain_sdk-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.840267 robotchain_sdk-1.0.1/robotchain_sdk/
--rw-rw-rw-   0        0        0      731 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.853260 robotchain_sdk-1.0.1/robotchain_sdk/ros/
--rw-rw-rw-   0        0        0     1080 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/ros/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.860260 robotchain_sdk-1.0.1/robotchain_sdk/utils/
--rw-rw-rw-   0        0        0      233 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.861260 robotchain_sdk-1.0.1/robotchain_sdk/utils/loging/
--rw-rw-rw-   0        0        0     2849 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/utils/loging/loging.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.844266 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/
--rw-rw-rw-   0        0        0     1948 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 16:10:28.863266 robotchain_sdk-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-31 16:09:16.000000 robotchain_sdk-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.539752 robotchain_sdk-1.0.3/
+-rw-rw-rw-   0        0        0       45 2023-07-31 16:09:08.000000 robotchain_sdk-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1948 2023-07-31 16:26:06.538755 robotchain_sdk-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.530753 robotchain_sdk-1.0.3/robotchain_sdk/
+-rw-rw-rw-   0        0        0      731 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.3/robotchain_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.535755 robotchain_sdk-1.0.3/robotchain_sdk/ros/
+-rw-rw-rw-   0        0        0     1080 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.3/robotchain_sdk/ros/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.536753 robotchain_sdk-1.0.3/robotchain_sdk/utils/
+-rw-rw-rw-   0        0        0      233 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.3/robotchain_sdk/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.537752 robotchain_sdk-1.0.3/robotchain_sdk/utils/loging/
+-rw-rw-rw-   0        0        0     2849 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.3/robotchain_sdk/utils/loging/loging.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:26:06.534753 robotchain_sdk-1.0.3/robotchain_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1948 2023-07-31 16:26:06.000000 robotchain_sdk-1.0.3/robotchain_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-31 16:26:06.000000 robotchain_sdk-1.0.3/robotchain_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:26:06.000000 robotchain_sdk-1.0.3/robotchain_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-31 16:26:06.000000 robotchain_sdk-1.0.3/robotchain_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:26:06.539752 robotchain_sdk-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-07-31 16:26:01.000000 robotchain_sdk-1.0.3/setup.py
```

### Comparing `robotchain_sdk-1.0.1/PKG-INFO` & `robotchain_sdk-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain_sdk
-Version: 1.0.1
+Version: 1.0.3
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotchain_sdk-1.0.1/robotchain_sdk/__init__.py` & `robotchain_sdk-1.0.3/robotchain_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.1/robotchain_sdk/ros/__init__.py` & `robotchain_sdk-1.0.3/robotchain_sdk/ros/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.1/robotchain_sdk/utils/loging/loging.py` & `robotchain_sdk-1.0.3/robotchain_sdk/utils/loging/loging.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.1/robotchain_sdk.egg-info/PKG-INFO` & `robotchain_sdk-1.0.3/robotchain_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain-sdk
-Version: 1.0.1
+Version: 1.0.3
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `robotchain_sdk-1.0.1/setup.py` & `robotchain_sdk-1.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="robotchain_sdk",
-    version="1.0.1",
+    version="1.0.3",
     author="MakerYang",
     author_email="admin@wileho.com",
     description="Python development framework for robotchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geekros/python_framework_sdk",
     packages=find_packages(),
```

