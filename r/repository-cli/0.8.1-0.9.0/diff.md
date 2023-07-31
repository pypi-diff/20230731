# Comparing `tmp/repository-cli-0.8.1.tar.gz` & `tmp/repository-cli-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repository-cli-0.8.1.tar", last modified: Wed Jun  7 09:23:18 2023, max compression
+gzip compressed data, was "repository-cli-0.9.0.tar", last modified: Mon Jul 31 07:40:20 2023, max compression
```

## Comparing `repository-cli-0.8.1.tar` & `repository-cli-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.360529 repository-cli-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.360529 repository-cli-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 09:23:12.000000 repository-cli-0.8.1/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 09:23:12.000000 repository-cli-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-07 09:23:12.000000 repository-cli-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-07 09:23:12.000000 repository-cli-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-07 09:23:12.000000 repository-cli-0.8.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 09:23:12.000000 repository-cli-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 09:23:12.000000 repository-cli-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-07 09:23:18.364529 repository-cli-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 09:23:12.000000 repository-cli-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-07 09:23:12.000000 repository-cli-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/repository_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/click_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/click_param_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)    19389 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/records.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-07 09:23:12.000000 repository-cli-0.8.1/repository_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/repository_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 09:23:18.000000 repository-cli-0.8.1/repository_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 09:23:12.000000 repository-cli-0.8.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-06-07 09:23:12.000000 repository-cli-0.8.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 09:23:18.364529 repository-cli-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 09:23:12.000000 repository-cli-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:23:18.364529 repository-cli-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_rdmrecords_pids.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 09:23:12.000000 repository-cli-0.8.1/tests/test_repository_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.635957 repository-cli-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-31 07:40:13.000000 repository-cli-0.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.627957 repository-cli-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.631957 repository-cli-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-31 07:40:13.000000 repository-cli-0.9.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 07:40:13.000000 repository-cli-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-31 07:40:13.000000 repository-cli-0.9.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-31 07:40:13.000000 repository-cli-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-31 07:40:13.000000 repository-cli-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-31 07:40:13.000000 repository-cli-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 07:40:13.000000 repository-cli-0.9.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-31 07:40:13.000000 repository-cli-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 07:40:13.000000 repository-cli-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-31 07:40:20.635957 repository-cli-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-31 07:40:13.000000 repository-cli-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.631957 repository-cli-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10996 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 07:40:13.000000 repository-cli-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.635957 repository-cli-0.9.0/repository_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/click_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/click_param_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19527 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-31 07:40:13.000000 repository-cli-0.9.0/repository_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.635957 repository-cli-0.9.0/repository_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 07:40:20.000000 repository-cli-0.9.0/repository_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-31 07:40:13.000000 repository-cli-0.9.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-07-31 07:40:13.000000 repository-cli-0.9.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-31 07:40:20.639957 repository-cli-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-31 07:40:13.000000 repository-cli-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:40:20.635957 repository-cli-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-07-31 07:40:13.000000 repository-cli-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-31 07:40:13.000000 repository-cli-0.9.0/tests/test_rdmrecords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-07-31 07:40:13.000000 repository-cli-0.9.0/tests/test_rdmrecords_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-31 07:40:13.000000 repository-cli-0.9.0/tests/test_rdmrecords_pids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-31 07:40:13.000000 repository-cli-0.9.0/tests/test_repository_cli.py
```

### Comparing `repository-cli-0.8.1/.github/workflows/tests.yml` & `repository-cli-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/CHANGES.rst` & `repository-cli-0.9.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-07-31)
+
+- records: add data_model parameter
+- typing: use new optional syntax
+- service: add lom service
+- global: update ruff
+
+
 Version v0.8.1 (release 2023-06-07)
 
 - refactor: move json validation into JSON
 - refactor: get_record_or_draft
 
 
 Version v0.8.0 (release 2023-06-01)
```

### Comparing `repository-cli-0.8.1/CONTRIBUTING.rst` & `repository-cli-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/LICENSE` & `repository-cli-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/MANIFEST.in` & `repository-cli-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/PKG-INFO` & `repository-cli-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,22 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-07-31)
+
+- records: add data_model parameter
+- typing: use new optional syntax
+- service: add lom service
+- global: update ruff
+
+
 Version v0.8.1 (release 2023-06-07)
 
 - refactor: move json validation into JSON
 - refactor: get_record_or_draft
 
 
 Version v0.8.0 (release 2023-06-01)
```

### Comparing `repository-cli-0.8.1/README.rst` & `repository-cli-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/docs/Makefile` & `repository-cli-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/docs/api.rst` & `repository-cli-0.9.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/docs/conf.py` & `repository-cli-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/docs/index.rst` & `repository-cli-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/docs/make.bat` & `repository-cli-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/repository_cli/cli.py` & `repository-cli-0.9.0/repository_cli/cli.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/repository_cli/click_options.py` & `repository-cli-0.9.0/repository_cli/click_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 @optional_brackets
 def option_data_model() -> Callable[[T], T]:
     """Get parameter option for data model."""
     return option(
         "--data-model",
-        type=Choice(["rdm", "marc21"]),
+        type=Choice(["rdm", "marc21", "lom"]),
         default="rdm",
     )
 
 
 @optional_brackets
 def option_record_type() -> Callable[[T], T]:
     """Get parameter option for record type."""
```

### Comparing `repository-cli-0.8.1/repository_cli/click_param_types.py` & `repository-cli-0.9.0/repository_cli/click_param_types.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 # Copyright (C) 2021-2023 Graz University of Technology.
 #
 # repository-cli is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Commonly used param types for CLI commands."""
 
+from __future__ import annotations
 
 import sys
 from json import JSONDecodeError, load, loads
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any
 
 from click import Context, Parameter, ParamType, secho
 
 from .types import Color
 
 
 def _error_msg(art: str, key: str) -> str:
@@ -27,23 +28,23 @@
 
 
 class JSON(ParamType):
     """JSON provides the ability to load a json from a string or a file."""
 
     name = "JSON"
 
-    def __init__(self, validate: list[str] = None) -> None:
+    def __init__(self, validate: list[str] | None = None) -> None:
         """Construct Json ParamType."""
         self.validate = validate
 
     def convert(
         self,
         value: Any,  # noqa: ANN401
-        param: Optional["Parameter"],  # noqa: ARG002
-        ctx: Optional["Context"],  # noqa: ARG002
+        param: Parameter | None,  # noqa: ARG002
+        ctx: Context | None,  # noqa: ARG002
     ) -> Any:  # noqa: ANN401
         """The method converts the json-file to the dictionary representation."""
         try:
             if Path(value).is_file():
                 with Path(value).open("r", encoding="utf8") as file_pointer:
                     obj = load(file_pointer)
             else:
```

### Comparing `repository-cli-0.8.1/repository_cli/ext.py` & `repository-cli-0.9.0/repository_cli/ext.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/repository_cli/records.py` & `repository-cli-0.9.0/repository_cli/records.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,22 +236,23 @@
 
     service.delete(id_=pid, identity=identity)
     secho(f"'{pid}', soft-deleted", fg=Color.success)
 
 
 @group_records.command("delete-draft")
 @option_pid
+@option_data_model
 @with_appcontext
-def delete_draft(pid: str) -> None:
+def delete_draft(pid: str, data_model: str) -> None:
     """Delete draft.
 
     example call:
         invenio repository records delete-draft -p "fcze8-4vx33"
     """
-    service = get_records_service()
+    service = get_records_service(data_model)
     identity = get_identity(permission_name="system_process", role_name="admin")
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     draft = get_draft(service=service, pid=pid, identity=identity)
@@ -266,22 +267,23 @@
 @group_records.group("pids")
 def group_pids() -> None:
     """Management commands for record pids."""
 
 
 @group_pids.command("list")
 @option_pid
+@option_data_model
 @with_appcontext
-def list_pids(pid: str) -> None:
+def list_pids(pid: str, data_model: str) -> None:
     """List record's pids.
 
     example call:
         invenio repository records pids list -p <pid>
     """
-    service = get_records_service()
+    service = get_records_service(data_model)
     identity = get_identity()
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     record_data = service.read(id_=pid, identity=identity).data.copy()
@@ -293,24 +295,25 @@
     for index, current_pid in enumerate(current_pids):
         secho(json.dumps(current_pid, indent=2), fg=Color.alternate[index % 2])
 
 
 @group_pids.command("replace")
 @option_pid
 @option_pid_identifier
+@option_data_model
 @with_appcontext
-def replace_pid(pid: str, pid_identifier: str) -> None:
+def replace_pid(pid: str, pid_identifier: str, data_model: str) -> None:
     """Update pid doi to unmanaged.
 
     example call:
         invenio repository records pids replace -p "fcze8-4vx33"
         --pid-identifier '{"doi": {
         "identifier": "10.48436/fcze8-4vx33", "provider": "unmanaged"}}'
     """
-    service = get_records_service()
+    service = get_records_service(data_model)
     identity = get_identity(permission_name="system_process", role_name="admin")
 
     if not exists_record(service, pid, identity):
         secho(f"'{pid}', does not exist or is deleted", fg=Color.error)
         return
 
     old_data = service.read(id_=pid, identity=identity).data.copy()
```

### Comparing `repository-cli-0.8.1/repository_cli/types.py` & `repository-cli-0.9.0/repository_cli/types.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/repository_cli/users.py` & `repository-cli-0.9.0/repository_cli/users.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/repository_cli/utils.py` & `repository-cli-0.9.0/repository_cli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import TYPE_CHECKING
 
 from flask_principal import Identity, RoleNeed
 from invenio_access.permissions import any_user, system_process
 from invenio_accounts import current_accounts
 from invenio_rdm_records.proxies import current_rdm_records
 from invenio_rdm_records.records.models import RDMDraftMetadata, RDMRecordMetadata
+from invenio_records_lom import current_records_lom
+from invenio_records_lom.records.models import LOMDraftMetadata, LOMRecordMetadata
 from invenio_records_marc21 import Marc21Metadata, current_records_marc21
 from invenio_records_marc21.records import DraftMetadata as Marc21DraftMetadata
 from invenio_records_marc21.records import RecordMetadata as Marc21RecordMetadata
 from sqlalchemy.orm.exc import NoResultFound
 
 if TYPE_CHECKING:
     from invenio_db import db
@@ -35,15 +37,18 @@
 
     def __init__(self, role: str) -> None:
         """Construct IdentityNotFound."""
         msg = f"Role {role} does not exist"
         super().__init__(msg)
 
 
-def get_identity(permission_name: str = "any_user", role_name: str = None) -> Identity:
+def get_identity(
+    permission_name: str = "any_user",
+    role_name: str | None = None,
+) -> Identity:
     """Get an identity to perform tasks.
 
     Default permission is "any_user"
     """
     identity = Identity(0)
     permission = any_user
     if permission_name == "system_process":
@@ -64,19 +69,16 @@
     """Get current draft of record.
 
     None will be returned if there is no draft.
     """
     # check if record exists
     service.read(id_=pid, identity=identity)
 
-    draft = None
     with suppress(Exception):
-        draft = service.read_draft(id_=pid, identity=identity)
-
-    return draft
+        return service.read_draft(id_=pid, identity=identity)
 
 
 def get_record_item(service: RecordService, pid: str, identity: Identity) -> RecordItem:
     """Get record item."""
     try:
         record_item = service.read(id_=pid, identity=identity)
     except NoResultFound:
@@ -103,32 +105,35 @@
 
 
 def get_records_service(data_model: str = "rdm") -> RecordService:
     """Get records service."""
     available_services = {
         "rdm": current_rdm_records.records_service,
         "marc21": current_records_marc21.records_service,
+        "lom": current_records_lom.records_service,
     }
 
     return available_services.get(data_model, current_rdm_records.records_service)
 
 
 def get_metadata_model(
     data_model: str = "rdm",
     record_type: str = "record",
 ) -> db.Model:
     """Get the record model."""
     available_models = {
         "record": {
             "rdm": RDMRecordMetadata,
             "marc21": Marc21RecordMetadata,
+            "lom": LOMRecordMetadata,
         },
         "draft": {
             "rdm": RDMDraftMetadata,
             "marc21": Marc21DraftMetadata,
+            "lom": LOMDraftMetadata,
         },
     }
 
     try:
         _type = available_models.get(record_type)
     except KeyError as exc:
         msg = "the used record_type should be of the list [record, draft]"
```

### Comparing `repository-cli-0.8.1/repository_cli.egg-info/PKG-INFO` & `repository-cli-0.9.0/repository_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-cli
-Version: 0.8.1
+Version: 0.9.0
 Summary: "CLI utilities for TU Graz Repository."
 Home-page: https://github.com/inveniosoftware/repository-cli
 Author: Graz University of Technology
 Author-email: info@inveniosoftware.org
 License: MIT
 Keywords: invenio repository cli
 Platform: any
@@ -52,14 +52,22 @@
 
     repository-cli is free software; you can redistribute it and/or modify
     it under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-07-31)
+
+- records: add data_model parameter
+- typing: use new optional syntax
+- service: add lom service
+- global: update ruff
+
+
 Version v0.8.1 (release 2023-06-07)
 
 - refactor: move json validation into JSON
 - refactor: get_record_or_draft
 
 
 Version v0.8.0 (release 2023-06-01)
```

### Comparing `repository-cli-0.8.1/repository_cli.egg-info/SOURCES.txt` & `repository-cli-0.9.0/repository_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/run-tests.sh` & `repository-cli-0.9.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/setup.cfg` & `repository-cli-0.9.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 packages = find:
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
 	click>=7.1.1
 	invenio-rdm-records[opensearch2]>=0.39.2,<2.0.0
 	invenio-records-marc21>=0.9
+	invenio-records-lom>=0.10
 	jq>=1.4.0
 	tabulate>=0.9.0
 
 [options.extras_require]
 tests = 
 	pytest-invenio>=1.4.0
 	pytest-black>=0.3.0
```

### Comparing `repository-cli-0.8.1/tests/conftest.py` & `repository-cli-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/tests/test_rdmrecords.py` & `repository-cli-0.9.0/tests/test_rdmrecords.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/tests/test_rdmrecords_identifiers.py` & `repository-cli-0.9.0/tests/test_rdmrecords_identifiers.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/tests/test_rdmrecords_pids.py` & `repository-cli-0.9.0/tests/test_rdmrecords_pids.py`

 * *Files identical despite different names*

### Comparing `repository-cli-0.8.1/tests/test_repository_cli.py` & `repository-cli-0.9.0/tests/test_repository_cli.py`

 * *Files identical despite different names*

