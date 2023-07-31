# Comparing `tmp/merge_files-0.1.3.tar.gz` & `tmp/merge_files-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merge_files-0.1.3.tar", last modified: Sun Mar 26 00:48:48 2023, max compression
+gzip compressed data, was "merge_files-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `merge_files-0.1.3.tar` & `merge_files-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      178 2023-02-27 00:44:22.863557 merge_files-0.1.3/README.md
--rw-r--r--   0        0        0      894 2023-03-26 00:38:55.990759 merge_files-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       47 2023-03-01 03:35:55.029690 merge_files-0.1.3/src/merge_files/__init__.py
--rw-r--r--   0        0        0       62 2023-02-27 00:26:31.697843 merge_files-0.1.3/src/merge_files/__main__.py
--rwxr-xr-x   0        0        0     1299 2023-03-26 00:34:15.219091 merge_files-0.1.3/src/merge_files/main.py
--rw-r--r--   0        0        0      455 2023-03-26 00:35:20.783014 merge_files-0.1.3/src/merge_files/mergers/__init__.py
--rw-r--r--   0        0        0      843 2023-03-25 23:15:23.913685 merge_files-0.1.3/src/merge_files/mergers/concatenate.py
--rw-r--r--   0        0        0     1435 2023-03-25 23:15:23.917685 merge_files-0.1.3/src/merge_files/mergers/env.py
--rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 merge_files-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-07-31 13:10:11.944050 merge_files-0.1.4/README.md
+-rw-r--r--   0        0        0      894 2023-07-31 13:10:11.944050 merge_files-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-03-01 03:35:55.029690 merge_files-0.1.4/src/merge_files/__init__.py
+-rw-r--r--   0        0        0       62 2023-02-27 00:26:31.697843 merge_files-0.1.4/src/merge_files/__main__.py
+-rw-r--r--   0        0        0     2050 2023-07-31 13:11:16.784289 merge_files-0.1.4/src/merge_files/format/file/binary.py
+-rwxr-xr-x   0        0        0     1374 2023-07-31 13:13:44.956833 merge_files-0.1.4/src/merge_files/main.py
+-rw-r--r--   0        0        0      455 2023-07-31 13:10:11.944050 merge_files-0.1.4/src/merge_files/mergers/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-31 13:10:11.948051 merge_files-0.1.4/src/merge_files/mergers/concatenate.py
+-rw-r--r--   0        0        0     1435 2023-07-31 13:10:11.948051 merge_files-0.1.4/src/merge_files/mergers/env.py
+-rw-r--r--   0        0        0     1014 1970-01-01 00:00:00.000000 merge_files-0.1.4/PKG-INFO
```

### Comparing `merge_files-0.1.3/pyproject.toml` & `merge_files-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "merge_files"
 description = "Merge two .env files files together"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "Gareth Davidson", email = "gaz@bitplane.net" }
 ]
 
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `merge_files-0.1.3/src/merge_files/main.py` & `merge_files-0.1.4/src/merge_files/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,16 +33,19 @@
     Main entry point for the merge-files command line tool.
     """
     args = parse_args(sys.argv[1:])
 
     with open(args.source, "rb") as source_file:
         source = source_file.read()
 
-    with open(args.dest, "rb") as dest_file:
-        dest = dest_file.read()
+    if not os.path.exists(args.dest):
+        dest = b""
+    else:
+        with open(args.dest, "rb") as dest_file:
+            dest = dest_file.read()
 
     merger = get(args.source, args.dest)
     output_data = merger(source, dest, args.update)
 
     with open(args.dest, "wb") as dest_file:
         dest_file.write(output_data)
```

### Comparing `merge_files-0.1.3/src/merge_files/mergers/concatenate.py` & `merge_files-0.1.4/src/merge_files/mergers/concatenate.py`

 * *Files identical despite different names*

### Comparing `merge_files-0.1.3/src/merge_files/mergers/env.py` & `merge_files-0.1.4/src/merge_files/mergers/env.py`

 * *Files identical despite different names*

### Comparing `merge_files-0.1.3/PKG-INFO` & `merge_files-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merge_files
-Version: 0.1.3
+Version: 0.1.4
 Summary: Merge two .env files files together
 Author-email: Gareth Davidson <gaz@bitplane.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Public Domain
 Classifier: Operating System :: OS Independent
```

