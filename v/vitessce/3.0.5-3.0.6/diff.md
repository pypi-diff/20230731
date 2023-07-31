# Comparing `tmp/vitessce-3.0.5.tar.gz` & `tmp/vitessce-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vitessce-3.0.5.tar", last modified: Tue Jul 11 20:49:38 2023, max compression
+gzip compressed data, was "vitessce-3.0.6.tar", last modified: Mon Jul 31 12:47:03 2023, max compression
```

## Comparing `vitessce-3.0.5.tar` & `vitessce-3.0.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.423904 vitessce-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 20:47:35.000000 vitessce-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 20:47:35.000000 vitessce-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-11 20:49:38.423904 vitessce-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-11 20:47:35.000000 vitessce-3.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-11 20:47:35.000000 vitessce-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-11 20:49:38.423904 vitessce-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:47:35.000000 vitessce-3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.419904 vitessce-3.0.5/vitessce/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50062 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.423904 vitessce-3.0.5/vitessce/data_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/multivec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/data_utils/ome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-11 20:47:35.000000 vitessce-3.0.5/vitessce/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:49:38.419904 vitessce-3.0.5/vitessce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7874 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 20:49:38.000000 vitessce-3.0.5/vitessce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:47:03.234284 vitessce-3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 12:44:39.000000 vitessce-3.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-31 12:44:39.000000 vitessce-3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-31 12:47:03.234284 vitessce-3.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-31 12:44:39.000000 vitessce-3.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-31 12:44:39.000000 vitessce-3.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-31 12:47:03.234284 vitessce-3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 12:44:39.000000 vitessce-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:47:03.234284 vitessce-3.0.6/vitessce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50080 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/config_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13522 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:47:03.234284 vitessce-3.0.6/vitessce/data_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/data_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10297 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/data_utils/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/data_utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/data_utils/multivec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/data_utils/ome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32997 2023-07-31 12:44:40.000000 vitessce-3.0.6/vitessce/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 12:47:03.234284 vitessce-3.0.6/vitessce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-31 12:47:03.000000 vitessce-3.0.6/vitessce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-31 12:47:03.000000 vitessce-3.0.6/vitessce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 12:47:03.000000 vitessce-3.0.6/vitessce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-31 12:47:03.000000 vitessce-3.0.6/vitessce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 12:47:03.000000 vitessce-3.0.6/vitessce.egg-info/top_level.txt
```

### Comparing `vitessce-3.0.5/LICENSE` & `vitessce-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/PKG-INFO` & `vitessce-3.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.0.5
+Version: 3.0.6
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -135,14 +135,17 @@
 Check that you have activated the correct conda or other virtual environment as you expect.
 When sharing errors, it can be helpful to share the current versions of packages in the environment, e.g., by `conda list` or `pip list`.
 
 ### Restart Kernel and Clear All Outputs, then refresh the browser tab
 
 To ensure that older widget JavaScript output is not causing conflicts with newer JavaScript output (which may persist via notebook outputs even without running notebook cells), clear old outputs by Kernel -> Restart Kernel and Clear All Outputs. Then refresh the browser tab (containing Jupyter) to ensure all JavaScript outputs are fresh.
 
+This is also typically required when running `!pip install vitessce[all]` from within a Jupyter notebook cell in the same session as running `vc.widget()` for the first time.
+The Kernel restart/Output clearing is required when a new Jupyter widget is installed in the environment, otherwise Jupyter will not yet recognize the newly-installed widget (as the notebook was opened with a different set of Jupyter widgets installed, and widget discovery is performed only at certain stages in the notebook lifecycle).
+
 ### Check the widget configuration
 
 If the widget renders successfully, you can get its current configuration by
 
 ```py
 vw = vc.widget()
 vw
```

### Comparing `vitessce-3.0.5/README.md` & `vitessce-3.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -86,14 +86,17 @@
 Check that you have activated the correct conda or other virtual environment as you expect.
 When sharing errors, it can be helpful to share the current versions of packages in the environment, e.g., by `conda list` or `pip list`.
 
 ### Restart Kernel and Clear All Outputs, then refresh the browser tab
 
 To ensure that older widget JavaScript output is not causing conflicts with newer JavaScript output (which may persist via notebook outputs even without running notebook cells), clear old outputs by Kernel -> Restart Kernel and Clear All Outputs. Then refresh the browser tab (containing Jupyter) to ensure all JavaScript outputs are fresh.
 
+This is also typically required when running `!pip install vitessce[all]` from within a Jupyter notebook cell in the same session as running `vc.widget()` for the first time.
+The Kernel restart/Output clearing is required when a new Jupyter widget is installed in the environment, otherwise Jupyter will not yet recognize the newly-installed widget (as the notebook was opened with a different set of Jupyter widgets installed, and widget discovery is performed only at certain stages in the notebook lifecycle).
+
 ### Check the widget configuration
 
 If the widget renders successfully, you can get its current configuration by
 
 ```py
 vw = vc.widget()
 vw
```

### Comparing `vitessce-3.0.5/pyproject.toml` & `vitessce-3.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0", "wheel>=0.38.4"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vitessce"
-version = "3.0.5"
+version = "3.0.6"
 authors = [
   { name="Mark Keller", email="mark_keller@hms.harvard.edu" },
 ]
 description = "Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.7"
@@ -29,16 +29,18 @@
   'numcodecs>=0.5.7',
   'scipy>=1.2.1',
   'negspy>=0.2.24',
   'pandas>=1.1.2',
   'black>=21.11b1',
   'numpy>=1.21.2',
   'anndata>=0.7.8,<0.9',
+  'scanpy>=1.9.3',
   'ome-zarr==0.2.1',
   'tifffile>=2020.10.1',
+  'jsonschema>=3.2'
 ]
 
 [project.optional-dependencies]
 dev = [
   'build==0.1.0',
   'pytest>=6.2.4',
   'loompy>=3.0.6',
```

### Comparing `vitessce-3.0.5/vitessce/__init__.py` & `vitessce-3.0.6/vitessce/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     DataType,
     FileType,
     # For backwards compatibility, also export ViewType as Component
     ViewType as Component,
     BASE_URL_PLACEHOLDER,
 )
 
+from .config_converter import (
+    CellBrowserToAnndataZarrConverter,  # only exported for testing.
+    convert_cell_browser_project_to_anndata,
+)
+
 from .wrappers import AbstractWrapper
 
 # We allow installation without all of the dependencies that the widget requires.
 # The imports below will fail in that case, and corresponding globals will be undefined.
 try:
     from .widget import VitessceWidget, data_server
 except ModuleNotFoundError as e:  # pragma: no cover
```

### Comparing `vitessce-3.0.5/vitessce/config.py` & `vitessce-3.0.6/vitessce/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,16 @@
         return vconcat(self, other)
 
 
 def hconcat(*views):
     """
     A helper function to create a ``VitessceConfigViewHConcat`` instance.
 
-    :param \*views: A variable number of views to concatenate horizontally.
-    :type \*views: VitessceConfigView or VitessceConfigViewVConcat or VitessceConfigViewHConcat
+    :param \\*views: A variable number of views to concatenate horizontally.
+    :type \\*views: VitessceConfigView or VitessceConfigViewVConcat or VitessceConfigViewHConcat
 
     :returns: The concatenated view instance.
     :rtype: VitessceConfigViewHConcat
 
     .. code-block:: python
         :emphasize-lines: 8
 
@@ -290,16 +290,16 @@
         return vconcat(self, other)
 
 
 def vconcat(*views):
     """
     A helper function to create a ``VitessceConfigViewVConcat`` instance.
 
-    :param \*views: A variable number of views to concatenate vertically.
-    :type \*views: VitessceConfigView or VitessceConfigViewVConcat or VitessceConfigViewHConcat
+    :param \\*views: A variable number of views to concatenate vertically.
+    :type \\*views: VitessceConfigView or VitessceConfigViewVConcat or VitessceConfigViewHConcat
 
     :returns: The concatenated view instance.
     :rtype: VitessceConfigViewVConcat
 
     .. code-block:: python
         :emphasize-lines: 8
 
@@ -370,16 +370,16 @@
         """
         return self.view["coordinationScopes"].get(c_type)
 
     def use_coordination(self, *c_scopes):
         """
         Attach a coordination scope to this view instance. All views using the same coordination scope for a particular coordination type will effectively be linked together.
 
-        :param \*c_scopes: A variable number of coordination scope instances can be passed.
-        :type \*c_scopes: VitessceConfigCoordinationScope
+        :param \\*c_scopes: A variable number of coordination scope instances can be passed.
+        :type \\*c_scopes: VitessceConfigCoordinationScope
 
         :returns: Self, to allow chaining.
         :rtype: VitessceConfigView
 
         .. code-block:: python
             :emphasize-lines: 12-13
 
@@ -423,15 +423,15 @@
         self.view["h"] = h
         return self
 
     def set_props(self, **kwargs):
         """
         Set the props for this view.
 
-        :param \*\*kwargs: A variable number of named props.
+        :param \\*\\*kwargs: A variable number of named props.
 
         :returns: Self, to allow chaining.
         :rtype: VitessceConfigView
         """
         if "props" in self.view:
             self.view["props"].update(kwargs)
         else:
@@ -749,16 +749,16 @@
         self.config["layout"].append(vcv)
         return vcv
 
     def add_coordination(self, *c_types):
         """
         Add scope(s) for new coordination type(s) to the config.
 
-        :param \*c_types: A variable number of coordination types.
-        :type \*c_types: str or vitessce.constants.CoordinationType
+        :param \\*c_types: A variable number of coordination types.
+        :type \\*c_types: str or vitessce.constants.CoordinationType
 
         :returns: The instances for the new scope objects corresponding to each coordination type. These can be linked to views via the ``VitessceConfigView.use_coordination()`` method.
         :rtype: list[VitessceConfigCoordinationScope]
 
         .. code-block:: python
             :emphasize-lines: 7-11
 
@@ -1172,15 +1172,15 @@
         return ipython_display(self, **kwargs)
 
     def export(self, to, *args, **kwargs):
         """
         Export this config's data objects to the local file system or a cloud storage system and get the resulting view config.
 
         :param str to: The export destination. Valid values include "S3" and "files".
-        :param \*\*kwargs: Keyword arguments to pass to the export function.
+        :param \\*\\*kwargs: Keyword arguments to pass to the export function.
         :returns: The config as a dict, with URLs for the bucket filled in.
         :rtype: dict
 
         .. code-block:: python
             :emphasize-lines: 8
 
             from vitessce import VitessceConfig, ViewType as cvtm, CoordinationType as ct
@@ -1206,15 +1206,15 @@
     A class to represent a Vitessce view config, where the methods ``add_dataset``, ``add_view``, and ``set_coordination_value`` return self (the config instance). This class inherits from ``VitessceConfig``.
     """
 
     def __init__(self, schema_version, **kwargs):
         """
         Construct a Vitessce view config object.
 
-        :param \*\*kwargs:  Takes the same arguments as the constructor on the ``VitessceConfig`` class.
+        :param \\*\\*kwargs:  Takes the same arguments as the constructor on the ``VitessceConfig`` class.
 
         .. code-block:: python
             :emphasize-lines: 3
 
             from vitessce import VitessceChainableConfig
 
             vc = VitessceChainableConfig(schema_version='1.0.15', name='My Config')
@@ -1227,15 +1227,15 @@
         new_vc.config = self.config.copy()
         return new_vc
 
     def add_dataset(self, copy=True, **kwargs):
         """
         Add a dataset to this config.
 
-        :param \*\*kwargs: Takes the same arguments as the ``add_dataset`` method on the ``VitessceConfig`` class.
+        :param \\*\\*kwargs: Takes the same arguments as the ``add_dataset`` method on the ``VitessceConfig`` class.
 
         :returns: The config instance.
         :rtype: VitessceChainableConfig
         """
         if copy:
             new_vc = copy_module.copy(self)
             return new_vc.add_dataset(copy=False, **kwargs)
@@ -1243,15 +1243,15 @@
         return self
 
     def add_view(self, component, copy=True, **kwargs):
         """
         Add a view to this config.
 
         :param component: Takes the same arguments as the ``add_view`` method on the ``VitessceConfig`` class.
-        :param \*\*kwargs: Takes the same arguments as the ``add_view`` method on the ``VitessceConfig`` class.
+        :param \\*\\*kwargs: Takes the same arguments as the ``add_view`` method on the ``VitessceConfig`` class.
 
         :returns: The config instance.
         :rtype: VitessceChainableConfig
         """
         if copy:
             new_vc = copy_module.copy(self)
             return new_vc.add_view(component, copy=False, **kwargs)
```

### Comparing `vitessce-3.0.5/vitessce/constants.py` & `vitessce-3.0.6/vitessce/constants.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/data_utils/anndata.py` & `vitessce-3.0.6/vitessce/data_utils/anndata.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/data_utils/entities.py` & `vitessce-3.0.6/vitessce/data_utils/entities.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
         :param str name: The unique identifier for the mapping, like UMAP, tSNE or PCA.
         :param list coords: A list of lists like [[1, 2], [3, 4], ...] in the order of cell_ids for each cell to be mapped to a scatterplot coorindate.
         """
         if len(coords) != len(self._cell_ids):
             raise ArgumentLengthDoesNotMatchCellIdsException(
                 'Coordinates length does not match Cell IDs Length')
-        if type(name) != str:
+        if not isinstance(name, str):
             raise TypeError(
                 'name argument needs to be a string for adding a scatterplot mapping')
         for idx, id in enumerate(self._cell_ids):
             if 'mappings' not in self.json[id]:
                 self.json[id]['mappings'] = {name: coords[idx]}
             else:
                 self.json[id]['mappings'][name] = coords[idx]
@@ -52,30 +52,30 @@
         Add a centroid for a spatial segmentation outline to each cell.
 
         :param list centroids: A list of lists like [[1, 2], [3, 4], ...] in the order of cell_ids for each cell to be mapped to a centroid coorindate.
         """
         if len(centroids) != len(self._cell_ids):
             raise ArgumentLengthDoesNotMatchCellIdsException(
                 'Centroid length does not match Cell IDs Length')
-        if type(centroids) != list or any([len(centroid) != 2 or type(centroid) != list for centroid in centroids]):
+        if not isinstance(centroids, list) or any([len(centroid) != 2 or not isinstance(centroid, list) for centroid in centroids]):
             raise TypeError('Centroids should be a list of two element lists')
         for idx, id in enumerate(self._cell_ids):
             self.json[id]['xy'] = centroids[idx]
 
     def add_polygon_outline(self, polygon_outline):
         """
         Add a polygon for a spatial segmentation outline to each cell.
 
         :param list polygon_outline: A list of lists of lists like [[[1, 2], [3, 4], [5, 6]], [[7, 8], [9, 10], [11, 12]]...] in the order of cell_ids for each cell to be mapped to its segmentation.
         """
         if len(polygon_outline) != len(self._cell_ids):
             raise ArgumentLengthDoesNotMatchCellIdsException(
                 'Segmentations length does not match Cell IDs Length')
         for idx, id in enumerate(self._cell_ids):
-            if type(polygon_outline[idx]) != list or any([len(coord) != 2 or type(coord) != list for coord in polygon_outline[idx]]):
+            if not isinstance(polygon_outline[idx], list) or any([len(coord) != 2 or not isinstance(coord, list) for coord in polygon_outline[idx]]):
                 raise TypeError(
                     f'Polygon outline for {id} should be a list of two element lists i.e xy coordinates')
             self.json[id]['poly'] = polygon_outline[idx]
 
 
 class CellSets:
```

### Comparing `vitessce-3.0.5/vitessce/data_utils/multivec.py` & `vitessce-3.0.6/vitessce/data_utils/multivec.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/data_utils/ome.py` & `vitessce-3.0.6/vitessce/data_utils/ome.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/export.py` & `vitessce-3.0.6/vitessce/export.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,27 +30,27 @@
     uploaded_routes = []
     for route in routes:
         route_path = route.path[1:]
         key = (prefix + "/" if len(prefix) > 0 else "") + route_path
 
         print(f"Uploading {bucket_name}:{key}")
 
-        if type(route) == JsonRoute:
+        if isinstance(route, JsonRoute):
             if route not in uploaded_routes:
                 data_json = route.data_json
                 bucket.put_object(Key=key, Body=json.dumps(data_json).encode())
                 uploaded_routes.append(route)
-        elif type(route) == FileRoute:
+        elif isinstance(route, FileRoute):
             if route not in uploaded_routes:
                 local_file_path = route.file_path
                 s3.meta.client.upload_file(local_file_path, bucket_name, key)
                 uploaded_routes.append(route)
-        elif type(route) == Mount:
+        elif isinstance(route, Mount):
             route_app = route.app
-            if type(route_app) == StaticFiles:
+            if isinstance(route_app, StaticFiles):
                 if route not in uploaded_routes:
                     uploaded_routes.append(route)
                     static_dir = route_app.directory
                     for root, dirs, files in os.walk(static_dir):
                         for filename in files:
                             file_key = key + \
                                 join(root, filename)[len(static_dir):]
@@ -72,26 +72,26 @@
 
     config_dict = config.to_dict(base_url=base_url)
     routes = config.get_routes()
     for route in routes:
         route_path = route.path[1:]
         out_path = join(out_dir, route_path)
 
-        if type(route) == JsonRoute:
+        if isinstance(route, JsonRoute):
             data_json = route.data_json
             os.makedirs(os.path.dirname(out_path), exist_ok=True)
             with open(out_path, 'w') as f:
                 json.dump(data_json, f)
-        elif type(route) == FileRoute:
+        elif isinstance(route, FileRoute):
             local_file_path = route.file_path
             os.makedirs(os.path.dirname(out_path), exist_ok=True)
             copyfile(local_file_path, out_path)
-        elif type(route) == Mount:
+        elif isinstance(route, Mount):
             route_app = route.app
-            if type(route_app) == StaticFiles:
+            if isinstance(route_app, StaticFiles):
                 static_dir = route_app.directory
 
                 for root, dirs, files in os.walk(static_dir):
                     for filename in files:
                         file_key = out_path + \
                             join(root, filename)[len(static_dir):]
                         os.makedirs(os.path.dirname(file_key), exist_ok=True)
```

### Comparing `vitessce-3.0.5/vitessce/repr.py` & `vitessce-3.0.6/vitessce/repr.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/routes.py` & `vitessce-3.0.6/vitessce/routes.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce/widget.py` & `vitessce-3.0.6/vitessce/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         uid_str = str(uuid.uuid4())[:4]
     else:
         uid_str = uid
     return uid_str
 
 
 ESM = """
-import { importWithMap } from 'https://unpkg.com/dynamic-importmap@0.0.1';
+import { importWithMap } from 'https://unpkg.com/dynamic-importmap@0.1.0';
 const importMap = {
   imports: {
     "react": "https://esm.sh/react@18.2.0?dev",
     "react-dom": "https://esm.sh/react-dom@18.2.0?dev",
     "react-dom/client": "https://esm.sh/react-dom@18.2.0/client?dev",
   },
 };
```

### Comparing `vitessce-3.0.5/vitessce/wrappers.py` & `vitessce-3.0.6/vitessce/wrappers.py`

 * *Files identical despite different names*

### Comparing `vitessce-3.0.5/vitessce.egg-info/PKG-INFO` & `vitessce-3.0.6/vitessce.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vitessce
-Version: 3.0.5
+Version: 3.0.6
 Summary: Jupyter widget facilitating interactive visualization of spatial single-cell data with Vitessce
 Author-email: Mark Keller <mark_keller@hms.harvard.edu>
 License: MIT License
         
         Copyright (c) 2020 Gehlenborg Lab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -135,14 +135,17 @@
 Check that you have activated the correct conda or other virtual environment as you expect.
 When sharing errors, it can be helpful to share the current versions of packages in the environment, e.g., by `conda list` or `pip list`.
 
 ### Restart Kernel and Clear All Outputs, then refresh the browser tab
 
 To ensure that older widget JavaScript output is not causing conflicts with newer JavaScript output (which may persist via notebook outputs even without running notebook cells), clear old outputs by Kernel -> Restart Kernel and Clear All Outputs. Then refresh the browser tab (containing Jupyter) to ensure all JavaScript outputs are fresh.
 
+This is also typically required when running `!pip install vitessce[all]` from within a Jupyter notebook cell in the same session as running `vc.widget()` for the first time.
+The Kernel restart/Output clearing is required when a new Jupyter widget is installed in the environment, otherwise Jupyter will not yet recognize the newly-installed widget (as the notebook was opened with a different set of Jupyter widgets installed, and widget discovery is performed only at certain stages in the notebook lifecycle).
+
 ### Check the widget configuration
 
 If the widget renders successfully, you can get its current configuration by
 
 ```py
 vw = vc.widget()
 vw
```

### Comparing `vitessce-3.0.5/vitessce.egg-info/requires.txt` & `vitessce-3.0.6/vitessce.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 numcodecs>=0.5.7
 scipy>=1.2.1
 negspy>=0.2.24
 pandas>=1.1.2
 black>=21.11b1
 numpy>=1.21.2
 anndata<0.9,>=0.7.8
+scanpy>=1.9.3
 ome-zarr==0.2.1
 tifffile>=2020.10.1
+jsonschema>=3.2
 
 [all]
 jupyter-server-proxy>=1.5.2
 anywidget==0.4.2
 uvicorn>=0.17.0
 ujson>=4.0.1
 starlette==0.14.0
```

