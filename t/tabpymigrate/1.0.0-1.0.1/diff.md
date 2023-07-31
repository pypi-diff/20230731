# Comparing `tmp/tabpymigrate-1.0.0.tar.gz` & `tmp/tabpymigrate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabpymigrate-1.0.0.tar", last modified: Mon Jul 31 18:11:41 2023, max compression
+gzip compressed data, was "tabpymigrate-1.0.1.tar", last modified: Mon Jul 31 18:17:50 2023, max compression
```

## Comparing `tabpymigrate-1.0.0.tar` & `tabpymigrate-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:11:41.652236 tabpymigrate-1.0.0/
--rw-r--r--   0 pgopalak   (501) staff       (20)     1724 2023-07-31 18:11:41.652094 tabpymigrate-1.0.0/PKG-INFO
--rw-r--r--   0 pgopalak   (501) staff       (20)     1095 2023-07-30 15:16:24.000000 tabpymigrate-1.0.0/README.md
--rw-r--r--   0 pgopalak   (501) staff       (20)     1391 2023-07-31 18:10:43.000000 tabpymigrate-1.0.0/pyproject.toml
--rw-r--r--   0 pgopalak   (501) staff       (20)       38 2023-07-31 18:11:41.652280 tabpymigrate-1.0.0/setup.cfg
-drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:11:41.651007 tabpymigrate-1.0.0/tabpymigrate/
--rw-r--r--   0 pgopalak   (501) staff       (20)       39 2023-07-30 06:04:25.000000 tabpymigrate-1.0.0/tabpymigrate/__init__.py
--rw-r--r--   0 pgopalak   (501) staff       (20)      953 2023-07-27 19:46:46.000000 tabpymigrate-1.0.0/tabpymigrate/config.py
--rw-r--r--   0 pgopalak   (501) staff       (20)     3897 2023-07-30 13:38:55.000000 tabpymigrate-1.0.0/tabpymigrate/mapping.py
--rw-r--r--   0 pgopalak   (501) staff       (20)     6775 2023-07-30 13:10:05.000000 tabpymigrate-1.0.0/tabpymigrate/tabpymigrate.py
--rw-r--r--   0 pgopalak   (501) staff       (20)    11508 2023-07-30 10:44:34.000000 tabpymigrate-1.0.0/tabpymigrate/tabpymigrate_download.py
--rw-r--r--   0 pgopalak   (501) staff       (20)    14365 2023-07-30 13:46:29.000000 tabpymigrate-1.0.0/tabpymigrate/tabpymigrate_publish.py
-drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:11:41.651899 tabpymigrate-1.0.0/tabpymigrate.egg-info/
--rw-r--r--   0 pgopalak   (501) staff       (20)     1724 2023-07-31 18:11:41.000000 tabpymigrate-1.0.0/tabpymigrate.egg-info/PKG-INFO
--rw-r--r--   0 pgopalak   (501) staff       (20)      379 2023-07-31 18:11:41.000000 tabpymigrate-1.0.0/tabpymigrate.egg-info/SOURCES.txt
--rw-r--r--   0 pgopalak   (501) staff       (20)        1 2023-07-31 18:11:41.000000 tabpymigrate-1.0.0/tabpymigrate.egg-info/dependency_links.txt
--rw-r--r--   0 pgopalak   (501) staff       (20)      189 2023-07-31 18:11:41.000000 tabpymigrate-1.0.0/tabpymigrate.egg-info/requires.txt
--rw-r--r--   0 pgopalak   (501) staff       (20)       13 2023-07-31 18:11:41.000000 tabpymigrate-1.0.0/tabpymigrate.egg-info/top_level.txt
+drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:17:50.228350 tabpymigrate-1.0.1/
+-rw-r--r--   0 pgopalak   (501) staff       (20)     1858 2023-07-31 18:17:50.228190 tabpymigrate-1.0.1/PKG-INFO
+-rw-r--r--   0 pgopalak   (501) staff       (20)     1229 2023-07-31 18:17:23.000000 tabpymigrate-1.0.1/README.md
+-rw-r--r--   0 pgopalak   (501) staff       (20)     1391 2023-07-31 18:17:28.000000 tabpymigrate-1.0.1/pyproject.toml
+-rw-r--r--   0 pgopalak   (501) staff       (20)       38 2023-07-31 18:17:50.228397 tabpymigrate-1.0.1/setup.cfg
+drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:17:50.227041 tabpymigrate-1.0.1/tabpymigrate/
+-rw-r--r--   0 pgopalak   (501) staff       (20)       39 2023-07-30 06:04:25.000000 tabpymigrate-1.0.1/tabpymigrate/__init__.py
+-rw-r--r--   0 pgopalak   (501) staff       (20)      953 2023-07-27 19:46:46.000000 tabpymigrate-1.0.1/tabpymigrate/config.py
+-rw-r--r--   0 pgopalak   (501) staff       (20)     3897 2023-07-30 13:38:55.000000 tabpymigrate-1.0.1/tabpymigrate/mapping.py
+-rw-r--r--   0 pgopalak   (501) staff       (20)     6775 2023-07-30 13:10:05.000000 tabpymigrate-1.0.1/tabpymigrate/tabpymigrate.py
+-rw-r--r--   0 pgopalak   (501) staff       (20)    11508 2023-07-30 10:44:34.000000 tabpymigrate-1.0.1/tabpymigrate/tabpymigrate_download.py
+-rw-r--r--   0 pgopalak   (501) staff       (20)    14365 2023-07-30 13:46:29.000000 tabpymigrate-1.0.1/tabpymigrate/tabpymigrate_publish.py
+drwxr-xr-x   0 pgopalak   (501) staff       (20)        0 2023-07-31 18:17:50.227988 tabpymigrate-1.0.1/tabpymigrate.egg-info/
+-rw-r--r--   0 pgopalak   (501) staff       (20)     1858 2023-07-31 18:17:50.000000 tabpymigrate-1.0.1/tabpymigrate.egg-info/PKG-INFO
+-rw-r--r--   0 pgopalak   (501) staff       (20)      379 2023-07-31 18:17:50.000000 tabpymigrate-1.0.1/tabpymigrate.egg-info/SOURCES.txt
+-rw-r--r--   0 pgopalak   (501) staff       (20)        1 2023-07-31 18:17:50.000000 tabpymigrate-1.0.1/tabpymigrate.egg-info/dependency_links.txt
+-rw-r--r--   0 pgopalak   (501) staff       (20)      189 2023-07-31 18:17:50.000000 tabpymigrate-1.0.1/tabpymigrate.egg-info/requires.txt
+-rw-r--r--   0 pgopalak   (501) staff       (20)       13 2023-07-31 18:17:50.000000 tabpymigrate-1.0.1/tabpymigrate.egg-info/top_level.txt
```

### Comparing `tabpymigrate-1.0.0/PKG-INFO` & `tabpymigrate-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpymigrate
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python project to download and deploy objects to Tableau Server via REST API.
 Author-email: Tableau <kavikag00@gmail.com>
 Project-URL: repository, https://github.com/codespg/tabpymigrate
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 # TabPyMigrate
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your_username/TabPyMigrate/blob/main/LICENSE)
 
 > Short project description
 
 TabPyMigrate is a tool to migrate your Tableau Flow, Datasources, Workbooks from one server to another easily.
+This is similar to TabMigrate and works with Tableay Rest API to download and deploy tableau objects. Easy to configure/Run from CLI.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
```

### Comparing `tabpymigrate-1.0.0/README.md` & `tabpymigrate-1.0.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # TabPyMigrate
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your_username/TabPyMigrate/blob/main/LICENSE)
 
 > Short project description
 
 TabPyMigrate is a tool to migrate your Tableau Flow, Datasources, Workbooks from one server to another easily.
+This is similar to TabMigrate and works with Tableay Rest API to download and deploy tableau objects. Easy to configure/Run from CLI.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
```

### Comparing `tabpymigrate-1.0.0/pyproject.toml` & `tabpymigrate-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=45.0", "versioneer>=0.24", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name="tabpymigrate"
-version="1.0.0"
+version="1.0.1"
 description='Python project to download and deploy objects to Tableau Server via REST API.'
 authors = [{name="Tableau", email="kavikag00@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 
 dependencies = [
     'defusedxml>=0.7.1',
```

### Comparing `tabpymigrate-1.0.0/tabpymigrate/config.py` & `tabpymigrate-1.0.1/tabpymigrate/config.py`

 * *Files identical despite different names*

### Comparing `tabpymigrate-1.0.0/tabpymigrate/mapping.py` & `tabpymigrate-1.0.1/tabpymigrate/mapping.py`

 * *Files identical despite different names*

### Comparing `tabpymigrate-1.0.0/tabpymigrate/tabpymigrate.py` & `tabpymigrate-1.0.1/tabpymigrate/tabpymigrate.py`

 * *Files identical despite different names*

### Comparing `tabpymigrate-1.0.0/tabpymigrate/tabpymigrate_download.py` & `tabpymigrate-1.0.1/tabpymigrate/tabpymigrate_download.py`

 * *Files identical despite different names*

### Comparing `tabpymigrate-1.0.0/tabpymigrate/tabpymigrate_publish.py` & `tabpymigrate-1.0.1/tabpymigrate/tabpymigrate_publish.py`

 * *Files identical despite different names*

### Comparing `tabpymigrate-1.0.0/tabpymigrate.egg-info/PKG-INFO` & `tabpymigrate-1.0.1/tabpymigrate.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabpymigrate
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python project to download and deploy objects to Tableau Server via REST API.
 Author-email: Tableau <kavikag00@gmail.com>
 Project-URL: repository, https://github.com/codespg/tabpymigrate
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -17,14 +17,15 @@
 # TabPyMigrate
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your_username/TabPyMigrate/blob/main/LICENSE)
 
 > Short project description
 
 TabPyMigrate is a tool to migrate your Tableau Flow, Datasources, Workbooks from one server to another easily.
+This is similar to TabMigrate and works with Tableay Rest API to download and deploy tableau objects. Easy to configure/Run from CLI.
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
 - [License](#license)
```

