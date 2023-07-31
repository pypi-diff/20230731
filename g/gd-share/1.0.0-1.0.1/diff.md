# Comparing `tmp/gd_share-1.0.0.tar.gz` & `tmp/gd_share-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gd_share-1.0.0.tar", max compression
+gzip compressed data, was "gd_share-1.0.1.tar", max compression
```

## Comparing `gd_share-1.0.0.tar` & `gd_share-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1092 2023-07-05 15:54:24.806035 gd_share-1.0.0/LICENSE
--rw-r--r--   0        0        0     2997 2023-07-05 15:54:24.806035 gd_share-1.0.0/README.md
--rw-r--r--   0        0        0      359 2023-07-05 15:54:24.810035 gd_share-1.0.0/gd/share/__init__.py
--rw-r--r--   0        0        0      101 2023-07-05 15:54:24.810035 gd_share-1.0.0/gd/share/__main__.py
--rw-r--r--   0        0        0     1756 2023-07-05 15:54:24.810035 gd_share-1.0.0/gd/share/main.py
--rw-r--r--   0        0        0        0 2023-07-05 15:54:24.810035 gd_share-1.0.0/gd/share/py.typed
--rw-r--r--   0        0        0      145 2023-07-05 15:54:24.810035 gd_share-1.0.0/gd/share/version.py
--rw-r--r--   0        0        0     3143 2023-07-05 15:54:24.810035 gd_share-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 gd_share-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-31 19:04:16.483003 gd_share-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2997 2023-07-31 19:04:16.483003 gd_share-1.0.1/README.md
+-rw-r--r--   0        0        0      359 2023-07-31 19:04:16.487002 gd_share-1.0.1/gd/share/__init__.py
+-rw-r--r--   0        0        0      101 2023-07-31 19:04:16.487002 gd_share-1.0.1/gd/share/__main__.py
+-rw-r--r--   0        0        0     1756 2023-07-31 19:04:16.487002 gd_share-1.0.1/gd/share/main.py
+-rw-r--r--   0        0        0        0 2023-07-31 19:04:16.487002 gd_share-1.0.1/gd/share/py.typed
+-rw-r--r--   0        0        0      145 2023-07-31 19:04:16.487002 gd_share-1.0.1/gd/share/version.py
+-rw-r--r--   0        0        0     3145 2023-07-31 19:04:16.487002 gd_share-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4173 1970-01-01 00:00:00.000000 gd_share-1.0.1/PKG-INFO
```

### Comparing `gd_share-1.0.0/LICENSE` & `gd_share-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gd_share-1.0.0/README.md` & `gd_share-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add gd.share
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-"gd.share" = "^1.0.0"
+"gd.share" = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies."gd.share"]
 git = "https://github.com/nekitdev/gd.share.git"
```

### Comparing `gd_share-1.0.0/gd/share/main.py` & `gd_share-1.0.1/gd/share/main.py`

 * *Files identical despite different names*

### Comparing `gd_share-1.0.0/pyproject.toml` & `gd_share-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "gd.share"
-version = "1.0.0"
-description = "Geometry Dash Discord Rich Presence."
+version = "1.0.1"
+description = "Sharing Geometry Dash levels through CLI."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/gd.share"
 repository = "https://github.com/nekitdev/gd.share"
 documentation = "https://nekitdev.github.io/gd.share"
 
-keywords = ["python", "gd", "presence"]
+keywords = ["python", "gd", "share"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Typing :: Typed",
 ]
@@ -132,15 +132,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "gd.share"
-version = "1.0.0"
+version = "1.0.1"
 url = "https://github.com/nekitdev/gd.share"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `gd_share-1.0.0/PKG-INFO` & `gd_share-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: gd-share
-Version: 1.0.0
-Summary: Geometry Dash Discord Rich Presence.
+Version: 1.0.1
+Summary: Sharing Geometry Dash levels through CLI.
 Home-page: https://github.com/nekitdev/gd.share
 License: MIT
-Keywords: python,gd,presence
+Keywords: python,gd,share
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -70,15 +70,15 @@
 $ poetry add gd.share
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-"gd.share" = "^1.0.0"
+"gd.share" = "^1.0.1"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies."gd.share"]
 git = "https://github.com/nekitdev/gd.share.git"
```

