# Comparing `tmp/adafruit-circuitpython-neokey-1.0.9.tar.gz` & `tmp/adafruit-circuitpython-neokey-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neokey-1.0.9.tar", last modified: Tue Aug  9 19:58:52 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-neokey-1.1.0.tar", last modified: Mon Jul 31 19:36:24 2023, max compression
```

## Comparing `adafruit-circuitpython-neokey-1.0.9.tar` & `adafruit-circuitpython-neokey-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.139067 adafruit-circuitpython-neokey-1.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.139067 adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3537 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:58:52.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1864 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/neokey1x4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5667 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/examples/neokey1x4_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/examples/neokey_1x4_multikey.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-08-09 19:58:44.000000 adafruit-circuitpython-neokey-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-09 19:58:36.000000 adafruit-circuitpython-neokey-1.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:58:52.143067 adafruit-circuitpython-neokey-1.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.978174 adafruit-circuitpython-neokey-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.982174 adafruit-circuitpython-neokey-1.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.982174 adafruit-circuitpython-neokey-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.982174 adafruit-circuitpython-neokey-1.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.982174 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-31 19:36:24.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 19:36:24.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:36:24.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 19:36:24.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 19:36:24.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.982174 adafruit-circuitpython-neokey-1.1.0/adafruit_neokey/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_neokey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/adafruit_neokey/neokey1x4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/examples/neokey1x4_allkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/examples/neokey1x4_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/examples/neokey_1x4_multikey.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-31 19:36:17.000000 adafruit-circuitpython-neokey-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-31 19:36:08.000000 adafruit-circuitpython-neokey-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:36:24.986174 adafruit-circuitpython-neokey-1.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neokey-1.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/.gitignore` & `adafruit-circuitpython-neokey-1.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/.pre-commit-config.yaml` & `adafruit-circuitpython-neokey-1.1.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/.pylintrc` & `adafruit-circuitpython-neokey-1.1.0/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neokey-1.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/LICENSE` & `adafruit-circuitpython-neokey-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neokey-1.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/LICENSES/MIT.txt` & `adafruit-circuitpython-neokey-1.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neokey-1.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/PKG-INFO` & `adafruit-circuitpython-neokey-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neokey
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython library for using Adafruit NeoKey.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
 Keywords: adafruit,neokey,neopixel,mechanical,keyboard,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/README.rst` & `adafruit-circuitpython-neokey-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/PKG-INFO` & `adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neokey
-Version: 1.0.9
+Version: 1.1.0
 Summary: CircuitPython library for using Adafruit NeoKey.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoKey
 Keywords: adafruit,neokey,neopixel,mechanical,keyboard,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/adafruit_circuitpython_neokey.egg-info/SOURCES.txt` & `adafruit-circuitpython-neokey-1.1.0/adafruit_circuitpython_neokey.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_neokey.egg-info/PKG-INFO
 adafruit_circuitpython_neokey.egg-info/SOURCES.txt
 adafruit_circuitpython_neokey.egg-info/dependency_links.txt
 adafruit_circuitpython_neokey.egg-info/requires.txt
@@ -29,9 +30,10 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/neokey1x4_allkeys.py
 examples/neokey1x4_simpletest.py
 examples/neokey_1x4_multikey.py
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/adafruit_neokey/neokey1x4.py` & `adafruit-circuitpython-neokey-1.1.0/adafruit_neokey/neokey1x4.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
 # imports
 
-__version__ = "1.0.9"
+__version__ = "1.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoKey.git"
 
 from micropython import const
 from adafruit_seesaw import neopixel
 from adafruit_seesaw.seesaw import Seesaw
 
 try:
@@ -67,7 +67,20 @@
         for b in range(4, 8):
             self.pin_mode(b, self.INPUT_PULLUP)
 
     def __getitem__(self, index: int) -> bool:
         if not isinstance(index, int) or (index < 0) or (index > 3):
             raise RuntimeError("Index must be 0 thru 3")
         return not self.digital_read(index + 4)
+
+    def get_keys(self) -> typing.List[bool]:
+        """Read all 4 keys at once and return an array of booleans.
+
+        Returns:
+            typing.List[bool]: _description_
+        """
+        # use a bit mask with ports 4-7 to read all 4 keys at once
+        bulk_read = self.digital_read_bulk(0xF0)
+
+        # convert the leftmost 4 bits to an array of booleans and return
+        keys = [bulk_read & (1 << i) == 0 for i in range(4, 8)]
+        return keys
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/docs/_static/favicon.ico` & `adafruit-circuitpython-neokey-1.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/docs/conf.py` & `adafruit-circuitpython-neokey-1.1.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
@@ -47,15 +49,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit NeoKey Library"
-copyright = "2021 ladyada"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-neokey-1.0.9/docs/index.rst` & `adafruit-circuitpython-neokey-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/examples/neokey1x4_simpletest.py` & `adafruit-circuitpython-neokey-1.1.0/examples/neokey1x4_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/examples/neokey_1x4_multikey.py` & `adafruit-circuitpython-neokey-1.1.0/examples/neokey_1x4_multikey.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neokey-1.0.9/pyproject.toml` & `adafruit-circuitpython-neokey-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neokey"
 description = "CircuitPython library for using Adafruit NeoKey."
-version = "1.0.9"
+version = "1.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoKey"}
 keywords = [
     "adafruit",
```

