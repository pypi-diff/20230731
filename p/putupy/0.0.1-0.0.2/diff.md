# Comparing `tmp/putupy-0.0.1.tar.gz` & `tmp/putupy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "putupy-0.0.1.tar", last modified: Mon Jul 31 15:15:37 2023, max compression
+gzip compressed data, was "putupy-0.0.2.tar", last modified: Mon Jul 31 15:53:31 2023, max compression
```

## Comparing `putupy-0.0.1.tar` & `putupy-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:15:37.194098 putupy-0.0.1/
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)     1080 2023-07-31 13:11:31.000000 putupy-0.0.1/LICENSE
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      500 2023-07-31 15:15:37.193658 putupy-0.0.1/PKG-INFO
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       15 2023-07-31 13:11:40.000000 putupy-0.0.1/README.md
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      558 2023-07-31 13:16:07.000000 putupy-0.0.1/pyproject.toml
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       38 2023-07-31 15:15:37.194248 putupy-0.0.1/setup.cfg
-drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:15:37.181963 putupy-0.0.1/src/
-drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:15:37.186554 putupy-0.0.1/src/putupy/
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 13:00:00.000000 putupy-0.0.1/src/putupy/__init__.py
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       42 2023-07-31 13:14:17.000000 putupy-0.0.1/src/putupy/base.py
-drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:15:37.192582 putupy-0.0.1/src/putupy/firstmodule/
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 13:00:25.000000 putupy-0.0.1/src/putupy/firstmodule/__init__.py
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       42 2023-07-31 13:13:11.000000 putupy-0.0.1/src/putupy/firstmodule/fmodule.py
-drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:15:37.190505 putupy-0.0.1/src/putupy.egg-info/
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      500 2023-07-31 15:15:37.000000 putupy-0.0.1/src/putupy.egg-info/PKG-INFO
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      279 2023-07-31 15:15:37.000000 putupy-0.0.1/src/putupy.egg-info/SOURCES.txt
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        1 2023-07-31 15:15:37.000000 putupy-0.0.1/src/putupy.egg-info/dependency_links.txt
--rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        7 2023-07-31 15:15:37.000000 putupy-0.0.1/src/putupy.egg-info/top_level.txt
+drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:53:31.851222 putupy-0.0.2/
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)     1080 2023-07-31 13:11:31.000000 putupy-0.0.2/LICENSE
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      868 2023-07-31 15:53:31.850780 putupy-0.0.2/PKG-INFO
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      382 2023-07-31 15:51:06.000000 putupy-0.0.2/README.md
+drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:53:31.842427 putupy-0.0.2/putupy/
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 13:00:00.000000 putupy-0.0.2/putupy/__init__.py
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       42 2023-07-31 13:14:17.000000 putupy-0.0.2/putupy/base.py
+drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:53:31.848650 putupy-0.0.2/putupy/firstmodule/
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 13:00:25.000000 putupy-0.0.2/putupy/firstmodule/__init__.py
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       42 2023-07-31 13:13:11.000000 putupy-0.0.2/putupy/firstmodule/fmodule.py
+drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:53:31.846099 putupy-0.0.2/putupy.egg-info/
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      868 2023-07-31 15:53:31.000000 putupy-0.0.2/putupy.egg-info/PKG-INFO
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      268 2023-07-31 15:53:31.000000 putupy-0.0.2/putupy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        1 2023-07-31 15:53:31.000000 putupy-0.0.2/putupy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        7 2023-07-31 15:53:31.000000 putupy-0.0.2/putupy.egg-info/top_level.txt
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      558 2023-07-31 15:52:59.000000 putupy-0.0.2/pyproject.toml
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)       38 2023-07-31 15:53:31.851398 putupy-0.0.2/setup.cfg
+drwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)        0 2023-07-31 15:53:31.849721 putupy-0.0.2/tests/
+-rwxrwxrwx   0 putuwaw   (1000) putuwaw   (1000)      316 2023-07-31 15:42:35.000000 putupy-0.0.2/tests/test_number.py
```

### Comparing `putupy-0.0.1/LICENSE` & `putupy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `putupy-0.0.1/pyproject.toml` & `putupy-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "putupy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Putu Widyantara", email="putuwaw973@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

