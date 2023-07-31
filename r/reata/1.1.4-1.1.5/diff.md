# Comparing `tmp/reata-1.1.4.tar.gz` & `tmp/reata-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reata-1.1.4.tar", last modified: Sun Jul 30 07:09:48 2023, max compression
+gzip compressed data, was "reata-1.1.5.tar", last modified: Mon Jul 31 03:18:21 2023, max compression
```

## Comparing `reata-1.1.4.tar` & `reata-1.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-30 07:09:48.000000 reata-1.1.4/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.4/LICENSE
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-30 07:09:48.000000 reata-1.1.4/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.4/README.rst
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-30 07:09:48.000000 reata-1.1.4/reata/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     6008 2023-07-30 07:06:23.000000 reata-1.1.4/reata/__futures__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.4/reata/__init__.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-04-13 02:09:12.000000 reata-1.1.4/reata/client.py
--rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.4/reata/schema.py
-drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/
--rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/PKG-INFO
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/SOURCES.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/dependency_links.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       73 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/requires.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-07-30 07:09:48.000000 reata-1.1.4/reata.egg-info/top_level.txt
--rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-07-30 07:09:48.000000 reata-1.1.4/setup.cfg
--rw-rw-r--   0 subvert   (1000) subvert   (1000)      599 2023-07-30 07:06:23.000000 reata-1.1.4/setup.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    35149 2022-12-27 12:35:32.000000 reata-1.1.5/LICENSE
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-31 03:18:21.000000 reata-1.1.5/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     1812 2023-01-08 05:17:25.000000 reata-1.1.5/README.rst
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/reata/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     6008 2023-07-30 07:06:23.000000 reata-1.1.5/reata/__futures__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       74 2023-01-08 04:34:06.000000 reata-1.1.5/reata/__init__.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    22848 2023-04-13 02:09:12.000000 reata-1.1.5/reata/client.py
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)     2974 2023-07-15 21:59:03.000000 reata-1.1.5/reata/schema.py
+drwxrwxr-x   0 subvert   (1000) subvert   (1000)        0 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)    42542 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/PKG-INFO
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      242 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/SOURCES.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        1 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/dependency_links.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       73 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/requires.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)        6 2023-07-31 03:18:21.000000 reata-1.1.5/reata.egg-info/top_level.txt
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)       38 2023-07-31 03:18:21.000000 reata-1.1.5/setup.cfg
+-rw-rw-r--   0 subvert   (1000) subvert   (1000)      599 2023-07-31 03:17:42.000000 reata-1.1.5/setup.py
```

### Comparing `reata-1.1.4/LICENSE` & `reata-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `reata-1.1.4/PKG-INFO` & `reata-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.4
+Version: 1.1.5
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.4/README.rst` & `reata-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `reata-1.1.4/reata/__futures__.py` & `reata-1.1.5/reata/__futures__.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.4/reata/client.py` & `reata-1.1.5/reata/client.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.4/reata/schema.py` & `reata-1.1.5/reata/schema.py`

 * *Files identical despite different names*

### Comparing `reata-1.1.4/reata.egg-info/PKG-INFO` & `reata-1.1.5/reata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reata
-Version: 1.1.4
+Version: 1.1.5
 Summary: A simple MySQL DBAPI wrapper for simplifying data processing pipelines.
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `reata-1.1.4/setup.py` & `reata-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from setuptools import find_packages, setup
 
 src = Path(__file__).parent
 
 setup(
     name="reata",
-    version="1.1.4",
+    version="1.1.5",
     description=(
         "A simple MySQL DBAPI wrapper for simplifying "
         "data processing pipelines."
     ),
     long_description=(src/"README.rst").read_text(),
     packages=find_packages(),
     install_requires=[
```

