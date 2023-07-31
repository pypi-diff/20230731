# Comparing `tmp/pyaogmaneo-2.1.1.tar.gz` & `tmp/pyaogmaneo-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.1.1.tar", last modified: Sat Jul 29 15:23:29 2023, max compression
+gzip compressed data, was "pyaogmaneo-2.1.2.tar", last modified: Mon Jul 31 00:20:52 2023, max compression
```

## Comparing `pyaogmaneo-2.1.1.tar` & `pyaogmaneo-2.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.150615 pyaogmaneo-2.1.1/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/CMake/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.1/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-29 15:21:13.000000 pyaogmaneo-2.1.1/CMakeLists.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.1/LICENSE.md
--rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.1/MANIFEST.in
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/README.md
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/
--rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-29 15:23:29.000000 pyaogmaneo-2.1.1/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.1/pyproject.toml
--rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-29 15:23:29.150615 pyaogmaneo-2.1.1/setup.cfg
--rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-29 15:20:49.000000 pyaogmaneo-2.1.1/setup.py
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/source/
-drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-29 15:23:29.147282 pyaogmaneo-2.1.1/source/pyaogmaneo/
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)    15776 2023-07-29 00:23:47.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     7013 2023-07-29 15:21:32.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-28 23:07:46.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 ericl     (1000) ericl     (1001)     9243 2023-07-29 15:11:58.000000 pyaogmaneo-2.1.1/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/CMake/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1250 2023-03-18 01:02:16.000000 pyaogmaneo-2.1.2/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2620 2023-07-31 00:18:20.000000 pyaogmaneo-2.1.2/CMakeLists.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    17842 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.2/LICENSE.md
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       64 2022-12-03 02:07:03.000000 pyaogmaneo-2.1.2/MANIFEST.in
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     2412 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/README.md
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      785 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      505 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)        1 2023-06-29 17:53:40.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       11 2023-07-31 00:20:52.000000 pyaogmaneo-2.1.2/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 ericl     (1000) ericl     (1001)      101 2023-01-13 01:36:37.000000 pyaogmaneo-2.1.2/pyproject.toml
+-rw-r--r--   0 ericl     (1000) ericl     (1001)       38 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/setup.cfg
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     4204 2023-07-31 00:18:29.000000 pyaogmaneo-2.1.2/setup.py
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/source/
+drwxr-xr-x   0 ericl     (1000) ericl     (1001)        0 2023-07-31 00:20:52.900270 pyaogmaneo-2.1.2/source/pyaogmaneo/
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1071 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     1783 2023-06-22 14:37:40.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)    15776 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     7013 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     8140 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     3217 2023-07-26 01:03:23.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 ericl     (1000) ericl     (1001)     9243 2023-07-30 17:43:03.000000 pyaogmaneo-2.1.2/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.1.1/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.1.2/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/CMakeLists.txt` & `pyaogmaneo-2.1.2/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 76314e0d90d723c8d655815d190bef46409e86d8
+        GIT_TAG 50588dd81a02a94747abe79f2fb81c721a33f81d
     )
 
     FetchContent_GetProperties(AOgmaNeo)
 
     if(NOT AOgmaNeo_POPULATED)
         FetchContent_Populate(AOgmaNeo)
         add_subdirectory(${aogmaneo_SOURCE_DIR} ${aogmaneo_BINARY_DIR})
```

### Comparing `pyaogmaneo-2.1.1/LICENSE.md` & `pyaogmaneo-2.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/PKG-INFO` & `pyaogmaneo-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.1/README.md` & `pyaogmaneo-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.1.2/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.1.1/setup.py` & `pyaogmaneo-2.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.1.1",
+    version="2.1.2",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_hierarchy.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_image_encoder.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.1.1/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.1.2/source/pyaogmaneo/py_module.cpp`

 * *Files identical despite different names*

