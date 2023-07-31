# Comparing `tmp/python-typing-update-0.5.1.tar.gz` & `tmp/python-typing-update-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-typing-update-0.5.1.tar", last modified: Tue Nov 29 13:16:54 2022, max compression
+gzip compressed data, was "python-typing-update-0.6.0.tar", last modified: Mon Jul 31 10:20:46 2023, max compression
```

## Comparing `python-typing-update-0.5.1.tar` & `python-typing-update-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 13:16:54.132076 python-typing-update-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (122)       22 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     5850 2022-11-29 13:16:54.132076 python-typing-update-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5165 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2553 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 13:16:54.132076 python-typing-update-0.5.1/python_typing_update/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3985 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/const.py
--rw-r--r--   0 runner    (1001) docker     (122)     8699 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/main.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     6578 2022-11-29 13:16:31.000000 python-typing-update-0.5.1/python_typing_update/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-29 13:16:54.132076 python-typing-update-0.5.1/python_typing_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5850 2022-11-29 13:16:53.000000 python-typing-update-0.5.1/python_typing_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      501 2022-11-29 13:16:54.000000 python-typing-update-0.5.1/python_typing_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-29 13:16:53.000000 python-typing-update-0.5.1/python_typing_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       76 2022-11-29 13:16:53.000000 python-typing-update-0.5.1/python_typing_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      119 2022-11-29 13:16:53.000000 python-typing-update-0.5.1/python_typing_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-11-29 13:16:53.000000 python-typing-update-0.5.1/python_typing_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      198 2022-11-29 13:16:54.132076 python-typing-update-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:46.288739 python-typing-update-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-31 10:20:46.288739 python-typing-update-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:46.288739 python-typing-update-0.6.0/python_typing_update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6578 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/python_typing_update/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:46.288739 python-typing-update-0.6.0/python_typing_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 10:20:46.000000 python-typing-update-0.6.0/python_typing_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-31 10:20:46.292739 python-typing-update-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 10:20:46.288739 python-typing-update-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-31 10:20:27.000000 python-typing-update-0.6.0/tests/test_utils.py
```

### Comparing `python-typing-update-0.5.1/LICENSE` & `python-typing-update-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-typing-update-0.5.1/PKG-INFO` & `python-typing-update-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-typing-update
-Version: 0.5.1
+Version: 0.6.0
 Summary: Update Python typing syntax
 Home-page: https://github.com/cdce8p/python-typing-update
 Author: Marc Mueller
 License: MIT
 Keywords: typing,pep585,pep604
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `python-typing-update-0.5.1/README.md` & `python-typing-update-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python-typing-update-0.5.1/pyproject.toml` & `python-typing-update-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools~=62.3", "wheel~=0.37.1"]
+requires = ["setuptools~=68.0", "wheel~=0.41.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "python-typing-update"
-version     = "0.5.1"  # template: x.x.x[.dev1]
+version     = "0.6.0"  # template: x.x.x[.dev1]
 license     = {text = "MIT"}
 description = "Update Python typing syntax"
 readme      = "README.md"
 authors     = [{name = "Marc Mueller"}]
 keywords    = ["typing", "pep585", "pep604"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -17,24 +17,24 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
 ]
 requires-python = ">=3.8"
 dependencies    = [
-    "aiofiles==22.1.0",
-    "autoflake==2.0.0",
-    "isort==5.10.1",
-    "pyupgrade==3.2.2",
-    "reorder-python-imports==3.9.0",
+    "aiofiles==23.1.0",
+    "autoflake==2.2.0",
+    "isort==5.12.0",
+    "pyupgrade==3.10.1",
+    "reorder-python-imports==3.10.0",
 ]
 
 [project.optional-dependencies]
 black = [
-    "black==22.10.0",
+    "black==23.7.0",
 ]
 
 [project.scripts]
 python-typing-update = "python_typing_update.__main__:main"
 
 [tool.setuptools]
 license-files = ["LICENSE", "AUTHORS"]
```

### Comparing `python-typing-update-0.5.1/python_typing_update/__main__.py` & `python-typing-update-0.6.0/python_typing_update/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,22 @@
         '--py39-plus',
         action='store_const', dest='min_version', const=(3, 9),
     )
     group_py_version.add_argument(
         '--py310-plus',
         action='store_const', dest='min_version', const=(3, 10),
     )
+    group_py_version.add_argument(
+        '--py311-plus',
+        action='store_const', dest='min_version', const=(3, 11),
+    )
+    group_py_version.add_argument(
+        '--py312-plus',
+        action='store_const', dest='min_version', const=(3, 12),
+    )
 
     argv = argv or sys.argv[1:]
     args = parser.parse_args(argv)
 
     logging.basicConfig()
     if args.verbose > 0:
         logger.setLevel(logging.DEBUG)
```

### Comparing `python-typing-update-0.5.1/python_typing_update/main.py` & `python-typing-update-0.6.0/python_typing_update/main.py`

 * *Files identical despite different names*

### Comparing `python-typing-update-0.5.1/python_typing_update/utils.py` & `python-typing-update-0.6.0/python_typing_update/utils.py`

 * *Files identical despite different names*

### Comparing `python-typing-update-0.5.1/python_typing_update.egg-info/PKG-INFO` & `python-typing-update-0.6.0/python_typing_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-typing-update
-Version: 0.5.1
+Version: 0.6.0
 Summary: Update Python typing syntax
 Home-page: https://github.com/cdce8p/python-typing-update
 Author: Marc Mueller
 License: MIT
 Keywords: typing,pep585,pep604
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

