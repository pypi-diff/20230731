# Comparing `tmp/ulid_rs_py-0.1.0.tar.gz` & `tmp/ulid_rs_py-0.1.1.tar.gz`

## Comparing `ulid_rs_py-0.1.0.tar` & `ulid_rs_py-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,19 @@
--rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123    14851 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/Cargo.lock
--rw-r--r--   0     1001      123     1063 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/LICENSE
--rw-r--r--   0     1001      123       65 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/README.md
--rw-r--r--   0     1001      123     1385 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     3619 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     2303 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/tests/test_ulid.py
--rw-r--r--   0     1001      123      157 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/ulid/__init__.py
--rw-r--r--   0     1001      123       22 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/ulid/__version__.py
--rw-r--r--   0     1001      123      606 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/ulid/_ulid_rs_py.pyi
--rw-r--r--   0     1001      123        0 2023-07-27 11:34:30.000000 ulid_rs_py-0.1.0/ulid/py.typed
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.1/Cargo.toml
+-rw-r--r--   0     1001      123    14851 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/Cargo.lock
+-rw-r--r--   0     1001      123     1063 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/LICENSE
+-rw-r--r--   0     1001      123     1643 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/README.md
+-rw-r--r--   0     1001      123     1385 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/pyproject.toml
+-rw-r--r--   0     1001      123     3622 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/src/lib.rs
+-rw-r--r--   0     1001      123      674 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/README.md
+-rw-r--r--   0     1001      123        0 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/__init__.py
+-rw-r--r--   0     1001      123     2142 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/benchmark.py
+-rw-r--r--   0     1001      123    32004 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_str.svg
+-rw-r--r--   0     1001      123    31573 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_timestamp.svg
+-rw-r--r--   0     1001      123    31374 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-from_uuid.svg
+-rw-r--r--   0     1001      123    30691 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/benchmarks/result/benchmark_20230728_090826-new.svg
+-rw-r--r--   0     1001      123     2303 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/tests/test_ulid.py
+-rw-r--r--   0     1001      123      157 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/__init__.py
+-rw-r--r--   0     1001      123       22 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/__version__.py
+-rw-r--r--   0     1001      123      606 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/_ulid_rs_py.pyi
+-rw-r--r--   0     1001      123        0 2023-07-31 05:03:21.000000 ulid_rs_py-0.1.1/ulid/py.typed
+-rw-r--r--   0        0        0     3121 1970-01-01 00:00:00.000000 ulid_rs_py-0.1.1/PKG-INFO
```

### Comparing `ulid_rs_py-0.1.0/Cargo.toml` & `ulid_rs_py-0.1.1/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ulid-rs-py"
-version = "0.1.0"
+version = "0.1.1"
 description = "Use rust ulid crate to rewrite python ulid library"
 authors = [
     "vvanglro <vvanglro@gmail.com>"
 ]
 license = "MIT"
 edition = "2021"
 keywords = ["ulid"]
```

### Comparing `ulid_rs_py-0.1.0/Cargo.lock` & `ulid_rs_py-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
 dependencies = [
  "rand",
  "uuid",
 ]
 
 [[package]]
 name = "ulid-rs-py"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "chrono",
  "pyo3",
  "pyo3-build-config",
  "ulid",
  "uuid",
 ]
```

### Comparing `ulid_rs_py-0.1.0/LICENSE` & `ulid_rs_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.0/pyproject.toml` & `ulid_rs_py-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.0/src/lib.rs` & `ulid_rs_py-0.1.1/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use chrono::{Timelike, TimeZone, Utc};
+use chrono::{TimeZone, Timelike, Utc};
 use pyo3::create_exception;
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use pyo3::types::{PyDateAccess, PyDateTime, PyTimeAccess};
 use ulid::Ulid;
 use uuid::Uuid;
 
@@ -21,15 +21,15 @@
 #[pymethods]
 impl PyUlid {
     pub fn __repr__(&self) -> PyResult<String> {
         Ok(format!("<ULID('{}')>", self.0.to_string()))
     }
 
     pub fn bytes(&self) -> PyResult<[u8; 16]> {
-        Ok(self.0.0.to_be_bytes())
+        Ok(self.0 .0.to_be_bytes())
     }
 
     pub fn timestamp(&self) -> PyResult<u64> {
         Ok(self.0.timestamp_ms())
     }
 
     pub fn randomness(&self) -> PyResult<u128> {
@@ -39,15 +39,15 @@
     pub fn str(&self) -> PyResult<String> {
         Ok(self.0.to_string())
     }
 
     pub fn increment(&self) -> PyResult<Option<PyUlid>> {
         match self.0.increment() {
             None => Ok(None),
-            Some(resp) => { Ok(Option::from(self::PyUlid::new(resp))) }
+            Some(resp) => Ok(Option::from(self::PyUlid::new(resp))),
         }
     }
 }
 
 #[pyfunction]
 fn new(_py: Python) -> PyResult<PyUlid> {
     _py.allow_threads(|| {
@@ -57,41 +57,41 @@
 }
 
 #[pyfunction]
 #[pyo3(signature = (value))]
 fn from_string(_py: Python, value: &str) -> PyResult<PyUlid> {
     match _py.allow_threads(|| Ulid::from_string(&value)) {
         Ok(ulid_result) => Ok(PyUlid::new(ulid_result)),
-        Err(err) => Err(DecodeError::new_err(err.to_string()))
+        Err(err) => Err(DecodeError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (value))]
 fn from_uuid(_py: Python, value: &str) -> PyResult<PyUlid> {
     match _py.allow_threads(|| Uuid::parse_str(&value)) {
-        Ok(instance_uuid) => {
-            Ok(PyUlid::new(ulid::Ulid::from(instance_uuid)))
-        }
-        Err(err) => Err(InvalidUuidError::new_err(err.to_string()))
+        Ok(instance_uuid) => Ok(PyUlid::new(ulid::Ulid::from(instance_uuid))),
+        Err(err) => Err(InvalidUuidError::new_err(err.to_string())),
     }
 }
 
 #[pyfunction]
 #[pyo3(signature = (value))]
 fn from_timestamp(_py: Python, value: &PyDateTime) -> PyResult<PyUlid> {
     let year = value.get_year();
     let month = value.get_month() as u32;
     let day = value.get_day() as u32;
     let hour = value.get_hour() as u32;
     let minute = value.get_minute() as u32;
     let second = value.get_second() as u32;
     let microsecond = value.get_microsecond() as u32;
     _py.allow_threads(|| {
-        let dt = Utc.with_ymd_and_hms(year, month, day, hour, minute, second).unwrap()
+        let dt = Utc
+            .with_ymd_and_hms(year, month, day, hour, minute, second)
+            .unwrap()
             .with_nanosecond(microsecond)
             .unwrap();
         let system_time = dt.into();
         let ulid = Ulid::from_datetime(system_time);
         Ok(PyUlid::new(ulid))
     })
 }
```

### Comparing `ulid_rs_py-0.1.0/tests/test_ulid.py` & `ulid_rs_py-0.1.1/tests/test_ulid.py`

 * *Files identical despite different names*

### Comparing `ulid_rs_py-0.1.0/ulid/_ulid_rs_py.pyi` & `ulid_rs_py-0.1.1/ulid/_ulid_rs_py.pyi`

 * *Files identical despite different names*

