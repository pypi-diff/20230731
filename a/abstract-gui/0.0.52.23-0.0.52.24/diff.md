# Comparing `tmp/abstract_gui-0.0.52.23.tar.gz` & `tmp/abstract_gui-0.0.52.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.52.23.tar", last modified: Mon Jul 31 04:57:09 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.52.24.tar", last modified: Mon Jul 31 04:58:20 2023, max compression
```

## Comparing `abstract_gui-0.0.52.23.tar` & `abstract_gui-0.0.52.24.tar`

### file list

```diff
@@ -1,17 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.52.23/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.52.23/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 04:56:46.000000 abstract_gui-0.0.52.23/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       27 2023-07-31 04:44:21.000000 abstract_gui-0.0.52.23/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19814 2023-07-31 04:56:20.000000 abstract_gui-0.0.52.23/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1288 2023-07-31 04:48:59.000000 abstract_gui-0.0.52.23/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:57:09.748572 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:57:09.000000 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 04:57:09.000000 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:57:09.000000 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 04:57:09.000000 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 04:57:09.000000 abstract_gui-0.0.52.23/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:58:20.172509 abstract_gui-0.0.52.24/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.52.24/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.52.24/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 04:58:20.172509 abstract_gui-0.0.52.24/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 04:58:09.000000 abstract_gui-0.0.52.24/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 04:58:20.168509 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 04:58:20.000000 abstract_gui-0.0.52.24/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.52.23/PKG-INFO` & `abstract_gui-0.0.52.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.52.23
+Version: 0.0.52.24
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.52.23/README.md` & `abstract_gui-0.0.52.24/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.52.23/setup.py` & `abstract_gui-0.0.52.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.52.23',
+    version='0.0.52.24',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.52.23/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.52.24/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.52.23
+Version: 0.0.52.24
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

