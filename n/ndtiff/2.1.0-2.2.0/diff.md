# Comparing `tmp/ndtiff-2.1.0.tar.gz` & `tmp/ndtiff-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndtiff-2.1.0.tar", last modified: Tue Jun  6 20:39:08 2023, max compression
+gzip compressed data, was "ndtiff-2.2.0.tar", last modified: Mon Jul 31 17:12:21 2023, max compression
```

## Comparing `ndtiff-2.1.0.tar` & `ndtiff-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 20:39:08.480429 ndtiff-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 20:38:58.000000 ndtiff-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.476429 ndtiff-2.1.0/ndtiff/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/_superclass.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    42655 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/nd_tiff_current.py
--rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/nd_tiff_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/ndtiff_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/ndtiff/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/data_loading_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-06 20:38:58.000000 ndtiff-2.1.0/ndtiff/test/test_custom_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:39:08.480429 ndtiff-2.1.0/ndtiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 20:39:08.000000 ndtiff-2.1.0/ndtiff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-06 20:38:58.000000 ndtiff-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:39:08.480429 ndtiff-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-06 20:38:58.000000 ndtiff-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-31 17:12:21.884292 ndtiff-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 17:12:07.000000 ndtiff-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/_superclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43626 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/nd_tiff_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28685 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/nd_tiff_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44915 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/ndtiff_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/data_loading_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-07-31 17:12:07.000000 ndtiff-2.2.0/ndtiff/test/test_custom_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:12:21.884292 ndtiff-2.2.0/ndtiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 17:12:21.000000 ndtiff-2.2.0/ndtiff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 17:12:07.000000 ndtiff-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:12:21.884292 ndtiff-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-31 17:12:07.000000 ndtiff-2.2.0/setup.py
```

### Comparing `ndtiff-2.1.0/PKG-INFO` & `ndtiff-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.1.0/ndtiff/_superclass.py` & `ndtiff-2.2.0/ndtiff/_superclass.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff/file_io.py` & `ndtiff-2.2.0/ndtiff/file_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff/nd_tiff_current.py` & `ndtiff-2.2.0/ndtiff/nd_tiff_current.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import numpy as np
 import sys
 import json
 import dask.array as da
 import warnings
 import struct
+from sortedcontainers import SortedSet
 import threading
 from functools import partial
 from ndtiff.file_io import NDTiffFileIO, BUILTIN_FILE_IO
 import time
 
 _POSITION_AXIS = "position"
 _ROW_AXIS = "row"
@@ -220,19 +221,17 @@
         )
 
         self.axes = {}
         self.axes_types = {}
         for axes_combo in self.index.keys():
             for axis, position in axes_combo:
                 if axis not in self.axes.keys():
-                    self.axes[axis] = []
+                    self.axes[axis] = SortedSet()
                     self.axes_types[axis] = type(position)
-                self.axes[axis].append(position)
-                # get sorted unique elements
-                self.axes[axis] = sorted(list(set(self.axes[axis])))
+                self.axes[axis].add(position)
         # Sort axes according to _AXIS_ORDER
         self.axes = dict(sorted(self.axes.items(), key=_get_axis_order_key, reverse=True))
 
         # figure out the mapping of channel name to position by reading image metadata
         self._channels = {}
         self._parse_string_axes()
 
@@ -419,18 +418,17 @@
                 # Should be the same on every file so resetting them is fine
                 self.major_version, self.minor_version = new_reader.major_version, new_reader.minor_version
 
 
             # update the axes that have been seen
             for axis_name in axes.keys():
                 if axis_name not in self.axes.keys():
-                    self.axes[axis_name] = []
+                    self.axes[axis_name] = SortedSet()
                     self.axes_types[axis_name] = type(axes[axis_name])
-                self.axes[axis_name].append(axes[axis_name])
-                self.axes[axis_name] = sorted(list(set(self.axes[axis_name])))
+                self.axes[axis_name].add(axes[axis_name])
 
             # update the map of channel names to channel indices
             self._parse_string_axes(axes)
 
         if not hasattr(self, 'image_width'):
             self._parse_first_index(index_entry)
 
@@ -453,51 +451,67 @@
         for axis_name in axis_positions.keys():
             # convert any string-valued axes passed as ints into strings
             if self.axes_types[axis_name] == str and type(axis_positions[axis_name]) == int:
                 axis_positions[axis_name] = self._string_axes_values[axis_name][axis_positions[axis_name]]
 
         return axis_positions
 
-    def _parse_string_axes(self, axes=None):
+    def _parse_string_axes(self, single_axes_position=None):
         """
         As of NDTiff 3.2, axes are allowed to take string values: e.g. {'channel': 'DAPI'}
         This is allowed on any axis. This function returns a tuple of possible values along
         the string axis in order to be able to interconvert integer values and string values.
 
-        param axes: if not None, only parse the string axis values for the given axes
+        param single_axes_position: if provided, only parse this newly added entry
         """
         # iterate through the key_combos for each image
         if self.major_version >= 3 and self.minor_version >= 2:
-            self._string_axes_values = {axis_name: [] for axis_name in self.axes_types.keys()
-                                        if self.axes_types[axis_name] is str}
-            for key in self.index.keys() if axes is None else [[(key, axes[key]) for key in axes.keys()]]:
-                for axis_name, position in key:
+            # keep track of the values for each axis with string values if not doing so already
+            if not hasattr(self, '_string_axes_values'):
+                self._string_axes_values = {}
+            # if this is a new axis_value for a string axis, add a list to populate
+            for string_axis_name in [axis_name for axis_name in self.axes_types.keys() if self.axes_types[axis_name] is str]:
+                if string_axis_name not in self._string_axes_values.keys():
+                    self._string_axes_values[string_axis_name] = []
+
+            # add new axis values to the list of values that have been seen
+            if single_axes_position is None:
+                # parse all axes_positions in the dataset
+                for single_axes_position in self.index.keys():
+                    # this is a set of tuples of (axis_name, axis_value)
+                    for axis_name, axis_value in single_axes_position:
+                        if axis_name in self._string_axes_values.keys() and \
+                                axis_value not in self._string_axes_values[axis_name]:
+                            self._string_axes_values[axis_name].append(axis_value)
+            else:
+                # parse only this set of axes positions
+                for axis_name, axis_value in single_axes_position.items():
                     if axis_name in self._string_axes_values.keys() and \
-                            position not in self._string_axes_values[axis_name]:
-                        self._string_axes_values[axis_name].append(position)
+                            axis_value not in self._string_axes_values[axis_name]:
+                        self._string_axes_values[axis_name].append(axis_value)
 
             if _CHANNEL_AXIS in self._string_axes_values:
                 self._channels = {name: self._string_axes_values[_CHANNEL_AXIS].index(name)
                                   for name in self._string_axes_values[_CHANNEL_AXIS]}
         else:
             # before string-valued axes were allowed in NDTiff 3.1
             if 'ChNames' in self.summary_metadata:
                 # It was created by a MM MDA/Clojure acquistiion engine
                 self._channels = {name: i for i, name in enumerate(self.summary_metadata['ChNames'])}
             else:
                 # AcqEngJ
                 if _CHANNEL_AXIS in self.axes.keys():
                     for key in self.index.keys():
-                        axes = {axis: position for axis, position in key}
+                        single_axes_position = {axis: position for axis, position in key}
                         if (
-                            _CHANNEL_AXIS in axes.keys()
-                            and axes[_CHANNEL_AXIS] not in self._channels.values()
+                            _CHANNEL_AXIS in single_axes_position.keys()
+                            and single_axes_position[_CHANNEL_AXIS] not in self._channels.values()
                         ):
-                            channel_name = self.read_metadata(**axes)["Channel"]
-                            self._channels[channel_name] = axes[_CHANNEL_AXIS]
+                            channel_name = self.read_metadata(**single_axes_position)["Channel"]
+                            self._channels[channel_name] = single_axes_position[_CHANNEL_AXIS]
                         if len(self._channels.values()) == len(self.axes[_CHANNEL_AXIS]):
                             break
 
 
     def _parse_first_index(self, first_index):
         """
         Read through first index to get some global data about images (assuming it is same for all)
@@ -692,15 +706,15 @@
         )
 
         rgb = self.bytes_per_pixel == 3 and self.dtype == np.uint8
 
         if axes is None:
             axes = self.axes.keys()
         axes_to_slice = kwargs
-        axes_to_stack = {key: self.axes[key] for key in axes if key not in kwargs.keys()}
+        axes_to_stack = {key: list(self.axes[key]) for key in axes if key not in kwargs.keys()}
         if stitched:
             if 'row' in axes_to_stack:
                 del axes_to_stack['row']
             if 'column' in axes_to_stack:
                 del axes_to_stack['column']
             if 'row' in axes_to_slice:
                 del axes_to_slice['row']
```

### Comparing `ndtiff-2.1.0/ndtiff/nd_tiff_v2.py` & `ndtiff-2.2.0/ndtiff/nd_tiff_v2.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff/ndtiff_v1.py` & `ndtiff-2.2.0/ndtiff/ndtiff_v1.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff/test/data_loading_test.py` & `ndtiff-2.2.0/ndtiff/test/data_loading_test.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff/test/test_custom_io.py` & `ndtiff-2.2.0/ndtiff/test/test_custom_io.py`

 * *Files identical despite different names*

### Comparing `ndtiff-2.1.0/ndtiff.egg-info/PKG-INFO` & `ndtiff-2.2.0/ndtiff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndtiff
-Version: 2.1.0
+Version: 2.2.0
 Summary: Python libraries for NDTiff datasets
 Home-page: https://github.com/micro-manager/NDTiffStorage
 Author: Henry Pinkard
 Author-email: henry.pinkard@gmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ndtiff-2.1.0/setup.py` & `ndtiff-2.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 # extract version
 path = path.realpath("ndtiff/_version.py")
 version_ns = {}
 with open(path, encoding="utf8") as f:
     exec(f.read(), {}, version_ns)
 version = version_ns["__version__"]
 
+with open("requirements.txt") as f:
+    requirements = f.read().splitlines()
+
 setuptools.setup(
     name="ndtiff",
     version=version,
     author="Henry Pinkard",
     author_email="henry.pinkard@gmail.com",
     description="Python libraries for NDTiff datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/micro-manager/NDTiffStorage",
     packages=setuptools.find_packages(),
-    install_requires=[
-        "numpy",
-        "dask[array]>=2022.2.0",
-    ],
+    install_requires=requirements,
     python_requires=">=3.6",
     extras_require={
         "test": [
             "pytest",
         ]
     },
     classifiers=[
```

