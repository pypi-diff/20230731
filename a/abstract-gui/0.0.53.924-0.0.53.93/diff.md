# Comparing `tmp/abstract_gui-0.0.53.924.tar.gz` & `tmp/abstract_gui-0.0.53.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.924.tar", last modified: Mon Jul 31 06:36:50 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.93.tar", last modified: Mon Jul 31 07:06:52 2023, max compression
```

## Comparing `abstract_gui-0.0.53.924.tar` & `abstract_gui-0.0.53.93.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/
--rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.924/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.924/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1126 2023-07-31 06:36:45.000000 abstract_gui-0.0.53.924/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.924/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    20153 2023-07-31 06:36:41.000000 abstract_gui-0.0.53.924/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.924/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 06:36:50.377067 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9212 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 06:36:50.000000 abstract_gui-0.0.53.924/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.93/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.93/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:06:34.000000 abstract_gui-0.0.53.93/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.93/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    21438 2023-07-31 07:06:27.000000 abstract_gui-0.0.53.93/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.93/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:06:52.031646 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:06:51.000000 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:06:52.000000 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:06:51.000000 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:06:51.000000 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:06:51.000000 abstract_gui-0.0.53.93/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.924/PKG-INFO` & `abstract_gui-0.0.53.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.924
+Version: 0.0.53.93
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.924/README.md` & `abstract_gui-0.0.53.93/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.924/setup.py` & `abstract_gui-0.0.53.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.924',
+    version='0.0.53.93',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.924/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.93/src/abstract_gui/abstract_gui.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,43 +14,47 @@
 
                 retrieve_global_variables(self, script_name, global_variables):
                     Stores the global variables of a script in the global_vars dictionary.
 
                 return_global_variables(self, script_name):
                     Returns the global variables of a script.
         """
-        
-        def __init__(self,script_name):
+        def __init__(self):
                 """
                 Initializes the WindowGlobalBridge with an empty dictionary for global_vars.
                 """
-                self.script_name = script_name
                 self.global_vars = {}
-
-        def retrieve_global_variables(self, global_variables):
+        def create_script_name(self,script_name:str='default_script_name'):
+                if script_name in self.global_vars:
+                    script_name = script_name+'_0'
+                while script_name in self.global_vars:
+                    script_number = int(script_name.split('_')[-1])
+                    scrript_name = script_name[:-len(str(script_number))]+str(script_number+1)
+                return script_name
+        def retrieve_global_variables(self, script_name, global_variables):
                 """
                 Stores the global variables of a script in the global_vars dictionary.
 
                 Args:
                     script_name (str): The name of the script.
                     global_variables (dict): The global variables to store for the script.
                 """
-                self.global_vars[self.script_name] = global_variables
+                self.global_vars[script_name] = global_variables
         
-        def return_global_variables(self):
+        def return_global_variables(self, script_name):
                 """
                 Returns the global variables of a script.
 
                 Args:
                     script_name (str): The name of the script.
 
                 Returns:
                     dict: The global variables of the script. If no global variables are found, it returns an empty dictionary.
                 """
-                return self.global_vars.get(self.script_name, {})
+                return self.global_vars.get(script_name, {})
 class WindowManager:
     """
     A class to manage PySimpleGUI windows and their events.
 
     Attributes:
         all_windows (dict): A dictionary to store registered windows along with their details.
         last_window (str): The name of the last accessed window.
@@ -230,15 +234,15 @@
         """
         name = window
         if self.is_window_object(window):
             name = self.search_global_windows(window)
             if name is False:
                 name = self.register_window(window)
         if name in self.get_window_names():
-            self.all_windows['last_window'] = name
+             = name
     def send_to_bridge(self):
         self.global_vars["all_windows"] = self.all_windows
         self.global_bridge.retrieve_global_variables(self.script_name, self.global_vars)
     def close_window(self, window=None):
         """
         Closes the given PySimpleGUI window.
 
@@ -269,15 +273,34 @@
         if event == self.close_window_element() and self.all_windows[name]["closed"] == False:
             self.all_windows[name]["closed"] = True
             self.all_windows[name]["event"] = 'EXIT'
             return 
         self.all_windows[name]["event"] = event
         self.all_windows[name]["values"] = values
         self.update_last_window(window)
-
+    def get_last_window_info(self):
+        last_window = self.all_windows['last_window']
+        if last_window != None:
+            return self.all_windows[last_window]
+    def get_last_windo_method(self):
+        window_info = self.get_last_window_info()
+        if window_info != None:
+            if "method" in window_info:
+                return window_info["method"]
+    def update_values(window=self.get_last_windo_method(),key:str=None,value:any=None,values:any=None,args:dict=None):
+        if window != None and key != None:
+            if self.verify_window(window):
+                if args == None:
+                    args = {}
+                if values != None:
+                    args["values"]=values
+                if value != None:
+                    args["value"]=value
+                if args != {}:
+                    window[key].update(**args)
     def get_event(self, window=None):
         """
         Get the last event from a window.
 
         Args:
             win (any, optional): The window to get the event from. If not provided, the last accessed window is used.
 
@@ -497,12 +520,13 @@
         title = f'Please choose a {type.lower()}'
     window = get_gui_fun('Window',{"title":f'{type} Explorer', "layout":[[get_gui_fun('Text',{"text":title})],
                                                                          [get_gui_fun('Input'), get_gui_fun(f'{type}Browse',{**args,"initial_folder":initial_folder})],
                                                                          [get_gui_fun('OK'), get_gui_fun('Cancel')]]
                                    }
                          )
     return WindowManager.while_basic(window)['Browse']
-def create_window_manager(script_name="main_script",global_var=globals()):
-    bridge = WindowGlobalBridge(script_name)
+def create_window_manager(script_name='default_script_name',global_var=globals()):
+    bridge = WindowGlobalBridge()
+    script_name = bridge.create_script_name(script_name)
     global_var[script_name] = script_name
     bridge.retrieve_global_variables(script_name, global_var)
-    return WindowManager(script_name, bridge),bridge
+    return WindowManager(script_name, bridge),bridge,script_name
```

### Comparing `abstract_gui-0.0.53.924/src/abstract_gui/main.py` & `abstract_gui-0.0.53.93/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.924/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.93/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.924
+Version: 0.0.53.93
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

