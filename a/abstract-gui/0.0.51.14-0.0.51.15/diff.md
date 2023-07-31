# Comparing `tmp/abstract_gui-0.0.51.14.tar.gz` & `tmp/abstract_gui-0.0.51.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.51.14.tar", last modified: Mon Jul 31 04:00:31 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.51.15.tar", last modified: Mon Jul 31 04:03:31 2023, max compression
```

## Comparing `abstract_gui-0.0.51.14.tar` & `abstract_gui-0.0.51.15.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:00:31.709383 abstract_gui-0.0.51.14/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:00:31.709383 abstract_gui-0.0.51.14/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.51.14/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.14/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 04:00:31.709383 abstract_gui-0.0.51.14/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 04:00:19.000000 abstract_gui-0.0.51.14/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:00:31.705383 abstract_gui-0.0.51.14/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:00:31.705383 abstract_gui-0.0.51.14/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.14/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.14/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:00:31.709383 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     9211 2023-07-31 04:00:31.000000 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      296 2023-07-31 04:00:31.000000 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-31 04:00:31.000000 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-31 04:00:31.000000 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 04:00:31.000000 abstract_gui-0.0.51.14/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.51.15/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.15/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 04:03:21.000000 abstract_gui-0.0.51.15/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 04:03:15.000000 abstract_gui-0.0.51.15/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.15/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:03:31.115576 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     9211 2023-07-31 04:03:31.000000 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      296 2023-07-31 04:03:31.000000 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-31 04:03:31.000000 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-31 04:03:31.000000 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 04:03:31.000000 abstract_gui-0.0.51.15/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.51.14/PKG-INFO` & `abstract_gui-0.0.51.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.51.14
+Version: 0.0.51.15
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.51.14/README.md` & `abstract_gui-0.0.51.15/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.51.14/setup.py` & `abstract_gui-0.0.51.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.51.14',
+    version='0.0.51.15',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.51.14/src/abstract_gui/main.py` & `abstract_gui-0.0.51.15/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.51.14/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.51.15/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.51.14
+Version: 0.0.51.15
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

