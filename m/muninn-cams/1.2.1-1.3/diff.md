# Comparing `tmp/muninn-cams-1.2.1.tar.gz` & `tmp/muninn-cams-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muninn-cams-1.2.1.tar", last modified: Mon Nov 28 12:17:13 2022, max compression
+gzip compressed data, was "dist/muninn-cams-1.3.tar", last modified: Mon Jul 31 11:01:02 2023, max compression
```

## Comparing `muninn-cams-1.2.1.tar` & `muninn-cams-1.3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/
--rw-r--r--   0 sander     (501) staff       (20)      598 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)     1513 2022-07-04 13:55:22.000000 muninn-cams-1.2.1/LICENSE
--rw-r--r--   0 sander     (501) staff       (20)      691 2022-11-28 12:01:06.000000 muninn-cams-1.2.1/setup.py
--rw-r--r--   0 sander     (501) staff       (20)       38 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/setup.cfg
--rw-r--r--   0 sander     (501) staff       (20)      844 2022-03-02 12:40:38.000000 muninn-cams-1.2.1/README.rst
--rw-r--r--   0 sander     (501) staff       (20)    21672 2022-11-28 12:00:49.000000 muninn-cams-1.2.1/muninn_cams.py
-drwxr-xr-x   0 sander     (501) staff       (20)        0 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/
--rw-r--r--   0 sander     (501) staff       (20)      598 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/PKG-INFO
--rw-r--r--   0 sander     (501) staff       (20)      216 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/SOURCES.txt
--rw-r--r--   0 sander     (501) staff       (20)       24 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/requires.txt
--rw-r--r--   0 sander     (501) staff       (20)       12 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/top_level.txt
--rw-r--r--   0 sander     (501) staff       (20)        1 2022-11-28 12:17:13.000000 muninn-cams-1.2.1/muninn_cams.egg-info/dependency_links.txt
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-31 11:01:02.000000 muninn-cams-1.3/
+-rw-r--r--   0 sander     (501) staff       (20)      596 2023-07-31 11:01:02.000000 muninn-cams-1.3/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)      689 2023-07-31 10:55:32.000000 muninn-cams-1.3/setup.py
+-rw-r--r--   0 sander     (501) staff       (20)       38 2023-07-31 11:01:02.000000 muninn-cams-1.3/setup.cfg
+-rw-r--r--   0 sander     (501) staff       (20)      844 2022-03-02 12:40:38.000000 muninn-cams-1.3/README.rst
+-rw-r--r--   0 sander     (501) staff       (20)    14655 2023-07-07 08:00:53.000000 muninn-cams-1.3/muninn_cams.py
+drwxr-xr-x   0 sander     (501) staff       (20)        0 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/
+-rw-r--r--   0 sander     (501) staff       (20)      596 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/PKG-INFO
+-rw-r--r--   0 sander     (501) staff       (20)      208 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/SOURCES.txt
+-rw-r--r--   0 sander     (501) staff       (20)       24 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/requires.txt
+-rw-r--r--   0 sander     (501) staff       (20)       12 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/top_level.txt
+-rw-r--r--   0 sander     (501) staff       (20)        1 2023-07-31 11:01:02.000000 muninn-cams-1.3/muninn_cams.egg-info/dependency_links.txt
```

### Comparing `muninn-cams-1.2.1/PKG-INFO` & `muninn-cams-1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: muninn-cams
-Version: 1.2.1
+Version: 1.3
 Summary: Muninn extension for CAMS GRIB products from the ECMWF mars archive
 Home-page: https://github.com/stcorp/muninn-cams
 Author: S[&]T
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `muninn-cams-1.2.1/setup.py` & `muninn-cams-1.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="muninn-cams",
-    version="1.2.1",
+    version="1.3",
     description="Muninn extension for CAMS GRIB products from the ECMWF mars archive",
     url="https://github.com/stcorp/muninn-cams",
     author="S[&]T",
     license="BSD",
     py_modules=["muninn_cams"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `muninn-cams-1.2.1/README.rst` & `muninn-cams-1.3/README.rst`

 * *Files identical despite different names*

### Comparing `muninn-cams-1.2.1/muninn_cams.egg-info/PKG-INFO` & `muninn-cams-1.3/muninn_cams.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: muninn-cams
-Version: 1.2.1
+Version: 1.3
 Summary: Muninn extension for CAMS GRIB products from the ECMWF mars archive
 Home-page: https://github.com/stcorp/muninn-cams
 Author: S[&]T
 Author-email: UNKNOWN
 License: BSD
 Description: UNKNOWN
 Platform: UNKNOWN
```

