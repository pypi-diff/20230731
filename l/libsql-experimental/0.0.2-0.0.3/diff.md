# Comparing `tmp/libsql_experimental-0.0.2.tar.gz` & `tmp/libsql_experimental-0.0.3.tar.gz`

## Comparing `libsql_experimental-0.0.2.tar` & `libsql_experimental-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      265 1970-01-01 00:00:00.000000 libsql_experimental-0.0.2/Cargo.toml
--rw-r--r--   0     1001      123     2040 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123       12 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/.gitignore
--rw-r--r--   0     1001      123      877 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/README.md
--rw-r--r--   0     1001      123       10 2023-07-31 09:17:03.000000 libsql_experimental-0.0.2/dist/libsql_experimental-0.0.2.tar.gz
--rw-r--r--   0     1001      123      271 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/example.py
--rwxr-xr-x   0     1001      123      278 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/perf-libsql.py
--rwxr-xr-x   0     1001      123      254 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/perf-sqlite3.py
--rw-r--r--   0     1001      123      379 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/pyproject.toml
--rw-r--r--   0     1001      123     3859 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/src/lib.rs
--rw-r--r--   0     1001      123     1102 2023-07-31 09:15:21.000000 libsql_experimental-0.0.2/tests/test_basic.py
--rw-r--r--   0     1001      123    43394 2023-07-31 09:17:00.000000 libsql_experimental-0.0.2/Cargo.lock
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 libsql_experimental-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 libsql_experimental-0.0.3/Cargo.toml
+-rw-r--r--   0     1001      123     2040 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123       12 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/LICENSE.md
+-rw-r--r--   0     1001      123     2436 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/README.md
+-rw-r--r--   0     1001      123       10 2023-07-31 09:44:03.000000 libsql_experimental-0.0.3/dist/libsql_experimental-0.0.3.tar.gz
+-rw-r--r--   0     1001      123      271 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/example.py
+-rwxr-xr-x   0     1001      123      278 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/perf-libsql.py
+-rwxr-xr-x   0     1001      123      254 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/perf-sqlite3.py
+-rw-r--r--   0     1001      123      379 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/pyproject.toml
+-rw-r--r--   0     1001      123     4419 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/src/lib.rs
+-rw-r--r--   0     1001      123     1102 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/tests/test_basic.py
+-rw-r--r--   0     1001      123    43847 2023-07-31 09:42:21.000000 libsql_experimental-0.0.3/Cargo.lock
+-rw-r--r--   0        0        0     2799 1970-01-01 00:00:00.000000 libsql_experimental-0.0.3/PKG-INFO
```

### Comparing `libsql_experimental-0.0.2/.github/workflows/CI.yml` & `libsql_experimental-0.0.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.2/src/lib.rs` & `libsql_experimental-0.0.3/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,44 @@
 use ::libsql as libsql_core;
 
 fn to_py_err(error: libsql_core::errors::Error) -> PyErr {
     PyValueError::new_err(format!("{}", error))
 }
 
 #[pyfunction]
-fn connect(url: String) -> PyResult<Connection> {
-    let db = libsql_core::Database::open(url).map_err(to_py_err)?;
-    Ok(Connection { db })
+#[pyo3(signature = (database, sync_url=None))]
+fn connect(database: String, sync_url: Option<String>) -> PyResult<Connection> {
+    let rt = tokio::runtime::Runtime::new().unwrap();
+    let db = match sync_url {
+        Some(sync_url) => {
+            let opts = libsql_core::Opts::with_http_sync(sync_url);
+            rt.block_on(libsql_core::Database::open_with_opts(database, opts)).map_err(to_py_err)?
+        },
+        None => libsql_core::Database::open(database).map_err(to_py_err)?,
+    };
+    Ok(Connection { db, rt })
 }
 
 #[pyclass]
 pub struct Connection {
     db: libsql_core::Database,
+    rt: tokio::runtime::Runtime,
 }
 
 #[pymethods]
 impl Connection {
     fn cursor(self_: PyRef<'_, Self>) -> PyResult<Cursor> {
         let conn = self_.db.connect().map_err(to_py_err)?;
         Ok(Cursor { conn })
     }
+
+    fn sync(self_: PyRef<'_, Self>) -> PyResult<()> {
+        self_.rt.block_on(self_.db.sync()).map_err(to_py_err)?;
+        Ok(())
+    }
 }
 
 #[pyclass]
 pub struct Cursor {
     conn: libsql_core::Connection,
 }
```

### Comparing `libsql_experimental-0.0.2/tests/test_basic.py` & `libsql_experimental-0.0.3/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `libsql_experimental-0.0.2/Cargo.lock` & `libsql_experimental-0.0.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -430,14 +430,20 @@
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+
+[[package]]
 name = "http"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
 dependencies = [
  "bytes",
  "fnv",
@@ -593,18 +599,19 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "libsql-python"
-version = "0.0.2"
+version = "0.0.3"
 dependencies = [
  "libsql",
  "pyo3",
+ "tokio",
 ]
 
 [[package]]
 name = "libsql-sys"
 version = "0.2.11"
 source = "git+https://github.com/libsql/libsql/?rev=36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed#36ff3f38f6fd90ceb48a6bf5bffcf0bb996485ed"
 dependencies = [
@@ -761,14 +768,24 @@
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
+name = "num_cpus"
+version = "1.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
+dependencies = [
+ "hermit-abi",
+ "libc",
+]
+
+[[package]]
 name = "object"
 version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bda667d9f2b5051b8833f59f3bf748b28ef54f850f4fcb389a252aa383866d1"
 dependencies = [
  "memchr",
 ]
@@ -1307,14 +1324,15 @@
 checksum = "532826ff75199d5833b9d2c5fe410f29235e25704ee5f0ef599fb51c21f4a4da"
 dependencies = [
  "autocfg",
  "backtrace",
  "bytes",
  "libc",
  "mio",
+ "num_cpus",
  "pin-project-lite",
  "socket2",
  "tokio-macros",
  "windows-sys",
 ]
 
 [[package]]
```

