# Comparing `tmp/hydrodataset-0.1.0.tar.gz` & `tmp/hydrodataset-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrodataset-0.1.0.tar", last modified: Tue Jul 25 08:13:52 2023, max compression
+gzip compressed data, was "hydrodataset-0.1.2.tar", last modified: Mon Jul 31 09:38:15 2023, max compression
```

## Comparing `hydrodataset-0.1.0.tar` & `hydrodataset-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/hydrodataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61052 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/camels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/grdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hydro_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hydro_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/hysets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/lamah.py
--rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/mopex.py
--rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/hydrodataset/multi_datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/hydrodataset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 08:13:52.000000 hydrodataset-0.1.0/hydrodataset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:52.463416 hydrodataset-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_camels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_caravan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_hysets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-07-25 08:13:38.000000 hydrodataset-0.1.0/test/test_multi_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/hydrodataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64414 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/camels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/caravan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/grdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hydro_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hydro_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/hysets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14604 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/lamah.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13929 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/mopex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39072 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/hydrodataset/multi_datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/hydrodataset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:38:15.000000 hydrodataset-0.1.2/hydrodataset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 09:38:15.436135 hydrodataset-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-31 09:38:05.000000 hydrodataset-0.1.2/setup.py
```

### Comparing `hydrodataset-0.1.0/LICENSE` & `hydrodataset-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/PKG-INFO` & `hydrodataset-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2023-07-25 15:13:52
+ * @LastEditTime: 2023-07-26 13:35:41
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -204,12 +204,16 @@
 | **Number** | **Dataset** | **Description**                                         |
 | ---------- | ----------- | ------------------------------------------------------- |
 | 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
 | 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
 | 3          | **HYSETS**  | HYSETS dataset for North America                        |
 | 4          | **Caravan** | Caravan dataset for global                              |
 
+For units, we use [pint](https://github.com/hgrecco/pint), and [pint-xarray](https://github.com/xarray-contrib/pint-xarray) to handle them.
+
+We highly recommend you to use [xarray](http://xarray.pydata.org/en/stable/) to read the data, as it is a powerful tool for handling multi-dimensional data. Then, you can see the units of all variables in the xarray dataset.
+
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.1.0/README.md` & `hydrodataset-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2023-07-25 15:13:52
+ * @LastEditTime: 2023-07-26 13:35:41
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -182,12 +182,16 @@
 | **Number** | **Dataset** | **Description**                                         |
 | ---------- | ----------- | ------------------------------------------------------- |
 | 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
 | 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
 | 3          | **HYSETS**  | HYSETS dataset for North America                        |
 | 4          | **Caravan** | Caravan dataset for global                              |
 
+For units, we use [pint](https://github.com/hgrecco/pint), and [pint-xarray](https://github.com/xarray-contrib/pint-xarray) to handle them.
+
+We highly recommend you to use [xarray](http://xarray.pydata.org/en/stable/) to read the data, as it is a powerful tool for handling multi-dimensional data. Then, you can see the units of all variables in the xarray dataset.
+
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.1.0/hydrodataset/__init__.py` & `hydrodataset-0.1.2/hydrodataset/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 from pathlib import Path
 import os
 
 __author__ = """Wenyu Ouyang"""
 __email__ = "wenyuouyang@outlook.com"
-__version__ = '0.1.0'
+__version__ = '0.1.2'
 
 # we use a .hydrodataset dir to save the setting
 hydrodataset_setting_dir = Path.home().joinpath(".hydrodataset")
 if not hydrodataset_setting_dir.is_dir():
     hydrodataset_setting_dir.mkdir(parents=True)
 hydrodataset_cache_dir = hydrodataset_setting_dir.joinpath("cache")
 if not hydrodataset_cache_dir.is_dir():
```

### Comparing `hydrodataset-0.1.0/hydrodataset/camels.py` & `hydrodataset-0.1.2/hydrodataset/camels.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-01-05 18:01:11
-LastEditTime: 2023-07-16 16:34:22
+LastEditTime: 2023-07-31 10:06:56
 LastEditors: Wenyu Ouyang
 Description: Read Camels Series ("AUStralia", "BRazil", "ChiLe", "GreatBritain", "UnitedStates") datasets
-FilePath: \hydrodataset\hydrodataset\camels.py
+FilePath: /hydrodataset/hydrodataset/camels.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import json
 import warnings
 import collections
 import fnmatch
 import logging
@@ -16,14 +16,15 @@
 from typing import Union
 import pandas as pd
 import numpy as np
 from pandas.core.dtypes.common import is_string_dtype, is_numeric_dtype
 from pathlib import Path
 from urllib.request import urlopen
 from tqdm import tqdm
+import xarray as xr
 from hydrodataset import CACHE_DIR, hydro_utils, HydroDataset, CAMELS_REGIONS
 
 CAMELS_NO_DATASET_ERROR_LOG = (
     "We cannot read this dataset now. Please check if you choose correctly:\n"
     + str(CAMELS_REGIONS)
 )
 
@@ -79,15 +80,15 @@
         region
             the default is CAMELS(-US), since it's the first CAMELS dataset.
             All are included in CAMELS_REGIONS
         """
         super().__init__(data_path)
         if region not in CAMELS_REGIONS:
             raise NotImplementedError(
-                "Please chose one region in: " + str(CAMELS_REGIONS)
+                f"Please chose one region in: {str(CAMELS_REGIONS)}"
             )
         self.region = region
         self.data_source_description = self.set_data_source_describe()
         if download:
             self.download_data_source()
         self.sites = self.read_site_info()
 
@@ -102,284 +103,295 @@
         -------
         collections.OrderedDict
             the description for a CAMELS dataset
         """
         camels_db = self.data_source_dir
 
         if self.region == "US":
-            # shp file of basins
-            camels_shp_file = camels_db.joinpath(
-                "basin_set_full_res", "HCDN_nhru_final_671.shp"
-            )
-            # config of flow data
-            flow_dir = camels_db.joinpath(
-                "basin_timeseries_v1p2_metForcing_obsFlow",
-                "basin_dataset_public_v1p2",
-                "usgs_streamflow",
-            )
-            flow_after_2015_dir = camels_db.joinpath(
-                "camels_streamflow", "camels_streamflow"
-            )
-            # forcing
-            forcing_dir = camels_db.joinpath(
-                "basin_timeseries_v1p2_metForcing_obsFlow",
-                "basin_dataset_public_v1p2",
-                "basin_mean_forcing",
-            )
-            forcing_types = ["daymet", "maurer", "nldas"]
-            # attr
-            attr_dir = camels_db
-            gauge_id_file = attr_dir.joinpath("camels_name.txt")
-            attr_key_lst = ["topo", "clim", "hydro", "vege", "soil", "geol"]
-            base_url = "https://gdex.ucar.edu/dataset/camels"
-            download_url_lst = [
-                f"{base_url}/file/basin_set_full_res.zip",
-                # f"{base_url}/file/basin_timeseries_v1p2_metForcing_obsFlow.zip",
-                f"{base_url}/file/camels_attributes_v2.0.xlsx",
-                f"{base_url}/file/camels_clim.txt",
-                f"{base_url}/file/camels_geol.txt",
-                f"{base_url}/file/camels_hydro.txt",
-                f"{base_url}/file/camels_name.txt",
-                f"{base_url}/file/camels_soil.txt",
-                f"{base_url}/file/camels_topo.txt",
-                f"{base_url}/file/camels_vege.txt",
-            ]
-
-            return collections.OrderedDict(
-                CAMELS_DIR=camels_db,
-                CAMELS_FLOW_DIR=flow_dir,
-                CAMELS_FLOW_AFTER2015_DIR=flow_after_2015_dir,
-                CAMELS_FORCING_DIR=forcing_dir,
-                CAMELS_FORCING_TYPE=forcing_types,
-                CAMELS_ATTR_DIR=attr_dir,
-                CAMELS_ATTR_KEY_LST=attr_key_lst,
-                CAMELS_GAUGE_FILE=gauge_id_file,
-                CAMELS_BASINS_SHP_FILE=camels_shp_file,
-                CAMELS_DOWNLOAD_URL_LST=download_url_lst,
-            )
+            return self._set_data_source_camelsus_describe(camels_db)
         elif self.region == "AUS":
-            # id and name
-            gauge_id_file = camels_db.joinpath(
-                "01_id_name_metadata",
-                "01_id_name_metadata",
-                "id_name_metadata.csv",
-            )
-            # shp file of basins
-            camels_shp_file = camels_db.joinpath(
-                "02_location_boundary_area",
-                "02_location_boundary_area",
-                "shp",
-                "CAMELS_AUS_BasinOutlets_adopted.shp",
-            )
-            # config of flow data
-            flow_dir = camels_db.joinpath("03_streamflow", "03_streamflow")
-            # attr
-            attr_dir = camels_db.joinpath("04_attributes", "04_attributes")
-            # forcing
-            forcing_dir = camels_db.joinpath(
-                "05_hydrometeorology", "05_hydrometeorology"
-            )
-
-            return collections.OrderedDict(
-                CAMELS_DIR=camels_db,
-                CAMELS_FLOW_DIR=flow_dir,
-                CAMELS_FORCING_DIR=forcing_dir,
-                CAMELS_ATTR_DIR=attr_dir,
-                CAMELS_GAUGE_FILE=gauge_id_file,
-                CAMELS_BASINS_SHP_FILE=camels_shp_file,
-            )
+            return self._set_data_source_camelsaus_describe(camels_db)
         elif self.region == "BR":
-            # attr
-            attr_dir = camels_db.joinpath(
-                "01_CAMELS_BR_attributes", "01_CAMELS_BR_attributes"
-            )
-            # we don't need the location attr file
-            attr_key_lst = [
-                "climate",
-                "geology",
-                "human_intervention",
-                "hydrology",
-                "land_cover",
-                "quality_check",
-                "soil",
-                "topography",
-            ]
-            # id and name, there are two types stations in CAMELS_BR, and we only chose the 897-stations version
-            gauge_id_file = attr_dir.joinpath("camels_br_topography.txt")
-            # shp file of basins
-            camels_shp_file = camels_db.joinpath(
-                "14_CAMELS_BR_catchment_boundaries",
-                "14_CAMELS_BR_catchment_boundaries",
-                "camels_br_catchments.shp",
-            )
-            # config of flow data
-            flow_dir_m3s = camels_db.joinpath(
-                "02_CAMELS_BR_streamflow_m3s", "02_CAMELS_BR_streamflow_m3s"
-            )
-            flow_dir_mm_selected_catchments = camels_db.joinpath(
-                "03_CAMELS_BR_streamflow_mm_selected_catchments",
-                "03_CAMELS_BR_streamflow_mm_selected_catchments",
-            )
-            flow_dir_simulated = camels_db.joinpath(
-                "04_CAMELS_BR_streamflow_simulated",
-                "04_CAMELS_BR_streamflow_simulated",
-            )
-
-            # forcing
-            forcing_dir_precipitation_chirps = camels_db.joinpath(
-                "05_CAMELS_BR_precipitation_chirps",
-                "05_CAMELS_BR_precipitation_chirps",
-            )
-            forcing_dir_precipitation_mswep = camels_db.joinpath(
-                "06_CAMELS_BR_precipitation_mswep",
-                "06_CAMELS_BR_precipitation_mswep",
-            )
-            forcing_dir_precipitation_cpc = camels_db.joinpath(
-                "07_CAMELS_BR_precipitation_cpc",
-                "07_CAMELS_BR_precipitation_cpc",
-            )
-            forcing_dir_evapotransp_gleam = camels_db.joinpath(
-                "08_CAMELS_BR_evapotransp_gleam",
-                "08_CAMELS_BR_evapotransp_gleam",
-            )
-            forcing_dir_evapotransp_mgb = camels_db.joinpath(
-                "09_CAMELS_BR_evapotransp_mgb",
-                "09_CAMELS_BR_evapotransp_mgb",
-            )
-            forcing_dir_potential_evapotransp_gleam = camels_db.joinpath(
-                "10_CAMELS_BR_potential_evapotransp_gleam",
-                "10_CAMELS_BR_potential_evapotransp_gleam",
-            )
-            forcing_dir_temperature_min_cpc = camels_db.joinpath(
-                "11_CAMELS_BR_temperature_min_cpc",
-                "11_CAMELS_BR_temperature_min_cpc",
-            )
-            forcing_dir_temperature_mean_cpc = camels_db.joinpath(
-                "12_CAMELS_BR_temperature_mean_cpc",
-                "12_CAMELS_BR_temperature_mean_cpc",
-            )
-            forcing_dir_temperature_max_cpc = camels_db.joinpath(
-                "13_CAMELS_BR_temperature_max_cpc",
-                "13_CAMELS_BR_temperature_max_cpc",
-            )
-            return collections.OrderedDict(
-                CAMELS_DIR=camels_db,
-                CAMELS_FLOW_DIR=[
-                    flow_dir_m3s,
-                    flow_dir_mm_selected_catchments,
-                    flow_dir_simulated,
-                ],
-                CAMELS_FORCING_DIR=[
-                    forcing_dir_precipitation_chirps,
-                    forcing_dir_precipitation_mswep,
-                    forcing_dir_precipitation_cpc,
-                    forcing_dir_evapotransp_gleam,
-                    forcing_dir_evapotransp_mgb,
-                    forcing_dir_potential_evapotransp_gleam,
-                    forcing_dir_temperature_min_cpc,
-                    forcing_dir_temperature_mean_cpc,
-                    forcing_dir_temperature_max_cpc,
-                ],
-                CAMELS_ATTR_DIR=attr_dir,
-                CAMELS_ATTR_KEY_LST=attr_key_lst,
-                CAMELS_GAUGE_FILE=gauge_id_file,
-                CAMELS_BASINS_SHP_FILE=camels_shp_file,
-            )
+            return self._set_data_source_camelsbr_describe(camels_db)
         elif self.region == "CL":
-            # attr
-            attr_dir = camels_db.joinpath("1_CAMELScl_attributes")
-            attr_file = attr_dir.joinpath("1_CAMELScl_attributes.txt")
-            # shp file of basins
-            camels_shp_file = camels_db.joinpath(
-                "CAMELScl_catchment_boundaries",
-                "catchments_camels_cl_v1.3.shp",
-            )
-            # config of flow data
-            flow_dir_m3s = camels_db.joinpath("2_CAMELScl_streamflow_m3s")
-            flow_dir_mm = camels_db.joinpath("3_CAMELScl_streamflow_mm")
-
-            # forcing
-            forcing_dir_precip_cr2met = camels_db.joinpath("4_CAMELScl_precip_cr2met")
-            forcing_dir_precip_chirps = camels_db.joinpath("5_CAMELScl_precip_chirps")
-            forcing_dir_precip_mswep = camels_db.joinpath("6_CAMELScl_precip_mswep")
-            forcing_dir_precip_tmpa = camels_db.joinpath("7_CAMELScl_precip_tmpa")
-            forcing_dir_tmin_cr2met = camels_db.joinpath("8_CAMELScl_tmin_cr2met")
-            forcing_dir_tmax_cr2met = camels_db.joinpath("9_CAMELScl_tmax_cr2met")
-            forcing_dir_tmean_cr2met = camels_db.joinpath("10_CAMELScl_tmean_cr2met")
-            forcing_dir_pet_8d_modis = camels_db.joinpath("11_CAMELScl_pet_8d_modis")
-            forcing_dir_pet_hargreaves = camels_db.joinpath(
-                "12_CAMELScl_pet_hargreaves"
-            )
-            forcing_dir_swe = camels_db.joinpath("13_CAMELScl_swe")
-            return collections.OrderedDict(
-                CAMELS_DIR=camels_db,
-                CAMELS_FLOW_DIR=[flow_dir_m3s, flow_dir_mm],
-                CAMELS_FORCING_DIR=[
-                    forcing_dir_precip_cr2met,
-                    forcing_dir_precip_chirps,
-                    forcing_dir_precip_mswep,
-                    forcing_dir_precip_tmpa,
-                    forcing_dir_tmin_cr2met,
-                    forcing_dir_tmax_cr2met,
-                    forcing_dir_tmean_cr2met,
-                    forcing_dir_pet_8d_modis,
-                    forcing_dir_pet_hargreaves,
-                    forcing_dir_swe,
-                ],
-                CAMELS_ATTR_DIR=attr_dir,
-                CAMELS_GAUGE_FILE=attr_file,
-                CAMELS_BASINS_SHP_FILE=camels_shp_file,
-            )
+            return self._set_data_source_camelscl_describe(camels_db)
         elif self.region == "GB":
-            # shp file of basins
-            camels_shp_file = camels_db.joinpath(
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "data",
-                "CAMELS_GB_catchment_boundaries",
-                "CAMELS_GB_catchment_boundaries.shp",
-            )
-            # flow and forcing data are in a same file
-            flow_dir = camels_db.joinpath(
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "data",
-                "timeseries",
-            )
-            forcing_dir = flow_dir
-            # attr
-            attr_dir = camels_db.joinpath(
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
-                "data",
-            )
-            gauge_id_file = attr_dir.joinpath("CAMELS_GB_hydrometry_attributes.csv")
-            attr_key_lst = [
-                "climatic",
-                "humaninfluence",
-                "hydrogeology",
-                "hydrologic",
-                "hydrometry",
-                "landcover",
-                "soil",
-                "topographic",
-            ]
-
-            return collections.OrderedDict(
-                CAMELS_DIR=camels_db,
-                CAMELS_FLOW_DIR=flow_dir,
-                CAMELS_FORCING_DIR=forcing_dir,
-                CAMELS_ATTR_DIR=attr_dir,
-                CAMELS_ATTR_KEY_LST=attr_key_lst,
-                CAMELS_GAUGE_FILE=gauge_id_file,
-                CAMELS_BASINS_SHP_FILE=camels_shp_file,
-            )
+            return self._set_data_source_camelsgb_describe(camels_db)
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
 
+    def _set_data_source_camelsgb_describe(self, camels_db):
+        # shp file of basins
+        camels_shp_file = camels_db.joinpath(
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "data",
+            "CAMELS_GB_catchment_boundaries",
+            "CAMELS_GB_catchment_boundaries.shp",
+        )
+        # flow and forcing data are in a same file
+        flow_dir = camels_db.joinpath(
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "data",
+            "timeseries",
+        )
+        forcing_dir = flow_dir
+        # attr
+        attr_dir = camels_db.joinpath(
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "8344e4f3-d2ea-44f5-8afa-86d2987543a9",
+            "data",
+        )
+        gauge_id_file = attr_dir.joinpath("CAMELS_GB_hydrometry_attributes.csv")
+        attr_key_lst = [
+            "climatic",
+            "humaninfluence",
+            "hydrogeology",
+            "hydrologic",
+            "hydrometry",
+            "landcover",
+            "soil",
+            "topographic",
+        ]
+
+        return collections.OrderedDict(
+            CAMELS_DIR=camels_db,
+            CAMELS_FLOW_DIR=flow_dir,
+            CAMELS_FORCING_DIR=forcing_dir,
+            CAMELS_ATTR_DIR=attr_dir,
+            CAMELS_ATTR_KEY_LST=attr_key_lst,
+            CAMELS_GAUGE_FILE=gauge_id_file,
+            CAMELS_BASINS_SHP_FILE=camels_shp_file,
+        )
+
+    def _set_data_source_camelscl_describe(self, camels_db):
+        # attr
+        attr_dir = camels_db.joinpath("1_CAMELScl_attributes")
+        attr_file = attr_dir.joinpath("1_CAMELScl_attributes.txt")
+        # shp file of basins
+        camels_shp_file = camels_db.joinpath(
+            "CAMELScl_catchment_boundaries",
+            "catchments_camels_cl_v1.3.shp",
+        )
+        # config of flow data
+        flow_dir_m3s = camels_db.joinpath("2_CAMELScl_streamflow_m3s")
+        flow_dir_mm = camels_db.joinpath("3_CAMELScl_streamflow_mm")
+
+        # forcing
+        forcing_dir_precip_cr2met = camels_db.joinpath("4_CAMELScl_precip_cr2met")
+        forcing_dir_precip_chirps = camels_db.joinpath("5_CAMELScl_precip_chirps")
+        forcing_dir_precip_mswep = camels_db.joinpath("6_CAMELScl_precip_mswep")
+        forcing_dir_precip_tmpa = camels_db.joinpath("7_CAMELScl_precip_tmpa")
+        forcing_dir_tmin_cr2met = camels_db.joinpath("8_CAMELScl_tmin_cr2met")
+        forcing_dir_tmax_cr2met = camels_db.joinpath("9_CAMELScl_tmax_cr2met")
+        forcing_dir_tmean_cr2met = camels_db.joinpath("10_CAMELScl_tmean_cr2met")
+        forcing_dir_pet_8d_modis = camels_db.joinpath("11_CAMELScl_pet_8d_modis")
+        forcing_dir_pet_hargreaves = camels_db.joinpath("12_CAMELScl_pet_hargreaves")
+        forcing_dir_swe = camels_db.joinpath("13_CAMELScl_swe")
+        return collections.OrderedDict(
+            CAMELS_DIR=camels_db,
+            CAMELS_FLOW_DIR=[flow_dir_m3s, flow_dir_mm],
+            CAMELS_FORCING_DIR=[
+                forcing_dir_precip_cr2met,
+                forcing_dir_precip_chirps,
+                forcing_dir_precip_mswep,
+                forcing_dir_precip_tmpa,
+                forcing_dir_tmin_cr2met,
+                forcing_dir_tmax_cr2met,
+                forcing_dir_tmean_cr2met,
+                forcing_dir_pet_8d_modis,
+                forcing_dir_pet_hargreaves,
+                forcing_dir_swe,
+            ],
+            CAMELS_ATTR_DIR=attr_dir,
+            CAMELS_GAUGE_FILE=attr_file,
+            CAMELS_BASINS_SHP_FILE=camels_shp_file,
+        )
+
+    def _set_data_source_camelsbr_describe(self, camels_db):
+        # attr
+        attr_dir = camels_db.joinpath(
+            "01_CAMELS_BR_attributes", "01_CAMELS_BR_attributes"
+        )
+        # we don't need the location attr file
+        attr_key_lst = [
+            "climate",
+            "geology",
+            "human_intervention",
+            "hydrology",
+            "land_cover",
+            "quality_check",
+            "soil",
+            "topography",
+        ]
+        # id and name, there are two types stations in CAMELS_BR, and we only chose the 897-stations version
+        gauge_id_file = attr_dir.joinpath("camels_br_topography.txt")
+        # shp file of basins
+        camels_shp_file = camels_db.joinpath(
+            "14_CAMELS_BR_catchment_boundaries",
+            "14_CAMELS_BR_catchment_boundaries",
+            "camels_br_catchments.shp",
+        )
+        # config of flow data
+        flow_dir_m3s = camels_db.joinpath(
+            "02_CAMELS_BR_streamflow_m3s", "02_CAMELS_BR_streamflow_m3s"
+        )
+        flow_dir_mm_selected_catchments = camels_db.joinpath(
+            "03_CAMELS_BR_streamflow_mm_selected_catchments",
+            "03_CAMELS_BR_streamflow_mm_selected_catchments",
+        )
+        flow_dir_simulated = camels_db.joinpath(
+            "04_CAMELS_BR_streamflow_simulated",
+            "04_CAMELS_BR_streamflow_simulated",
+        )
+
+        # forcing
+        forcing_dir_precipitation_chirps = camels_db.joinpath(
+            "05_CAMELS_BR_precipitation_chirps",
+            "05_CAMELS_BR_precipitation_chirps",
+        )
+        forcing_dir_precipitation_mswep = camels_db.joinpath(
+            "06_CAMELS_BR_precipitation_mswep",
+            "06_CAMELS_BR_precipitation_mswep",
+        )
+        forcing_dir_precipitation_cpc = camels_db.joinpath(
+            "07_CAMELS_BR_precipitation_cpc",
+            "07_CAMELS_BR_precipitation_cpc",
+        )
+        forcing_dir_evapotransp_gleam = camels_db.joinpath(
+            "08_CAMELS_BR_evapotransp_gleam",
+            "08_CAMELS_BR_evapotransp_gleam",
+        )
+        forcing_dir_evapotransp_mgb = camels_db.joinpath(
+            "09_CAMELS_BR_evapotransp_mgb",
+            "09_CAMELS_BR_evapotransp_mgb",
+        )
+        forcing_dir_potential_evapotransp_gleam = camels_db.joinpath(
+            "10_CAMELS_BR_potential_evapotransp_gleam",
+            "10_CAMELS_BR_potential_evapotransp_gleam",
+        )
+        forcing_dir_temperature_min_cpc = camels_db.joinpath(
+            "11_CAMELS_BR_temperature_min_cpc",
+            "11_CAMELS_BR_temperature_min_cpc",
+        )
+        forcing_dir_temperature_mean_cpc = camels_db.joinpath(
+            "12_CAMELS_BR_temperature_mean_cpc",
+            "12_CAMELS_BR_temperature_mean_cpc",
+        )
+        forcing_dir_temperature_max_cpc = camels_db.joinpath(
+            "13_CAMELS_BR_temperature_max_cpc",
+            "13_CAMELS_BR_temperature_max_cpc",
+        )
+        return collections.OrderedDict(
+            CAMELS_DIR=camels_db,
+            CAMELS_FLOW_DIR=[
+                flow_dir_m3s,
+                flow_dir_mm_selected_catchments,
+                flow_dir_simulated,
+            ],
+            CAMELS_FORCING_DIR=[
+                forcing_dir_precipitation_chirps,
+                forcing_dir_precipitation_mswep,
+                forcing_dir_precipitation_cpc,
+                forcing_dir_evapotransp_gleam,
+                forcing_dir_evapotransp_mgb,
+                forcing_dir_potential_evapotransp_gleam,
+                forcing_dir_temperature_min_cpc,
+                forcing_dir_temperature_mean_cpc,
+                forcing_dir_temperature_max_cpc,
+            ],
+            CAMELS_ATTR_DIR=attr_dir,
+            CAMELS_ATTR_KEY_LST=attr_key_lst,
+            CAMELS_GAUGE_FILE=gauge_id_file,
+            CAMELS_BASINS_SHP_FILE=camels_shp_file,
+        )
+
+    def _set_data_source_camelsaus_describe(self, camels_db):
+        # id and name
+        gauge_id_file = camels_db.joinpath(
+            "01_id_name_metadata",
+            "01_id_name_metadata",
+            "id_name_metadata.csv",
+        )
+        # shp file of basins
+        camels_shp_file = camels_db.joinpath(
+            "02_location_boundary_area",
+            "02_location_boundary_area",
+            "shp",
+            "CAMELS_AUS_BasinOutlets_adopted.shp",
+        )
+        # config of flow data
+        flow_dir = camels_db.joinpath("03_streamflow", "03_streamflow")
+        # attr
+        attr_dir = camels_db.joinpath("04_attributes", "04_attributes")
+        # forcing
+        forcing_dir = camels_db.joinpath("05_hydrometeorology", "05_hydrometeorology")
+
+        return collections.OrderedDict(
+            CAMELS_DIR=camels_db,
+            CAMELS_FLOW_DIR=flow_dir,
+            CAMELS_FORCING_DIR=forcing_dir,
+            CAMELS_ATTR_DIR=attr_dir,
+            CAMELS_GAUGE_FILE=gauge_id_file,
+            CAMELS_BASINS_SHP_FILE=camels_shp_file,
+        )
+
+    def _set_data_source_camelsus_describe(self, camels_db):
+        # shp file of basins
+        camels_shp_file = camels_db.joinpath(
+            "basin_set_full_res", "HCDN_nhru_final_671.shp"
+        )
+        # config of flow data
+        flow_dir = camels_db.joinpath(
+            "basin_timeseries_v1p2_metForcing_obsFlow",
+            "basin_dataset_public_v1p2",
+            "usgs_streamflow",
+        )
+        flow_after_2015_dir = camels_db.joinpath(
+            "camels_streamflow", "camels_streamflow"
+        )
+        # forcing
+        forcing_dir = camels_db.joinpath(
+            "basin_timeseries_v1p2_metForcing_obsFlow",
+            "basin_dataset_public_v1p2",
+            "basin_mean_forcing",
+        )
+        forcing_types = ["daymet", "maurer", "nldas"]
+        # attr
+        attr_dir = camels_db
+        gauge_id_file = attr_dir.joinpath("camels_name.txt")
+        attr_key_lst = ["topo", "clim", "hydro", "vege", "soil", "geol"]
+        base_url = "https://gdex.ucar.edu/dataset/camels"
+        download_url_lst = [
+            f"{base_url}/file/basin_set_full_res.zip",
+            # f"{base_url}/file/basin_timeseries_v1p2_metForcing_obsFlow.zip",
+            f"{base_url}/file/camels_attributes_v2.0.xlsx",
+            f"{base_url}/file/camels_clim.txt",
+            f"{base_url}/file/camels_geol.txt",
+            f"{base_url}/file/camels_hydro.txt",
+            f"{base_url}/file/camels_name.txt",
+            f"{base_url}/file/camels_soil.txt",
+            f"{base_url}/file/camels_topo.txt",
+            f"{base_url}/file/camels_vege.txt",
+        ]
+
+        return collections.OrderedDict(
+            CAMELS_DIR=camels_db,
+            CAMELS_FLOW_DIR=flow_dir,
+            CAMELS_FLOW_AFTER2015_DIR=flow_after_2015_dir,
+            CAMELS_FORCING_DIR=forcing_dir,
+            CAMELS_FORCING_TYPE=forcing_types,
+            CAMELS_ATTR_DIR=attr_dir,
+            CAMELS_ATTR_KEY_LST=attr_key_lst,
+            CAMELS_GAUGE_FILE=gauge_id_file,
+            CAMELS_BASINS_SHP_FILE=camels_shp_file,
+            CAMELS_DOWNLOAD_URL_LST=download_url_lst,
+        )
+
     def download_data_source(self) -> None:
         """
         Download the required zip files
 
         Now we only support CAMELS-US's downloading.
         For others, please download it manually,
         and put all files of a dataset in one directory.
@@ -445,63 +457,50 @@
         Returns
         -------
         np.array
             attribute types
         """
         data_folder = self.data_source_description["CAMELS_ATTR_DIR"]
         if self.region == "US":
-            var_dict = dict()
-            var_lst = list()
-            key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
-            for key in key_lst:
-                data_file = os.path.join(data_folder, "camels_" + key + ".txt")
-                data_temp = pd.read_csv(data_file, sep=";")
-                var_lst_temp = list(data_temp.columns[1:])
-                var_dict[key] = var_lst_temp
-                var_lst.extend(var_lst_temp)
-            return np.array(var_lst)
+            return self._get_constant_cols_some(data_folder, "camels_", ".txt", ";")
         elif self.region == "AUS":
             attr_all_file = os.path.join(
                 self.data_source_description["CAMELS_DIR"],
                 "CAMELS_AUS_Attributes-Indices_MasterTable.csv",
             )
             camels_aus_attr_indices_data = pd.read_csv(attr_all_file, sep=",")
             # exclude station id
             return camels_aus_attr_indices_data.columns.values[1:]
         elif self.region == "BR":
-            var_dict = dict()
-            var_lst = list()
-            key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
-            for key in key_lst:
-                data_file = os.path.join(data_folder, "camels_br_" + key + ".txt")
-                data_temp = pd.read_csv(data_file, sep="\s+")
-                var_lst_temp = list(data_temp.columns[1:])
-                var_dict[key] = var_lst_temp
-                var_lst.extend(var_lst_temp)
-            return np.array(var_lst)
+            return self._get_constant_cols_some(
+                data_folder, "camels_br_", ".txt", "\s+"
+            )
         elif self.region == "CL":
             camels_cl_attr_data = self.sites
             # exclude station id
             return camels_cl_attr_data.index.values
         elif self.region == "GB":
-            var_dict = dict()
-            var_lst = list()
-            key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
-            for key in key_lst:
-                data_file = os.path.join(
-                    data_folder, "CAMELS_GB_" + key + "_attributes.csv"
-                )
-                data_temp = pd.read_csv(data_file, sep=",")
-                var_lst_temp = list(data_temp.columns[1:])
-                var_dict[key] = var_lst_temp
-                var_lst.extend(var_lst_temp)
-            return np.array(var_lst)
+            return self._get_constant_cols_some(
+                data_folder, "CAMELS_GB_", "_attributes.csv", ","
+            )
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
 
+    def _get_constant_cols_some(self, data_folder, arg1, arg2, sep):
+        var_dict = {}
+        var_lst = []
+        key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
+        for key in key_lst:
+            data_file = os.path.join(data_folder, arg1 + key + arg2)
+            data_temp = pd.read_csv(data_file, sep=sep)
+            var_lst_temp = list(data_temp.columns[1:])
+            var_dict[key] = var_lst_temp
+            var_lst.extend(var_lst_temp)
+        return np.array(var_lst)
+
     def get_relevant_cols(self) -> np.array:
         """
         all readable forcing types
 
         Returns
         -------
         np.array
@@ -649,24 +648,28 @@
             usgs_id + "_streamflow_qc.txt",
         )
         data_temp = pd.read_csv(usgs_file, sep=r"\s+", header=None)
         obs = data_temp[4].values
         obs[obs < 0] = np.nan
         t_lst = hydro_utils.t_range_days(t_range)
         nt = t_lst.shape[0]
-        if len(obs) != nt:
-            out = np.full([nt], np.nan)
-            df_date = data_temp[[1, 2, 3]]
-            df_date.columns = ["year", "month", "day"]
-            date = pd.to_datetime(df_date).values.astype("datetime64[D]")
-            [C, ind1, ind2] = np.intersect1d(date, t_lst, return_indices=True)
-            out[ind2] = obs[ind1]
-        else:
-            out = obs
-        return out
+        return (
+            self._read_usgs_gage_for_some(nt, data_temp, t_lst, obs)
+            if len(obs) != nt
+            else obs
+        )
+
+    def _read_usgs_gage_for_some(self, nt, data_temp, t_lst, obs):
+        result = np.full([nt], np.nan)
+        df_date = data_temp[[1, 2, 3]]
+        df_date.columns = ["year", "month", "day"]
+        date = pd.to_datetime(df_date).values.astype("datetime64[D]")
+        [C, ind1, ind2] = np.intersect1d(date, t_lst, return_indices=True)
+        result[ind2] = obs[ind1]
+        return result
 
     def read_camels_streamflow(self, usgs_id, t_range):
         """
         read streamflow data of a station for date after 2015 from CAMELS-US
 
         The streamflow data is downloaded from USGS website by HyRivers tools
 
@@ -691,24 +694,29 @@
             usgs_id + "_streamflow_qc.txt",
         )
         data_temp = pd.read_csv(usgs_file, sep=",", header=None, skiprows=1)
         obs = data_temp[4].values
         obs[obs < 0] = np.nan
         t_lst = hydro_utils.t_range_days(t_range)
         nt = t_lst.shape[0]
-        if len(obs) != nt:
-            out = np.full([nt], np.nan)
-            df_date = data_temp[[1, 2, 3]]
-            df_date.columns = ["year", "month", "day"]
-            date = pd.to_datetime(df_date).values.astype("datetime64[D]")
-            [C, ind1, ind2] = np.intersect1d(date, t_lst, return_indices=True)
-            out[ind2] = obs[ind1]
-        else:
-            out = obs
-        return out
+        return (
+            self._extracted_from_read_camels_streamflow_33(nt, data_temp, t_lst, obs)
+            if len(obs) != nt
+            else obs
+        )
+
+    # TODO Rename this here and in `read_camels_streamflow`
+    def _extracted_from_read_camels_streamflow_33(self, nt, data_temp, t_lst, obs):
+        result = np.full([nt], np.nan)
+        df_date = data_temp[[1, 2, 3]]
+        df_date.columns = ["year", "month", "day"]
+        date = pd.to_datetime(df_date).values.astype("datetime64[D]")
+        [C, ind1, ind2] = np.intersect1d(date, t_lst, return_indices=True)
+        result[ind2] = obs[ind1]
+        return result
 
     def read_br_gage_flow(self, gage_id, t_range, flow_type):
         """
         Read gage's streamflow from CAMELS-BR
 
         Parameters
         ----------
@@ -736,16 +744,15 @@
             flow_type = "simulated_streamflow"
         gage_file = os.path.join(dir_, gage_id + "_" + flow_type + ".txt")
         data_temp = pd.read_csv(gage_file, sep=r"\s+")
         obs = data_temp.iloc[:, 3].values
         obs[obs < 0] = np.nan
         df_date = data_temp[["year", "month", "day"]]
         date = pd.to_datetime(df_date).values.astype("datetime64[D]")
-        out = time_intersect_dynamic_data(obs, date, t_range)
-        return out
+        return time_intersect_dynamic_data(obs, date, t_range)
 
     def read_gb_gage_flow_forcing(self, gage_id, t_range, var_type):
         """
         Read gage's streamflow or forcing from CAMELS-GB
 
         Parameters
         ----------
@@ -769,16 +776,15 @@
             "CAMELS_GB_hydromet_timeseries_" + gage_id + "_19701001-20150930.csv",
         )
         data_temp = pd.read_csv(gage_file, sep=",")
         obs = data_temp[var_type].values
         if var_type in ["discharge_spec", "discharge_vol"]:
             obs[obs < 0] = np.nan
         date = pd.to_datetime(data_temp["date"]).values.astype("datetime64[D]")
-        out = time_intersect_dynamic_data(obs, date, t_range)
-        return out
+        return time_intersect_dynamic_data(obs, date, t_range)
 
     def read_target_cols(
         self,
         gage_id_lst: Union[list, np.array] = None,
         t_range: list = None,
         target_cols: Union[list, np.array] = None,
         **kwargs,
@@ -1009,18 +1015,15 @@
     def read_forcing_gage(self, usgs_id, var_lst, t_range_list, forcing_type="daymet"):
         # data_source = daymet or maurer or nldas
         logging.debug("reading %s forcing data", usgs_id)
         gage_id_df = self.sites
         huc = gage_id_df[gage_id_df["gauge_id"] == usgs_id]["huc_02"].values[0]
 
         data_folder = self.data_source_description["CAMELS_FORCING_DIR"]
-        if forcing_type == "daymet":
-            temp_s = "cida"
-        else:
-            temp_s = forcing_type
+        temp_s = "cida" if forcing_type == "daymet" else forcing_type
         data_file = os.path.join(
             data_folder,
             forcing_type,
             huc,
             "%s_lump_%s_forcing_leap.txt" % (usgs_id, temp_s),
         )
         data_temp = pd.read_csv(data_file, sep=r"\s+", header=None, skiprows=4)
@@ -1081,16 +1084,15 @@
         ]:
             var_type = var_type[:-4]
         gage_file = os.path.join(dir_, gage_id + "_" + var_type + ".txt")
         data_temp = pd.read_csv(gage_file, sep=r"\s+")
         obs = data_temp.iloc[:, 3].values
         df_date = data_temp[["year", "month", "day"]]
         date = pd.to_datetime(df_date).values.astype("datetime64[D]")
-        out = time_intersect_dynamic_data(obs, date, t_range)
-        return out
+        return time_intersect_dynamic_data(obs, date, t_range)
 
     def read_relevant_cols(
         self,
         gage_id_lst: list = None,
         t_range: list = None,
         var_lst: list = None,
         forcing_type="daymet",
@@ -1132,29 +1134,28 @@
                         "01_precipitation_timeseries",
                     )
                 elif "et_" in var_lst[k] or "evap_" in var_lst[k]:
                     forcing_dir = os.path.join(
                         self.data_source_description["CAMELS_FORCING_DIR"],
                         "02_EvaporativeDemand_timeseries",
                     )
+                elif "_AWAP" in var_lst[k]:
+                    forcing_dir = os.path.join(
+                        self.data_source_description["CAMELS_FORCING_DIR"],
+                        "03_Other",
+                        "AWAP",
+                    )
+                elif "_SILO" in var_lst[k]:
+                    forcing_dir = os.path.join(
+                        self.data_source_description["CAMELS_FORCING_DIR"],
+                        "03_Other",
+                        "SILO",
+                    )
                 else:
-                    if "_AWAP" in var_lst[k]:
-                        forcing_dir = os.path.join(
-                            self.data_source_description["CAMELS_FORCING_DIR"],
-                            "03_Other",
-                            "AWAP",
-                        )
-                    elif "_SILO" in var_lst[k]:
-                        forcing_dir = os.path.join(
-                            self.data_source_description["CAMELS_FORCING_DIR"],
-                            "03_Other",
-                            "SILO",
-                        )
-                    else:
-                        raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
+                    raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
                 forcing_data = pd.read_csv(
                     os.path.join(forcing_dir, var_lst[k] + ".csv")
                 )
                 df_date = forcing_data[["year", "month", "day"]]
                 date = pd.to_datetime(df_date).values.astype("datetime64[D]")
                 [c, ind1, ind2] = np.intersect1d(
                     date, t_range_list, return_indices=True
@@ -1202,18 +1203,18 @@
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
         return x
 
     def read_attr_all(self):
         data_folder = self.data_source_description["CAMELS_ATTR_DIR"]
         key_lst = self.data_source_description["CAMELS_ATTR_KEY_LST"]
-        f_dict = dict()  # factorize dict
-        var_dict = dict()
-        var_lst = list()
-        out_lst = list()
+        f_dict = {}
+        var_dict = {}
+        var_lst = []
+        out_lst = []
         gage_dict = self.sites
         if self.region == "US":
             camels_str = "camels_"
             sep_ = ";"
         elif self.region == "BR":
             camels_str = "camels_br_"
             sep_ = "\s+"
@@ -1279,15 +1280,15 @@
                 columns=all_attr_tmp.index,
             )
             # some none str attributes are treated as str, we need to trans them to float
             all_cols = all_attr.columns
             for col in all_cols:
                 try:
                     all_attr[col] = all_attr[col].astype(float)
-                except:
+                except Exception:
                     continue
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
         # gage_all_attr = all_attr[all_attr['station_id'].isin(gage_id_lst)]
         var_lst = self.get_constant_cols().tolist()
         data_temp = all_attr[var_lst]
         # for factorized data, we need factorize all gages' data to keep the factorized number same all the time
@@ -1366,40 +1367,39 @@
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
         ind_var = [var_lst_all.index(var) for var in var_lst]
         id_lst_all = self.read_object_ids()
         # Notice the sequence of station ids ! Some id_lst_all are not sorted, so don't use np.intersect1d
         ind_grid = [id_lst_all.tolist().index(tmp) for tmp in gage_id_lst]
         temp = attr_all[ind_grid, :]
         out = temp[:, ind_var]
-        if is_return_dict:
-            return out, var_dict, f_dict
-        else:
-            return out
+        return (out, var_dict, f_dict) if is_return_dict else out
 
-    def read_basin_area(self, object_ids) -> np.array:
+    def read_area(self, gage_id_lst) -> np.array:
         if self.region == "US":
-            return self.read_constant_cols(
-                object_ids, ["area_gages2"], is_return_dict=False
-            )
+            return self.read_attr_xrdataset(gage_id_lst, ["area_gages2"])
         elif self.region == "AUS":
             return self.read_constant_cols(
-                object_ids, ["catchment_area"], is_return_dict=False
+                gage_id_lst, ["catchment_area"], is_return_dict=False
             )
         elif self.region in ["BR", "CL", "GB"]:
-            return self.read_constant_cols(object_ids, ["area"], is_return_dict=False)
+            return self.read_constant_cols(gage_id_lst, ["area"], is_return_dict=False)
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
 
-    def read_mean_prep(self, object_ids) -> np.array:
+    def read_mean_prcp(self, gage_id_lst) -> np.array:
         if self.region in ["US", "AUS", "BR", "GB"]:
-            return self.read_constant_cols(object_ids, ["p_mean"], is_return_dict=False)
+            if self.region == "US":
+                return self.read_attr_xrdataset(gage_id_lst, ["p_mean"])
+            return self.read_constant_cols(
+                gage_id_lst, ["p_mean"], is_return_dict=False
+            )
         elif self.region == "CL":
             # there are different p_mean values for different forcings, here we chose p_mean_cr2met now
             return self.read_constant_cols(
-                object_ids, ["p_mean_cr2met"], is_return_dict=False
+                gage_id_lst, ["p_mean_cr2met"], is_return_dict=False
             )
         else:
             raise NotImplementedError(CAMELS_NO_DATASET_ERROR_LOG)
 
     def cache_forcing_np_json(self):
         """
         Save all daymet basin-forcing data in a numpy array file in the cache directory.
@@ -1463,22 +1463,25 @@
         data = self.read_target_cols(
             gage_id_lst=basins,
             t_range=t_range,
             target_cols=variables,
         )
         np.save(cache_npy_file, data)
 
-    def cache_attributes_feather(self):
+    def cache_attributes_xrdataset(self):
         """Convert all the attributes to a single dataframe
         TODO: now only support CAMELS-US
 
         Returns
         -------
         None
         """
+        # NOTICE: although it seems that we don't use pint_xarray, we have to import this package
+        import pint_xarray
+
         attr_files = self.data_source_dir.glob("camels_*.txt")
         attrs = {
             f.stem.split("_")[1]: pd.read_csv(
                 f, sep=";", index_col=0, dtype={"huc_02": str, "gauge_id": str}
             )
             for f in attr_files
         }
@@ -1493,49 +1496,115 @@
                 (name[0], name[1].upper() if len(name[1]) == 2 else name[1].title())
             )
 
         attrs_df["gauge_name"] = [fix_station_nm(n) for n in attrs_df["gauge_name"]]
         obj_cols = attrs_df.columns[attrs_df.dtypes == "object"]
         for c in obj_cols:
             attrs_df[c] = attrs_df[c].str.strip().astype(str)
-        cache_attrs_df_file = CACHE_DIR.joinpath("camels_attributes_v2.0.feather")
-        attrs_df.reset_index().to_feather(cache_attrs_df_file)
+        # unify id to basin
+        attrs_df.index.name = "basin"
+        # We use xarray dataset to cache all data
+        ds_from_df = attrs_df.to_xarray()
+        units = [
+            "degrees",  # gauge_lat
+            "degrees",  # gauge_lon
+            "m",  # elev_mean
+            "m/km",  # slope_mean
+            "km^2",  # area_gages2
+            "km^2",  # area_geospa_fabric
+            "dimensionless",  # geol_1st_class
+            "dimensionless",  # glim_1st_class_frac
+            "dimensionless",  # geol_2nd_class
+            "dimensionless",  # glim_2nd_class_frac
+            "dimensionless",  # carbonate_rocks_frac
+            "dimensionless",  # geol_porostiy
+            "m^2",  # geol_permeability
+            "dimensionless",  # frac_forest
+            "dimensionless",  # lai_max
+            "dimensionless",  # lai_diff
+            "dimensionless",  # gvf_max
+            "dimensionless",  # gvf_diff
+            "dimensionless",  # dom_land_cover_frac
+            "dimensionless",  # dom_land_cover
+            "m",  # root_depth_50
+            "m",  # root_depth_99
+            "mm/day",  # q_mean
+            "dimensionless",  # runoff_ratio
+            "dimensionless",  # slope_fdc
+            "dimensionless",  # baseflow_index
+            "dimensionless",  # stream_elas
+            "mm/day",  # q5
+            "mm/day",  # q95
+            "days/year",  # high_q_freq
+            "day",  # high_q_dur
+            "days/year",  # low_q_freq
+            "day",  # low_q_dur
+            "percent",  # zero_q_freq
+            "dimensionless",  # hfd_mean, day of year
+            "m",  # soil_depth_pelletier
+            "m",  # soil_depth_statsgo
+            "dimensionless",  # soil_porosity
+            "cm/hr",  # soil_conductivity
+            "m",  # max_water_content
+            "percent",  # sand_frac
+            "percent",  # silt_frac
+            "percent",  # clay_frac
+            "percent",  # water_frac
+            "percent",  # organic_frac
+            "percent",  # other_frac
+            "mm/day",  # p_mean
+            "mm/day",  # pet_mean
+            "dimensionless",  # p_seasonality
+            "dimensionless",  # frac_snow
+            "dimensionless",  # aridity
+            "days/year",  # high_prec_freq
+            "day",  # high_prec_dur
+            "dimensionless",  # high_prec_timing, it is season: spring, summer, fall, winter
+            "days/year",  # low_prec_freq
+            "day",  # low_prec_dur
+            "dimensionless",  # low_prec_timing, season
+            "dimensionless",  # huc_02
+            "dimensionless",  # gauge_name
+        ]
+        # Assign units to the variables in the Dataset
+        for col, unit in zip(list(ds_from_df), units):
+            ds_from_df[col].attrs["units"] = unit
+        return ds_from_df
 
     def cache_streamflow_xrdataset(self):
         """Save all basins' streamflow data in a netcdf file in the cache directory
 
         TODO: ONLY SUPPORT CAMELS-US now
         """
         cache_npy_file = CACHE_DIR.joinpath("camels_streamflow.npy")
         json_file = CACHE_DIR.joinpath("camels_streamflow.json")
         if (not os.path.isfile(cache_npy_file)) or (not os.path.isfile(json_file)):
             self.cache_streamflow_np_json()
         streamflow = np.load(cache_npy_file)
         with open(json_file, "r") as fp:
             streamflow_dict = json.load(fp, object_pairs_hook=collections.OrderedDict)
-        import xarray as xr
+        import pint_xarray
 
         basins = streamflow_dict["basin"]
         times = pd.date_range(
             streamflow_dict["time"][0], periods=len(streamflow_dict["time"])
         )
-        streamflow_ds = xr.Dataset(
+        return xr.Dataset(
             {
                 "streamflow": (
                     ["basin", "time"],
                     streamflow.reshape(streamflow.shape[0], streamflow.shape[1]),
+                    {"units": "foot^3/s"},
                 )
             },
             coords={
                 "basin": basins,
                 "time": times,
             },
         )
-        streamflow_ds["streamflow"].attrs["units"] = "cfs"
-        streamflow_ds.to_netcdf(CACHE_DIR.joinpath("camels_streamflow.nc"))
 
     def cache_forcing_xrdataset(self):
         """Save all daymet basin-forcing data in a netcdf file in the cache directory.
 
         TODO: ONLY SUPPORT CAMELS-US now
         """
         cache_npy_file = CACHE_DIR.joinpath("camels_daymet_forcing.npy")
@@ -1543,23 +1612,24 @@
         if (not os.path.isfile(cache_npy_file)) or (not os.path.isfile(json_file)):
             self.cache_forcing_np_json()
         daymet_forcing = np.load(cache_npy_file)
         with open(json_file, "r") as fp:
             daymet_forcing_dict = json.load(
                 fp, object_pairs_hook=collections.OrderedDict
             )
-        import xarray as xr
+        import pint_xarray
 
         basins = daymet_forcing_dict["basin"]
         times = pd.date_range(
             daymet_forcing_dict["time"][0], periods=len(daymet_forcing_dict["time"])
         )
         variables = daymet_forcing_dict["variable"]
-        units = ["s", "mm/day", "W/m2", "mm", "C", "C", "Pa"]
-        forcing_ds = xr.Dataset(
+        # All units' names are from Pint https://github.com/hgrecco/pint/blob/master/pint/default_en.txt
+        units = ["s", "mm/day", "W/m^2", "mm", "°C", "°C", "Pa"]
+        return xr.Dataset(
             data_vars={
                 **{
                     variables[i]: (
                         ["basin", "time"],
                         daymet_forcing[:, :, i],
                         {"units": units[i]},
                     )
@@ -1568,8 +1638,41 @@
             },
             coords={
                 "basin": basins,
                 "time": times,
             },
             attrs={"forcing_type": "daymet"},
         )
-        forcing_ds.to_netcdf(CACHE_DIR.joinpath("camels_daymet_forcing.nc"))
+
+    def cache_xrdataset(self):
+        """Save all data in a netcdf file in the cache directory"""
+        warnings.warn("Check you units of all variables")
+        ds_attr = self.cache_attributes_xrdataset()
+        ds_attr.to_netcdf(CACHE_DIR.joinpath("camelsus_attributes.nc"))
+        ds_streamflow = self.cache_streamflow_xrdataset()
+        ds_forcing = self.cache_forcing_xrdataset()
+        ds = xr.merge([ds_streamflow, ds_forcing])
+        ds.to_netcdf(CACHE_DIR.joinpath("camelsus_timeseries.nc"))
+
+    def read_ts_xrdataset(
+        self,
+        gage_id_lst: list = None,
+        t_range: list = None,
+        var_lst: list = None,
+        **kwargs,
+    ):
+        if var_lst is None:
+            return None
+        ts = xr.open_dataset(CACHE_DIR.joinpath("camelsus_timeseries.nc"))
+        all_vars = ts.data_vars
+        if any(var not in ts.variables for var in var_lst):
+            raise ValueError(f"var_lst must all be in {all_vars}")
+        return ts[var_lst].sel(basin=gage_id_lst, time=slice(t_range[0], t_range[1]))
+
+    def read_attr_xrdataset(self, gage_id_lst=None, var_lst=None, **kwargs):
+        if var_lst is None or len(var_lst) == 0:
+            return None
+        attr = xr.open_dataset(CACHE_DIR.joinpath("camelsus_attributes.nc"))
+        if "all_number" in list(kwargs.keys()) and kwargs["all_number"]:
+            attr_num = hydro_utils.map_string_vars(attr)
+            return attr_num[var_lst].sel(basin=gage_id_lst)
+        return attr[var_lst].sel(basin=gage_id_lst)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hydrodataset-0.1.0/hydrodataset/caravan.py` & `hydrodataset-0.1.2/hydrodataset/caravan.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset/grdc.py` & `hydrodataset-0.1.2/hydrodataset/grdc.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset/hydro_dataset.py` & `hydrodataset-0.1.2/hydrodataset/hydro_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-09-05 23:20:24
-LastEditTime: 2022-09-07 10:07:34
+LastEditTime: 2023-07-27 21:44:01
 LastEditors: Wenyu Ouyang
 Description: main modules for hydrodataset
 FilePath: \hydrodataset\hydrodataset\hydro_dataset.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 from pathlib import Path
 from abc import ABC
@@ -13,14 +13,16 @@
 import numpy as np
 from hydrodataset import ROOT_DIR
 
 
 class HydroDataset(ABC):
     """An interface for Hydrological Dataset
 
+    For unit, we use Pint package's unit system -- unit registry
+
     Parameters
     ----------
     ABC : _type_
         _description_
     """
 
     def __init__(self, data_path):
@@ -75,7 +77,33 @@
     def get_target_cols(self) -> np.array:
         """the target cols in this data_source"""
         raise NotImplementedError
 
     def get_other_cols(self) -> dict:
         """the other cols in this data_source"""
         raise NotImplementedError
+
+    def cache_xrdataset(self, **kwargs):
+        """cache xarray dataset and pandas feather for faster reading"""
+        raise NotImplementedError
+
+    def read_ts_xrdataset(
+        self,
+        gage_id_lst: list = None,
+        t_range: list = None,
+        var_lst: list = None,
+        **kwargs
+    ):
+        """read time-series xarray dataset"""
+        raise NotImplementedError
+
+    def read_attr_xrdataset(self, gage_id_lst=None, var_lst=None, **kwargs):
+        """read attribute pandas feather"""
+        raise NotImplementedError
+
+    def read_area(self, gage_id_lst=None):
+        """read area of each basin/unit"""
+        raise NotImplementedError
+
+    def read_mean_prcp(self, gage_id_lst=None):
+        """read mean precipitation of each basin/unit"""
+        raise NotImplementedError
```

### Comparing `hydrodataset-0.1.0/hydrodataset/hydro_utils.py` & `hydrodataset-0.1.2/hydrodataset/hydro_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,47 @@
 """
 Author: Wenyu Ouyang
 Date: 2022-09-06 16:53:45
-LastEditTime: 2022-09-08 19:28:44
+LastEditTime: 2023-07-30 20:09:20
 LastEditors: Wenyu Ouyang
 Description: util functions
 FilePath: \hydrodataset\hydrodataset\hydro_utils.py
 Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 """
 import datetime as dt
 import io
 from pathlib import Path
 from typing import Union
 import zipfile
 import numpy as np
 import requests
 import async_retriever as ar
 from hydrodataset import CACHE_DIR
+import xarray as xr
+
+
+def map_string_vars(ds):
+    # Iterate over all variables in the dataset
+    for var in ds.data_vars:
+        # Check if the variable contains string data
+        if ds[var].dtype == object:
+            # Convert the DataArray to a pandas Series
+            var_series = ds[var].to_series()
+
+            # Get all unique strings and create a mapping to integers
+            unique_strings = sorted(var_series.unique())
+            mapping = {value: i for i, value in enumerate(unique_strings)}
+
+            # Apply the mapping to the series
+            mapped_series = var_series.map(mapping)
+
+            # Convert the series back to a DataArray and replace the old one in the Dataset
+            ds[var] = xr.DataArray(mapped_series)
+
+    return ds
 
 
 def download_one_zip(data_url: str, data_dir: str) -> None:
     """
     A normal way to download one zip file from url as data_file
 
     We recommend you to use async_retriever to download files
@@ -45,15 +67,15 @@
     Parameters
     ----------
     urls : list
         list of all urls
     the_dir : Path
         the directory containing all downloaded files
     """
-    cache_names = CACHE_DIR.joinpath(the_dir.stem + ".sqlite")
+    cache_names = CACHE_DIR.joinpath(f"{the_dir.stem}.sqlite")
     r = ar.retrieve(urls, "binary", cache_name=cache_names, ssl=False)
     files = [the_dir.joinpath(url.split("/")[-1]) for url in urls]
     [files[i].write_bytes(io.BytesIO(r[i]).getbuffer()) for i in range(len(files))]
 
 
 def zip_extract(the_dir) -> None:
     """Extract the downloaded zip files in the_dir"""
@@ -62,20 +84,17 @@
             # extract files to a directory named by f.stem
             zf.extractall(the_dir.joinpath(f.stem))
 
 
 def t_range_days(t_range, *, step=np.timedelta64(1, "D")):
     sd = dt.datetime.strptime(t_range[0], "%Y-%m-%d")
     ed = dt.datetime.strptime(t_range[1], "%Y-%m-%d")
-    t_array = np.arange(sd, ed, step)
-    return t_array
+    return np.arange(sd, ed, step)
 
 
 def t2str(t_: Union[str, dt.datetime]):
     if type(t_) is str:
-        t_str = dt.datetime.strptime(t_, "%Y-%m-%d")
-        return t_str
+        return dt.datetime.strptime(t_, "%Y-%m-%d")
     elif type(t_) is dt.datetime:
-        t = t_.strftime("%Y-%m-%d")
-        return t
+        return t_.strftime("%Y-%m-%d")
     else:
         raise NotImplementedError("We don't support this data type yet")
```

### Comparing `hydrodataset-0.1.0/hydrodataset/hysets.py` & `hydrodataset-0.1.2/hydrodataset/hysets.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset/lamah.py` & `hydrodataset-0.1.2/hydrodataset/lamah.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset/mopex.py` & `hydrodataset-0.1.2/hydrodataset/mopex.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset/multi_datasets.py` & `hydrodataset-0.1.2/hydrodataset/multi_datasets.py`

 * *Files identical despite different names*

### Comparing `hydrodataset-0.1.0/hydrodataset.egg-info/PKG-INFO` & `hydrodataset-0.1.2/hydrodataset.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrodataset
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Python package for downloading and reading hydrological datasets
 Home-page: https://github.com/OuyangWenyu/hydrodataset
 Author: Wenyu Ouyang
 Author-email: wenyuouyang@outlook.com
 License: MIT license
 Keywords: hydrodataset
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 <!--
  * @Author: Wenyu Ouyang
  * @Date: 2021-12-05 22:13:21
- * @LastEditTime: 2023-07-25 15:13:52
+ * @LastEditTime: 2023-07-26 13:35:41
  * @LastEditors: Wenyu Ouyang
  * @Description: README for hydrodataset
  * @FilePath: \hydrodataset\README.md
  * Copyright (c) 2021-2022 Wenyu Ouyang. All rights reserved.
 -->
 # hydrodataset
 
@@ -204,12 +204,16 @@
 | **Number** | **Dataset** | **Description**                                         |
 | ---------- | ----------- | ------------------------------------------------------- |
 | 1          | **CAMELS**  | CAMELS series datasets including CAMELS-AUS/BR/CL/GB/US |
 | 2          | **LamaH**   | LamaH-CE dataset for Central Europe                     |
 | 3          | **HYSETS**  | HYSETS dataset for North America                        |
 | 4          | **Caravan** | Caravan dataset for global                              |
 
+For units, we use [pint](https://github.com/hgrecco/pint), and [pint-xarray](https://github.com/xarray-contrib/pint-xarray) to handle them.
+
+We highly recommend you to use [xarray](http://xarray.pydata.org/en/stable/) to read the data, as it is a powerful tool for handling multi-dimensional data. Then, you can see the units of all variables in the xarray dataset.
+
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter) and the [giswqs/pypackage](https://github.com/giswqs/pypackage) project template.
 
 It was inspired by [HydroData](https://github.com/mikejohnson51/HydroData) and used some tools made by [cheginit](https://github.com/cheginit).
```

### Comparing `hydrodataset-0.1.0/hydrodataset.egg-info/SOURCES.txt` & `hydrodataset-0.1.2/hydrodataset.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,12 +16,8 @@
 hydrodataset/mopex.py
 hydrodataset/multi_datasets.py
 hydrodataset.egg-info/PKG-INFO
 hydrodataset.egg-info/SOURCES.txt
 hydrodataset.egg-info/dependency_links.txt
 hydrodataset.egg-info/not-zip-safe
 hydrodataset.egg-info/requires.txt
-hydrodataset.egg-info/top_level.txt
-test/test_camels.py
-test/test_caravan.py
-test/test_hysets.py
-test/test_multi_datasets.py
+hydrodataset.egg-info/top_level.txt
```

### Comparing `hydrodataset-0.1.0/setup.py` & `hydrodataset-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,70 @@
 #!/usr/bin/env python
 
-"""The setup script."""
+"""
+Author: Wenyu Ouyang
+Date: 2022-09-05 23:22:54
+LastEditTime: 2023-07-31 17:21:05
+LastEditors: Wenyu Ouyang
+Description: The setup script
+FilePath: /hydrodataset/setup.py
+Copyright (c) 2023-2024 Wenyu Ouyang. All rights reserved.
+"""
 
 import io
+import pathlib
 from os import path as op
 from setuptools import setup, find_packages
 
-with open('README.md') as readme_file:
+with open("README.md", "r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
-
 here = op.abspath(op.dirname(__file__))
 
+
 # get the dependencies and installs
 with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
     all_reqs = f.read().split("\n")
 
 install_requires = [x.strip() for x in all_reqs if "git+" not in x]
 dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
 
-requirements = [ ]
-
-setup_requirements = ['pytest-runner', ]
+requirements = []
 
-test_requirements = ['pytest>=3', ]
+setup_requirements = [
+    "pytest-runner",
+]
+
+test_requirements = [
+    "pytest>=3",
+]
 
 setup(
     author="Wenyu Ouyang",
-    author_email='wenyuouyang@outlook.com',
-    python_requires='>=3.7',
+    author_email="wenyuouyang@outlook.com",
+    python_requires=">=3.7",
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Development Status :: 2 - Pre-Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     description="A Python package for downloading and reading hydrological datasets",
     install_requires=install_requires,
     dependency_links=dependency_links,
     license="MIT license",
     long_description=readme,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
     include_package_data=True,
-    keywords='hydrodataset',
-    name='hydrodataset',
-    packages=find_packages(include=['hydrodataset', 'hydrodataset.*']),
+    keywords="hydrodataset",
+    name="hydrodataset",
+    packages=find_packages(include=["hydrodataset", "hydrodataset.*"]),
     setup_requires=setup_requirements,
-    test_suite='tests',
+    test_suite="tests",
     tests_require=test_requirements,
-    url='https://github.com/OuyangWenyu/hydrodataset',
-    version='0.1.0',
+    url="https://github.com/OuyangWenyu/hydrodataset",
+    version='0.1.2',
     zip_safe=False,
 )
```

