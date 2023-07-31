# Comparing `tmp/sldc-cytomine-2.2.0.tar.gz` & `tmp/sldc-cytomine-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sldc-cytomine-2.2.0.tar", last modified: Fri Nov 18 10:24:52 2022, max compression
+gzip compressed data, was "sldc-cytomine-2.3.0.tar", last modified: Mon Jul 31 16:47:06 2023, max compression
```

## Comparing `sldc-cytomine-2.2.0.tar` & `sldc-cytomine-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 10:24:52.424911 sldc-cytomine-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-18 10:24:52.424911 sldc-cytomine-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 10:24:52.424911 sldc-cytomine-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 10:24:52.420911 sldc-cytomine-2.2.0/sldc_cytomine/
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (121)     6048 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/dump.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     7927 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/tile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5925 2022-11-18 10:24:37.000000 sldc-cytomine-2.2.0/sldc_cytomine/tile_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 10:24:52.424911 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-11-18 10:24:52.000000 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-11-18 10:24:52.000000 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 10:24:52.000000 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-18 10:24:52.000000 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-18 10:24:52.000000 sldc-cytomine-2.2.0/sldc_cytomine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:47:06.089528 sldc-cytomine-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 16:47:06.089528 sldc-cytomine-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:47:06.089528 sldc-cytomine-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:47:06.089528 sldc-cytomine-2.3.0/sldc_cytomine/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-07-31 16:46:56.000000 sldc-cytomine-2.3.0/sldc_cytomine/tile_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:47:06.089528 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-31 16:47:06.000000 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-31 16:47:06.000000 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:47:06.000000 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 16:47:06.000000 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 16:47:06.000000 sldc-cytomine-2.3.0/sldc_cytomine.egg-info/top_level.txt
```

### Comparing `sldc-cytomine-2.2.0/PKG-INFO` & `sldc-cytomine-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sldc-cytomine
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cytomine-SLDC, a SLDC binding to Cytomine
 Home-page: https://github.com/waliens/sldc
 Author: Romain Mormont
 Author-email: romain.mormont@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

### Comparing `sldc-cytomine-2.2.0/setup.py` & `sldc-cytomine-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "v2.2.0"
+__version__ = "v2.3.0"
 
 setup(
     name="sldc-cytomine",
     version=__version__,
     description="Cytomine-SLDC, a SLDC binding to Cytomine",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine/autodetect.py` & `sldc-cytomine-2.3.0/sldc_cytomine/autodetect.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine/dump.py` & `sldc-cytomine-2.3.0/sldc_cytomine/dump.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine/image.py` & `sldc-cytomine-2.3.0/sldc_cytomine/image.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine/tile.py` & `sldc-cytomine-2.3.0/sldc_cytomine/tile.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,17 @@
   def np_image(self):
     try:
       if not os.path.exists(self.cache_filepath) and not self.download_tile_image():
         raise TileExtractionException("Cannot fetch tile at for '{}'.".format(self.cache_filename))
 
       np_array = imread(self.cache_filepath)
 
-      if np_array.shape[:2] != (self.height, self.width) or  np_array.shape[2] != self.base_image.channels:
-        raise TileExtractionException("Fetched image has invalid size : {} instead "
-                                      "of {}".format(np_array.shape, (self.width, self.height, self.channels)))
+      # if np_array.shape[:2] != (self.height, self.width) or  np_array.shape[2] != self.base_image.channels:
+      #   raise TileExtractionException("Fetched image has invalid size : {} instead "
+      #                                 "of {}".format(np_array.shape, (self.width, self.height, self.channels)))
 
       if np_array.shape[2] == 4:
         np_array = np_array[:, :, 3]
       np_array = np_array.astype("uint8")
       return self.add_polygon_mask(np_array)
     except IOError as e:
       raise TileExtractionException(str(e))
@@ -89,14 +89,34 @@
       "fif": _slice.path,
       "mimeType": _slice.mime,
       "tileIndex": iip_tile_index,
       "z": slide.api_zoom_level
     })
 
 
+class CytominePimsTile(CytomineDownloadableTile):
+  """Tile fetch using the Zoomify protocol (for older Cytomine versions)"""
+  def download_tile_image(self):
+    slide = self.base_image
+    if not isinstance(slide, CytomineSlide):
+      raise TypeError(f"CytominePims tile should be used in conjunction with CytomineSlide only (as base image), found `{type(slide)}`")
+    iip_topology = TileTopology(slide, None, max_width=256, max_height=256, overlap=0)
+    col_tile = self.abs_offset_x // 256
+    row_tile = self.abs_offset_y // 256
+    tile_index = col_tile + row_tile * iip_topology.tile_horizontal_count
+    _slice = slide.slice_instance
+    zoom = self.base_image.image_instance.zoom - slide.zoom_level
+    return Cytomine.get_instance().download_file(f"{_slice.imageServerUrl}/image/{_slice.path}/normalized-tile/zoom/{zoom}/ti/{tile_index}.jpg", self.cache_filepath, False, payload={
+      "z_slices": "0",
+      "timepoints": "0",
+      "channels": "0,1,2",
+      "colormaps": "#f00,#0f0,#00f",
+    })
+
+
 class CytomineWindowTile(CytomineDownloadableTile):
   """Tiling using the window service"""
   def download_tile_image(self):
     return self.base_image.image_instance.window(
       x=self.abs_offset_x,
       y=self.abs_offset_y,
       w=self.width,
```

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine/tile_builder.py` & `sldc-cytomine-2.3.0/sldc_cytomine/tile_builder.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.2.0/sldc_cytomine.egg-info/PKG-INFO` & `sldc-cytomine-2.3.0/sldc_cytomine.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sldc-cytomine
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cytomine-SLDC, a SLDC binding to Cytomine
 Home-page: https://github.com/waliens/sldc
 Author: Romain Mormont
 Author-email: romain.mormont@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

