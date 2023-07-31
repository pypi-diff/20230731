# Comparing `tmp/hplc-py-0.1.0.post1.tar.gz` & `tmp/hplc-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hplc-py-0.1.0.post1.tar", last modified: Mon Jul 31 00:13:21 2023, max compression
+gzip compressed data, was "hplc-py-0.1.1.tar", last modified: Mon Jul 31 00:13:15 2023, max compression
```

## Comparing `hplc-py-0.1.0.post1.tar` & `hplc-py-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:21.258575 hplc-py-0.1.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    34666 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-31 00:13:21.258575 hplc-py-0.1.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:21.254574 hplc-py-0.1.0.post1/hplc/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/hplc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/hplc/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    54407 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/hplc/quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:21.254574 hplc-py-0.1.0.post1/hplc_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-31 00:13:21.000000 hplc-py-0.1.0.post1/hplc_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 00:13:21.000000 hplc-py-0.1.0.post1/hplc_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:13:21.000000 hplc-py-0.1.0.post1/hplc_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 00:13:21.000000 hplc-py-0.1.0.post1/hplc_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:13:21.258575 hplc-py-0.1.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:21.258575 hplc-py-0.1.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-31 00:13:10.000000 hplc-py-0.1.0.post1/tests/test_chromatogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:15.509523 hplc-py-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34666 2023-07-31 00:13:03.000000 hplc-py-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 00:13:15.509523 hplc-py-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-07-31 00:13:03.000000 hplc-py-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:15.509523 hplc-py-0.1.1/hplc/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 00:13:03.000000 hplc-py-0.1.1/hplc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-31 00:13:03.000000 hplc-py-0.1.1/hplc/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54407 2023-07-31 00:13:03.000000 hplc-py-0.1.1/hplc/quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:15.509523 hplc-py-0.1.1/hplc_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 00:13:15.000000 hplc-py-0.1.1/hplc_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-31 00:13:15.000000 hplc-py-0.1.1/hplc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:13:15.000000 hplc-py-0.1.1/hplc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 00:13:15.000000 hplc-py-0.1.1/hplc_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:13:15.509523 hplc-py-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-31 00:13:03.000000 hplc-py-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:13:15.509523 hplc-py-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-07-31 00:13:03.000000 hplc-py-0.1.1/tests/test_chromatogram.py
```

### Comparing `hplc-py-0.1.0.post1/LICENSE` & `hplc-py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hplc-py-0.1.0.post1/PKG-INFO` & `hplc-py-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hplc-py
-Version: 0.1.0.post1
+Version: 0.1.1
 Summary: Python utilities for the processing and quantification of chromatograms from High Performance Liquid Chromatography (HPLC).
 Home-page: https://github.com/cremerlab/hplc-py
 Author: Griffin Chure
 Author-email: griffinchure@gmail.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hplc-py-0.1.0.post1/README.md` & `hplc-py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hplc-py-0.1.0.post1/hplc/io.py` & `hplc-py-0.1.1/hplc/io.py`

 * *Files identical despite different names*

### Comparing `hplc-py-0.1.0.post1/hplc/quant.py` & `hplc-py-0.1.1/hplc/quant.py`

 * *Files identical despite different names*

### Comparing `hplc-py-0.1.0.post1/hplc_py.egg-info/PKG-INFO` & `hplc-py-0.1.1/hplc_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hplc-py
-Version: 0.1.0.post1
+Version: 0.1.1
 Summary: Python utilities for the processing and quantification of chromatograms from High Performance Liquid Chromatography (HPLC).
 Home-page: https://github.com/cremerlab/hplc-py
 Author: Griffin Chure
 Author-email: griffinchure@gmail.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `hplc-py-0.1.0.post1/setup.py` & `hplc-py-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "0.1.0.post1"
+__version__ = "0.1.01"
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
@@ -20,10 +20,11 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
     ],
     author="Griffin Chure",
     author_email="griffinchure@gmail.com",
-    packages=find_packages(exclude=('docs', 'docs', 'hplc.egg-info')),
+    packages=find_packages(
+        exclude=('docs', 'doc', 'sandbox', 'dev', 'hplc.egg-info')),
     include_package_data=True
 )
```

### Comparing `hplc-py-0.1.0.post1/tests/test_chromatogram.py` & `hplc-py-0.1.1/tests/test_chromatogram.py`

 * *Files identical despite different names*

