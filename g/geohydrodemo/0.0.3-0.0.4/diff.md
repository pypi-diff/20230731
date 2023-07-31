# Comparing `tmp/geohydrodemo-0.0.3.tar.gz` & `tmp/geohydrodemo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geohydrodemo-0.0.3.tar", last modified: Fri Jul 28 08:50:47 2023, max compression
+gzip compressed data, was "geohydrodemo-0.0.4.tar", last modified: Mon Jul 31 06:04:06 2023, max compression
```

## Comparing `geohydrodemo-0.0.3.tar` & `geohydrodemo-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/geohydrodemo/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/geohydrodemo/geohydrodemo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/geohydrodemo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 08:50:47.000000 geohydrodemo-0.0.3/geohydrodemo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-28 08:50:47.297252 geohydrodemo-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-28 08:50:37.000000 geohydrodemo-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:04:06.704888 geohydrodemo-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 06:04:06.704888 geohydrodemo-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:04:06.700888 geohydrodemo-0.0.4/geohydrodemo/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/geohydrodemo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/geohydrodemo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/geohydrodemo/geohydrodemo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:04:06.700888 geohydrodemo-0.0.4/geohydrodemo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 06:04:06.000000 geohydrodemo-0.0.4/geohydrodemo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 06:04:06.704888 geohydrodemo-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-31 06:03:57.000000 geohydrodemo-0.0.4/setup.py
```

### Comparing `geohydrodemo-0.0.3/LICENSE` & `geohydrodemo-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geohydrodemo-0.0.3/PKG-INFO` & `geohydrodemo-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohydrodemo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for interactive mapping
 Home-page: https://github.com/bojichen/geohydrodemo
 Author: Boji Chen
 Author-email: bojichen@connect.hku.hk
 License: MIT license
 Keywords: geohydrodemo
 Classifier: Intended Audience :: Developers
```

### Comparing `geohydrodemo-0.0.3/geohydrodemo.egg-info/PKG-INFO` & `geohydrodemo-0.0.4/geohydrodemo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geohydrodemo
-Version: 0.0.3
+Version: 0.0.4
 Summary: A python package for interactive mapping
 Home-page: https://github.com/bojichen/geohydrodemo
 Author: Boji Chen
 Author-email: bojichen@connect.hku.hk
 License: MIT license
 Keywords: geohydrodemo
 Classifier: Intended Audience :: Developers
```

### Comparing `geohydrodemo-0.0.3/setup.py` & `geohydrodemo-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='geohydrodemo',
     name='geohydrodemo',
     packages=find_packages(include=['geohydrodemo', 'geohydrodemo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bojichen/geohydrodemo',
-    version='0.0.3',
+    version='0.0.4',
     zip_safe=False,
 )
```

