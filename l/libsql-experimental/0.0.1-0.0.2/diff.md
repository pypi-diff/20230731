# Comparing `tmp/libsql_experimental-0.0.1.tar.gz` & `tmp/libsql_experimental-0.0.2.tar.gz`

## Comparing `libsql_experimental-0.0.1.tar` & `libsql_experimental-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 libsql_experimental-0.0.1/Cargo.toml
--rw-r--r--   0     1001      123     2040 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123       12 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/.gitignore
--rw-r--r--   0     1001      123      877 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/README.md
--rw-r--r--   0     1001      123       10 2023-07-27 10:52:33.000000 libsql_experimental-0.0.1/dist/libsql_experimental-0.0.1.tar.gz
--rw-r--r--   0     1001      123      271 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/example.py
--rwxr-xr-x   0     1001      123      278 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/perf-libsql.py
--rwxr-xr-x   0     1001      123      254 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/perf-sqlite3.py
--rw-r--r--   0     1001      123      379 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/pyproject.toml
--rw-r--r--   0     1001      123     3861 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/src/lib.rs
--rw-r--r--   0     1001      123     1102 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/tests/test_basic.py
--rw-r--r--   0     1001      123    43394 2023-07-27 10:50:46.000000 libsql_experimental-0.0.1/Cargo.lock
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 libsql_experimental-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 libsql_experimental-0.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     2040 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123       12 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/.gitignore
+-rw-r--r--   0     1001      123      877 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/README.md
+-rw-r--r--   0     1001      123       10 2023-07-31 09:17:03.000000 libsql_experimental-0.0.2/dist/libsql_experimental-0.0.2.tar.gz
+-rw-r--r--   0     1001      123      271 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/example.py
+-rwxr-xr-x   0     1001      123      278 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/perf-libsql.py
+-rwxr-xr-x   0     1001      123      254 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/perf-sqlite3.py
+-rw-r--r--   0     1001      123      379 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/pyproject.toml
+-rw-r--r--   0     1001      123     3859 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     1102 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/tests/test_basic.py
+-rw-r--r--   0     1001      123    43394 2023-07-31 09:17:00.000000 libsql_experimental-0.0.2/Cargo.lock
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 libsql_experimental-0.0.2/PKG-INFO
```

### Comparing `libsql_experimental-0.0.1/.github/workflows/CI.yml` & `libsql_experimental-0.0.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.1/README.md` & `libsql_experimental-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.1/src/lib.rs` & `libsql_experimental-0.0.2/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         let params: libsql_core::Params = match parameters {
             Some(parameters) => {
                 let mut params = vec![];
                 for parameter in parameters.iter() {
                     let param = match parameter.extract::<i32>() {
                         Ok(value) => libsql_core::Value::Integer(value as i64),
                         Err(_) => match parameter.extract::<f64>() {
-                            Ok(value) => libsql_core::Value::Float(value),
+                            Ok(value) => libsql_core::Value::Real(value),
                             Err(_) => match parameter.extract::<&str>() {
                                 Ok(value) => libsql_core::Value::Text(value.to_string()),
                                 Err(_) => todo!(),
                             },
                         },
                     };
                     params.push(param);
@@ -81,15 +81,15 @@
                         for col_idx in 0..rows.column_count() {
                             let col_type = row.column_type(col_idx).map_err(to_py_err)?;
                             let value = match col_type {
                                 libsql_core::ValueType::Integer => {
                                     let value = row.get::<i32>(col_idx).map_err(to_py_err)?;
                                     value.into_py(self_.py())
                                 }
-                                libsql_core::ValueType::Float => todo!(),
+                                libsql_core::ValueType::Real => todo!(),
                                 libsql_core::ValueType::Blob => todo!(),
                                 libsql_core::ValueType::Text => {
                                     let value = row.get::<&str>(col_idx).map_err(to_py_err)?;
                                     value.into_py(self_.py())
                                 }
                                 libsql_core::ValueType::Null => todo!(),
                             };
```

### Comparing `libsql_experimental-0.0.1/tests/test_basic.py` & `libsql_experimental-0.0.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.1/Cargo.lock` & `libsql_experimental-0.0.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -578,51 +578,51 @@
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libsql"
-version = "0.1.5"
-source = "git+https://github.com/libsql/libsql/?rev=09fb0a4ded17fb4395187716feb6ae429839ea7e#09fb0a4ded17fb4395187716feb6ae429839ea7e"
+version = "0.1.6"
+source = "git+https://github.com/libsql/libsql/?rev=36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed#36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed"
 dependencies = [
  "futures",
  "libsql-sys",
  "libsql_replication",
  "parking_lot",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "libsql-python"
-version = "0.0.1"
+version = "0.0.2"
 dependencies = [
  "libsql",
  "pyo3",
 ]
 
 [[package]]
 name = "libsql-sys"
-version = "0.2.10"
-source = "git+https://github.com/libsql/libsql/?rev=09fb0a4ded17fb4395187716feb6ae429839ea7e#09fb0a4ded17fb4395187716feb6ae429839ea7e"
+version = "0.2.11"
+source = "git+https://github.com/libsql/libsql/?rev=36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed#36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed"
 dependencies = [
  "bindgen",
  "cc",
  "default-env",
  "once_cell",
  "tracing",
 ]
 
 [[package]]
 name = "libsql_replication"
 version = "0.0.2"
-source = "git+https://github.com/libsql/libsql/?rev=09fb0a4ded17fb4395187716feb6ae429839ea7e#09fb0a4ded17fb4395187716feb6ae429839ea7e"
+source = "git+https://github.com/libsql/libsql/?rev=36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed#36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed"
 dependencies = [
  "anyhow",
  "bytemuck",
  "bytes",
  "crossbeam",
  "futures",
  "libsql-sys",
```

### Comparing `libsql_experimental-0.0.1/PKG-INFO` & `libsql_experimental-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsql-experimental
-Version: 0.0.1
+Version: 0.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # libSQL API for Python
```

