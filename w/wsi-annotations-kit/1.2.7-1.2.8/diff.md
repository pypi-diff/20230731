# Comparing `tmp/wsi-annotations-kit-1.2.7.tar.gz` & `tmp/wsi-annotations-kit-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.2.7.tar", last modified: Mon Jul 31 18:55:26 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.8.tar", last modified: Mon Jul 31 19:06:16 2023, max compression
```

## Comparing `wsi-annotations-kit-1.2.7.tar` & `wsi-annotations-kit-1.2.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.7/LICENSE
--rw-rw-rw-   0        0        0      745 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.7/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-31 18:55:21.000000 wsi-annotations-kit-1.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21942 2023-07-31 18:55:15.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:55:26.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-31 18:55:25.000000 wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.8/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 19:06:09.000000 wsi-annotations-kit-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    22020 2023-07-31 19:05:59.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-07-31 19:06:15.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-31 19:06:16.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 19:06:15.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-31 19:06:15.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-31 19:06:15.000000 wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.2.7/LICENSE` & `wsi-annotations-kit-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.2.7/PKG-INFO` & `wsi-annotations-kit-1.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.7
+Version: 1.2.8
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.2.7/setup.py` & `wsi-annotations-kit-1.2.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.2.7",
+    version="1.2.8",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.2.7/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2.8/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,21 +423,21 @@
 
                 if self.verbose:
                     pbar.update(idx)
                     pbar.set_description(f'Working on: {structure}: {len(structures_in_xml)} found')
                 
                 for struct_idx,region in enumerate(structures_in_xml):
                     vertices = region.findall('./Vertices/Vertex')
-
+                    print(len(vertices))
                     coords = []
                     for vert in vertices:
                         pixel_coords = (np.float32(vert.attrib['X']),np.float32(vert.attrib['Y']))
 
                         coords.append(pixel_coords)
-
+                    print(len(coords))
                     if len(coords)>2:
                         if 'Text' in region.attrib:
                             if not region.attrib['Text']=='':
                                 name = region.attrib['Text']
                             else:
                                 name = None
                         else:
```

### Comparing `wsi-annotations-kit-1.2.7/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2.8/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.7
+Version: 1.2.8
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

