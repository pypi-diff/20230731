# Comparing `tmp/mms_nirs-0.1.4.tar.gz` & `tmp/mms_nirs-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_nirs-0.1.4.tar", max compression
+gzip compressed data, was "mms_nirs-0.1.5.tar", max compression
```

## Comparing `mms_nirs-0.1.4.tar` & `mms_nirs-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.4/README.md
--rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.4/mms_nirs/UCLN/DefaultValues.py
--rw-r--r--   0        0        0     3309 2023-05-16 10:47:43.079500 mms_nirs-0.1.4/mms_nirs/UCLN/UCLN.py
--rw-r--r--   0        0        0      152 2023-05-16 10:47:43.079500 mms_nirs-0.1.4/mms_nirs/UCLN/__init__.py
--rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.4/mms_nirs/UCLN/defaults.csv
--rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.4/mms_nirs/__init__.py
--rw-r--r--   0        0        0      892 2023-05-16 10:48:10.839500 mms_nirs-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 mms_nirs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-03 11:01:49.168314 mms_nirs-0.1.5/README.md
+-rw-r--r--   0        0        0      333 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/__init__.py
+-rw-r--r--   0        0        0     3323 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/calc_values.py
+-rw-r--r--   0        0        0     4835 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/derivative_fit.py
+-rw-r--r--   0        0        0     5525 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/fminsearchbnd.py
+-rw-r--r--   0        0        0     4335 2023-07-31 12:30:11.002332 mms_nirs-0.1.5/mms_nirs/BRUNO/model_types.py
+-rw-r--r--   0        0        0      662 2023-05-09 17:15:42.681482 mms_nirs-0.1.5/mms_nirs/UCLN/DefaultValues.py
+-rw-r--r--   0        0        0     3309 2023-07-31 09:39:28.273500 mms_nirs-0.1.5/mms_nirs/UCLN/UCLN.py
+-rw-r--r--   0        0        0      152 2023-05-16 10:47:43.079500 mms_nirs-0.1.5/mms_nirs/UCLN/__init__.py
+-rw-r--r--   0        0        0     3876 2023-05-09 17:15:42.681482 mms_nirs-0.1.5/mms_nirs/UCLN/defaults.csv
+-rw-r--r--   0        0        0        0 2023-05-02 14:50:03.986089 mms_nirs-0.1.5/mms_nirs/__init__.py
+-rw-r--r--   0        0        0      908 2023-07-31 12:34:33.022303 mms_nirs-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 mms_nirs-0.1.5/PKG-INFO
```

### Comparing `mms_nirs-0.1.4/mms_nirs/UCLN/DefaultValues.py` & `mms_nirs-0.1.5/mms_nirs/UCLN/DefaultValues.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.4/mms_nirs/UCLN/UCLN.py` & `mms_nirs-0.1.5/mms_nirs/UCLN/UCLN.py`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.4/mms_nirs/UCLN/defaults.csv` & `mms_nirs-0.1.5/mms_nirs/UCLN/defaults.csv`

 * *Files identical despite different names*

### Comparing `mms_nirs-0.1.4/pyproject.toml` & `mms_nirs-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "mms-nirs"
-version = "0.1.4"
+version = "0.1.5"
 description = "Algorithms used in the multimodal spectroscopy group to process NIRS data"
 authors = ["Josh Buckland, <joshua.russell-buckland@ucl.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "mms_nirs" }]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 numpy = "^1.24.3"
 scipy = "^1.10.1"
 pandas = "^2.0.1"
 pyarrow = "^12.0.0"
+sympy = "^1.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 black = "^23.3.0"
 poetry2setup = "^1.1.0"
```

### Comparing `mms_nirs-0.1.4/PKG-INFO` & `mms_nirs-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: mms-nirs
-Version: 0.1.4
+Version: 0.1.5
 Summary: Algorithms used in the multimodal spectroscopy group to process NIRS data
 License: MIT
 Author: Josh Buckland,
 Author-email: joshua.russell-buckland@ucl.ac.uk
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
+Requires-Dist: sympy (>=1.12,<2.0)
 Description-Content-Type: text/markdown
 
 # MMS NIRS
 
 ## What
 
 This repo contains Python code that can be used with the NIRS data generated at the multimodal spectroscopy group at UCL.
```

