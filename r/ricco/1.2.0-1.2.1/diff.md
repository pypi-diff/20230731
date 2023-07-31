# Comparing `tmp/ricco-1.2.0.tar.gz` & `tmp/ricco-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricco-1.2.0.tar", last modified: Thu Jul 27 09:11:15 2023, max compression
+gzip compressed data, was "ricco-1.2.1.tar", last modified: Mon Jul 31 09:05:38 2023, max compression
```

## Comparing `ricco-1.2.0.tar` & `ricco-1.2.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.971664 ricco-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 09:11:15.971664 ricco-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-27 09:11:04.000000 ricco-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 09:11:15.971664 ricco-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-27 09:11:04.000000 ricco-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/etl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/geocode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/amap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/baidu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/geocode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geocode/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16678 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/df.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/geometry/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/area_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/city_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/epsg_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/resource/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.971664 ricco-1.2.0/src/ricco/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/address_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/building_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/coord_trans.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/dt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/id_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/topology_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-27 09:11:04.000000 ricco-1.2.0/src/ricco/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 09:11:15.967664 ricco-1.2.0/src/ricco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-27 09:11:15.000000 ricco-1.2.0/src/ricco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.726503 ricco-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-31 09:05:38.726503 ricco-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 09:05:25.000000 ricco-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:05:38.726503 ricco-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-31 09:05:25.000000 ricco-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/ricco/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/ricco/etl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/ricco/geocode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geocode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geocode/amap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geocode/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geocode/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geocode/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/ricco/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geometry/df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/geometry/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.726503 ricco-1.2.1/src/ricco/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   161544 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/area_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15551 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/city_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23330 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/epsg_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/resource/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.726503 ricco-1.2.1/src/ricco/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/building_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/coord_trans.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/dt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/id_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/topology_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13540 2023-07-31 09:05:25.000000 ricco-1.2.1/src/ricco/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:05:38.722503 ricco-1.2.1/src/ricco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-31 09:05:38.000000 ricco-1.2.1/src/ricco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-31 09:05:38.000000 ricco-1.2.1/src/ricco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:05:38.000000 ricco-1.2.1/src/ricco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 09:05:38.000000 ricco-1.2.1/src/ricco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 09:05:38.000000 ricco-1.2.1/src/ricco.egg-info/top_level.txt
```

### Comparing `ricco-1.2.0/PKG-INFO` & `ricco-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.2.0
+Version: 1.2.1
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.2.0/setup.py` & `ricco-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/__init__.py` & `ricco-1.2.1/src/ricco/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.2.0'
+__version__ = '1.2.1'
 
 from .etl import file
 from .etl import load
 from .etl import transformer
 from .etl.extract import rdf
 from .etl.transformer import expand_dict
 from .etl.transformer import table2dict
```

### Comparing `ricco-1.2.0/src/ricco/etl/extract.py` & `ricco-1.2.1/src/ricco/etl/extract.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/etl/file.py` & `ricco-1.2.1/src/ricco/etl/file.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/etl/load.py` & `ricco-1.2.1/src/ricco/etl/load.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/etl/stat.py` & `ricco-1.2.1/src/ricco/etl/stat.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/etl/transformer.py` & `ricco-1.2.1/src/ricco/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/geocode/amap.py` & `ricco-1.2.1/src/ricco/geocode/amap.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/geocode/baidu.py` & `ricco-1.2.1/src/ricco/geocode/baidu.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/geocode/geocode.py` & `ricco-1.2.1/src/ricco/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/geocode/util.py` & `ricco-1.2.1/src/ricco/geocode/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/geometry/__init__.py` & `ricco-1.2.1/src/ricco/geometry/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .df import auto2shapely
 from .df import buffer
+from .df import get_area
 from .df import lnglat2shapely
 from .df import lnglat2wkb
 from .df import lnglat2wkt
 from .df import mark_tags_v2
 from .df import nearest_neighbor
 from .df import projection
 from .df import shapely2lnglat
```

### Comparing `ricco-1.2.0/src/ricco/geometry/df.py` & `ricco-1.2.1/src/ricco/geometry/df.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,67 +26,71 @@
 
 warnings.filterwarnings('ignore', category=ShapelyDeprecationWarning)
 
 
 def projection(
     gdf: gpd.GeoDataFrame,
     epsg: int = None,
-    city: str = None):
+    city: str = None,
+    geometry='geometry'):
   """投影变换"""
   if not epsg:
     epsg = get_epsg(city) if city else get_epsg_by_lng(
-        gdf['geometry'].centroid.x.tolist()
+        gdf[geometry].centroid.x.tolist()
     )
   return gdf.to_crs(epsg=epsg)
 
 
 @geom_progress
 def wkb2shapely(df, geometry='geometry',
                 epsg_code: int = 4326) -> gpd.GeoDataFrame:
   df = df.copy()
   df[geometry] = df[geometry].progress_apply(wkb_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
 @geom_progress
 def shapely2wkb(df, geometry='geometry'):
+  df = df.copy()
   df[geometry] = df[geometry].progress_apply(wkb_dumps)
   return df
 
 
 @geom_progress
 def wkt2shapely(df, geometry='geometry',
                 epsg_code: int = 4326) -> gpd.GeoDataFrame:
+  df = df.copy()
   df[geometry] = df[geometry].progress_apply(wkt_loads)
   return gpd.GeoDataFrame(df, geometry=geometry, crs=epsg_code)
 
 
 @geom_progress
 def shapely2wkt(df, geometry='geometry'):
+  df = df.copy()
   df[geometry] = df[geometry].progress_apply(wkt_dumps)
   return df
 
 
 @geom_progress
 def lnglat2shapely(df,
                    lng='lng',
                    lat='lat',
                    geometry='geometry',
                    delete=True,
                    epsg_code: int = 4326) -> gpd.GeoDataFrame:
   from pandas.errors import SettingWithCopyWarning
   warnings.filterwarnings('ignore', category=SettingWithCopyWarning)
-
+  df = df.copy()
   df[geometry] = df.progress_apply(
       lambda d: Point((d[lng], d[lat]))
       if not_empty(d[lng]) and not_empty(d[lat])
       else None,
       axis=1
   )
-  df = gpd.GeoDataFrame(df, crs=epsg_code)
+  df = gpd.GeoDataFrame(df, crs=epsg_code, geometry=geometry)
   if delete:
     del df[lng], df[lat]
   return df
 
 
 @geom_progress
 def shapely2lnglat(df, geometry='geometry',
@@ -98,14 +102,15 @@
   当为True时，不在面内的中心点将用一个在面内的点代替
   """
 
   def get_xy(x):
     p = get_inner_point(x, within=within)
     return p.centroid.x, p.centroid.y
 
+  df = df.copy()
   df[[lng, lat]] = df[[geometry]].progress_apply(
       lambda r: get_xy(r[geometry]) if r[geometry] else (None, None),
       result_type='expand',
       axis=1
   )
   if delete:
     del df[geometry]
@@ -124,19 +129,17 @@
 def lnglat2wkb(df,
                lng='lng',
                lat='lat',
                geometry='geometry',
                delete=False, code=4326):
   """经纬度转wkb格式的geometry"""
   df = lnglat2shapely(
-      df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
+      df, lng, lat, geometry=geometry, delete=delete, epsg_code=code
   )
   df = shapely2wkb(df, geometry=geometry)
-  if not delete:
-    df = df.rename(columns={'lng': lng, 'lat': lat})
   return df
 
 
 def wkt2lnglat(df, geometry='geometry', delete=False, within=False):
   """geometry转经纬度，求中心点经纬度"""
   df = wkt2shapely(df, geometry=geometry)
   df = shapely2lnglat(df, geometry=geometry, within=within, delete=delete)
@@ -148,19 +151,17 @@
 def lnglat2wkt(df,
                lng='lng',
                lat='lat',
                geometry='geometry',
                delete=False, code=4326):
   """经纬度转wkb格式的geometry"""
   df = lnglat2shapely(
-      df, 'lng', 'lat', geometry=geometry, delete=delete, epsg_code=code
+      df, lng, lat, geometry=geometry, delete=delete, epsg_code=code
   )
   df = shapely2wkt(df, geometry=geometry)
-  if not delete:
-    df = df.rename(columns={'lng': lng, 'lat': lat})
   return df
 
 
 def wkb2wkt(df, geometry='geometry', epsg_code: int = 4326):
   """wkb转wkt"""
   df = wkb2shapely(df, geometry=geometry, epsg_code=epsg_code)
   return shapely2wkt(df, geometry=geometry)
@@ -168,53 +169,70 @@
 
 def wkt2wkb(df, geometry='geometry', epsg_code: int = 4326):
   """wkb转wkt"""
   df = wkt2shapely(df, geometry=geometry, epsg_code=epsg_code)
   return shapely2wkb(df, geometry=geometry)
 
 
+def shapely2central_shapely(df, geometry='geometry', within=False):
+  df = shapely2lnglat(df, geometry=geometry, within=within)
+  return lnglat2shapely(df, geometry=geometry, delete=True)
+
+
 def auto2shapely(df, geometry='geometry'):
-  geom = first_notnull_value(df[geometry])
-  geom_format = infer_geom_format(geom)
+  _geom = first_notnull_value(df[geometry])
+  geom_format = infer_geom_format(_geom)
   if geom_format == 'wkb':
     return wkb2shapely(df, geometry=geometry)
   elif geom_format == 'wkt':
     return wkt2shapely(df, geometry=geometry)
   elif geom_format == 'shapely':
     return gpd.GeoDataFrame(df, geometry=geometry)
   else:
     raise TypeError('未知的地理格式，支持wkb,wkt,shapely三种格式')
 
 
-def shapely2x(df, geometry_format: str):
+def shapely2x(df, geometry_format: str, geometry='geometry'):
   """将shapely转为指定的格式"""
   if geometry_format == 'wkb':
-    return shapely2wkb(df)
+    return shapely2wkb(df, geometry=geometry)
   elif geometry_format == 'wkt':
-    return shapely2wkt(df)
+    return shapely2wkt(df, geometry=geometry)
   elif geometry_format == 'shapely':
     return df
   else:
     raise ValueError('不支持的geometry格式')
 
 
+def auto2x(df, geometry_format: str, geometry='geometry'):
+  """将shapely转为指定的格式"""
+  geom = first_notnull_value(df[geometry])
+  __geom_format = infer_geom_format(geom)
+  if __geom_format == geometry_format:
+    return df
+  df = auto2shapely(df, geometry=geometry)
+  return shapely2x(df, geometry_format=geometry_format, geometry=geometry)
+
+
 def distance_min(geometry, gdf: gpd.GeoDataFrame) -> float:
   """
   计算单个geometry到数据集gdf中元素的最短距离
   Args:
     geometry: 单个geometry，shapely格式
     gdf: 数据集，GeoDataFrame格式
   """
   return gdf.distance(geometry).min()
 
 
 @geom_progress
-def distance_gdf(df: gpd.GeoDataFrame, df_target: gpd.GeoDataFrame, c_dst: str):
+def distance_gdf(df: gpd.GeoDataFrame, df_target: gpd.GeoDataFrame, c_dst: str,
+                 left_geometry='geometry'):
   """计算一个数据集中的每个元素到另一个数据集之间的最短距离"""
-  df[c_dst] = df['geometry'].progress_apply(
+  df = df.copy()
+  df[c_dst] = df[left_geometry].progress_apply(
       lambda p: distance_min(p, df_target) if not_empty(p) else np.nan
   )
   return df
 
 
 def split_grids(df: gpd.GeoDataFrame, step: int, city: str = None):
   """
@@ -306,118 +324,147 @@
                      predicate='intersects').drop('index_right', axis=1)
 
   # 将geometry转为wkb格式
   df_res = shapely2wkb(df_res)
   return df_res
 
 
+def _ensure_geometry(_df,
+                     ensure_point=False,
+                     warning_message=False,
+                     geometry='geometry',
+                     lng='lng', lat='lat'):
+  """转换并仅保留geometry列"""
+  if geometry in _df:
+    _df = auto2shapely(_df[[geometry]], geometry=geometry)[[geometry]]
+    if ensure_point:
+      geom = first_notnull_value(_df[geometry])
+      if geom.geom_type not in ['point', 'Point']:
+        if warning_message:
+          warnings.warn('非点数据，将自动提取中心点')
+        _df = shapely2central_shapely(_df, within=True, geometry=geometry)
+    return _df
+  elif lng in _df and lat in _df:
+    return lnglat2shapely(
+        _df[[lng, lat]],
+        lng=lng, lat=lat,
+        geometry=geometry,
+        delete=False,
+    )[[geometry]]
+  else:
+    raise KeyError(f'文件中必须有"lng"+"lat"列或"{geometry}"列')
+
+
 def mark_tags_v2(
     point_df: pd.DataFrame,
     polygon_df: pd.DataFrame,
     col_list: list = None,
     predicate='intersects',
     drop_geometry=False,
     geometry_format='wkb',
-    warning_message=True):
+    warning_message=True,
+    point_lng='lng',
+    point_lat='lat',
+    point_geometry='geometry',
+    polygon_geometry='geometry',
+):
   """
-  使用面数据通过空间关联（sjoin）给点数据打标签
+  使用面数据通过空间关联（sjoin）给数据打标签
 
   Args:
       point_df: 点数据
       polygon_df: 面数据
       col_list: 面数据中要关联到结果中的列，若为空则全部关联
       predicate: 关联方法，默认'intersects'
       drop_geometry: 结果是否删除geometry，默认删除
       geometry_format: 输出的geometry格式，支持wkb,、wkt、shapely，默认wkb
       warning_message: 是否输出警告信息
   """
+  point_df = point_df.copy()
   if not col_list:
     col_list = polygon_df.columns.to_list()
   else:
     col_list = ensure_list(col_list)
-    polygon_df = polygon_df[[*col_list, 'geometry']]
+    polygon_df = polygon_df[[*col_list, polygon_geometry]]
 
   for c in col_list:
-    if c in point_df and c not in ['lng', 'lat', 'geometry']:
+    if c in point_df and c not in [point_lng, point_lat, point_geometry]:
       c_n = f'{c}_origin'
       if warning_message:
         warnings.warn(f'点数据中存在面文件中待关联的列，已重命名：{c} --> {c_n}')
       point_df.rename(columns={c: c_n}, inplace=True)
-
-  if 'geometry' in point_df:
-    point_df = auto2shapely(point_df)
-    geom = first_notnull_value(point_df['geometry'])
-    if geom.geom_type not in ['point', 'Point']:
-      if warning_message:
-        warnings.warn('左侧数据实际非点数据，将自动提取中心点进行关联')
-      point_df['geometry_backup'] = point_df['geometry']
-      point_df = shapely2lnglat(point_df, within=True)
-      point_df = lnglat2shapely(point_df, delete=False)
-  elif 'lng' in point_df and 'lat' in point_df:
-    point_df = lnglat2shapely(point_df, delete=False)
-  else:
-    raise KeyError('点文件中必须有经纬度或geometry')
-
-  polygon_df = auto2shapely(polygon_df)
-
-  point_df = gpd.sjoin(
-      point_df,
-      polygon_df,
-      how='left',
-      predicate=predicate,
-  ).drop('index_right', axis=1)
-
-  if 'geometry_backup' in point_df:
-    del point_df['geometry']
-    point_df.rename(columns={'geometry_backup': 'geometry'}, inplace=True)
-
-  if drop_geometry:
-    del point_df['geometry']
+  # 转换为shapely格式
+  df = _ensure_geometry(point_df, True, warning_message,
+                        lng=point_lng, lat=point_lat, geometry=point_geometry)
+  polygon_df = auto2shapely(polygon_df, geometry=polygon_geometry)
+  # 空间关联
+  df = df.sjoin(
+      polygon_df, how='left', predicate=predicate,
+  ).drop(['index_right'], axis=1)
+  # 统一geometry输出格式、删除geometry、避免多次转换
+  if point_geometry in point_df:
+    if geometry_format != 'shapely':
+      del df[point_geometry]
+    if geometry_format == 'shapely' or drop_geometry:
+      del point_df[point_geometry]
+    else:
+      point_df = auto2x(point_df, geometry_format, geometry=point_geometry)
+  elif drop_geometry:
+    del df[point_geometry]
   else:
-    point_df = shapely2x(point_df, geometry_format)
-
-  return pd.DataFrame(point_df)
+    df = shapely2x(df, geometry_format, geometry=point_geometry)
+  # 将空间关联后的数据关联到原来的Dataframe上
+  return point_df.join(df, how='left')
 
 
 def nearest_neighbor(
     df: pd.DataFrame,
     df_target: pd.DataFrame,
     c_dst='min_distance',
     epsg: int = None) -> pd.DataFrame:
   """
   近邻分析，计算一个数据集中的元素到另一个数据集中全部元素的最短距离（单位：米）
 
   Args:
     df:
     df_target:
-    c_dst: 输出最短距离的列名
-    epsg: 对于跨时区或不在同一个城市的可以指定epsg code
+    c_dst: 输出最短距离的列名，默认为“min_distance”
+    epsg: 对于跨时区或不在同一个城市的可以指定epsg code，默认会根据经度中位数获取
   """
-
-  def ensure_geometry(_df):
-    if 'geometry' in _df:
-      return auto2shapely(_df[['geometry']])[['geometry']]
-    elif 'lng' in _df and 'lat' in _df:
-      return lnglat2shapely(
-          _df[['lng', 'lat']],
-          delete=False)[['geometry']]
-    else:
-      raise KeyError('文件中必须有经纬度或geometry')
-
   # 将两个数据集都转为shapely格式
-  df_left = ensure_geometry(df)
-  df_target = ensure_geometry(df_target)
+  df_left = _ensure_geometry(df)
+  df_target = _ensure_geometry(df_target)
   # 投影
   df_left = projection(df_left, epsg=epsg)
   df_target = projection(df_target, epsg=epsg)
   # 计算最短距离
   df_left = distance_gdf(df_left, df_target, c_dst)
   # 将距离合并到原来的数据集上
-  df = df.merge(df_left[[c_dst]], left_index=True, right_index=True, how='left')
-  return pd.DataFrame(df).sort_index()
+  return df.join(df_left[[c_dst]], how='left')
+
+
+def get_area(
+    df: pd.DataFrame,
+    c_dst='area',
+    epsg: int = None) -> pd.DataFrame:
+  """
+  计算面积（单位：平方米）
+  Args:
+    df: 要计算的面数据
+    c_dst: 输出面积的列名，默认为“area”
+    epsg: 对于跨时区或不在同一个城市的可以指定epsg code，默认会根据经度中位数获取
+  """
+  # 将数据集转为shapely格式
+  df_left = _ensure_geometry(df)
+  # 投影
+  df_left = projection(df_left, epsg=epsg)
+  # 计算面积
+  df_left[c_dst] = df_left.area
+  # 将面积合并到原来的数据集上
+  return df.join(df_left[[c_dst]], how='left')
 
 
 def buffer(df: pd.DataFrame, radius: Union[int, float],
            city: str = None,
            geo_type: str = 'point',
            geometry: str = 'geometry',
            buffer_geometry: str = 'buffer_geometry',
@@ -450,48 +497,30 @@
     >>> buffer(df=df, radius=1500, city='北京', geo_type='point')
         id        lng       lat                                    buffer_geometry
     0   1  116.18601  40.02894  0103000020E6100000010000004100000092A0207A070D...
     1   2  116.18366  40.03550  0103000020E6100000010000004100000071178800E10C...
     2   3  116.18529  40.03565  0103000020E610000001000000410000008A2570B5FB0C...
 
   """
-  df = df.reset_index(drop=True)
-  cols = []
-  if geometry in df:
-    cols.append(geometry)
-  if 'lng' in df and 'lat' in df:
-    cols.extend(['lng', 'lat'])
-  df_tmp = df[cols]
-  df_tmp.rename(columns={geometry: 'geometry'}, inplace=True)
-
+  df = df.copy()
   if geo_type == 'point':
-    if 'geometry' in df_tmp:
-      df_tmp = auto2shapely(df_tmp)
-      geom = first_notnull_value(df_tmp['geometry'])
-      if geom.geom_type not in ['point', 'Point']:
-        warnings.warn('数据实际非点数据，将自动提取中心点进行关联')
-        df_tmp = shapely2lnglat(df_tmp)
-        df_tmp = lnglat2shapely(df_tmp, delete=False)
-    elif 'lng' in df_tmp and 'lat' in df_tmp:
-      df_tmp = lnglat2shapely(df_tmp, delete=False)
-    else:
-      raise KeyError('点文件中必须有经纬度或geometry')
-  elif geo_type == 'line' or geo_type == 'polygon':
-    df_tmp = auto2shapely(df_tmp, geometry=geometry)
+    df_buffer = _ensure_geometry(df, True)
+  elif geo_type in ['line', 'polygon']:
+    df_buffer = auto2shapely(df, geometry=geometry)[[geometry]]
   else:
     raise ValueError('geo_type必须为point，line或polygon')
 
-  df_buffer = df_tmp[['geometry']]
   df_buffer = projection(df_buffer, city=city)
-  df_buffer['geometry'] = df_buffer.geometry.buffer(radius)
-  df_buffer = projection(df_buffer, epsg=4326)
+  df_buffer[buffer_geometry] = df_buffer.buffer(radius)
+  df_buffer = gpd.GeoDataFrame(
+      df_buffer[[buffer_geometry]], geometry=buffer_geometry
+  )
+  df_buffer = projection(df_buffer, epsg=4326, geometry=buffer_geometry)
   df_buffer = shapely2x(df_buffer, geo_format)
-  df_buffer.rename(columns={'geometry': buffer_geometry}, inplace=True)
-  df = df.join(df_buffer, how='left')
-  return df
+  return df.join(df_buffer, how='left')
 
 
 def spatial_agg(point_df: pd.DataFrame, polygon_df: pd.DataFrame,
                 by: Union[str, List[str]],
                 agg: dict,
                 polygon_geometry: str = 'geometry') -> pd.DataFrame:
   """
@@ -502,14 +531,12 @@
     by: Union[str, List[str]], 空间统计单位字段；
     agg: dict, 空间统计操作。格式为{'被统计字段名': '操作名', ...}的字典。如{'poi':'sum'};
     polygon_geometry: str, 面数据geometry字段名，默认"geometry";
 
   Returns: pd.DataFrame, 包含空间统计单位字段和被统计字段和面数据geometry的DataFrame
   """
 
-  polygon_df.rename({polygon_geometry: 'geometry'}, inplace=True)
-  polygon_df = polygon_df[[by, 'geometry']]
+  polygon_df = polygon_df[[by, polygon_geometry]]
   point_df = mark_tags_v2(polygon_df=polygon_df, point_df=point_df,
-                          drop_geometry=True)
+                          drop_geometry=True, polygon_geometry=polygon_geometry)
   df_grouped = point_df.groupby(by=by, as_index=False).agg(agg)
-
   return df_grouped
```

### Comparing `ricco-1.2.0/src/ricco/geometry/util.py` & `ricco-1.2.1/src/ricco/geometry/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/local.py` & `ricco-1.2.1/src/ricco/local.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/resource/area_code.py` & `ricco-1.2.1/src/ricco/resource/area_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/resource/city_id.py` & `ricco-1.2.1/src/ricco/resource/city_id.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/resource/epsg_code.py` & `ricco-1.2.1/src/ricco/resource/epsg_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/resource/names.py` & `ricco-1.2.1/src/ricco/resource/names.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/resource/phone_number.py` & `ricco-1.2.1/src/ricco/resource/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/address_tools.py` & `ricco-1.2.1/src/ricco/util/address_tools.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/assertion.py` & `ricco-1.2.1/src/ricco/util/assertion.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/building_address.py` & `ricco-1.2.1/src/ricco/util/building_address.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/coord_trans.py` & `ricco-1.2.1/src/ricco/util/coord_trans.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/decorator.py` & `ricco-1.2.1/src/ricco/util/decorator.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/docx.py` & `ricco-1.2.1/src/ricco/util/docx.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/dt.py` & `ricco-1.2.1/src/ricco/util/dt.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/geom.py` & `ricco-1.2.1/src/ricco/util/geom.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/id_number.py` & `ricco-1.2.1/src/ricco/util/id_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/os.py` & `ricco-1.2.1/src/ricco/util/os.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import logging
 import os
 import zipfile
+
 from .util import ensure_list
 
 
 def ext(filepath):
   """扩展名"""
   return os.path.splitext(filepath)[1]
 
@@ -101,17 +102,15 @@
 
 def dir_iter(root, exts: (list, str) = None, abspath=False):
   """
   文件夹中的文件路径生成器，用于遍历文件夹中的文件
   Args:
     root: 文件目录
     exts: 文件扩展名，不指定则返回所有文件
-
-  Returns:
-
+    abspath: 是否返回绝对路径
   """
 
   for filename in os.listdir(root):
     filepath = os.path.join(root, filename)
     if abspath:
       filepath = os.path.abspath(filepath)
     if exts:
```

### Comparing `ricco-1.2.0/src/ricco/util/phone_number.py` & `ricco-1.2.1/src/ricco/util/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/strings.py` & `ricco-1.2.1/src/ricco/util/strings.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/topology_check.py` & `ricco-1.2.1/src/ricco/util/topology_check.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco/util/util.py` & `ricco-1.2.1/src/ricco/util/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.2.0/src/ricco.egg-info/PKG-INFO` & `ricco-1.2.1/src/ricco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.2.0
+Version: 1.2.1
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ricco-1.2.0/src/ricco.egg-info/SOURCES.txt` & `ricco-1.2.1/src/ricco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

