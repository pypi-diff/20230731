# Comparing `tmp/pycln-2.1.7.tar.gz` & `tmp/pycln-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycln-2.1.7.tar", max compression
+gzip compressed data, was "pycln-2.2.0.tar", max compression
```

## Comparing `pycln-2.1.7.tar` & `pycln-2.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1099 2023-01-16 09:14:47.289812 pycln-2.1.7/LICENSE
--rw-r--r--   0        0        0     7370 2023-05-31 14:51:44.454169 pycln-2.1.7/README.md
--rw-r--r--   0        0        0     1160 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/__init__.py
--rw-r--r--   0        0        0      113 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/__main__.py
--rw-r--r--   0        0        0     6828 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/cli.py
--rw-r--r--   0        0        0       26 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/utils/__init__.py
--rw-r--r--   0        0        0     3192 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/utils/_exceptions.py
--rw-r--r--   0        0        0     1813 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/utils/_nodes.py
--rw-r--r--   0        0        0     7477 2023-05-26 13:19:42.548063 pycln-2.1.7/pycln/utils/config.py
--rw-r--r--   0        0        0     3908 2023-05-31 14:51:44.464169 pycln-2.1.7/pycln/utils/iou.py
--rw-r--r--   0        0        0    12640 2023-05-31 14:51:44.464169 pycln-2.1.7/pycln/utils/pathu.py
--rw-r--r--   0        0        0    21013 2023-07-19 15:43:44.529950 pycln-2.1.7/pycln/utils/refactor.py
--rw-r--r--   0        0        0     4138 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/utils/regexu.py
--rw-r--r--   0        0        0    18739 2023-01-16 09:14:47.309812 pycln-2.1.7/pycln/utils/report.py
--rw-r--r--   0        0        0    35157 2023-07-27 12:47:16.416601 pycln-2.1.7/pycln/utils/scan.py
--rw-r--r--   0        0        0     8055 2023-01-16 13:00:31.890686 pycln-2.1.7/pycln/utils/transform.py
--rw-r--r--   0        0        0     1805 2023-07-27 12:47:16.416601 pycln-2.1.7/pyproject.toml
--rw-r--r--   0        0        0       66 2023-01-16 09:14:47.329812 pycln-2.1.7/vendor/custom/__init__.py
--rw-r--r--   0        0        0     2018 2023-01-16 09:14:47.329812 pycln-2.1.7/vendor/custom/_site.py
--rw-r--r--   0        0        0     8637 1970-01-01 00:00:00.000000 pycln-2.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-01-16 09:14:47.289812 pycln-2.2.0/LICENSE
+-rw-r--r--   0        0        0     7370 2023-05-31 14:51:44.454169 pycln-2.2.0/README.md
+-rw-r--r--   0        0        0     1160 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/__init__.py
+-rw-r--r--   0        0        0      113 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/__main__.py
+-rw-r--r--   0        0        0     6828 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/cli.py
+-rw-r--r--   0        0        0       26 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/__init__.py
+-rw-r--r--   0        0        0     3192 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/_exceptions.py
+-rw-r--r--   0        0        0     1813 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/_nodes.py
+-rw-r--r--   0        0        0     7477 2023-05-26 13:19:42.548063 pycln-2.2.0/pycln/utils/config.py
+-rw-r--r--   0        0        0     3908 2023-05-31 14:51:44.464169 pycln-2.2.0/pycln/utils/iou.py
+-rw-r--r--   0        0        0    12640 2023-05-31 14:51:44.464169 pycln-2.2.0/pycln/utils/pathu.py
+-rw-r--r--   0        0        0    21013 2023-07-19 15:43:44.529950 pycln-2.2.0/pycln/utils/refactor.py
+-rw-r--r--   0        0        0     4138 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/regexu.py
+-rw-r--r--   0        0        0    18739 2023-01-16 09:14:47.309812 pycln-2.2.0/pycln/utils/report.py
+-rw-r--r--   0        0        0    35157 2023-07-27 12:47:16.416601 pycln-2.2.0/pycln/utils/scan.py
+-rw-r--r--   0        0        0     8055 2023-01-16 13:00:31.890686 pycln-2.2.0/pycln/utils/transform.py
+-rw-r--r--   0        0        0     1776 2023-07-31 15:33:30.490746 pycln-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-01-16 09:14:47.329812 pycln-2.2.0/vendor/custom/__init__.py
+-rw-r--r--   0        0        0     2018 2023-01-16 09:14:47.329812 pycln-2.2.0/vendor/custom/_site.py
+-rw-r--r--   0        0        0     8599 1970-01-01 00:00:00.000000 pycln-2.2.0/PKG-INFO
```

### Comparing `pycln-2.1.7/LICENSE` & `pycln-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/README.md` & `pycln-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/__init__.py` & `pycln-2.2.0/pycln/__init__.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/cli.py` & `pycln-2.2.0/pycln/cli.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/_exceptions.py` & `pycln-2.2.0/pycln/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/_nodes.py` & `pycln-2.2.0/pycln/utils/_nodes.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/config.py` & `pycln-2.2.0/pycln/utils/config.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/iou.py` & `pycln-2.2.0/pycln/utils/iou.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/pathu.py` & `pycln-2.2.0/pycln/utils/pathu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/refactor.py` & `pycln-2.2.0/pycln/utils/refactor.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/regexu.py` & `pycln-2.2.0/pycln/utils/regexu.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/report.py` & `pycln-2.2.0/pycln/utils/report.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/scan.py` & `pycln-2.2.0/pycln/utils/scan.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pycln/utils/transform.py` & `pycln-2.2.0/pycln/utils/transform.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/pyproject.toml` & `pycln-2.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pycln"
-version = "2.1.7"
+version = "2.2.0"
 description = "A formatter for finding and removing unused import statements."
 authors = ["Hadi Alqattan <alqattanhadizaki@gmail.com>"]
 homepage = "https://hadialqattan.github.io/pycln"
 repository = "https://github.com/hadialqattan/pycln"
 keywords = ["formatter", "linter", "quality-assurance", "tools", "cli"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -21,20 +21,20 @@
 packages = [{ include = "pycln" }, { include = "vendor" }]
 
 [tool.poetry.scripts]
 pycln = "pycln.cli:app"
 
 [tool.poetry.dependencies]
 python = ">=3.6.2, <4"
-typer = ">=0.4.1,<0.10.0"
+typer = ">=0.4.1"
 dataclasses = {version = "^0.7", python = "3.6"}
-pyyaml = ">=5.3.1,<7.0.0"
-pathspec = ">=0.9.0,<0.12.0"
-tomlkit = "^0.11.1"
-libcst = [{version = ">=0.3.10,<1.1.0", python = ">=3.7"}, {version = ">=0.3.10,<0.4.0", python = "<3.7"}]
+pyyaml = ">=5.3.1"
+pathspec = ">=0.9.0"
+tomlkit = ">=0.11.1"
+libcst = [{version = ">=0.3.10", python = ">=3.7"}, {version = ">=0.3.10,<0.4.0", python = "<3.7"}]
 
 [tool.poetry.dev-dependencies]
 requests = "^2.24.0"
 semver = "^2.10.2"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
 pytest-randomly = "^3.4.1"
```

### Comparing `pycln-2.1.7/vendor/custom/_site.py` & `pycln-2.2.0/vendor/custom/_site.py`

 * *Files identical despite different names*

### Comparing `pycln-2.1.7/PKG-INFO` & `pycln-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycln
-Version: 2.1.7
+Version: 2.2.0
 Summary: A formatter for finding and removing unused import statements.
 Home-page: https://hadialqattan.github.io/pycln
 License: MIT
 Keywords: formatter,linter,quality-assurance,tools,cli
 Author: Hadi Alqattan
 Author-email: alqattanhadizaki@gmail.com
 Requires-Python: >=3.6.2,<4
@@ -15,20 +15,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
+Requires-Dist: libcst (>=0.3.10) ; python_version >= "3.7"
 Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7"
-Requires-Dist: libcst (>=0.3.10,<1.1.0) ; python_version >= "3.7"
-Requires-Dist: pathspec (>=0.9.0,<0.12.0)
-Requires-Dist: pyyaml (>=5.3.1,<7.0.0)
-Requires-Dist: tomlkit (>=0.11.1,<0.12.0)
-Requires-Dist: typer (>=0.4.1,<0.10.0)
+Requires-Dist: pathspec (>=0.9.0)
+Requires-Dist: pyyaml (>=5.3.1)
+Requires-Dist: tomlkit (>=0.11.1)
+Requires-Dist: typer (>=0.4.1)
 Project-URL: Repository, https://github.com/hadialqattan/pycln
 Description-Content-Type: text/markdown
 
 <img src="https://raw.githubusercontent.com/hadialqattan/pycln/master/docs/_media/logo-background.png" width="100%" alt="Logo">
 
 <h2 align="center">
     A formatter for finding and removing unused import statements.
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: pycln Version: 2.1.7 Summary: A formatter for
+Metadata-Version: 2.1 Name: pycln Version: 2.2.0 Summary: A formatter for
 finding and removing unused import statements. Home-page: https://
 hadialqattan.github.io/pycln License: MIT Keywords: formatter,linter,quality-
 assurance,tools,cli Author: Hadi Alqattan Author-email:
 alqattanhadizaki@gmail.com Requires-Python: >=3.6.2,<4 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6 Classifier: Topic ::
 Utilities Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version == "3.6"
-Requires-Dist: libcst (>=0.3.10,<0.4.0) ; python_version < "3.7" Requires-Dist:
-libcst (>=0.3.10,<1.1.0) ; python_version >= "3.7" Requires-Dist: pathspec
-(>=0.9.0,<0.12.0) Requires-Dist: pyyaml (>=5.3.1,<7.0.0) Requires-Dist: tomlkit
-(>=0.11.1,<0.12.0) Requires-Dist: typer (>=0.4.1,<0.10.0) Project-URL:
-Repository, https://github.com/hadialqattan/pycln Description-Content-Type:
-text/markdown [Logo]
+Requires-Dist: libcst (>=0.3.10) ; python_version >= "3.7" Requires-Dist:
+libcst (>=0.3.10,<0.4.0) ; python_version < "3.7" Requires-Dist: pathspec
+(>=0.9.0) Requires-Dist: pyyaml (>=5.3.1) Requires-Dist: tomlkit (>=0.11.1)
+Requires-Dist: typer (>=0.4.1) Project-URL: Repository, https://github.com/
+hadialqattan/pycln Description-Content-Type: text/markdown [Logo]
   ***** A formatter for finding and removing unused import statements. *****
    [Pycln_Docs] [CI] [CD] [FUZZ] [Codacy_Badge] [Codecov] [Maintainability]
  [PYPI - Python Version] [PYPI_-_Pycln_Version] [Total_Downloads] [Downloads]
 [Forks] [Stars] [Issues] [Pull_Requests] [Contributors] [Last_Commit] [License]
    [Docstrings:_reStructuredText] [Code_style:_black] [Code_style:_prettier]
 --- **[Read the documentation on Github pages!](https://hadialqattan.github.io/
 pycln)** --- ## Installation and usage ### Installation Pycln requires Python
```

