# Comparing `tmp/githup-0.0.2.tar.gz` & `tmp/githup-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "githup-0.0.2.tar", last modified: Mon Jul 31 12:10:10 2023, max compression
+gzip compressed data, was "githup-0.0.3.tar", last modified: Mon Jul 31 12:25:49 2023, max compression
```

## Comparing `githup-0.0.2.tar` & `githup-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:10:10.459894 githup-0.0.2/
--rw-rw-rw-   0        0        0      682 2023-07-31 12:10:10.458881 githup-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 12:10:10.438934 githup-0.0.2/githup/
--rw-rw-rw-   0        0        0       23 2023-07-18 22:58:28.000000 githup-0.0.2/githup/__init__.py
--rw-rw-rw-   0        0        0     3086 2023-07-18 21:52:28.000000 githup-0.0.2/githup/githup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:10:10.457882 githup-0.0.2/githup.egg-info/
--rw-rw-rw-   0        0        0      682 2023-07-31 12:10:10.000000 githup-0.0.2/githup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-07-31 12:10:10.000000 githup-0.0.2/githup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:10:10.000000 githup-0.0.2/githup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 12:10:10.000000 githup-0.0.2/githup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 12:10:10.000000 githup-0.0.2/githup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:10:10.460876 githup-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      950 2023-07-31 12:09:40.000000 githup-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:25:49.743194 githup-0.0.3/
+-rw-rw-rw-   0        0        0      682 2023-07-31 12:25:49.742200 githup-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 12:25:49.712278 githup-0.0.3/githup/
+-rw-rw-rw-   0        0        0       23 2023-07-18 22:58:28.000000 githup-0.0.3/githup/__init__.py
+-rw-rw-rw-   0        0        0     3086 2023-07-18 21:52:28.000000 githup-0.0.3/githup/githup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:25:49.740230 githup-0.0.3/githup.egg-info/
+-rw-rw-rw-   0        0        0      682 2023-07-31 12:25:49.000000 githup-0.0.3/githup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      164 2023-07-31 12:25:49.000000 githup-0.0.3/githup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:25:49.000000 githup-0.0.3/githup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 12:25:49.000000 githup-0.0.3/githup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:25:49.743194 githup-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-31 12:24:00.000000 githup-0.0.3/setup.py
```

### Comparing `githup-0.0.2/PKG-INFO` & `githup-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githup
-Version: 0.0.2
+Version: 0.0.3
 Summary: Upload files on GitHub using Python
 Home-page: UNKNOWN
 Author: Cyril Frébel
 Author-email: cyril.frebel@proton.me
 License: UNKNOWN
 Keywords: python,upload,github,files
 Platform: UNKNOWN
```

### Comparing `githup-0.0.2/githup/githup.py` & `githup-0.0.3/githup/githup.py`

 * *Files identical despite different names*

### Comparing `githup-0.0.2/githup.egg-info/PKG-INFO` & `githup-0.0.3/githup.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: githup
-Version: 0.0.2
+Version: 0.0.3
 Summary: Upload files on GitHub using Python
 Home-page: UNKNOWN
 Author: Cyril Frébel
 Author-email: cyril.frebel@proton.me
 License: UNKNOWN
 Keywords: python,upload,github,files
 Platform: UNKNOWN
```

### Comparing `githup-0.0.2/setup.py` & `githup-0.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Upload files on GitHub using Python'
 LONG_DESCRIPTION = 'download/initiate/commit new repositories and create files to upload them on GitHub using Python'
 
 # Setting up
 setup(
     name="githup",
     version=VERSION,
     author="Cyril Frébel",
     author_email="cyril.frebel@proton.me",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['shutil'],
     keywords=['python', 'upload', 'github', 'files'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

