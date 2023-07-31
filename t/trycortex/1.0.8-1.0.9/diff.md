# Comparing `tmp/trycortex-1.0.8.tar.gz` & `tmp/trycortex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycortex-1.0.8.tar", max compression
+gzip compressed data, was "trycortex-1.0.9.tar", max compression
```

## Comparing `trycortex-1.0.8.tar` & `trycortex-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.8/README.md
--rw-r--r--   0        0        0      489 2023-07-25 21:49:43.355138 trycortex-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       90 2023-07-13 21:47:58.631841 trycortex-1.0.8/trycortex/__init__.py
--rw-r--r--   0        0        0    12976 2023-07-19 20:20:29.647945 trycortex-1.0.8/trycortex/api.py
--rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.8/trycortex/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 22:58:20.969482 trycortex-1.0.8/trycortex/cli/callable/__init__.py
--rw-r--r--   0        0        0     1600 2023-07-25 19:54:37.293457 trycortex-1.0.8/trycortex/cli/callable/callable_config.py
--rw-r--r--   0        0        0     6869 2023-07-25 21:48:58.385594 trycortex-1.0.8/trycortex/cli/callable/commands.py
--rw-r--r--   0        0        0      308 2023-07-25 19:54:52.811386 trycortex-1.0.8/trycortex/cli/cli.py
--rw-r--r--   0        0        0     1522 2023-07-15 00:34:23.304330 trycortex-1.0.8/trycortex/cli/utils.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 trycortex-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-07-13 22:45:36.236046 trycortex-1.0.9/README.md
+-rw-r--r--   0        0        0      489 2023-07-25 21:57:24.254449 trycortex-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-07-25 21:57:12.092754 trycortex-1.0.9/trycortex/__init__.py
+-rw-r--r--   0        0        0    12976 2023-07-19 20:20:29.647945 trycortex-1.0.9/trycortex/api.py
+-rw-r--r--   0        0        0        0 2023-07-13 23:06:56.199856 trycortex-1.0.9/trycortex/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-14 22:58:20.969482 trycortex-1.0.9/trycortex/cli/callable/__init__.py
+-rw-r--r--   0        0        0     1600 2023-07-25 19:54:37.293457 trycortex-1.0.9/trycortex/cli/callable/callable_config.py
+-rw-r--r--   0        0        0     6869 2023-07-25 21:53:32.266952 trycortex-1.0.9/trycortex/cli/callable/commands.py
+-rw-r--r--   0        0        0      308 2023-07-25 19:54:52.811386 trycortex-1.0.9/trycortex/cli/cli.py
+-rw-r--r--   0        0        0     1522 2023-07-15 00:34:23.304330 trycortex-1.0.9/trycortex/cli/utils.py
+-rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 trycortex-1.0.9/PKG-INFO
```

### Comparing `trycortex-1.0.8/trycortex/api.py` & `trycortex-1.0.9/trycortex/api.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.8/trycortex/cli/callable/callable_config.py` & `trycortex-1.0.9/trycortex/cli/callable/callable_config.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.8/trycortex/cli/callable/commands.py` & `trycortex-1.0.9/trycortex/cli/callable/commands.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.8/trycortex/cli/utils.py` & `trycortex-1.0.9/trycortex/cli/utils.py`

 * *Files identical despite different names*

### Comparing `trycortex-1.0.8/PKG-INFO` & `trycortex-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycortex
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for Cortex
 Author: Charles
 Author-email: charlespun6@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

