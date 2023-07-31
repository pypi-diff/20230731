# Comparing `tmp/pyairtable-2.0.0.tar.gz` & `tmp/pyairtable-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyairtable-2.0.0.tar", last modified: Mon Jul 31 19:28:47 2023, max compression
+gzip compressed data, was "pyairtable-2.0.0rc1.tar", last modified: Tue Jul 18 18:44:16 2023, max compression
```

## Comparing `pyairtable-2.0.0.tar` & `pyairtable-2.0.0rc1.tar`

### file list

```diff
@@ -1,56 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.748532 pyairtable-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-31 19:28:39.000000 pyairtable-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-31 19:28:39.000000 pyairtable-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 19:28:47.748532 pyairtable-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-31 19:28:39.000000 pyairtable-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.744532 pyairtable-2.0.0/pyairtable/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.744532 pyairtable-2.0.0/pyairtable/api/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)    19095 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/formulas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.744532 pyairtable-2.0.0/pyairtable/models/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/models/collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/models/comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.748532 pyairtable-2.0.0/pyairtable/orm/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28895 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/orm/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    15412 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/orm/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyairtable/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.744532 pyairtable-2.0.0/pyairtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-31 19:28:47.000000 pyairtable-2.0.0/pyairtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-31 19:28:47.000000 pyairtable-2.0.0/pyairtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:28:47.000000 pyairtable-2.0.0/pyairtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 19:28:47.000000 pyairtable-2.0.0/pyairtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-31 19:28:47.000000 pyairtable-2.0.0/pyairtable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 19:28:39.000000 pyairtable-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-31 19:28:47.748532 pyairtable-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-31 19:28:39.000000 pyairtable-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:28:47.748532 pyairtable-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_api_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_api_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_api_retrying.py
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_api_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_api_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_formulas.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_models_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_models_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_orm_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_orm_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_request_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_url_escape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-31 19:28:39.000000 pyairtable-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.925053 pyairtable-2.0.0rc1/pyairtable/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/pyairtable/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/pyairtable/orm/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28850 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/orm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/orm/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyairtable/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/pyairtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-18 18:44:16.000000 pyairtable-2.0.0rc1/pyairtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-18 18:44:16.000000 pyairtable-2.0.0rc1/pyairtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:44:16.000000 pyairtable-2.0.0rc1/pyairtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 18:44:16.000000 pyairtable-2.0.0rc1/pyairtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 18:44:16.000000 pyairtable-2.0.0rc1/pyairtable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 18:44:16.933053 pyairtable-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:44:16.929053 pyairtable-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_api_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_api_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_api_retrying.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_api_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_api_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_formulas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11545 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_orm_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_orm_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_request_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_url_escape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-18 18:44:08.000000 pyairtable-2.0.0rc1/tox.ini
```

### Comparing `pyairtable-2.0.0/LICENSE` & `pyairtable-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/PKG-INFO` & `pyairtable-2.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairtable
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Python Client for the Airtable API
 Home-page: https://github.com/gtalarico/pyairtable
 Author: Gui Talarico
 License: MIT
 Keywords: airtable,api,client,pyairtable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
 
 ### Getting started
 
 If it's your first time working on this library, clone the repo, set up pre-commit hooks, and make sure you can run tests (and they pass). If that doesn't work out of the box, please check your local development environment before filing an issue.
 
 ```sh
 % make setup
-% make test
+% tox
 ```
 
 ### Reporting a bug
 
 We encourage anyone to [submit an issue](https://github.com/gtalarico/pyairtable/issues/new) to let us know about bugs, as long as you've followed these steps:
 
 1. Confirm you're on the latest version of the library and you can run the test suite locally.
@@ -68,10 +68,12 @@
 
 Anyone who uses this library is welcome to [submit a pull request](https://github.com/gtalarico/pyairtable/pulls) for a bug fix or a new feature. We do ask that all pull requests adhere to the following guidelines:
 
 1. Public functions/methods have docstrings and type annotations.
 2. New functionality is accompanied by clear, descriptive unit tests.
 3. You can run `make test && make docs` successfully.
 
+If you have an enterprise API key that can run end-to-end tests, please also run `env AIRTABLE_API_KEY=... make test-e2e`.
+
 If you want to discuss an idea you're working on but haven't yet finished all of the above, please [open a draft pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#draft-pull-requests). That will be a clear signal that you're not asking to merge your code (yet) and are just looking for discussion or feedback.
 
 Thanks in advance for sharing your ideas!
```

### Comparing `pyairtable-2.0.0/README.md` & `pyairtable-2.0.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 ### Getting started
 
 If it's your first time working on this library, clone the repo, set up pre-commit hooks, and make sure you can run tests (and they pass). If that doesn't work out of the box, please check your local development environment before filing an issue.
 
 ```sh
 % make setup
-% make test
+% tox
 ```
 
 ### Reporting a bug
 
 We encourage anyone to [submit an issue](https://github.com/gtalarico/pyairtable/issues/new) to let us know about bugs, as long as you've followed these steps:
 
 1. Confirm you're on the latest version of the library and you can run the test suite locally.
@@ -48,10 +48,12 @@
 
 Anyone who uses this library is welcome to [submit a pull request](https://github.com/gtalarico/pyairtable/pulls) for a bug fix or a new feature. We do ask that all pull requests adhere to the following guidelines:
 
 1. Public functions/methods have docstrings and type annotations.
 2. New functionality is accompanied by clear, descriptive unit tests.
 3. You can run `make test && make docs` successfully.
 
+If you have an enterprise API key that can run end-to-end tests, please also run `env AIRTABLE_API_KEY=... make test-e2e`.
+
 If you want to discuss an idea you're working on but haven't yet finished all of the above, please [open a draft pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#draft-pull-requests). That will be a clear signal that you're not asking to merge your code (yet) and are just looking for discussion or feedback.
 
 Thanks in advance for sharing your ideas!
```

### Comparing `pyairtable-2.0.0/pyairtable/api/api.py` & `pyairtable-2.0.0rc1/pyairtable/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -179,48 +179,14 @@
                 if "error" in error_dict:
                     err_msg += " [Error: {}]".format(error_dict["error"])
             exc.args = (*exc.args, err_msg)
             raise exc
         else:
             return response.json()
 
-    def iterate_requests(
-        self,
-        method: str,
-        url: str,
-        fallback: Optional[Tuple[str, str]] = None,
-        options: Optional[Dict[str, Any]] = None,
-    ) -> Iterator[Any]:
-        """
-        Makes one or more requests and iterates through each result.
-
-        If the response payload contains an 'offset' value, this method will perform
-        another request with that offset value as a parameter (query params for GET,
-        body payload for POST/PATCH/etc).
-
-        If the response payload is not a 'dict', it will be yielded as normal
-        and the method will return.
-
-        Args:
-            method: HTTP method to use.
-            url: The URL we're attempting to call.
-            fallback: The method and URL to use if we have to convert a GET to a POST.
-            options: Airtable-specific query params to use while fetching records.
-                See :ref:`Parameters` for valid options.
-        """
-        options = options or {}
-        while True:
-            response = self.request(method, url, fallback=fallback, options=options)
-            yield response
-            if not isinstance(response, dict):
-                return
-            if not (offset := response.get("offset")):
-                return
-            options = {**options, "offset": offset}
-
     def chunked(self, iterable: Sequence[T]) -> Iterator[Sequence[T]]:
         """
         Iterates through chunks of the given sequence that are equal in size
         to the maximum number of records per request allowed by the API.
         """
         return chunked(iterable, self.MAX_RECORDS_PER_REQUEST)
```

### Comparing `pyairtable-2.0.0/pyairtable/api/base.py` & `pyairtable-2.0.0rc1/pyairtable/api/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 
 
 class Base:
     """
     Represents an Airtable base.
     """
 
-    #: The connection to the Airtable API.
     api: "pyairtable.api.api.Api"
-
-    #: The base ID, in the format ``appXXXXXXXXXXXXXX``
     id: str
 
     def __init__(self, api: Union["pyairtable.api.api.Api", str], base_id: str):
         """
         Old style constructor takes ``str`` arguments, and will create its own
         instance of :class:`Api`.
```

### Comparing `pyairtable-2.0.0/pyairtable/api/params.py` & `pyairtable-2.0.0rc1/pyairtable/api/params.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/pyairtable/api/retrying.py` & `pyairtable-2.0.0rc1/pyairtable/api/retrying.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/pyairtable/api/table.py` & `pyairtable-2.0.0rc1/pyairtable/api/table.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import posixpath
 import urllib.parse
 import warnings
 from typing import Any, Iterator, List, Optional, Union, overload
 
-import pyairtable.models
+import pyairtable.api.api
+import pyairtable.api.base
 from pyairtable.api.retrying import Retry
 from pyairtable.api.types import (
     FieldName,
     Fields,
     RecordDeletedDict,
     RecordDict,
     RecordId,
     UpdateRecordDict,
-    UpsertResultDict,
     assert_typed_dict,
     assert_typed_dicts,
 )
 
 
 class Table:
     """
@@ -24,18 +23,16 @@
 
     Usage:
         >>> api = Api(access_token)
         >>> table = api.table("base_id", "table_name")
         >>> records = table.all()
     """
 
-    #: The base that this table belongs to.
+    api: "pyairtable.api.api.Api"
     base: "pyairtable.api.base.Base"
-
-    #: Can be either the table name or the table ID (``tblXXXXXXXXXXXXXX``).
     name: str
 
     @overload
     def __init__(
         self,
         api_key: str,
         base_id: str,
@@ -96,39 +93,33 @@
             base = base_id
         else:
             raise TypeError(
                 "Table() expects either (str, str, str) or (None, Base, str);"
                 f" got ({type(api_key)}, {type(base_id)}, {type(table_name)})"
             )
 
+        self.api = base.api
         self.base = base
         self.name = table_name
 
     def __repr__(self) -> str:
         return f"<Table base_id={self.base.id!r} table_name={self.name!r}>"
 
     @property
     def url(self) -> str:
         """
-        Returns the URL for this table.
+        Return the URL for this table.
         """
         return self.api.build_url(self.base.id, urllib.parse.quote(self.name, safe=""))
 
-    def record_url(self, record_id: RecordId, *components: str) -> str:
-        """
-        Returns the URL for the given record ID, with optional trailing components.
-        """
-        return posixpath.join(self.url, record_id, *components)
-
-    @property
-    def api(self) -> "pyairtable.api.api.Api":
+    def record_url(self, record_id: RecordId) -> str:
         """
-        Returns the same API connection as table's :class:`~pyairtable.Base`.
+        Return the URL for the given record ID.
         """
-        return self.base.api
+        return f"{self.url}/{record_id}"
 
     def get(self, record_id: RecordId, **options: Any) -> RecordDict:
         """
         Retrieves a record by its ID.
 
         >>> table.get('recwPQIfs4wKPyc9D')
         {'id': 'recwPQIfs4wKPyc9D', 'fields': {'First Name': 'John', 'Age': 21}}
@@ -169,21 +160,29 @@
             sort: |kwarg_sort|
             formula: |kwarg_formula|
             cell_format: |kwarg_cell_format|
             user_locale: |kwarg_user_locale|
             time_zone: |kwarg_time_zone|
             return_fields_by_field_id: |kwarg_return_fields_by_field_id|
         """
-        for page in self.api.iterate_requests(
-            method="get",
-            url=self.url,
-            fallback=("post", f"{self.url}/listRecords"),
-            options=options,
-        ):
-            yield assert_typed_dicts(RecordDict, page.get("records", []))
+        offset = None
+        while True:
+            if offset:
+                options.update({"offset": offset})
+            data = self.api.request(
+                method="get",
+                url=self.url,
+                fallback=("post", f"{self.url}/listRecords"),
+                options=options,
+            )
+            records = assert_typed_dicts(RecordDict, data.get("records", []))
+            yield records
+            offset = data.get("offset")
+            if not offset:
+                break
 
     def all(self, **options: Any) -> List[RecordDict]:
         """
         Retrieves all matching records in a single list.
 
         >>> api.all('base_id', 'table_name', view='MyView', fields=['ColA', '-ColB'])
         [{'fields': ...}, ...]
@@ -370,15 +369,15 @@
     def batch_upsert(
         self,
         records: List[UpdateRecordDict],
         key_fields: List[FieldName],
         replace: bool = False,
         typecast: bool = False,
         return_fields_by_field_id: bool = False,
-    ) -> UpsertResultDict:
+    ) -> List[RecordDict]:
         """
         Updates or creates records in batches, either using ``id`` (if given) or using a set of
         fields (``key_fields``) to look for matches. For more information on how this operation
         behaves, see Airtable's API documentation for `Update multiple records <https://airtable.com/developers/web/api/update-multiple-records#request-performupsert-fieldstomergeon>`__.
 
         .. versionadded:: 1.5.0
 
@@ -387,34 +386,29 @@
             key_fields: List of field names that Airtable should use to match
                 records in the input with existing records on the server.
             replace: |kwarg_replace|
             typecast: |kwarg_typecast|
             return_fields_by_field_id: |kwarg_return_fields_by_field_id|
 
         Returns:
-            Lists of created/updated record IDs, along with the list of all records affected.
+            The list of updated records.
         """
         # The API will reject a request where a record is missing any of fieldsToMergeOn,
         # but we might not reach that error until we've done several batch operations.
         # To spare implementers from having to recover from a partially applied upsert,
         # and to simplify our API, we will raise an exception before any network calls.
         for record in records:
             if "id" in record:
                 continue
             missing = set(key_fields) - set(record.get("fields", []))
             if missing:
                 raise ValueError(f"missing {missing!r} in {record['fields'].keys()!r}")
 
+        updated_records = []
         method = "put" if replace else "patch"
-        result: UpsertResultDict = {
-            "updatedRecords": [],
-            "createdRecords": [],
-            "records": [],
-        }
-
         for chunk in self.api.chunked(records):
             formatted_records = [
                 {k: v for (k, v) in record.items() if k in ("id", "fields")}
                 for record in chunk
             ]
             response = self.api.request(
                 method=method,
@@ -422,21 +416,17 @@
                 json={
                     "records": formatted_records,
                     "typecast": typecast,
                     "returnFieldsByFieldId": return_fields_by_field_id,
                     "performUpsert": {"fieldsToMergeOn": key_fields},
                 },
             )
-            result["updatedRecords"].extend(response["updatedRecords"])
-            result["createdRecords"].extend(response["createdRecords"])
-            result["records"].extend(
-                assert_typed_dicts(RecordDict, response["records"])
-            )
+            updated_records += assert_typed_dicts(RecordDict, response["records"])
 
-        return result
+        return updated_records
 
     def delete(self, record_id: RecordId) -> RecordDeletedDict:
         """
         Deletes the given record.
 
         >>> table.delete('recwPQIfs4wKPyc9D')
         {'id': 'recwPQIfs4wKPyc9D', 'deleted': True}
@@ -471,83 +461,7 @@
         deleted_records = []
 
         for chunk in self.api.chunked(record_ids):
             result = self.api.request("delete", self.url, params={"records[]": chunk})
             deleted_records += assert_typed_dicts(RecordDeletedDict, result["records"])
 
         return deleted_records
-
-    def comments(self, record_id: RecordId) -> List["pyairtable.models.Comment"]:
-        """
-        Returns a list of comments on the given record.
-
-        Usage:
-            >>> table = Api.table("appNxslc6jG0XedVM", "tblslc6jG0XedVMNx")
-            >>> table.comments("recMNxslc6jG0XedV")
-            [
-                Comment(
-                    id='comdVMNxslc6jG0Xe',
-                    text='Hello, @[usrVMNxslc6jG0Xed]!',
-                    created_time='2023-06-07T17:46:24.435891',
-                    last_updated_time=None,
-                    mentioned={
-                        'usrVMNxslc6jG0Xed': Mentioned(
-                            display_name='Alice',
-                            email='alice@example.com',
-                            id='usrVMNxslc6jG0Xed',
-                            type='user'
-                        )
-                    },
-                    author=Collaborator(
-                        id='usr0000pyairtable',
-                        email='pyairtable@example.com',
-                        name='Your pyairtable access token'
-                    )
-                )
-            ]
-
-        Args:
-            record_id: |arg_record_id|
-        """
-        url = self.record_url(record_id, "comments")
-        return [
-            pyairtable.models.Comment.from_api(
-                api=self.api,
-                url=self.record_url(record_id, "comments", comment["id"]),
-                obj=comment,
-            )
-            for page in self.api.iterate_requests("GET", url)
-            for comment in page["comments"]
-        ]
-
-    def add_comment(
-        self,
-        record_id: RecordId,
-        text: str,
-    ) -> "pyairtable.models.Comment":
-        """
-        Creates a comment on a record.
-        See `Create comment <https://airtable.com/developers/web/api/create-comment>`_ for details.
-
-        Usage:
-            >>> table = Api.table("appNxslc6jG0XedVM", "tblslc6jG0XedVMNx")
-            >>> comment = table.add_comment("recMNxslc6jG0XedV", "Hello, @[usrVMNxslc6jG0Xed]!")
-            >>> comment.text = "Never mind!"
-            >>> comment.save()
-            >>> comment.delete()
-
-        Args:
-            record_id: |arg_record_id|
-            text: The text of the comment. Use ``@[usrIdentifier]`` to mention users.
-        """
-        url = self.record_url(record_id, "comments")
-        response = self.api.request("POST", url, json={"text": text})
-        return pyairtable.models.Comment.from_api(
-            api=self.api,
-            url=self.record_url(record_id, "comments", response["id"]),
-            obj=response,
-        )
-
-
-# These are at the bottom of the module to avoid circular imports
-import pyairtable.api.api  # noqa
-import pyairtable.api.base  # noqa
```

### Comparing `pyairtable-2.0.0/pyairtable/api/types.py` & `pyairtable-2.0.0rc1/pyairtable/api/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -243,35 +243,14 @@
         {'id': 'recAdw9EjV90xbZ', 'deleted': True}
     """
 
     id: RecordId
     deleted: bool
 
 
-class UpsertResultDict(TypedDict):
-    """
-    A ``dict`` representing the payload returned by the Airtable API after an upsert.
-    For more details on this data structure, see the
-    `Update multiple records <https://airtable.com/developers/web/api/update-multiple-records>`__
-    API documentation.
-
-    Usage:
-        >>> table.batch_upsert(records, key_fields=["Name"])
-        {
-            'createdRecords': [...],
-            'updatedRecords': [...],
-            'records': [...]
-        }
-    """
-
-    createdRecords: List[RecordId]
-    updatedRecords: List[RecordId]
-    records: List[RecordDict]
-
-
 class UserAndScopesDict(TypedDict, total=False):
     """
     A ``dict`` representing the `Get user ID & scopes <https://airtable.com/developers/web/api/get-user-id-scopes>`_ endpoint.
 
     Usage:
         >>> api.whoami()
         {'id': 'usrX9e810wHn3mMLz'}
```

### Comparing `pyairtable-2.0.0/pyairtable/formulas.py` & `pyairtable-2.0.0rc1/pyairtable/formulas.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/pyairtable/metadata.py` & `pyairtable-2.0.0rc1/pyairtable/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,16 @@
                     "permissionLevel": "edit"
                 }
             ]
         }
     """
     api = api.api if isinstance(api, Base) else api
     base_list_url = api.build_url("meta", "bases")
-    return {
-        "bases": [
-            base
-            for page in api.iterate_requests("get", base_list_url)
-            for base in page.get("bases", [])
-        ]
-    }
+    assert isinstance(response := api.request("get", base_list_url), dict)
+    return response
 
 
 def get_base_schema(base: Union[Base, Table]) -> Dict[Any, Any]:
     """
     Returns Schema of a Base
     For More Details `Metadata Api Documentation <https://airtable.com/api/meta>`_
```

### Comparing `pyairtable-2.0.0/pyairtable/orm/fields.py` & `pyairtable-2.0.0rc1/pyairtable/orm/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,16 +548,15 @@
         # retrieve their values in bulk, and store them keyed by ID
         # so we can maintain the order we received from the API.
         new_records = {}
         if new_record_ids := [v for v in records if isinstance(v, RecordId)]:
             new_records = {
                 record.id: record
                 for record in self.linked_model.from_ids(
-                    cast(List[RecordId], new_record_ids),
-                    fetch=(not self._lazy),
+                    cast(List[RecordId], new_record_ids)
                 )
             }
         # If the list contains record IDs, replace the contents with instances.
         # Other code may already have references to this specific list, so
         # we replace the existing list's values.
         records[:] = [
             new_records[cast(RecordId, value)] if isinstance(value, RecordId) else value
```

### Comparing `pyairtable-2.0.0/pyairtable/orm/model.py` & `pyairtable-2.0.0rc1/pyairtable/orm/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,66 +10,37 @@
     FieldName,
     RecordDict,
     RecordId,
     UpdateRecordDict,
     WritableFields,
 )
 from pyairtable.formulas import OR, STR_VALUE
-from pyairtable.models import Comment
 from pyairtable.orm.fields import AnyField, Field
 
 
 class Model:
     """
-    Supports creating ORM-style classes representing Airtable tables.
-    For more details, see :ref:`orm`.
+    This class allows you create an orm-style class for your Airtable tables.
 
-    A nested class called ``Meta`` is required and can specify
-    the following attributes:
+    This is a meta class and can only be used to define sub-classes.
 
-        * ``api_key`` (required) - API key or personal access token.
-        * ``base_id`` (required) - Base ID (not name).
-        * ``table_name`` (required) - Table ID or name.
-        * ``timeout`` - A tuple indicating a connect and read timeout. Defaults to no timeout.
-        * ``typecast`` - |kwarg_typecast| Defaults to ``True``.
+    The ``Meta`` is reuired and must specify all three attributes: ``base_id``,
+    ``table_id``, and ``api_key``.
 
-    .. code-block:: python
-
-        from pyairtable.orm import Model, fields
-
-        class Contact(Model):
-            first_name = fields.TextField("First Name")
-            age = fields.IntegerField("Age")
-
-            class Meta:
-                base_id = "appaPqizdsNHDvlEm"
-                table_name = "Contact"
-                api_key = "keyapikey"
-                timeout = (5, 5)
-                typecast = True
-
-    You can implement meta attributes as callables if certain values
-    need to be dynamically provided or are unavailable at import time:
-
-    .. code-block:: python
-
-        from pyairtable.orm import Model, fields
-        from your_app.config import get_secret
-
-        class Contact(Model):
-            first_name = fields.TextField("First Name")
-            age = fields.IntegerField("Age")
-
-            class Meta:
-                base_id = "appaPqizdsNHDvlEm"
-                table_name = "Contact"
-
-                @staticmethod
-                def api_key():
-                    return get_secret("AIRTABLE_API_KEY")
+    >>> from pyairtable.orm import Model, fields
+    >>> class Contact(Model):
+    ...     first_name = fields.TextField("First Name")
+    ...     age = fields.IntegerField("Age")
+    ...
+    ...     class Meta:
+    ...         base_id = "appaPqizdsNHDvlEm"
+    ...         table_name = "Contact"
+    ...         api_key = "keyapikey"
+    ...         timeout: Optional[Tuple[int, int]] = (5, 5)
+    ...         typecast: bool = True
     """
 
     id: str = ""
     created_time: str = ""
     _deleted: bool = False
     _fields: Dict[FieldName, Any]
 
@@ -130,26 +101,14 @@
         ...     "First Name": "first_name"
         ...     "Age": "age"
         ... }
         """
         return {v.field_name: k for k, v in cls._attribute_descriptor_map().items()}
 
     def __init__(self, **fields: Any):
-        """
-        Constructs a model instance with field values based on the given keyword args.
-
-        >>> Contact(name="Alice", birthday=date(1980, 1, 1))
-        <unsaved Contact>
-
-        The keyword argument ``id=`` special-cased and sets the record ID, not a field value.
-
-        >>> Contact(id="recWPqD9izdsNvlE", name="Bob")
-        <Contact id='recWPqD9izdsNvlE'>
-        """
-
         if "id" in fields:
             self.id = fields.pop("id")
 
         # Field values in internal (not API) representation
         self._fields = {}
 
         # Call __set__ on each field to set field values
@@ -161,16 +120,14 @@
     @classmethod
     def _get_meta(cls, name: str, default: Any = None, required: bool = False) -> Any:
         if not hasattr(cls, "Meta"):
             raise AttributeError(f"{cls.__name__}.Meta must be defined")
         if required and not hasattr(cls.Meta, name):
             raise ValueError(f"{cls.__name__}.Meta.{name} must be defined")
         value = getattr(cls.Meta, name, default)
-        if callable(value):
-            value = value()
         if required and value is None:
             raise ValueError(f"{cls.__name__}.Meta.{name} cannot be None")
         return value
 
     @classmethod
     def _validate_class(cls) -> None:
         # Verify required Meta attributes were set
@@ -204,27 +161,23 @@
         return cls.get_base().table(cls._get_meta("table_name"))
 
     @classmethod
     def _typecast(cls) -> bool:
         return bool(cls._get_meta("typecast", default=True))
 
     def exists(self) -> bool:
-        """
-        Whether the instance has been saved to Airtable already.
-        """
+        """Returns boolean indicating if instance exists (has 'id' attribute)"""
         return bool(self.id)
 
     def save(self) -> bool:
         """
         Saves or updates a model.
+        If instance has no 'id', it will be created, otherwise updated.
 
-        If the instance does not exist already, it will be created;
-        otherwise, the existing record will be updated.
-
-        Returns ``True`` if a record was created and ``False`` if it was updated.
+        Returns ``True`` if was created and `False` if it was updated
         """
         if self._deleted:
             raise RuntimeError(f"{self.id} was deleted")
         table = self.get_table()
         fields = self.to_record(only_writable=True)["fields"]
 
         if not self.id:
@@ -235,17 +188,15 @@
             did_create = False
 
         self.id = record["id"]
         self.created_time = record["createdTime"]
         return did_create
 
     def delete(self) -> bool:
-        """
-        Deletes the record. Raises ``ValueError`` if the record does not exist.
-        """
+        """Deletes record. Must have 'id' field"""
         if not self.id:
             raise ValueError("cannot be deleted because it does not have id")
         table = self.get_table()
         result = table.delete(self.id)
         self._deleted = True
         # Is it even possible to get "deleted" False?
         return bool(result["deleted"])
@@ -409,21 +360,7 @@
         given a model which has never been saved to Airtable.
         """
         if not all(model.id for model in models):
             raise ValueError("cannot delete an unsaved model")
         if not all(isinstance(model, cls) for model in models):
             raise TypeError(set(type(model) for model in models))
         cls.get_table().batch_delete([model.id for model in models])
-
-    def comments(self) -> List[Comment]:
-        """
-        Return a list of comments on this record.
-        See :meth:`Table.comments <pyairtable.Table.comments>`.
-        """
-        return self.get_table().comments(self.id)
-
-    def add_comment(self, text: str) -> Comment:
-        """
-        Add a comment to this record.
-        See :meth:`Table.add_comment <pyairtable.Table.add_comment>`.
-        """
-        return self.get_table().add_comment(self.id, text)
```

### Comparing `pyairtable-2.0.0/pyairtable/testing.py` & `pyairtable-2.0.0rc1/pyairtable/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         "createdTime": datetime.datetime.now().isoformat() + "Z",
         "fields": {**(fields or {}), **other_fields},
     }
 
 
 def fake_user(value: Any = None) -> CollaboratorDict:
     id = fake_id("usr", value)
-    return {"id": id, "email": f"{value or id}@example.com", "name": "Fake User"}
+    return {"id": id, "email": f"{value or id}@example.com"}
 
 
 def fake_attachment() -> AttachmentDict:
     return {
         "id": fake_id("att"),
         "url": "https://example.com/",
         "filename": "foo.txt",
```

### Comparing `pyairtable-2.0.0/pyairtable/utils.py` & `pyairtable-2.0.0rc1/pyairtable/utils.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/pyairtable.egg-info/PKG-INFO` & `pyairtable-2.0.0rc1/pyairtable.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyairtable
-Version: 2.0.0
+Version: 2.0.0rc1
 Summary: Python Client for the Airtable API
 Home-page: https://github.com/gtalarico/pyairtable
 Author: Gui Talarico
 License: MIT
 Keywords: airtable,api,client,pyairtable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
 
 ### Getting started
 
 If it's your first time working on this library, clone the repo, set up pre-commit hooks, and make sure you can run tests (and they pass). If that doesn't work out of the box, please check your local development environment before filing an issue.
 
 ```sh
 % make setup
-% make test
+% tox
 ```
 
 ### Reporting a bug
 
 We encourage anyone to [submit an issue](https://github.com/gtalarico/pyairtable/issues/new) to let us know about bugs, as long as you've followed these steps:
 
 1. Confirm you're on the latest version of the library and you can run the test suite locally.
@@ -68,10 +68,12 @@
 
 Anyone who uses this library is welcome to [submit a pull request](https://github.com/gtalarico/pyairtable/pulls) for a bug fix or a new feature. We do ask that all pull requests adhere to the following guidelines:
 
 1. Public functions/methods have docstrings and type annotations.
 2. New functionality is accompanied by clear, descriptive unit tests.
 3. You can run `make test && make docs` successfully.
 
+If you have an enterprise API key that can run end-to-end tests, please also run `env AIRTABLE_API_KEY=... make test-e2e`.
+
 If you want to discuss an idea you're working on but haven't yet finished all of the above, please [open a draft pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#draft-pull-requests). That will be a clear signal that you're not asking to merge your code (yet) and are just looking for discussion or feedback.
 
 Thanks in advance for sharing your ideas!
```

### Comparing `pyairtable-2.0.0/pyairtable.egg-info/SOURCES.txt` & `pyairtable-2.0.0rc1/pyairtable.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -19,29 +19,23 @@
 pyairtable/api/__init__.py
 pyairtable/api/api.py
 pyairtable/api/base.py
 pyairtable/api/params.py
 pyairtable/api/retrying.py
 pyairtable/api/table.py
 pyairtable/api/types.py
-pyairtable/models/__init__.py
-pyairtable/models/_base.py
-pyairtable/models/collaborator.py
-pyairtable/models/comment.py
 pyairtable/orm/__init__.py
 pyairtable/orm/fields.py
 pyairtable/orm/model.py
 tests/test_api_api.py
 tests/test_api_base.py
 tests/test_api_retrying.py
 tests/test_api_table.py
 tests/test_api_types.py
 tests/test_formulas.py
-tests/test_models_collaborator.py
-tests/test_models_comment.py
 tests/test_orm.py
 tests/test_orm_fields.py
 tests/test_orm_model.py
 tests/test_params.py
 tests/test_request_errors.py
 tests/test_typing.py
 tests/test_url_escape.py
```

### Comparing `pyairtable-2.0.0/setup.cfg` & `pyairtable-2.0.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Software Development
 
 [options]
 packages = find:
 install_requires = 
-	inflection
 	pydantic ~= 1.10
 	requests >= 2.22.0
 	typing_extensions
 	urllib3 >= 1.26
 
 [aliases]
 test = pytest
```

### Comparing `pyairtable-2.0.0/tests/test_api_api.py` & `pyairtable-2.0.0rc1/tests/test_api_api.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_api_base.py` & `pyairtable-2.0.0rc1/tests/test_api_base.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_api_retrying.py` & `pyairtable-2.0.0rc1/tests/test_api_retrying.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_api_table.py` & `pyairtable-2.0.0rc1/tests/test_api_table.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from posixpath import join as urljoin
 
 import pytest
 from requests import Request
 from requests_mock import Mocker
 
 from pyairtable import Api, Base, Table
-from pyairtable.testing import fake_record
 from pyairtable.utils import chunked
 
 
 def test_constructor(base: Base):
     """
     Test the constructor.
     """
@@ -241,59 +240,48 @@
             additional_matcher=match_request_data(post_data),
         )
         resp = table.update(id_, post_data, replace=replace)
     assert dict_equals(resp, mock_response_single)
 
 
 @pytest.mark.parametrize("replace,http_method", [(False, "PATCH"), (True, "PUT")])
-def test_batch_update(table: Table, replace, http_method):
-    records = [fake_record(fieldvalue=index) for index in range(50)]
+def test_batch_update(table: Table, mock_response_batch, replace, http_method):
+    records = [
+        {"id": x["id"], "fields": x["fields"]} for x in mock_response_batch["records"]
+    ]
     with Mocker() as mock:
-        mock.register_uri(
-            http_method,
-            table.url,
-            response_list=[
-                {"json": {"records": chunk}} for chunk in table.api.chunked(records)
-            ],
-        )
+        for chunk in _chunk(mock_response_batch["records"], 10):
+            mock.register_uri(
+                http_method,
+                table.url,
+                status_code=201,
+                json={"records": chunk},
+            )
         resp = table.batch_update(records, replace=replace)
 
-    assert resp == records
+    assert resp == mock_response_batch["records"]
 
 
 @pytest.mark.parametrize("replace,http_method", [(False, "PATCH"), (True, "PUT")])
-def test_batch_upsert(table: Table, replace, http_method, monkeypatch):
-    field_name = "Name"
-    exists1 = fake_record({field_name: "Exists 1"})
-    exists2 = fake_record({field_name: "Exists 2"})
-    created = fake_record({field_name: "Does not exist"})
-    payload = [
-        {"id": exists1["id"], "fields": {field_name: "Exists 1"}},
-        {"fields": {field_name: "Exists 2"}},
-        {"fields": {field_name: "Does not exist"}},
-    ]
-    responses = [
-        {"createdRecords": [], "updatedRecords": [exists1["id"]], "records": [exists1]},
-        {"createdRecords": [], "updatedRecords": [exists2["id"]], "records": [exists2]},
-        {"createdRecords": [created["id"]], "updatedRecords": [], "records": [created]},
+def test_batch_upsert(table: Table, mock_response_batch, replace, http_method):
+    records = [
+        {"id": x["id"], "fields": x["fields"]} for x in mock_response_batch["records"]
     ]
+    fields = ["Name"]
     with Mocker() as mock:
-        mock.register_uri(
-            http_method,
-            table.url,
-            response_list=[{"json": response} for response in responses],
-        )
-        monkeypatch.setattr(table.api, "MAX_RECORDS_PER_REQUEST", 1)
-        resp = table.batch_upsert(payload, key_fields=[field_name], replace=replace)
+        for chunk in _chunk(mock_response_batch["records"], 10):
+            mock.register_uri(
+                http_method,
+                table.url,
+                status_code=201,
+                json={"records": chunk},
+            )
+        resp = table.batch_upsert(records, key_fields=fields, replace=replace)
 
-    assert resp == {
-        "createdRecords": [created["id"]],
-        "updatedRecords": [exists1["id"], exists2["id"]],
-        "records": [exists1, exists2, created],
-    }
+    assert resp == mock_response_batch["records"]
 
 
 def test_batch_upsert__missing_field(table: Table, requests_mock):
     """
     Test that batch_upsert raises an exception if a record in the input
     is missing one of the key_fields, since this will create an error
     on the API.
```

### Comparing `pyairtable-2.0.0/tests/test_api_types.py` & `pyairtable-2.0.0rc1/tests/test_api_types.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_formulas.py` & `pyairtable-2.0.0rc1/tests/test_formulas.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_orm.py` & `pyairtable-2.0.0rc1/tests/test_orm.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_orm_fields.py` & `pyairtable-2.0.0rc1/tests/test_orm_fields.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_params.py` & `pyairtable-2.0.0rc1/tests/test_params.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_request_errors.py` & `pyairtable-2.0.0rc1/tests/test_request_errors.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_typing.py` & `pyairtable-2.0.0rc1/tests/test_typing.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert_type(table.all(), List[T.RecordDict])
     assert_type(table.first(), Optional[T.RecordDict])
     assert_type(table.create({}), T.RecordDict)
     assert_type(table.update(record_id, {}), T.RecordDict)
     assert_type(table.delete(record_id), T.RecordDeletedDict)
     assert_type(table.batch_create([]), List[T.RecordDict])
     assert_type(table.batch_update([]), List[T.RecordDict])
-    assert_type(table.batch_upsert([], []), T.UpsertResultDict)
+    assert_type(table.batch_upsert([], []), List[T.RecordDict])
     assert_type(table.batch_delete([]), List[T.RecordDeletedDict])
 
     # Ensure we can set all kinds of field values
     table.update(record_id, {"Field Name": "name"})
     table.update(record_id, {"Field Name": 1})
     table.update(record_id, {"Field Name": 1.0})
     table.update(record_id, {"Field Name": True})
```

### Comparing `pyairtable-2.0.0/tests/test_url_escape.py` & `pyairtable-2.0.0rc1/tests/test_url_escape.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tests/test_utils.py` & `pyairtable-2.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyairtable-2.0.0/tox.ini` & `pyairtable-2.0.0rc1/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 deps = -r requirements-dev.txt
 commands = mypy --strict pyairtable tests/test_typing.py
 
 [testenv]
 passenv = AIRTABLE_API_KEY
 addopts = -v
 testpaths = tests
-commands = python -m pytest {posargs}
+commands = python -m pytest {posargs:-m 'not integration'}
 deps =
     -r requirements-test.txt
     requestsmin: requests==2.22.0  # Keep in sync with setup.cfg
     requestsmax: requests>=2.22.0  # Keep in sync with setup.cfg
 
 [testenv:coverage]
 passenv = COVERAGE_FORMAT
```

