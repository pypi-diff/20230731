# Comparing `tmp/qsharp-chemistry-0.28.291393b1.tar.gz` & `tmp/qsharp-chemistry-0.28.291394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsharp-chemistry-0.28.291393b1.tar", last modified: Fri Jul 28 04:11:28 2023, max compression
+gzip compressed data, was "qsharp-chemistry-0.28.291394.tar", last modified: Fri Jul 28 04:05:45 2023, max compression
```

## Comparing `qsharp-chemistry-0.28.291393b1.tar` & `qsharp-chemistry-0.28.291394.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/
--rw-rw-rw-   0        0        0     2900 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-07-28 03:56:44.000000 qsharp-chemistry-0.28.291393b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/qsharp/
-drwxrwxrwx   0        0        0        0 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/qsharp/chemistry/
--rw-rw-rw-   0        0        0     7166 2023-07-28 03:56:44.000000 qsharp-chemistry-0.28.291393b1/qsharp/chemistry/__init__.py
--rw-rw-rw-   0        0        0      270 2023-07-28 04:11:27.000000 qsharp-chemistry-0.28.291393b1/qsharp/chemistry/version.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/qsharp/tests/
--rw-rw-rw-   0        0        0        0 2023-07-28 03:56:44.000000 qsharp-chemistry-0.28.291393b1/qsharp/tests/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-07-28 03:56:44.000000 qsharp-chemistry-0.28.291393b1/qsharp/tests/test_chemistry.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/
--rw-rw-rw-   0        0        0     2900 2023-07-28 04:11:28.000000 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-07-28 04:11:28.000000 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:11:28.000000 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-28 04:11:28.000000 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 04:11:28.000000 qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 04:11:28.339594 qsharp-chemistry-0.28.291393b1/setup.cfg
--rw-rw-rw-   0        0        0     2148 2023-07-28 03:56:44.000000 qsharp-chemistry-0.28.291393b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/
+-rw-rw-rw-   0        0        0     2898 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-07-28 03:52:59.000000 qsharp-chemistry-0.28.291394/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/qsharp/
+drwxrwxrwx   0        0        0        0 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/qsharp/chemistry/
+-rw-rw-rw-   0        0        0     7166 2023-07-28 03:52:59.000000 qsharp-chemistry-0.28.291394/qsharp/chemistry/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp/chemistry/version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/qsharp/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:52:59.000000 qsharp-chemistry-0.28.291394/qsharp/tests/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-07-28 03:52:59.000000 qsharp-chemistry-0.28.291394/qsharp/tests/test_chemistry.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/
+-rw-rw-rw-   0        0        0     2898 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 04:05:45.000000 qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:05:45.918783 qsharp-chemistry-0.28.291394/setup.cfg
+-rw-rw-rw-   0        0        0     2148 2023-07-28 03:52:59.000000 qsharp-chemistry-0.28.291394/setup.py
```

### Comparing `qsharp-chemistry-0.28.291393b1/PKG-INFO` & `qsharp-chemistry-0.28.291394/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-chemistry
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python chemistry libraries for Q#.
 Home-page: https://github.com/microsoft/QuantumLibraries
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-chemistry-0.28.291393b1/README.md` & `qsharp-chemistry-0.28.291394/README.md`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.291393b1/qsharp/chemistry/__init__.py` & `qsharp-chemistry-0.28.291394/qsharp/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.291393b1/qsharp/tests/test_chemistry.py` & `qsharp-chemistry-0.28.291394/qsharp/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.291393b1/qsharp_chemistry.egg-info/PKG-INFO` & `qsharp-chemistry-0.28.291394/qsharp_chemistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-chemistry
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python chemistry libraries for Q#.
 Home-page: https://github.com/microsoft/QuantumLibraries
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-chemistry-0.28.291393b1/setup.py` & `qsharp-chemistry-0.28.291394/setup.py`

 * *Files identical despite different names*

