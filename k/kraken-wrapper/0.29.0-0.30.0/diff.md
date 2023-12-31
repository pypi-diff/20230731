# Comparing `tmp/kraken_wrapper-0.29.0.tar.gz` & `tmp/kraken_wrapper-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.29.0.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.30.0.tar", max compression
```

## Comparing `kraken_wrapper-0.29.0.tar` & `kraken_wrapper-0.30.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      998 2023-07-03 15:02:12.198680 kraken_wrapper-0.29.0/LICENSE
--rw-r--r--   0        0        0      378 2023-06-26 11:13:42.662140 kraken_wrapper-0.29.0/README.md
--rw-r--r--   0        0        0     2308 2023-07-13 08:25:42.771390 kraken_wrapper-0.29.0/pyproject.toml
--rw-r--r--   0        0        0      134 2023-07-13 08:25:42.771494 kraken_wrapper-0.29.0/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     7715 2023-07-13 08:25:27.835681 kraken_wrapper-0.29.0/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3478 2023-06-26 11:13:42.664260 kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-06-20 12:31:06.105651 kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-06-20 12:31:06.105769 kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     4290 2023-07-03 15:02:12.204283 kraken_wrapper-0.29.0/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-06-20 12:31:06.106048 kraken_wrapper-0.29.0/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-06-20 12:31:06.106187 kraken_wrapper-0.29.0/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-06-20 12:31:06.106313 kraken_wrapper-0.29.0/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15982 2023-07-03 15:02:12.208021 kraken_wrapper-0.29.0/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-06-20 12:31:06.106556 kraken_wrapper-0.29.0/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 kraken_wrapper-0.29.0/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-07-31 08:56:49.313120 kraken_wrapper-0.30.0/LICENSE
+-rw-r--r--   0        0        0      378 2023-07-31 08:56:49.313352 kraken_wrapper-0.30.0/README.md
+-rw-r--r--   0        0        0     2308 2023-07-31 09:06:28.975072 kraken_wrapper-0.30.0/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-07-31 09:06:28.975182 kraken_wrapper-0.30.0/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     7715 2023-07-31 08:56:49.314662 kraken_wrapper-0.30.0/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3478 2023-07-31 08:56:49.314907 kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-05-16 06:59:55.186954 kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-05-16 06:59:55.187085 kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     4290 2023-07-31 08:56:49.315273 kraken_wrapper-0.30.0/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-05-16 06:59:55.187323 kraken_wrapper-0.30.0/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-05-16 06:59:55.187437 kraken_wrapper-0.30.0/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-05-16 06:59:55.187563 kraken_wrapper-0.30.0/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15982 2023-07-31 08:56:49.315757 kraken_wrapper-0.30.0/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:55.187792 kraken_wrapper-0.30.0/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 kraken_wrapper-0.30.0/PKG-INFO
```

### Comparing `kraken_wrapper-0.29.0/LICENSE` & `kraken_wrapper-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/pyproject.toml` & `kraken_wrapper-0.30.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.29.0"
+version = "0.30.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 keyring = "^23.8.2"
-kraken-common = "^0.29.0"
+kraken-common = "^0.30.0"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 rich = "^13.4.2"
 
 # NOTE(@NiklasRosenstein): Need to pin transitive dependency markdown-it under 3.0 because it dropped Python 3.9
 #       support after that version. Technically this shouldn't be a big issue for runtime, but Mypy checks site
```

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/src/kraken/wrapper/main.py` & `kraken_wrapper-0.30.0/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.29.0/PKG-INFO` & `kraken_wrapper-0.30.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.29.0
+Version: 0.30.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.29.0,<0.30.0)
+Requires-Dist: kraken-common (>=0.30.0,<0.31.0)
 Requires-Dist: markdown-it-py (<3.0.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Requires-Dist: typing-extensions (<4.7.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
```

