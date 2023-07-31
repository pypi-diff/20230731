# Comparing `tmp/calitp_data_analysis-2023.7.25.tar.gz` & `tmp/calitp_data_analysis-2023.7.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_data_analysis-2023.7.25.tar", max compression
+gzip compressed data, was "calitp_data_analysis-2023.7.31.tar", max compression
```

## Comparing `calitp_data_analysis-2023.7.25.tar` & `calitp_data_analysis-2023.7.31.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-24 20:14:34.415032 calitp_data_analysis-2023.7.25/calitp_data_analysis/__init__.py
--rw-r--r--   0        0        0     1427 2023-07-24 20:14:34.415355 calitp_data_analysis-2023.7.25/calitp_data_analysis/magics.py
--rw-r--r--   0        0        0     3981 2023-07-25 15:57:06.188713 calitp_data_analysis-2023.7.25/calitp_data_analysis/sql.py
--rw-r--r--   0        0        0     3273 2023-07-25 15:55:15.481636 calitp_data_analysis-2023.7.25/calitp_data_analysis/tables.py
--rw-r--r--   0        0        0      901 2023-07-25 19:38:01.858484 calitp_data_analysis-2023.7.25/pyproject.toml
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 calitp_data_analysis-2023.7.25/PKG-INFO
+-rw-r--r--   0        0        0      340 2023-07-31 21:14:30.982755 calitp_data_analysis-2023.7.31/calitp_data_analysis/__init__.py
+-rw-r--r--   0        0        0     1427 2023-07-31 15:40:25.466680 calitp_data_analysis-2023.7.31/calitp_data_analysis/magics.py
+-rw-r--r--   0        0        0     3981 2023-07-31 15:40:25.467222 calitp_data_analysis-2023.7.31/calitp_data_analysis/sql.py
+-rw-r--r--   0        0        0     3273 2023-07-31 15:40:25.467759 calitp_data_analysis-2023.7.31/calitp_data_analysis/tables.py
+-rw-r--r--   0        0        0      901 2023-07-31 21:13:28.929910 calitp_data_analysis-2023.7.31/pyproject.toml
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 calitp_data_analysis-2023.7.31/PKG-INFO
```

### Comparing `calitp_data_analysis-2023.7.25/calitp_data_analysis/magics.py` & `calitp_data_analysis-2023.7.31/calitp_data_analysis/magics.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2023.7.25/calitp_data_analysis/sql.py` & `calitp_data_analysis-2023.7.31/calitp_data_analysis/sql.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2023.7.25/calitp_data_analysis/tables.py` & `calitp_data_analysis-2023.7.31/calitp_data_analysis/tables.py`

 * *Files identical despite different names*

### Comparing `calitp_data_analysis-2023.7.25/pyproject.toml` & `calitp_data_analysis-2023.7.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp-data-analysis"
-version = "2023.7.25"
+version = "2023.7.31"
 description = "Shared code for querying Cal-ITP data in notebooks, primarily."
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 
 [tool.poetry.dependencies]
 python = "~3.9"
 ipython = "^8.9.0"
 siuba = "^0.4.2"
```

### Comparing `calitp_data_analysis-2023.7.25/PKG-INFO` & `calitp_data_analysis-2023.7.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-data-analysis
-Version: 2023.7.25
+Version: 2023.7.31
 Summary: Shared code for querying Cal-ITP data in notebooks, primarily.
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: gcsfs (!=2022.7.1)
```

