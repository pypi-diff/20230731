# Comparing `tmp/pygrb_lc-0.1.5.tar.gz` & `tmp/pygrb_lc-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygrb_lc-0.1.5.tar", last modified: Thu Jul 27 22:46:35 2023, max compression
+gzip compressed data, was "pygrb_lc-0.1.6.tar", last modified: Mon Jul 31 11:01:08 2023, max compression
```

## Comparing `pygrb_lc-0.1.5.tar` & `pygrb_lc-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:35.538818 pygrb_lc-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/src/pygrb_lc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/blind_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/crossmatching.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/furie.py
--rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/src/pygrb_lc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/src/pygrb_lc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-27 22:46:35.000000 pygrb_lc-0.1.5/src/pygrb_lc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-27 22:46:35.000000 pygrb_lc-0.1.5/src/pygrb_lc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 22:46:35.000000 pygrb_lc-0.1.5/src/pygrb_lc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-27 22:46:35.000000 pygrb_lc-0.1.5/src/pygrb_lc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:35.542818 pygrb_lc-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/tests/test_light_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-27 22:46:25.000000 pygrb_lc-0.1.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:01:08.428286 pygrb_lc-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/src/pygrb_lc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/blind_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/crossmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/furie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/src/pygrb_lc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/src/pygrb_lc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-31 11:01:08.000000 pygrb_lc-0.1.6/src/pygrb_lc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-31 11:01:08.000000 pygrb_lc-0.1.6/src/pygrb_lc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:01:08.000000 pygrb_lc-0.1.6/src/pygrb_lc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 11:01:08.000000 pygrb_lc-0.1.6/src/pygrb_lc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:01:08.432286 pygrb_lc-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/tests/test_light_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 11:00:53.000000 pygrb_lc-0.1.6/tests/test_utils.py
```

### Comparing `pygrb_lc-0.1.5/LICENSE` & `pygrb_lc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/PKG-INFO` & `pygrb_lc-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb_lc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.5/README.md` & `pygrb_lc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/setup.cfg` & `pygrb_lc-0.1.6/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pygrb_lc
-version = 0.1.5
+version = 0.1.6
 author = Mozgunov Georgiy
 author_email = georgiy99@bk.ru
 description = Python package for GRB analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Jorezzz/pygrb_lc
 project_urls =
```

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/blind_search.py` & `pygrb_lc-0.1.6/src/pygrb_lc/blind_search.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/catalogs.py` & `pygrb_lc-0.1.6/src/pygrb_lc/catalogs.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/config.py` & `pygrb_lc-0.1.6/src/pygrb_lc/config.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/crossmatching.py` & `pygrb_lc-0.1.6/src/pygrb_lc/crossmatching.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/furie.py` & `pygrb_lc-0.1.6/src/pygrb_lc/furie.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         self.interval_t90 = interval_t90
 
         rebined_param = np.polyfit(self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).times,
                                    self.light_curve.rebin(bkg_substraction_resolution).set_intervals(*bkg_intervals).signal,
                                    bkg_polynom_degree)
         rebined_param = rebined_param * (self.light_curve.original_resolution/self.light_curve.resolution)
         self.rebined_param = rebined_param
-        self.N = np.sum(self.light_curve.rebin().set_intervals(*bkg_intervals).signal)
+        self.N = np.sum(self.light_curve.rebin().set_intervals(*interval_t90).signal)
 
         signal = self.light_curve.rebin().substract_polynom(rebined_param).set_intervals(interval_t90).signal
         
 
         if window is not None:
             signal = signal * window(signal.shape[0])
```

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/light_curves.py` & `pygrb_lc-0.1.6/src/pygrb_lc/light_curves.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/time.py` & `pygrb_lc-0.1.6/src/pygrb_lc/time.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc/utils.py` & `pygrb_lc-0.1.6/src/pygrb_lc/utils.py`

 * *Files identical despite different names*

### Comparing `pygrb_lc-0.1.5/src/pygrb_lc.egg-info/PKG-INFO` & `pygrb_lc-0.1.6/src/pygrb_lc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygrb-lc
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python package for GRB analysis
 Home-page: https://github.com/Jorezzz/pygrb_lc
 Author: Mozgunov Georgiy
 Author-email: georgiy99@bk.ru
 Project-URL: Bug Tracker, https://github.com/Jorezzz/pygrb_lc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pygrb_lc-0.1.5/tests/test_utils.py` & `pygrb_lc-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

