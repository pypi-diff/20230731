# Comparing `tmp/abstract_gui-0.0.53.6.tar.gz` & `tmp/abstract_gui-0.0.53.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.6.tar", last modified: Mon Jul 31 06:10:20 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.7.tar", last modified: Mon Jul 31 06:12:35 2023, max compression
```

## Comparing `abstract_gui-0.0.53.6.tar` & `abstract_gui-0.0.53.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:10:20.782342 abstract_gui-0.0.53.6/
--rw-r--r--   0 root         (0) root         (0)     9210 2023-07-31 06:10:20.782342 abstract_gui-0.0.53.6/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.6/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.6/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 06:10:20.782342 abstract_gui-0.0.53.6/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-31 06:10:08.000000 abstract_gui-0.0.53.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:10:20.778342 abstract_gui-0.0.53.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:10:20.778342 abstract_gui-0.0.53.6/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:35:15.000000 abstract_gui-0.0.53.6/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19824 2023-07-31 05:28:15.000000 abstract_gui-0.0.53.6/src/abstract_gui/abstract_gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:10:20.782342 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9210 2023-07-31 06:10:20.000000 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-31 06:10:20.000000 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:10:20.000000 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 06:10:20.000000 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 06:10:20.000000 abstract_gui-0.0.53.6/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/
+-rw-r--r--   0 root         (0) root         (0)     9210 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.7/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.7/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-31 06:12:25.000000 abstract_gui-0.0.53.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-31 05:35:15.000000 abstract_gui-0.0.53.7/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19824 2023-07-31 05:28:15.000000 abstract_gui-0.0.53.7/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.7/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:12:35.797166 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9210 2023-07-31 06:12:35.000000 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 06:12:35.000000 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:12:35.000000 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 06:12:35.000000 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 06:12:35.000000 abstract_gui-0.0.53.7/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.6/PKG-INFO` & `abstract_gui-0.0.53.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.6
+Version: 0.0.53.7
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.6/README.md` & `abstract_gui-0.0.53.7/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.6/setup.py` & `abstract_gui-0.0.53.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.6',
+    version='0.0.53.7',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.6/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.7/src/abstract_gui/abstract_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.6/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.7/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.6
+Version: 0.0.53.7
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```
