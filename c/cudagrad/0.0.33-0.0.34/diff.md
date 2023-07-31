# Comparing `tmp/cudagrad-0.0.33.tar.gz` & `tmp/cudagrad-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.33.tar", last modified: Sat Jul 29 20:03:05 2023, max compression
+gzip compressed data, was "cudagrad-0.0.34.tar", last modified: Mon Jul 31 02:04:30 2023, max compression
```

## Comparing `cudagrad-0.0.33.tar` & `cudagrad-0.0.34.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.302396 cudagrad-0.0.33/
--rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-29 19:31:23.000000 cudagrad-0.0.33/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 20:03:05.302240 cudagrad-0.0.33/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3157 2023-07-28 03:27:33.000000 cudagrad-0.0.33/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.299239 cudagrad-0.0.33/cudagrad/
--rw-r--r--   0 ryan       (501) staff       (20)      131 2023-07-29 20:02:43.000000 cudagrad-0.0.33/cudagrad/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     5925 2023-07-27 03:50:10.000000 cudagrad-0.0.33/cudagrad/mlp.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.300230 cudagrad-0.0.33/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3660 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.33/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-29 20:03:05.000000 cudagrad-0.0.33/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-29 20:02:43.000000 cudagrad-0.0.33/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-29 20:03:05.302499 cudagrad-0.0.33/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.33/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.301491 cudagrad-0.0.33/src/
--rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.33/src/bindings.cpp
--rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.33/src/cudagrad.hpp
--rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.33/src/ops.cu
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-29 20:03:05.301797 cudagrad-0.0.33/tests/
--rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.33/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.017207 cudagrad-0.0.34/
+-rw-r--r--   0 ryan       (501) staff       (20)       44 2023-07-29 19:31:23.000000 cudagrad-0.0.34/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3662 2023-07-31 02:04:30.017089 cudagrad-0.0.34/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     3159 2023-07-29 20:12:25.000000 cudagrad-0.0.34/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.014887 cudagrad-0.0.34/cudagrad/
+-rw-r--r--   0 ryan       (501) staff       (20)      131 2023-07-31 02:04:13.000000 cudagrad-0.0.34/cudagrad/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5852 2023-07-31 02:00:43.000000 cudagrad-0.0.34/cudagrad/mlp.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.015724 cudagrad-0.0.34/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3662 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      331 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-27 00:32:51.000000 cudagrad-0.0.34/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-31 02:04:29.000000 cudagrad-0.0.34/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      984 2023-07-31 02:04:13.000000 cudagrad-0.0.34/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-31 02:04:30.017250 cudagrad-0.0.34/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1659 2023-07-27 00:49:51.000000 cudagrad-0.0.34/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.016532 cudagrad-0.0.34/src/
+-rw-r--r--   0 ryan       (501) staff       (20)     2910 2023-07-29 19:18:45.000000 cudagrad-0.0.34/src/bindings.cpp
+-rw-r--r--   0 ryan       (501) staff       (20)    20457 2023-07-29 19:17:36.000000 cudagrad-0.0.34/src/cudagrad.hpp
+-rw-r--r--   0 ryan       (501) staff       (20)      254 2023-07-29 18:53:13.000000 cudagrad-0.0.34/src/ops.cu
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-31 02:04:30.016807 cudagrad-0.0.34/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)     1083 2023-07-29 16:33:01.000000 cudagrad-0.0.34/tests/test.py
```

### Comparing `cudagrad-0.0.33/PKG-INFO` & `cudagrad-0.0.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.33
+Version: 0.0.34
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
-  auto e = (cg::matmul(a, b) + c) * d;
+  auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
   using namespace std;
   for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
   for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
   for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
```

### Comparing `cudagrad-0.0.33/README.md` & `cudagrad-0.0.34/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
-  auto e = (cg::matmul(a, b) + c) * d;
+  auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
   using namespace std;
   for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
   for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
   for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
```

### Comparing `cudagrad-0.0.33/cudagrad/mlp.py` & `cudagrad-0.0.34/cudagrad/mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # type: ignore
 # %%
 import random
 from typing import *  # type: ignore
 
-import matplotlib.pyplot as plt
-import numpy as np
-
 from .cudagrad_bindings import *  # type: ignore
 
 # %matplotlib inline
 
-np.random.seed(1337)
 random.seed(1337)
 
 from micrograd.engine import Value
 from micrograd.nn import MLP, Layer, Neuron
 
 # %%
 if __name__ == "__main__":
```

### Comparing `cudagrad-0.0.33/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.34/cudagrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.33
+Version: 0.0.34
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <ryanm.inbox@gmail.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
@@ -25,15 +25,15 @@
 // c++ -std=c++11 -I./src examples/example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
-  auto e = (cg::matmul(a, b) + c) * d;
+  auto e = (a.get()->matmul(b) + c) * d;
   auto f = e.get()->sum();
   f.get()->backward();
 
   using namespace std;
   for (auto& x : f.get()->data_) {cout<<x<<" ";} // 2794
   for (auto& x : f.get()->size_) {cout<<x<<" ";} // 1
   for (auto& x : a.get()->grad_) {cout<<x<<" ";} // 143 187 143 187
```

### Comparing `cudagrad-0.0.33/pyproject.toml` & `cudagrad-0.0.34/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=40.8.0", "wheel", "pybind11>=2.10.1", "toml",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.33"
+version = "0.0.34"
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "Operating System :: OS Independent",]
 # TEMP while we implement mlp
 dependencies = [ "micrograd",]
 [[project.authors]]
```

### Comparing `cudagrad-0.0.33/setup.py` & `cudagrad-0.0.34/setup.py`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.33/src/bindings.cpp` & `cudagrad-0.0.34/src/bindings.cpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.33/src/cudagrad.hpp` & `cudagrad-0.0.34/src/cudagrad.hpp`

 * *Files identical despite different names*

### Comparing `cudagrad-0.0.33/tests/test.py` & `cudagrad-0.0.34/tests/test.py`

 * *Files identical despite different names*

