# Comparing `tmp/pydozer_log-0.1.27-pp39-pypy39_pp73-manylinux_2_34_s390x.whl.zip` & `tmp/pydozer_log-0.1.31-pp39-pypy39_pp73-manylinux_2_34_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1901426 bytes, number of entries: 5
--rw-r--r--  4.6 unx     2020 b- defN 23-Jun-30 12:15 pydozer_log-0.1.27.dist-info/METADATA
--rw-r--r--  4.6 unx      112 b- defN 23-Jun-30 12:15 pydozer_log-0.1.27.dist-info/WHEEL
--rw-r--r--  4.6 unx      127 b- defN 23-Jun-30 12:15 pydozer_log/__init__.py
--rwxr-xr-x  4.6 unx  7871200 b- defN 23-Jun-30 12:15 pydozer_log/pydozer_log.pypy39-pp73-s390x-linux-gnu.so
--rw-r--r--  4.6 unx      415 b- defN 23-Jun-30 12:15 pydozer_log-0.1.27.dist-info/RECORD
-5 files, 7873874 bytes uncompressed, 1900658 bytes compressed:  75.9%
+Zip file size: 7815012 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2102 b- defN 23-Jul-31 01:08 pydozer_log-0.1.31.dist-info/METADATA
+-rw-r--r--  4.6 unx      111 b- defN 23-Jul-31 01:08 pydozer_log-0.1.31.dist-info/WHEEL
+-rw-r--r--  4.6 unx      127 b- defN 23-Jul-31 01:08 pydozer_log/__init__.py
+-rwxr-xr-x  4.6 unx 22953328 b- defN 23-Jul-31 01:08 pydozer_log/pydozer_log.pypy39-pp73-x86-linux-gnu.so
+-rw-r--r--  4.6 unx      414 b- defN 23-Jul-31 01:08 pydozer_log-0.1.31.dist-info/RECORD
+5 files, 22956082 bytes uncompressed, 7814248 bytes compressed:  66.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: pydozer_log-0.1.27.dist-info/METADATA
+Filename: pydozer_log-0.1.31.dist-info/METADATA
 Comment: 
 
-Filename: pydozer_log-0.1.27.dist-info/WHEEL
+Filename: pydozer_log-0.1.31.dist-info/WHEEL
 Comment: 
 
 Filename: pydozer_log/__init__.py
 Comment: 
 
-Filename: pydozer_log/pydozer_log.pypy39-pp73-s390x-linux-gnu.so
+Filename: pydozer_log/pydozer_log.pypy39-pp73-x86-linux-gnu.so
 Comment: 
 
-Filename: pydozer_log-0.1.27.dist-info/RECORD
+Filename: pydozer_log-0.1.31.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pydozer_log-0.1.27.dist-info/METADATA` & `pydozer_log-0.1.31.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydozer_log
-Version: 0.1.27
+Version: 0.1.31
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # dozer-log-python
@@ -13,15 +13,15 @@
 
 ## Installation
 
 `pip install pydozer_log`
 
 ### Troubleshoot
 
-This library contains native code so have limited platform support. 
+This library contains native code so have limited platform support.
 
 If above command gives you:
 
 ```text
 ERROR: Could not find a version that satisfies the requirement pydozer_log (from versions: none)
 ERROR: No matching distribution found for pydozer_log
 ```
@@ -30,20 +30,20 @@
 
 As a general rule, we support CPython >= 3.10 on Windows, MacOS and Linux, both amd and arm architectures. Meanwhile, some other versions of PyPy and CPython with certain platform combinations are also supported.
 
 To see all supported platforms, please check the file list at <https://pypi.org/project/pydozer-log/#files>.
 
 ## Usage
 
-Assume your Dozer home directory is `.dozer` and you have an endpoint named `trips`. You can read the Dozer logs in Python as follows:
+Assume your have Dozer running and the app is listening to `http://127.0.0.1:50053`, and you have an endpoint named `trips`. You can read the Dozer logs in Python as follows:
 
 ```python
 import pydozer_log
 
-reader = await pydozer_log.LogReader.new('.dozer', 'trips')
+reader = await pydozer_log.LogReader.new('http://127.0.0.1:50053', 'trips')
 print(await reader.next_op())
 ```
 
 ## Develop
 
 Install `maturin` in your Python environment:
 
@@ -60,11 +60,13 @@
 The whole library is behind a feature flag, so you need to specify `--features python-extension-module` to enable it.
 This is a [known issue](https://pyo3.rs/v0.18.3/faq.html#i-cant-run-cargo-test-or-i-cant-build-in-a-cargo-workspace-im-having-linker-issues-like-symbol-not-found-or-undefined-reference-to-_pyexc_systemerror) of `pyo3`.
 
 See [PyO3](https://pyo3.rs) for more information.
 
 ## Run example
 
+From the repository root:
+
 ```bash
 python examples/reader.py
 ```
```

