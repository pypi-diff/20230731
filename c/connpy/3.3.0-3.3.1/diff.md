# Comparing `tmp/connpy-3.3.0.tar.gz` & `tmp/connpy-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.3.0.tar", last modified: Tue Jul 11 22:34:40 2023, max compression
+gzip compressed data, was "connpy-3.3.1.tar", last modified: Mon Jul 31 15:19:31 2023, max compression
```

## Comparing `connpy-3.3.0.tar` & `connpy-3.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 22:34:26.000000 connpy-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-11 22:34:40.562689 connpy-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-11 22:34:26.000000 connpy-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24594 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4518 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56866 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29185 2023-07-11 22:34:26.000000 connpy-3.3.0/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 22:34:40.562689 connpy-3.3.0/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 22:34:40.000000 connpy-3.3.0/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-11 22:34:40.566689 connpy-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 22:34:26.000000 connpy-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:31.631940 connpy-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 15:19:17.000000 connpy-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-31 15:19:31.631940 connpy-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-07-31 15:19:17.000000 connpy-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:31.631940 connpy-3.3.1/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24594 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5102 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4518 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56982 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29185 2023-07-31 15:19:17.000000 connpy-3.3.1/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:31.631940 connpy-3.3.1/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 15:19:31.000000 connpy-3.3.1/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 15:19:31.631940 connpy-3.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 15:19:17.000000 connpy-3.3.1/setup.py
```

### Comparing `connpy-3.3.0/LICENSE` & `connpy-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/PKG-INFO` & `connpy-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.3.0
+Version: 3.3.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.3.0/README.md` & `connpy-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/__init__.py` & `connpy-3.3.1/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/ai.py` & `connpy-3.3.1/connpy/ai.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/api.py` & `connpy-3.3.1/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/completion.py` & `connpy-3.3.1/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/configfile.py` & `connpy-3.3.1/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy/connapp.py` & `connpy-3.3.1/connpy/connapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,17 +594,21 @@
         if not re.match(regex, current):
             raise inquirer.errors.ValidationError("", reason="Can't send empty messages")
         return True
 
     def _process_input(self, input, history):
         response = self.myai.ask(input , chat_history = history, dryrun = True)
         if not response["app_related"]:
-            if not history:
-                history = []
-            history.extend(response["chat_history"])
+            try:
+                if not history:
+                    history = []
+                history.extend(response["chat_history"])
+            except:
+                if not history:
+                    history = None
             return response["response"], history
         else:
             history = None
             if response["action"] == "list_nodes":
                 if response["filter"]:
                     nodes = self.config._getallnodes(response["filter"])
                 else:
```

### Comparing `connpy-3.3.0/connpy/core.py` & `connpy-3.3.1/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.3.0/connpy.egg-info/PKG-INFO` & `connpy-3.3.1/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.3.0
+Version: 3.3.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.3.0/setup.cfg` & `connpy-3.3.1/setup.cfg`

 * *Files identical despite different names*

