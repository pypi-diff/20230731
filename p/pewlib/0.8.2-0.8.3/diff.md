# Comparing `tmp/pewlib-0.8.2.tar.gz` & `tmp/pewlib-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pewlib-0.8.2.tar", last modified: Mon Jul 31 00:50:27 2023, max compression
+gzip compressed data, was "pewlib-0.8.3.tar", last modified: Mon Jul 31 04:16:17 2023, max compression
```

## Comparing `pewlib-0.8.2.tar` & `pewlib-0.8.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 00:50:17.000000 pewlib-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 00:50:27.540753 pewlib-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-31 00:50:17.000000 pewlib-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/npz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/perkinelmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/textimage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/io/vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/laser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/pewlib/process/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/process/threshold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/pewlib/srr/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-31 00:50:17.000000 pewlib-0.8.2/pewlib/srr/srr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.536753 pewlib-0.8.2/pewlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 00:50:27.000000 pewlib-0.8.2/pewlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:50:27.540753 pewlib-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 00:50:17.000000 pewlib-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:50:27.540753 pewlib-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_colocal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_convolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_agilent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_io_thermo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_laser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_peakfinding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_srr.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 00:50:17.000000 pewlib-0.8.2/tests/test_threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.012446 pewlib-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-31 04:16:06.000000 pewlib-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 04:16:17.012446 pewlib-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-31 04:16:06.000000 pewlib-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.004446 pewlib-0.8.3/pewlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.008446 pewlib-0.8.3/pewlib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/npz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/perkinelmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/textimage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/io/vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/laser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.008446 pewlib-0.8.3/pewlib/process/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14654 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/process/threshold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.008446 pewlib-0.8.3/pewlib/srr/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/srr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/srr/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-07-31 04:16:06.000000 pewlib-0.8.3/pewlib/srr/srr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.008446 pewlib-0.8.3/pewlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-31 04:16:16.000000 pewlib-0.8.3/pewlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 04:16:17.000000 pewlib-0.8.3/pewlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 04:16:16.000000 pewlib-0.8.3/pewlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-31 04:16:16.000000 pewlib-0.8.3/pewlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 04:16:16.000000 pewlib-0.8.3/pewlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 04:16:16.000000 pewlib-0.8.3/pewlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 04:16:17.012446 pewlib-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-31 04:16:06.000000 pewlib-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 04:16:17.012446 pewlib-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_colocal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_convolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_io_agilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_io_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_io_thermo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_laser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_peakfinding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_srr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-31 04:16:06.000000 pewlib-0.8.3/tests/test_threshold.py
```

### Comparing `pewlib-0.8.2/LICENSE` & `pewlib-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/PKG-INFO` & `pewlib-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.2
+Version: 0.8.3
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
```

### Comparing `pewlib-0.8.2/pewlib/__main__.py` & `pewlib-0.8.3/pewlib/__main__.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/calibration.py` & `pewlib-0.8.3/pewlib/calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/config.py` & `pewlib-0.8.3/pewlib/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/io/agilent.py` & `pewlib-0.8.3/pewlib/io/agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/io/csv.py` & `pewlib-0.8.3/pewlib/io/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,22 +25,22 @@
         drop_names: columns dropped from imports
         kw_genfromtxt: kwargs for numpy.genfromtxt
         regex: regex string for matching filenames
     """
 
     def __init__(
         self,
-        drop_names: List[str] = [],
+        drop_names: List[str] | None = None,
         kw_genfromtxt: dict | None = None,
         regex: str = r".*\.csv",
         drop_nan_rows: bool = False,
         drop_nan_columns: bool = False,
         transposed: bool = False,
     ):
-        self.drop_names = drop_names
+        self.drop_names = drop_names or []
         self.kw_genfromtxt = kw_genfromtxt
         self.regex = re.compile(regex, re.IGNORECASE)
 
         self.drop_nan_rows = drop_nan_rows
         self.drop_nan_columns = drop_nan_columns
         self.transposed = transposed
 
@@ -68,22 +68,32 @@
         return path
 
 
 class NuOption(GenericOption):
     """Option for Nu Instruments data."""
 
     def __init__(self):
-        super().__init__(drop_names=["X_(um)", "Y_(um)"], regex=r"acq.*\.csv")
+        super().__init__(
+            drop_names=["Cycle_time_(ms)", "x_[um]", "y_[um]"],
+            kw_genfromtxt={"skip_header": 11},
+            regex=r"line_\d+\.csv",
+        )
 
     def readParams(self, data: np.ndarray) -> dict:
-        if "Y_(um)" in data.dtype.names:
-            return {"spotsize": np.round(np.mean(np.diff(data["Y_(um)"], axis=0)), 2)}
+        params = {}
+        if "Cycle time (ms)" in data.dtype.names:
+            params["scantime"] = np.round(
+                1000.0 * np.mean(np.diff(data["Cycle time (ms)"], axis=1)), 4
+            )
+        if "y_[um]" in data.dtype.names:
+            params["spotsize"] = np.round(np.mean(np.diff(data["y_[um]"], axis=0)), 2)
         else:  # pragma: no cover
-            logger.warning("Y_(um) not found, unable to read spotsize.")
-            return super().readParams(data)
+            logger.warning("y_[um] not found, unable to read spotsize.")
+        return params
+        # return super().readParams(data)
 
     def sortkey(self, path: Path) -> int:
         """Sorts files numerically."""
         return int("".join(filter(str.isdigit, path.stem)) or -1)
 
 
 class ThermoLDROption(GenericOption):
@@ -122,15 +132,15 @@
 
     def readParams(self, data: np.ndarray) -> dict:
         if "t_elapsed_Buf" in data.dtype.names:
             return {
                 "scantime": np.round(np.mean(np.diff(data["t_elapsed_Buf"], axis=1)), 4)
             }
         else:  # pragma: no cover
-            logger.warning("Y_(um) not found, unable to read spotsize.")
+            logger.warning("'t_elapsed_Buf' not found, unable to read scantime.")
             return super().readParams(data)
 
     def sortkey(self, path: Path) -> float:
         """Sorts files using the timestamp in name."""
         match = self.regex.match(path.name)
         return time.mktime(time.strptime(match.group(1), "%Y.%m.%d-%Hh%Mm%Ss"))
```

### Comparing `pewlib-0.8.2/pewlib/io/npz.py` & `pewlib-0.8.3/pewlib/io/npz.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """
 Import and export in pew's custom file format, based on numpy's compressed '.npz'.
 This format svaes image data, laser parameters and calibrations in one file.
 """
 import logging
 import time
 from pathlib import Path
-from typing import Dict, Union
+from typing import Dict, List, Union
 
 import numpy as np
 
 from pewlib import Calibration, Config, Laser, __version__
 from pewlib.config import SpotConfig
-from pewlib.laser import Laser
 from pewlib.srr import SRRConfig, SRRLaser
 
 logger = logging.getLogger(__name__)
 
 
-def pack_info(info: Dict[str, str], sep: str = "\t") -> np.ndarray:
+def pack_info(
+    info: Dict[str, str], sep: str = "\t", remove_keys: List[str] | None = None
+) -> np.ndarray:
+    if remove_keys is None:
+        remove_keys = ["File Path"]
     string = sep.join(
         f"{key.replace(sep, ' ')}{sep}{val.replace(sep, ' ')}"
         for key, val in info.items()
-        if key not in ["File Path"]
+        if key not in remove_keys
     )  # Makes no sense to store file path so drop it
     return np.array(string)
 
 
 def unpack_info(x: np.ndarray, sep: str = "\t") -> Dict[str, str]:
     tokens = str(x).split(sep)
     return {key: val for key, val in zip(tokens[::2], tokens[1::2])}
 
 
 def pack_calibration(dict: Dict[str, Calibration]) -> np.ndarray:
     size = max(v.x.size for v in dict.values())
     data = np.stack([v.to_array(size=size) for v in dict.values()])
     elements = np.array([k for k in dict.keys()])
-    # recfunctions.append_fields does not like 0 length, i.e. when no calibration with points
+    # recfunctions.append_fields does not like 0 length,
+    # i.e. when no calibration with points
     packed = np.empty(
         data.size, dtype=[("element", elements.dtype), ("calibration", data.dtype)]
     )
     packed["element"] = elements
     packed["calibration"] = data
     return packed
```

### Comparing `pewlib-0.8.2/pewlib/io/perkinelmer.py` & `pewlib-0.8.3/pewlib/io/perkinelmer.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/io/textimage.py` & `pewlib-0.8.3/pewlib/io/textimage.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/io/thermo.py` & `pewlib-0.8.3/pewlib/io/thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/io/vtk.py` & `pewlib-0.8.3/pewlib/io/vtk.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/laser.py` & `pewlib-0.8.3/pewlib/laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/calc.py` & `pewlib-0.8.3/pewlib/process/calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/colocal.py` & `pewlib-0.8.3/pewlib/process/colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/convolve.py` & `pewlib-0.8.3/pewlib/process/convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/filters.py` & `pewlib-0.8.3/pewlib/process/filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/peakfinding.py` & `pewlib-0.8.3/pewlib/process/peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/register.py` & `pewlib-0.8.3/pewlib/process/register.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/process/threshold.py` & `pewlib-0.8.3/pewlib/process/threshold.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/srr/config.py` & `pewlib-0.8.3/pewlib/srr/config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib/srr/srr.py` & `pewlib-0.8.3/pewlib/srr/srr.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/pewlib.egg-info/PKG-INFO` & `pewlib-0.8.3/pewlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pewlib
-Version: 0.8.2
+Version: 0.8.3
 Summary: Import, processing and export library for LA-ICP-MS data.
 Home-page: https://github.com/djdt/pewlib
 Author: T. Lockwood
 Author-email: thomas.lockwood@uts.edu.au
 Project-URL: Documentation, https://djdt.github.io/pewlib
 Project-URL: Source, https://gtihub.com/djdt/pewlib
 Description-Content-Type: text/markdown
```

### Comparing `pewlib-0.8.2/pewlib.egg-info/SOURCES.txt` & `pewlib-0.8.3/pewlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/setup.py` & `pewlib-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_calc.py` & `pewlib-0.8.3/tests/test_calc.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_calibration.py` & `pewlib-0.8.3/tests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_colocal.py` & `pewlib-0.8.3/tests/test_colocal.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_config.py` & `pewlib-0.8.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_convolve.py` & `pewlib-0.8.3/tests/test_convolve.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_filters.py` & `pewlib-0.8.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_io.py` & `pewlib-0.8.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_io_agilent.py` & `pewlib-0.8.3/tests/test_io_agilent.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_io_csv.py` & `pewlib-0.8.3/tests/test_io_csv.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_io_thermo.py` & `pewlib-0.8.3/tests/test_io_thermo.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_laser.py` & `pewlib-0.8.3/tests/test_laser.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_peakfinding.py` & `pewlib-0.8.3/tests/test_peakfinding.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_register.py` & `pewlib-0.8.3/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `pewlib-0.8.2/tests/test_srr.py` & `pewlib-0.8.3/tests/test_srr.py`

 * *Files identical despite different names*

