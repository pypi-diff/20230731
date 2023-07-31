# Comparing `tmp/jij_cimod-1.4.9.tar.gz` & `tmp/jij_cimod-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jij_cimod-1.4.9.tar", last modified: Tue Jun 28 04:21:09 2022, max compression
+gzip compressed data, was "jij_cimod-1.5.0.tar", last modified: Mon Jul 31 06:03:38 2023, max compression
```

## Comparing `jij_cimod-1.4.9.tar` & `jij_cimod-1.5.0.tar`

### file list

```diff
@@ -1,71 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)     1719 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.gitattribute
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/.reviewdog.yml
--rw-r--r--   0 runner    (1001) docker     (121)     5447 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.261040 jij_cimod-1.4.9/cimod/
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/cimod/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3168 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/main.cpp
--rw-r--r--   0 runner    (1001) docker     (121)    12692 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/main.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.261040 jij_cimod-1.4.9/cimod/model/
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31154 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/binary_polynomial_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    13751 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/binary_quadratic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cimod/model/legacy/
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14098 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/model/legacy/binary_quadratic_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cimod/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/decolator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (121)     1119 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cimod/vartype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/cmake/
--rw-r--r--   0 runner    (1001) docker     (121)     5228 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/FindGcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)    12711 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/FindLcov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     9023 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/Findcodecov.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     4448 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/GenerateDocs.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1937 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/PythonAutoDetectOSX.cmake
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/cmake/llvm-cov-wrapper
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.265040 jij_cimod-1.4.9/external/
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/eigen.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/googletest.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/json.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/pybind11-json.cmake
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/external/pybind11.cmake
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.269040 jij_cimod-1.4.9/jij_cimod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 04:21:08.000000 jij_cimod-1.4.9/jij_cimod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-06-28 04:21:09.000000 jij_cimod-1.4.9/jij_cimod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3303 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1847 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.269040 jij_cimod-1.4.9/src/
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)    44450 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_polynomial_model.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    66766 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_quadratic_model.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    41145 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/binary_quadratic_model_dict.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1131 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/disable_eigen_warning.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/hash.hpp
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/json.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/utilities.hpp
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/src/vartypes.hpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 04:21:09.273041 jij_cimod-1.4.9/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    56485 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     2066 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_0_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)    30862 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_bqm.hpp
--rw-r--r--   0 runner    (1001) docker     (121)    12348 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_legacy_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    74844 2022-06-28 04:20:46.000000 jij_cimod-1.4.9/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.977972 jij_cimod-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/.reviewdog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-31 06:03:38.977972 jij_cimod-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.961972 jij_cimod-1.5.0/cimod/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/cimod/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/main.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.965972 jij_cimod-1.5.0/cimod/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31140 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/model/binary_polynomial_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/model/binary_quadratic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.965972 jij_cimod-1.5.0/cimod/model/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/model/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/model/legacy/binary_quadratic_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.965972 jij_cimod-1.5.0/cimod/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/utils/decolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cimod/vartype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.969972 jij_cimod-1.5.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/FindGcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/FindLcov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/Findcodecov.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/GenerateDocs.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/PythonAutoDetectOSX.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/cmake/llvm-cov-wrapper
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/doc-requirements.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.969972 jij_cimod-1.5.0/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/external/eigen.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/external/googletest.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/external/json.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/external/pybind11-json.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/external/pybind11.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.969972 jij_cimod-1.5.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.973972 jij_cimod-1.5.0/include/cimod/
+-rw-r--r--   0 runner    (1001) docker     (123)    44495 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/binary_polynomial_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    66672 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/binary_quadratic_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    40987 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/binary_quadratic_model_dict.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/disable_eigen_warning.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/hash.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/json.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/utilities.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/include/cimod/vartypes.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.977972 jij_cimod-1.5.0/jij_cimod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 06:03:38.000000 jij_cimod-1.5.0/jij_cimod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-31 06:03:38.981972 jij_cimod-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 06:03:38.977972 jij_cimod-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56503 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/test_0_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30868 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/test_bqm.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/test_legacy_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75135 2023-07-31 06:03:17.000000 jij_cimod-1.5.0/tests/test_model.py
```

### Comparing `jij_cimod-1.4.9/LICENSE` & `jij_cimod-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/MANIFEST.in` & `jij_cimod-1.5.0/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,32 @@
+prune benchmark
+prune project_template
+prune public
+prune www
+prune share
+prune **/include
+prune docs
+prune example
+prune .github
+prune .git
+prune cmake
+
 include setup.py
 include setup.cfg
 include CMakeLists.txt
 include LICENSE
 include README.md
 include pyproject.toml
+include include/CMakeLists.txt
 
-graft openjij
+graft cimod
 graft tests 
 graft src 
 graft external
-
-prune cmake
+graft include/cimod
 
 include cmake/GenerateDocs.cmake
 include cmake/PythonAutoDetectOSX.cmake
 include cmake/FindGcov.cmake 
 include cmake/FindLcov.cmake
 include cmake/Findcodecov.cmake
 include cmake/llvm-cov-wrapper
@@ -31,18 +43,11 @@
 global-exclude dev-requirements.txt
 global-exclude format-requirements.txt
 global-exclude build-requirements.in
 global-exclude build-requirements.txt
 global-exclude .gitignore 
 global-exclude Doxyfile
 global-exclude Doxyfile.bak
-
-prune benchmark
-prune project_template
-prune public
-prune www
-prune share
-prune include
-prune docs
-prune example
-prune .github
-prune .git
+global-exclude .coveragerc
+global-exclude .gitattribute
+global-exclude CODE_OF_CONDUCT.md
+global-exclude doc-requirements
```

### Comparing `jij_cimod-1.4.9/PKG-INFO` & `jij_cimod-1.5.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,56 +1,34 @@
-Metadata-Version: 2.1
-Name: jij_cimod
-Version: 1.4.9
-Summary: C++ library for a binary (and polynomial) quadratic model.
-Home-page: https://www.openjij.org
-Author: Jij Inc.
-Author-email: info@j-ij.com
-License: Apache License 2.0
-Project-URL: Source, https://github.com/OpenJij/cimod
-Project-URL: Documentation, https://cimod.openjij.org
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# cimod : C++ header-only library for a binary quadratic model
 
-# cimod : C++ header-only library for a binary quadratic model 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/jij-cimod.svg)](https://pypi.python.org/pypi/ji-cimod/)
 [![PyPI format](https://img.shields.io/pypi/format/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI license](https://img.shields.io/pypi/l/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI download month](https://img.shields.io/pypi/dm/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
+[![Downloads](https://pepy.tech/badge/jij-cimod)](https://pepy.tech/project/jij-cimod)
 
 [![Test](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml)
 [![Build&Upload](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml)
 [![CodeQL](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml)
 [![Build Documentation](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml)
 [![pages-build-deployment](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/55990ff022864098a2413c0cc4ab8299)](https://www.codacy.com/gh/OpenJij/cimod/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/cimod&utm_campaign=Badge_Grade)
+[![Maintainability](https://api.codeclimate.com/v1/badges/59876c82cc2200ef1dfa/maintainability)](https://codeclimate.com/github/OpenJij/cimod/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/cimod/branch/master/graph/badge.svg?token=BE45W9FJHA)](https://codecov.io/gh/OpenJij/cimod)
 
-## Coverage Graph 
-|**Sunburst**|**Grid**|**Icicle**|
-| ---- | ---- | ---- |
-|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a>|
+## Coverage Graph
 
+| **Sunburst**                                                                                                                                                     | **Grid**                                                                                                                                                     | **Icicle**                                                                                                                                                     |
+| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a> |
 
-* [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Python Documents](https://openjij.github.io/cimod/)
 
 # How to use
 
 You should only include a header `src/binary_quadratic_model.hpp` in your project.
 
 ## Example
 
@@ -106,25 +84,27 @@
 bqm = cimod.BinaryQuadraticModel(linear, quadratic, offset, vartype)
 
 print(bqm.linear)
 print(bqm.quadratic)
 
 ```
 
-## For Contributor 
+## For Contributor
+
 Use `pre-commit` for auto chech before git commit.
 `.pre-commit-config.yaml`
-``` 
+
+```
 # pipx install pre-commit 
 # or 
 # pip install pre-commit
 pre-commit install
 ```
 
-## Install 
+## Install
 
 ### via this directory
 
 ```sh
 $ python -m pip install -vvv .
 ```
 
@@ -133,70 +113,77 @@
 ```sh
 # Binary
 $ pip install jij-cimod
 # From Source 
 $ pip install --no-binary=jij-cimod jij-cimod 
 ```
 
-## Test 
+## Test
+
+### Python
 
-### Python 
 ```sh
 $ python -m venv .venv
 $ pip install pip-tools 
-$ pip-compile
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt
 $ source .venv/bin/activate
 $ export CMAKE_BUILD_TYPE=Debug
 $ python setup.py --force-cmake install --build-type Debug -G Ninja
 $ python setup.py --build-type Debug test 
 $ python -m coverage html
 ```
 
-### C++ 
+### C++
+
 ```sh
 $ mkdir build 
 $ cmake -DCMAKE_BUILD_TYPE=Debug -S . -B build
 $ cmake --build build --parallel
 $ cd build
 $ ./tests/cimod_test
 # Alternatively Use CTest 
 $ ctest --extra-verbose --parallel --schedule-random
 ```
 
 Needs: CMake > 3.22, C++17
 
-- Format 
+- Format
+
 ```sh
 $ pip-compile format-requirements.in
 $ pip-sync format-requirements.txt
 ```
-``` sh
+
+```sh
 $ python -m isort 
 $ python -m black 
 ```
 
 - Aggressive Format
-```sh 
+
+```sh
 $ python -m isort --force-single-line-imports --verbose ./cimod
 $ python -m autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports --remove-unused-variables ./cimod
 $ python -m autopep8 --in-place --aggressive --aggressive  --recursive ./cimod
 $ python -m isort ./cimod
 $ python -m black ./cimod
 ```
 
 - Lint
-```sh 
-$ pip-compile
+
+```sh
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-compile lint-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt lint-requirements.txt
 ```
-``` sh 
+
+```sh
 $ python -m flake8
 $ python -m mypy
 $ python -m pyright
 ```
 
 ## Benchmark
 
@@ -252,30 +239,33 @@
     c = benchmark(N, cimod)
     print("{} {} {}".format(N, d, c))
     fil.write("{} {} {}\n".format(N, d, c))
 ```
 
 ### Software versions
 
-|       Package        | Version |
-| -------------------- | ------- |
-| [cimod](https://github.com/OpenJij/cimod)     | 1.0.3   |
-| [dimod](https://github.com/dwavesystems/dimod)| 0.9.2   |
+| Package                                        | Version |
+| ---------------------------------------------- | ------- |
+| [cimod](https://github.com/OpenJij/cimod)      | 1.0.3   |
+| [dimod](https://github.com/dwavesystems/dimod) | 0.9.2   |
 
 ### Result
+
 ![benchmark](https://github.com/OpenJij/cimod/blob/image_store/figure.png)
 
+### Licences
+
+Copyright 2022 Jij Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");\
+you may not use this file except in compliance with the License.\
+You may obtain a copy of the License at
 
-### Licences 
-Copyright 2022 Jij Inc.  
+```
+ http://www.apache.org/licenses/LICENSE-2.0  
+```
 
-Licensed under the Apache License, Version 2.0 (the "License");  
-you may not use this file except in compliance with the License.  
-You may obtain a copy of the License at  
-
-     http://www.apache.org/licenses/LICENSE-2.0  
-
-Unless required by applicable law or agreed to in writing, software  
-distributed under the License is distributed on an "AS IS" BASIS,  
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
-See the License for the specific language governing permissions and  
-limitations under the License.  
+Unless required by applicable law or agreed to in writing, software\
+distributed under the License is distributed on an "AS IS" BASIS,\
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\
+See the License for the specific language governing permissions and\
+limitations under the License.
```

### Comparing `jij_cimod-1.4.9/README.md` & `jij_cimod-1.5.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,62 @@
-# cimod : C++ header-only library for a binary quadratic model 
+Metadata-Version: 2.1
+Name: jij_cimod
+Version: 1.5.0
+Summary: C++ library for a binary (and polynomial) quadratic model.
+Home-page: https://www.openjij.org
+Author: Jij Inc.
+Author-email: info@openjij.org
+License: Apache License 2.0
+Project-URL: Source, https://github.com/OpenJij/cimod
+Project-URL: Documentation, http://openjij.github.io/Cimod-Documentation/
+Project-URL: PythonDocumentation, https://openjij.github.io/cimod/
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Requires-Python: <3.12,>=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# cimod : C++ header-only library for a binary quadratic model
+
 [![PyPI version shields.io](https://img.shields.io/pypi/v/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/jij-cimod.svg)](https://pypi.python.org/pypi/ji-cimod/)
 [![PyPI format](https://img.shields.io/pypi/format/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI license](https://img.shields.io/pypi/l/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI download month](https://img.shields.io/pypi/dm/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
+[![Downloads](https://pepy.tech/badge/jij-cimod)](https://pepy.tech/project/jij-cimod)
 
 [![Test](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml)
 [![Build&Upload](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml)
 [![CodeQL](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml)
 [![Build Documentation](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml)
 [![pages-build-deployment](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/55990ff022864098a2413c0cc4ab8299)](https://www.codacy.com/gh/OpenJij/cimod/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/cimod&utm_campaign=Badge_Grade)
+[![Maintainability](https://api.codeclimate.com/v1/badges/59876c82cc2200ef1dfa/maintainability)](https://codeclimate.com/github/OpenJij/cimod/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/cimod/branch/master/graph/badge.svg?token=BE45W9FJHA)](https://codecov.io/gh/OpenJij/cimod)
 
-## Coverage Graph 
-|**Sunburst**|**Grid**|**Icicle**|
-| ---- | ---- | ---- |
-|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a>|
+## Coverage Graph
 
+| **Sunburst**                                                                                                                                                     | **Grid**                                                                                                                                                     | **Icicle**                                                                                                                                                     |
+| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a> |
 
-* [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Python Documents](https://openjij.github.io/cimod/)
 
 # How to use
 
 You should only include a header `src/binary_quadratic_model.hpp` in your project.
 
 ## Example
 
@@ -79,25 +112,27 @@
 bqm = cimod.BinaryQuadraticModel(linear, quadratic, offset, vartype)
 
 print(bqm.linear)
 print(bqm.quadratic)
 
 ```
 
-## For Contributor 
+## For Contributor
+
 Use `pre-commit` for auto chech before git commit.
 `.pre-commit-config.yaml`
-``` 
+
+```
 # pipx install pre-commit 
 # or 
 # pip install pre-commit
 pre-commit install
 ```
 
-## Install 
+## Install
 
 ### via this directory
 
 ```sh
 $ python -m pip install -vvv .
 ```
 
@@ -106,70 +141,77 @@
 ```sh
 # Binary
 $ pip install jij-cimod
 # From Source 
 $ pip install --no-binary=jij-cimod jij-cimod 
 ```
 
-## Test 
+## Test
+
+### Python
 
-### Python 
 ```sh
 $ python -m venv .venv
 $ pip install pip-tools 
-$ pip-compile
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt
 $ source .venv/bin/activate
 $ export CMAKE_BUILD_TYPE=Debug
 $ python setup.py --force-cmake install --build-type Debug -G Ninja
 $ python setup.py --build-type Debug test 
 $ python -m coverage html
 ```
 
-### C++ 
+### C++
+
 ```sh
 $ mkdir build 
 $ cmake -DCMAKE_BUILD_TYPE=Debug -S . -B build
 $ cmake --build build --parallel
 $ cd build
 $ ./tests/cimod_test
 # Alternatively Use CTest 
 $ ctest --extra-verbose --parallel --schedule-random
 ```
 
 Needs: CMake > 3.22, C++17
 
-- Format 
+- Format
+
 ```sh
 $ pip-compile format-requirements.in
 $ pip-sync format-requirements.txt
 ```
-``` sh
+
+```sh
 $ python -m isort 
 $ python -m black 
 ```
 
 - Aggressive Format
-```sh 
+
+```sh
 $ python -m isort --force-single-line-imports --verbose ./cimod
 $ python -m autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports --remove-unused-variables ./cimod
 $ python -m autopep8 --in-place --aggressive --aggressive  --recursive ./cimod
 $ python -m isort ./cimod
 $ python -m black ./cimod
 ```
 
 - Lint
-```sh 
-$ pip-compile
+
+```sh
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-compile lint-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt lint-requirements.txt
 ```
-``` sh 
+
+```sh
 $ python -m flake8
 $ python -m mypy
 $ python -m pyright
 ```
 
 ## Benchmark
 
@@ -225,30 +267,33 @@
     c = benchmark(N, cimod)
     print("{} {} {}".format(N, d, c))
     fil.write("{} {} {}\n".format(N, d, c))
 ```
 
 ### Software versions
 
-|       Package        | Version |
-| -------------------- | ------- |
-| [cimod](https://github.com/OpenJij/cimod)     | 1.0.3   |
-| [dimod](https://github.com/dwavesystems/dimod)| 0.9.2   |
+| Package                                        | Version |
+| ---------------------------------------------- | ------- |
+| [cimod](https://github.com/OpenJij/cimod)      | 1.0.3   |
+| [dimod](https://github.com/dwavesystems/dimod) | 0.9.2   |
 
 ### Result
+
 ![benchmark](https://github.com/OpenJij/cimod/blob/image_store/figure.png)
 
+### Licences
+
+Copyright 2022 Jij Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");\
+you may not use this file except in compliance with the License.\
+You may obtain a copy of the License at
 
-### Licences 
-Copyright 2022 Jij Inc.  
+```
+ http://www.apache.org/licenses/LICENSE-2.0  
+```
 
-Licensed under the Apache License, Version 2.0 (the "License");  
-you may not use this file except in compliance with the License.  
-You may obtain a copy of the License at  
-
-     http://www.apache.org/licenses/LICENSE-2.0  
-
-Unless required by applicable law or agreed to in writing, software  
-distributed under the License is distributed on an "AS IS" BASIS,  
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
-See the License for the specific language governing permissions and  
-limitations under the License.  
+Unless required by applicable law or agreed to in writing, software\
+distributed under the License is distributed on an "AS IS" BASIS,\
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\
+See the License for the specific language governing permissions and\
+limitations under the License.
```

### Comparing `jij_cimod-1.4.9/cimod/CMakeLists.txt` & `jij_cimod-1.5.0/cimod/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cimod/__init__.py` & `jij_cimod-1.5.0/cimod/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from pkgutil import extend_path
 
 __path__ = extend_path(__path__, __name__)
 
+from cimod import cxxcimod
+
 from cimod.model.binary_polynomial_model import (
     BinaryPolynomialModel,
     make_BinaryPolynomialModel,
     make_BinaryPolynomialModel_from_JSON,
 )
 from cimod.model.binary_quadratic_model import (
     BinaryQuadraticModel,
     make_BinaryQuadraticModel,
     make_BinaryQuadraticModel_from_JSON,
 )
 from cimod.vartype import BINARY, SPIN, Vartype
 
 __all__ = [
-    "SPIN",
-    "BINARY",
-    "Vartype",
-    "make_BinaryQuadraticModel",
-    "make_BinaryQuadraticModel_from_JSON",
-    "BinaryQuadraticModel",
-    "make_BinaryPolynomialModel",
-    "make_BinaryPolynomialModel_from_JSON",
-    "BinaryPolynomialModel",
+        "cxxcimod",
+        "SPIN",
+        "BINARY",
+        "Vartype",
+        "make_BinaryQuadraticModel",
+        "make_BinaryQuadraticModel_from_JSON",
+        "BinaryQuadraticModel",
+        "make_BinaryPolynomialModel",
+        "make_BinaryPolynomialModel_from_JSON",
+        "BinaryPolynomialModel",
 ]
```

### Comparing `jij_cimod-1.4.9/cimod/main.cpp` & `jij_cimod-1.5.0/cimod/main.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 
 //    Licensed under the Apache License, Version 2.0 (the "License");
 //    you may not use this file except in compliance with the License.
 //    You may obtain a copy of the License at
 
 //        http://www.apache.org/licenses/LICENSE-2.0
 
-//    Unless required by applicable law or agreed to in writing, software 
-//    distributed under the License is distributed on an "AS IS" BASIS, 
+//    Unless required by applicable law or agreed to in writing, software
+//    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 #include "main.hpp"
+
 #include <string>
 
 namespace py = pybind11;
 
 using namespace py::literals;
 using namespace cimod;
 
-PYBIND11_MODULE(cxxcimod, m){
-    m.doc() = "C++ library for a binary quadratic model";
+PYBIND11_MODULE( cxxcimod, m ) {
+  m.doc() = "C++ library for a binary quadratic model";
 
-    /**********************************************************
-    //BinaryQuadraticModel and BinaryPolynomialModel
-     **********************************************************/
-
-    py::enum_<Vartype>(m, "Vartype")
-        .value("SPIN", Vartype::SPIN)
-        .value("BINARY", Vartype::BINARY)
-        .value("NONE", Vartype::NONE)
-        .export_values();
-
-    declare_BQM<int64_t, double, cimod::Dense>(m, "BinaryQuadraticModel_Dense");
-    declare_BQM<std::string, double, cimod::Dense>(m, "BinaryQuadraticModel_str_Dense");
-    declare_BQM<std::tuple<size_t, size_t>, double, cimod::Dense>(m, "BinaryQuadraticModel_tuple2_Dense");
-    declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Dense>(m, "BinaryQuadraticModel_tuple3_Dense");
-    declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Dense>(m, "BinaryQuadraticModel_tuple4_Dense");
-
-    declare_BQM<int64_t, double, cimod::Sparse>(m, "BinaryQuadraticModel_Sparse");
-    declare_BQM<std::string, double, cimod::Sparse>(m, "BinaryQuadraticModel_str_Sparse");
-    declare_BQM<std::tuple<size_t, size_t>, double, cimod::Sparse>(m, "BinaryQuadraticModel_tuple2_Sparse");
-    declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Sparse>(m, "BinaryQuadraticModel_tuple3_Sparse");
-    declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Sparse>(m, "BinaryQuadraticModel_tuple4_Sparse");
-
-    declare_BQM<int64_t, double, cimod::Dict>(m, "BinaryQuadraticModel_Dict");
-    declare_BQM<std::string, double, cimod::Dict>(m, "BinaryQuadraticModel_str_Dict");
-    declare_BQM<std::tuple<size_t, size_t>, double, cimod::Dict>(m, "BinaryQuadraticModel_tuple2_Dict");
-    declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Dict>(m, "BinaryQuadraticModel_tuple3_Dict");
-    declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Dict>(m, "BinaryQuadraticModel_tuple4_Dict");
-
-    declare_BPM<int64_t, double>(m, "BinaryPolynomialModel");
-    declare_BPM<std::string, double>(m, "BinaryPolynomialModel_str");
-    declare_BPM<std::tuple<int64_t, int64_t>, double>(m, "BinaryPolynomialModel_tuple2");
-    declare_BPM<std::tuple<int64_t, int64_t, int64_t>, double>(m, "BinaryPolynomialModel_tuple3");
-    declare_BPM<std::tuple<int64_t, int64_t, int64_t, int64_t>, double>(m, "BinaryPolynomialModel_tuple4");
-   
+  /**********************************************************
+  //BinaryQuadraticModel and BinaryPolynomialModel
+   **********************************************************/
+
+  py::enum_<Vartype>( m, "Vartype" )
+      .value( "SPIN", Vartype::SPIN )
+      .value( "BINARY", Vartype::BINARY )
+      .value( "NONE", Vartype::NONE )
+      .export_values();
+
+  declare_BQM<int64_t, double, cimod::Dense>( m, "BinaryQuadraticModel_Dense" );
+  declare_BQM<std::string, double, cimod::Dense>( m, "BinaryQuadraticModel_str_Dense" );
+  declare_BQM<std::tuple<size_t, size_t>, double, cimod::Dense>( m, "BinaryQuadraticModel_tuple2_Dense" );
+  declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Dense>( m, "BinaryQuadraticModel_tuple3_Dense" );
+  declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Dense>( m, "BinaryQuadraticModel_tuple4_Dense" );
+
+  declare_BQM<int64_t, double, cimod::Sparse>( m, "BinaryQuadraticModel_Sparse" );
+  declare_BQM<std::string, double, cimod::Sparse>( m, "BinaryQuadraticModel_str_Sparse" );
+  declare_BQM<std::tuple<size_t, size_t>, double, cimod::Sparse>( m, "BinaryQuadraticModel_tuple2_Sparse" );
+  declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Sparse>( m, "BinaryQuadraticModel_tuple3_Sparse" );
+  declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Sparse>( m, "BinaryQuadraticModel_tuple4_Sparse" );
+
+  declare_BQM<int64_t, double, cimod::Dict>( m, "BinaryQuadraticModel_Dict" );
+  declare_BQM<std::string, double, cimod::Dict>( m, "BinaryQuadraticModel_str_Dict" );
+  declare_BQM<std::tuple<size_t, size_t>, double, cimod::Dict>( m, "BinaryQuadraticModel_tuple2_Dict" );
+  declare_BQM<std::tuple<size_t, size_t, size_t>, double, cimod::Dict>( m, "BinaryQuadraticModel_tuple3_Dict" );
+  declare_BQM<std::tuple<size_t, size_t, size_t, size_t>, double, cimod::Dict>( m, "BinaryQuadraticModel_tuple4_Dict" );
+
+  declare_BPM<int64_t, double>( m, "BinaryPolynomialModel" );
+  declare_BPM<std::string, double>( m, "BinaryPolynomialModel_str" );
+  declare_BPM<std::tuple<int64_t, int64_t>, double>( m, "BinaryPolynomialModel_tuple2" );
+  declare_BPM<std::tuple<int64_t, int64_t, int64_t>, double>( m, "BinaryPolynomialModel_tuple3" );
+  declare_BPM<std::tuple<int64_t, int64_t, int64_t, int64_t>, double>( m, "BinaryPolynomialModel_tuple4" );
 }
```

### Comparing `jij_cimod-1.4.9/cimod/main.hpp` & `jij_cimod-1.5.0/cimod/main.hpp`

 * *Files 26% similar despite different names*

```diff
@@ -2,218 +2,327 @@
 
 //    Licensed under the Apache License, Version 2.0 (the "License");
 //    you may not use this file except in compliance with the License.
 //    You may obtain a copy of the License at
 
 //        http://www.apache.org/licenses/LICENSE-2.0
 
-//    Unless required by applicable law or agreed to in writing, software 
-//    distributed under the License is distributed on an "AS IS" BASIS, 
+//    Unless required by applicable law or agreed to in writing, software
+//    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 //
 
 #pragma once
 
-#include <disable_eigen_warning.hpp>
 
-#include <pybind11_json/pybind11_json.hpp>
-#include <nlohmann/json.hpp>
+#include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 #include <pybind11/functional.h>
 #include <pybind11/eigen.h>
-#include <pybind11/pybind11.h>
 
-#include <binary_quadratic_model.hpp>
-#include <binary_quadratic_model_dict.hpp>
-#include <binary_polynomial_model.hpp>
+#include <pybind11_json/pybind11_json.hpp>
+
+#include <nlohmann/json.hpp>
 
 #include <sstream>
 
+#include <cimod/binary_polynomial_model.hpp>
+#include <cimod/binary_quadratic_model.hpp>
+#include <cimod/binary_quadratic_model_dict.hpp>
+#include <cimod/disable_eigen_warning.hpp>
+
 namespace py = pybind11;
 
 using namespace py::literals;
 using namespace cimod;
 
 template<typename IndexType, typename FloatType, typename DataType>
-inline void declare_BQM(py::module& m, const std::string& name){
-
-    using BQM = BinaryQuadraticModel<IndexType, FloatType, DataType>;
+inline void declare_BQM( py::module& m, const std::string& name ) {
 
-    using DenseMatrix = Eigen::Matrix<FloatType, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>;
+  using BQM = BinaryQuadraticModel<IndexType, FloatType, DataType>;
 
-    auto pyclass_BQM = py::class_<BQM>(m, name.c_str());
+  using DenseMatrix = Eigen::Matrix<FloatType, Eigen::Dynamic, Eigen::Dynamic, Eigen::RowMajor>;
+  using SparseMatrix = Eigen::SparseMatrix<FloatType, Eigen::RowMajor>;
 
-    pyclass_BQM
-        .def(py::init<Linear<IndexType, FloatType>, Quadratic<IndexType, FloatType>, FloatType, Vartype>(), "linear"_a, "quadratic"_a, "offset"_a, "vartype"_a)
-        .def(py::init<Linear<IndexType, FloatType>, Quadratic<IndexType, FloatType>, Vartype>(), "linear"_a, "quadratic"_a, "vartype"_a)
-        .def(py::init<Eigen::Ref<const DenseMatrix>, std::vector<IndexType>, FloatType, Vartype, bool>(), "mat"_a, "labels_vec"_a, "offset"_a, "vartype"_a, "fix_format"_a=true)
-        .def(py::init<Eigen::Ref<const DenseMatrix>, std::vector<IndexType>, Vartype, bool>(), "mat"_a, "labels_vec"_a, "vartype"_a, "fix_format"_a=false)
-        .def(py::init<const BQM&>(), "bqm"_a)
-        .def("length", &BQM::length)
-        .def("get_num_variables", &BQM::get_num_variables)
-        .def("get_linear", py::overload_cast<IndexType>(&BQM::get_linear, py::const_))
-        .def("get_linear", py::overload_cast<>(&BQM::get_linear, py::const_))
-        .def("get_quadratic", py::overload_cast<IndexType ,IndexType>(&BQM::get_quadratic, py::const_))
-        .def("get_quadratic", py::overload_cast<>(&BQM::get_quadratic, py::const_))
-        .def("get_offset", &BQM::get_offset)
-        .def("get_vartype", &BQM::get_vartype)
-        .def("get_variables", &BQM::get_variables)
-        //.def("print", &BQM::print)
-        .def("empty", &BQM::empty, "vartype"_a)
-        .def("add_variable", &BQM::add_variable, "v"_a, "bias"_a)
-        .def("add_variables_from", &BQM::add_variables_from, "linear"_a)
-        .def("add_interaction", &BQM::add_interaction, "u"_a, "v"_a, "bias"_a)
-        .def("add_interactions_from", &BQM::add_interactions_from, "quadratic"_a)
-        .def("remove_variable", &BQM::remove_variable, "v"_a)
-        .def("remove_variables_from", &BQM::remove_variables_from, "variables"_a)
-        .def("remove_interaction", &BQM::remove_interaction, "u"_a, "v"_a)
-        .def("remove_interactions_from", &BQM::remove_interactions_from, "interactions"_a)
-        .def("add_offset", &BQM::add_offset, "offset"_a)
-        .def("remove_offset", &BQM::remove_offset)
-        .def("scale", &BQM::scale, "scalar"_a, "ignored_variables"_a=std::vector<IndexType>(), "ignored_interactions"_a=std::vector<std::pair<IndexType, IndexType>>(), "ignored_offset"_a=false)
-        .def("normalize", &BQM::normalize, "bias_range"_a=std::pair<FloatType, FloatType>(1.0, 1.0), "use_quadratic_range"_a=false, "quadratic_range"_a=std::pair<FloatType, FloatType>(1.0, 1.0), "ignored_variables"_a=std::vector<IndexType>(), "ignored_interactions"_a=std::vector<std::pair<IndexType, IndexType>>(), "ignored_offset"_a=false)
-        .def("fix_variable", &BQM::fix_variable, "v"_a, "value"_a)
-        .def("fix_variables", &BQM::fix_variables, "fixed"_a)
-        .def("flip_variable", &BQM::flip_variable, "v"_a)
-        //.def("contract_variables", &BQM::contract_variables, "u"_a, "v"_a)
-        .def("change_vartype", py::overload_cast<const Vartype&>(&BQM::change_vartype), "vartype"_a)
-        .def("change_vartype", py::overload_cast<const Vartype&, bool>(&BQM::change_vartype), "vartype"_a, "inplace"_a)
-        .def("energy", &BQM::energy, "sample"_a)
-        .def("energies", &BQM::energies, "samples_like"_a)
-        .def("to_qubo", &BQM::to_qubo)
-        .def("to_ising", &BQM::to_ising)
-        .def_static("from_qubo", &BQM::from_qubo, "Q"_a, "offset"_a=0.0)
-        .def_static("from_ising", &BQM::from_ising, "h"_a, "J"_a, "offset"_a=0.0)
-        .def("interaction_matrix", py::overload_cast<>(&BQM::interaction_matrix, py::const_))
-        //.def("to_serialiable", &BQM::to_serializable)
-        //.def_static("from_serialiable", &BQM::from_serializable, "input"_a);
-        .def("to_serializable", [](const BQM& self){return static_cast<py::object>(self.to_serializable());})
-        .def_static("from_serializable", [](const py::object& input){return BQM::from_serializable(static_cast<nlohmann::json>(input));}, "input"_a);
-
-    //interaction_matrix for Dict (legacy BQM) class
-    if constexpr (std::is_same_v<DataType, cimod::Dict>)
-        pyclass_BQM
-            .def("_generate_indices", &BQM::_generate_indices)
-            .def("interaction_matrix", py::overload_cast<const std::vector<IndexType>&>(&BQM::interaction_matrix, py::const_));
-            
+  auto pyclass_BQM = py::class_<BQM>( m, name.c_str() );
 
+  pyclass_BQM
+      .def(
+          py::init<Linear<IndexType, FloatType>, Quadratic<IndexType, FloatType>, FloatType, Vartype>(),
+          "linear"_a,
+          "quadratic"_a,
+          "offset"_a,
+          "vartype"_a )
+      .def(
+          py::init<Linear<IndexType, FloatType>, Quadratic<IndexType, FloatType>, Vartype>(),
+          "linear"_a,
+          "quadratic"_a,
+          "vartype"_a )
+      .def(
+          py::init<Eigen::Ref<const DenseMatrix>, std::vector<IndexType>, FloatType, Vartype, bool>(),
+          "mat"_a,
+          "labels_vec"_a,
+          "offset"_a,
+          "vartype"_a,
+          "fix_format"_a = true )
+      .def(
+          py::init<Eigen::Ref<const DenseMatrix>, std::vector<IndexType>, Vartype, bool>(),
+          "mat"_a,
+          "labels_vec"_a,
+          "vartype"_a,
+          "fix_format"_a = true )
+      .def(
+          py::init<const SparseMatrix&, std::vector<IndexType>, FloatType, Vartype>(),
+          "mat"_a,
+          "labels_vec"_a,
+          "offset"_a,
+          "vartype"_a)
+      .def(
+          py::init<const SparseMatrix&, std::vector<IndexType>, Vartype>(),
+          "mat"_a,
+          "labels_vec"_a,
+          "vartype"_a)
+      .def( py::init<const BQM&>(), "bqm"_a )
+      .def( "length", &BQM::length )
+      .def( "get_num_variables", &BQM::get_num_variables )
+      .def( "get_linear", py::overload_cast<IndexType>( &BQM::get_linear, py::const_ ) )
+      .def( "get_linear", py::overload_cast<>( &BQM::get_linear, py::const_ ) )
+      .def( "get_quadratic", py::overload_cast<IndexType, IndexType>( &BQM::get_quadratic, py::const_ ) )
+      .def( "get_quadratic", py::overload_cast<>( &BQM::get_quadratic, py::const_ ) )
+      .def( "get_offset", &BQM::get_offset )
+      .def( "get_vartype", &BQM::get_vartype )
+      .def( "get_variables", &BQM::get_variables )
+      //.def("print", &BQM::print)
+      .def( "empty", &BQM::empty, "vartype"_a )
+      .def( "add_variable", &BQM::add_variable, "v"_a, "bias"_a )
+      .def( "add_variables_from", &BQM::add_variables_from, "linear"_a )
+      .def( "add_interaction", &BQM::add_interaction, "u"_a, "v"_a, "bias"_a )
+      .def( "add_interactions_from", &BQM::add_interactions_from, "quadratic"_a )
+      .def( "remove_variable", &BQM::remove_variable, "v"_a )
+      .def( "remove_variables_from", &BQM::remove_variables_from, "variables"_a )
+      .def( "remove_interaction", &BQM::remove_interaction, "u"_a, "v"_a )
+      .def( "remove_interactions_from", &BQM::remove_interactions_from, "interactions"_a )
+      .def( "add_offset", &BQM::add_offset, "offset"_a )
+      .def( "remove_offset", &BQM::remove_offset )
+      .def(
+          "scale",
+          &BQM::scale,
+          "scalar"_a,
+          "ignored_variables"_a = std::vector<IndexType>(),
+          "ignored_interactions"_a = std::vector<std::pair<IndexType, IndexType>>(),
+          "ignored_offset"_a = false )
+      .def(
+          "normalize",
+          &BQM::normalize,
+          "bias_range"_a = std::pair<FloatType, FloatType>( 1.0, 1.0 ),
+          "use_quadratic_range"_a = false,
+          "quadratic_range"_a = std::pair<FloatType, FloatType>( 1.0, 1.0 ),
+          "ignored_variables"_a = std::vector<IndexType>(),
+          "ignored_interactions"_a = std::vector<std::pair<IndexType, IndexType>>(),
+          "ignored_offset"_a = false )
+      .def( "fix_variable", &BQM::fix_variable, "v"_a, "value"_a )
+      .def( "fix_variables", &BQM::fix_variables, "fixed"_a )
+      .def( "flip_variable", &BQM::flip_variable, "v"_a )
+      //.def("contract_variables", &BQM::contract_variables, "u"_a, "v"_a)
+      .def( "change_vartype", py::overload_cast<const Vartype&>( &BQM::change_vartype ), "vartype"_a )
+      .def( "change_vartype", py::overload_cast<const Vartype&, bool>( &BQM::change_vartype ), "vartype"_a, "inplace"_a )
+      .def( "energy", &BQM::energy, "sample"_a )
+      .def( "energies", &BQM::energies, "samples_like"_a )
+      .def( "to_qubo", &BQM::to_qubo )
+      .def( "to_ising", &BQM::to_ising )
+      .def_static( "from_qubo", &BQM::from_qubo, "Q"_a, "offset"_a = 0.0 )
+      .def_static( "from_ising", &BQM::from_ising, "h"_a, "J"_a, "offset"_a = 0.0 )
+      .def( "interaction_matrix", py::overload_cast<>( &BQM::interaction_matrix, py::const_ ) )
+      //.def("to_serialiable", &BQM::to_serializable)
+      //.def_static("from_serialiable", &BQM::from_serializable, "input"_a);
+      .def( "to_serializable", []( const BQM& self ) { return static_cast<py::object>( self.to_serializable() ); } )
+      .def_static(
+          "from_serializable",
+          []( const py::object& input ) { return BQM::from_serializable( static_cast<nlohmann::json>( input ) ); },
+          "input"_a );
+
+  // interaction_matrix for Dict (legacy BQM) class
+  if constexpr ( std::is_same_v<DataType, cimod::Dict> )
+    pyclass_BQM.def( "_generate_indices", &BQM::_generate_indices )
+        .def(
+            "interaction_matrix", py::overload_cast<const std::vector<IndexType>&>( &BQM::interaction_matrix, py::const_ ) );
 }
 
-
 template<typename IndexType, typename FloatType>
-inline void declare_BPM(py::module& m, const std::string& name){
-   
-   using BPM = BinaryPolynomialModel<IndexType, FloatType>;
-   
-   py::class_<BPM>(m, name.c_str())
-   .def(py::init<Polynomial<IndexType, FloatType>&, const Vartype>(), "polynomial"_a, "vartype"_a)
-   .def(py::init<PolynomialKeyList<IndexType>&, PolynomialValueList<FloatType>&, const Vartype>(), "keys"_a, "values"_a, "vartype"_a)
-   .def(py::init<const std::vector<IndexType>&, const PolynomialKeyList<std::size_t>&, const PolynomialValueList<FloatType>&, const Vartype>(),
-        "variables"_a, "keys_distance"_a, "values"_a, "vartype"_a)
-   .def("get_polynomial"          , [](const BPM& self) {
-      py::dict py_polynomial;
-      const auto &poly_key_list   = self.GetKeyList();
-      const auto &poly_value_list = self.GetValueList();
-      for (std::size_t i = 0; i < poly_key_list.size(); ++i) {
-         py::tuple tuple;
-         for (const auto &index: poly_key_list[i]) {
-            tuple = tuple + py::make_tuple(index);
-         }
-         py_polynomial[tuple] = poly_value_list[i];
-      }
-      return py_polynomial;
-   })
-   .def("get_polynomial"           , py::overload_cast<std::vector<IndexType>&>(&BPM::GetPolynomial, py::const_), "key"_a)
-   .def("get_variables_to_integers",py::overload_cast<>(&BPM::GetVariablesToIntegers))
-   .def("get_variables_to_integers",py::overload_cast<const IndexType&>(&BPM::GetVariablesToIntegers), "v"_a)
-   .def("get_key_list"            , &BPM::GetKeyList)
-   .def("get_value_list"          , &BPM::GetValueList)
-   .def("get_variables"           , py::overload_cast<>(&BPM::GetSortedVariables))
-   .def("indices"                 , py::overload_cast<>(&BPM::GetSortedVariables))//This will be depricated
-   .def("get_degree"              , &BPM::GetDegree)
-   .def("get_offset"              , &BPM::GetOffset)
-   .def("get_vartype"             , &BPM::GetVartype)
-   .def("get_num_interactions"    , &BPM::GetNumInteractions)
-   .def("get_num_variables"       , &BPM::GetNumVariables)
-   .def("empty"                   , &BPM::Empty, "vartype"_a)
-   .def("clear"                   , &BPM::Clear)
-   .def("remove_interaction"      , py::overload_cast<std::vector<IndexType>&>(&BPM::RemoveInteraction), "key"_a)
-   .def("remove_interactions_from", py::overload_cast<PolynomialKeyList<IndexType>&>(&BPM::RemoveInteractionsFrom), "keys"_a)
-   .def("remove_offset"           , &BPM::RemoveOffset)
-   .def("remove_variable"         , &BPM::RemoveVariable, "v"_a)
-   .def("remove_variables_from"   , &BPM::RemoveVariablesFrom, "variables"_a)
-   .def("add_interaction"         , py::overload_cast<std::vector<IndexType>&, const FloatType&, const Vartype>(&BPM::AddInteraction), "key"_a, "value"_a, "vartype"_a = Vartype::NONE)
-   .def("add_interactions_from"   , py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&, const Vartype>(&BPM::AddInteractionsFrom), "keys"_a, "values"_a, "vartype"_a = Vartype::NONE)
-   .def("add_interactions_from"   , py::overload_cast<const Polynomial<IndexType, FloatType>&, const Vartype>(&BPM::AddInteractionsFrom), "polynomial"_a, "vartype"_a = Vartype::NONE)
-   .def("add_offset"              , &BPM::AddOffset, "offset"_a)
-   .def("energy"                  , py::overload_cast<const Sample<IndexType>&, bool>(&BPM::Energy, py::const_), "sample"_a, "omp_flag"_a = true)
-   .def("energy"                  , py::overload_cast<const std::vector<int32_t>&, bool>(&BPM::Energy), "sample"_a, "omp_flag"_a = true)
-   .def("energies"                , py::overload_cast<const std::vector<Sample<IndexType>>&>(&BPM::Energies, py::const_), "samples"_a)
-   .def("energies"                , py::overload_cast<const std::vector<std::vector<int32_t>>&>(&BPM::Energies), "samples"_a)
-   .def("scale"                   , &BPM::Scale, "scalar"_a, "ignored_interactions"_a = PolynomialKeyList<IndexType>{}, "ignored_offset"_a = false)
-   .def("normalize"               , &BPM::normalize, "range"_a = std::pair<FloatType, FloatType>{1.0, 1.0}, "ignored_interactions"_a = PolynomialKeyList<IndexType>{}, "ignored_offset"_a = false)
-   .def("change_vartype"          , py::overload_cast<const Vartype, const bool>(&BPM::ChangeVartype), "vartype"_a, "inplace"_a)
-   .def("change_vartype"          , py::overload_cast<const Vartype>(&BPM::ChangeVartype), "vartype"_a)
-   .def("has_variable"            , &BPM::HasVariable, "v"_a)
-   .def("to_hubo"                 , [](const BPM& self){
-      py::dict py_polynomial;
-      for (const auto &it: self.ToHubo()) {
-         py::tuple tuple;
-         for (const auto &index: it.first) {
-            tuple = tuple + py::make_tuple(index);
-         }
-         py_polynomial[tuple] = it.second;
-      }
-      return py_polynomial;
-   })
-   .def("to_hising"               , [](const BPM& self) {
-      py::dict py_polynomial;
-      for (const auto &it: self.ToHising()) {
-         py::tuple tuple;
-         for (const auto &index: it.first) {
-            tuple = tuple + py::make_tuple(index);
-         }
-         py_polynomial[tuple] = it.second;
-      }
-      return py_polynomial;
-   })
-   .def("to_serializable"         , [](const BPM& self){return static_cast<py::object>(self.ToSerializable());})
-   .def_static("from_serializable", [](const py::object& input){return BPM::FromSerializable(static_cast<nlohmann::json>(input));}, "input"_a)
-   .def_static("from_hubo"        , py::overload_cast<const Polynomial<IndexType, FloatType>&>(&BPM::FromHubo), "polynomial"_a)
-   .def_static("from_hubo"        , py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&>(&BPM::FromHubo), "keys"_a, "value"_a)
-   .def_static("from_hising"      , py::overload_cast<const Polynomial<IndexType, FloatType>&>(&BPM::FromHising), "polynomial"_a)
-   .def_static("from_hising"      , py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&>(&BPM::FromHising), "keys"_a, "value"_a)
-   .def("__repr__", [](const BPM& self) {
-      const auto &poly_key_list   = self.GetKeyList();
-      const auto &poly_value_list = self.GetValueList();
-      std::ostringstream out;
-      out << "cxxcimod.BinaryPolynomialModel({";
-      for (std::size_t i = 0; i < poly_key_list.size(); ++i) {
-         py::tuple tuple;
-         for (const auto &it: poly_key_list[i]) {
-            tuple = tuple + py::make_tuple(it);
-         }
-         out << tuple.attr("__repr__")();
-         if (i == poly_key_list.size() - 1) {
-            out << ": " << poly_value_list[i];
-         }
-         else {
-            out << ": " << poly_value_list[i] << ", ";
-         }
-      }
-      out << "}, ";
-      if (self.GetVartype() == Vartype::SPIN) {
-         out << "Vartype.SPIN" << ")";
-      }
-      else if (self.GetVartype() == Vartype::BINARY){
-         out << "Vartype.BINARY" << ")";
-      }
-      else {
-         out << "Vartype.NONE" << ")";
-      }
-      return out.str();
-   });
-   
-   
+inline void declare_BPM( py::module& m, const std::string& name ) {
+
+  using BPM = BinaryPolynomialModel<IndexType, FloatType>;
+
+  py::class_<BPM>( m, name.c_str() )
+      .def( py::init<Polynomial<IndexType, FloatType>&, const Vartype>(), "polynomial"_a, "vartype"_a )
+      .def(
+          py::init<PolynomialKeyList<IndexType>&, PolynomialValueList<FloatType>&, const Vartype>(),
+          "keys"_a,
+          "values"_a,
+          "vartype"_a )
+      .def(
+          py::init<
+              const std::vector<IndexType>&,
+              const PolynomialKeyList<std::size_t>&,
+              const PolynomialValueList<FloatType>&,
+              const Vartype>(),
+          "variables"_a,
+          "keys_distance"_a,
+          "values"_a,
+          "vartype"_a )
+      .def(
+          "get_polynomial",
+          []( const BPM& self ) {
+            py::dict py_polynomial;
+            const auto& poly_key_list = self.GetKeyList();
+            const auto& poly_value_list = self.GetValueList();
+            for ( std::size_t i = 0; i < poly_key_list.size(); ++i ) {
+              py::tuple tuple;
+              for ( const auto& index : poly_key_list[ i ] ) {
+                tuple = tuple + py::make_tuple( index );
+              }
+              py_polynomial[ tuple ] = poly_value_list[ i ];
+            }
+            return py_polynomial;
+          } )
+      .def( "get_polynomial", py::overload_cast<std::vector<IndexType>&>( &BPM::GetPolynomial, py::const_ ), "key"_a )
+      .def( "get_variables_to_integers", py::overload_cast<>( &BPM::GetVariablesToIntegers ) )
+      .def( "get_variables_to_integers", py::overload_cast<const IndexType&>( &BPM::GetVariablesToIntegers ), "v"_a )
+      .def( "get_key_list", &BPM::GetKeyList )
+      .def( "get_value_list", &BPM::GetValueList )
+      .def( "get_variables", py::overload_cast<>( &BPM::GetSortedVariables ) )
+      .def( "indices", py::overload_cast<>( &BPM::GetSortedVariables ) ) // This will be depricated
+      .def( "get_degree", &BPM::GetDegree )
+      .def( "get_offset", &BPM::GetOffset )
+      .def( "get_vartype", &BPM::GetVartype )
+      .def( "get_num_interactions", &BPM::GetNumInteractions )
+      .def( "get_num_variables", &BPM::GetNumVariables )
+      .def( "empty", &BPM::Empty, "vartype"_a )
+      .def( "clear", &BPM::Clear )
+      .def( "remove_interaction", py::overload_cast<std::vector<IndexType>&>( &BPM::RemoveInteraction ), "key"_a )
+      .def(
+          "remove_interactions_from",
+          py::overload_cast<PolynomialKeyList<IndexType>&>( &BPM::RemoveInteractionsFrom ),
+          "keys"_a )
+      .def( "remove_offset", &BPM::RemoveOffset )
+      .def( "remove_variable", &BPM::RemoveVariable, "v"_a )
+      .def( "remove_variables_from", &BPM::RemoveVariablesFrom, "variables"_a )
+      .def(
+          "add_interaction",
+          py::overload_cast<std::vector<IndexType>&, const FloatType&, const Vartype>( &BPM::AddInteraction ),
+          "key"_a,
+          "value"_a,
+          "vartype"_a = Vartype::NONE )
+      .def(
+          "add_interactions_from",
+          py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&, const Vartype>(
+              &BPM::AddInteractionsFrom ),
+          "keys"_a,
+          "values"_a,
+          "vartype"_a = Vartype::NONE )
+      .def(
+          "add_interactions_from",
+          py::overload_cast<const Polynomial<IndexType, FloatType>&, const Vartype>( &BPM::AddInteractionsFrom ),
+          "polynomial"_a,
+          "vartype"_a = Vartype::NONE )
+      .def( "add_offset", &BPM::AddOffset, "offset"_a )
+      .def(
+          "energy",
+          py::overload_cast<const Sample<IndexType>&, bool>( &BPM::Energy, py::const_ ),
+          "sample"_a,
+          "omp_flag"_a = true )
+      .def( "energy", py::overload_cast<const std::vector<int32_t>&, bool>( &BPM::Energy ), "sample"_a, "omp_flag"_a = true )
+      .def( "energies", py::overload_cast<const std::vector<Sample<IndexType>>&>( &BPM::Energies, py::const_ ), "samples"_a )
+      .def( "energies", py::overload_cast<const std::vector<std::vector<int32_t>>&>( &BPM::Energies ), "samples"_a )
+      .def(
+          "scale",
+          &BPM::Scale,
+          "scalar"_a,
+          "ignored_interactions"_a = PolynomialKeyList<IndexType>{},
+          "ignored_offset"_a = false )
+      .def(
+          "normalize",
+          &BPM::normalize,
+          "range"_a = std::pair<FloatType, FloatType>{ 1.0, 1.0 },
+          "ignored_interactions"_a = PolynomialKeyList<IndexType>{},
+          "ignored_offset"_a = false )
+      .def( "change_vartype", py::overload_cast<const Vartype, const bool>( &BPM::ChangeVartype ), "vartype"_a, "inplace"_a )
+      .def( "change_vartype", py::overload_cast<const Vartype>( &BPM::ChangeVartype ), "vartype"_a )
+      .def( "has_variable", &BPM::HasVariable, "v"_a )
+      .def(
+          "to_hubo",
+          []( const BPM& self ) {
+            py::dict py_polynomial;
+            for ( const auto& it : self.ToHubo() ) {
+              py::tuple tuple;
+              for ( const auto& index : it.first ) {
+                tuple = tuple + py::make_tuple( index );
+              }
+              py_polynomial[ tuple ] = it.second;
+            }
+            return py_polynomial;
+          } )
+      .def(
+          "to_hising",
+          []( const BPM& self ) {
+            py::dict py_polynomial;
+            for ( const auto& it : self.ToHising() ) {
+              py::tuple tuple;
+              for ( const auto& index : it.first ) {
+                tuple = tuple + py::make_tuple( index );
+              }
+              py_polynomial[ tuple ] = it.second;
+            }
+            return py_polynomial;
+          } )
+      .def( "to_serializable", []( const BPM& self ) { return static_cast<py::object>( self.ToSerializable() ); } )
+      .def_static(
+          "from_serializable",
+          []( const py::object& input ) { return BPM::FromSerializable( static_cast<nlohmann::json>( input ) ); },
+          "input"_a )
+      .def_static(
+          "from_hubo", py::overload_cast<const Polynomial<IndexType, FloatType>&>( &BPM::FromHubo ), "polynomial"_a )
+      .def_static(
+          "from_hubo",
+          py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&>( &BPM::FromHubo ),
+          "keys"_a,
+          "value"_a )
+      .def_static(
+          "from_hising", py::overload_cast<const Polynomial<IndexType, FloatType>&>( &BPM::FromHising ), "polynomial"_a )
+      .def_static(
+          "from_hising",
+          py::overload_cast<PolynomialKeyList<IndexType>&, const PolynomialValueList<FloatType>&>( &BPM::FromHising ),
+          "keys"_a,
+          "value"_a )
+      .def( "__repr__", []( const BPM& self ) {
+        const auto& poly_key_list = self.GetKeyList();
+        const auto& poly_value_list = self.GetValueList();
+        std::ostringstream out;
+        out << "cxxcimod.BinaryPolynomialModel({";
+        for ( std::size_t i = 0; i < poly_key_list.size(); ++i ) {
+          py::tuple tuple;
+          for ( const auto& it : poly_key_list[ i ] ) {
+            tuple = tuple + py::make_tuple( it );
+          }
+          out << tuple.attr( "__repr__" )();
+          if ( i == poly_key_list.size() - 1 ) {
+            out << ": " << poly_value_list[ i ];
+          } else {
+            out << ": " << poly_value_list[ i ] << ", ";
+          }
+        }
+        out << "}, ";
+        if ( self.GetVartype() == Vartype::SPIN ) {
+          out << "Vartype.SPIN"
+              << ")";
+        } else if ( self.GetVartype() == Vartype::BINARY ) {
+          out << "Vartype.BINARY"
+              << ")";
+        } else {
+          out << "Vartype.NONE"
+              << ")";
+        }
+        return out.str();
+      } );
 }
```

### Comparing `jij_cimod-1.4.9/cimod/model/__init__.py` & `jij_cimod-1.5.0/cimod/model/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cimod/model/binary_polynomial_model.py` & `jij_cimod-1.5.0/cimod/model/binary_polynomial_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 from __future__ import annotations
 
 import cimod.cxxcimod as cxxcimod
 import dimod
 
 from cimod.vartype import to_cxxcimod
 
-__all__ = []
-
 
 class Polynomial:
     def __init__(self, bpm):
         self.__bpm = bpm
 
     def items(self, *args, **kwargs):
         return self.__bpm.get_polynomial().items(*args, **kwargs)
```

### Comparing `jij_cimod-1.4.9/cimod/model/binary_quadratic_model.py` & `jij_cimod-1.5.0/cimod/model/binary_quadratic_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,67 +18,69 @@
 
 import cimod
 import cimod.cxxcimod as cxxcimod
 import dimod
 import numpy as np
 
 from cimod.vartype import to_cxxcimod
+from scipy.sparse import dok_matrix, csr_matrix
 
-__all__ = []
+from typing import Tuple, Union
+from collections import defaultdict
 
 
 def get_cxxcimod_class(linear, quadratic, sparse):
     # select base class
     index = set()
     base = None
 
     if linear != {}:
         index.add(next(iter(linear)))
     if quadratic != {}:
         index.add(next(iter(quadratic))[0])
         index.add(next(iter(quadratic))[1])
 
     if len(set(type(i) for i in index)) != 1:
-        raise TypeError("invalid types of linear and quadratic")
+        # assume that index type is int
+        ind = int(0)
     else:
-
         ind = next(iter(index))
 
-        if sparse:
-            if isinstance(ind, int):
-                base = cxxcimod.BinaryQuadraticModel_Sparse
-            elif isinstance(ind, str):
-                base = cxxcimod.BinaryQuadraticModel_str_Sparse
-            elif isinstance(ind, tuple):
-                if len(ind) == 2:
-                    base = cxxcimod.BinaryQuadraticModel_tuple2_Sparse
-                elif len(ind) == 3:
-                    base = cxxcimod.BinaryQuadraticModel_tuple3_Sparse
-                elif len(ind) == 4:
-                    base = cxxcimod.BinaryQuadraticModel_tuple4_Sparse
-                else:
-                    raise TypeError("invalid length of tuple")
+    if sparse:
+        if isinstance(ind, int):
+            base = cxxcimod.BinaryQuadraticModel_Sparse
+        elif isinstance(ind, str):
+            base = cxxcimod.BinaryQuadraticModel_str_Sparse
+        elif isinstance(ind, tuple):
+            if len(ind) == 2:
+                base = cxxcimod.BinaryQuadraticModel_tuple2_Sparse
+            elif len(ind) == 3:
+                base = cxxcimod.BinaryQuadraticModel_tuple3_Sparse
+            elif len(ind) == 4:
+                base = cxxcimod.BinaryQuadraticModel_tuple4_Sparse
             else:
-                raise TypeError("invalid types of linear and quadratic")
+                raise TypeError("invalid length of tuple")
         else:
-            if isinstance(ind, int):
-                base = cxxcimod.BinaryQuadraticModel_Dense
-            elif isinstance(ind, str):
-                base = cxxcimod.BinaryQuadraticModel_str_Dense
-            elif isinstance(ind, tuple):
-                if len(ind) == 2:
-                    base = cxxcimod.BinaryQuadraticModel_tuple2_Dense
-                elif len(ind) == 3:
-                    base = cxxcimod.BinaryQuadraticModel_tuple3_Dense
-                elif len(ind) == 4:
-                    base = cxxcimod.BinaryQuadraticModel_tuple4_Dense
-                else:
-                    raise TypeError("invalid length of tuple")
+            raise TypeError("invalid types of linear and quadratic")
+    else:
+        if isinstance(ind, int):
+            base = cxxcimod.BinaryQuadraticModel_Dense
+        elif isinstance(ind, str):
+            base = cxxcimod.BinaryQuadraticModel_str_Dense
+        elif isinstance(ind, tuple):
+            if len(ind) == 2:
+                base = cxxcimod.BinaryQuadraticModel_tuple2_Dense
+            elif len(ind) == 3:
+                base = cxxcimod.BinaryQuadraticModel_tuple3_Dense
+            elif len(ind) == 4:
+                base = cxxcimod.BinaryQuadraticModel_tuple4_Dense
             else:
-                raise TypeError("invalid types of linear and quadratic")
+                raise TypeError("invalid length of tuple")
+        else:
+            raise TypeError("invalid types of linear and quadratic")
 
     return base
 
 
 def extract_offset_and_vartype(*args, **kwargs):
     if kwargs == {}:
         if len(args) == 0:
@@ -159,45 +161,48 @@
                 cimod.SPIN,
                 cimod.BINARY,
                 "SPIN",
                 "BINARY",
             ]
             args = [
                 to_cxxcimod(elem)
-                if not isinstance(elem, np.ndarray) and vartypes.count(elem) != 0
+                if not isinstance(elem, (np.ndarray, csr_matrix)) and vartypes.count(elem) != 0
                 else elem
                 for elem in args
             ]
             kwargs = {
                 k: to_cxxcimod(v)
-                if not isinstance(elem, np.ndarray) and vartypes.count(v) != 0
+                if not isinstance(v, (np.ndarray, csr_matrix)) and vartypes.count(v) != 0
                 else v
                 for k, v in kwargs.items()
             }
+
             self.model_type = "cimod.BinaryQuadraticModel"
-            # if linear and quadratic are given and mode is dense
+            # if linear and quadratic are given. generate matrix and initialize as matrix
             if (
                 len(args) >= 2
                 and isinstance(args[0], dict)
                 and isinstance(args[1], dict)
-                and sparse is False
             ):
                 linear = args[0]
                 quadratic = args[1]
                 offset, vartype = extract_offset_and_vartype(*args[2:], **kwargs)
 
-                mat, idx_to_label = self._generate_mat(linear, quadratic, False)
+                mat, idx_to_label = self._generate_mat(linear, quadratic, False, sparse)
 
-                super().__init__(mat, idx_to_label, offset, vartype, fix_format=False)
+                if sparse is False:
+                    super().__init__(mat, idx_to_label, offset, vartype, fix_format=False)
+                else:
+                    super().__init__(mat, idx_to_label, offset, vartype)
 
             else:
                 super().__init__(*args, **kwargs)
 
         @staticmethod
-        def _generate_mat(linear, quadratic, include_quaddiag):
+        def _generate_mat(linear: dict, quadratic: dict, include_quaddiag: bool, sparse: bool) -> Tuple[Union[np.ndarray, csr_matrix], dict]:
             labels = set()
 
             for i in linear.keys():
                 labels.add(i)
 
             for i, j in quadratic.keys():
                 if (i == j) and (include_quaddiag == False):
@@ -213,29 +218,46 @@
                 labels.add(j)
 
             idx_to_label = sorted(labels)
             label_to_idx = {elem: k for k, elem in enumerate(idx_to_label)}
 
             mat_size = len(idx_to_label) + 1
 
-            mat = np.zeros(shape=(mat_size, mat_size))
+
+            # generate matrix (dense or sparse)
+            if sparse is False:
+                mat = np.zeros(shape=(mat_size, mat_size))
+            else:
+                # first defines dict and use `_update` function to make `dok_matrix`
+                # then convert to `csr_matrix`
+                mat = defaultdict(float)
+
             mat[mat_size - 1, mat_size - 1] = 1
 
             for i, val in linear.items():
                 mat[label_to_idx[i], mat_size - 1] += val
 
             for (i, j), val in quadratic.items():
                 idx_i = label_to_idx[i]
                 idx_j = label_to_idx[j]
                 if idx_i != idx_j:
                     mat[min(idx_i, idx_j), max(idx_i, idx_j)] += val
                 else:
                     mat[idx_i, mat_size - 1] += val
 
-            return mat, idx_to_label
+            if sparse is False:
+                return mat, idx_to_label
+            else:
+                dok_mat = dok_matrix((mat_size, mat_size))
+                # using `_update` function skips index checking
+                dok_mat._update(mat)
+                csr_mat = dok_mat.tocsr()
+                csr_mat.sort_indices()
+                return csr_mat, idx_to_label
+
 
         @property
         def vartype(self):
             vartype = super().get_vartype()
             if vartype == cxxcimod.Vartype.SPIN:
                 return dimod.SPIN
             else:
@@ -316,23 +338,23 @@
 
         @classmethod
         def from_qubo(cls, Q, offset=0.0, **kwargs):
             # cxxbqm = Base.from_qubo(Q, offset)
             # return cls(cxxbqm, **kwargs)
             # separate linear and quadratic
 
-            mat, idx_to_label = cls._generate_mat({}, Q, True)
+            mat, idx_to_label = cls._generate_mat({}, Q, True, sparse)
 
             return cls(mat, idx_to_label, offset, "BINARY", **kwargs)
 
         @classmethod
         def from_ising(cls, linear, quadratic, offset=0.0, **kwargs):
             # cxxbqm = Base.from_ising(linear, quadratic, offset)
             # return cls(cxxbqm, **kwargs)
-            mat, idx_to_label = cls._generate_mat(linear, quadratic, False)
+            mat, idx_to_label = cls._generate_mat(linear, quadratic, False, sparse)
 
             return cls(mat, idx_to_label, offset, "SPIN", **kwargs)
 
         @classmethod
         def from_serializable(cls, obj, **kwargs):
             cxxbqm = Base.from_serializable(obj)
             return cls(cxxbqm, **kwargs)
@@ -358,15 +380,16 @@
     else:
         raise TypeError("Invalid bqm_schema")
 
     return make_BinaryQuadraticModel(mock_linear, {}, sparse)
 
 
 def BinaryQuadraticModel(linear, quadratic, *args, **kwargs):
-    Model = make_BinaryQuadraticModel(linear, quadratic, kwargs.pop("sparse", False))
+    sparse_option = kwargs.pop("sparse", False)
+    Model = make_BinaryQuadraticModel(linear, quadratic, sparse_option)
 
     # offset and vartype
     offset, vartype = extract_offset_and_vartype(*args, **kwargs)
 
     return Model(linear, quadratic, offset, vartype)
 
 
@@ -374,31 +397,41 @@
     mat, variables: list = None, offset=0.0, vartype="BINARY", **kwargs
 ):
     if variables is None:
         # generate array
         num_variables = mat.shape[0]
         variables = list(range(num_variables))
 
+    sparse_option = kwargs.pop("sparse", False)
+
     return make_BinaryQuadraticModel(
-        {variables[0]: 1.0}, {}, kwargs.pop("sparse", False)
+        {variables[0]: 1.0}, {}, sparse_option
     ).from_numpy_matrix(mat, variables, offset, vartype, True, **kwargs)
 
 
 BinaryQuadraticModel.from_numpy_matrix = bqm_from_numpy_matrix
 
-BinaryQuadraticModel.from_qubo = (
-    lambda Q, offset=0.0, **kwargs: make_BinaryQuadraticModel(
-        {}, Q, kwargs.pop("sparse", False)
+def bqm_from_qubo(Q, offset=0.0, **kwargs):
+    sparse_option = kwargs.pop("sparse", False)
+
+    return make_BinaryQuadraticModel(
+        {}, Q, sparse_option
     ).from_qubo(Q, offset, **kwargs)
-)
 
-BinaryQuadraticModel.from_ising = (
-    lambda linear, quadratic, offset=0.0, **kwargs: make_BinaryQuadraticModel(
-        linear, quadratic, kwargs.pop("sparse", False)
+BinaryQuadraticModel.from_qubo = bqm_from_qubo
+
+
+def bqm_from_ising(linear, quadratic, offset=0.0, **kwargs):
+    sparse_option = kwargs.pop("sparse", False)
+
+    return make_BinaryQuadraticModel(
+        linear, quadratic, sparse_option
     ).from_ising(linear, quadratic, offset, **kwargs)
-)
+
+BinaryQuadraticModel.from_ising = bqm_from_ising
+
 
 BinaryQuadraticModel.from_serializable = (
     lambda obj, **kwargs: make_BinaryQuadraticModel_from_JSON(obj).from_serializable(
         obj, **kwargs
     )
 )
```

### Comparing `jij_cimod-1.4.9/cimod/model/legacy/__init__.py` & `jij_cimod-1.5.0/cimod/model/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cimod/model/legacy/binary_quadratic_model.py` & `jij_cimod-1.5.0/cimod/model/legacy/binary_quadratic_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 import cimod.cxxcimod as cxxcimod
 import dimod
 import numpy as np
 
 from cimod.utils.decolator import recalc
 from cimod.vartype import to_cxxcimod
 
-__all__ = []
-
 
 def make_BinaryQuadraticModel(linear, quadratic):
     """BinaryQuadraticModel factory.
        Generate BinaryQuadraticModel class with the base class specified by the arguments linear and quadratic
     Args:
         linear (dict): linear bias
         quadratic (dict): quadratic bias
```

### Comparing `jij_cimod-1.4.9/cimod/utils/__init__.py` & `jij_cimod-1.5.0/cimod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cimod/utils/decolator.py` & `jij_cimod-1.5.0/cimod/utils/decolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-__all__ = []
-
-
 def disabled(func):
     def wrapper(*args, **kwargs):
         raise NotImplementedError("The function {} is disabled.".format(func.__name__))
 
     return wrapper
```

### Comparing `jij_cimod-1.4.9/cimod/utils/response.py` & `jij_cimod-1.5.0/cimod/utils/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import dimod
 
-__all__ = []
-
-
 def get_state_and_energy(
     model, result_state, offset=0, model_variables=[]
 ) -> tuple[dict, float]:
     """get converted state and energy.
     This function receives raw array of spins or binaries.
     If vartype of model and the vartype of the raw array are different, the raw array is automatically converted to the vartype of model with any offset shift.
```

### Comparing `jij_cimod-1.4.9/cimod/vartype.py` & `jij_cimod-1.5.0/cimod/vartype.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,19 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import cimod.cxxcimod, dimod
 
-from dimod import SPIN as _SPIN
-from dimod import BINARY as _BINARY
-from dimod import Vartype as _Vartype
-
-__all__ = []
+from dimod import BINARY as _BINARY, SPIN as _SPIN, Vartype as _Vartype
 
 SPIN = _SPIN
 BINARY = _BINARY
 Vartype = _Vartype
 
 
 def to_cxxcimod(vartype):
```

### Comparing `jij_cimod-1.4.9/cmake/FindGcov.cmake` & `jij_cimod-1.5.0/cmake/FindGcov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cmake/FindLcov.cmake` & `jij_cimod-1.5.0/cmake/FindLcov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cmake/Findcodecov.cmake` & `jij_cimod-1.5.0/cmake/Findcodecov.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cmake/PythonAutoDetectOSX.cmake` & `jij_cimod-1.5.0/cmake/PythonAutoDetectOSX.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/cmake/llvm-cov-wrapper` & `jij_cimod-1.5.0/cmake/llvm-cov-wrapper`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/external/eigen.cmake` & `jij_cimod-1.5.0/external/eigen.cmake`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/external/json.cmake` & `jij_cimod-1.5.0/external/json.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 set(BUILD_TESTING OFF)
 
 #### nlohmann_json ####
 FetchContent_Declare(
      nlohmann_json
      GIT_REPOSITORY  https://github.com/nlohmann/json
-     GIT_TAG         v3.10.5
+     GIT_TAG         v3.11.2
      GIT_SHALLOW     TRUE
      )
      
 FetchContent_MakeAvailable(nlohmann_json)
 
 # Since the git repository of nlohmann/json is huge, we store only a single-include file json.hpp in our project.
 #set(BUILD_TESTING OFF)
```

### Comparing `jij_cimod-1.4.9/jij_cimod.egg-info/PKG-INFO` & `jij_cimod-1.5.0/jij_cimod.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 Metadata-Version: 2.1
 Name: jij-cimod
-Version: 1.4.9
+Version: 1.5.0
 Summary: C++ library for a binary (and polynomial) quadratic model.
 Home-page: https://www.openjij.org
 Author: Jij Inc.
-Author-email: info@j-ij.com
+Author-email: info@openjij.org
 License: Apache License 2.0
 Project-URL: Source, https://github.com/OpenJij/cimod
-Project-URL: Documentation, https://cimod.openjij.org
+Project-URL: Documentation, http://openjij.github.io/Cimod-Documentation/
+Project-URL: PythonDocumentation, https://openjij.github.io/cimod/
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# cimod : C++ header-only library for a binary quadratic model 
+# cimod : C++ header-only library for a binary quadratic model
+
 [![PyPI version shields.io](https://img.shields.io/pypi/v/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI implementation](https://img.shields.io/pypi/implementation/jij-cimod.svg)](https://pypi.python.org/pypi/ji-cimod/)
 [![PyPI format](https://img.shields.io/pypi/format/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI license](https://img.shields.io/pypi/l/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
 [![PyPI download month](https://img.shields.io/pypi/dm/jij-cimod.svg)](https://pypi.python.org/pypi/jij-cimod/)
+[![Downloads](https://pepy.tech/badge/jij-cimod)](https://pepy.tech/project/jij-cimod)
 
 [![Test](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/ci-test.yml)
 [![Build&Upload](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/build_and_upload.yaml)
 [![CodeQL](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/codeql.yml)
 [![Build Documentation](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/buid-doc.yml)
 [![pages-build-deployment](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/OpenJij/cimod/actions/workflows/pages/pages-build-deployment)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/55990ff022864098a2413c0cc4ab8299)](https://www.codacy.com/gh/OpenJij/cimod/dashboard?utm_source=github.com&utm_medium=referral&utm_content=OpenJij/cimod&utm_campaign=Badge_Grade)
+[![Maintainability](https://api.codeclimate.com/v1/badges/59876c82cc2200ef1dfa/maintainability)](https://codeclimate.com/github/OpenJij/cimod/maintainability)
 [![codecov](https://codecov.io/gh/OpenJij/cimod/branch/master/graph/badge.svg?token=BE45W9FJHA)](https://codecov.io/gh/OpenJij/cimod)
 
-## Coverage Graph 
-|**Sunburst**|**Grid**|**Icicle**|
-| ---- | ---- | ---- |
-|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a>|<a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a>|
+## Coverage Graph
 
+| **Sunburst**                                                                                                                                                     | **Grid**                                                                                                                                                     | **Icicle**                                                                                                                                                     |
+| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/sunburst.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/tree.svg?token=BE45W9FJHA" width="100%"/></a> | <a href="https://codecov.io/gh/OpenJij/cimod"><img src="https://codecov.io/gh/OpenJij/cimod/branch/main/graphs/icicle.svg?token=BE45W9FJHA" width="100%"/></a> |
 
-* [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Documents](https://openjij.github.io/Cimod-Documentation/)
+- [Python Documents](https://openjij.github.io/cimod/)
 
 # How to use
 
 You should only include a header `src/binary_quadratic_model.hpp` in your project.
 
 ## Example
 
@@ -106,25 +112,27 @@
 bqm = cimod.BinaryQuadraticModel(linear, quadratic, offset, vartype)
 
 print(bqm.linear)
 print(bqm.quadratic)
 
 ```
 
-## For Contributor 
+## For Contributor
+
 Use `pre-commit` for auto chech before git commit.
 `.pre-commit-config.yaml`
-``` 
+
+```
 # pipx install pre-commit 
 # or 
 # pip install pre-commit
 pre-commit install
 ```
 
-## Install 
+## Install
 
 ### via this directory
 
 ```sh
 $ python -m pip install -vvv .
 ```
 
@@ -133,70 +141,77 @@
 ```sh
 # Binary
 $ pip install jij-cimod
 # From Source 
 $ pip install --no-binary=jij-cimod jij-cimod 
 ```
 
-## Test 
+## Test
+
+### Python
 
-### Python 
 ```sh
 $ python -m venv .venv
 $ pip install pip-tools 
-$ pip-compile
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt
 $ source .venv/bin/activate
 $ export CMAKE_BUILD_TYPE=Debug
 $ python setup.py --force-cmake install --build-type Debug -G Ninja
 $ python setup.py --build-type Debug test 
 $ python -m coverage html
 ```
 
-### C++ 
+### C++
+
 ```sh
 $ mkdir build 
 $ cmake -DCMAKE_BUILD_TYPE=Debug -S . -B build
 $ cmake --build build --parallel
 $ cd build
 $ ./tests/cimod_test
 # Alternatively Use CTest 
 $ ctest --extra-verbose --parallel --schedule-random
 ```
 
 Needs: CMake > 3.22, C++17
 
-- Format 
+- Format
+
 ```sh
 $ pip-compile format-requirements.in
 $ pip-sync format-requirements.txt
 ```
-``` sh
+
+```sh
 $ python -m isort 
 $ python -m black 
 ```
 
 - Aggressive Format
-```sh 
+
+```sh
 $ python -m isort --force-single-line-imports --verbose ./cimod
 $ python -m autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports --remove-unused-variables ./cimod
 $ python -m autopep8 --in-place --aggressive --aggressive  --recursive ./cimod
 $ python -m isort ./cimod
 $ python -m black ./cimod
 ```
 
 - Lint
-```sh 
-$ pip-compile
+
+```sh
+$ pip-compile setup.cfg
 $ pip-compile dev-requirements.in
 $ pip-compile lint-requirements.in
 $ pip-sync requirements.txt dev-requirements.txt lint-requirements.txt
 ```
-``` sh 
+
+```sh
 $ python -m flake8
 $ python -m mypy
 $ python -m pyright
 ```
 
 ## Benchmark
 
@@ -252,30 +267,33 @@
     c = benchmark(N, cimod)
     print("{} {} {}".format(N, d, c))
     fil.write("{} {} {}\n".format(N, d, c))
 ```
 
 ### Software versions
 
-|       Package        | Version |
-| -------------------- | ------- |
-| [cimod](https://github.com/OpenJij/cimod)     | 1.0.3   |
-| [dimod](https://github.com/dwavesystems/dimod)| 0.9.2   |
+| Package                                        | Version |
+| ---------------------------------------------- | ------- |
+| [cimod](https://github.com/OpenJij/cimod)      | 1.0.3   |
+| [dimod](https://github.com/dwavesystems/dimod) | 0.9.2   |
 
 ### Result
+
 ![benchmark](https://github.com/OpenJij/cimod/blob/image_store/figure.png)
 
+### Licences
+
+Copyright 2022 Jij Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");\
+you may not use this file except in compliance with the License.\
+You may obtain a copy of the License at
 
-### Licences 
-Copyright 2022 Jij Inc.  
+```
+ http://www.apache.org/licenses/LICENSE-2.0  
+```
 
-Licensed under the Apache License, Version 2.0 (the "License");  
-you may not use this file except in compliance with the License.  
-You may obtain a copy of the License at  
-
-     http://www.apache.org/licenses/LICENSE-2.0  
-
-Unless required by applicable law or agreed to in writing, software  
-distributed under the License is distributed on an "AS IS" BASIS,  
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
-See the License for the specific language governing permissions and  
-limitations under the License.  
+Unless required by applicable law or agreed to in writing, software\
+distributed under the License is distributed on an "AS IS" BASIS,\
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\
+See the License for the specific language governing permissions and\
+limitations under the License.
```

### Comparing `jij_cimod-1.4.9/jij_cimod.egg-info/SOURCES.txt` & `jij_cimod-1.5.0/jij_cimod.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-.coveragerc
-.gitattribute
 .reviewdog.yml
 CMakeLists.txt
-CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 SECURITY.md
+doc-requirements.in
 pyproject.toml
 setup.cfg
 setup.py
 cimod/CMakeLists.txt
 cimod/__init__.py
 cimod/_version.py
 cimod/main.cpp
@@ -32,29 +30,29 @@
 cmake/PythonAutoDetectOSX.cmake
 cmake/llvm-cov-wrapper
 external/eigen.cmake
 external/googletest.cmake
 external/json.cmake
 external/pybind11-json.cmake
 external/pybind11.cmake
+include/CMakeLists.txt
+include/cimod/binary_polynomial_model.hpp
+include/cimod/binary_quadratic_model.hpp
+include/cimod/binary_quadratic_model_dict.hpp
+include/cimod/disable_eigen_warning.hpp
+include/cimod/hash.hpp
+include/cimod/json.hpp
+include/cimod/utilities.hpp
+include/cimod/vartypes.hpp
 jij_cimod.egg-info/PKG-INFO
 jij_cimod.egg-info/SOURCES.txt
 jij_cimod.egg-info/dependency_links.txt
 jij_cimod.egg-info/not-zip-safe
 jij_cimod.egg-info/requires.txt
 jij_cimod.egg-info/top_level.txt
-src/CMakeLists.txt
-src/binary_polynomial_model.hpp
-src/binary_quadratic_model.hpp
-src/binary_quadratic_model_dict.hpp
-src/disable_eigen_warning.hpp
-src/hash.hpp
-src/json.hpp
-src/utilities.hpp
-src/vartypes.hpp
 tests/CMakeLists.txt
 tests/__init__.py
 tests/test.cpp
 tests/test_0_basic.py
 tests/test_bqm.hpp
 tests/test_legacy_model.py
 tests/test_model.py
```

### Comparing `jij_cimod-1.4.9/pyproject.toml` & `jij_cimod-1.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 ]
 reportImportCycles = 'warning'
 reportUnusedImport = 'warning'
 reportUnusedVariable =  'warning'
 reportDuplicateImport = 'warning'
 
 [tool.cibuildwheel]
-skip = ["cp36*", "*musllinux_x86_64", "*musllinux_aarch64", "pp*"]
+skip = ["cp36*", "cp37*", "*musllinux_x86_64", "*musllinux_aarch64", "pp*"]
 build-verbosity = 1
 dependency-versions = "latest"
 
 [tool.cibuildwheel.linux]
 archs = ["x86_64", "aarch64"]
 build-frontend = "build"
 #environment = "-CFLAGS='-march=haswell' -CXXFLAGS='-march=haswell' -FFLAGS='-march=haswell'"
@@ -106,18 +106,18 @@
 manylinux-aarch64-image = "quay.io/pypa/manylinux_2_28_aarch64:latest"
 repair-wheel-command = "auditwheel repair --lib-sdir . -w {dest_dir} {wheel}"
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "arm64"]
 build-frontend = "build"
 before-build = [ 
-    "pip install pybind11 cmake ninja", 
+    "pip install --upgrade pip wheel build pybind11 cmake ninja", 
 ]
 
 [tool.cibuildwheel.windows]
 archs = ["AMD64"]
 #"vcpkg --triplet x64-windows-static install openblas[threads] --recurse", 
 #"vcpkg --triplet x64-windows-static install clapack --recurse", 
 before-build = [ 
-    "pip install cmake pybind11 delvewheel", 
+    "pip install --upgrade pip wheel build cmake pybind11 delvewheel", 
 ]
 repair-wheel-command = "delvewheel repair -w {dest_dir} {wheel}"
```

### Comparing `jij_cimod-1.4.9/setup.cfg` & `jij_cimod-1.5.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -5,45 +5,49 @@
 [aliases]
 test = pytest
 
 [metadata]
 name = jij_cimod
 url = https://www.openjij.org
 author = Jij Inc.
-author_email = info@j-ij.com
+author_email = info@openjij.org
 description = C++ library for a binary (and polynomial) quadratic model.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_files = LICENSE
 license = Apache License 2.0
 classifiers = 
 	License :: OSI Approved :: Apache Software License
 	Intended Audience :: Science/Research
 	Programming Language :: Python
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 project_urls = 
 	Source=https://github.com/OpenJij/cimod
-	Documentation=https://cimod.openjij.org
+	Documentation=http://openjij.github.io/Cimod-Documentation/
+	PythonDocumentation=https://openjij.github.io/cimod/
 
 [options]
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.12
+install_requires = 
+	numpy >=1.17.3, < 1.26.0
+	dimod < 0.13.0
+	scipy >= 1.7.3, < 1.12.0
 tests_require = 
 	pytest
 	pytest-mock
 	pytest-cov
-	pytest-html
 	pytest-runner
 	pytest-randomly
 	pytest-spec
 	coverage
 
 [egg_info]
 tag_build =
```

### Comparing `jij_cimod-1.4.9/setup.py` & `jij_cimod-1.5.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,54 +10,34 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
-from packaging.version import LegacyVersion
-
 try:
     from skbuild import setup
-    from skbuild.cmaker import get_cmake_version
-    from skbuild.exceptions import SKBuildError
 except ImportError:
-    print(
-        "Please update pip, you need pip 10 or greater,\n"
-        " or you need to install the PEP 518 requirements in pyproject.toml yourself",
-        file=sys.stderr,
-    )
-    raise
+    from setuptools import setup
 
 setup_requires = [
-    "numpy < 1.23.0",
-    "pybind11 >= 2.9.2, < 2.10.0",
+    "numpy",
+    "pybind11",
+    "cmake > 3.20",
+    "scikit-build > 0.16.0"
 ]
 
 if any(arg in sys.argv for arg in ("pytest", "test")):
     setup_requires.append("pytest-runner")
 
-# Add CMake as a build requirement if cmake is not installed or is too low a version.
-try:
-    if LegacyVersion(get_cmake_version()) < LegacyVersion("3.20"):
-        setup_requires.append("cmake")
-except SKBuildError:
-    setup_requires.append("cmake")
-
 setup(
     setup_requires=setup_requires,
-    install_requires=[
-        "numpy < 1.23.0",
-        'dimod <= 0.10.17; python_version < "3.10"',
-        'dimod < 0.12.0; python_version >= "3.10"',
-        "scipy >= 1.7.3, < 1.9.0",
-    ],
     packages=[
         "cimod",
         "cimod.utils",
         "cimod.model",
         "cimod.model.legacy",
     ],
     cmake_install_dir="cimod",
-    include_package_data=True,
+    include_package_data=False,
     zip_safe=False,
 )
```

### Comparing `jij_cimod-1.4.9/src/CMakeLists.txt` & `jij_cimod-1.5.0/include/CMakeLists.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,22 +9,17 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 add_library(cxxcimod_header_only INTERFACE)
-  
-#target_precompile_headers(cxxcimod_header_only INTERFACE
-#  json.hpp
-#  disable_eigen_warning.hpp
-#) 
 
 target_include_directories(cxxcimod_header_only INTERFACE 
-  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
+  $<BUILD_INTERFACE:${CIMOD_INCLUDE_DIR}>
   $<INSTALL_INTERFACE:include>
 )
 
 target_link_libraries(cxxcimod_header_only INTERFACE 
     nlohmann_json::nlohmann_json
     $<IF:$<TARGET_EXISTS:Eigen3::Eigen>,Eigen3::Eigen,cimod-eigen_lib>
     $<$<TARGET_EXISTS:OpenMP::OpenMP_CXX>:OpenMP::OpenMP_CXX>
```

### Comparing `jij_cimod-1.4.9/src/binary_polynomial_model.hpp` & `jij_cimod-1.5.0/include/cimod/binary_polynomial_model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -112,31 +112,34 @@
  * }
  *
  * @endcode
  */
 
 #pragma once
 
-#include "hash.hpp"
-#include "utilities.hpp"
-#include "vartypes.hpp"
-
 #include <algorithm>
 #include <bitset>
 #include <cstdint>
 #include <iostream>
-#include <nlohmann/json.hpp>
 #include <set>
 #include <string>
 #include <tuple>
 #include <typeinfo>
 #include <unordered_map>
+#include <unordered_set>
 #include <utility>
 #include <vector>
 
+#include <nlohmann/json.hpp>
+
+#include "cimod/hash.hpp"
+#include "cimod/utilities.hpp"
+#include "cimod/vartypes.hpp"
+
+
 namespace cimod {
 
   //! @brief Type alias for the polynomial interactions as std::unordered_map.
   //! @tparam IndexType
   //! @tparam FloatType
   template<typename IndexType, typename FloatType>
   using Polynomial = std::unordered_map<std::vector<IndexType>, FloatType, vector_hash>;
```

### Comparing `jij_cimod-1.4.9/src/binary_quadratic_model.hpp` & `jij_cimod-1.5.0/include/cimod/binary_quadratic_model.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -70,35 +70,16 @@
  * bqm.print();
  *
  * return 0;
  * }
  * @endcode
  */
 
-/**
- * @file binary_quadratic_model.hpp
- * @author Kohji Nishimura
- * @brief Dense BinaryQuadraticModel class
- * @version 1.0.0
- * @date 2020-03-24
- *
- * @copyright Copyright (c) Jij Inc. 2020
- *
- */
-
 #pragma once
 
-#include "disable_eigen_warning.hpp"
-#include "hash.hpp"
-#include "json.hpp"
-#include "utilities.hpp"
-#include "vartypes.hpp"
-
-#include <Eigen/Dense>
-#include <Eigen/Sparse>
 #include <algorithm>
 #include <cassert>
 #include <cstdint>
 #include <functional>
 #include <iostream>
 #include <limits>
 #include <set>
@@ -107,14 +88,23 @@
 #include <type_traits>
 #include <typeinfo>
 #include <unordered_map>
 #include <unordered_set>
 #include <utility>
 #include <vector>
 
+#include <Eigen/Dense>
+#include <Eigen/Sparse>
+
+#include "cimod/disable_eigen_warning.hpp"
+#include "cimod/hash.hpp"
+#include "cimod/json.hpp"
+#include "cimod/utilities.hpp"
+#include "cimod/vartypes.hpp"
+
 namespace cimod {
   /**
    * @brief Type alias for linear bias
    *
    * @tparam IndexType
    */
   template<typename IndexType, typename FloatType>
@@ -919,15 +909,16 @@
      * \f]
      *
      * @param mat
      * @param labels_vec
      */
     inline void _initialize_quadmat( const SparseMatrix &mat, const std::vector<IndexType> &labels_vec ) {
       this->_quadmat = mat;
-      _idx_to_label = std::vector<IndexType>( labels_vec.begin(), labels_vec.end() );
+      std::unordered_set<IndexType> labels( labels_vec.begin(), labels_vec.end() );
+      _idx_to_label = std::vector<IndexType>( labels.begin(), labels.end() );
       std::sort( _idx_to_label.begin(), _idx_to_label.end() );
       _set_label_to_idx();
     }
 
     /**
      * @brief change internal variable from Ising to QUBO ones for dense matrix
      * The following conversion is applied:
```

### Comparing `jij_cimod-1.4.9/src/binary_quadratic_model_dict.hpp` & `jij_cimod-1.5.0/include/cimod/binary_quadratic_model_dict.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -8,48 +8,38 @@
 
 //    Unless required by applicable law or agreed to in writing, software
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
-/**
- * @file binary_quadratic_model.hpp
- * @author Fumiya Watanabe
- * @brief BinaryQuadraticModel class
- * @version 1.0.0
- * @date 2020-03-24
- *
- * @copyright Copyright (c) Jij Inc. 2020
- *
- */
-
 #pragma once
 
-#include "binary_quadratic_model.hpp"
-#include "disable_eigen_warning.hpp"
-#include "hash.hpp"
-#include "json.hpp"
-#include "utilities.hpp"
-#include "vartypes.hpp"
-
-#include <Eigen/Dense>
 #include <algorithm>
 #include <cstdint>
 #include <functional>
 #include <iostream>
 #include <set>
 #include <string>
 #include <tuple>
 #include <typeinfo>
 #include <unordered_map>
 #include <unordered_set>
 #include <utility>
 #include <vector>
 
+#include <Eigen/Dense>
+
+#include "cimod/binary_quadratic_model.hpp"
+#include "cimod/disable_eigen_warning.hpp"
+#include "cimod/hash.hpp"
+#include "cimod/json.hpp"
+#include "cimod/utilities.hpp"
+#include "cimod/vartypes.hpp"
+
 namespace cimod {
 
   struct Dict { };
 
   /**
    * @brief Class for legacy binary quadratic model (dict datastructure).
    */
```

### Comparing `jij_cimod-1.4.9/src/disable_eigen_warning.hpp` & `jij_cimod-1.5.0/include/cimod/disable_eigen_warning.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/src/hash.hpp` & `jij_cimod-1.5.0/include/cimod/hash.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,14 @@
 
 //    Unless required by applicable law or agreed to in writing, software
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
-/**
- * @file hash.hpp
- * @author Fumiya Watanabe
- * @brief Hash function for std::pair
- * @version 1.0.0
- * @date 2020-03-13
- *
- * @copyright Copyright (c) Jij Inc. 2020
- *
- */
-
 #pragma once
 
 #include <cstdint>
 #include <iostream>
 #include <utility>
 #include <vector>
```

### Comparing `jij_cimod-1.4.9/src/json.hpp` & `jij_cimod-1.5.0/include/cimod/json.hpp`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/src/utilities.hpp` & `jij_cimod-1.5.0/include/cimod/utilities.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 #pragma once
 
-#include "vartypes.hpp"
-
 #include <unordered_map>
+#include <unordered_set>
+
+#include "cimod/vartypes.hpp"
 
 namespace cimod {
   /**
    * @brief Insert or assign a element of unordered_map (for C++14 or C++11)
    *
    * @tparam C_key
    * @tparam C_value
```

### Comparing `jij_cimod-1.4.9/src/vartypes.hpp` & `jij_cimod-1.5.0/include/cimod/vartypes.hpp`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,14 @@
 
 //    Unless required by applicable law or agreed to in writing, software
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
-/**
- * @file vartypes.hpp
- * @author Fumiya Watanabe
- * @brief Definition of variable type
- * @version 1.0.0
- * @date 2020-03-17
- *
- * @copyright Copyright (c) Jij Inc. 2020
- *
- */
-
 #pragma once
 
 #include <iostream>
 
 namespace cimod {
   /**
    * @brief Enum class for representing problem type
```

### Comparing `jij_cimod-1.4.9/tests/CMakeLists.txt` & `jij_cimod-1.5.0/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/tests/__init__.py` & `jij_cimod-1.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/tests/test.cpp` & `jij_cimod-1.5.0/tests/test.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 //    distributed under the License is distributed on an "AS IS" BASIS,
 //    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 #include <gtest/gtest.h>
 
-#include <binary_quadratic_model.hpp>
-#include <binary_polynomial_model.hpp>
-#include <binary_quadratic_model_dict.hpp>
-
-#include "test_bqm.hpp"
-
 #include <nlohmann/json.hpp>
 
 #include <unordered_map>
 #include <utility>
 #include <vector>
 #include <cstdint>
 #include <string>
 #include <iostream>
 #include <tuple>
 
+#include <cimod/binary_quadratic_model.hpp>
+#include <cimod/binary_polynomial_model.hpp>
+#include <cimod/binary_quadratic_model_dict.hpp>
+
+#include "test_bqm.hpp"
+
 using json = nlohmann::json;
 using namespace cimod;
 
 namespace
 {
     TEST(DenseConstructionTest, Construction)
     {
```

### Comparing `jij_cimod-1.4.9/tests/test_0_basic.py` & `jij_cimod-1.5.0/tests/test_0_basic.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/tests/test_bqm.hpp` & `jij_cimod-1.5.0/tests/test_bqm.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 //    See the License for the specific language governing permissions and
 //    limitations under the License.
 
 #pragma once
 
 #include <gtest/gtest.h>
 
-#include <binary_quadratic_model.hpp>
-
-#include <nlohmann/json.hpp>
-
 #include <unordered_map>
 #include <utility>
 #include <vector>
 #include <cstdint>
 #include <string>
 #include <iostream>
 #include <tuple>
 
+#include <nlohmann/json.hpp>
+
+#include <cimod/binary_quadratic_model.hpp>
+
 using json = nlohmann::json;
 using namespace cimod;
 
 template<typename IndexType, typename FloatType, typename DataType>
 using BQM = BinaryQuadraticModel<IndexType, FloatType, DataType>;
 
 template<typename DataType>
```

### Comparing `jij_cimod-1.4.9/tests/test_legacy_model.py` & `jij_cimod-1.5.0/tests/test_legacy_model.py`

 * *Files identical despite different names*

### Comparing `jij_cimod-1.4.9/tests/test_model.py` & `jij_cimod-1.5.0/tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,20 @@
             self.assertEqual(type(bqm.interaction_matrix()), mat_type)
 
             bqm = cimod.model.BinaryQuadraticModel(self.h, self.J, 'SPIN', sparse=sparse)
             self.assertAlmostEqual(bqm.offset, 0)
             self.assertAlmostEqual(bqm.vartype, dimod.SPIN)
             self.assertEqual(type(bqm.interaction_matrix()), mat_type)
 
+            # empty object
+            bqm = cimod.model.BinaryQuadraticModel({}, {}, 'SPIN', sparse=sparse)
+            self.assertAlmostEqual(bqm.offset, 0)
+            self.assertAlmostEqual(bqm.vartype, dimod.SPIN)
+            self.assertEqual(type(bqm.interaction_matrix()), mat_type)
+
     def test_bqm_calc_energy(self):
         # Test to calculate energy
 
         # Test Ising energy
         for (sparse, mat_type) in [(True, csr_matrix), (False, np.ndarray)]:
             bqm = cimod.model.BinaryQuadraticModel(self.h, self.J, 'SPIN', sparse=sparse)
             ising_energy_bqm = bqm.energy(self.spins)
```

