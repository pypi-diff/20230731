# Comparing `tmp/metarace-2.1.4.tar.gz` & `tmp/metarace-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metarace-2.1.4.tar", last modified: Fri Jul 21 04:54:02 2023, max compression
+gzip compressed data, was "metarace-2.1.5.tar", last modified: Mon Jul 31 16:53:24 2023, max compression
```

## Comparing `metarace-2.1.4.tar` & `metarace-2.1.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.231471 metarace-2.1.4/
--rw-------   0 ndf       (1000) ndf       (1000)     1092 2023-07-11 12:51:50.000000 metarace-2.1.4/LICENSE
--rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.4/MANIFEST.in
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-21 04:54:02.231471 metarace-2.1.4/PKG-INFO
--rw-------   0 ndf       (1000) ndf       (1000)     3921 2023-07-11 12:41:25.000000 metarace-2.1.4/README.md
--rw-r--r--   0 ndf       (1000) ndf       (1000)      798 2023-07-21 04:52:20.000000 metarace-2.1.4/pyproject.toml
--rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-21 04:54:02.231471 metarace-2.1.4/setup.cfg
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.215471 metarace-2.1.4/src/
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.223471 metarace-2.1.4/src/metarace/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     9422 2023-07-21 04:52:36.000000 metarace-2.1.4/src/metarace/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.4/src/metarace/countback.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.227471 metarace-2.1.4/src/metarace/data/
--rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/IOC_Codes.csv
--rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.4/src/metarace/data/__init__.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armfin.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armint.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_armstart.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_idle.svg
--rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/bg_src.svg
--rw-------   0 ndf       (1000) ndf       (1000)        4 2023-07-11 12:42:36.000000 metarace-2.1.4/src/metarace/data/metarace.json
--rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.4/src/metarace/data/metarace_icon.svg
--rw-------   0 ndf       (1000) ndf       (1000)     2048 2023-06-05 01:23:26.000000 metarace-2.1.4/src/metarace/data/pdf_template.json
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.227471 metarace-2.1.4/src/metarace/decoder/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     5721 2023-07-13 12:30:30.000000 metarace-2.1.4/src/metarace/decoder/__init__.py
--rw-------   0 ndf       (1000) ndf       (1000)    16233 2023-07-13 12:30:42.000000 metarace-2.1.4/src/metarace/decoder/rrs.py
--rw-------   0 ndf       (1000) ndf       (1000)    32745 2023-07-21 01:34:17.000000 metarace-2.1.4/src/metarace/decoder/rru.py
--rw-------   0 ndf       (1000) ndf       (1000)    25107 2023-07-17 04:57:46.000000 metarace-2.1.4/src/metarace/decoder/thbc.py
--rw-------   0 ndf       (1000) ndf       (1000)    11415 2023-07-13 12:29:27.000000 metarace-2.1.4/src/metarace/eventdb.py
--rw-------   0 ndf       (1000) ndf       (1000)     6290 2023-07-13 12:29:44.000000 metarace-2.1.4/src/metarace/export.py
--rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.4/src/metarace/htlib.py
--rw-------   0 ndf       (1000) ndf       (1000)    12251 2023-07-13 12:30:06.000000 metarace-2.1.4/src/metarace/jsonconfig.py
--rw-------   0 ndf       (1000) ndf       (1000)   204351 2023-07-13 12:29:15.000000 metarace-2.1.4/src/metarace/report.py
--rw-------   0 ndf       (1000) ndf       (1000)    25632 2023-07-16 01:35:36.000000 metarace-2.1.4/src/metarace/riderdb.py
--rw-------   0 ndf       (1000) ndf       (1000)    17984 2023-07-19 07:30:40.000000 metarace-2.1.4/src/metarace/strops.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    14783 2023-07-13 12:28:46.000000 metarace-2.1.4/src/metarace/telegraph.py
--rw-------   0 ndf       (1000) ndf       (1000)    16903 2023-07-15 05:11:51.000000 metarace-2.1.4/src/metarace/timy.py
--rw-r--r--   0 ndf       (1000) ndf       (1000)    20994 2023-07-13 12:27:42.000000 metarace-2.1.4/src/metarace/tod.py
--rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.4/src/metarace/unt4.py
-drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-21 04:54:02.223471 metarace-2.1.4/src/metarace.egg-info/
--rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/PKG-INFO
--rw-r--r--   0 ndf       (1000) ndf       (1000)      969 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/SOURCES.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/dependency_links.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/requires.txt
--rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-21 04:54:02.000000 metarace-2.1.4/src/metarace.egg-info/top_level.txt
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.047315 metarace-2.1.5/
+-rw-------   0 ndf       (1000) ndf       (1000)     1092 2023-07-11 12:51:50.000000 metarace-2.1.5/LICENSE
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       28 2022-05-31 01:20:37.000000 metarace-2.1.5/MANIFEST.in
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-31 16:53:24.047315 metarace-2.1.5/PKG-INFO
+-rw-------   0 ndf       (1000) ndf       (1000)     3921 2023-07-11 12:41:25.000000 metarace-2.1.5/README.md
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      798 2023-07-31 16:50:02.000000 metarace-2.1.5/pyproject.toml
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       38 2023-07-31 16:53:24.047315 metarace-2.1.5/setup.cfg
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.039315 metarace-2.1.5/src/
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.043315 metarace-2.1.5/src/metarace/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     9800 2023-07-31 16:51:45.000000 metarace-2.1.5/src/metarace/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4268 2023-06-25 00:11:43.000000 metarace-2.1.5/src/metarace/countback.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.047315 metarace-2.1.5/src/metarace/data/
+-rw-------   0 ndf       (1000) ndf       (1000)     3067 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/IOC_Codes.csv
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        0 2023-06-28 11:57:11.000000 metarace-2.1.5/src/metarace/data/__init__.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/bg_armfin.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/bg_armint.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/bg_armstart.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     1454 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/bg_idle.svg
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     2369 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/bg_src.svg
+-rw-------   0 ndf       (1000) ndf       (1000)        4 2023-07-11 12:42:36.000000 metarace-2.1.5/src/metarace/data/metarace.json
+-rw-------   0 ndf       (1000) ndf       (1000)     8729 2022-01-22 22:18:40.000000 metarace-2.1.5/src/metarace/data/metarace_icon.svg
+-rw-------   0 ndf       (1000) ndf       (1000)     2573 2023-07-31 16:42:48.000000 metarace-2.1.5/src/metarace/data/pdf_template.json
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.047315 metarace-2.1.5/src/metarace/decoder/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     5721 2023-07-13 12:30:30.000000 metarace-2.1.5/src/metarace/decoder/__init__.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16233 2023-07-13 12:30:42.000000 metarace-2.1.5/src/metarace/decoder/rrs.py
+-rw-------   0 ndf       (1000) ndf       (1000)    32847 2023-07-31 10:23:12.000000 metarace-2.1.5/src/metarace/decoder/rru.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25107 2023-07-17 04:57:46.000000 metarace-2.1.5/src/metarace/decoder/thbc.py
+-rw-------   0 ndf       (1000) ndf       (1000)    11415 2023-07-13 12:29:27.000000 metarace-2.1.5/src/metarace/eventdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)     6290 2023-07-13 12:29:44.000000 metarace-2.1.5/src/metarace/export.py
+-rw-------   0 ndf       (1000) ndf       (1000)     5970 2023-06-28 00:17:21.000000 metarace-2.1.5/src/metarace/htlib.py
+-rw-------   0 ndf       (1000) ndf       (1000)    13505 2023-07-25 06:16:55.000000 metarace-2.1.5/src/metarace/jsonconfig.py
+-rw-------   0 ndf       (1000) ndf       (1000)   205158 2023-07-31 16:43:25.000000 metarace-2.1.5/src/metarace/report.py
+-rw-------   0 ndf       (1000) ndf       (1000)    25632 2023-07-16 01:35:36.000000 metarace-2.1.5/src/metarace/riderdb.py
+-rw-------   0 ndf       (1000) ndf       (1000)    17984 2023-07-19 07:30:40.000000 metarace-2.1.5/src/metarace/strops.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    14783 2023-07-13 12:28:46.000000 metarace-2.1.5/src/metarace/telegraph.py
+-rw-------   0 ndf       (1000) ndf       (1000)    16903 2023-07-15 05:11:51.000000 metarace-2.1.5/src/metarace/timy.py
+-rw-r--r--   0 ndf       (1000) ndf       (1000)    20994 2023-07-13 12:27:42.000000 metarace-2.1.5/src/metarace/tod.py
+-rw-------   0 ndf       (1000) ndf       (1000)     4485 2023-06-25 00:09:26.000000 metarace-2.1.5/src/metarace/unt4.py
+drwxr-xr-x   0 ndf       (1000) ndf       (1000)        0 2023-07-31 16:53:24.043315 metarace-2.1.5/src/metarace.egg-info/
+-rw-r--r--   0 ndf       (1000) ndf       (1000)     4490 2023-07-31 16:53:23.000000 metarace-2.1.5/src/metarace.egg-info/PKG-INFO
+-rw-r--r--   0 ndf       (1000) ndf       (1000)      969 2023-07-31 16:53:24.000000 metarace-2.1.5/src/metarace.egg-info/SOURCES.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        1 2023-07-31 16:53:23.000000 metarace-2.1.5/src/metarace.egg-info/dependency_links.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)       67 2023-07-31 16:53:23.000000 metarace-2.1.5/src/metarace.egg-info/requires.txt
+-rw-r--r--   0 ndf       (1000) ndf       (1000)        9 2023-07-31 16:53:23.000000 metarace-2.1.5/src/metarace.egg-info/top_level.txt
```

### Comparing `metarace-2.1.4/LICENSE` & `metarace-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/PKG-INFO` & `metarace-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.4
+Version: 2.1.5
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
```

### Comparing `metarace-2.1.4/README.md` & `metarace-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/pyproject.toml` & `metarace-2.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metarace"
-version = "2.1.4"
+version = "2.1.5"
 description = "Cyclesport results and timing toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "MIT"}
 keywords = ["cyclesport", "results", "timing"]
 authors = [
     {email = "ndf-zz@6-v.org", name = "Nathan Fraser"}
```

### Comparing `metarace-2.1.4/src/metarace/__init__.py` & `metarace-2.1.5/src/metarace/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 # SPDX-License-Identifier: MIT
 """A collection of tools for preparing cycle race results."""
 
 import os
 import logging
-import fcntl
 import errno
 from tempfile import NamedTemporaryFile
 from shutil import copyfile
 from metarace import jsonconfig
 try:
     from importlib.resources import files, as_file
 except ImportError:
     print('Python >= 3.9 is required to use this module')
+flockstyle = None
+try:
+    import fcntl
+    flockstyle = 'o-g'
+except ImportError:
+    pass
+if flockstyle is None:
+    # possibly a windows machine
+    import msvcrt
+    flockstyle = 'deviant'
 
-VERSION = '2.1.4'
+VERSION = '2.1.5'
 DATA_PATH = os.path.realpath(
     os.path.expanduser(os.path.join('~', 'Documents', 'metarace')))
 DEFAULTS_PATH = os.path.join(DATA_PATH, 'default')
 RESOURCE_PKG = 'metarace.data'
 LOGO = 'metarace_icon.svg'
 SYSCONF = 'metarace.json'
 PDF_TEMPLATE = 'pdf_template.json'
@@ -209,29 +218,35 @@
         if exc_type is not None:
             return False  # raise exception
         # otherwise, file is saved ok in temp file
         os.chmod(self.__tfile.name, self.__perm)
         try:
             os.rename(self.__tfile.name, self.__sfile)
         except OSError as e:
-            _log.debug('os.rename failed: %s', e)
             copyfile(self.__tfile.name, self.__sfile)
-            _log.warn('Un-safely moved file: %r', self.__sfile)
             os.unlink(self.__tfile.name)
         return True
 
 
 def lockpath(configpath):
     """Open an advisory lock file in the meet config path."""
+    if flockstyle is None:
+        _log.error('Meet path locking not available')
+        return None
     lf = None
     lfn = os.path.join(configpath, '.lock')
     try:
         lf = open(lfn, 'a+b')
-        fcntl.flock(lf, fcntl.LOCK_EX | fcntl.LOCK_NB)
-        _log.debug('Config lock %r acquired', lfn)
+        if flockstyle == 'o-g':
+            fcntl.flock(lf, fcntl.LOCK_EX | fcntl.LOCK_NB)
+            _log.debug('Config lock %r acquired by fcntl', lfn)
+        else:
+            lf.seek(0)
+            msvcrt.locking(lf.fileno(), msvcrt.LK_NBLCK, 1)
+            _log.debug('Config lock %r acquired by msvcrt', lfn)
     except Exception as e:
         if lf is not None:
             lf.close()
             lf = None
         _log.error('Unable to acquire config lock %r: %s', lfn, e)
     return lf
```

### Comparing `metarace-2.1.4/src/metarace/countback.py` & `metarace-2.1.5/src/metarace/countback.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/IOC_Codes.csv` & `metarace-2.1.5/src/metarace/data/IOC_Codes.csv`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/bg_armfin.svg` & `metarace-2.1.5/src/metarace/data/bg_armfin.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/bg_armint.svg` & `metarace-2.1.5/src/metarace/data/bg_armint.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/bg_armstart.svg` & `metarace-2.1.5/src/metarace/data/bg_armstart.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/bg_idle.svg` & `metarace-2.1.5/src/metarace/data/bg_idle.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/bg_src.svg` & `metarace-2.1.5/src/metarace/data/bg_src.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/data/metarace_icon.svg` & `metarace-2.1.5/src/metarace/data/metarace_icon.svg`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/decoder/__init__.py` & `metarace-2.1.5/src/metarace/decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/decoder/rrs.py` & `metarace-2.1.5/src/metarace/decoder/rrs.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/decoder/rru.py` & `metarace-2.1.5/src/metarace/decoder/rru.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,14 +711,16 @@
                 loopid = 'C1'  # add faked id for passives
             else:
                 loopid = strops.id2chan(int(loopid, 16) + 1)
             activestore = False
             if adata:
                 aval = int(adata, 16)
                 activestore = (int(adata, 16) & 0x40) == 0x40
+                if activestore:
+                    _log.debug('Stored passing %s: %r', tagid, adata)
             if tagid == _RRU_MARKER:
                 tagid = ''
 
             if battery and tagid:
                 try:
                     bv = int(battery, 16) / 10
                     if bv < _RRU_LOWBATT:
```

### Comparing `metarace-2.1.4/src/metarace/decoder/thbc.py` & `metarace-2.1.5/src/metarace/decoder/thbc.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/eventdb.py` & `metarace-2.1.5/src/metarace/eventdb.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/export.py` & `metarace-2.1.5/src/metarace/export.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/htlib.py` & `metarace-2.1.5/src/metarace/htlib.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/jsonconfig.py` & `metarace-2.1.5/src/metarace/jsonconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 		'check' : yes/no checkbox
 		'choice' : select box choice of options
 
 """
 
 import json
 import os
+import csv
 import logging
 from metarace.tod import tod, fromobj, mktod
 from metarace.strops import confopt_chan, CHAN_UNKNOWN
 
 _log = logging.getLogger('jsonconfig')
 _log.setLevel(logging.DEBUG)
 
@@ -253,14 +254,40 @@
                 else:
                     pass
                     #_log.debug('Skip option: %r', option)
             else:
                 pass
                 #_log.debug('Option: %r type none', option)
 
+    def import_csv(self, filename, defaults=None):
+        """Import values from csv into self according to schema"""
+        with open(filename, encoding='utf-8') as f:
+            section = None
+            cr = csv.reader(f)
+            for r in cr:
+                if len(r) > 1 and r[0]:
+                    key = r[0].strip()
+                    val = r[1].strip()
+                    if key.lower() == 'section':
+                        section = val
+                        self.add_section(section)
+                        _log.debug('CSV import set section to %r', section)
+                        if defaults is not None:
+                            self.merge(defaults, section)
+                    elif section is not None:
+                        self.set(section, key, val)
+                        nv = self.get_value(section, key)
+                        _log.debug('CSV Import key %r: %r => (%s) %r', key,
+                                   val, nv.__class__.__name__, nv)
+                        # Write back schema-adjusted value
+                        self.set(section, key, nv)
+                    else:
+                        _log.debug('CSV import key %r ignored, no section',
+                                   key)
+
     def import_section(self, section, obj):
         """Copy values from obj into section according to schema"""
         if section not in self.__schema:
             _log.error('No schema for section import %r', section)
             return False
         for option in self.__schema[section]:
             schema = self.__schema[section][option]
```

### Comparing `metarace-2.1.4/src/metarace/report.py` & `metarace-2.1.5/src/metarace/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,28 +83,28 @@
 # Transitional baseline position - to be replaced with font metrics
 _CELL_BASELINE = 0.715
 
 # defaults
 PANGO_SCALE = float(Pango.SCALE)
 PANGO_INVSCALE = 1.0 / float(Pango.SCALE)
 FEPSILON = 0.0001  # float epsilon
-BODYFONT = 'serif 7.0'  # body text
-BODYOBLIQUE = 'serif italic 7.0'  # body text oblique
-BODYBOLDFONT = 'serif bold 7.0'  # bold body text
-BODYSMALL = 'serif 6.0'  # small body text
-MONOSPACEFONT = 'monospace Bold 7.0'  # monospaced text
-SECTIONFONT = 'sans-serif Bold 7.0'  # section headings
-SUBHEADFONT = 'serif italic 7.0'  # section subheadings
-TITLEFONT = 'sans-serif bold 8.0'  # page title
-SUBTITLEFONT = 'sans-serif bold 7.5'  # page subtitle
-HOSTFONT = 'sans-serif oblique 7.0'  # page title
-ANNOTFONT = 'sans-serif oblique 6.0'  # header and footer annotations
-PROVFONT = 'sans-serif bold Ultra-Condensed 90'  # provisonal underlay font
-GAMUTSTDFONT = 'sans-serif bold condensed'  # default gamut standard font
-GAMUTOBFONT = 'sans-serif bold condensed italic'  # default gamut oblique font
+BODYFONT = 'Nimbus Roman, Serif, 7.0'  # body text
+BODYOBLIQUE = 'Nimbus Roman, Serif, Italic 7.0'  # body text italic
+BODYBOLDFONT = 'Nimbus Roman, Serif, Bold 7.0'  # bold body text
+BODYSMALL = 'Nimbus Roman, Serif, 6.0'  # small body text
+MONOSPACEFONT = 'Nimbus Mono PS, Monospace, Bold 7.0'  # monospaced text
+SECTIONFONT = 'Nimbus Sans, Sans-serif, Bold 7.0'  # section headings
+SUBHEADFONT = 'Nimbus Roman, Serif, Italic 7.0'  # section subheadings
+TITLEFONT = 'Nimbus Sans, Sans-serif, Bold 8.0'  # page title
+SUBTITLEFONT = 'Nimbus Sans, Sans-serif, Bold 7.5'  # page subtitle
+HOSTFONT = 'Nimbus Sans, Sans-serif, Italic 7.0'  # page title
+ANNOTFONT = 'Nimbus Sans, Sans-serif, Italic 6.0'  # header and footer annotations
+PROVFONT = 'Nimbus Sans Narrow, Sans-serif, Bold 90'  # provisonal underlay font
+GAMUTSTDFONT = 'Nimbus Sans Narrow, Sans-serif, Bold'  # default gamut standard font
+GAMUTOBFONT = 'Nimbus Sans Narrow, Sans-serif, Bold Oblique'  # default gamut oblique font
 LINE_HEIGHT = mm2pt(5.0)  # body text line height
 PAGE_OVERFLOW = mm2pt(3.0)  # tolerated section overflow
 SECTION_HEIGHT = mm2pt(5.3)  # height of section title
 TWOCOL_WIDTH = mm2pt(75.0)  # width of col on 2 col page
 THREECOL_WIDTH = mm2pt(50.0)  # width of col on 3 col page
 TABLESTYLE = 'table table-striped table-sm w-auto align-middle'  # html table style
 BUTTONSTYLE = 'btn btn-primary btn-sm'  # html normal button link
@@ -3872,14 +3872,21 @@
         self.coverpage = None
         self.loadconfig(template)
 
         # override timestamp
         self.strings['timestamp'] = (
             str(datetime.date.today().strftime('%A, %B %d %Y ')) +
             tod.now().meridiem())
+        self.strings[
+            'watermark'] = 'Report: %s; Library: %s; Template: %s %r ' % (
+                APIVERSION, metarace.VERSION, self.template_version,
+                self.template_descr)
+        if metarace.sysconf.has_value('report', 'watermark'):
+            self.strings['watermark'] += metarace.sysconf.get(
+                'report', 'watermark')
 
         # Status and context values
         self.provisional = False
         self.reportstatus = None  # optional flag for virtual etc
         self.serialno = str(int(time.time()))  # may be overidden
         self.eventid = None  # stage no or other identifier
         self.customlinks = []  # manual override links
@@ -4010,19 +4017,24 @@
         tfile = metarace.default_file(tfile)
         if not cr.load(tfile):
             try:
                 _log.debug('Loading default template from resource')
                 cr.reads(metarace.resource_text(metarace.PDF_TEMPLATE))
             except Exception as e:
                 _log.error('%s loading template: %s', e.__class__.__name__, e)
+        self.template_version = ''
+        self.template_descr = ''
         if cr.has_option('description', 'text'):
             _log.debug('API: %s, template: %s', APIVERSION,
                        cr.get('description', 'text'))
+            self.template_descr = cr.get('description', 'text')
         else:
             _log.debug('API: %s, template: UNKNOWN', APIVERSION)
+        if cr.has_option('description', 'version'):
+            self.template_version = cr.get('description', 'version')
 
         # read in page options
         if cr.has_option('page', 'width'):
             self.pagew = str2len(cr.get('page', 'width'))
         if cr.has_option('page', 'height'):
             self.pageh = str2len(cr.get('page', 'height'))
         if cr.has_option('page', 'sidemargin'):
```

### Comparing `metarace-2.1.4/src/metarace/riderdb.py` & `metarace-2.1.5/src/metarace/riderdb.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/strops.py` & `metarace-2.1.5/src/metarace/strops.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/telegraph.py` & `metarace-2.1.5/src/metarace/telegraph.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/timy.py` & `metarace-2.1.5/src/metarace/timy.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/tod.py` & `metarace-2.1.5/src/metarace/tod.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace/unt4.py` & `metarace-2.1.5/src/metarace/unt4.py`

 * *Files identical despite different names*

### Comparing `metarace-2.1.4/src/metarace.egg-info/PKG-INFO` & `metarace-2.1.5/src/metarace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metarace
-Version: 2.1.4
+Version: 2.1.5
 Summary: Cyclesport results and timing toolkit
 Author-email: Nathan Fraser <ndf-zz@6-v.org>
 License: MIT
 Project-URL: homepage, https://github.com/ndf-zz/metarace
 Keywords: cyclesport,results,timing
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Other/Nonlisted Topic
```

### Comparing `metarace-2.1.4/src/metarace.egg-info/SOURCES.txt` & `metarace-2.1.5/src/metarace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

