# Comparing `tmp/chiku-0.0.8.tar.gz` & `tmp/chiku-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiku-0.0.8.tar", last modified: Tue Mar 14 22:00:20 2023, max compression
+gzip compressed data, was "chiku-0.0.9.tar", last modified: Tue Mar 14 23:20:39 2023, max compression
```

## Comparing `chiku-0.0.8.tar` & `chiku-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 22:00:20.377992 chiku-0.0.8/
--rw-r--r--   0 devharsh   (501) staff       (20)    34523 2023-03-14 16:39:06.000000 chiku-0.0.8/LICENSE
--rw-r--r--   0 devharsh   (501) staff       (20)      660 2023-03-14 22:00:20.377349 chiku-0.0.8/PKG-INFO
--rw-r--r--   0 devharsh   (501) staff       (20)       61 2023-03-14 16:39:06.000000 chiku-0.0.8/README.md
--rw-r--r--   0 devharsh   (501) staff       (20)      729 2023-03-14 21:58:54.000000 chiku-0.0.8/pyproject.toml
--rw-r--r--   0 devharsh   (501) staff       (20)       38 2023-03-14 22:00:20.378172 chiku-0.0.8/setup.cfg
-drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 22:00:20.363126 chiku-0.0.8/src/
-drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 22:00:20.370792 chiku-0.0.8/src/chiku/
--rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.8/src/chiku/__init__.py
--rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.8/src/chiku/chebyshev.py
--rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.8/src/chiku/fourier.py
--rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.8/src/chiku/pade.py
--rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.8/src/chiku/remez.py
--rw-r--r--   0 devharsh   (501) staff       (20)     1465 2023-03-14 21:50:42.000000 chiku-0.0.8/src/chiku/taylor.py
--rw-r--r--   0 devharsh   (501) staff       (20)     1215 2023-03-14 17:09:24.000000 chiku-0.0.8/src/chiku/tf_ann.py
-drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 22:00:20.374669 chiku-0.0.8/src/chiku.egg-info/
--rw-r--r--   0 devharsh   (501) staff       (20)      660 2023-03-14 22:00:20.000000 chiku-0.0.8/src/chiku.egg-info/PKG-INFO
--rw-r--r--   0 devharsh   (501) staff       (20)      349 2023-03-14 22:00:20.000000 chiku-0.0.8/src/chiku.egg-info/SOURCES.txt
--rw-r--r--   0 devharsh   (501) staff       (20)        1 2023-03-14 22:00:20.000000 chiku-0.0.8/src/chiku.egg-info/dependency_links.txt
--rw-r--r--   0 devharsh   (501) staff       (20)        6 2023-03-14 22:00:20.000000 chiku-0.0.8/src/chiku.egg-info/top_level.txt
-drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 22:00:20.376395 chiku-0.0.8/tests/
--rw-r--r--   0 devharsh   (501) staff       (20)      389 2023-03-14 21:56:03.000000 chiku-0.0.8/tests/test_taylor.py
--rw-r--r--   0 devharsh   (501) staff       (20)      404 2023-03-14 21:37:55.000000 chiku-0.0.8/tests/test_tf_ann.py
+drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 23:20:39.720966 chiku-0.0.9/
+-rw-r--r--   0 devharsh   (501) staff       (20)    34523 2023-03-14 16:39:06.000000 chiku-0.0.9/LICENSE
+-rw-r--r--   0 devharsh   (501) staff       (20)      660 2023-03-14 23:20:39.720318 chiku-0.0.9/PKG-INFO
+-rw-r--r--   0 devharsh   (501) staff       (20)       61 2023-03-14 16:39:06.000000 chiku-0.0.9/README.md
+-rw-r--r--   0 devharsh   (501) staff       (20)      729 2023-03-14 23:10:50.000000 chiku-0.0.9/pyproject.toml
+-rw-r--r--   0 devharsh   (501) staff       (20)       38 2023-03-14 23:20:39.721157 chiku-0.0.9/setup.cfg
+drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 23:20:39.705809 chiku-0.0.9/src/
+drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 23:20:39.712741 chiku-0.0.9/src/chiku/
+-rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.9/src/chiku/__init__.py
+-rw-r--r--   0 devharsh   (501) staff       (20)      826 2023-03-14 22:27:01.000000 chiku-0.0.9/src/chiku/chebyshev.py
+-rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.9/src/chiku/fourier.py
+-rw-r--r--   0 devharsh   (501) staff       (20)        0 2023-03-14 16:39:06.000000 chiku-0.0.9/src/chiku/pade.py
+-rw-r--r--   0 devharsh   (501) staff       (20)        2 2023-03-14 23:10:29.000000 chiku-0.0.9/src/chiku/remez.py
+-rw-r--r--   0 devharsh   (501) staff       (20)     1465 2023-03-14 21:50:42.000000 chiku-0.0.9/src/chiku/taylor.py
+-rw-r--r--   0 devharsh   (501) staff       (20)     1215 2023-03-14 17:09:24.000000 chiku-0.0.9/src/chiku/tf_ann.py
+drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 23:20:39.716271 chiku-0.0.9/src/chiku.egg-info/
+-rw-r--r--   0 devharsh   (501) staff       (20)      660 2023-03-14 23:20:39.000000 chiku-0.0.9/src/chiku.egg-info/PKG-INFO
+-rw-r--r--   0 devharsh   (501) staff       (20)      373 2023-03-14 23:20:39.000000 chiku-0.0.9/src/chiku.egg-info/SOURCES.txt
+-rw-r--r--   0 devharsh   (501) staff       (20)        1 2023-03-14 23:20:39.000000 chiku-0.0.9/src/chiku.egg-info/dependency_links.txt
+-rw-r--r--   0 devharsh   (501) staff       (20)        6 2023-03-14 23:20:39.000000 chiku-0.0.9/src/chiku.egg-info/top_level.txt
+drwxr-xr-x   0 devharsh   (501) staff       (20)        0 2023-03-14 23:20:39.718802 chiku-0.0.9/tests/
+-rw-r--r--   0 devharsh   (501) staff       (20)      404 2023-03-14 22:24:27.000000 chiku-0.0.9/tests/test_chebyshev.py
+-rw-r--r--   0 devharsh   (501) staff       (20)      389 2023-03-14 21:56:03.000000 chiku-0.0.9/tests/test_taylor.py
+-rw-r--r--   0 devharsh   (501) staff       (20)      404 2023-03-14 21:37:55.000000 chiku-0.0.9/tests/test_tf_ann.py
```

### Comparing `chiku-0.0.8/LICENSE` & `chiku-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chiku-0.0.8/PKG-INFO` & `chiku-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiku
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for polynomial approximation of arbitrary functions.
 Author-email: Devharsh Trivedi <devharsh@live.in>
 Project-URL: Homepage, https://com.puter.tips/
 Project-URL: Docs, https://com.puter.tips/
 Project-URL: Bug Tracker, https://com.puter.tips/
 Project-URL: repository, https://com.puter.tips/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chiku-0.0.8/pyproject.toml` & `chiku-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "tensorflow",
     "numdifftools"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chiku"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name="Devharsh Trivedi", email="devharsh@live.in" },
 ]
 description = "A Python package for polynomial approximation of arbitrary functions."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `chiku-0.0.8/src/chiku/taylor.py` & `chiku-0.0.9/src/chiku/taylor.py`

 * *Files identical despite different names*

### Comparing `chiku-0.0.8/src/chiku/tf_ann.py` & `chiku-0.0.9/src/chiku/tf_ann.py`

 * *Files identical despite different names*

### Comparing `chiku-0.0.8/src/chiku.egg-info/PKG-INFO` & `chiku-0.0.9/src/chiku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiku
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python package for polynomial approximation of arbitrary functions.
 Author-email: Devharsh Trivedi <devharsh@live.in>
 Project-URL: Homepage, https://com.puter.tips/
 Project-URL: Docs, https://com.puter.tips/
 Project-URL: Bug Tracker, https://com.puter.tips/
 Project-URL: repository, https://com.puter.tips/
 Classifier: Programming Language :: Python :: 3
```

