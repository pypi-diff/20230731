# Comparing `tmp/ww3py-0.0.1.tar.gz` & `tmp/ww3py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ww3py-0.0.1.tar", last modified: Mon Jan 30 06:36:59 2023, max compression
+gzip compressed data, was "dist/ww3py-0.0.3.tar", last modified: Mon Jul 31 14:02:04 2023, max compression
```

## Comparing `ww3py-0.0.1.tar` & `ww3py-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,34 @@
-drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:36:59.000000 ww3py-0.0.1/
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      596 2023-01-30 06:36:59.000000 ww3py-0.0.1/PKG-INFO
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       38 2023-01-30 06:36:59.000000 ww3py-0.0.1/setup.cfg
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     1044 2023-01-30 06:36:56.000000 ww3py-0.0.1/setup.py
-drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:36:59.000000 ww3py-0.0.1/ww3py/
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       39 2023-01-30 06:18:22.000000 ww3py-0.0.1/ww3py/__init__.py
-drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:36:59.000000 ww3py-0.0.1/ww3py/exec/
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 04:15:11.000000 ww3py-0.0.1/ww3py/exec/__init__.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     3221 2023-01-30 04:43:09.000000 ww3py-0.0.1/ww3py/exec/exe_ww3.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     3271 2023-01-30 04:43:40.000000 ww3py-0.0.1/ww3py/exec/pos_ww3.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    12912 2023-01-30 04:43:25.000000 ww3py-0.0.1/ww3py/exec/pre_ww3.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      683 2023-01-30 03:47:56.000000 ww3py-0.0.1/ww3py/exec/utils.py
-drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:36:59.000000 ww3py-0.0.1/ww3py/plot/
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:25:18.000000 ww3py-0.0.1/ww3py/plot/__init__.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      717 2023-01-30 03:47:56.000000 ww3py-0.0.1/ww3py/plot/init_custom.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    12070 2023-01-30 04:40:48.000000 ww3py-0.0.1/ww3py/plot/misc.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     1634 2023-01-30 03:47:56.000000 ww3py-0.0.1/ww3py/plot/soft_topo_cmap.py
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     4409 2023-01-30 03:47:56.000000 ww3py-0.0.1/ww3py/plot/utils.py
-drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-01-30 06:36:59.000000 ww3py-0.0.1/ww3py.egg-info/
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      596 2023-01-30 06:36:58.000000 ww3py-0.0.1/ww3py.egg-info/PKG-INFO
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      368 2023-01-30 06:36:58.000000 ww3py-0.0.1/ww3py.egg-info/SOURCES.txt
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        1 2023-01-30 06:36:58.000000 ww3py-0.0.1/ww3py.egg-info/dependency_links.txt
--rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        6 2023-01-30 06:36:58.000000 ww3py-0.0.1/ww3py.egg-info/top_level.txt
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      596 2023-07-31 14:02:04.000000 ww3py-0.0.3/PKG-INFO
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       38 2023-07-31 14:02:04.000000 ww3py-0.0.3/setup.cfg
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     1044 2023-07-31 13:59:31.000000 ww3py-0.0.3/setup.py
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       37 2023-01-31 04:47:25.000000 ww3py-0.0.3/ww3py/__init__.py
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py/exec/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       68 2023-01-31 04:33:40.000000 ww3py-0.0.3/ww3py/exec/__init__.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     3965 2023-07-22 12:19:17.000000 ww3py-0.0.3/ww3py/exec/exe_ww3.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     5306 2023-07-16 10:17:50.000000 ww3py-0.0.3/ww3py/exec/pos_ww3.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    13116 2023-07-22 12:10:07.000000 ww3py-0.0.3/ww3py/exec/pre_ww3.py
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py/plot/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      261 2023-07-27 04:54:58.000000 ww3py-0.0.3/ww3py/plot/__init__.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    10049 2023-06-14 21:49:15.000000 ww3py-0.0.3/ww3py/plot/dir_dist.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      730 2023-07-22 09:30:35.000000 ww3py-0.0.3/ww3py/plot/init_custom.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     6198 2023-03-27 14:18:30.000000 ww3py-0.0.3/ww3py/plot/misc.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     9408 2023-07-31 13:07:27.000000 ww3py-0.0.3/ww3py/plot/series.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     7765 2023-07-31 13:06:36.000000 ww3py-0.0.3/ww3py/plot/skill_1d_series.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     9604 2023-07-31 09:11:02.000000 ww3py-0.0.3/ww3py/plot/skill_2d_series.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     1639 2023-07-22 09:31:50.000000 ww3py-0.0.3/ww3py/plot/soft_topo_cmap.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     5305 2023-07-26 05:44:06.000000 ww3py-0.0.3/ww3py/plot/spectra_1d.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    19288 2023-07-31 09:05:22.000000 ww3py-0.0.3/ww3py/plot/spectra_2d.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)    21722 2023-07-31 13:42:27.000000 ww3py-0.0.3/ww3py/plot/src_terms.py
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py/util/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)       86 2023-07-04 03:59:11.000000 ww3py-0.0.3/ww3py/util/__init__.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     4110 2023-07-31 13:03:35.000000 ww3py-0.0.3/ww3py/util/customize.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     7898 2023-07-31 05:31:17.000000 ww3py-0.0.3/ww3py/util/data.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      683 2023-01-31 03:15:05.000000 ww3py-0.0.3/ww3py/util/files.py
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)     1498 2023-07-26 14:56:14.000000 ww3py-0.0.3/ww3py/util/misce.py
+drwxrwxr-x   0 fayalacruz (15350) punim1660 (11741)        0 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py.egg-info/
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      596 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py.egg-info/PKG-INFO
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)      612 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py.egg-info/SOURCES.txt
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        1 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py.egg-info/dependency_links.txt
+-rw-rw-r--   0 fayalacruz (15350) punim1660 (11741)        6 2023-07-31 14:02:04.000000 ww3py-0.0.3/ww3py.egg-info/top_level.txt
```

### Comparing `ww3py-0.0.1/PKG-INFO` & `ww3py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ww3py
-Version: 0.0.1
+Version: 0.0.3
 Summary: A handle python package to WWIII simulations
 Home-page: UNKNOWN
 Author: Franklin Ayala
 Author-email: <ffayalac@unal.edu.co>
 License: UNKNOWN
 Description: This is the first release for ww3py on 30/01/2023
 Keywords: python,first package
```

### Comparing `ww3py-0.0.1/setup.py` & `ww3py-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'A handle python package to WWIII simulations'
 LONG_DESCRIPTION = 'This is the first release for ww3py on 30/01/2023'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ww3py",
```

### Comparing `ww3py-0.0.1/ww3py/exec/exe_ww3.py` & `ww3py-0.0.3/ww3py/exec/exe_ww3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,79 @@
+import os,sys
+PROJECT_ROOT = os.path.abspath(os.path.join(
+                  os.path.dirname(__file__), 
+                  os.pardir)
+)
+sys.path.append(PROJECT_ROOT)
+
 import subprocess
-import os
 import shutil
-from . import utils
+import util
 import wget
 import fileinput
+import glob
 
 class buoys_matcher():
     def __init__(self,root_path,ini_date) -> None:
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.inp_plots_path = f'{root_path}info/plots/'
-    
+        self.idate = ini_date
+        self.url_sufixs = {'stdmet':'h','swden':'w','swr1':'j','swr2':'k','swdir':'d','swdir2':'i'}
+
     def dwnd_one_buoy(self,buoy_id):
-            name_buoy_file=buoy_id+'h2020.txt.gz'
-            url = 'https://www.ndbc.noaa.gov/data/historical/stdmet/'+name_buoy_file
-            filename = wget.download(url,self.inp_plots_path)
-            os.system(f'gzip -d {self.inp_plots_path}{name_buoy_file}')
-            os.system(f'rm {self.inp_plots_path}{name_buoy_file}')
+            self.path_buoy = f'{self.inp_plots_path}{buoy_id}/'
+            os.system(f'mkdir {self.path_buoy}')
+            for suf,label in self.url_sufixs.items():
+                name_buoy_file=f'{buoy_id}{label}{self.idate.strftime("%Y")}.txt.gz'
+                url = f'https://www.ndbc.noaa.gov/data/historical/{suf}/{name_buoy_file}'
+                filename = wget.download(url,self.path_buoy)
+
+                os.system(f'gzip -d {self.path_buoy}{name_buoy_file}')
 
     def dwnd_all_buoys(self):
         name_buoys=['42056','42057','42058','42059','42060']
         for buoy in name_buoys:
-            self.check_file=utils.verify_files(f'{self.inp_plots_path}{buoy}h2020.txt')
-            if not self.check_file:
+            if len(glob.glob(f'{self.inp_plots_path}{buoy}/*.txt'))==6:
+                print ('All buoy data is already downloaded')
+            else:
                 self.dwnd_one_buoy(buoy)
 
 class running_ww3():
-    def __init__(self,name,root_path,spartan_path,ini_date,shel_dict,run_mode):
+    def __init__(self,name,root_path,spartan_path,ini_date,exe_path,shel_dict,run_mode):
         self.name = name
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.spartan_path = spartan_path
         self.inp_path = f'{root_path}info/inp/'
+        self.exe_path = exe_path
         self.shel_dict = shel_dict
         self.run_mode = run_mode
         self.idate = ini_date
     
     def fill_shel(self):
         print ('\n*** Editing ww3_shel.inp ***\n')
         shutil.copy(f'{self.inp_path}ww3_shel.inp_code', f'{self.run_path}ww3_shel.inp')
-        utils.fill_files(f'{self.run_path}ww3_shel.inp',self.shel_dict)
+        util.fill_files(f'{self.run_path}ww3_shel.inp',self.shel_dict)
 
     def run_shel(self):
         print ('\n*** Running main program: ww3_shel ***\n')
         if self.run_mode!='spartan':
             f = open('shel.log', "w") 
             subprocess.call([f'{self.run_path}ww3_shel'],cwd=self.run_path,stdout=f)  
             shutil.move('shel.log', f'{self.run_path}shel.log')
         else:
             shutil.copy(f'{self.inp_path}template.slurm', f'{self.run_path}{self.name}.slurm')
             with fileinput.FileInput(f'{self.run_path}{self.name}.slurm',inplace=True, backup='') as file:
                 for line in file:
                     print(line.replace('name_job',self.name),end='')
 
             os.system(f'mkdir -p {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
-            os.system(f'cp -r {self.run_path}*.ww3 {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
-            os.system(f'cp -r {self.run_path}ww3_shel* {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
+            os.system(f'cp -r {self.run_path}wind.ww3 {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
+            os.system(f'cp -r {self.run_path}mod_def.ww3 {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
+            os.system(f'cp -r {self.run_path}ww3_shel.inp {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
+            os.system(f'ln -s {self.exe_path}ww3_shel {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
             os.system(f'cp -r {self.run_path}*.slurm {self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}')
         self.out_grd_path=f'{self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}/out_grd.ww3'
         self.out_pnt_path=f'{self.spartan_path}{self.idate.strftime("%Y%m%d%H")}_{self.name}/out_pnt.ww3'
-        if utils.verify_files(self.out_grd_path) and utils.verify_files(self.out_pnt_path):
+        if util.verify_files(self.out_grd_path) and util.verify_files(self.out_pnt_path):
             print('\n The case has been runned in Spartan \n')
         else:
             raise UserWarning('The slurm file has to be launched to the queue for the execution \n with 2 nodes and 16 tasks can take around 3.5 hours')
```

### Comparing `ww3py-0.0.1/ww3py/exec/pre_ww3.py` & `ww3py-0.0.3/ww3py/exec/pre_ww3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-# -*- coding: utf-8 -*-
-#!/usr/bin/python
+import os,sys
+PROJECT_ROOT = os.path.abspath(os.path.join(
+                  os.path.dirname(__file__), 
+                  os.pardir)
+)
+sys.path.append(PROJECT_ROOT)
 
 import subprocess
 import cdsapi
 from datetime import datetime
 import pandas as pd
-import os
 import numpy as np
 import shutil
-from . import utils
+import util
 import glob as glob
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 import cartopy.feature as cfeature
 from cartopy.mpl.ticker import LongitudeFormatter, LatitudeFormatter
 
 class oper_carpetas():
@@ -38,15 +41,15 @@
         self.raw_name = self.idate.strftime("%Y%m%d")+'_era5_raw.nc'
         self.fin_name = self.idate.strftime("%Y%m%d")+'_era5.nc'
         self.raw_path = f'{self.forc_path}{self.raw_name}'
         self.fin_path = f'{self.forc_path}{self.fin_name}'
 
     def dwnd_era5(self):
         print ('\n *** Downloading and modifying ERA5 data via cdsapi *** \n')
-        self.check_file=utils.verify_files(self.raw_path)
+        self.check_file=util.verify_files(self.raw_path)
         if not self.check_file:
             self.era5_var_ids = ['10m_u_component_of_wind','10m_v_component_of_wind']
             self.c = cdsapi.Client()
             self.hours = list(pd.date_range(datetime(1900,1,1,0,0),\
                     datetime(1900,1,1,23,0),freq='H').strftime('%H:%M'))
 
             self.dates=list(pd.date_range(self.idate.date(),self.edate.date(),freq='d').strftime('%Y-%m-%d'))
@@ -61,48 +64,49 @@
                 'date':self.dates[:],
                 'time':self.hours[:],
                 'format':'netcdf'
             },
                 self.raw_path)
 
     def mdf_era5(self):
-        self.check_file=utils.verify_files(self.fin_path)
+        self.check_file=util.verify_files(self.fin_path)
         if not self.check_file:
             # This can be done with xarray
             os.system(f'ncpdq -h -O -a -latitude {self.raw_path} {self.fin_path}') 
 
     def plt_era5(self):
         pass
     
     def lnk_era5(self):
-        utils.verify_links(self.fin_name,self.forc_path,self.run_path)
+        os.system(f'rm -rf {self.run_path}*.nc')
+        util.verify_links(self.fin_name,self.forc_path,self.run_path)
 
 class bthm_data():
     def __init__(self,root_path,gridgen_path,ini_date,name,res,sbst_grd):
         self.gridgen_path = gridgen_path 
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.inp_path = f'{root_path}info/inp/'
         self.info_grid_path = f'{root_path}info/gridgen/'
         self.name = name
         self.res = res
         self.sbst_grd = sbst_grd
         self.bath_files = ['bottom.inp','mask.inp','obstr.inp']
 
     def generate_bthm(self):
         print ('\n *** Generating bathymetry data with gridgen ***\n')
-        self.vrf_list = np.array([utils.verify_files(f'{self.info_grid_path}{file}') for file in self.bath_files])
+        self.vrf_list = np.array([util.verify_files(f'{self.info_grid_path}{file}') for file in self.bath_files])
 
         if np.all(self.vrf_list):
             print(f'The bathimetric files : {self.bath_files} already exist')
         else:        
             shutil.copy(f'{self.inp_path}create_grid_code.m', f'{self.info_grid_path}create_grid.m')
             self.gridgen_dict={'bin_path':f'{self.gridgen_path}bin/','reference_path':f'{self.gridgen_path}reference_data/',\
                             'output_path':self.info_grid_path,'res_x':self.res,'res_y':self.res,'name_case':self.name}
             self.gridgen_dict.update(self.sbst_grd)
-            utils.fill_files(f'{self.info_grid_path}create_grid.m',self.gridgen_dict)
+            util.fill_files(f'{self.info_grid_path}create_grid.m',self.gridgen_dict)
             print('Please run the following commands in a node in Spartan before to continue:\n. The atlab ')
             print(f'cd {self.info_grid_path}')
             print('matlab -nodisplay -nodesktop -batch "run create_grid.m"\n')
             raise UserWarning('The model will fail if the previous commands are not runned')
 
     def plt_bottom(self):
         self.bottom=np.genfromtxt(f'{self.info_grid_path}bottom.inp')
@@ -214,60 +218,62 @@
         self.cbar2=plt.colorbar(cf2,cax=self.cax2,orientation="vertical",pad=0.12)
         self.cbar2.ax.set_ylabel('obstruction scale',rotation=90,labelpad=0.45)
 
         self.fig.savefig(f'{self.info_grid_path}Sy_obstr_gridgen.png',dpi=1000,bbox_inches='tight',pad_inches=0.05)
 
     def lnk_bthm_data(self):
         for file in self.bath_files:
-            utils.verify_links(file,self.info_grid_path,self.run_path)
+            util.verify_links(file,self.info_grid_path,self.run_path)
 
 class exec_files():
     def __init__(self,root_path,exe_path,ini_date):
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.exe_path = exe_path
     
     def copy_exe(self):
-        os.system(f'cp {self.exe_path}* {self.run_path}')
+        os.system(f'ln -s {self.exe_path}* {self.run_path}')
 
 class strt_grd_inp():
     def __init__(self,root_path,ini_date,start_dict,grid_dict):
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.inp_path = f'{root_path}info/inp/'
         self.start_dict = start_dict
         self.grid_dict = grid_dict
 
     def fill_grd(self):
         print ('\n*** Editing ww3_grid.inp and ww3_strt.inp ***\n')
         shutil.copy(f'{self.inp_path}ww3_grid.inp_code', f'{self.run_path}ww3_grid.inp')
-        utils.fill_files(f'{self.run_path}ww3_grid.inp',self.grid_dict)
+        util.fill_files(f'{self.run_path}ww3_grid.inp',self.grid_dict)
 
     def fill_strt(self):
         shutil.copy(f'{self.inp_path}ww3_strt.inp_code', f'{self.run_path}ww3_strt.inp')
-        utils.fill_files(f'{self.run_path}ww3_strt.inp',self.start_dict)
+        util.fill_files(f'{self.run_path}ww3_strt.inp',self.start_dict)
 
 class prnc_inp():
     def __init__(self,root_path,ini_date,prnc_dict):
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.inp_path = f'{root_path}info/inp/'
         self.prnc_dict = prnc_dict
 
     def fill_prnc(self):
         print ('\n*** Editing ww3_prnc.inp ***\n')
         shutil.copy(f'{self.inp_path}ww3_prnc.inp_code', f'{self.run_path}ww3_prnc.inp')
-        utils.fill_files(f'{self.run_path}ww3_prnc.inp',self.prnc_dict)
+        util.fill_files(f'{self.run_path}ww3_prnc.inp',self.prnc_dict)
 
 class exe_pre():
     def __init__(self,root_path,exe_path,ini_date):
         self.run_path = f'{root_path}run/{ini_date.strftime("%Y%m%d%H")}/'
         self.exe_path = exe_path
         self.pre_programs = ['ww3_grid','ww3_strt','ww3_prnc']
 
     def run_exe_pre(self):
         print ('\n*** Running pre-processing programs of ww3 ***\n')
         for program in self.pre_programs:
             f = open(f'{self.run_path}{program[4:]}.log', "w") # this creates the file
             subprocess.call([f'{self.run_path}{program}'],cwd=self.run_path,stdout=f)  
+        os.system(f'rm -rf {self.run_path}out_*.ww3')
+
 
 
 if __name__ == '__main__':
     # print_a() is only executed when the module is run directly.
     print('executed directly')
```

### Comparing `ww3py-0.0.1/ww3py/exec/utils.py` & `ww3py-0.0.3/ww3py/util/files.py`

 * *Files identical despite different names*

### Comparing `ww3py-0.0.1/ww3py/plot/init_custom.py` & `ww3py-0.0.3/ww3py/plot/init_custom.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
-mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm/info/plots/Helvetica.ttf')
-mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm/info/plots/Helvetica-Light.ttf')
-mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm/info/plots/Helvetica-Bold.ttf')
+mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm_ctrl/info/plots/Helvetica.ttf')
+mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm_ctrl/info/plots/Helvetica-Light.ttf')
+mpl.font_manager.fontManager.addfont('/home/fayalacruz/runs/reg_storm_ctrl/info/plots/Helvetica-Bold.ttf')
 
 newparams = {'axes.grid': False,
-             'lines.linewidth': 1.5,
-             'ytick.labelsize':11,
-             'xtick.labelsize':11,
-             'axes.labelsize':12,
-             'axes.titlesize':18,
-             'legend.fontsize':13,
-             'figure.titlesize':16,
+             'lines.linewidth': 1,
+             'ytick.labelsize':12,
+             'xtick.labelsize':12,
+             'axes.labelsize':13,
+             'axes.titlesize':13,
+             'legend.fontsize':14,
+             'figure.titlesize':14,
              'font.family':'Helvetica Light'}
 plt.rcParams.update(newparams)
```

### Comparing `ww3py-0.0.1/ww3py/plot/soft_topo_cmap.py` & `ww3py-0.0.3/ww3py/plot/soft_topo_cmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 
 def register_soft_cmap (cmap_path):
     cmap_array=np.genfromtxt(cmap_path)
     customColourMap= LinearSegmentedColormap.from_list('soft_topo', cmap_array[::-1], N=256)
     plt.register_cmap(cmap=customColourMap)
     return 
 
-cmap_txt_path = '/home/fayalacruz/runs/reg_storm/info/plots/smooth_topo.txt'
+cmap_txt_path = '/home/fayalacruz/runs/reg_storm_ctrl/info/plots/smooth_topo.txt'
 register_soft_cmap(cmap_txt_path)
```

### Comparing `ww3py-0.0.1/ww3py.egg-info/PKG-INFO` & `ww3py-0.0.3/ww3py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ww3py
-Version: 0.0.1
+Version: 0.0.3
 Summary: A handle python package to WWIII simulations
 Home-page: UNKNOWN
 Author: Franklin Ayala
 Author-email: <ffayalac@unal.edu.co>
 License: UNKNOWN
 Description: This is the first release for ww3py on 30/01/2023
 Keywords: python,first package
```

