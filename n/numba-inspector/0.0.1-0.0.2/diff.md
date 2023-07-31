# Comparing `tmp/numba_inspector-0.0.1.tar.gz` & `tmp/numba_inspector-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba_inspector-0.0.1.tar", max compression
+gzip compressed data, was "numba_inspector-0.0.2.tar", max compression
```

## Comparing `numba_inspector-0.0.1.tar` & `numba_inspector-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1386 2023-07-10 20:00:21.880231 numba_inspector-0.0.1/README.md
--rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.1/numba_inspector/__init__.py
--rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.1/numba_inspector/frontend/__init__.py
--rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.1/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.1/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
--rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.1/numba_inspector/frontend/annotate.py
--rw-r--r--   0        0        0     8969 2023-07-20 22:05:37.975821 numba_inspector-0.0.1/numba_inspector/ipython_magic.py
--rw-r--r--   0        0        0      395 2023-07-31 12:08:23.550732 numba_inspector-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 numba_inspector-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1386 2023-07-10 20:00:21.880231 numba_inspector-0.0.2/README.md
+-rw-r--r--   0        0        0      265 2023-07-10 14:32:37.520531 numba_inspector-0.0.2/numba_inspector/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 14:24:29.660514 numba_inspector-0.0.2/numba_inspector/frontend/__init__.py
+-rw-r--r--   0        0        0      159 2023-07-10 14:47:47.708513 numba_inspector-0.0.2/numba_inspector/frontend/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    33486 2023-07-10 17:43:41.334660 numba_inspector-0.0.2/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc
+-rw-r--r--   0        0        0    36003 2023-07-10 17:43:35.494660 numba_inspector-0.0.2/numba_inspector/frontend/annotate.py
+-rw-r--r--   0        0        0     8969 2023-07-20 22:05:37.975821 numba_inspector-0.0.2/numba_inspector/ipython_magic.py
+-rw-r--r--   0        0        0      415 2023-07-31 12:32:15.729761 numba_inspector-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 numba_inspector-0.0.2/PKG-INFO
```

### Comparing `numba_inspector-0.0.1/README.md` & `numba_inspector-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.1/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc` & `numba_inspector-0.0.2/numba_inspector/frontend/__pycache__/annotate.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.1/numba_inspector/frontend/annotate.py` & `numba_inspector-0.0.2/numba_inspector/frontend/annotate.py`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.1/numba_inspector/ipython_magic.py` & `numba_inspector-0.0.2/numba_inspector/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `numba_inspector-0.0.1/PKG-INFO` & `numba_inspector-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: numba-inspector
-Version: 0.0.1
+Version: 0.0.2
 Summary: Visualize and Debug Numba compiled code in Jupyter
 Author: Matthew Murray
 Author-email: matthewmurray711@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: notebook (>=7.0.0,<8.0.0)
 Requires-Dist: numba (>=0.57.1,<0.58.0)
 Description-Content-Type: text/markdown
 
 # numba-inspector
 View Numba compiled code in Jupyter
 
 ## Quickstart
```

