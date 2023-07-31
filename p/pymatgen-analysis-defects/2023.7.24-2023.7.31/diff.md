# Comparing `tmp/pymatgen-analysis-defects-2023.7.24.tar.gz` & `tmp/pymatgen-analysis-defects-2023.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-analysis-defects-2023.7.24.tar", last modified: Mon Jul 24 21:13:17 2023, max compression
+gzip compressed data, was "pymatgen-analysis-defects-2023.7.31.tar", last modified: Mon Jul 31 20:16:13 2023, max compression
```

## Comparing `pymatgen-analysis-defects-2023.7.24.tar` & `pymatgen-analysis-defects-2023.7.31.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.735245 pymatgen-analysis-defects-2023.7.24/pymatgen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.735245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    28842 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/
--rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/freysoldt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/kumagai.py
--rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/finder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)    39802 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-24 21:13:17.000000 pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:13:17.739245 pymatgen-analysis-defects-2023.7.24/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_ccd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-24 21:13:03.000000 pymatgen-analysis-defects-2023.7.24/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_recombination.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_supercells.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-24 21:13:04.000000 pymatgen-analysis-defects-2023.7.24/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.259025 pymatgen-analysis-defects-2023.7.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-31 20:16:13.259025 pymatgen-analysis-defects-2023.7.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.251025 pymatgen-analysis-defects-2023.7.31/pymatgen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.251025 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.255025 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28842 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.255025 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14730 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/freysoldt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/kumagai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.255025 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/plotting/optical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42555 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39802 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.255025 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-31 20:16:13.000000 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-31 20:16:13.000000 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:16:13.000000 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-31 20:16:13.000000 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 20:16:13.000000 pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:16:13.259025 pymatgen-analysis-defects-2023.7.31/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:16:13.259025 pymatgen-analysis-defects-2023.7.31/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/tests/test_ccd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-31 20:15:58.000000 pymatgen-analysis-defects-2023.7.31/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_recombination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_supercells.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-31 20:15:59.000000 pymatgen-analysis-defects-2023.7.31/tests/test_utils.py
```

### Comparing `pymatgen-analysis-defects-2023.7.24/LICENSE` & `pymatgen-analysis-defects-2023.7.31/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/PKG-INFO` & `pymatgen-analysis-defects-2023.7.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.7.24
+Version: 2023.7.31
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.7.24/README.rst` & `pymatgen-analysis-defects-2023.7.31/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/ccd.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/ccd.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/constants.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/constants.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/core.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/freysoldt.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/freysoldt.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/corrections/kumagai.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/corrections/kumagai.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/finder.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/generators.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/recombination.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/supercells.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/thermo.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen/analysis/defects/utils.py` & `pymatgen-analysis-defects-2023.7.31/pymatgen/analysis/defects/utils.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/PKG-INFO` & `pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymatgen-analysis-defects
-Version: 2023.7.24
+Version: 2023.7.31
 Summary: Pymatgen extension for defects analysis
 Author-email: Jimmy-Xuan Shen <jmmshn@gmail.com>
 License: modified BSD
 Project-URL: documentation, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: homepage, https://materialsproject.github.io/pymatgen-analysis-defects/
 Project-URL: repository, https://github.com/materialsproject/pymatgen-analysis-defects
 Keywords: high-throughput,automated,dft,defects
```

### Comparing `pymatgen-analysis-defects-2023.7.24/pymatgen_analysis_defects.egg-info/SOURCES.txt` & `pymatgen-analysis-defects-2023.7.31/pymatgen_analysis_defects.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 pymatgen/analysis/defects/core.py
 pymatgen/analysis/defects/finder.py
 pymatgen/analysis/defects/generators.py
 pymatgen/analysis/defects/recombination.py
 pymatgen/analysis/defects/supercells.py
 pymatgen/analysis/defects/thermo.py
 pymatgen/analysis/defects/utils.py
+pymatgen/analysis/defects/corrections/__init__.py
 pymatgen/analysis/defects/corrections/freysoldt.py
 pymatgen/analysis/defects/corrections/kumagai.py
+pymatgen/analysis/defects/plotting/__init__.py
+pymatgen/analysis/defects/plotting/optical.py
 pymatgen_analysis_defects.egg-info/PKG-INFO
 pymatgen_analysis_defects.egg-info/SOURCES.txt
 pymatgen_analysis_defects.egg-info/dependency_links.txt
 pymatgen_analysis_defects.egg-info/requires.txt
 pymatgen_analysis_defects.egg-info/top_level.txt
 tests/test_ccd.py
 tests/test_core.py
```

### Comparing `pymatgen-analysis-defects-2023.7.24/pyproject.toml` & `pymatgen-analysis-defects-2023.7.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_ccd.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_ccd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from collections import namedtuple
 
 import numpy as np
+import pandas as pd
 import pytest
 
 from pymatgen.analysis.defects.ccd import (
     HarmonicDefect,
     Waveder,
     _get_wswq_slope,
     plot_pes,
 )
+from pymatgen.analysis.defects.plotting.optical import plot_optical_transitions
 
 
 @pytest.fixture(scope="session")
 def hd0(v_ga):
     vaspruns = v_ga[(0, -1)]["vaspruns"]
     procar = v_ga[(0, -1)]["procar"]
     hd0 = HarmonicDefect.from_vaspruns(
@@ -147,10 +149,24 @@
     hd0.waveder = Waveder.from_binary(dir0_opt / "WAVEDER")
     energy, eps_vbm, eps_cbm = hd0.get_dielectric_function(idir=0, jdir=0)
     inter_vbm = np.trapz(np.imag(eps_vbm[:100]), energy[:100])
     inter_cbm = np.trapz(np.imag(eps_cbm[:100]), energy[:100])
     assert pytest.approx(inter_vbm, abs=0.01) == 6.31
     assert pytest.approx(inter_cbm, abs=0.01) == 0.27
 
+    df, cmap, norm = plot_optical_transitions(hd0, kpt_index=0, band_window=5)
+    assert isinstance(df, pd.DataFrame)
+    assert len(df) == 11
+
+    df, cmap, norm = plot_optical_transitions(
+        hd0,
+        kpt_index=-100,
+        band_window=5,
+        user_defect_band=(100, 0, 0),
+        shift_eig={100: 0},
+    )
+    assert df.iloc[5]["ib"] == 100
+    assert df.iloc[5]["jb"] == 100
+
 
 def test_plot_pes(hd0):
     plot_pes(hd0)
```

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_core.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_corrections.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_finder.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_generators.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_recombination.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_recombination.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_supercells.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_supercells.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_thermo.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `pymatgen-analysis-defects-2023.7.24/tests/test_utils.py` & `pymatgen-analysis-defects-2023.7.31/tests/test_utils.py`

 * *Files identical despite different names*

