# Comparing `tmp/abstract_gui-0.0.52.24.tar.gz` & `tmp/abstract_gui-0.0.52.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.52.24.tar", last modified: Mon Jul 31 04:58:20 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.52.25.tar", last modified: Mon Jul 31 05:02:42 2023, max compression
```

## Comparing `abstract_gui-0.0.52.24.tar` & `abstract_gui-0.0.52.25.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:58:20.172509 abstract_gui-0.0.52.24/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.52.24/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.52.24/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 04:58:20.172509 abstract_gui-0.0.52.24/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 04:58:09.000000 abstract_gui-0.0.52.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:02:42.736976 abstract_gui-0.0.52.25/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 05:02:42.736976 abstract_gui-0.0.52.25/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.52.25/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.52.25/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 05:02:42.736976 abstract_gui-0.0.52.25/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 05:02:34.000000 abstract_gui-0.0.52.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:02:42.732976 abstract_gui-0.0.52.25/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 05:02:42.736976 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 05:02:42.000000 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-31 05:02:42.000000 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:02:42.000000 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 05:02:42.000000 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 05:02:42.000000 abstract_gui-0.0.52.25/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.52.24/PKG-INFO` & `abstract_gui-0.0.52.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.52.24
+Version: 0.0.52.25
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.52.24/README.md` & `abstract_gui-0.0.52.25/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.52.24/setup.py` & `abstract_gui-0.0.52.25/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.52.24',
+    version='0.0.52.25',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.52.24/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.52.25/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.52.24
+Version: 0.0.52.25
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

