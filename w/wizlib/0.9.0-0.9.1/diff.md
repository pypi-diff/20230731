# Comparing `tmp/wizlib-0.9.0.tar.gz` & `tmp/wizlib-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.9.0.tar", last modified: Mon Jul 31 01:10:39 2023, max compression
+gzip compressed data, was "wizlib-0.9.1.tar", last modified: Mon Jul 31 01:50:17 2023, max compression
```

## Comparing `wizlib-0.9.0.tar` & `wizlib-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.463452 wizlib-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-31 01:09:48.000000 wizlib-0.9.0/.version
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:10:39.463452 wizlib-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-31 01:10:30.000000 wizlib-0.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-31 01:10:30.000000 wizlib-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 01:10:39.463452 wizlib-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.460452 wizlib-0.9.0/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3150 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.461452 wizlib-0.9.0/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2763 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.462452 wizlib-0.9.0/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:50:17.683741 wizlib-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-31 01:49:27.000000 wizlib-0.9.1/.version
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:50:17.682741 wizlib-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-31 01:50:09.000000 wizlib-0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-31 01:50:09.000000 wizlib-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 01:50:17.683741 wizlib-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:50:17.680741 wizlib-0.9.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-31 01:50:09.000000 wizlib-0.9.1/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-31 01:50:09.000000 wizlib-0.9.1/test/test_command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3150 2023-07-31 01:50:09.000000 wizlib-0.9.1/test/test_config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-31 01:50:09.000000 wizlib-0.9.1/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:50:17.681741 wizlib-0.9.1/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2938 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-31 01:50:09.000000 wizlib-0.9.1/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:50:17.682741 wizlib-0.9.1/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:50:17.000000 wizlib-0.9.1/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-31 01:50:17.000000 wizlib-0.9.1/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 01:50:17.000000 wizlib-0.9.1/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-31 01:50:17.000000 wizlib-0.9.1/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 01:50:17.000000 wizlib-0.9.1/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.9.0/PKG-INFO` & `wizlib-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.9.0/README.md` & `wizlib-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/pyproject.toml` & `wizlib-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/test/test_command_handler.py` & `wizlib-0.9.1/test/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/test/test_config_machine.py` & `wizlib-0.9.1/test/test_config_machine.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/test/test_super_wrapper.py` & `wizlib-0.9.1/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/wizlib/class_family.py` & `wizlib-0.9.1/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/wizlib/command_handler.py` & `wizlib-0.9.1/wizlib/command_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from argparse import ArgumentError, ArgumentParser
 from dataclasses import dataclass
 
 from wizlib.class_family import ClassFamily
 from wizlib.super_wrapper import SuperWrapper
 
 
+RED = '\033[91m'
+RESET = '\033[0m'
+
+
 class CommandHandler:
     """Handle commands from a ClassFamily"""
 
     def __init__(self, atriarch):
         """Pass in the command base class, the atriarch of a
         classfamily that meeting the CommandHandler spec"""
         self.parser = ArgumentParser(prog=atriarch.appname,
@@ -45,19 +49,22 @@
             return result, command.status
         else:
             return None, None
 
     @classmethod
     def shell(cls, atriarch):
         """Call this from a shell/main entrypoint"""
-        result, status = cls(atriarch).handle(sys.argv[1:])
-        if result:
-            print(result)
-        if status:
-            print(status)
+        try:
+            result, status = cls(atriarch).handle(sys.argv[1:])
+            if result:
+                print(result)
+            if status:
+                print(status)
+        except Exception as error:
+            print(f"\n{RED}{type(error).__name__}: {error}{RESET}\n")
 
 
 @dataclass
 class Command(ClassFamily, SuperWrapper):
 
     status = ''
```

### Comparing `wizlib-0.9.0/wizlib/config_machine.py` & `wizlib-0.9.1/wizlib/config_machine.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/wizlib/rlinput.py` & `wizlib-0.9.1/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.9.0/wizlib.egg-info/PKG-INFO` & `wizlib-0.9.1/wizlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.9.0
+Version: 0.9.1
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

