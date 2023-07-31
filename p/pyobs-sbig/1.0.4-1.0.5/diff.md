# Comparing `tmp/pyobs_sbig-1.0.4.tar.gz` & `tmp/pyobs_sbig-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_sbig-1.0.4.tar", max compression
+gzip compressed data, was "pyobs_sbig-1.0.5.tar", max compression
```

## Comparing `pyobs_sbig-1.0.4.tar` & `pyobs_sbig-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1099 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/LICENSE
--rw-r--r--   0        0        0     1219 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/build.py
--rw-r--r--   0        0        0      121 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/__init__.py
--rw-r--r--   0        0        0     1592 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbig6303e.py
--rw-r--r--   0        0        0    10011 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigcamera.py
--rw-r--r--   0        0        0     7661 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigfiltercamera.py
--rw-r--r--   0        0        0     9399 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pxd
--rw-r--r--   0        0        0     9472 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pyx
--rw-r--r--   0        0        0      715 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    46914 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/src/csbigcam.cpp
--rw-r--r--   0        0        0     6041 2023-07-04 18:33:27.882204 pyobs_sbig-1.0.4/src/csbigcam.h
--rw-r--r--   0        0        0    60914 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/csbigimg.cpp
--rw-r--r--   0        0        0    10777 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/csbigimg.h
--rw-r--r--   0        0        0      850 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/lpardrv.h
--rw-r--r--   0        0        0    28066 2023-07-04 18:33:27.886204 pyobs_sbig-1.0.4/src/sbigudrv.h
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1394 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/build.py
+-rw-r--r--   0        0        0      121 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/__init__.py
+-rw-r--r--   0        0        0     1592 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/sbig6303e.py
+-rw-r--r--   0        0        0    10011 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/sbigcamera.py
+-rw-r--r--   0        0        0     7661 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/sbigfiltercamera.py
+-rw-r--r--   0        0        0     9399 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/sbigudrv.pxd
+-rw-r--r--   0        0        0     9472 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyobs_sbig/sbigudrv.pyx
+-rw-r--r--   0        0        0      722 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    46914 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/csbigcam.cpp
+-rw-r--r--   0        0        0     6041 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/csbigcam.h
+-rw-r--r--   0        0        0    60914 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/csbigimg.cpp
+-rw-r--r--   0        0        0    10777 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/csbigimg.h
+-rw-r--r--   0        0        0      850 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/lpardrv.h
+-rw-r--r--   0        0        0    28066 2023-07-31 09:00:23.408999 pyobs_sbig-1.0.5/src/sbigudrv.h
+-rw-r--r--   0        0        0      574 1970-01-01 00:00:00.000000 pyobs_sbig-1.0.5/PKG-INFO
```

### Comparing `pyobs_sbig-1.0.4/LICENSE` & `pyobs_sbig-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyobs_sbig/sbig6303e.py` & `pyobs_sbig-1.0.5/pyobs_sbig/sbig6303e.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyobs_sbig/sbigcamera.py` & `pyobs_sbig-1.0.5/pyobs_sbig/sbigcamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyobs_sbig/sbigfiltercamera.py` & `pyobs_sbig-1.0.5/pyobs_sbig/sbigfiltercamera.py`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pxd` & `pyobs_sbig-1.0.5/pyobs_sbig/sbigudrv.pxd`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyobs_sbig/sbigudrv.pyx` & `pyobs_sbig-1.0.5/pyobs_sbig/sbigudrv.pyx`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/pyproject.toml` & `pyobs_sbig-1.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "pyobs-sbig"
-version = "1.0.4"
+version = "1.0.5"
 description = "pyobs module for SBIG cameras"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 include = ['src']
 #build = 'build.py'
 
 [tool.poetry.build]
 script = "build.py"
 generate-setup-file = false
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-numpy = "^1.21"
-astropy = "^5.0"
-pyobs-core = "^1.0"
+numpy = "^1.25.1"
+astropy = "^5.3.1"
+pyobs-core = "^1.4.5"
 
 [tool.poetry.dev-dependencies]
-black = "^21.12b0"
-pre-commit = "^2.16"
+black = "^23.7.0"
+pre-commit = "^3.3.3"
 sphinx-rtd-theme = "^1.0"
 Sphinx = "^4.4"
-Cython = "^0.29"
+Cython = "^3.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "Cython>=0.29.0", "numpy>=1.21.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `pyobs_sbig-1.0.4/src/csbigcam.cpp` & `pyobs_sbig-1.0.5/src/csbigcam.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/src/csbigcam.h` & `pyobs_sbig-1.0.5/src/csbigcam.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/src/csbigimg.cpp` & `pyobs_sbig-1.0.5/src/csbigimg.cpp`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/src/csbigimg.h` & `pyobs_sbig-1.0.5/src/csbigimg.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/src/lpardrv.h` & `pyobs_sbig-1.0.5/src/lpardrv.h`

 * *Files identical despite different names*

### Comparing `pyobs_sbig-1.0.4/src/sbigudrv.h` & `pyobs_sbig-1.0.5/src/sbigudrv.h`

 * *Files identical despite different names*

