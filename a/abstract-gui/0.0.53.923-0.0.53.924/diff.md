# Comparing `tmp/abstract_gui-0.0.53.923.tar.gz` & `tmp/abstract_gui-0.0.53.924.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.923.tar", last modified: Mon Jul 31 06:32:53 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.924.tar", last modified: Mon Jul 31 06:36:50 2023, max compression
```

## Comparing `abstract_gui-0.0.53.923.tar` & `abstract_gui-0.0.53.924.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/
--rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.923/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.923/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-31 06:32:49.000000 abstract_gui-0.0.53.923/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.923/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20090 2023-07-31 06:32:16.000000 abstract_gui-0.0.53.923/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.923/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:32:53.383464 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:32:53.000000 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 06:32:53.000000 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:32:53.000000 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 06:32:53.000000 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 06:32:53.000000 abstract_gui-0.0.53.923/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.924/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.924/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-31 06:36:45.000000 abstract_gui-0.0.53.924/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.924/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    20153 2023-07-31 06:36:41.000000 abstract_gui-0.0.53.924/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.924/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.923/PKG-INFO` & `abstract_gui-0.0.53.924/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.923
+Version: 0.0.53.924
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.923/README.md` & `abstract_gui-0.0.53.924/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.923/setup.py` & `abstract_gui-0.0.53.924/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.923',
+    version='0.0.53.924',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.923/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.924/src/abstract_gui/abstract_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,41 +14,43 @@
 
                 retrieve_global_variables(self, script_name, global_variables):
                     Stores the global variables of a script in the global_vars dictionary.
 
                 return_global_variables(self, script_name):
                     Returns the global variables of a script.
         """
-        def __init__(self):
+        
+        def __init__(self,script_name):
                 """
                 Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
                 """
+                self.script_name = script_name
                 self.global_vars = {}
 
-        def retrieve_global_variables(self, script_name, global_variables):
+        def retrieve_global_variables(self, global_variables):
                 """
                 Stores the global variables of a script in the global_vars dictionary.
 
                 Args:
                     script_name (str): The name of the script.
                     global_variables (dict): The global variables to store for the script.
                 """
-                self.global_vars[script_name] = global_variables
+                self.global_vars[self.script_name] = global_variables
         
-        def return_global_variables(self, script_name):
+        def return_global_variables(self):
                 """
                 Returns the global variables of a script.
 
                 Args:
                     script_name (str): The name of the script.
 
                 Returns:
                     dict: The global variables of the script. If no global variables are found, it returns an empty dictionary.
                 """
-                return self.global_vars.get(script_name, {})
+                return self.global_vars.get(self.script_name, {})
 class WindowManager:
     """
     A class to manage PySimpleGUI windows and their events.
 
     Attributes:
         all_windows (dict): A dictionary to store registered windows along with their details.
         last_window (str): The name of the last accessed window.
@@ -496,11 +498,11 @@
     window = get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
                                                                          [get_gui_fun('Input'), get_gui_fun(f'{type}Browse',{**args,"initial_folder":initial_folder})],
                                                                          [get_gui_fun('OK'), get_gui_fun('Cancel')]]
                                    }
                          )
     return WindowManager.while_basic(window)['Browse']
 def create_window_manager(script_name="main_script",global_var=globals()):
-    bridge = WindowGlobalBridge()
+    bridge = WindowGlobalBridge(script_name)
     global_var[script_name] = script_name
     bridge.retrieve_global_variables(script_name, global_var)
     return WindowManager(script_name, bridge),bridge
```

### Comparing `abstract_gui-0.0.53.923/src/abstract_gui/main.py` & `abstract_gui-0.0.53.924/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.923/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.924/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.923
+Version: 0.0.53.924
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

