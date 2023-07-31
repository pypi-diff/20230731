# Comparing `tmp/abstract_gui-0.0.53.94.tar.gz` & `tmp/abstract_gui-0.0.53.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.94.tar", last modified: Mon Jul 31 07:10:26 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.95.tar", last modified: Mon Jul 31 07:12:45 2023, max compression
```

## Comparing `abstract_gui-0.0.53.94.tar` & `abstract_gui-0.0.53.95.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:10:26.717594 abstract_gui-0.0.53.94/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:10:26.717594 abstract_gui-0.0.53.94/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.94/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.94/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:10:26.721594 abstract_gui-0.0.53.94/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:10:15.000000 abstract_gui-0.0.53.94/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:10:26.717594 abstract_gui-0.0.53.94/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:10:26.717594 abstract_gui-0.0.53.94/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.94/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21469 2023-07-31 07:10:10.000000 abstract_gui-0.0.53.94/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.94/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:10:26.717594 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:10:26.000000 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:10:26.000000 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:10:26.000000 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:10:26.000000 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:10:26.000000 abstract_gui-0.0.53.94/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.95/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.95/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:12:41.000000 abstract_gui-0.0.53.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.95/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21529 2023-07-31 07:12:32.000000 abstract_gui-0.0.53.95/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.95/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.94/PKG-INFO` & `abstract_gui-0.0.53.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.94
+Version: 0.0.53.95
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.94/README.md` & `abstract_gui-0.0.53.95/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.94/setup.py` & `abstract_gui-0.0.53.95/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.94',
+    version='0.0.53.95',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.94/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.95/src/abstract_gui/abstract_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,20 +277,22 @@
         self.all_windows[name]["event"] = event
         self.all_windows[name]["values"] = values
         self.update_last_window(window)
     def get_last_window_info(self):
         last_window = self.all_windows['last_window']
         if last_window != None:
             return self.all_windows[last_window]
-    def get_last_windo_method(self):
+    def get_last_window_method(self):
         window_info = self.get_last_window_info()
         if window_info != None:
             if "method" in window_info:
                 return window_info["method"]
-    def update_values(window=self.get_last_windo_method(),key:str=None,value:any=None,values:any=None,args:dict=None):
+    def update_values(self,window=None,key:str=None,value:any=None,values:any=None,args:dict=None):
+        if window == None:
+            window = self.get_last_window_method()
         if window != None and key != None:
             if self.verify_window(window):
                 if args == None:
                     args = {}
                 if values != None:
                     args["values"]=values
                 if value != None:
```

### Comparing `abstract_gui-0.0.53.94/src/abstract_gui/main.py` & `abstract_gui-0.0.53.95/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.94/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.95/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.94
+Version: 0.0.53.95
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

