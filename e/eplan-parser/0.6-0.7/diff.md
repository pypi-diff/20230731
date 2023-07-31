# Comparing `tmp/eplan_parser-0.6.tar.gz` & `tmp/eplan_parser-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eplan_parser-0.6.tar", last modified: Thu Feb 23 10:42:34 2023, max compression
+gzip compressed data, was "eplan_parser-0.7.tar", last modified: Mon Jul 31 09:17:58 2023, max compression
```

## Comparing `eplan_parser-0.6.tar` & `eplan_parser-0.7.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-23 10:42:34.901036 eplan_parser-0.6/
--rw-r--r--   0 alex      (1000) alex      (1000)     1063 2023-02-20 16:10:05.000000 eplan_parser-0.6/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     2103 2023-02-23 10:42:34.900036 eplan_parser-0.6/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1525 2023-02-23 10:29:46.000000 eplan_parser-0.6/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-23 10:42:34.899036 eplan_parser-0.6/eplan_parser/
--rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-02-20 16:17:47.000000 eplan_parser-0.6/eplan_parser/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)    11262 2023-02-23 10:40:52.000000 eplan_parser-0.6/eplan_parser/output_parser.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-02-23 10:42:34.900036 eplan_parser-0.6/eplan_parser.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     2103 2023-02-23 10:42:34.000000 eplan_parser-0.6/eplan_parser.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      270 2023-02-23 10:42:34.000000 eplan_parser-0.6/eplan_parser.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-02-23 10:42:34.000000 eplan_parser-0.6/eplan_parser.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       78 2023-02-23 10:42:34.000000 eplan_parser-0.6/eplan_parser.egg-info/entry_points.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       13 2023-02-23 10:42:34.000000 eplan_parser-0.6/eplan_parser.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      717 2023-02-23 10:42:23.000000 eplan_parser-0.6/pyproject.toml
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-02-23 10:42:34.901036 eplan_parser-0.6/setup.cfg
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-31 09:17:58.651107 eplan_parser-0.7/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1063 2023-02-20 16:10:05.000000 eplan_parser-0.7/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     2103 2023-07-31 09:17:58.650107 eplan_parser-0.7/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1525 2023-02-23 10:29:46.000000 eplan_parser-0.7/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-31 09:17:58.649107 eplan_parser-0.7/eplan_parser/
+-rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-02-20 16:17:47.000000 eplan_parser-0.7/eplan_parser/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1451 2023-06-01 07:39:25.000000 eplan_parser-0.7/eplan_parser/get_keys.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3563 2023-06-01 09:24:20.000000 eplan_parser-0.7/eplan_parser/input_gen.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    11423 2023-07-31 09:16:17.000000 eplan_parser-0.7/eplan_parser/output_parser.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-07-31 09:17:58.650107 eplan_parser-0.7/eplan_parser.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     2103 2023-07-31 09:17:58.000000 eplan_parser-0.7/eplan_parser.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)      321 2023-07-31 09:17:58.000000 eplan_parser-0.7/eplan_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-07-31 09:17:58.000000 eplan_parser-0.7/eplan_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       78 2023-07-31 09:17:58.000000 eplan_parser-0.7/eplan_parser.egg-info/entry_points.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       13 2023-07-31 09:17:58.000000 eplan_parser-0.7/eplan_parser.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      717 2023-07-31 09:17:39.000000 eplan_parser-0.7/pyproject.toml
+-rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-07-31 09:17:58.651107 eplan_parser-0.7/setup.cfg
```

### Comparing `eplan_parser-0.6/LICENSE` & `eplan_parser-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `eplan_parser-0.6/PKG-INFO` & `eplan_parser-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eplan_parser
-Version: 0.6
+Version: 0.7
 Summary: Parser for the output files of EnergyPLAN
 Author-email: Alex Sartori <alex.sartori1997@gmail.com>
 Project-URL: Homepage, https://github.com/AlexSartori/eplan_parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eplan_parser-0.6/README.md` & `eplan_parser-0.7/README.md`

 * *Files identical despite different names*

### Comparing `eplan_parser-0.6/eplan_parser/output_parser.py` & `eplan_parser-0.7/eplan_parser/output_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 
 import re, sys, json
+import os.path
 
 
 def __print_err(msg):
     print(' \u001b[31m✖\u001b[0m - ' + msg)
 
 def __print_wrn(msg):
     print(' \u001b[33m!\u001b[0m - ' + msg)
@@ -189,15 +190,15 @@
 
         for i, v in enumerate(vals):
             col = header[i]
             data[col].append(v)
     
     return data
 
-    
+
 def get_yearly_totals_header(lines, index):
     if not check_index(lines, index, 'Yearly Totals'):
         __print_err('Cannot find header for Yearly Totals in index')
         return None
     
     idx = index['Yearly Totals']
     line_1, line_2 = lines[idx-3], lines[idx-2]
@@ -253,17 +254,20 @@
         (fname, written_bytes/(1024*1024), written_bytes)
     )
 
 
 def read_energyplan_file(fname):
     lines = []
     
-    with open(fname, encoding='iso-8859-15') as f:
-        lines = f.readlines()
-        __print_suc('Read %d lines from "%s"' % (len(lines), fname))
+    if os.path.exists(fname) and os.path.isfile(fname):
+        with open(fname, encoding='iso-8859-15') as f:
+            lines = f.readlines()
+            __print_suc('Read %d lines from "%s"' % (len(lines), fname))
+    else:
+        __print_err('File "%s" does not exist or is not a file' % fname)
 
     return lines
 
 
 def load_dataset(fname):
     lines = read_energyplan_file(fname)
     dataset = {}
@@ -342,8 +346,7 @@
         return
 
     # Load the dataset
     dataset = load_dataset(sys.argv[1])
 
     # Export the dataset
     export_to_json(sys.argv[2], dataset)
-
```

### Comparing `eplan_parser-0.6/eplan_parser.egg-info/PKG-INFO` & `eplan_parser-0.7/eplan_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eplan-parser
-Version: 0.6
+Version: 0.7
 Summary: Parser for the output files of EnergyPLAN
 Author-email: Alex Sartori <alex.sartori1997@gmail.com>
 Project-URL: Homepage, https://github.com/AlexSartori/eplan_parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `eplan_parser-0.6/pyproject.toml` & `eplan_parser-0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "eplan_parser"
-version = "0.6"
+version = "0.7"
 authors = [
   { name="Alex Sartori", email="alex.sartori1997@gmail.com" },
 ]
 description = "Parser for the output files of EnergyPLAN"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

