# Comparing `tmp/ulid_rs_py-0.1.1.tar.gz` & `tmp/ulid_rs_py-0.1.2.tar.gz`

## Comparing `ulid_rs_py-0.1.1.tar` & `ulid_rs_py-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.1/Cargo.toml
--rw-r--r--   0     1001      123    14851 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/Cargo.lock
--rw-r--r--   0     1001      123     1063 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/LICENSE
--rw-r--r--   0     1001      123     1643 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/README.md
--rw-r--r--   0     1001      123     1385 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/pyproject.toml
--rw-r--r--   0     1001      123     3622 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/src/lib.rs
--rw-r--r--   0     1001      123      674 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/README.md
--rw-r--r--   0     1001      123        0 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/__init__.py
--rw-r--r--   0     1001      123     2142 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/benchmark.py
--rw-r--r--   0     1001      123    32004 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_str.svg
--rw-r--r--   0     1001      123    31573 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_timestamp.svg
--rw-r--r--   0     1001      123    31374 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_uuid.svg
--rw-r--r--   0     1001      123    30691 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-new.svg
--rw-r--r--   0     1001      123     2303 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/test_ulid.py
--rw-r--r--   0     1001      123      157 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/__init__.py
--rw-r--r--   0     1001      123       22 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/__version__.py
--rw-r--r--   0     1001      123      606 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/_ulid_rs_py.pyi
--rw-r--r--   0     1001      123        0 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/py.typed
--rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      123    14851 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      123     1063 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/LICENSE
+-rw-r--r--   0     1001      123     1691 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/README.md
+-rw-r--r--   0     1001      123     1382 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      123     3622 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      123      674 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/README.md
+-rw-r--r--   0     1001      123        0 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123     2142 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/benchmark.py
+-rw-r--r--   0     1001      123    32004 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_str.svg
+-rw-r--r--   0     1001      123    31573 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_timestamp.svg
+-rw-r--r--   0     1001      123    31374 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_uuid.svg
+-rw-r--r--   0     1001      123    30691 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-new.svg
+-rw-r--r--   0     1001      123     2303 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/tests/test_ulid.py
+-rw-r--r--   0     1001      123      157 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/ulid/__init__.py
+-rw-r--r--   0     1001      123       22 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/ulid/__version__.py
+-rw-r--r--   0     1001      123      606 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/ulid/_ulid_rs_py.pyi
+-rw-r--r--   0     1001      123        0 2023-07-31 06:26:35.000000 ulid_rs_py-0.1.2/ulid/py.typed
+-rw-r--r--   0        0        0     3165 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.2/PKG-INFO
```

### Comparing `ulid_rs_py-0.1.1/Cargo.toml` & `ulid_rs_py-0.1.2/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "ulid-rs-py"
-version = "0.1.1"
+version = "0.1.2"
 description = "Use rust ulid crate to rewrite python ulid library"
 authors = [
     "vvanglro <vvanglro@gmail.com>"
 ]
 license = "MIT"
 edition = "2021"
 keywords = ["ulid"]
 
 readme = "README.md"
-homepage = "https://github.com/vvanglro/ulid-rs-py"
-repository = "https://github.com/vvanglro/ulid-rs-py"
+homepage = "https://github.com/rp-libs/ulid-rs-py"
+repository = "https://github.com/rp-libs/ulid-rs-py"
 
 include = [
     "/Cargo.toml",
     "/pyproject.toml",
     "/LICENSE",
     "/README.md",
     "/src",
```

### Comparing `ulid_rs_py-0.1.1/Cargo.lock` & `ulid_rs_py-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 dependencies = [
  "rand",
  "uuid",
 ]
 
 [[package]]
 name = "ulid-rs-py"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "chrono",
  "pyo3",
  "pyo3-build-config",
  "ulid",
  "uuid",
 ]
```

### Comparing `ulid_rs_py-0.1.1/LICENSE` & `ulid_rs_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/README.md` & `ulid_rs_py-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,8 +59,8 @@
 assert py_ulid.str() == py_ulid_tt.str()
 
 ```
 
 ---
 
 ## Benchmarks
-For details, see [benchmark](tests/benchmarks/README.md).
+For details, see [benchmark](https://github.com/rp-libs/ulid-rs-py/blob/main/tests/benchmarks/README.md).
```

### Comparing `ulid_rs_py-0.1.1/pyproject.toml` & `ulid_rs_py-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     "license",
     "readme",
     "version"
 ]
 requires-python = ">=3.8"
 
 [project.urls]
-Homepage = "https://github.com/vvanglro/ulid-rs-py"
-Funding = "https://github.com/vvanglro/ulid-rs-py"
-Source = "https://github.com/vvanglro/ulid-rs-py"
+Homepage = "https://github.com/rp-libs/ulid-rs-py"
+Funding = "https://github.com/rp-libs/ulid-rs-py"
+Source = "https://github.com/rp-libs/ulid-rs-py"
 
 [project.optional-dependencies]
 test = [
     "pytest~=7.1.2"
 ]
 
 [tool.maturin]
```

### Comparing `ulid_rs_py-0.1.1/src/lib.rs` & `ulid_rs_py-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/README.md` & `ulid_rs_py-0.1.2/tests/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/benchmark.py` & `ulid_rs_py-0.1.2/tests/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_str.svg` & `ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_str.svg`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_timestamp.svg` & `ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_timestamp.svg`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_uuid.svg` & `ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-from_uuid.svg`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-new.svg` & `ulid_rs_py-0.1.2/tests/benchmarks/result/benchmark_20230728_090826-new.svg`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/tests/test_ulid.py` & `ulid_rs_py-0.1.2/tests/test_ulid.py`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/ulid/_ulid_rs_py.pyi` & `ulid_rs_py-0.1.2/ulid/_ulid_rs_py.pyi`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.1/PKG-INFO` & `ulid_rs_py-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ulid-rs-py
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
@@ -18,23 +18,23 @@
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pytest ~=7.1.2 ; extra == 'test'
 Provides-Extra: test
 License-File: LICENSE
 Summary: Use rust ulid crate to rewrite python ulid library
 Keywords: ulid
-Home-Page: https://github.com/vvanglro/ulid-rs-py
+Home-Page: https://github.com/rp-libs/ulid-rs-py
 Author: vvanglro <vvanglro@gmail.com>
 Author-email: vvanglro <vvanglro@gmail.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Homepage, https://github.com/vvanglro/ulid-rs-py
-Project-URL: Funding, https://github.com/vvanglro/ulid-rs-py
-Project-URL: Source, https://github.com/vvanglro/ulid-rs-py
+Project-URL: Homepage, https://github.com/rp-libs/ulid-rs-py
+Project-URL: Funding, https://github.com/rp-libs/ulid-rs-py
+Project-URL: Source, https://github.com/rp-libs/ulid-rs-py
 
 # ulid-rs-py
 
 [![Package version](https://img.shields.io/pypi/v/ulid-rs-py?color=%2334D058&label=pypi%20package)](https://pypi.org/project/ulid-rs-py/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/ulid-rs-py.svg?color=%2334D058)](https://pypi.org/project/ulid-rs-py/)
 
 Use rust ulid crate to rewrite python ulid library.
@@ -93,9 +93,9 @@
 assert py_ulid.str() == py_ulid_tt.str()
 
 ```
 
 ---
 
 ## Benchmarks
-For details, see [benchmark](tests/benchmarks/README.md).
+For details, see [benchmark](https://github.com/rp-libs/ulid-rs-py/blob/main/tests/benchmarks/README.md).
```

