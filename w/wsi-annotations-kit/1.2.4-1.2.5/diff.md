# Comparing `tmp/wsi-annotations-kit-1.2.4.tar.gz` & `tmp/wsi-annotations-kit-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.2.4.tar", last modified: Thu Jul 13 16:49:13 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.5.tar", last modified: Mon Jul 31 18:29:39 2023, max compression
```

## Comparing `wsi-annotations-kit-1.2.4.tar` & `wsi-annotations-kit-1.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.4/LICENSE
--rw-rw-rw-   0        0        0      745 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-13 16:49:08.000000 wsi-annotations-kit-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21953 2023-07-13 16:49:01.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-07-13 16:49:12.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-13 16:49:13.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 16:49:12.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-13 16:49:12.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-13 16:49:12.000000 wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 18:28:41.000000 wsi-annotations-kit-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21935 2023-07-31 18:28:29.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.2.4/LICENSE` & `wsi-annotations-kit-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.2.4/PKG-INFO` & `wsi-annotations-kit-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.4
+Version: 1.2.5
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.2.4/setup.py` & `wsi-annotations-kit-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.2.4",
+    version="1.2.5",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.2.4/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2.5/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
 
         self.invalid_count = 0
 
         # ann_dict = dictionary like {'structure_name':id} 
         # where id can either be layer id for aperio, index for json, or the property key that has the structure name for geojson
         self.ann_dict = ann_dict
 
-        self.annotation = self.ingest_annotations()
+        self.ingest_annotations()
 
     def ingest_annotations(self):
 
         self.annotation = Annotation()
         self.annotation.add_names(list(self.ann_dict.keys()))
 
         if self.file_ext=='xml':
```

### Comparing `wsi-annotations-kit-1.2.4/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.4
+Version: 1.2.5
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

