# Comparing `tmp/surrealdb-beta-0.0.2.tar.gz` & `tmp/surrealdb-beta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surrealdb-beta-0.0.2.tar", last modified: Mon Jul 31 09:38:20 2023, max compression
+gzip compressed data, was "surrealdb-beta-0.0.3.tar", last modified: Mon Jul 31 10:59:51 2023, max compression
```

## Comparing `surrealdb-beta-0.0.2.tar` & `surrealdb-beta-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 09:37:47.000000 surrealdb-beta-0.0.2/surrealdb/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/connection_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb/execution_mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-31 09:37:43.000000 surrealdb-beta-0.0.2/surrealdb/execution_mixins/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:38:20.308621 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 09:38:20.000000 surrealdb-beta-0.0.2/surrealdb_beta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:51.166909 surrealdb-beta-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-31 10:59:51.166909 surrealdb-beta-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 10:59:51.166909 surrealdb-beta-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:51.162909 surrealdb-beta-0.0.3/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 10:59:30.000000 surrealdb-beta-0.0.3/surrealdb/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/connection_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:51.162909 surrealdb-beta-0.0.3/surrealdb/execution_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-31 10:59:26.000000 surrealdb-beta-0.0.3/surrealdb/execution_mixins/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:59:51.166909 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-31 10:59:51.000000 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-31 10:59:51.000000 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:59:51.000000 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:59:50.000000 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 10:59:51.000000 surrealdb-beta-0.0.3/surrealdb_beta.egg-info/top_level.txt
```

### Comparing `surrealdb-beta-0.0.2/LICENSE` & `surrealdb-beta-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/PKG-INFO` & `surrealdb-beta-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: surrealdb-beta
-Version: 0.0.2
-Summary: Calculates a Fibonacci number
+Version: 0.0.3
+Summary: SurrealDB python client written in Rust.
 Author: Maxwell Flitton
 Author-email: maxwell@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img width="300" src="https://raw.githubusercontent.com/surrealdb/surrealdb/main/img/icon.png" alt="SurrealDB Icon">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: surrealdb-beta Version: 0.0.2 Summary: Calculates a
-Fibonacci number Author: Maxwell Flitton Author-email: maxwell@gmail.com
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: surrealdb-beta Version: 0.0.3 Summary: SurrealDB
+python client written in Rust. Author: Maxwell Flitton Author-email:
+maxwell@gmail.com Description-Content-Type: text/markdown License-File: LICENSE
                                [SurrealDB Icon]
 
                        [SurrealDB_Logo] [SurrealDB_Logo]
               **** [SurrealDB] [SurrealDB] is the ultimate cloud
                    database for tomorrow's applications ****
           **** Develop easier.   Build faster.   Scale quicker. ****
```

### Comparing `surrealdb-beta-0.0.2/README.md` & `surrealdb-beta-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/setup.py` & `surrealdb-beta-0.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     version = fh.read().split("=")[1].replace("'", "")
 
 
 setup(
     name="surrealdb-beta",
     author="Maxwell Flitton",
     author_email="maxwell@gmail.com",
-    description="Calculates a Fibonacci number",
+    description="SurrealDB python client written in Rust.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     version=version,
     rust_extensions=[RustExtension("surrealdb.rust_surrealdb", binding=Binding.PyO3)],
     packages=[
         "surrealdb",
         "surrealdb.execution_mixins"
```

### Comparing `surrealdb-beta-0.0.2/surrealdb/connection_interface.py` & `surrealdb-beta-0.0.3/surrealdb/connection_interface.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb/execution_mixins/auth.py` & `surrealdb-beta-0.0.3/surrealdb/execution_mixins/auth.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb/execution_mixins/create.py` & `surrealdb-beta-0.0.3/surrealdb/execution_mixins/create.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb/execution_mixins/query.py` & `surrealdb-beta-0.0.3/surrealdb/execution_mixins/query.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb/execution_mixins/set.py` & `surrealdb-beta-0.0.3/surrealdb/execution_mixins/set.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb/execution_mixins/update.py` & `surrealdb-beta-0.0.3/surrealdb/execution_mixins/update.py`

 * *Files identical despite different names*

### Comparing `surrealdb-beta-0.0.2/surrealdb_beta.egg-info/PKG-INFO` & `surrealdb-beta-0.0.3/surrealdb_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: surrealdb-beta
-Version: 0.0.2
-Summary: Calculates a Fibonacci number
+Version: 0.0.3
+Summary: SurrealDB python client written in Rust.
 Author: Maxwell Flitton
 Author-email: maxwell@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
     <img width="300" src="https://raw.githubusercontent.com/surrealdb/surrealdb/main/img/icon.png" alt="SurrealDB Icon">
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: surrealdb-beta Version: 0.0.2 Summary: Calculates a
-Fibonacci number Author: Maxwell Flitton Author-email: maxwell@gmail.com
-Description-Content-Type: text/markdown License-File: LICENSE
+Metadata-Version: 2.1 Name: surrealdb-beta Version: 0.0.3 Summary: SurrealDB
+python client written in Rust. Author: Maxwell Flitton Author-email:
+maxwell@gmail.com Description-Content-Type: text/markdown License-File: LICENSE
                                [SurrealDB Icon]
 
                        [SurrealDB_Logo] [SurrealDB_Logo]
               **** [SurrealDB] [SurrealDB] is the ultimate cloud
                    database for tomorrow's applications ****
           **** Develop easier.   Build faster.   Scale quicker. ****
```

### Comparing `surrealdb-beta-0.0.2/surrealdb_beta.egg-info/SOURCES.txt` & `surrealdb-beta-0.0.3/surrealdb_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

