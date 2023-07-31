# Comparing `tmp/abstract_gui-0.0.51.12.tar.gz` & `tmp/abstract_gui-0.0.51.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.51.12.tar", last modified: Mon Jul 31 00:15:34 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.51.13.tar", last modified: Mon Jul 31 00:18:41 2023, max compression
```

## Comparing `abstract_gui-0.0.51.12.tar` & `abstract_gui-0.0.51.13.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.51.12/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.12/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 00:15:13.000000 abstract_gui-0.0.51.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/src/abstract_gui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/src/abstract_gui/PyQt5/
--rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.12/src/abstract_gui/PyQt5/PyQt5_browser_window.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.12/src/abstract_gui/PyQt5/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.12/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.12/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/src/abstract_gui/simple_gui/
--rw-rw-r--   0 root         (0) root         (0)      192 2023-07-31 00:14:51.000000 abstract_gui-0.0.51.12/src/abstract_gui/simple_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19685 2023-07-31 00:14:46.000000 abstract_gui-0.0.51.12/src/abstract_gui/simple_gui/dynamic_gui.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:15:34.523391 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     9211 2023-07-31 00:15:34.000000 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      461 2023-07-31 00:15:34.000000 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-07-31 00:15:34.000000 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       31 2023-07-31 00:15:34.000000 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 00:15:34.000000 abstract_gui-0.0.51.12/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.51.13/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.13/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 00:18:26.000000 abstract_gui-0.0.51.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.061848 abstract_gui-0.0.51.13/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/src/abstract_gui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/src/abstract_gui/PyQt5/
+-rw-rw-r--   0 root         (0) root         (0)     2500 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.13/src/abstract_gui/PyQt5/PyQt5_browser_window.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.13/src/abstract_gui/PyQt5/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.13/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1294 2023-07-29 19:09:21.000000 abstract_gui-0.0.51.13/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/src/abstract_gui/simple_gui/
+-rw-rw-r--   0 root         (0) root         (0)      192 2023-07-31 00:14:51.000000 abstract_gui-0.0.51.13/src/abstract_gui/simple_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19854 2023-07-31 00:18:10.000000 abstract_gui-0.0.51.13/src/abstract_gui/simple_gui/dynamic_gui.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 00:18:41.065848 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     9211 2023-07-31 00:18:41.000000 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      461 2023-07-31 00:18:41.000000 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-07-31 00:18:41.000000 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       31 2023-07-31 00:18:41.000000 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-07-31 00:18:41.000000 abstract_gui-0.0.51.13/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.51.12/PKG-INFO` & `abstract_gui-0.0.51.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.51.12
+Version: 0.0.51.13
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.51.12/README.md` & `abstract_gui-0.0.51.13/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.51.12/setup.py` & `abstract_gui-0.0.51.13/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.51.12',
+    version='0.0.51.13',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.51.12/src/abstract_gui/PyQt5/PyQt5_browser_window.py` & `abstract_gui-0.0.51.13/src/abstract_gui/PyQt5/PyQt5_browser_window.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.51.12/src/abstract_gui/main.py` & `abstract_gui-0.0.51.13/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.51.12/src/abstract_gui/simple_gui/dynamic_gui.py` & `abstract_gui-0.0.51.13/src/abstract_gui/simple_gui/dynamic_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from __init__ import *
+import PySimpleGUI as sg
+from abstract_utilities.class_utils import get_fun
+from abstract_utilities.thread_utils import thread_alive
+from abstract_utilities.path_utils import get_current_path
 
 class WindowGlobalBridge:
         """
         A class to manage the global variables shared between different scripts.
 
         Attributes:
                 global_vars (dict): A dictionary to store global variables for each script.
```

### Comparing `abstract_gui-0.0.51.12/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.51.13/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.51.12
+Version: 0.0.51.13
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

