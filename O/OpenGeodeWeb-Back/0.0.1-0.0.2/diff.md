# Comparing `tmp/opengeodeweb_back-0.0.1.tar.gz` & `tmp/OpenGeodeWeb-Back-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "OpenGeodeWeb-Back-0.0.2.tar", last modified: Mon Jul 31 10:09:32 2023, max compression
```

## Comparing `opengeodeweb_back-0.0.1.tar` & `OpenGeodeWeb-Back-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/requirements.in
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/requirements.txt
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/.github/workflows/Branch-protection.yml
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/.github/workflows/CD.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/src/OpenGeodeWeb-Back/__init__.py
--rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/src/OpenGeodeWeb-Back/geode_functions.py
--rw-r--r--   0        0        0    14018 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/src/OpenGeodeWeb-Back/geode_objects.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/LICENSE
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/README.md
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 opengeodeweb_back-0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.228092 OpenGeodeWeb-Back-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.228092 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7295 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14018 2023-07-31 10:09:22.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:09:32.232092 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 10:09:32.000000 OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb_Back.egg-info/top_level.txt
```

### Comparing `opengeodeweb_back-0.0.1/src/OpenGeodeWeb-Back/geode_functions.py` & `OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -144,26 +144,37 @@
     return geode_objects.objects_list()[geode_object]["builder"](data)
 
 
 def load(file_path):
     return geode_objects.objects_list()[geode_object]["load"](file_path)
 
 
-def save(data, geode_object, id, filename):
+def save(data, geode_object, folder, filename):
     geode_objects.objects_list()[geode_object]["save"](
-        data, os.path.join(UPLOAD_FOLDER, filename)
+        data, os.path.join(folder, filename)
     )
 
 
-def save_viewable(data, geode_object, id):
+def save_viewable(data, geode_object, folder, id):
     geode_objects.objects_list()[geode_object]["save_viewable"](
-        data, os.path.join(UPLOAD_FOLDER, id)
+        data, os.path.join(folder, id)
     )
 
 
+def get_form_variables(form, variables_array):
+    variables_dict = {}
+
+    for variable in variables_array:
+        if form.get(variable) is None:
+            flask.abort(400, f"No {variable} sent")
+        else:
+            variables_dict[variable] = form.get(variable)
+    return variables_dict
+
+
 def get_geographic_coordinate_systems(geode_object):
     if is_3D(geode_object):
         return og_gs.GeographicCoordinateSystem3D.geographic_coordinate_systems()
     else:
         return og_gs.GeographicCoordinateSystem2D.geographic_coordinate_systems()
```

### Comparing `opengeodeweb_back-0.0.1/src/OpenGeodeWeb-Back/geode_objects.py` & `OpenGeodeWeb-Back-0.0.2/src/OpenGeodeWeb-Back/geode_objects.py`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-0.0.1/LICENSE` & `OpenGeodeWeb-Back-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opengeodeweb_back-0.0.1/README.md` & `OpenGeodeWeb-Back-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,24 @@
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
   <img src="https://codecov.io/gh/Geode-solutions/OpenGeodeWeb-Back/branch/master/graph/badge.svg" alt="Coverage Status">
   <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeodeWeb-Back.svg" alt="Version">
   <img src="https://img.shields.io/pypi/v/opengeode-core" alt="PyPI" >
 </p>
 
 <p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/Python-3-blue.svg" alt="Language">
   <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
   <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
 </p>
 
 ---
 
 ## Introduction
 
-OpenGeodeWeb-Back is an open source framework that proposes handy functions and wrappers for the OpenGeode ecosystem
+OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 
 
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeodeWeb-Back/releases).
 
 
 ## License
```

### Comparing `opengeodeweb_back-0.0.1/PKG-INFO` & `OpenGeodeWeb-Back-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 0.0.1
-Summary: Open source library of python functions and OpenGeode wrappers
+Version: 0.0.2
+Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
+Author-email: Geode-solutions <contact@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
-Author-email: Geode-solutions <contact@geode-solutions.com>
-License-File: LICENSE
+Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
   <img src="https://codecov.io/gh/Geode-solutions/OpenGeodeWeb-Back/branch/master/graph/badge.svg" alt="Coverage Status">
   <img src="https://img.shields.io/github/release/Geode-solutions/OpenGeodeWeb-Back.svg" alt="Version">
   <img src="https://img.shields.io/pypi/v/opengeode-core" alt="PyPI" >
 </p>
 
 <p align="center">
-  <img src="https://img.shields.io/badge/C%2B%2B-11-blue.svg" alt="Language">
+  <img src="https://img.shields.io/badge/Python-3-blue.svg" alt="Language">
   <img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License">
   <img src="https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg" alt="Semantic-release">
 </p>
 
 ---
 
 ## Introduction
 
-OpenGeodeWeb-Back is an open source framework that proposes handy functions and wrappers for the OpenGeode ecosystem
+OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 
 
 ## Changelog
 Detailed changes for each release are documented in the [release notes](https://github.com/Geode-solutions/OpenGeodeWeb-Back/releases).
 
 
 ## License
```

