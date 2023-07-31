# Comparing `tmp/abstract_gui-0.0.53.95.tar.gz` & `tmp/abstract_gui-0.0.53.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.95.tar", last modified: Mon Jul 31 07:12:45 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.53.96.tar", last modified: Mon Jul 31 07:52:02 2023, max compression
```

## Comparing `abstract_gui-0.0.53.95.tar` & `abstract_gui-0.0.53.96.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.95/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.95/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:12:41.000000 abstract_gui-0.0.53.95/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.95/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    21529 2023-07-31 07:12:32.000000 abstract_gui-0.0.53.95/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.95/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:12:45.784266 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:12:45.000000 abstract_gui-0.0.53.95/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.96/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.96/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 07:51:44.000000 abstract_gui-0.0.53.96/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.561093 abstract_gui-0.0.53.96/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.96/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22283 2023-07-31 07:51:30.000000 abstract_gui-0.0.53.96/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.96/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 07:52:02.565093 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 07:52:02.000000 abstract_gui-0.0.53.96/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.95/PKG-INFO` & `abstract_gui-0.0.53.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.95
+Version: 0.0.53.96
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_gui-0.0.53.95/README.md` & `abstract_gui-0.0.53.96/README.md`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.95/setup.py` & `abstract_gui-0.0.53.96/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.95',
+    version='0.0.53.96',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.95/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.53.96/src/abstract_gui/abstract_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,37 +166,38 @@
         """
         if window in self.get_window_names():
             name = window
         if self.is_window_object(window):
             name = self.search_global_windows(window)
             if name is False:
                 name = self.create_window_name()
-            self.all_windows[name] = {"method": window,"title":None,"closed":False, "values": {}, "event": "", "event_function": None}
+            self.all_windows[name] = {"method": window,"title":None,"closed":False, "values": {}, "event": "", "event_function": None,"exit_events":None}
             self.all_windows[name]["closed"]=False
         if window == None:
             name = self.create_window_name()
-            self.all_windows[name] = {"method": None,"title":None,"closed":False, "values": {}, "event": "", "event_function": None}
+            self.all_windows[name] = {"method": None,"title":None,"closed":False, "values": {}, "event": "", "event_function": None, "exit_events":None}
         return name
-    def get_new_window(self, title=None, layout=None, args=None, event_function=None):
+    def get_new_window(self, title:str=None, layout:list=None, args:dict=None, event_function:str=None,exit_events:(list or str)=None):
         """
         Create a new window.
 
         Args:
             title (str, optional): The title of the window. If not provided, 'window' is used.
             layout (list, optional): The layout of the window. If not provided, an empty layout is used.
             args (dict, optional): Additional arguments for the window.
             event_function (str, optional): The event function for the window.
 
         Returns:
             any: A new PySimpleGUI window.
         """
-        args = verify_args(args=args, layout=layout, title=title, event_function=event_function)
+        args = verify_args(args=args, layout=layout, title=title, event_function=event_function,exit_events=exit_events)
         name = self.register_window()
         self.all_windows[name]["method"] = get_window(title=title, layout=layout, args=args)
         self.all_windows[name]["event_function"] = args["event_function"]
+        self.all_windows[name]["exit_events"] = args["exit_events"]
         self.all_windows[name]["title"] = title
         return self.all_windows[name]["method"]
     def search_global_windows(self, window):
         """
         Search for a window in the global variables.
 
         Args:
@@ -337,15 +338,15 @@
 
         Args:
             window (any, optional): The window to run the event loop for. If not provided, the last accessed window is used.
         """
         self.global_vars = self.global_bridge.return_global_variables(self.script_name)
         while self.verify_window(window):
             self.read_window(window)
-            if self.win_closed(self.get_event(window)):
+            if self.win_closed(window):
                 self.close_window(window)
                 return self.all_windows[self.search_global_windows(window)]["values"]  # Return the stored data instead of all_windows
             event_function = self.all_windows[self.search_global_windows(window)]["event_function"]
 
             if event_function is not None:
                 self.global_vars[event_function](self.get_event(window))
         self.close_window(window)
@@ -361,26 +362,32 @@
         if obj in window_names:
             name = obj
         if self.is_window_object(obj):
             name = self.search_global_windows(obj)
             if name is False:
                 name = self.create_window_name()
         return name
-    def win_closed(self, event=''):
+    def win_closed(self, window):
         """
         Check if a window event calls to close the window.
 
         Args:
             event (str): The event to check.
 
         Returns:
             bool: True if the window is closed, False otherwise.
         """
-        obj_ls = ["exit", "Exit", "EXIT", self.close_window_element()]
-        return any(event == obj for obj in obj_ls)
+        event = self.get_event(window)
+        window_info = self.all_windows[self.search_global_windows(window)]
+        exit_events = []
+        if "exit_events" in window_info:
+            exit_events = list(window_info['exit_events'])
+        if self.close_window_element() not in exit_events:
+            exit_events.append(self.close_window_element())
+        return any(event == obj for obj in exit_events)
     def delete_from_list(self, _list, var):
         return [each for each in _list if each != var]
     def is_window_object(self, obj):
         """
         Check if an object is a PySimpleGUI window object.
 
         Args:
@@ -412,35 +419,37 @@
             window (any): The window to unregister.
         """
         win = self.search_global_windows(window)
         if win in self.get_window_names():
             del self.all_windows[win]
         elif self.is_window_object(win):
             del self.all_windows[window]
-def verify_args(args=None, layout=None, title=None, event_function=None):
+def verify_args(args:dict=None, layout:list=None, title:str=None, event_function:str=None,exit_events:(list or str)=None):
         args = args or {}
         layout = layout or [[]]
         title = title or 'window'
+        exit_events = exit_events or ["exit", "Exit", "EXIT"]
         args.setdefault("title", title)
         args.setdefault("layout", layout)
         args.setdefault("event_function", event_function)
+        args.setdefault("exit_events", list(exit_events))
         return args
 def get_window(title=None, layout=None, args=None):
         """
         Get a PySimpleGUI window.
 
         Args:
             win_name (str, optional): The name of the window. If not provided, a unique name is generated.
             layout (list, optional): The layout of the window. If not provided, an empty layout is used.
             args (dict, optional): Additional arguments for the window.
 
         Returns:
             any: A PySimpleGUI window.
         """
-        args = verify_args(args, layout, title)
+        args = verify_args(args=args, layout=layout, title=title)
         return get_gui_fun('Window', {**args})
 def out_of_bounds(upper: (int or float) = 100, lower: (int or float) = 0, obj: (int or float) = -1):
     """
     Checks if the given object is out of the specified upper and lower bounds.
 
     Args:
         upper (int or float): The upper bound.
@@ -496,17 +505,17 @@
         name (str): The name of the PySimpleGUI function.
         args (dict): The arguments to pass to the PySimpleGUI function.
 
     Returns:
         callable: A callable object that invokes the PySimpleGUI function with the specified arguments when called.
     """
     return get_fun({"instance": sg, "name": name, "args": args})
-def expandable(size: tuple = (None, None)):
+def expandable(size: tuple = (None, None),scrollable:bool=True,auto_size_text:bool=True,expand_x:bool=True,expand_y:bool=True):
     """Returns a dictionary with window parameters for creating an expandable PySimpleGUI window."""
-    return {"size": size, "resizable": True, "scrollable": True, "auto_size_text": True, "expand_x": True, "expand_y": True}
+    return {"size": size, "resizable": resizable, "scrollable": scrollable, "auto_size_text": auto_size_text, "expand_x": expand_x, "expand_y": expand_y}
 def get_browser(title:str=None,type:str='Folder',args:dict={},initial_folder:str=get_current_path()):
     """
     Function to get a browser GUI based on the type specified.
 
     Parameters:
     type (str): The type of GUI window to display. Defaults to 'Folder'.
     title (str): The title of the GUI window. Defaults to 'Directory'.
```

### Comparing `abstract_gui-0.0.53.95/src/abstract_gui/main.py` & `abstract_gui-0.0.53.96/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.95/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.53.96/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.95
+Version: 0.0.53.96
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

