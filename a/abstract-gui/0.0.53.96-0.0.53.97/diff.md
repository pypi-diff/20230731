# Comparing `tmp/abstract_gui-0.0.53.96.tar.gz` & `tmp/abstract_gui-0.0.53.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.96.tar", last modified: Mon Jul 31 07:52:02 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.97.tar", last modified: Mon Jul 31 08:04:33 2023, max compression
```

## Comparing `abstract_gui-0.0.53.96.tar` & `abstract_gui-0.0.53.97.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.96/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.96/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:51:44.000000 abstract_gui-0.0.53.96/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.561093 abstract_gui-0.0.53.96/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.96/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22283 2023-07-31 07:51:30.000000 abstract_gui-0.0.53.96/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.96/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.97/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.97/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 08:04:28.000000 abstract_gui-0.0.53.97/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.97/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22303 2023-07-31 08:03:34.000000 abstract_gui-0.0.53.97/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.97/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.96/PKG-INFO` & `abstract_gui-0.0.53.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.96
+Version: 0.0.53.97
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.96/README.md` & `abstract_gui-0.0.53.97/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.96/setup.py` & `abstract_gui-0.0.53.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.96',
+    version='0.0.53.97',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.96/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.97/src/abstract_gui/abstract_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
         name (str): The name of the PySimpleGUI function.
         args (dict): The arguments to pass to the PySimpleGUI function.
 
     Returns:
         callable: A callable object that invokes the PySimpleGUI function with the specified arguments when called.
     """
     return get_fun({"instance": sg, "name": name, "args": args})
-def expandable(size: tuple = (None, None),scrollable:bool=True,auto_size_text:bool=True,expand_x:bool=True,expand_y:bool=True):
+def expandable(size: tuple = (None, None),resizable:bool=True,scrollable:bool=True,auto_size_text:bool=True,expand_x:bool=True,expand_y:bool=True):
     """Returns a dictionary with window parameters for creating an expandable PySimpleGUI window."""
     return {"size": size, "resizable": resizable, "scrollable": scrollable, "auto_size_text": auto_size_text, "expand_x": expand_x, "expand_y": expand_y}
 def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path()):
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
```

### Comparing `abstract_gui-0.0.53.96/src/abstract_gui/main.py` & `abstract_gui-0.0.53.97/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.96/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.97/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.96
+Version: 0.0.53.97
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

