# Comparing `tmp/aeronet_vector-0.1.0.tar.gz` & `tmp/aeronet_vector-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeronet_vector-0.1.0.tar", last modified: Mon Jul 31 11:07:07 2023, max compression
+gzip compressed data, was "aeronet_vector-0.1.0a1.tar", last modified: Mon Jul 24 09:42:51 2023, max compression
```

## Comparing `aeronet_vector-0.1.0.tar` & `aeronet_vector-0.1.0a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-31 11:07:07.436089 aeronet_vector-0.1.0/
--rw-r--r--   0 trekin     (501) staff       (20)      678 2023-07-31 11:07:07.435609 aeronet_vector-0.1.0/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)     2371 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/README.rst
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-31 11:07:07.433550 aeronet_vector-0.1.0/aeronet_vector/
--rw-r--r--   0 trekin     (501) staff       (20)       78 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/aeronet_vector/__init__.py
--rw-r--r--   0 trekin     (501) staff       (20)       63 2023-07-31 11:03:03.000000 aeronet_vector-0.1.0/aeronet_vector/__version__.py
--rw-r--r--   0 trekin     (501) staff       (20)     4168 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/aeronet_vector/feature.py
--rw-r--r--   0 trekin     (501) staff       (20)     8364 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/aeronet_vector/featurecollection.py
--rw-r--r--   0 trekin     (501) staff       (20)     1009 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/aeronet_vector/merge.py
--rw-r--r--   0 trekin     (501) staff       (20)      486 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/aeronet_vector/utils.py
-drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-31 11:07:07.435108 aeronet_vector-0.1.0/aeronet_vector.egg-info/
--rw-r--r--   0 trekin     (501) staff       (20)      678 2023-07-31 11:07:07.000000 aeronet_vector-0.1.0/aeronet_vector.egg-info/PKG-INFO
--rw-r--r--   0 trekin     (501) staff       (20)      375 2023-07-31 11:07:07.000000 aeronet_vector-0.1.0/aeronet_vector.egg-info/SOURCES.txt
--rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-31 11:07:07.000000 aeronet_vector-0.1.0/aeronet_vector.egg-info/dependency_links.txt
--rw-r--r--   0 trekin     (501) staff       (20)       77 2023-07-31 11:07:07.000000 aeronet_vector-0.1.0/aeronet_vector.egg-info/requires.txt
--rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-31 11:07:07.000000 aeronet_vector-0.1.0/aeronet_vector.egg-info/top_level.txt
--rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-31 11:07:07.436217 aeronet_vector-0.1.0/setup.cfg
--rw-r--r--   0 trekin     (501) staff       (20)     3780 2023-07-31 11:02:03.000000 aeronet_vector-0.1.0/setup.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.763417 aeronet_vector-0.1.0a1/
+-rw-r--r--   0 trekin     (501) staff       (20)      680 2023-07-24 09:42:51.762643 aeronet_vector-0.1.0a1/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)     2371 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/README.rst
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.757223 aeronet_vector-0.1.0a1/aeronet_vector/
+-rw-r--r--   0 trekin     (501) staff       (20)       78 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/__init__.py
+-rw-r--r--   0 trekin     (501) staff       (20)       69 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/__version__.py
+-rw-r--r--   0 trekin     (501) staff       (20)     4168 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/feature.py
+-rw-r--r--   0 trekin     (501) staff       (20)     8364 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/featurecollection.py
+-rw-r--r--   0 trekin     (501) staff       (20)     1009 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/merge.py
+-rw-r--r--   0 trekin     (501) staff       (20)      486 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/aeronet_vector/utils.py
+drwxr-xr-x   0 trekin     (501) staff       (20)        0 2023-07-24 09:42:51.759914 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/
+-rw-r--r--   0 trekin     (501) staff       (20)      680 2023-07-24 09:42:51.000000 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/PKG-INFO
+-rw-r--r--   0 trekin     (501) staff       (20)      375 2023-07-24 09:42:51.000000 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/SOURCES.txt
+-rw-r--r--   0 trekin     (501) staff       (20)        1 2023-07-24 09:42:51.000000 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/dependency_links.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       77 2023-07-24 09:42:51.000000 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/requires.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       15 2023-07-24 09:42:51.000000 aeronet_vector-0.1.0a1/aeronet_vector.egg-info/top_level.txt
+-rw-r--r--   0 trekin     (501) staff       (20)       38 2023-07-24 09:42:51.763673 aeronet_vector-0.1.0a1/setup.cfg
+-rw-r--r--   0 trekin     (501) staff       (20)     3780 2023-07-21 05:30:39.000000 aeronet_vector-0.1.0a1/setup.py
```

### Comparing `aeronet_vector-0.1.0/PKG-INFO` & `aeronet_vector-0.1.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet_vector
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: Vector operations for aeronetlib. Based on shapely + r-tree indexing
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_vector-0.1.0/README.rst` & `aeronet_vector-0.1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.1.0/aeronet_vector/feature.py` & `aeronet_vector-0.1.0a1/aeronet_vector/feature.py`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.1.0/aeronet_vector/featurecollection.py` & `aeronet_vector-0.1.0a1/aeronet_vector/featurecollection.py`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.1.0/aeronet_vector/merge.py` & `aeronet_vector-0.1.0a1/aeronet_vector/merge.py`

 * *Files identical despite different names*

### Comparing `aeronet_vector-0.1.0/aeronet_vector.egg-info/PKG-INFO` & `aeronet_vector-0.1.0a1/aeronet_vector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeronet-vector
-Version: 0.1.0
+Version: 0.1.0a1
 Summary: Vector operations for aeronetlib. Based on shapely + r-tree indexing
 Home-page: 
 Author: Geoalert
 Author-email: hello@geoalert.io
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `aeronet_vector-0.1.0/setup.py` & `aeronet_vector-0.1.0a1/setup.py`

 * *Files identical despite different names*

