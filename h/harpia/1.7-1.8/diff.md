# Comparing `tmp/harpia-1.7.tar.gz` & `tmp/harpia-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.7.tar", last modified: Mon Jul 31 02:59:02 2023, max compression
+gzip compressed data, was "harpia-1.8.tar", last modified: Mon Jul 31 03:19:23 2023, max compression
```

## Comparing `harpia-1.7.tar` & `harpia-1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.869860 harpia-1.7/
--rw-rw-rw-   0        0        0     1080 2023-07-31 02:15:18.000000 harpia-1.7/LICENSE
--rw-rw-rw-   0        0        0      553 2023-07-31 02:59:02.869860 harpia-1.7/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 02:15:18.000000 harpia-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.832808 harpia-1.7/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 02:15:18.000000 harpia-1.7/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.846231 harpia-1.7/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.852721 harpia-1.7/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1143 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     7198 2023-07-31 02:55:09.000000 harpia-1.7/harpia/tropomi/no2/converter.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.867846 harpia-1.7/harpia/tropomi/no2/lib/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
-drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.845234 harpia-1.7/harpia.egg-info/
--rw-rw-rw-   0        0        0      553 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      589 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 02:59:02.869860 harpia-1.7/setup.cfg
--rw-rw-rw-   0        0        0     2160 2023-07-31 02:55:52.000000 harpia-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:23.060959 harpia-1.8/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:16:29.000000 harpia-1.8/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-07-31 03:19:23.059555 harpia-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:16:29.000000 harpia-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:22.999518 harpia-1.8/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:16:29.000000 harpia-1.8/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:23.017777 harpia-1.8/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:23.026026 harpia-1.8/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1143 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6928 2023-07-31 03:18:08.000000 harpia-1.8/harpia/tropomi/no2/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:23.058556 harpia-1.8/harpia/tropomi/no2/lib/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:16:29.000000 harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
+drwxrwxrwx   0        0        0        0 2023-07-31 03:19:23.017777 harpia-1.8/harpia.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-07-31 03:19:22.000000 harpia-1.8/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-07-31 03:19:22.000000 harpia-1.8/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 03:19:22.000000 harpia-1.8/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-31 03:19:22.000000 harpia-1.8/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 03:19:22.000000 harpia-1.8/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 03:19:23.060959 harpia-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2160 2023-07-31 03:16:42.000000 harpia-1.8/setup.py
```

### Comparing `harpia-1.7/LICENSE` & `harpia-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.7/PKG-INFO` & `harpia-1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.7
+Version: 1.8
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.7/harpia/__init__.py` & `harpia-1.8/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/__init__.py` & `harpia-1.8/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/__init__.py` & `harpia-1.8/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/converter.py` & `harpia-1.8/harpia/tropomi/no2/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 import os
 import numpy as np
 from netCDF4 import Dataset
 import pandas as pd
 import geopandas
 from rasterio.features import rasterize
 import rasterio
-from importlib_resources import files, as_file
-from harpia.tropomi.no2 import converter
-import harpia.tropomi.no2.lib
 import pkg_resources
+from harpia.tropomi.no2 import converter
 
 def sat_to_df(data_file_path):
     
     file=Dataset(data_file_path, "r" , format="NETCDF4")
     
     
     qa_value=file.groups['PRODUCT'].variables['qa_value']
@@ -177,29 +175,25 @@
     
     region_corener=converter.set_region(region)
     
     gdf=converter.clip_gdf(gdf,region_corener)
     gdf=gdf.reset_index()
     if not gdf.empty:
         for res in resolution_list:
-            raster_file_name='raster_template_'+'130w60w20n55n'+'_'+res+'.tif'
-            source=files(harpia.tropomi.no2.lib).joinpath(raster_file_name)
-            with as_file(source) as raster_template:
-            
-            #raster_template=converter.get_raster_template('130w60w20n55n',res)
-                new_raster_name=granule_end_date+'_'+res+'_'+str(qa_value_threshold)+'_raster.tif'
-                new_raster=os.path.join(writing_directory, new_raster_name)
+            raster_template=converter.get_raster_template('130w60w20n55n',res)
+            new_raster_name=granule_end_date+'_'+res+'_'+str(qa_value_threshold)+'_raster.tif'
+            new_raster=os.path.join(writing_directory, new_raster_name)
     
-                rasterized=converter.gdf_to_raster(gdf,raster_template, new_raster)
+            rasterized=converter.gdf_to_raster(gdf,raster_template, new_raster)
         
    
-
+            pkg_resources.cleanup_resources()
 
 
 def converter_run(read_directory,write_directory, granule_end_date, qa_value_threshold, df_print=False):
  
-    if df_print:
-            converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
+    #if df_print:
+    #        converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
         
     converter.convert_to_raster(read_directory,write_directory, ['005','010','025','050','100'], granule_end_date, qa_value_threshold)
```

### Comparing `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif` & `harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif` & `harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif` & `harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif` & `harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif` & `harpia-1.8/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.7/harpia.egg-info/PKG-INFO` & `harpia-1.8/harpia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.7
+Version: 1.8
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.7/harpia.egg-info/SOURCES.txt` & `harpia-1.8/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.7/setup.py` & `harpia-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.7",
+    version="1.8",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```

