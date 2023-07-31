# Comparing `tmp/pycur-2023.7.30.3.tar.gz` & `tmp/pycur-2023.7.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycur-2023.7.30.3.tar", last modified: Sun Jul 30 09:26:24 2023, max compression
+gzip compressed data, was "dist/pycur-2023.7.31.0.tar", last modified: Mon Jul 31 07:49:01 2023, max compression
```

## Comparing `pycur-2023.7.30.3.tar` & `pycur-2023.7.31.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/
--rw-rw-r--   0 app       (1000) app       (1000)      681 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/PKG-INFO
-drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur/
--rw-r--r--   0 app       (1000) app       (1000)     1431 2023-07-30 09:26:19.000000 pycur-2023.7.30.3/pycur/__init__.py
-drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/
--rw-rw-r--   0 app       (1000) app       (1000)      681 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/PKG-INFO
--rw-rw-r--   0 app       (1000) app       (1000)      142 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/SOURCES.txt
--rw-rw-r--   0 app       (1000) app       (1000)        1 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/dependency_links.txt
--rw-rw-r--   0 app       (1000) app       (1000)        6 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/pycur.egg-info/top_level.txt
--rw-rw-r--   0 app       (1000) app       (1000)       38 2023-07-30 09:26:24.000000 pycur-2023.7.30.3/setup.cfg
--rw-r--r--   0 app       (1000) app       (1000)      356 2023-07-30 09:19:47.000000 pycur-2023.7.30.3/setup.py
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/
+-rw-rw-r--   0 app       (1000) app       (1000)      698 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/PKG-INFO
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur/
+-rw-r--r--   0 app       (1000) app       (1000)     1431 2023-07-31 07:48:57.000000 pycur-2023.7.31.0/pycur/__init__.py
+drwxrwxr-x   0 app       (1000) app       (1000)        0 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur.egg-info/
+-rw-rw-r--   0 app       (1000) app       (1000)      698 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur.egg-info/PKG-INFO
+-rw-rw-r--   0 app       (1000) app       (1000)      142 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur.egg-info/SOURCES.txt
+-rw-rw-r--   0 app       (1000) app       (1000)        1 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur.egg-info/dependency_links.txt
+-rw-rw-r--   0 app       (1000) app       (1000)        6 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/pycur.egg-info/top_level.txt
+-rw-rw-r--   0 app       (1000) app       (1000)       38 2023-07-31 07:49:01.000000 pycur-2023.7.31.0/setup.cfg
+-rw-r--r--   0 app       (1000) app       (1000)      389 2023-07-31 07:47:00.000000 pycur-2023.7.31.0/setup.py
```

### Comparing `pycur-2023.7.30.3/PKG-INFO` & `pycur-2023.7.31.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pycur
-Version: 2023.7.30.3
+Version: 2023.7.31.0
 Summary: Modifying cursors is now easier than ever!
-Home-page: UNKNOWN
+Home-page: https://pycur.glitch.me/
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `pycur-2023.7.30.3/pycur/__init__.py` & `pycur-2023.7.31.0/pycur/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2023.07.30.3"
+__version__ = "2023.07.31.0"
 
 class Error(BaseException): pass
 
 class Color:
 	def __init__(self, r, g, b):
 		if True in [(mode > 255 or mode < 0) for mode in [r, g, b]]:
 			raise Error("RGB values must be in the range of 0-255")
```

### Comparing `pycur-2023.7.30.3/pycur.egg-info/PKG-INFO` & `pycur-2023.7.31.0/pycur.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pycur
-Version: 2023.7.30.3
+Version: 2023.7.31.0
 Summary: Modifying cursors is now easier than ever!
-Home-page: UNKNOWN
+Home-page: https://pycur.glitch.me/
 Author: RixTheTyrunt
 Author-email: rixthetyrunt@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

