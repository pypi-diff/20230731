# Comparing `tmp/pewlib-0.8.1.tar.gz` & `tmp/pewlib-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pewlib-0.8.1.tar", last modified: Fri Jul 21 07:18:40 2023, max compression
+gzip compressed data, was "pewlib-0.8.2.tar", last modified: Mon Jul 31 00:50:27 2023, max compression
```

## Comparing `pewlib-0.8.1.tar` & `pewlib-0.8.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.528747 pewlib-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-21 07:18:25.000000 pewlib-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 07:18:40.528747 pewlib-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-21 07:18:25.000000 pewlib-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.508747 pewlib-0.8.1/pewlib/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.516747 pewlib-0.8.1/pewlib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/npz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/perkinelmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/textimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/io/vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/laser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.520747 pewlib-0.8.1/pewlib/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/process/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.520747 pewlib-0.8.1/pewlib/srr/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-21 07:18:25.000000 pewlib-0.8.1/pewlib/srr/srr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.512747 pewlib-0.8.1/pewlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 07:18:40.000000 pewlib-0.8.1/pewlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 07:18:40.528747 pewlib-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-21 07:18:25.000000 pewlib-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 07:18:40.528747 pewlib-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_io_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_laser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_srr.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 07:18:25.000000 pewlib-0.8.1/tests/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 00:50:17.000000 pewlib-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 00:50:27.540753 pewlib-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-31 00:50:17.000000 pewlib-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/npz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/perkinelmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/textimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/laser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/pewlib/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/pewlib/srr/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/srr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:50:27.540753 pewlib-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 00:50:17.000000 pewlib-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_srr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_threshold.py
```

### Comparing `pewlib-0.8.1/LICENSE` & `pewlib-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/PKG-INFO` & `pewlib-0.8.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.1
+Version: 0.8.2
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pewlib
 
-![Build](https://github.com/djdt/pewlib/workflows/Build/badge.svg)
+![Build](https://github.com/djdt/pewlib/actions/workflows/build.yml/badge.svg)
 
 Pewlib is a library for importing, processing and exporting LA-ICP-MS data.
 Currently exports from Agilent, Thermo and PerkinElmer software is supported, as well as delimited text images.
 
 ## Installation
 
 Pewlib is availble on PyPI and installable via pip.
```

### Comparing `pewlib-0.8.1/pewlib/__main__.py` & `pewlib-0.8.2/pewlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/calibration.py` & `pewlib-0.8.2/pewlib/calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/config.py` & `pewlib-0.8.2/pewlib/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/agilent.py` & `pewlib-0.8.2/pewlib/io/agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/csv.py` & `pewlib-0.8.2/pewlib/io/csv.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/npz.py` & `pewlib-0.8.2/pewlib/io/npz.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """
 Import and export in pew's custom file format, based on numpy's compressed '.npz'.
 This format svaes image data, laser parameters and calibrations in one file.
 """
-import time
 import logging
+import time
 from pathlib import Path
+from typing import Dict, Union
 
 import numpy as np
 
-from pewlib import __version__
-from pewlib import Laser, Calibration, Config
+from pewlib import Calibration, Config, Laser, __version__
 from pewlib.config import SpotConfig
-
 from pewlib.laser import Laser
-from pewlib.srr import SRRLaser, SRRConfig
-
-from typing import Dict, Union
+from pewlib.srr import SRRConfig, SRRLaser
 
 logger = logging.getLogger(__name__)
 
 
 def pack_info(info: Dict[str, str], sep: str = "\t") -> np.ndarray:
     string = sep.join(
         f"{key.replace(sep, ' ')}{sep}{val.replace(sep, ' ')}"
@@ -97,29 +94,30 @@
         calibration = {}
         for name in data.dtype.names:
             calibration[name] = Calibration.from_array(npz[f"calibration_{name}"])
     else:
         calibration = unpack_calibration(npz["calibration"])
 
     if header["version"] < __version__:
-        logger.info(f"NPZ version of {path} is out of date. {npz['_version']} < 0.8.0.")
+        logger.info(
+            f"NPZ version of {path} is out of date. {header['version']} < 0.8.0."
+        )
 
     if header["class"] in ["Laser", "Raster"]:
         laser = Laser
         config = Config.from_array(npz["config"])
     elif header["class"] in ["Spot"]:
         laser = Laser
         config = SpotConfig.from_array(npz["config"])
     elif header["class"] in ["SRRLaser", "SRR"]:
         laser = SRRLaser  # type: ignore
         config = SRRConfig.from_array(npz["config"])
     else:  # pragma: no cover
         raise ValueError("NPZ unable to import laser class {npz['_class']}.")
 
-
     # Update the path
     info["Name"] = info.get("Name", path.stem)  # Ensure name
     info["File Path"] = str(path.resolve())
     info["File Version"] = str(header["version"])
 
     return laser(
         data=data,
```

### Comparing `pewlib-0.8.1/pewlib/io/perkinelmer.py` & `pewlib-0.8.2/pewlib/io/perkinelmer.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/textimage.py` & `pewlib-0.8.2/pewlib/io/textimage.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/thermo.py` & `pewlib-0.8.2/pewlib/io/thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/io/vtk.py` & `pewlib-0.8.2/pewlib/io/vtk.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/laser.py` & `pewlib-0.8.2/pewlib/laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/calc.py` & `pewlib-0.8.2/pewlib/process/calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/colocal.py` & `pewlib-0.8.2/pewlib/process/colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/convolve.py` & `pewlib-0.8.2/pewlib/process/convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/filters.py` & `pewlib-0.8.2/pewlib/process/filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/peakfinding.py` & `pewlib-0.8.2/pewlib/process/peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/register.py` & `pewlib-0.8.2/pewlib/process/register.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/process/threshold.py` & `pewlib-0.8.2/pewlib/process/threshold.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/srr/config.py` & `pewlib-0.8.2/pewlib/srr/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib/srr/srr.py` & `pewlib-0.8.2/pewlib/srr/srr.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/pewlib.egg-info/PKG-INFO` & `pewlib-0.8.2/pewlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.1
+Version: 0.8.2
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pewlib
 
-![Build](https://github.com/djdt/pewlib/workflows/Build/badge.svg)
+![Build](https://github.com/djdt/pewlib/actions/workflows/build.yml/badge.svg)
 
 Pewlib is a library for importing, processing and exporting LA-ICP-MS data.
 Currently exports from Agilent, Thermo and PerkinElmer software is supported, as well as delimited text images.
 
 ## Installation
 
 Pewlib is availble on PyPI and installable via pip.
```

### Comparing `pewlib-0.8.1/pewlib.egg-info/SOURCES.txt` & `pewlib-0.8.2/pewlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/setup.py` & `pewlib-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_calc.py` & `pewlib-0.8.2/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_calibration.py` & `pewlib-0.8.2/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_colocal.py` & `pewlib-0.8.2/tests/test_colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_config.py` & `pewlib-0.8.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_convolve.py` & `pewlib-0.8.2/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_filters.py` & `pewlib-0.8.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_io.py` & `pewlib-0.8.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_io_agilent.py` & `pewlib-0.8.2/tests/test_io_agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_io_csv.py` & `pewlib-0.8.2/tests/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_io_thermo.py` & `pewlib-0.8.2/tests/test_io_thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_laser.py` & `pewlib-0.8.2/tests/test_laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_peakfinding.py` & `pewlib-0.8.2/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_register.py` & `pewlib-0.8.2/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.1/tests/test_srr.py` & `pewlib-0.8.2/tests/test_srr.py`

 * *Files identical despite different names*

