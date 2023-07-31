# Comparing `tmp/harpia-1.6.tar.gz` & `tmp/harpia-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.6.tar", last modified: Fri Jul 28 19:42:55 2023, max compression
+gzip compressed data, was "harpia-1.7.tar", last modified: Mon Jul 31 02:59:02 2023, max compression
```

## Comparing `harpia-1.6.tar` & `harpia-1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.387645 harpia-1.6/
--rw-r--r--   0 ryan       (501) staff       (20)     1061 2023-07-20 05:11:32.000000 harpia-1.6/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 19:42:55.386942 harpia-1.6/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      183 2023-07-20 05:15:06.000000 harpia-1.6/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.341464 harpia-1.6/harpia/
--rw-r--r--   0 ryan       (501) staff       (20)     1105 2023-07-20 05:28:30.000000 harpia-1.6/harpia/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.343566 harpia-1.6/harpia/tropomi/
--rw-r--r--   0 ryan       (501) staff       (20)     1101 2023-07-20 05:28:42.000000 harpia-1.6/harpia/tropomi/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.344452 harpia-1.6/harpia/tropomi/no2/
--rw-r--r--   0 ryan       (501) staff       (20)     1107 2023-07-20 05:29:04.000000 harpia-1.6/harpia/tropomi/no2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     6945 2023-07-28 19:40:27.000000 harpia-1.6/harpia/tropomi/no2/converter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.385701 harpia-1.6/harpia/tropomi/no2/lib/
--rw-r--r--   0 ryan       (501) staff       (20)  7844566 2023-07-16 20:21:38.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
--rw-r--r--   0 ryan       (501) staff       (20)  1970880 2023-07-16 20:22:34.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
--rw-r--r--   0 ryan       (501) staff       (20)   317616 2023-07-16 20:23:30.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
--rw-r--r--   0 ryan       (501) staff       (20)    78826 2023-07-16 20:26:42.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
--rw-r--r--   0 ryan       (501) staff       (20)    19984 2023-07-16 20:28:46.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.343116 harpia-1.6/harpia.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      589 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       49 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        7 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-28 19:42:55.387793 harpia-1.6/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2103 2023-07-28 19:40:41.000000 harpia-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.869860 harpia-1.7/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 02:15:18.000000 harpia-1.7/LICENSE
+-rw-rw-rw-   0        0        0      553 2023-07-31 02:59:02.869860 harpia-1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 02:15:18.000000 harpia-1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.832808 harpia-1.7/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 02:15:18.000000 harpia-1.7/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.846231 harpia-1.7/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.852721 harpia-1.7/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1143 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     7198 2023-07-31 02:55:09.000000 harpia-1.7/harpia/tropomi/no2/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.867846 harpia-1.7/harpia/tropomi/no2/lib/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 02:15:18.000000 harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:02.845234 harpia-1.7/harpia.egg-info/
+-rw-rw-rw-   0        0        0      553 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      589 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 02:59:02.000000 harpia-1.7/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:59:02.869860 harpia-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2160 2023-07-31 02:55:52.000000 harpia-1.7/setup.py
```

### Comparing `harpia-1.6/harpia/tropomi/__init__.py` & `harpia-1.7/harpia/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-'''
-
-Copyright 2023 Ryan Solgi
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the "Software"), to deal in 
-the Software without restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
-Software, and to permit persons to whom the Software is furnished to do so, 
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-SOFTWARE.
-'''
-
-from . import no2
-
-
-
-
-
-
-
-
-
-
-
-
+'''
+
+Copyright 2023 Ryan Solgi
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of 
+this software and associated documentation files (the "Software"), to deal in 
+the Software without restriction, including without limitation the rights to use, 
+copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
+Software, and to permit persons to whom the Software is furnished to do so, 
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+SOFTWARE.
+'''
+
+from . import tropomi
+
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `harpia-1.6/harpia/tropomi/no2/converter.py` & `harpia-1.7/harpia/tropomi/no2/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import os
 import numpy as np
 from netCDF4 import Dataset
 import pandas as pd
 import geopandas
 from rasterio.features import rasterize
 import rasterio
-import pkg_resources
+from importlib_resources import files, as_file
 from harpia.tropomi.no2 import converter
-
+import harpia.tropomi.no2.lib
+import pkg_resources
 
 def sat_to_df(data_file_path):
     
     file=Dataset(data_file_path, "r" , format="NETCDF4")
     
     
     qa_value=file.groups['PRODUCT'].variables['qa_value']
@@ -176,29 +177,29 @@
     
     region_corener=converter.set_region(region)
     
     gdf=converter.clip_gdf(gdf,region_corener)
     gdf=gdf.reset_index()
     if not gdf.empty:
         for res in resolution_list:
-            raster_template=converter.get_raster_template('130w60w20n55n',res)
-            new_raster_name=granule_end_date+'_'+res+'_'+str(qa_value_threshold)+'_raster.tif'
-            new_raster=os.path.join(writing_directory, new_raster_name)
-    
-            rasterized=converter.gdf_to_raster(gdf,raster_template, new_raster)
-            raster_template.close()
-    del df
-    del gdf
+            raster_file_name='raster_template_'+'130w60w20n55n'+'_'+res+'.tif'
+            source=files(harpia.tropomi.no2.lib).joinpath(raster_file_name)
+            with as_file(source) as raster_template:
+            
+            #raster_template=converter.get_raster_template('130w60w20n55n',res)
+                new_raster_name=granule_end_date+'_'+res+'_'+str(qa_value_threshold)+'_raster.tif'
+                new_raster=os.path.join(writing_directory, new_raster_name)
     
-
+                rasterized=converter.gdf_to_raster(gdf,raster_template, new_raster)
+        
    
 
 
 
 def converter_run(read_directory,write_directory, granule_end_date, qa_value_threshold, df_print=False):
  
-    #if df_print:
-    #        converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
+    if df_print:
+            converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
         
     converter.convert_to_raster(read_directory,write_directory, ['005','010','025','050','100'], granule_end_date, qa_value_threshold)
```

### Comparing `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif` & `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif` & `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif` & `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif` & `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif` & `harpia-1.7/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.6/harpia.egg-info/SOURCES.txt` & `harpia-1.7/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.6/setup.py` & `harpia-1.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-'''
-    Copyright 2023 Ryan Solgi
-    
-    Permission is hereby granted, free of charge, to any person obtaining a copy of 
-    this software and associated documentation files (the "Software"), to deal in 
-    the Software without restriction, including without limitation the rights to use, 
-    copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
-    Software, and to permit persons to whom the Software is furnished to do so, 
-    subject to the following conditions:
-    
-    The above copyright notice and this permission notice shall be included in all
-    copies or substantial portions of the Software.
-    
-    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-    THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-    SOFTWARE.
-
-'''
-
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="harpia",
-    version="1.6",
-    author="Ryan Solgi",
-    author_email="ryan.solgi@gmail.com",
-    maintainer='Ryan Solgi',
-    description="A Python Package for Development",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/rmsolgi/harpia.git",
-    keywords=['harpia'],
-    packages=setuptools.find_packages(include=['*'], exclude=['tests']),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-    ],
-    install_requires=['numpy', 'datetime', 'netCDF4', 'pandas', 'geopandas', 'rasterio'],
-    include_package_data=True,
-    package_data={'': ['tropomi/no2/lib/*.tif']},
-    
-    )
-
-
-
-
-
-
+'''
+    Copyright 2023 Ryan Solgi
+    
+    Permission is hereby granted, free of charge, to any person obtaining a copy of 
+    this software and associated documentation files (the "Software"), to deal in 
+    the Software without restriction, including without limitation the rights to use, 
+    copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
+    Software, and to permit persons to whom the Software is furnished to do so, 
+    subject to the following conditions:
+    
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+    
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
+    THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
+    SOFTWARE.
+
+'''
+
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="harpia",
+    version="1.7",
+    author="Ryan Solgi",
+    author_email="ryan.solgi@gmail.com",
+    maintainer='Ryan Solgi',
+    description="A Python Package for Development",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/rmsolgi/harpia.git",
+    keywords=['harpia'],
+    packages=setuptools.find_packages(include=['*'], exclude=['tests']),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
+    install_requires=['numpy', 'datetime', 'netCDF4', 'pandas', 'geopandas', 'rasterio'],
+    include_package_data=True,
+    package_data={'': ['tropomi/no2/lib/*.tif']},
+    
+    )
+
+
+
+
+
+
```

