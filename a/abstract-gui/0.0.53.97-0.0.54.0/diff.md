# Comparing `tmp/abstract_gui-0.0.53.97.tar.gz` & `tmp/abstract_gui-0.0.54.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_gui-0.0.53.97.tar", last modified: Mon Jul 31 08:04:33 2023, max compression
+gzip compressed data, was "abstract_gui-0.0.54.0.tar", last modified: Mon Jul 31 08:20:35 2023, max compression
```

## Comparing `abstract_gui-0.0.53.97.tar` & `abstract_gui-0.0.54.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8473 2023-07-31 00:08:47.000000 abstract_gui-0.0.53.97/README.md
--rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.53.97/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1125 2023-07-31 08:04:28.000000 abstract_gui-0.0.53.97/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/abstract_gui/
--rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.53.97/src/abstract_gui/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22303 2023-07-31 08:03:34.000000 abstract_gui-0.0.53.97/src/abstract_gui/abstract_gui.py
--rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.53.97/src/abstract_gui/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:04:33.102896 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9211 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 08:04:33.000000 abstract_gui-0.0.53.97/src/abstract_gui.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/
+-rw-r--r--   0 root         (0) root         (0)    10093 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     9356 2023-07-31 08:20:01.000000 abstract_gui-0.0.54.0/README.md
+-rw-rw-r--   0 root         (0) root         (0)       85 2023-07-29 19:09:21.000000 abstract_gui-0.0.54.0/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1124 2023-07-31 08:15:39.000000 abstract_gui-0.0.54.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/src/abstract_gui/
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-07-31 06:21:46.000000 abstract_gui-0.0.54.0/src/abstract_gui/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22303 2023-07-31 08:18:20.000000 abstract_gui-0.0.54.0/src/abstract_gui/abstract_gui.py
+-rw-rw-r--   0 root         (0) root         (0)     1602 2023-07-31 04:07:58.000000 abstract_gui-0.0.54.0/src/abstract_gui/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 08:20:35.003931 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10093 2023-07-31 08:20:34.000000 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      329 2023-07-31 08:20:34.000000 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 08:20:34.000000 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-07-31 08:20:34.000000 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-31 08:20:34.000000 abstract_gui-0.0.54.0/src/abstract_gui.egg-info/top_level.txt
```

### Comparing `abstract_gui-0.0.53.97/PKG-INFO` & `abstract_gui-0.0.54.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_gui
-Version: 0.0.53.97
+Version: 0.0.54.0
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -263,26 +263,35 @@
 ```python
 # Import the module
 import abstract_gui
 
 # Create a global bridge instance
 global_bridge = abstract_gui.WindowGlobalBridge()
 
-# Create a window manager instance for a script named "example_script"
+# Create a window manager instance for a script named "example_script"; interacts with the global bridge for modular event handling for script specific functions
 window_manager = abstract_gui.WindowManager("example_script", global_bridge)
 
-# Create a new PySimpleGUI window using the window manager
-window = window_manager.get_new_window(title="Example Window", layout=[[abstract_gui.get_gui_fun('Text', {"text": "Hello, PySimpleGUI!"})]])
+#or use the window_manager initialization function
+window_mgr,bridge,script_name = abstract_gui.create_window_manager(script_name="example_script",global_var=globals())
+
+#Create components for a layout
+#input args, a dictionary with window parameters for any and all parameter inputs. an incompatible parameter will not be applied, error free component utilization
+layout = abstract_gui.get_gui_fun('Text', args={"text": "Hello, PySimpleGUI!"})
+
+#make component expandable (it will not error out if arguments are incompatible); with customizable legacy inputs
+#Returns a dictionary with window parameters for creating an expandable PySimpleGUI window.
+expand = abstract_gui.expandable()
+
+# Create a new PySimpleGUI window using the window manager, add the stringified function name as event_function for binded event handling
+#get_new_window(self, title=None, layout=None, args=None, event_function=None, exit_events:list=["exit", "Exit", "EXIT"])
+window = window_manager.get_new_window(title="Example Window", args={"layout":[[layout]],**expand})
 
 # Run the event loop for the window
 window_manager.while_basic(window)
 
-# Close the window
-window_manager.close_window(window)
-
 # Retrieve all registered windows and their details
 all_windows = window_manager.get_all_windows()
 ```
 
 Please refer to the source code for the complete list of classes and functions provided by the module, as well as their detailed documentation.
 
 ## Contributing
```

### Comparing `abstract_gui-0.0.53.97/README.md` & `abstract_gui-0.0.54.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -248,26 +248,35 @@
 ```python
 # Import the module
 import abstract_gui
 
 # Create a global bridge instance
 global_bridge = abstract_gui.WindowGlobalBridge()
 
-# Create a window manager instance for a script named "example_script"
+# Create a window manager instance for a script named "example_script"; interacts with the global bridge for modular event handling for script specific functions
 window_manager = abstract_gui.WindowManager("example_script", global_bridge)
 
-# Create a new PySimpleGUI window using the window manager
-window = window_manager.get_new_window(title="Example Window", layout=[[abstract_gui.get_gui_fun('Text', {"text": "Hello, PySimpleGUI!"})]])
+#or use the window_manager initialization function
+window_mgr,bridge,script_name = abstract_gui.create_window_manager(script_name="example_script",global_var=globals())
+
+#Create components for a layout
+#input args, a dictionary with window parameters for any and all parameter inputs. an incompatible parameter will not be applied, error free component utilization
+layout = abstract_gui.get_gui_fun('Text', args={"text": "Hello, PySimpleGUI!"})
+
+#make component expandable (it will not error out if arguments are incompatible); with customizable legacy inputs
+#Returns a dictionary with window parameters for creating an expandable PySimpleGUI window.
+expand = abstract_gui.expandable()
+
+# Create a new PySimpleGUI window using the window manager, add the stringified function name as event_function for binded event handling
+#get_new_window(self, title=None, layout=None, args=None, event_function=None, exit_events:list=["exit", "Exit", "EXIT"])
+window = window_manager.get_new_window(title="Example Window", args={"layout":[[layout]],**expand})
 
 # Run the event loop for the window
 window_manager.while_basic(window)
 
-# Close the window
-window_manager.close_window(window)
-
 # Retrieve all registered windows and their details
 all_windows = window_manager.get_all_windows()
 ```
 
 Please refer to the source code for the complete list of classes and functions provided by the module, as well as their detailed documentation.
 
 ## Contributing
```

### Comparing `abstract_gui-0.0.53.97/setup.py` & `abstract_gui-0.0.54.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_gui',
-    version='0.0.53.97',
+    version='0.0.54.0',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description='abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui',
     classifiers=[
```

### Comparing `abstract_gui-0.0.53.97/src/abstract_gui/abstract_gui.py` & `abstract_gui-0.0.54.0/src/abstract_gui/abstract_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.97/src/abstract_gui/main.py` & `abstract_gui-0.0.54.0/src/abstract_gui/main.py`

 * *Files identical despite different names*

### Comparing `abstract_gui-0.0.53.97/src/abstract_gui.egg-info/PKG-INFO` & `abstract_gui-0.0.54.0/src/abstract_gui.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract-gui
-Version: 0.0.53.97
+Version: 0.0.54.0
 Summary: abstract_gui is a python module for creating abstract GUI windows and interacting with them. It uses the PySimpleGUI library and provides additional utilities for simplifying the creation and handling of PySimpleGUI windows.
 Home-page: https://github.com/AbstractEndeavors/abstract_essentials/abstract_gui
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -263,26 +263,35 @@
 ```python
 # Import the module
 import abstract_gui
 
 # Create a global bridge instance
 global_bridge = abstract_gui.WindowGlobalBridge()
 
-# Create a window manager instance for a script named "example_script"
+# Create a window manager instance for a script named "example_script"; interacts with the global bridge for modular event handling for script specific functions
 window_manager = abstract_gui.WindowManager("example_script", global_bridge)
 
-# Create a new PySimpleGUI window using the window manager
-window = window_manager.get_new_window(title="Example Window", layout=[[abstract_gui.get_gui_fun('Text', {"text": "Hello, PySimpleGUI!"})]])
+#or use the window_manager initialization function
+window_mgr,bridge,script_name = abstract_gui.create_window_manager(script_name="example_script",global_var=globals())
+
+#Create components for a layout
+#input args, a dictionary with window parameters for any and all parameter inputs. an incompatible parameter will not be applied, error free component utilization
+layout = abstract_gui.get_gui_fun('Text', args={"text": "Hello, PySimpleGUI!"})
+
+#make component expandable (it will not error out if arguments are incompatible); with customizable legacy inputs
+#Returns a dictionary with window parameters for creating an expandable PySimpleGUI window.
+expand = abstract_gui.expandable()
+
+# Create a new PySimpleGUI window using the window manager, add the stringified function name as event_function for binded event handling
+#get_new_window(self, title=None, layout=None, args=None, event_function=None, exit_events:list=["exit", "Exit", "EXIT"])
+window = window_manager.get_new_window(title="Example Window", args={"layout":[[layout]],**expand})
 
 # Run the event loop for the window
 window_manager.while_basic(window)
 
-# Close the window
-window_manager.close_window(window)
-
 # Retrieve all registered windows and their details
 all_windows = window_manager.get_all_windows()
 ```
 
 Please refer to the source code for the complete list of classes and functions provided by the module, as well as their detailed documentation.
 
 ## Contributing
```

