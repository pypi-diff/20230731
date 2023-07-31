# Comparing `tmp/edgar-py-0.1.0.tar.gz` & `tmp/edgar-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgar-py-0.1.0.tar", last modified: Wed Jul 26 06:17:16 2023, max compression
+gzip compressed data, was "edgar-py-0.2.0.tar", last modified: Mon Jul 31 04:21:36 2023, max compression
```

## Comparing `edgar-py-0.1.0.tar` & `edgar-py-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.753755 edgar-py-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-07-19 23:13:03.000000 edgar-py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2109 2023-07-26 06:17:16.753755 edgar-py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-07-19 23:08:24.000000 edgar-py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.627907 edgar-py-0.1.0/edgar/
--rw-rw-rw-   0        0        0       40 2023-07-26 06:12:34.000000 edgar-py-0.1.0/edgar/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-19 23:08:10.000000 edgar-py-0.1.0/edgar/__main__.py
--rw-rw-rw-   0        0        0     2526 2023-07-26 06:12:34.000000 edgar-py-0.1.0/edgar/cik.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:17:16.745755 edgar-py-0.1.0/edgar_py.egg-info/
--rw-rw-rw-   0        0        0     2109 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      479 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 06:17:16.000000 edgar-py-0.1.0/edgar_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1714 2023-07-26 06:14:42.000000 edgar-py-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 06:17:16.753755 edgar-py-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 04:21:36.249349 edgar-py-0.2.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-19 23:13:03.000000 edgar-py-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2058 2023-07-31 04:21:36.249349 edgar-py-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-07-19 23:08:24.000000 edgar-py-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 04:21:36.189335 edgar-py-0.2.0/edgar/
+-rw-rw-rw-   0        0        0       10 2023-07-31 04:18:27.000000 edgar-py-0.2.0/edgar/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-19 23:08:10.000000 edgar-py-0.2.0/edgar/__main__.py
+-rw-rw-rw-   0        0        0    18595 2023-07-31 04:18:27.000000 edgar-py-0.2.0/edgar/cik.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:21:36.249349 edgar-py-0.2.0/edgar_py.egg-info/
+-rw-rw-rw-   0        0        0     2058 2023-07-31 04:21:36.000000 edgar-py-0.2.0/edgar_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-07-31 04:21:36.000000 edgar-py-0.2.0/edgar_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:21:36.000000 edgar-py-0.2.0/edgar_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      479 2023-07-31 04:21:36.000000 edgar-py-0.2.0/edgar_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 04:21:36.000000 edgar-py-0.2.0/edgar_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1668 2023-07-31 04:19:47.000000 edgar-py-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:21:36.249349 edgar-py-0.2.0/setup.cfg
```

### Comparing `edgar-py-0.1.0/LICENSE` & `edgar-py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgar-py-0.1.0/PKG-INFO` & `edgar-py-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Web scraper and API wrapper for the SEC EDGAR tool.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,14 @@
         
 Project-URL: homepage, https://github.com/JacobLee23/EDGAR-py
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `edgar-py-0.1.0/edgar_py.egg-info/PKG-INFO` & `edgar-py-0.2.0/edgar_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgar-py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Web scraper and API wrapper for the SEC EDGAR tool.
 Author-email: Jacob Lee <Jacob.J.Lee@outlook.com>
 License: MIT License
         
         Copyright (c) 2023 Jacob Lee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -27,15 +27,14 @@
         
 Project-URL: homepage, https://github.com/JacobLee23/EDGAR-py
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `edgar-py-0.1.0/pyproject.toml` & `edgar-py-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="edgar-py"
-version="0.1.0"
+version="0.2.0"
 description = "Web scraper and API wrapper for the SEC EDGAR tool."
 readme = "README.md"
 authors = [ { name = "Jacob Lee", email = "Jacob.J.Lee@outlook.com" } ]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Office/Business :: Financial :: Investment",
 ]
 requires-python = ">=3.8"
 dependencies = [
```

