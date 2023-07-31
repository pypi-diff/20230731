# Comparing `tmp/tortoise_api_model-0.0.7.tar.gz` & `tmp/tortoise_api_model-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_api_model-0.0.7.tar", last modified: Mon Jul 31 08:43:23 2023, max compression
+gzip compressed data, was "tortoise_api_model-0.1.0.tar", last modified: Mon Jul 31 11:47:54 2023, max compression
```

## Comparing `tortoise_api_model-0.0.7.tar` & `tortoise_api_model-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.155046 tortoise_api_model-0.0.7/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 08:43:23.154822 tortoise_api_model-0.0.7/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 08:43:23.155107 tortoise_api_model-0.0.7/setup.cfg
--rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-31 08:43:02.000000 tortoise_api_model-0.0.7/setup.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.153413 tortoise_api_model-0.0.7/tortoise_api_model/
--rw-r--r--   0 sol        (501) staff       (20)       90 2023-07-30 17:17:05.000000 tortoise_api_model-0.0.7/tortoise_api_model/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     1595 2023-07-30 20:10:46.000000 tortoise_api_model-0.0.7/tortoise_api_model/model.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 08:43:23.154549 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-31 08:43:23.000000 tortoise_api_model-0.0.7/tortoise_api_model.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.118318 tortoise_api_model-0.1.0/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 11:47:54.118059 tortoise_api_model-0.1.0/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-31 11:47:54.118383 tortoise_api_model-0.1.0/setup.cfg
+-rw-r--r--   0 sol        (501) staff       (20)      819 2023-07-31 11:46:49.000000 tortoise_api_model-0.1.0/setup.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.116377 tortoise_api_model-0.1.0/tortoise_api_model/
+-rw-r--r--   0 sol        (501) staff       (20)       90 2023-07-30 17:17:05.000000 tortoise_api_model-0.1.0/tortoise_api_model/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     1821 2023-07-31 11:47:20.000000 tortoise_api_model-0.1.0/tortoise_api_model/model.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-31 11:47:54.117770 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      486 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      276 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       19 2023-07-31 11:47:54.000000 tortoise_api_model-0.1.0/tortoise_api_model.egg-info/top_level.txt
```

### Comparing `tortoise_api_model-0.0.7/setup.py` & `tortoise_api_model-0.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.7'
+VERSION = '0.1.0'
 DESCRIPTION = 'Base model for tortoise-api'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="tortoise_api_model",
     version=VERSION,
```

### Comparing `tortoise_api_model-0.0.7/tortoise_api_model/model.py` & `tortoise_api_model-0.1.0/tortoise_api_model/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,14 +42,20 @@
     field_type = Range
     labels = ("from", "to")
 
     def __new__(cls, precision: int = 0, *args, **kwargs):
         cls.SQL_TYPE = "numrange" if precision else "int4range"
         return super().__new__(cls)
 
+    def to_python_value(self, value):
+        if value is not None and not isinstance(value, self.field_type):
+            value = self.field_type(*[float(v) for v in value])
+        self.validate(value)
+        return value
+
 class PointField(CollectionField[Point]):
     SQL_TYPE = "POINT"
     field_type = Point
     base_field = FloatField
     labels = ("lat", "lon")
 
 class PolygonField(ListField[Polygon]):
```

