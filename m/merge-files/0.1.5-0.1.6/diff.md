# Comparing `tmp/merge_files-0.1.5.tar.gz` & `tmp/merge_files-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merge_files-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "merge_files-0.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `merge_files-0.1.5.tar` & `merge_files-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      178 2023-07-31 13:38:04.114191 merge_files-0.1.5/README.md
--rw-r--r--   0        0        0      894 2023-07-31 13:54:40.813642 merge_files-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       47 2023-03-01 03:35:55.029690 merge_files-0.1.5/src/merge_files/__init__.py
--rw-r--r--   0        0        0       62 2023-02-27 00:26:31.697843 merge_files-0.1.5/src/merge_files/__main__.py
--rwxr-xr-x   0        0        0     1374 2023-07-31 13:38:04.114191 merge_files-0.1.5/src/merge_files/main.py
--rw-r--r--   0        0        0      618 2023-07-31 13:59:53.441613 merge_files-0.1.5/src/merge_files/mergers/__init__.py
--rw-r--r--   0        0        0      843 2023-07-31 13:38:04.114191 merge_files-0.1.5/src/merge_files/mergers/concatenate.py
--rw-r--r--   0        0        0     1435 2023-07-31 13:38:04.114191 merge_files-0.1.5/src/merge_files/mergers/env.py
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 merge_files-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-07-31 13:38:04.114191 merge_files-0.1.6/README.md
+-rw-r--r--   0        0        0      894 2023-07-31 14:31:16.692551 merge_files-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-03-01 03:35:55.029690 merge_files-0.1.6/src/merge_files/__init__.py
+-rw-r--r--   0        0        0       62 2023-02-27 00:26:31.697843 merge_files-0.1.6/src/merge_files/__main__.py
+-rwxr-xr-x   0        0        0     1384 2023-07-31 14:13:19.263121 merge_files-0.1.6/src/merge_files/main.py
+-rw-r--r--   0        0        0      618 2023-07-31 13:59:53.441613 merge_files-0.1.6/src/merge_files/mergers/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-31 13:38:04.114191 merge_files-0.1.6/src/merge_files/mergers/concatenate.py
+-rw-r--r--   0        0        0     1435 2023-07-31 13:38:04.114191 merge_files-0.1.6/src/merge_files/mergers/env.py
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 merge_files-0.1.6/PKG-INFO
```

### Comparing `merge_files-0.1.5/pyproject.toml` & `merge_files-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "merge_files"
 description = "Merge two .env files files together"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
     { name = "Gareth Davidson", email = "gaz@bitplane.net" }
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `merge_files-0.1.5/src/merge_files/main.py` & `merge_files-0.1.6/src/merge_files/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 """Merges the source file into the destination file.
 
 Supports .env, text and binary files.
 """
 import argparse
+import os
 import sys
 from typing import List
 
 from .mergers import get
 
 
 def parse_args(command_line: List[str]) -> argparse.Namespace:
```

### Comparing `merge_files-0.1.5/src/merge_files/mergers/__init__.py` & `merge_files-0.1.6/src/merge_files/mergers/__init__.py`

 * *Files identical despite different names*

### Comparing `merge_files-0.1.5/src/merge_files/mergers/concatenate.py` & `merge_files-0.1.6/src/merge_files/mergers/concatenate.py`

 * *Files identical despite different names*

### Comparing `merge_files-0.1.5/src/merge_files/mergers/env.py` & `merge_files-0.1.6/src/merge_files/mergers/env.py`

 * *Files identical despite different names*

### Comparing `merge_files-0.1.5/PKG-INFO` & `merge_files-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merge_files
-Version: 0.1.5
+Version: 0.1.6
 Summary: Merge two .env files files together
 Author-email: Gareth Davidson <gaz@bitplane.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
```

