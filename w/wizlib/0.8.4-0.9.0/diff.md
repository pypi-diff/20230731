# Comparing `tmp/wizlib-0.8.4.tar.gz` & `tmp/wizlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizlib-0.8.4.tar", last modified: Sun Jul 30 22:15:35 2023, max compression
+gzip compressed data, was "wizlib-0.9.0.tar", last modified: Mon Jul 31 01:10:39 2023, max compression
```

## Comparing `wizlib-0.8.4.tar` & `wizlib-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:15:35.517659 wizlib-0.8.4/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-30 22:14:45.000000 wizlib-0.8.4/.version
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-30 22:15:35.517659 wizlib-0.8.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-30 22:15:27.000000 wizlib-0.8.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-30 22:15:27.000000 wizlib-0.8.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-30 22:15:35.517659 wizlib-0.8.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:15:35.514659 wizlib-0.8.4/test/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-30 22:15:27.000000 wizlib-0.8.4/test/test_class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-30 22:15:27.000000 wizlib-0.8.4/test/test_command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     3150 2023-07-30 22:15:27.000000 wizlib-0.8.4/test/test_config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-30 22:15:27.000000 wizlib-0.8.4/test/test_super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:15:35.516659 wizlib-0.8.4/wizlib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/class_family.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/command_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/config_machine.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/rlinput.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-30 22:15:27.000000 wizlib-0.8.4/wizlib/super_wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:15:35.517659 wizlib-0.8.4/wizlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5384 2023-07-30 22:15:35.000000 wizlib-0.8.4/wizlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      427 2023-07-30 22:15:35.000000 wizlib-0.8.4/wizlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 22:15:35.000000 wizlib-0.8.4/wizlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      103 2023-07-30 22:15:35.000000 wizlib-0.8.4/wizlib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-30 22:15:35.000000 wizlib-0.8.4/wizlib.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.463452 wizlib-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-31 01:09:48.000000 wizlib-0.9.0/.version
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:10:39.463452 wizlib-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-31 01:10:30.000000 wizlib-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-31 01:10:30.000000 wizlib-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 01:10:39.463452 wizlib-0.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.460452 wizlib-0.9.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     3150 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2023-07-31 01:10:30.000000 wizlib-0.9.0/test/test_super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.461452 wizlib-0.9.0/wizlib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/class_family.py
+-rw-rw-rw-   0 root         (0) root         (0)     2763 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/command_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/config_machine.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/rlinput.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-07-31 01:10:30.000000 wizlib-0.9.0/wizlib/super_wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 01:10:39.462452 wizlib-0.9.0/wizlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5384 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      427 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-31 01:10:39.000000 wizlib-0.9.0/wizlib.egg-info/top_level.txt
```

### Comparing `wizlib-0.8.4/PKG-INFO` & `wizlib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.8.4
+Version: 0.9.0
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

### Comparing `wizlib-0.8.4/README.md` & `wizlib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/pyproject.toml` & `wizlib-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/test/test_command_handler.py` & `wizlib-0.9.0/test/test_command_handler.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/test/test_config_machine.py` & `wizlib-0.9.0/test/test_config_machine.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/test/test_super_wrapper.py` & `wizlib-0.9.0/test/test_super_wrapper.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/wizlib/class_family.py` & `wizlib-0.9.0/wizlib/class_family.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/wizlib/command_handler.py` & `wizlib-0.9.0/wizlib/command_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class CommandHandler:
     """Handle commands from a ClassFamily"""
 
     def __init__(self, atriarch):
         """Pass in the command base class, the atriarch of a
         classfamily that meeting the CommandHandler spec"""
-        self.parser = ArgumentParser(prog=atriarch.app_name,
+        self.parser = ArgumentParser(prog=atriarch.appname,
                                      exit_on_error=False)
         atriarch.add_app_args(self.parser)
         subparsers = self.parser.add_subparsers(dest='command')
         for command in atriarch.family_members('name'):
             key = command.get_member_attr('key')
             aliases = [key] if key else []
             subparser = subparsers.add_parser(command.name, aliases=aliases)
```

### Comparing `wizlib-0.8.4/wizlib/config_machine.py` & `wizlib-0.9.0/wizlib/config_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     appname - The name of the config file, environment variable, etc. - meant
     to be populated as a class attribute (though can also be passed to init)
 
     config - Path to a config file. Meant to be populated in the init method.
     """
 
-    appname: str = ''
+    appname = ''
     config: str = None
 
     @property
     def config_yaml(self):
         if hasattr(self, '_config_yaml'):
             return self._config_yaml
         if hasattr(self, 'config') and (val := self.config):
```

### Comparing `wizlib-0.8.4/wizlib/rlinput.py` & `wizlib-0.9.0/wizlib/rlinput.py`

 * *Files identical despite different names*

### Comparing `wizlib-0.8.4/wizlib.egg-info/PKG-INFO` & `wizlib-0.9.0/wizlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wizlib
-Version: 0.8.4
+Version: 0.9.0
 Summary: A collection of Python modules that are useful across multiple projects
 Author-email: Francis Potter <wizlib@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # WizLib
```

