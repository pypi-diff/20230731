# Comparing `tmp/jamofetch-3.7.2.tar.gz` & `tmp/jamofetch-3.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamofetch-3.7.2.tar", max compression
+gzip compressed data, was "jamofetch-3.7.3.tar", max compression
```

## Comparing `jamofetch-3.7.2.tar` & `jamofetch-3.7.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.7.2/README.md
--rw-r--r--   0        0        0      522 2023-07-30 20:20:26.699900 jamofetch-3.7.2/pyproject.toml
--rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.7.2/src/jamofetch/__init__.py
--rwxr-xr-x   0        0        0    10931 2023-07-30 20:05:03.823308 jamofetch-3.7.2/src/jamofetch/jamofetch.py
--rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.7.2/PKG-INFO
+-rw-r--r--   0        0        0     4675 2023-07-27 23:09:54.226061 jamofetch-3.7.3/README.md
+-rw-r--r--   0        0        0      522 2023-07-30 20:28:25.297045 jamofetch-3.7.3/pyproject.toml
+-rw-r--r--   0        0        0      111 2023-07-27 23:09:54.227061 jamofetch-3.7.3/src/jamofetch/__init__.py
+-rwxr-xr-x   0        0        0    10931 2023-07-30 20:05:03.823308 jamofetch-3.7.3/src/jamofetch/jamofetch.py
+-rw-r--r--   0        0        0     5204 1970-01-01 00:00:00.000000 jamofetch-3.7.3/PKG-INFO
```

### Comparing `jamofetch-3.7.2/README.md` & `jamofetch-3.7.3/README.md`

 * *Files identical despite different names*

### Comparing `jamofetch-3.7.2/pyproject.toml` & `jamofetch-3.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamofetch"
-version = "3.7.2"
+version = "3.7.3"
 description = "A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori."
 authors = ["Duncan Scott"]
 license = "None"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `jamofetch-3.7.2/src/jamofetch/jamofetch.py` & `jamofetch-3.7.3/src/jamofetch/jamofetch.py`

 * *Files identical despite different names*

### Comparing `jamofetch-3.7.2/PKG-INFO` & `jamofetch-3.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamofetch
-Version: 3.7.2
+Version: 3.7.3
 Summary: A thin wrapper to retrieve sequence from JAMO at NERSC and on Dori.
 License: None
 Author: Duncan Scott
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

