# Comparing `tmp/anesthetic-2.1.2.tar.gz` & `tmp/anesthetic-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.1.2.tar", last modified: Thu Jul 27 03:23:57 2023, max compression
+gzip compressed data, was "anesthetic-2.1.3.tar", last modified: Mon Jul 31 17:33:18 2023, max compression
```

## Comparing `anesthetic-2.1.2.tar` & `anesthetic-2.1.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.903610 anesthetic-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-27 03:23:49.000000 anesthetic-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 03:23:57.903610 anesthetic-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-27 03:23:49.000000 anesthetic-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.891610 anesthetic-2.1.2/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.895610 anesthetic-2.1.2/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.895610 anesthetic-2.1.2/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    54730 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.895610 anesthetic-2.1.2/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.895610 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.899610 anesthetic-2.1.2/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (123)    50784 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-07-27 03:23:49.000000 anesthetic-2.1.2/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.895610 anesthetic-2.1.2/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-27 03:23:57.000000 anesthetic-2.1.2/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-27 03:23:49.000000 anesthetic-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-27 03:23:57.903610 anesthetic-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 03:23:57.903610 anesthetic-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    65301 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34365 2023-07-27 03:23:49.000000 anesthetic-2.1.2/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.245205 anesthetic-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 17:33:05.000000 anesthetic-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-31 17:33:18.245205 anesthetic-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-31 17:33:05.000000 anesthetic-2.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.237205 anesthetic-2.1.3/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54730 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50784 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-07-31 17:33:05.000000 anesthetic-2.1.3/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.241205 anesthetic-2.1.3/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 17:33:18.000000 anesthetic-2.1.3/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-31 17:33:05.000000 anesthetic-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-31 17:33:18.245205 anesthetic-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:33:18.245205 anesthetic-2.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65301 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34365 2023-07-31 17:33:05.000000 anesthetic-2.1.3/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.1.2/LICENSE` & `anesthetic-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/PKG-INFO` & `anesthetic-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.2
+Version: 2.1.3
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.2
+:Version: 2.1.3
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.2/README.rst` & `anesthetic-2.1.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.2
+:Version: 2.1.3
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.2/anesthetic/__init__.py` & `anesthetic-2.1.3/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/_code_utils.py` & `anesthetic-2.1.3/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/_format.py` & `anesthetic-2.1.3/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/boundary.py` & `anesthetic-2.1.3/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/convert.py` & `anesthetic-2.1.3/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/examples/perfect_ns.py` & `anesthetic-2.1.3/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/examples/utils.py` & `anesthetic-2.1.3/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/gui/plot.py` & `anesthetic-2.1.3/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/gui/widgets.py` & `anesthetic-2.1.3/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/kde.py` & `anesthetic-2.1.3/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/labelled_pandas.py` & `anesthetic-2.1.3/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plot.py` & `anesthetic-2.1.3/anesthetic/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plotting/_core.py` & `anesthetic-2.1.3/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.1.3/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.1.3/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.1.3/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.1.3/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/chain.py` & `anesthetic-2.1.3/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/cobaya.py` & `anesthetic-2.1.3/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/getdist.py` & `anesthetic-2.1.3/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/hdf.py` & `anesthetic-2.1.3/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/multinest.py` & `anesthetic-2.1.3/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/polychord.py` & `anesthetic-2.1.3/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/read/ultranest.py` & `anesthetic-2.1.3/anesthetic/read/ultranest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/samples.py` & `anesthetic-2.1.3/anesthetic/samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/scripts.py` & `anesthetic-2.1.3/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/utils.py` & `anesthetic-2.1.3/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic/weighted_pandas.py` & `anesthetic-2.1.3/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.1.3/anesthetic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.2
+Version: 2.1.3
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.2
+:Version: 2.1.3
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.2/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.1.3/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/pyproject.toml` & `anesthetic-2.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 [project.urls]
 "Homepage" = "https://github.com/handley-lab/anesthetic"
 "Bug Tracker" = "https://github.com/handley-lab/anesthetic/issues"
 "Documentation" = "https://anesthetic.readthedocs.io/en/latest/"
 "JOSS paper" = "https://joss.theoj.org/papers/10.21105/joss.01414"
 
 [project.optional-dependencies]
-docs = ["sphinx", "sphinx_rtd_theme", "numpydoc"]
+docs = ["sphinx", "sphinx_rtd_theme", "sphinx-copybutton", "numpydoc"]
 test = ["pytest", "pytest-cov", "flake8", "pydocstyle", "packaging", "pre-commit"]
 ultranest = ["h5py"]
 astropy = ["astropy"]
 fastkde = ["fastkde"]
 getdist = ["getdist"]
 hdf5 = ["tables"]
 all = ["h5py", "astropy", "fastkde", "getdist", "tables"]
```

### Comparing `anesthetic-2.1.2/tests/test_convert.py` & `anesthetic-2.1.3/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_examples.py` & `anesthetic-2.1.3/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_gui.py` & `anesthetic-2.1.3/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_labelled_pandas.py` & `anesthetic-2.1.3/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_plot.py` & `anesthetic-2.1.3/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_reader.py` & `anesthetic-2.1.3/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_samples.py` & `anesthetic-2.1.3/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_scripts.py` & `anesthetic-2.1.3/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_utils.py` & `anesthetic-2.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.2/tests/test_weighted_pandas.py` & `anesthetic-2.1.3/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

