# Comparing `tmp/easy-reports-1.0.0.tar.gz` & `tmp/easy-reports-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-reports-1.0.0.tar", last modified: Sat Jul 29 13:54:46 2023, max compression
+gzip compressed data, was "easy-reports-1.0.1.tar", last modified: Mon Jul 31 17:31:04 2023, max compression
```

## Comparing `easy-reports-1.0.0.tar` & `easy-reports-1.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.956251 easy-reports-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-29 13:54:26.000000 easy-reports-1.0.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-29 13:54:26.000000 easy-reports-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-29 13:54:46.956251 easy-reports-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-29 13:54:26.000000 easy-reports-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-29 13:54:26.000000 easy-reports-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:54:46.956251 easy-reports-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.952251 easy-reports-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.956251 easy-reports-1.0.0/src/easy_reports/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.956251 easy-reports-1.0.0/src/easy_reports/boilerplate/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/boilerplate/report.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/email_smtplib.py
--rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-29 13:54:26.000000 easy-reports-1.0.0/src/easy_reports/excel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.956251 easy-reports-1.0.0/src/easy_reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 13:54:46.000000 easy-reports-1.0.0/src/easy_reports.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:46.956251 easy-reports-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/settings_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/settings_test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/settings_test_excel.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/settings_test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-29 13:54:26.000000 easy-reports-1.0.0/tests/test_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.542195 easy-reports-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-31 17:30:42.000000 easy-reports-1.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 17:30:42.000000 easy-reports-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-31 17:31:04.542195 easy-reports-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-07-31 17:30:42.000000 easy-reports-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-31 17:30:42.000000 easy-reports-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:31:04.542195 easy-reports-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.538195 easy-reports-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.538195 easy-reports-1.0.1/src/easy_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.538195 easy-reports-1.0.1/src/easy_reports/boilerplate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/boilerplate/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9423 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/email_smtplib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-07-31 17:30:42.000000 easy-reports-1.0.1/src/easy_reports/excel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.538195 easy-reports-1.0.1/src/easy_reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 17:31:04.000000 easy-reports-1.0.1/src/easy_reports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:31:04.542195 easy-reports-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/settings_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/settings_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/settings_test_excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/settings_test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-31 17:30:42.000000 easy-reports-1.0.1/tests/test_excel.py
```

### Comparing `easy-reports-1.0.0/LICENCE` & `easy-reports-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/PKG-INFO` & `easy-reports-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-reports
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simplified Report configuration, generation and distribution
 Author-email: Grzegorz Gyczew <ggyczew@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/ggyczew/ggy_easy_reports
 Project-URL: changelog, https://github.com/ggyczew/ggy_easy_reports/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `easy-reports-1.0.0/README.md` & `easy-reports-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/pyproject.toml` & `easy-reports-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "easy-reports"
-version = "1.0.0"
+version = "1.0.1"
 description = "Simplified Report configuration, generation and distribution"
 readme = "README.md"
 requires-python = ">=3.9.0"
 license = { text = "MIT" }
 authors = [{ name = "Grzegorz Gyczew", email = "ggyczew@gmail.com" }]
 
 classifiers = [
```

### Comparing `easy-reports-1.0.0/src/easy_reports/base.py` & `easy-reports-1.0.1/src/easy_reports/base.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/boilerplate/report.py` & `easy-reports-1.0.1/src/easy_reports/boilerplate/report.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/cli.py` & `easy-reports-1.0.1/src/easy_reports/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import click
 from easy_reports import EasyReport
+from pathlib import Path
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -15,15 +16,17 @@
     help="New report symbol. Will be used to create folder for it's definition",
 )
 def create(symbol):
     """Create new report boilerplate"""
     click.echo(f"Creating report {symbol}...")
 
     app = EasyReport()
-    app.base_config.from_pyfile('settings.py')
+
+    if Path('settings.py').exists():
+        app.base_config.from_pyfile('settings.py')
     app.create_boilerplate(symbol)
 
 
 def main() -> None:
     cli()
```

### Comparing `easy-reports-1.0.0/src/easy_reports/config.py` & `easy-reports-1.0.1/src/easy_reports/config.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/data.py` & `easy-reports-1.0.1/src/easy_reports/data.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/defaults.py` & `easy-reports-1.0.1/src/easy_reports/defaults.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/email.py` & `easy-reports-1.0.1/src/easy_reports/email.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/email_smtplib.py` & `easy-reports-1.0.1/src/easy_reports/email_smtplib.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports/excel.py` & `easy-reports-1.0.1/src/easy_reports/excel.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/src/easy_reports.egg-info/PKG-INFO` & `easy-reports-1.0.1/src/easy_reports.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-reports
-Version: 1.0.0
+Version: 1.0.1
 Summary: Simplified Report configuration, generation and distribution
 Author-email: Grzegorz Gyczew <ggyczew@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/ggyczew/ggy_easy_reports
 Project-URL: changelog, https://github.com/ggyczew/ggy_easy_reports/main/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `easy-reports-1.0.0/src/easy_reports.egg-info/SOURCES.txt` & `easy-reports-1.0.1/src/easy_reports.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/sample_data.py` & `easy-reports-1.0.1/tests/sample_data.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/settings_test_base.py` & `easy-reports-1.0.1/tests/settings_test_base.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/settings_test_data.py` & `easy-reports-1.0.1/tests/settings_test_data.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/settings_test_excel.py` & `easy-reports-1.0.1/tests/settings_test_excel.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/settings_test_report.py` & `easy-reports-1.0.1/tests/settings_test_report.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/test_base.py` & `easy-reports-1.0.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/test_config.py` & `easy-reports-1.0.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/test_data.py` & `easy-reports-1.0.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `easy-reports-1.0.0/tests/test_excel.py` & `easy-reports-1.0.1/tests/test_excel.py`

 * *Files identical despite different names*

