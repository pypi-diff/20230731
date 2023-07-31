# Comparing `tmp/drift-bytes-0.1.0.tar.gz` & `tmp/drift-bytes-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drift-bytes-0.1.0.tar", last modified: Thu Jul 20 14:06:55 2023, max compression
+gzip compressed data, was "drift-bytes-0.2.0.tar", last modified: Mon Jul 31 15:19:05 2023, max compression
```

## Comparing `drift-bytes-0.1.0.tar` & `drift-bytes-0.2.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.394607 drift-bytes-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/.clang-format
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.382606 drift-bytes-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     6955 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     2767 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/CPPLINT.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-20 14:06:55.394607 drift-bytes-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/cmake/
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/cmake/drift_bytes-config.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/conan/
--rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/conan/conanfile.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/conan/linux_armv8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/conan/test_package/
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/conan/test_package/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/conan/test_package/conanfile.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/conan/test_package/src/
--rw-r--r--   0 runner    (1001) docker     (122)      239 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/conan/test_package/src/example.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/drift_bytes/
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/drift_bytes/bytes.h
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/format.txt
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/src/drift_bytes/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/src/drift_bytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4567 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/src/drift_bytes/bytes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/src/drift_bytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-20 14:06:55.000000 drift-bytes-0.1.0/python/src/drift_bytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      833 2023-07-20 14:06:55.000000 drift-bytes-0.1.0/python/src/drift_bytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:06:55.000000 drift-bytes-0.1.0/python/src/drift_bytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-20 14:06:55.000000 drift-bytes-0.1.0/python/src/drift_bytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6060 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/src/main.cc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/python/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      384 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/tests/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (122)     2618 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/tests/test_bytes_scalars.py
--rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/python/tests/test_bytes_vectors.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-20 14:06:55.394607 drift-bytes-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:06:55.390606 drift-bytes-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2600 2023-07-20 14:06:23.000000 drift-bytes-0.1.0/tests/bytes_test.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.947524 drift-bytes-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      799 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/.clang-format
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.939524 drift-bytes-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     7162 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2828 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/CPPLINT.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-31 15:19:05.947524 drift-bytes-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1146 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/cmake/
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/cmake/drift_bytes-config.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/conan/
+-rw-r--r--   0 runner    (1001) docker     (122)     2061 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/conan/conanfile.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/conan/linux_armv8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/conan/test_package/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/conan/test_package/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/conan/test_package/conanfile.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/conan/test_package/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/conan/test_package/src/example.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/drift_bytes/
+-rw-r--r--   0 runner    (1001) docker     (122)     8761 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/drift_bytes/bytes.h
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/format.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/python/
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/python/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       53 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/python/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/python/src/drift_bytes/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/src/drift_bytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5897 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/src/drift_bytes/bytes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.943524 drift-bytes-0.2.0/python/src/drift_bytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1443 2023-07-31 15:19:05.000000 drift-bytes-0.2.0/python/src/drift_bytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      819 2023-07-31 15:19:05.000000 drift-bytes-0.2.0/python/src/drift_bytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 15:19:05.000000 drift-bytes-0.2.0/python/src/drift_bytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-31 15:19:05.000000 drift-bytes-0.2.0/python/src/drift_bytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/src/main.cc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.947524 drift-bytes-0.2.0/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/tests/test_buffers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      899 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/python/tests/test_variant.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 15:19:05.947524 drift-bytes-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2366 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 15:19:05.947524 drift-bytes-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-31 15:18:39.000000 drift-bytes-0.2.0/tests/bytes_test.cc
```

### Comparing `drift-bytes-0.1.0/.clang-format` & `drift-bytes-0.2.0/.clang-format`

 * *Files identical despite different names*

### Comparing `drift-bytes-0.1.0/.github/workflows/ci.yml` & `drift-bytes-0.2.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
       - uses: actions/checkout@v3
       - name: Install cpplint
         run: pip3 install -r format.txt
       - name: Check
         run: black --check .
 
   build_test:
-    needs: [ cpplint, black]
+    needs: [ cpplint, black ]
     runs-on: ${{ matrix.os }}
     name: Build and test C++ part
     strategy:
       matrix:
         build_type: [ Debug, Release ]
         os: [ ubuntu-22.04, windows-2019, macos-12 ]
     steps:
@@ -210,16 +210,23 @@
     steps:
       - uses: actions/checkout@v3
 
       - name: Prefix version for development version
         if: ${{ (github.ref == 'refs/heads/develop') }}
         run: echo "VERSION_SUFFIX=$(echo ${GITHUB_RUN_ID})" >> $GITHUB_ENV
 
+      - uses: actions/setup-python@v3
+
+      - name: Install cibuildwheel
+        run: python -m pip install cibuildwheel==2.14.1
+
       - name: Build wheels
-        uses: pypa/cibuildwheel@v2.13.1
+        run: python -m cibuildwheel --output-dir wheelhouse
+        env:
+          MACOSX_DEPLOYMENT_TARGET: 10.13
 
       - name: Verify clean directory
         run: |
           git diff --exit-code
         shell: bash
 
       - name: Upload wheels
```

### Comparing `drift-bytes-0.1.0/.pre-commit-config.yaml` & `drift-bytes-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drift-bytes-0.1.0/CMakeLists.txt` & `drift-bytes-0.2.0/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 cmake_minimum_required(VERSION 3.16)
 
-project(drift_bytes VERSION 0.1.0 LANGUAGES CXX)
+project(drift_bytes VERSION 0.2.0 LANGUAGES CXX)
 
 option(DB_BUILD_TESTS "Enable unit tests" OFF)
 
 set(TARGET_NAME ${PROJECT_NAME})
-add_library(${TARGET_NAME} INTERFACE)
 
+add_library(${TARGET_NAME} INTERFACE)
 add_library(${TARGET_NAME}::${TARGET_NAME} ALIAS ${TARGET_NAME})
 
 if(SKBUILD)
     list(APPEND CMAKE_MODULE_PATH ${CMAKE_BINARY_DIR})
     list(APPEND CMAKE_PREFIX_PATH ${CMAKE_BINARY_DIR})
     set(CMAKE_CURRENT_BINARY_DIR ${CMAKE_BINARY_DIR})
 
@@ -45,14 +45,15 @@
 
 link_libraries(${TARGET_NAME} cereal::cereal)
 
 set_target_properties(
     ${TARGET_NAME}
     PROPERTIES CXX_STANDARD 17 CXX_STANDARD_REQUIRED ON CXX_EXTENSIONS OFF
 )
+target_compile_features(${TARGET_NAME} INTERFACE cxx_std_17)
 
 target_include_directories(
     ${TARGET_NAME}
     INTERFACE
         ${cereal_INCLUDE_DIRS}
         $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>
 )
```

### Comparing `drift-bytes-0.1.0/LICENSE` & `drift-bytes-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drift-bytes-0.1.0/PKG-INFO` & `drift-bytes-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-bytes
-Version: 0.1.0
+Version: 0.2.0
 Summary: A serializer for typed data in the Drift infrastructure.
 Home-page: https://github.com/panda-official/DriftBytes
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `drift-bytes-0.1.0/README.md` & `drift-bytes-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -17,31 +17,41 @@
 ## Requirements
 
 * CMake >= 3.16
 * C++17 compiler
 * conan >= 1.56, < 2.0
 
 
+## Bindings
+
+* [Python](python/README.md)
+
 ## Usage Example
 
 ```c++
 #include <drift_bytes/bytes.h>
 
 #include <iostream>
 
-using drift_bytes::Bytes;
+using drift_bytes::InputBuffer;
+using drift_bytes::OutputBuffer;
+using drift_bytes::Variant;
 
 int main() {
-    uint8_t val{42};
-    auto bytes = Bytes();
-    bytes.scalar(val);
-    auto new_val = bytes.scalar<uint8_t>();
+  Variant some_value{42};
+
+  OutputBuffer buffer;
+  buffer.push_back(some_value);
 
-    std::cout << new_val << std::endl;
+  InputBuffer input(buffer.str());
+  Variant new_val = input.pop();
+
+  std::cout << new_val << std::endl;
 }
+
 ```
 
 ## Bulding
 
 ```bash
 mkdir build && cd build
 conan install ../conan --build=missing -of .
```

### Comparing `drift-bytes-0.1.0/conan/conanfile.py` & `drift-bytes-0.2.0/conan/conanfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from conan.tools.cmake import CMake, CMakeToolchain, cmake_layout
 
 required_conan_version = ">=1.58"
 
 
 class WaveletBufferConan(ConanFile):
     name = "drift_bytes"
-    version = "0.1.0"
+    version = "0.2.0"
     license = "MPL-2.0"
     author = "PANDA GmbH"
     description = "A serializer for typed data in the Drift infrastructure"
     url = "https://github.com/panda-official/DriftBytes"
     default_options = {
         "shared": False,
         "fPIC": True,
```

### Comparing `drift-bytes-0.1.0/conan/test_package/conanfile.py` & `drift-bytes-0.2.0/conan/test_package/conanfile.py`

 * *Files identical despite different names*

### Comparing `drift-bytes-0.1.0/pyproject.toml` & `drift-bytes-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 [tool.cibuildwheel.linux]
 archs = "x86_64"
 environment-pass = ["VERSION_SUFFIX"]
 
 [tool.pylint.MASTER]
 good-names = "b"
+extension-pkg-allow-list = ["pybind11", "drift_bytes._drift_bytes"]
```

### Comparing `drift-bytes-0.1.0/python/CMakeLists.txt` & `drift-bytes-0.2.0/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `drift-bytes-0.1.0/python/src/drift_bytes.egg-info/PKG-INFO` & `drift-bytes-0.2.0/python/src/drift_bytes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drift-bytes
-Version: 0.1.0
+Version: 0.2.0
 Summary: A serializer for typed data in the Drift infrastructure.
 Home-page: https://github.com/panda-official/DriftBytes
 Author: PANDA, GmbH
 Author-email: info@panda.technology
 License: MPL-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `drift-bytes-0.1.0/python/src/drift_bytes.egg-info/SOURCES.txt` & `drift-bytes-0.2.0/python/src/drift_bytes.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 python/src/main.cc
 python/src/drift_bytes/__init__.py
 python/src/drift_bytes/bytes.py
 python/src/drift_bytes.egg-info/PKG-INFO
 python/src/drift_bytes.egg-info/SOURCES.txt
 python/src/drift_bytes.egg-info/dependency_links.txt
 python/src/drift_bytes.egg-info/top_level.txt
-python/tests/test_bytes.py
-python/tests/test_bytes_scalars.py
-python/tests/test_bytes_vectors.py
+python/tests/__init__.py
+python/tests/test_buffers.py
+python/tests/test_variant.py
 tests/CMakeLists.txt
 tests/bytes_test.cc
```

### Comparing `drift-bytes-0.1.0/setup.py` & `drift-bytes-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "python" / "README.md").read_text()
 
 MAJOR_VERSION = 0
-MINOR_VERSION = 1
+MINOR_VERSION = 2
 PATCH_VERSION = 0
 
 PACKAGE_NAME = "drift-bytes"
 
 VERSION_SUFFIX = os.getenv("VERSION_SUFFIX")
```

