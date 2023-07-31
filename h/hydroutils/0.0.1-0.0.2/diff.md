# Comparing `tmp/hydroutils-0.0.1.tar.gz` & `tmp/hydroutils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydroutils-0.0.1.tar", last modified: Mon Jul 31 08:41:51 2023, max compression
+gzip compressed data, was "hydroutils-0.0.2.tar", last modified: Mon Jul 31 09:16:04 2023, max compression
```

## Comparing `hydroutils-0.0.1.tar` & `hydroutils-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxr-x   0 owen411   (1003) owen411   (1003)        0 2023-07-31 08:41:51.444522 hydroutils-0.0.1/
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      161 2023-07-31 08:32:56.000000 hydroutils-0.0.1/AUTHORS.rst
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     1071 2023-07-31 08:32:56.000000 hydroutils-0.0.1/LICENSE
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      122 2023-07-31 08:32:56.000000 hydroutils-0.0.1/MANIFEST.in
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     1572 2023-07-31 08:41:51.444522 hydroutils-0.0.1/PKG-INFO
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      741 2023-07-31 08:32:56.000000 hydroutils-0.0.1/README.md
-drwxrwxr-x   0 owen411   (1003) owen411   (1003)        0 2023-07-31 08:41:51.440522 hydroutils-0.0.1/hydroutils/
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      388 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/__init__.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      445 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/cli.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      929 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_arithmetric.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     6081 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_file.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      554 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_logger.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)    37019 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_plot.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)    22247 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_stat.py
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     3672 2023-07-31 08:32:56.000000 hydroutils-0.0.1/hydroutils/hydro_time.py
-drwxrwxr-x   0 owen411   (1003) owen411   (1003)        0 2023-07-31 08:41:51.440522 hydroutils-0.0.1/hydroutils.egg-info/
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     1572 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/PKG-INFO
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      541 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/SOURCES.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)       59 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/dependency_links.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)       51 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/entry_points.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)        1 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/not-zip-safe
--rw-rw-r--   0 owen411   (1003) owen411   (1003)       59 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/requires.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)       11 2023-07-31 08:41:51.000000 hydroutils-0.0.1/hydroutils.egg-info/top_level.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)       58 2023-07-31 08:32:56.000000 hydroutils-0.0.1/requirements.txt
--rw-rw-r--   0 owen411   (1003) owen411   (1003)      452 2023-07-31 08:41:51.444522 hydroutils-0.0.1/setup.cfg
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     2140 2023-07-31 08:32:56.000000 hydroutils-0.0.1/setup.py
-drwxrwxr-x   0 owen411   (1003) owen411   (1003)        0 2023-07-31 08:41:51.444522 hydroutils-0.0.1/tests/
--rw-rw-r--   0 owen411   (1003) owen411   (1003)     1112 2023-07-31 08:32:56.000000 hydroutils-0.0.1/tests/test_hydroutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:16:04.557672 hydroutils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 09:15:54.000000 hydroutils-0.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 09:15:54.000000 hydroutils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 09:15:54.000000 hydroutils-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-31 09:16:04.557672 hydroutils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-31 09:15:54.000000 hydroutils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:16:04.553672 hydroutils-0.0.2/hydroutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_arithmetric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37019 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22247 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-07-31 09:15:54.000000 hydroutils-0.0.2/hydroutils/hydro_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:16:04.557672 hydroutils-0.0.2/hydroutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 09:16:04.000000 hydroutils-0.0.2/hydroutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 09:15:54.000000 hydroutils-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-31 09:16:04.557672 hydroutils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-31 09:15:54.000000 hydroutils-0.0.2/setup.py
```

### Comparing `hydroutils-0.0.1/LICENSE` & `hydroutils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/PKG-INFO` & `hydroutils-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydroutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of commonly used util functions in hydrological modeling
 Home-page: https://github.com/OuyangWenyu/hydroutils
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydroutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hydroutils-0.0.1/README.md` & `hydroutils-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_arithmetric.py` & `hydroutils-0.0.2/hydroutils/hydro_arithmetric.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_file.py` & `hydroutils-0.0.2/hydroutils/hydro_file.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_logger.py` & `hydroutils-0.0.2/hydroutils/hydro_logger.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_plot.py` & `hydroutils-0.0.2/hydroutils/hydro_plot.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_stat.py` & `hydroutils-0.0.2/hydroutils/hydro_stat.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils/hydro_time.py` & `hydroutils-0.0.2/hydroutils/hydro_time.py`

 * *Files identical despite different names*

### Comparing `hydroutils-0.0.1/hydroutils.egg-info/PKG-INFO` & `hydroutils-0.0.2/hydroutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydroutils
-Version: 0.0.1
+Version: 0.0.2
 Summary: A collection of commonly used util functions in hydrological modeling
 Home-page: https://github.com/OuyangWenyu/hydroutils
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydroutils
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hydroutils-0.0.1/hydroutils.egg-info/SOURCES.txt` & `hydroutils-0.0.2/hydroutils.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 hydroutils/hydro_time.py
 hydroutils.egg-info/PKG-INFO
 hydroutils.egg-info/SOURCES.txt
 hydroutils.egg-info/dependency_links.txt
 hydroutils.egg-info/entry_points.txt
 hydroutils.egg-info/not-zip-safe
 hydroutils.egg-info/requires.txt
-hydroutils.egg-info/top_level.txt
-tests/test_hydroutils.py
+hydroutils.egg-info/top_level.txt
```

### Comparing `hydroutils-0.0.1/setup.py` & `hydroutils-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 """
 Author: Wenyu Ouyang
 Date: 2022-12-02 10:42:19
-LastEditTime: 2023-07-27 17:29:44
+LastEditTime: 2023-07-31 17:11:11
 LastEditors: Wenyu Ouyang
 Description: The setup script.
-FilePath: \hydroutils\setup.py
+FilePath: /hydroutils/setup.py
 Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
 """
 
 
 import io
 import pathlib
 from os import path as op
@@ -65,10 +65,10 @@
     keywords="hydroutils",
     name="hydroutils",
     packages=find_packages(include=["hydroutils", "hydroutils.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/OuyangWenyu/hydroutils",
-    version="0.0.1",
+    version='0.0.2',
     zip_safe=False,
 )
```

