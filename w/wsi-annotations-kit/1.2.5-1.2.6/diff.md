# Comparing `tmp/wsi-annotations-kit-1.2.5.tar.gz` & `tmp/wsi-annotations-kit-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.2.5.tar", last modified: Mon Jul 31 18:29:39 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.6.tar", last modified: Mon Jul 31 18:48:46 2023, max compression
```

## Comparing `wsi-annotations-kit-1.2.5.tar` & `wsi-annotations-kit-1.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.5/LICENSE
--rw-rw-rw-   0        0        0      745 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-07-31 18:28:41.000000 wsi-annotations-kit-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21935 2023-07-31 18:28:29.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-31 18:29:39.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-31 18:29:38.000000 wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-07-31 18:48:38.000000 wsi-annotations-kit-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21934 2023-07-31 18:48:26.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-31 18:48:46.000000 wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.2.5/LICENSE` & `wsi-annotations-kit-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.2.5/PKG-INFO` & `wsi-annotations-kit-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.5
+Version: 1.2.6
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.2.5/setup.py` & `wsi-annotations-kit-1.2.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.2.5",
+    version="1.2.6",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.2.5/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2.6/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
                 pbar = tqdm(list(self.ann_dict.keys()))
 
             # Add MPP here if there is one
 
             tree = ET.parse(self.starting_file)
             for idx, structure in enumerate(self.ann_dict):
 
-                structures_in_xml = tree.getroot().findall(f'Annotations[@Id="{str(self.ann_dict[structure])}"]/Regions/Region')
+                structures_in_xml = tree.getroot().findall(f'Annotation[@Id="{str(self.ann_dict[structure])}"]/Regions/Region')
 
                 if self.verbose:
                     pbar.update(idx)
                     pbar.set_description(f'Working on: {structure}: {len(structures_in_xml)} found')
                 
                 for struct_idx,region in enumerate(structures_in_xml):
                     vertices = region.findall('./Vertices/Vertex')
```

### Comparing `wsi-annotations-kit-1.2.5/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2.6/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.2.5
+Version: 1.2.6
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

