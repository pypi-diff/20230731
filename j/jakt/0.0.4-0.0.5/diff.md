# Comparing `tmp/jakt-0.0.4.tar.gz` & `tmp/jakt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jakt-0.0.4.tar", last modified: Mon Jul 31 12:54:34 2023, max compression
+gzip compressed data, was "jakt-0.0.5.tar", last modified: Mon Jul 31 13:59:07 2023, max compression
```

## Comparing `jakt-0.0.4.tar` & `jakt-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 12:54:24.000000 jakt-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 12:54:34.343167 jakt-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 12:54:24.000000 jakt-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/jakt/
--rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-31 12:54:24.000000 jakt-0.0.4/jakt/timeslot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:54:34.343167 jakt-0.0.4/jakt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 12:54:34.000000 jakt-0.0.4/jakt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 12:54:24.000000 jakt-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 12:54:24.000000 jakt-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:54:34.343167 jakt-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:59:07.744287 jakt-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-31 13:58:57.000000 jakt-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 13:59:07.744287 jakt-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-07-31 13:58:57.000000 jakt-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:59:07.744287 jakt-0.0.5/jakt/
+-rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-31 13:58:57.000000 jakt-0.0.5/jakt/timeslot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:59:07.744287 jakt-0.0.5/jakt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 13:59:07.000000 jakt-0.0.5/jakt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-31 13:58:57.000000 jakt-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 13:58:57.000000 jakt-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:59:07.744287 jakt-0.0.5/setup.cfg
```

### Comparing `jakt-0.0.4/LICENSE` & `jakt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jakt-0.0.4/PKG-INFO` & `jakt-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jakt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Just another (k)ommandline timetracker
 Author-email: kwillno <kristian@kwill.no>
 Project-URL: Homepage, https://github.com/kwillno/jakt
 Project-URL: Bug Tracker, https://github.com/kwillno/jakt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `jakt-0.0.4/README.md` & `jakt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `jakt-0.0.4/jakt/__init__.py` & `jakt-0.0.5/jakt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -213,17 +213,20 @@
     def getTimeslots(
         self, from_=False, to=False, project=False, tag=False
     ) -> list[timeslot]:
         """
         Returns a list of logged timeslots
         """
         try:
-            with open(self.pathTimeslots, "r") as f:
-                timeslots = json.load(f)
-                f.close()
+       	    try:
+                with open(self.pathTimeslots, "r") as f:
+                    timeslots = json.load(f)
+                    f.close()
+            except json.JSONDecodeError:
+                return[]
 
             # Create timeslot instances
             for i in range(len(timeslots)):
                 timeslots[i] = timeslot.from_json(timeslots[i])
 
             # TODO: Implement filtering with to and from_
             if to and from_:
```

### Comparing `jakt-0.0.4/jakt/cli.py` & `jakt-0.0.5/jakt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from .__init__ import jakt
 from .timeslot import timeslot
 from .exceptions import *
 
 
 @click.group()
-@click.version_option(version="0.0.4", prog_name="jakt")
+@click.version_option(version="0.0.5", prog_name="jakt")
 @click.pass_context
 def cli(ctx):
     """Jakt is just another (k)ommandline timetracker.
 
     Jakt helps you keep track of how you spend your time.
     Whether you want to keep better track of how much time
     you spend on each project or want to keep yourself
```

### Comparing `jakt-0.0.4/jakt/report.py` & `jakt-0.0.5/jakt/report.py`

 * *Files identical despite different names*

### Comparing `jakt-0.0.4/jakt/timeslot.py` & `jakt-0.0.5/jakt/timeslot.py`

 * *Files identical despite different names*

### Comparing `jakt-0.0.4/jakt.egg-info/PKG-INFO` & `jakt-0.0.5/jakt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jakt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Just another (k)ommandline timetracker
 Author-email: kwillno <kristian@kwill.no>
 Project-URL: Homepage, https://github.com/kwillno/jakt
 Project-URL: Bug Tracker, https://github.com/kwillno/jakt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
```

### Comparing `jakt-0.0.4/pyproject.toml` & `jakt-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "jakt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="kwillno", email="kristian@kwill.no" },
 ]
 description = "Just another (k)ommandline timetracker"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

