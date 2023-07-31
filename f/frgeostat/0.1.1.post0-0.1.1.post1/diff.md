# Comparing `tmp/frgeostat-0.1.1.post0.tar.gz` & `tmp/frgeostat-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frgeostat-0.1.1.post0.tar", max compression
+gzip compressed data, was "frgeostat-0.1.1.post1.tar", max compression
```

## Comparing `frgeostat-0.1.1.post0.tar` & `frgeostat-0.1.1.post1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      892 2023-07-31 05:22:41.212872 frgeostat-0.1.1.post0/README.md
--rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.1.post0/frgeostat/__init__.py
--rw-r--r--   0        0        0     2375 2023-07-31 04:23:17.826154 frgeostat-0.1.1.post0/frgeostat/cli.py
--rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.1.post0/frgeostat/communes.py
--rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.1.post0/frgeostat/config.toml
--rw-r--r--   0        0        0     7938 2023-07-31 05:16:51.213525 frgeostat-0.1.1.post0/frgeostat/departements.py
--rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.1.post0/frgeostat/utils.py
--rw-r--r--   0        0        0      863 2023-07-31 05:23:06.989602 frgeostat-0.1.1.post0/pyproject.toml
--rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 frgeostat-0.1.1.post0/PKG-INFO
+-rw-r--r--   0        0        0      892 2023-07-31 05:22:41.212872 frgeostat-0.1.1.post1/README.md
+-rw-r--r--   0        0        0        0 2023-07-28 12:51:52.685150 frgeostat-0.1.1.post1/frgeostat/__init__.py
+-rw-r--r--   0        0        0     2375 2023-07-31 04:23:17.826154 frgeostat-0.1.1.post1/frgeostat/cli.py
+-rw-r--r--   0        0        0     3705 2023-07-28 19:23:04.026154 frgeostat-0.1.1.post1/frgeostat/communes.py
+-rw-r--r--   0        0        0      326 2023-07-31 04:13:26.663405 frgeostat-0.1.1.post1/frgeostat/config.toml
+-rw-r--r--   0        0        0     7938 2023-07-31 05:16:51.213525 frgeostat-0.1.1.post1/frgeostat/departements.py
+-rw-r--r--   0        0        0      697 2023-07-31 04:21:33.051262 frgeostat-0.1.1.post1/frgeostat/utils.py
+-rw-r--r--   0        0        0      863 2023-07-31 05:24:41.609608 frgeostat-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 frgeostat-0.1.1.post1/PKG-INFO
```

### Comparing `frgeostat-0.1.1.post0/README.md` & `frgeostat-0.1.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post0/frgeostat/cli.py` & `frgeostat-0.1.1.post1/frgeostat/cli.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post0/frgeostat/communes.py` & `frgeostat-0.1.1.post1/frgeostat/communes.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post0/frgeostat/departements.py` & `frgeostat-0.1.1.post1/frgeostat/departements.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post0/frgeostat/utils.py` & `frgeostat-0.1.1.post1/frgeostat/utils.py`

 * *Files identical despite different names*

### Comparing `frgeostat-0.1.1.post0/pyproject.toml` & `frgeostat-0.1.1.post1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "frgeostat"
-version = "0.1.1-post0"
+version = "0.1.1-post1"
 description = "A small package to help creating maps of france with geo statistical data overlays."
 authors = ["volt-france <arno.veletanlic@volteuropa.org>"]
 readme = "README.md"
 homepage = "https://bureaux-vote.v.olt.sh"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `frgeostat-0.1.1.post0/PKG-INFO` & `frgeostat-0.1.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frgeostat
-Version: 0.1.1.post0
+Version: 0.1.1.post1
 Summary: A small package to help creating maps of france with geo statistical data overlays.
 Home-page: https://bureaux-vote.v.olt.sh
 Author: volt-france
 Author-email: arno.veletanlic@volteuropa.org
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

