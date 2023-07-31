# Comparing `tmp/sourmash_plugin_commonhash-0.2.tar.gz` & `tmp/sourmash_plugin_commonhash-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sourmash_plugin_commonhash-0.2.tar", last modified: Mon Jul 31 13:41:40 2023, max compression
+gzip compressed data, was "sourmash_plugin_commonhash-0.2.1.tar", last modified: Mon Jul 31 13:43:54 2023, max compression
```

## Comparing `sourmash_plugin_commonhash-0.2.tar` & `sourmash_plugin_commonhash-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:41:40.735244 sourmash_plugin_commonhash-0.2/
--rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2/LICENSE
--rw-r--r--   0 t          (502) staff       (20)     1657 2023-07-31 13:41:40.735117 sourmash_plugin_commonhash-0.2/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)     1425 2023-07-31 12:23:50.000000 sourmash_plugin_commonhash-0.2/README.md
--rw-r--r--   0 t          (502) staff       (20)      396 2023-07-31 13:40:37.000000 sourmash_plugin_commonhash-0.2/pyproject.toml
--rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:41:40.735279 sourmash_plugin_commonhash-0.2/setup.cfg
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:41:40.733812 sourmash_plugin_commonhash-0.2/src/
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:41:40.734686 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/
--rw-r--r--   0 t          (502) staff       (20)     1657 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/PKG-INFO
--rw-r--r--   0 t          (502) staff       (20)      422 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/SOURCES.txt
--rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/dependency_links.txt
--rw-r--r--   0 t          (502) staff       (20)       81 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/entry_points.txt
--rw-r--r--   0 t          (502) staff       (20)       19 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/requires.txt
--rw-r--r--   0 t          (502) staff       (20)       27 2023-07-31 13:41:40.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/top_level.txt
--rw-r--r--   0 t          (502) staff       (20)     3705 2023-07-31 12:31:46.000000 sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.py
-drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:41:40.734811 sourmash_plugin_commonhash-0.2/tests/
--rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2/tests/test_sourmash_plugin.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455639 sourmash_plugin_commonhash-0.2.1/
+-rw-r--r--   0 t          (502) staff       (20)     1540 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2.1/LICENSE
+-rw-r--r--   0 t          (502) staff       (20)     1693 2023-07-31 13:43:54.455493 sourmash_plugin_commonhash-0.2.1/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)     1459 2023-07-31 13:42:35.000000 sourmash_plugin_commonhash-0.2.1/README.md
+-rw-r--r--   0 t          (502) staff       (20)      398 2023-07-31 13:42:53.000000 sourmash_plugin_commonhash-0.2.1/pyproject.toml
+-rw-r--r--   0 t          (502) staff       (20)       38 2023-07-31 13:43:54.455684 sourmash_plugin_commonhash-0.2.1/setup.cfg
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.454034 sourmash_plugin_commonhash-0.2.1/src/
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455048 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/
+-rw-r--r--   0 t          (502) staff       (20)     1693 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/PKG-INFO
+-rw-r--r--   0 t          (502) staff       (20)      422 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/SOURCES.txt
+-rw-r--r--   0 t          (502) staff       (20)        1 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/dependency_links.txt
+-rw-r--r--   0 t          (502) staff       (20)       81 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/entry_points.txt
+-rw-r--r--   0 t          (502) staff       (20)       19 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/requires.txt
+-rw-r--r--   0 t          (502) staff       (20)       27 2023-07-31 13:43:54.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/top_level.txt
+-rw-r--r--   0 t          (502) staff       (20)     3705 2023-07-31 12:31:46.000000 sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.py
+drwxr-xr-x   0 t          (502) staff       (20)        0 2023-07-31 13:43:54.455168 sourmash_plugin_commonhash-0.2.1/tests/
+-rw-r--r--   0 t          (502) staff       (20)      446 2023-07-30 11:12:12.000000 sourmash_plugin_commonhash-0.2.1/tests/test_sourmash_plugin.py
```

### Comparing `sourmash_plugin_commonhash-0.2/LICENSE` & `sourmash_plugin_commonhash-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sourmash_plugin_commonhash-0.2/PKG-INFO` & `sourmash_plugin_commonhash-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash_plugin_commonhash
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin to calculate common hashes across multiple sketches.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_commonhash
 
@@ -33,15 +33,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash 
+sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2/README.md` & `sourmash_plugin_commonhash-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash 
+sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.egg-info/PKG-INFO` & `sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sourmash-plugin-commonhash
-Version: 0.2
+Version: 0.2.1
 Summary: sourmash plugin to calculate common hashes across multiple sketches.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sourmash_plugin_commonhash
 
@@ -33,15 +33,15 @@
 commonhash will output one filtered sketch for _each_ input sketch.
 You can then use the various `sourmash sig` commands to union these
 sketches, extract individual ones, etc.
 
 ### Example
 
 ```
-sourmash scripts commonhash 
+sourmash scripts commonhash example/*.sig.gz -o commonhash.zip
 ```
 
 should yield:
 
 ```
 ...
```

### Comparing `sourmash_plugin_commonhash-0.2/src/sourmash_plugin_commonhash.py` & `sourmash_plugin_commonhash-0.2.1/src/sourmash_plugin_commonhash.py`

 * *Files identical despite different names*

