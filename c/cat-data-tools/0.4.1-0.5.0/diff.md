# Comparing `tmp/cat_data_tools-0.4.1.tar.gz` & `tmp/cat_data_tools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_data_tools-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cat_data_tools-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cat_data_tools-0.4.1.tar` & `cat_data_tools-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      353 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/README.md
--rw-r--r--   0        0        0      125 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/__init__.py
--rw-r--r--   0        0        0      670 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/cli.py
--rw-r--r--   0        0        0      788 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/cat_data_tools/filter_data_by_month.py
--rw-r--r--   0        0        0      475 2023-07-28 20:34:27.716313 cat_data_tools-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 cat_data_tools-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      353 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/README.md
+-rw-r--r--   0        0        0      174 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/cat_data_tools/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/cat_data_tools/cli.py
+-rw-r--r--   0        0        0      783 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/cat_data_tools/filter_data_between_years.py
+-rw-r--r--   0        0        0      788 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/cat_data_tools/filter_data_by_month.py
+-rw-r--r--   0        0        0      475 2023-07-31 16:25:16.689893 cat_data_tools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      791 1970-01-01 00:00:00.000000 cat_data_tools-0.5.0/PKG-INFO
```

### Comparing `cat_data_tools-0.4.1/cat_data_tools/filter_data_by_month.py` & `cat_data_tools-0.5.0/cat_data_tools/filter_data_by_month.py`

 * *Files identical despite different names*

### Comparing `cat_data_tools-0.4.1/PKG-INFO` & `cat_data_tools-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cat_data_tools
-Version: 0.4.1
+Version: 0.5.0
 Summary: A template Python module
 Home-page: https://github.com/IslasGECI/cat_data_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cat_data_tools Version: 0.4.1 Summary: A template
+Metadata-Version: 2.1 Name: cat_data_tools Version: 0.5.0 Summary: A template
 Python module Home-page: https://github.com/IslasGECI/cat_data_tools Author:
 Ciencia de Datos â¢ GECI Author-email: ciencia.datos@islas.org.mx Requires-
 Python: >=3.9 Description-Content-Type: text/markdown Classifier: License ::
 OSI Approved :: GNU General Public License v3 or later (GPLv3+) Requires-Dist:
 numpy Requires-Dist: pandas Requires-Dist: typer # Cat data tools [https://
 www.islas.org.mx/img/logo.svg] [![codecov](https://codecov.io/gh/IslasGECI/
 cat_data_tools/branch/develop/graph/badge.svg?token=MvLBzyGSH3)](https://
```

