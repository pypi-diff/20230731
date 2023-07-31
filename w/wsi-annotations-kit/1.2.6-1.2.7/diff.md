# Comparing `tmp/wsi-annotations-kit-1.2.6.tar.gz` & `tmp/wsi-annotations-kit-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.2.6.tar", last modified: Mon Jul 31 18:48:46 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.7.tar", last modified: Mon Jul 31 18:55:26 2023, max compression
```

## Comparing `wsi-annotations-kit-1.2.6.tar` & `wsi-annotations-kit-1.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.6/LICENSE
--rw-rw-rw-   0        0        0      745 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-31 18:48:38.000000 wsi-annotations-kit-1.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21934 2023-07-31 18:48:26.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.7/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 18:55:21.000000 wsi-annotations-kit-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21942 2023-07-31 18:55:15.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.2.6/LICENSE` & `wsi-annotations-kit-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.2.6/PKG-INFO` & `wsi-annotations-kit-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.6
+Version: 1.2.7
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.2.6/setup.py` & `wsi-annotations-kit-1.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.2.6",
+    version="1.2.7",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.2.6/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2.7/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
                         # Checking if this polygon is valid
                         checked_poly = self.check_validity(region_poly)
 
                         # Adding to current annotations if valid
                         if not checked_poly is None:
                             self.annotation.add_shape(
                                 poly = checked_poly,
-                                crs = [0,0],
+                                box_crs = [0,0],
                                 structure = structure,
                                 name = name)
 
         if self.file_ext == 'geojson':
             # Loading initial annotations 
             with open(self.starting_file) as f:
                 geojson_polys = geojson.load(f)
@@ -520,15 +520,15 @@
                     # Probably don't need to check these? 
                     region_poly = Polygon(coordinates)
                     checked_poly = self.check_validity(region_poly)
 
                     if not checked_poly is None:
                         self.annotation.add_shape(
                             poly = checked_poly,
-                            crs = [0,0],
+                            box_crs = [0,0],
                             structure = structure,
                             name = name
                         )
 
         # Closing progress bar
         if self.verbose:
             pbar.close()
```

### Comparing `wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.6
+Version: 1.2.7
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

