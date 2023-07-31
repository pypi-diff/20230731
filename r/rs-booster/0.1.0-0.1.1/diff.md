# Comparing `tmp/rs-booster-0.1.0.tar.gz` & `tmp/rs-booster-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rs-booster-0.1.0.tar", last modified: Thu Sep  1 14:24:24 2022, max compression
+gzip compressed data, was "rs-booster-0.1.1.tar", last modified: Mon Jul 31 20:51:43 2023, max compression
```

## Comparing `rs-booster-0.1.0.tar` & `rs-booster-0.1.1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-09-01 14:24:09.000000 rs-booster-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-09-01 14:24:09.000000 rs-booster-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-09-01 14:24:24.096961 rs-booster-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2973 2022-09-01 14:24:09.000000 rs-booster-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rs_booster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-01 14:24:24.000000 rs-booster-0.1.0/rs_booster.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/diffmaps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/diffmaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3314 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/diffmaps/diffmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3806 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/diffmaps/internaldiffmap.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/diffmaps/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/esf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/esf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4794 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/esf/extrapolate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2921 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/io/precog2mtz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/realspace/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/realspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/realspace/find_peaks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/scaleit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/scaleit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/scaleit/scaleit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/stats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3077 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/stats/ccanom.py
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/stats/cchalf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3876 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/stats/ccpred.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/stats/ccsym.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/rsbooster/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-09-01 14:24:09.000000 rs-booster-0.1.0/rsbooster/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (121)      137 2022-09-01 14:24:24.100961 rs-booster-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-09-01 14:24:09.000000 rs-booster-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:24.096961 rs-booster-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-01 14:24:09.000000 rs-booster-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-09-01 14:24:09.000000 rs-booster-0.1.0/tests/test_rsbooster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 20:51:21.000000 rs-booster-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 20:51:21.000000 rs-booster-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 20:51:43.283376 rs-booster-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-31 20:51:21.000000 rs-booster-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rs_booster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 20:51:43.000000 rs-booster-0.1.1/rs_booster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/diffmaps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/diffmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/internaldiffmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/diffmaps/weights.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/esf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/esf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/esf/extrapolate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/io/precog2mtz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/realspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/realspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/realspace/find_peaks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/scaleit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/scaleit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/scaleit/scaleit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccanom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/cchalf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccpred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/ccsym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/stats/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/rsbooster/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-31 20:51:21.000000 rs-booster-0.1.1/rsbooster/utils/rfree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-31 20:51:43.287376 rs-booster-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-31 20:51:21.000000 rs-booster-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:43.283376 rs-booster-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/test_rfree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 20:51:21.000000 rs-booster-0.1.1/tests/test_rsbooster.py
```

### Comparing `rs-booster-0.1.0/LICENSE` & `rs-booster-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.0/PKG-INFO` & `rs-booster-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-booster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful scripts for analyzing diffraction
 Home-page: https://github.com/rs-station/rs-booster
 Author: Jack B. Greisman
 Author-email: greisman@g.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/rs-booster/issues
 Project-URL: Source Code, https://github.com/rs-station/rs-booster
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 
 rs-booster contains commandline scripts for diffraction data analysis tasks.
 
 This package can be viewed as a "booster pack" for reciprocalspaceship.
```

### Comparing `rs-booster-0.1.0/README.md` & `rs-booster-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.0/rs_booster.egg-info/PKG-INFO` & `rs-booster-0.1.1/rs_booster.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rs-booster
-Version: 0.1.0
+Version: 0.1.1
 Summary: Useful scripts for analyzing diffraction
 Home-page: https://github.com/rs-station/rs-booster
 Author: Jack B. Greisman
 Author-email: greisman@g.harvard.edu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rs-station/rs-booster/issues
 Project-URL: Source Code, https://github.com/rs-station/rs-booster
@@ -15,14 +15,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Requires-Python: >3.7
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
 
 rs-booster contains commandline scripts for diffraction data analysis tasks.
 
 This package can be viewed as a "booster pack" for reciprocalspaceship.
```

### Comparing `rs-booster-0.1.0/rs_booster.egg-info/SOURCES.txt` & `rs-booster-0.1.1/rs_booster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,11 +24,14 @@
 rsbooster/scaleit/__init__.py
 rsbooster/scaleit/scaleit.py
 rsbooster/stats/__init__.py
 rsbooster/stats/ccanom.py
 rsbooster/stats/cchalf.py
 rsbooster/stats/ccpred.py
 rsbooster/stats/ccsym.py
+rsbooster/stats/parser.py
 rsbooster/utils/__init__.py
 rsbooster/utils/io.py
+rsbooster/utils/rfree.py
 tests/__init__.py
+tests/test_rfree.py
 tests/test_rsbooster.py
```

### Comparing `rs-booster-0.1.0/rs_booster.egg-info/entry_points.txt` & `rs-booster-0.1.1/rs_booster.egg-info/entry_points.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,9 +5,10 @@
 rs.ccsym = rsbooster.stats.ccsym:main
 rs.diffmap = rsbooster.diffmaps.diffmap:main
 rs.extrapolate = rsbooster.esf.extrapolate:main
 rs.find_difference_peaks = rsbooster.realspace.find_peaks:find_difference_peaks
 rs.find_peaks = rsbooster.realspace.find_peaks:find_peaks
 rs.internal_diffmap = rsbooster.diffmaps.internaldiffmap:main
 rs.precog2mtz = rsbooster.io.precog2mtz:main
+rs.rfree = rsbooster.utils.rfree:main
 rs.scaleit = rsbooster.scaleit.scaleit:main
```

### Comparing `rs-booster-0.1.0/rsbooster/diffmaps/diffmap.py` & `rs-booster-0.1.1/rsbooster/diffmaps/diffmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,21 +64,21 @@
         default=None,
         help="If set, dmax to truncate difference map",
     )
     parser.add_argument(
         "-o", "--outfile", default="diffmap.mtz", help="Output MTZ filename"
     )
 
-    return parser.parse_args()
+    return parser#.parse_args()
 
 
 def main():
 
     # Parse commandline arguments
-    args = parse_arguments()
+    args = parse_arguments().parse_args()
     refmtz, phi_col = args.refmtz
 
     # Read MTZ files
     onmtz = subset_to_FSigF(*args.onmtz, {args.onmtz[1]: "F", args.onmtz[2]: "SigF"})
     offmtz = subset_to_FSigF(
         *args.offmtz, {args.offmtz[1]: "F", args.offmtz[2]: "SigF"}
     )
```

### Comparing `rs-booster-0.1.0/rsbooster/diffmaps/internaldiffmap.py` & `rs-booster-0.1.1/rsbooster/diffmaps/internaldiffmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,21 +71,21 @@
         "--spacegroup",
         help="Spacegroup to use for symmetry operation (only necessary if `op` specifies an ISYM).",
     )
     parser.add_argument(
         "-o", "--outfile", default="internal_diffmap.mtz", help="Output MTZ filename"
     )
 
-    return parser.parse_args()
+    return parser#.parse_args()
 
 
 def main():
 
     # Parse commandline arguments
-    args = parse_arguments()
+    args = parse_arguments().parse_args()
     refmtz, phi_col = args.refmtz
 
     # Read MTZ files
     mtz = subset_to_FSigF(
         *args.inputmtz, {args.inputmtz[1]: "F", args.inputmtz[2]: "SigF"}
     )
     ref = rs.read_mtz(refmtz)
```

### Comparing `rs-booster-0.1.0/rsbooster/esf/extrapolate.py` & `rs-booster-0.1.1/rsbooster/esf/extrapolate.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 where f, is the extrapolation factor.
 
 Notes
 -----
     - F_{off} and F_{calc} can be the same MTZ file, as done in Hekstra et al, 
       Nature (2016). In that case, the equation for SigF_{esf} is adjusted to
       use (f-1)**2 for SigF_{off} to avoid double-counting in the error propagation.
+    - At most one of F_{ref} and F_{calc} can be specified. If neither is specified, 
+      F_{calc} will be set to F_{off}.
     - After computing |F_{esf}|, any negative structure factor amplitudes are converted
       to positive values. This is to ensure that they are handled correctly downstream in
       phenix, and because they are technically amplitudes of complex numbers and the phase
       should just be flipped by 180 degrees.
 """
 
 import argparse
@@ -54,57 +56,59 @@
         "--offmtz",
         nargs=3,
         metavar=("mtz", "data_col", "sig_col"),
         required=True,
         help=("MTZ to be used as `off` data. Specified as (filename, F, SigF)"),
     )
 
-    # One of these must provided
+    # at most one of these must be provided
     parser.add_argument(
         "-calc",
         "--calcmtz",
         nargs=2,
         metavar=("mtz", "data_col"),
-        help=("MTZ to be used as `calc` data. Specified as (filename, F, SigF)"),
+        help=("MTZ to be used as `calc` data. Specified as (filename, F). At most one of `-calc` and `-ref` can be specified."),
     )
     parser.add_argument(
         "-ref",
         "--refmtz",
         nargs=3,
         metavar=("mtz", "data_col", "sig_col"),
-        help=("MTZ to be used as `ref` data. Specified as (filename, F, SigF)"),
+        help=("MTZ to be used as `ref` data. Specified as (filename, F, SigF). At most one of `-calc` and `-ref` can be specified."),
     )
 
     # Optional arguments
     parser.add_argument(
         "-f", "--factor", type=float, default=10.0, help="Extrapolation factor"
     )
     parser.add_argument(
         "-o", "--outfile", default="esf.mtz", help="Output MTZ filename"
     )
 
-    return parser.parse_args()
+    return parser#.parse_args()
 
 
 def main():
 
     # Parse commandline arguments
-    args = parse_arguments()
+    args = parse_arguments().parse_args()
     on, f_on, sigf_on = args.onmtz
     off, f_off, sigf_off = args.offmtz
 
     if args.calcmtz and args.refmtz:
         raise ValueError("Only specify `-calc` or `-ref`, not both.")
     elif args.calcmtz:
         calc, f_calc = args.calcmtz
         sigf_calc = None
     elif args.refmtz:
         calc, f_calc, sigf_calc = args.refmtz
     else:
-        raise ValueError("One of `-calc` or `-ref` must be specified.")
+        print("No `-calc` or `-ref` is specified. `-calc` is set to `-off`.")
+        calc, f_calc, _ = args.offmtz
+        sigf_calc = None
 
     # Read MTZ files
     on = rs.read_mtz(on)
     off = rs.read_mtz(off)
     calc = rs.read_mtz(calc)
 
     # Canonicalize column names
```

### Comparing `rs-booster-0.1.0/rsbooster/io/precog2mtz.py` & `rs-booster-0.1.1/rsbooster/io/precog2mtz.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     parser.add_argument(
         "-o",
         "--mtz-out",
         type=str,
         default="integrated.mtz",
         help="Name of the output mtz file.",
     )
-    parser = parser.parse_args()
+    # parser = parser.parse_args()
     return parser
 
 
 def make_dataset(filenames, spacegroup, cell):
     """
     Make an rs.DataSet from all *.ii the files in filenames.
 
@@ -69,15 +69,15 @@
         ds["BATCH"] = i
         ds["BATCH"] = ds["BATCH"].astype(rs.BatchDtype())
         datasets.append(ds)
     return rs.concat(datasets)
 
 
 def main():
-    parser = parse_arguments()
+    parser = parse_arguments().parse_args()
 
     # Parse the output filename(s)
     if isinstance(parser.ii_in, str):
         filenames = [parser.ii_in]
     else:
         filenames = parser.ii_in
```

### Comparing `rs-booster-0.1.0/rsbooster/realspace/find_peaks.py` & `rs-booster-0.1.1/rsbooster/realspace/find_peaks.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         }
         if negate:
             negative_keys = ['peak', 'peakz', 'score', 'scorez']
             for k in negative_keys:
                 record[k] = -record[k]
         peaks.append(record)
 
-    out = pd.DataFrame.from_records(peaks)
+    out = pd.DataFrame.from_records(peaks, columns=long_names.keys())
 
     #In case there are no peaks we need to test the length
     if len(out) > 0:
         out = out.sort_values(sort_by_key, ascending=False)
 
     if use_long_names:
         out = out.rename(columns = long_names)
@@ -212,25 +212,25 @@
         help="the minimum score of peaks with default zero.")
     parser.add_argument("--min-peak", type=float, default=0.,
         help="the minimum peak value with default zero.")
     parser.add_argument("-d", "--distance-cutoff", type=float, default=4.,
         help="the distance cutoff of nearest neighbor search with default of 4 angstroms.")
     parser.add_argument("--use-long-names", action='store_true',
         help="use more verbose column names in the peak report.")
-    parser = parser.parse_args()
+    # parser = parser.parse_args()
     return parser
 
 def find_peaks():
     main(difference_map=False, default_sigma_cutoff=1.5)
 
 def find_difference_peaks():
     main(difference_map=True, default_sigma_cutoff=3.0)
 
 def main(difference_map=False, default_sigma_cutoff=1.5):
-    parser = parse_args(default_sigma_cutoff)
+    parser = parse_args(default_sigma_cutoff).parse_args()
     structure = gemmi.read_pdb(parser.pdb_file)
     ds = rs.read_mtz(parser.mtz_file)
     mtz = ds[[parser.phase_key]].copy()
 
     if parser.weight_key is not None:
         mtz[parser.structure_factor_key] = ds[parser.structure_factor_key] * ds[parser.weight_key]
     else:
```

### Comparing `rs-booster-0.1.0/rsbooster/scaleit/scaleit.py` & `rs-booster-0.1.1/rsbooster/scaleit/scaleit.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     parser.add_argument(
         "-o",
         "--outfile",
         default="scaled.mtz",
         help="MTZ file to which scaleit output will be written",
     )
 
-    return parser.parse_args()
+    return parser#.parse_args()
 
 
 def load_mtz(mtzpath, data_col, sig_col):
     """Load mtz and do French-Wilson scaling, if necessary"""
     mtz = rs.read_mtz(mtzpath)
 
     # Check dtypes
@@ -105,15 +105,15 @@
 
     return
 
 
 def main():
 
     # Parse commandline arguments
-    args = parse_arguments()
+    args = parse_arguments().parse_args()
 
     # Test whether scaleit is on PATH
     if shutil.which("scaleit") is None:
         raise EnvironmentError(
             "Cannot find executable, scaleit. Please set up your CCP4 environment."
         )
```

### Comparing `rs-booster-0.1.0/rsbooster/stats/ccanom.py` & `rs-booster-0.1.1/rsbooster/stats/ccanom.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 """
 import argparse
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 
 
-def parse_arguments():
-    """Parse commandline arguments"""
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter, description=__doc__
-    )
-
-    # Required arguments
-    parser.add_argument(
-        "mtz",
-        nargs="+",
-        help="MTZs containing crossvalidation data from careless",
-    )
-    parser.add_argument(
-        "-m",
-        "--method",
-        default="spearman",
-        choices=["spearman", "pearson"],
-        help=("Method for computing correlation coefficient (spearman or pearson)"),
-    )
-
-    return parser.parse_args()
+from rsbooster.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
+    def __init__(self):
+        super().__init__(
+            description=__doc__
+        )
+        
+        # Required arguments
+        self.add_argument(
+            "mtz",
+            nargs="+",
+            help="MTZs containing crossvalidation data from careless",
+        )
+    
+        self.add_argument(
+            "-m",
+            "--method",
+            default="spearman",
+            choices=["spearman", "pearson"],
+            help=("Method for computing correlation coefficient (spearman or pearson)"),
+        )
 
 
 def make_halves_ccanom(mtz, bins=10):
     """Construct half-datasets for computing CCanom"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
@@ -47,16 +47,19 @@
 
     return temp, labels
 
 
 def analyze_ccanom_mtz(mtzpath, bins=10, return_labels=True, method="spearman"):
     """Compute CCsym from 2-fold cross-validation"""
 
-    mtz = rs.read_mtz(mtzpath)
-
+    if type(mtzpath) is rs.dataset.DataSet:
+        mtz=mtzpath
+    else:
+        mtz = rs.read_mtz(mtzpath)
+        
     # Error handling -- make sure MTZ file is appropriate
     if "half" not in mtz.columns:
         raise ValueError("Please provide MTZs from careless crossvalidation")
 
     if "F(+)" not in mtz.columns:
         raise ValueError("Please provide MTZs merged with `--anomalous` in careless")
 
@@ -71,19 +74,15 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def main():
-
-    # Parse commandline arguments
-    args = parse_arguments()
-
+def run_analysis(args):
     results = []
     labels = None
     for m in args.mtz:
         result = analyze_ccanom_mtz(m, method=args.method)
         if result is None:
             continue
         else:
@@ -92,22 +91,36 @@
             labels = result[1]
 
     results = rs.concat(results, check_isomorphous=False)
     results = results.reset_index(drop=True)
     results["CCanom"] = results[("DF1", "DF2")]
     results.drop(columns=[("DF1", "DF2")], inplace=True)
 
-    print(results)
+    for k in ('bin', 'repeat'):
+        results[k] = results[k].to_numpy('int32')
+
+    if args.output is not None:
+        results.to_csv(args.output)
+    else:
+        print(results.to_string())
+
+    # print(results.info())
 
     sns.lineplot(
-        data=results, x="bin", y="CCanom", hue="filename", ci="sd", palette="viridis"
+        data=results, x="bin", y="CCanom", hue="filename", errorbar="sd", palette="viridis"
     )
     plt.xticks(range(10), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$CC_{anom}$ " + f"({args.method})")
     plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.grid()
     plt.tight_layout()
-    plt.show()
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
+        plt.show()
 
+def parse_arguments():
+    return ArgumentParser()
 
-if __name__ == "__main__":
-    main()
+def main():
+    run_analysis(parse_arguments().parse_args())
```

### Comparing `rs-booster-0.1.0/rsbooster/stats/cchalf.py` & `rs-booster-0.1.1/rsbooster/stats/cchalf.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,36 +4,35 @@
 """
 import argparse
 import matplotlib.pyplot as plt
 import reciprocalspaceship as rs
 import seaborn as sns
 
 
-def parse_arguments():
-    """Parse commandline arguments"""
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter, description=__doc__
-    )
-
-    # Required arguments
-    parser.add_argument(
-        "mtz",
-        nargs="+",
-        help="MTZs containing crossvalidation data from careless",
-    )
-
-    parser.add_argument(
-        "-m",
-        "--method",
-        default="spearman",
-        choices=["spearman", "pearson"],
-        help=("Method for computing correlation coefficient (spearman or pearson)"),
-    )
-
-    return parser.parse_args()
+from rsbooster.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
+    def __init__(self):
+        super().__init__(
+            description=__doc__
+        )
+        
+        # Required arguments
+        self.add_argument(
+            "mtz",
+            nargs="+",
+            help="MTZs containing crossvalidation data from careless",
+        )
+    
+        self.add_argument(
+            "-m",
+            "--method",
+            default="spearman",
+            choices=["spearman", "pearson"],
+            help=("Method for computing correlation coefficient (spearman or pearson)"),
+        )
 
 
 def make_halves_cchalf(mtz, bins=10):
     """Construct half-datasets for computing CChalf"""
 
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
@@ -50,16 +49,19 @@
 
     return temp, labels
 
 
 def analyze_cchalf_mtz(mtzpath, bins=10, return_labels=True, method="spearman"):
     """Compute CChalf from 2-fold cross-validation"""
 
-    mtz = rs.read_mtz(mtzpath)
-
+    if type(mtzpath) is rs.dataset.DataSet:
+        mtz=mtzpath
+    else:
+        mtz = rs.read_mtz(mtzpath)
+        
     # Error handling -- make sure MTZ file is appropriate
     if "half" not in mtz.columns:
         raise ValueError("Please provide MTZs from careless crossvalidation")
 
     m, labels = make_halves_cchalf(mtz)
 
     grouper = m.groupby(["bin", "repeat"])[["F1", "F2"]]
@@ -69,19 +71,15 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def main():
-
-    # Parse commandline arguments
-    args = parse_arguments()
-
+def run_analysis(args):
     results = []
     labels = None
     for m in args.mtz:
         result = analyze_cchalf_mtz(m, method=args.method)
         if result is None:
             continue
         else:
@@ -90,22 +88,37 @@
             labels = result[1]
 
     results = rs.concat(results, check_isomorphous=False)
     results = results.reset_index(drop=True)
     results["CChalf"] = results[("F1", "F2")]
     results.drop(columns=[("F1", "F2")], inplace=True)
 
-    print(results)
+    for k in ('bin', 'repeat'):
+        results[k] = results[k].to_numpy('int32')
+
+    if args.output is not None:
+        results.to_csv(args.output)
+    else:
+        print(results.to_string())
+
+    print(results.info())
 
     sns.lineplot(
-        data=results, x="bin", y="CChalf", hue="filename", ci="sd", palette="viridis"
+        data=results, x="bin", y="CChalf", hue="filename", errorbar="sd", palette="viridis"
     )
     plt.xticks(range(10), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$CC_{1/2}$ " + f"({args.method})")
     plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.grid()
     plt.tight_layout()
-    plt.show()
+    if args.image is not None:
+        plt.savefig(args.image)
 
+    if args.show:
+        plt.show()
 
-if __name__ == "__main__":
-    main()
+
+def parse_arguments():
+    return ArgumentParser()
+
+def main():
+    run_analysis(parse_arguments().parse_args())
```

### Comparing `rs-booster-0.1.0/rsbooster/stats/ccpred.py` & `rs-booster-0.1.1/rsbooster/stats/ccpred.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,54 +9,59 @@
 import reciprocalspaceship as rs
 import gemmi
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
-def parse_arguments():
-    """Parse commandline arguments"""
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter, description=__doc__
-    )
-
-    # Required arguments
-    parser.add_argument(
-        "-i",
-        "--inputmtzs",
-        nargs="+",
-        action="append",
-        required=True,
-        help="MTZs containing holdout prediction data from careless",
-    )
-
-    # Optional arguments
-    parser.add_argument(
-        "-m",
-        "--method",
-        default="spearman",
-        choices=["spearman", "pearson"],
-        help=("Method for computing correlation coefficient (spearman or pearson)"),
-    )
-    parser.add_argument(
-        "--mod2",
-        action="store_true",
-        help=("Use (id mod 2) to assign delays (use when employing spacegroup hack)"),
-    )
+from rsbooster.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
+    def __init__(self):
+        super().__init__(
+            description=__doc__
+        )
 
-    return parser.parse_args()
+        # Required arguments
+        self.add_argument(
+            "mtzs",
+            nargs="+",
+            help="MTZs containing prediction data from careless",
+        )
+    
+        # Optional arguments
+        self.add_argument(
+            "-m",
+            "--method",
+            default="spearman",
+            choices=["spearman", "pearson"],
+            help=("Method for computing correlation coefficient (spearman or pearson)"),
+        )
+        self.add_argument(
+            "--mod2",
+            action="store_true",
+            help=("Use (id mod 2) to assign delays (use when employing spacegroup hack)"),
+        )
+        self.add_argument(
+            "--overall",
+            action="store_true",
+            default=False,
+            help=("Whether to report a single value for the entire dataset"),
+        )
 
 
 def compute_ccpred(
     mtzpath, overall=False, bins=10, return_labels=True, method="spearman", mod2=False
 ):
     """Compute CCsym from 2-fold cross-validation"""
 
-    mtz = rs.read_mtz(mtzpath)
-
+    if type(mtzpath) is rs.dataset.DataSet:
+        mtz=mtzpath
+    else:
+        mtz = rs.read_mtz(mtzpath)
+        
     if overall:
         grouper = mtz.groupby(["test"])[["Iobs", "Ipred"]]
     else:
         mtz, labels = mtz.assign_resolution_bins(bins)
         grouper = mtz.groupby(["bin", "test"])[["Iobs", "Ipred"]]
 
     result = (
@@ -75,44 +80,44 @@
 
     if return_labels and not overall:
         return result, labels
     else:
         return result
 
 
-def main():
-
-    # Parse commandline arguments
-    args = parse_arguments()
+def run_analysis(args):
 
     results = []
     labels = None
 
-    if isinstance(args.inputmtzs[0], list) and len(args.inputmtzs) > 1:
-        overall = True
-        mtzs = [item for sublist in args.inputmtzs for item in sublist]
-    else:
-        overall = False
-        mtzs = [item for sublist in args.inputmtzs for item in sublist]
-
-    for m in mtzs:
-        result = compute_ccpred(m, overall=overall, method=args.method, mod2=args.mod2)
+    # mtzs -> args.mtzs!
+    for m in args.mtzs: 
+        result = compute_ccpred(m, overall=args.overall, method=args.method, mod2=args.mod2)
         if isinstance(result, tuple):
             results.append(result[0])
             labels = result[1]
         else:
             results.append(result)
 
     results = rs.concat(results, check_isomorphous=False)
     results = results.reset_index(drop=True)
     results["CCpred"] = results[("Iobs", "Ipred")]
     results.drop(columns=[("Iobs", "Ipred")], inplace=True)
 
-    print(results)
-    if overall:
+    # print(results.info())
+    for k in ('bin', 'test'):
+        results[k] = results[k].to_numpy('int32')
+            
+    if args.output is not None:
+        results.to_csv(args.output)
+    else:
+        print(results.to_string())
+
+    print(results.info())
+    if args.overall:
         g = sns.relplot(
             data=results,
             x="id",
             y="CCpred",
             style="test",
             hue="delay",
             col="spacegroup",
@@ -136,12 +141,19 @@
             kind="line",
             palette="viridis",
         )
         for col_val, ax in g.axes_dict.items():
             ax.set_xticks(range(10))
             ax.set_xticklabels(labels, rotation=45, ha="right", rotation_mode="anchor")
             ax.grid(True)
+
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
         plt.show()
 
+def parse_arguments():
+    return ArgumentParser()
 
-if __name__ == "__main__":
-    main()
+def main():
+    run_analysis(parse_arguments().parse_args())
```

### Comparing `rs-booster-0.1.0/rsbooster/stats/ccsym.py` & `rs-booster-0.1.1/rsbooster/stats/ccsym.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,59 +10,59 @@
 import reciprocalspaceship as rs
 import gemmi
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 
-def parse_arguments():
-    """Parse commandline arguments"""
-    parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter, description=__doc__
-    )
-
-    # Required arguments
-    parser.add_argument(
-        "mtz",
-        nargs="+",
-        help="MTZs containing crossvalidation data from careless",
-    )
-    parser.add_argument(
-        "--op",
-        required=True,
-        help=(
-            "Symmetry operation to use to compute internal difference map. "
-            "Can be given as ISYM if used with a `spacegroup` argument"
-        ),
-    )
-
-    # Optional arguments
-    parser.add_argument(
-        "-sg",
-        "--spacegroup",
-        help=(
-            "Spacegroup to use for symmetry operation "
-            "(only necessary if `op` specifies an ISYM)."
-        ),
-    )
-    parser.add_argument(
-        "-m",
-        "--method",
-        default="spearman",
-        choices=["spearman", "pearson"],
-        help=("Method for computing correlation coefficient (spearman or pearson)"),
-    )
-    parser.add_argument(
-        "--mod2",
-        action="store_true",
-        help=("Use id mod 2 to assign delays (use when employing spacegroup hack)"),
-    )
-
-    return parser.parse_args()
-
+from rsbooster.stats.parser import BaseParser
+class ArgumentParser(BaseParser):
+    def __init__(self):
+        super().__init__(
+            description=__doc__
+        )
+        
+        # Required arguments
+        self.add_argument(
+            "mtz",
+            nargs="+",
+            help="MTZs containing crossvalidation data from careless",
+        )
+        self.add_argument(
+            "--op",
+            required=True,
+            help=(
+                "Symmetry operation to use to compute internal difference map. "
+                "Can be given as ISYM if used with a `spacegroup` argument"
+                "Symops start counting at 0 (the identity), but CCsym for the identity are NaNs."
+                "Minus signs in symops are presently causing problems!"
+            ),
+        )
+    
+        # Optional arguments
+        self.add_argument(
+            "-sg",
+            "--spacegroup",
+            help=(
+                "Spacegroup to use for symmetry operation "
+                "(only necessary if `op` specifies an ISYM)."
+            ),
+        )
+        self.add_argument(
+            "-m",
+            "--method",
+            default="spearman",
+            choices=["spearman", "pearson"],
+            help=("Method for computing correlation coefficient (spearman or pearson)"),
+        )
+        self.add_argument(
+            "--mod2",
+            action="store_true",
+            help=("Use id mod 2 to assign delays (use when employing spacegroup hack)"),
+        )
 
 def make_halves_ccsym(mtz, op, bins=10):
     """Construct half-datasets for computing CCsym"""
     half1 = mtz.loc[mtz.half == 0].copy()
     half2 = mtz.loc[mtz.half == 1].copy()
 
     temp1 = half1.merge(
@@ -88,17 +88,23 @@
 
 
 def analyze_ccsym_mtz(
     mtzpath, op, bins=10, return_labels=True, method="spearman", mod2=False
 ):
     """Compute CCsym from 2-fold cross-validation"""
 
-    mtz = rs.read_mtz(mtzpath)
+    if type(mtzpath) is rs.dataset.DataSet:
+        mtz=mtzpath
+    else:
+        mtz = rs.read_mtz(mtzpath)
+    
     m, labels = make_halves_ccsym(mtz, op)
 
+    # print(m)
+    # print(labels)
     grouper = m.groupby(["bin", "repeat"])[["DF1", "DF2"]]
     result = (
         grouper.corr(method=method).unstack()[("DF1", "DF2")].to_frame().reset_index()
     )
 
     if mod2:
         result["delay"] = np.floor(int(mtzpath[-5]) / 2)
@@ -107,26 +113,23 @@
 
     if return_labels:
         return result, labels
     else:
         return result
 
 
-def main():
-
-    # Parse commandline arguments
-    args = parse_arguments()
-
+def run_analysis(args):
     # Get symmetry operation
     try:
         isym = int(args.op)
         sg = gemmi.SpaceGroup(args.spacegroup)
         op = sg.operations().sym_ops[isym]
     except ValueError:
         op = gemmi.Op(args.op)
+    print(op)
 
     results = []
     labels = None
     for m in args.mtz:
         result = analyze_ccsym_mtz(m, op, method=args.method, mod2=args.mod2)
         if result is None:
             continue
@@ -134,23 +137,38 @@
             results.append(result[0])
             labels = result[1]
 
     results = rs.concat(results, check_isomorphous=False)
     results = results.reset_index(drop=True)
     results["CCsym"] = results[("DF1", "DF2")]
     results.drop(columns=[("DF1", "DF2")], inplace=True)
+        
+    for k in ('bin', 'repeat'):
+        results[k] = results[k].to_numpy('int32')
 
-    print(results)
+    if args.output is not None:
+        results.to_csv(args.output)
+    else:
+        print(results.to_string())
 
+    results.info()
     sns.lineplot(
-        data=results, x="bin", y="CCsym", hue="delay", ci="sd", palette="viridis"
+        data=results, x="bin", y="CCsym", hue="delay", errorbar="sd", palette="viridis"
     )
     plt.xticks(range(10), labels, rotation=45, ha="right", rotation_mode="anchor")
     plt.ylabel(r"$CC_{sym}$ " + f"({args.method})")
     plt.legend(loc="center left", bbox_to_anchor=(1, 0.5))
     plt.grid()
     plt.tight_layout()
-    plt.show()
+    
+    if args.image is not None:
+        plt.savefig(args.image)
+
+    if args.show:
+        plt.show()
 
 
-if __name__ == "__main__":
-    main()
+def parse_arguments():
+    return ArgumentParser()
+
+def main():
+    run_analysis(parse_arguments().parse_args())
```

### Comparing `rs-booster-0.1.0/rsbooster/utils/io.py` & `rs-booster-0.1.1/rsbooster/utils/io.py`

 * *Files identical despite different names*

### Comparing `rs-booster-0.1.0/setup.py` & `rs-booster-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,42 +20,55 @@
     "Bug Tracker": "https://github.com/rs-station/rs-booster/issues",
     "Source Code": "https://github.com/rs-station/rs-booster",
 }
 
 # Testing requirements
 tests_require = ["pytest", "pytest-xdist", "pytest-runner"]
 
+# Requirements for building docs
+docs_require = [
+        "sphinx",
+        "sphinx_rtd_theme",
+        "nbsphinx",
+        "sphinxcontrib-autoprogram",
+        "autodocsumm",
+        ]
+
 setup(
     name="rs-booster",
     packages=find_packages(),
     include_package_data=True,
     version=__version__,
     license="MIT",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author="Jack B. Greisman",
     author_email="greisman@g.harvard.edu",
     url="https://github.com/rs-station/rs-booster",
     project_urls=PROJECT_URLS,
     python_requires=">3.7",
     install_requires=["reciprocalspaceship", "matplotlib", "seaborn"],
-    extras_require={"dev": tests_require},
+    extras_require={
+        "dev": tests_require + docs_require,
+        "docs": docs_require
+    },
     entry_points={
         "console_scripts": [
             "rs.extrapolate=rsbooster.esf.extrapolate:main",
             "rs.scaleit=rsbooster.scaleit.scaleit:main",
             "rs.internal_diffmap=rsbooster.diffmaps.internaldiffmap:main",
             "rs.ccsym=rsbooster.stats.ccsym:main",
             "rs.ccanom=rsbooster.stats.ccanom:main",
             "rs.cchalf=rsbooster.stats.cchalf:main",
             "rs.ccpred=rsbooster.stats.ccpred:main",
             "rs.diffmap=rsbooster.diffmaps.diffmap:main",
             "rs.precog2mtz=rsbooster.io.precog2mtz:main",
             "rs.find_peaks=rsbooster.realspace.find_peaks:find_peaks",
             "rs.find_difference_peaks=rsbooster.realspace.find_peaks:find_difference_peaks",
+            "rs.rfree=rsbooster.utils.rfree:main",
         ]
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
```

