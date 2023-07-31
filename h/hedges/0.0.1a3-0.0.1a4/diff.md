# Comparing `tmp/hedges-0.0.1a3.tar.gz` & `tmp/hedges-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedges-0.0.1a3.tar", last modified: Thu Jul 27 23:10:03 2023, max compression
+gzip compressed data, was "hedges-0.0.1a4.tar", last modified: Mon Jul 31 20:47:07 2023, max compression
```

## Comparing `hedges-0.0.1a3.tar` & `hedges-0.0.1a4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       99 2023-07-19 18:52:52.000000 hedges-0.0.1a3/.gitignore
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      246 2023-07-23 20:16:02.000000 hedges-0.0.1a3/Makefile
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-27 23:10:03.460245 hedges-0.0.1a3/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7539 2023-07-27 23:08:35.000000 hedges-0.0.1a3/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:35:03.000000 hedges-0.0.1a3/hedges/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      162 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges/_version.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     3046 2023-07-25 08:44:31.000000 hedges-0.0.1a3/hedges/bc.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      679 2023-07-15 21:50:14.000000 hedges-0.0.1a3/hedges/fluxes.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)    15144 2023-07-19 18:59:52.000000 hedges-0.0.1a3/hedges/hyperbolic_solver_1d.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4976 2023-07-19 18:59:56.000000 hedges-0.0.1a3/hedges/quadrature.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     2993 2023-07-11 06:47:01.000000 hedges-0.0.1a3/hedges/rk.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges/swe_1d/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:32:56.000000 hedges-0.0.1a3/hedges/swe_1d/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)    10353 2023-07-27 22:43:29.000000 hedges-0.0.1a3/hedges/swe_1d/pde.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      827 2023-07-26 08:41:33.000000 hedges-0.0.1a3/hedges/swe_1d/steady.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 23:10:03.460245 hedges-0.0.1a3/hedges.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)      433 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)        1 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       23 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       12 2023-07-27 23:10:03.000000 hedges-0.0.1a3/hedges.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7804 2023-07-27 23:07:03.000000 hedges-0.0.1a3/main.ipynb
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4335 2023-07-27 23:06:15.000000 hedges-0.0.1a3/main.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)     1465 2023-07-19 18:54:57.000000 hedges-0.0.1a3/pyproject.toml
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       46 2023-07-19 18:10:56.000000 hedges-0.0.1a3/requirements.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1004)       38 2023-07-27 23:10:03.460245 hedges-0.0.1a3/setup.cfg
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-31 20:47:07.145480 hedges-0.0.1a4/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       99 2023-07-19 18:52:52.000000 hedges-0.0.1a4/.gitignore
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      246 2023-07-23 20:16:02.000000 hedges-0.0.1a4/Makefile
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-31 20:47:07.145480 hedges-0.0.1a4/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7539 2023-07-27 23:08:35.000000 hedges-0.0.1a4/README.md
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-31 20:47:07.142146 hedges-0.0.1a4/hedges/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:35:03.000000 hedges-0.0.1a4/hedges/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      162 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges/_version.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     3046 2023-07-25 08:44:31.000000 hedges-0.0.1a4/hedges/bc.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      679 2023-07-15 21:50:14.000000 hedges-0.0.1a4/hedges/fluxes.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)    15144 2023-07-19 18:59:52.000000 hedges-0.0.1a4/hedges/hyperbolic_solver_1d.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4976 2023-07-19 18:59:56.000000 hedges-0.0.1a4/hedges/quadrature.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     2993 2023-07-11 06:47:01.000000 hedges-0.0.1a4/hedges/rk.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-31 20:47:07.145480 hedges-0.0.1a4/hedges/swe_1d/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        0 2023-07-27 22:32:56.000000 hedges-0.0.1a4/hedges/swe_1d/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)    10353 2023-07-27 22:43:29.000000 hedges-0.0.1a4/hedges/swe_1d/pde.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      929 2023-07-31 20:36:33.000000 hedges-0.0.1a4/hedges/swe_1d/steady.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1004)        0 2023-07-31 20:47:07.145480 hedges-0.0.1a4/hedges.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     8690 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)      433 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)        1 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       23 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       12 2023-07-31 20:47:07.000000 hedges-0.0.1a4/hedges.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     7804 2023-07-27 23:07:03.000000 hedges-0.0.1a4/main.ipynb
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     4335 2023-07-27 23:25:01.000000 hedges-0.0.1a4/main.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)     1465 2023-07-19 18:54:57.000000 hedges-0.0.1a4/pyproject.toml
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       46 2023-07-19 18:10:56.000000 hedges-0.0.1a4/requirements.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1004)       38 2023-07-31 20:47:07.145480 hedges-0.0.1a4/setup.cfg
```

### Comparing `hedges-0.0.1a3/PKG-INFO` & `hedges-0.0.1a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedges
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A Discontinuous Galerkin solver oriented toward prototyping and education
 Author-email: schrodingersket <schrodingersket@gmail.com>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/schrodingersket/hedges
 Project-URL: Bug Tracker, https://github.com/schrodingersket/hedges/issues
 Keywords: Partial differential equations,Hyperbolic,Scientific computing,Scientific machine learning,Discontinuous Galerkin
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hedges-0.0.1a3/README.md` & `hedges-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/bc.py` & `hedges-0.0.1a4/hedges/bc.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/fluxes.py` & `hedges-0.0.1a4/hedges/fluxes.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/hyperbolic_solver_1d.py` & `hedges-0.0.1a4/hedges/hyperbolic_solver_1d.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/quadrature.py` & `hedges-0.0.1a4/hedges/quadrature.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/rk.py` & `hedges-0.0.1a4/hedges/rk.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges/swe_1d/pde.py` & `hedges-0.0.1a4/hedges/swe_1d/pde.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/hedges.egg-info/PKG-INFO` & `hedges-0.0.1a4/hedges.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedges
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A Discontinuous Galerkin solver oriented toward prototyping and education
 Author-email: schrodingersket <schrodingersket@gmail.com>
 License: LGPL-2.1
 Project-URL: Homepage, https://github.com/schrodingersket/hedges
 Project-URL: Bug Tracker, https://github.com/schrodingersket/hedges/issues
 Keywords: Partial differential equations,Hyperbolic,Scientific computing,Scientific machine learning,Discontinuous Galerkin
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `hedges-0.0.1a3/main.ipynb` & `hedges-0.0.1a4/main.ipynb`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/main.py` & `hedges-0.0.1a4/main.py`

 * *Files identical despite different names*

### Comparing `hedges-0.0.1a3/pyproject.toml` & `hedges-0.0.1a4/pyproject.toml`

 * *Files identical despite different names*

