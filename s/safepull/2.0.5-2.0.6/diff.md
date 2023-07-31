# Comparing `tmp/safepull-2.0.5.tar.gz` & `tmp/safepull-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safepull-2.0.5.tar", max compression
+gzip compressed data, was "safepull-2.0.6.tar", max compression
```

## Comparing `safepull-2.0.5.tar` & `safepull-2.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-07-15 16:01:22.713137 safepull-2.0.5/LICENSE
--rw-r--r--   0        0        0     5359 2023-07-15 16:01:22.713137 safepull-2.0.5/README.md
--rw-r--r--   0        0        0      619 2023-07-15 16:01:22.713137 safepull-2.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/__init__.py
--rw-r--r--   0        0        0       64 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/__main__.py
--rw-r--r--   0        0        0     3058 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/models.py
--rw-r--r--   0        0        0     3572 2023-07-15 16:01:22.713137 safepull-2.0.5/src/safepull/safepull.py
--rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 safepull-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-07-31 17:52:29.833470 safepull-2.0.6/LICENSE
+-rw-r--r--   0        0        0     5359 2023-07-31 17:52:29.833470 safepull-2.0.6/README.md
+-rw-r--r--   0        0        0      629 2023-07-31 17:52:29.833470 safepull-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 17:52:29.833470 safepull-2.0.6/src/safepull/__init__.py
+-rw-r--r--   0        0        0       64 2023-07-31 17:52:29.833470 safepull-2.0.6/src/safepull/__main__.py
+-rw-r--r--   0        0        0     3058 2023-07-31 17:52:29.833470 safepull-2.0.6/src/safepull/models.py
+-rw-r--r--   0        0        0     3572 2023-07-31 17:52:29.833470 safepull-2.0.6/src/safepull/safepull.py
+-rw-r--r--   0        0        0     5966 1970-01-01 00:00:00.000000 safepull-2.0.6/PKG-INFO
```

### Comparing `safepull-2.0.5/LICENSE` & `safepull-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `safepull-2.0.5/README.md` & `safepull-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `safepull-2.0.5/pyproject.toml` & `safepull-2.0.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "safepull"
-version = "2.0.5"
+version = "2.0.6"
 description = "A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py."
 authors = ["Rem <128343390+import-pandas-as-numpy@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
 rich = "^13.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.0.278"
+ruff = ">=0.0.278,<0.0.281"
 pre-commit = "^3.3.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `safepull-2.0.5/src/safepull/models.py` & `safepull-2.0.6/src/safepull/models.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.5/src/safepull/safepull.py` & `safepull-2.0.6/src/safepull/safepull.py`

 * *Files identical despite different names*

### Comparing `safepull-2.0.5/PKG-INFO` & `safepull-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safepull
-Version: 2.0.5
+Version: 2.0.6
 Summary: A CLI tool for downloading and extracting packages from PyPI without interfacing with setup.py.
 License: MIT
 Author: Rem
 Author-email: 128343390+import-pandas-as-numpy@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

