# Comparing `tmp/qslib-0.9.2.tar.gz` & `tmp/qslib-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qslib-0.9.2.tar", last modified: Mon Jul 31 18:16:06 2023, max compression
+gzip compressed data, was "qslib-1.8.2.tar", last modified: Sat Feb 25 16:40:15 2023, max compression
```

## Comparing `qslib-0.9.2.tar` & `qslib-1.8.2.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.770373 qslib-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-31 18:15:54.000000 qslib-0.9.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.758373 qslib-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.762373 qslib-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-31 18:15:54.000000 qslib-0.9.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-31 18:15:54.000000 qslib-0.9.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-07-31 18:15:54.000000 qslib-0.9.2/.github/workflows/python-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-31 18:15:54.000000 qslib-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 18:15:54.000000 qslib-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-31 18:15:54.000000 qslib-0.9.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.762373 qslib-0.9.2/.reuse/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-31 18:15:54.000000 qslib-0.9.2/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 18:15:54.000000 qslib-0.9.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-31 18:15:54.000000 qslib-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-07-31 18:15:54.000000 qslib-0.9.2/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.762373 qslib-0.9.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-07-31 18:15:54.000000 qslib-0.9.2/LICENSES/AGPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-07-31 18:15:54.000000 qslib-0.9.2/LICENSES/CC-BY-SA-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-07-31 18:15:54.000000 qslib-0.9.2/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-07-31 18:16:06.770373 qslib-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-31 18:15:54.000000 qslib-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.766373 qslib-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/CLA-individual.md
--rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.766373 qslib-0.9.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/commandline.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/experiments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/machines.rst
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/monitor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-31 18:15:54.000000 qslib-0.9.2/docs/tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.766373 qslib-0.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-07-31 18:15:54.000000 qslib-0.9.2/examples/qslib-example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 18:15:54.000000 qslib-0.9.2/examples/qslib-example.ipynb.license
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 18:15:54.000000 qslib-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-31 18:16:06.774373 qslib-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.762373 qslib-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.766373 qslib-0.9.2/src/qslib/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/_analysis_protocol_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    88832 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    23949 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25208 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/monitor_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/plate_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    62173 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/qs_is_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/qsconnection_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/rawquant_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/scpi_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-31 18:15:54.000000 qslib-0.9.2/src/qslib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.770373 qslib-0.9.2/src/qslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-31 18:16:06.000000 qslib-0.9.2/src/qslib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:16:06.770373 qslib-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   439264 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test.eds
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test.eds.license
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_accesslevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_experiment_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_experiment_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_fakeserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_is_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_real.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_scpicommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-31 18:15:54.000000 qslib-0.9.2/tests/test_util_fns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-31 18:15:54.000000 qslib-0.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.609372 qslib-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-02-25 16:40:05.000000 qslib-1.8.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.601372 qslib-1.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.601372 qslib-1.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-25 16:40:05.000000 qslib-1.8.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-02-25 16:40:05.000000 qslib-1.8.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-02-25 16:40:05.000000 qslib-1.8.2/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-25 16:40:05.000000 qslib-1.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-25 16:40:05.000000 qslib-1.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-25 16:40:05.000000 qslib-1.8.2/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.601372 qslib-1.8.2/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-25 16:40:05.000000 qslib-1.8.2/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-25 16:40:05.000000 qslib-1.8.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-02-25 16:40:05.000000 qslib-1.8.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-02-25 16:40:05.000000 qslib-1.8.2/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.601372 qslib-1.8.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-02-25 16:40:05.000000 qslib-1.8.2/LICENSES/AGPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21305 2023-02-25 16:40:05.000000 qslib-1.8.2/LICENSES/CC-BY-SA-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-02-25 16:40:05.000000 qslib-1.8.2/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-02-25 16:40:15.609372 qslib-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-02-25 16:40:05.000000 qslib-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.605372 qslib-1.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/CLA-individual.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.605372 qslib-1.8.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/commandline.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/experiments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/machines.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-02-25 16:40:05.000000 qslib-1.8.2/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.605372 qslib-1.8.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    36096 2023-02-25 16:40:05.000000 qslib-1.8.2/examples/qslib-example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-25 16:40:05.000000 qslib-1.8.2/examples/qslib-example.ipynb.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-02-25 16:40:05.000000 qslib-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-25 16:40:15.613372 qslib-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.601372 qslib-1.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.609372 qslib-1.8.2/src/qslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/_analysis_protocol_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87396 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/monitor_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/plate_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60094 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/qs_is_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/qsconnection_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/rawquant_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/scpi_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-25 16:40:05.000000 qslib-1.8.2/src/qslib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.609372 qslib-1.8.2/src/qslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-25 16:40:15.000000 qslib-1.8.2/src/qslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 16:40:15.609372 qslib-1.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   439264 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test.eds
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test.eds.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_accesslevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_experiment_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_experiment_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_fakeserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7831 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_scpicommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-02-25 16:40:05.000000 qslib-1.8.2/tests/test_util_fns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-25 16:40:05.000000 qslib-1.8.2/tox.ini
```

### Comparing `qslib-0.9.2/.coveragerc` & `qslib-1.8.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/.github/workflows/codeql-analysis.yml` & `qslib-1.8.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/.github/workflows/python-publish.yml` & `qslib-1.8.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/.github/workflows/python-tests.yml` & `qslib-1.8.2/.github/workflows/python-tests.yml`

 * *Files 9% similar despite different names*

```diff
@@ -49,15 +49,15 @@
   tests:
     runs-on: ${{ matrix.os }}
     needs: "mypy"
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.9", "3.10", "3.11"]
+        python-version: ["3.9", "3.10", "3.11.0"]
 
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
@@ -75,26 +75,29 @@
 
   direct_tests:
     runs-on: "self-hosted"
     needs: "tests"
 
     steps:
     - uses: actions/checkout@v3
+    # - name: Set up Python
+    #   uses: actions/setup-python@v4
+    #   with:
+    #     python-version: '3.11.0'
     - name: Install dependencies
       run: |
-        ~/qpcr-sim/actions-runner/runner-venv/bin/python -m pip install -U pip setuptools_scm[toml] wheel setuptools
-        ~/qpcr-sim/actions-runner/runner-venv/bin/python -m pip install -U flake8 mypy pytest pytest-cov pytest-asyncio hypothesis
-        ~/qpcr-sim/actions-runner/runner-venv/bin/python -m pip install -U .[monitor] --no-build-isolation
+        python -m pip install --upgrade pip setuptools_scm[toml] wheel setuptools
+        python -m pip install -U flake8 mypy pytest pytest-cov pytest-asyncio hypothesis
+        python -m pip install -U .[monitor] --no-build-isolation
     - name: Setup environment
       run: |
         start_realtest_environment
     - name: Test with tox/pytest
       run: |
-        ~/qpcr-sim/actions-runner/runner-venv/bin/python -m pytest -k 'test_real' --cov --cov-report=xml
+        python -m pytest -k 'test_real' --cov --cov-report=xml
     - name: Stop environment
       run: |
         stop_realtest_environment
     - name: "Upload coverage to Codecov"
       uses: codecov/codecov-action@v3
       with:
         fail_ci_if_error: false
-        token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `qslib-0.9.2/.gitignore` & `qslib-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/.pre-commit-config.yaml` & `qslib-1.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/CHANGELOG.md` & `qslib-1.8.2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,14 @@
 SPDX-FileCopyrightText: 2021-2022 Constantine Evans <const@costi.eu>
 
 SPDX-License-Identifier: AGPL-3.0-only
 -->
 
 # Changelog
 
-## Version 0.9.2
-
-- Fix a communications bug where a packet that can cause commands to hang in certain rare situations.
-
-## Version 0.9.1
-
-- Minor bug fixes and dependency updates (to fix pandas errors).
-- Fixes to support Pandas 2.0.
-- Ensure that some invalid characters are not used in machine names.
-- Check for files with and without spaces on machine when loading a new experiment (in case run was started outside of qslib).
-- Parse IOError messages from the machine.
-
-## Version 0.9.0
-
-- Fix `Stage.stepped_ramp` when all temperature increments are the same, but temperatures are not.
-- Add a `start_increment` option to `Stage.stepped_ramp` for cases where the user does not want the
-  ramp to actually start at the starting temperature, but at the first increment away from it (eg,
-  when continuing a previous ramp).
-- Ensure that units are delta units when appropriate in protocols, regardless of whether the user
-  entered them as delta units (eg, so "2°C" will work as a temperature step).
-
 ## Version 0.8.2
 
 - Add check for existing, completed EDS files with same name, and option to `Experiment.run` to overwrite completed or working files.
 - Fix XML protocol parsing bug for increment units with non-qslib EDS files.
 - Fix stage lines in plots.
 - Improve error messages.
```

### Comparing `qslib-0.9.2/LICENSE.txt` & `qslib-1.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/LICENSES/AGPL-3.0-only.txt` & `qslib-1.8.2/LICENSES/AGPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/LICENSES/CC-BY-SA-3.0.txt` & `qslib-1.8.2/LICENSES/CC-BY-SA-3.0.txt`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/LICENSES/GPL-3.0-only.txt` & `qslib-1.8.2/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/PKG-INFO` & `qslib-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qslib
-Version: 0.9.2
+Version: 1.8.2
 Summary: Library for communicating with and using the QuantStudio qPCR machine, intended for non-qPCR uses.
 Home-page: https://github.com/cgevans/qslib/
 Author: Constantine Evans
 Author-email: Constantine Evans <const@costi.eu>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
```

### Comparing `qslib-0.9.2/README.md` & `qslib-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/CLA-individual.md` & `qslib-1.8.2/docs/CLA-individual.md`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/LICENSE.txt` & `qslib-1.8.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/Makefile` & `qslib-1.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/changelog.md` & `qslib-1.8.2/docs/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,14 @@
 SPDX-FileCopyrightText: 2021-2022 Constantine Evans <const@costi.eu>
 
 SPDX-License-Identifier: AGPL-3.0-only
 -->
 
 # Changelog
 
-## Version 0.9.2
-
-- Fix a communications bug where a packet that can cause commands to hang in certain rare situations.
-
-## Version 0.9.1
-
-- Minor bug fixes and dependency updates (to fix pandas errors).
-- Fixes to support Pandas 2.0.
-- Ensure that some invalid characters are not used in machine names.
-- Check for files with and without spaces on machine when loading a new experiment (in case run was started outside of qslib).
-- Parse IOError messages from the machine.
-
-## Version 0.9.0
-
-- Fix `Stage.stepped_ramp` when all temperature increments are the same, but temperatures are not.
-- Add a `start_increment` option to `Stage.stepped_ramp` for cases where the user does not want the
-  ramp to actually start at the starting temperature, but at the first increment away from it (eg,
-  when continuing a previous ramp).
-- Ensure that units are delta units when appropriate in protocols, regardless of whether the user
-  entered them as delta units (eg, so "2°C" will work as a temperature step).
-
 ## Version 0.8.2
 
 - Add check for existing, completed EDS files with same name, and option to `Experiment.run` to overwrite completed or working files.
 - Fix XML protocol parsing bug for increment units with non-qslib EDS files.
 - Fix stage lines in plots.
 - Improve error messages.
```

### Comparing `qslib-0.9.2/docs/conf.py` & `qslib-1.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/experiments.rst` & `qslib-1.8.2/docs/experiments.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,14 @@
 These are often compatible with AB's software.
 
 .. autosummary::
    Protocol
    Stage
    Step
 
-There are also some convenience commands to construct often-used stages:
-
-.. autosummary::
-   Stage.stepped_ramp
-   Stage.hold_at
-
 While the parameters for these classes default to seconds and degrees Celsius, when using numbers as input, they also use the
 pint library to accept strings (or pint Quantity objects).  Thus, you can use :code:`"1 hr"` or :code:`"1 hour"` instead of :code:`3600`,
 or :code:`"59 °C"` or :code:`"59 degC"` for a temperature.  Note that for temperature increments, pint distinguishes between a temperature
 change and absolute temperature unit, so you would need to use, for example :code:`"-1 delta_degC"`.
 
 QSLib also supports custom steps, which can contain arbitrary SCPI commands.  For common commands, it also
 includes classes that allow more convenient use:
```

### Comparing `qslib-0.9.2/docs/index.rst` & `qslib-1.8.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/machines.rst` & `qslib-1.8.2/docs/machines.rst`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/setup.rst` & `qslib-1.8.2/docs/setup.rst`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/docs/tutorial.rst` & `qslib-1.8.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/examples/qslib-example.ipynb` & `qslib-1.8.2/examples/qslib-example.ipynb`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/pyproject.toml` & `qslib-1.8.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Programming Language :: Python :: 3.11",
     "Framework :: Matplotlib",
     "Framework :: Jupyter" ]
 
 dynamic = ["version"]
 
 dependencies = [
-"pandas >= 1.5",
+"pandas >= 1",
 "numpy >= 1",
 "tabulate >= 0.8",
 "pyparsing >= 3",
 "typeguard >= 2",
 "nest_asyncio >= 1.5",
 "click >=8.0,<9.0",
 "toml",
@@ -109,10 +109,7 @@
 
 
 [tool.mypy]
 python_version = "3.10"
 # warn_return_any = true
 warn_unused_configs = true
 ignore_missing_imports = true
-
-[tool.ruff]
-line-length = 120
```

### Comparing `qslib-0.9.2/setup.cfg` & `qslib-1.8.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.9
 install_requires = 
-	pandas >= 1.5
+	pandas >= 1
 	numpy >= 1
 	tabulate >= 0.8
 	pyparsing >=3
 	typeguard >=2
 	nest_asyncio >= 1.5
 	click >=8.0,<9.0
 	toml
```

### Comparing `qslib-0.9.2/src/qslib/__init__.py` & `qslib-1.8.2/src/qslib/__init__.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/_analysis_protocol_text.py` & `qslib-1.8.2/src/qslib/_analysis_protocol_text.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/_util.py` & `qslib-1.8.2/src/qslib/_util.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/base.py` & `qslib-1.8.2/src/qslib/base.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/cli.py` & `qslib-1.8.2/src/qslib/cli.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/data.py` & `qslib-1.8.2/src/qslib/data.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/experiment.py` & `qslib-1.8.2/src/qslib/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,20 @@
 from ._analysis_protocol_text import _ANALYSIS_PROTOCOL_TEXT
 from ._util import _nowuuid, _pp_seqsliceint, _set_or_create
 from .base import RunStatus
 from .data import FilterDataReading, FilterSet, df_from_readings
 from .machine import Machine
 from .processors import NormRaw, Processor
 from .protocol import Protocol, Stage, Step
-from .qs_is_protocol import QS_IOError
 from .rawquant_compat import _fdc_to_rawdata
 from .version import __version__
 
 if TYPE_CHECKING:  # pragma: no cover
     import matplotlib.pyplot as plt
 
-# Let's just assume all of these are problematic, for now.
-INVALID_NAME_RE = re.compile(r"[\[\]{}!/:;@&=+$,?#|\\]")
-
-
-def _safe_exp_name(name: str) -> str:
-    m = INVALID_NAME_RE.search(name)
-
-    if m:
-        raise ValueError(f"Invalid characters ({m[0]}) in run name: {name}.")
-
-    return name.replace(" ", "_")
-
 
 TEMPLATE_NAME = "ruo"
 
 _MANIFEST_CONTENTS = f"""Manifest-Version: 1.0
 Content-Type: Std
 Implementation-Title: QSLib
 Implementation-Version: {__version__}
@@ -487,16 +474,16 @@
         if len(self.plate_setup.sample_wells) <= 12:
             return self.info()
         else:
             return self.info(plate="table")
 
     @property
     def runtitle_safe(self) -> str:
-        """Run name with " " replaced by "_"; raises ValueError if name has other problematic characters."""
-        return _safe_exp_name(self.name)
+        """Run name with " " replaced by "_"."""
+        return self.name.replace(" ", "_")
 
     @property
     def rawdata(self) -> pd.DataFrame:
         warn("rawdata is deprecated; use welldata instead")
         if (self.activestarttime is None) or (self.welldata is None):
             raise DataError
         return _fdc_to_rawdata(
@@ -1054,18 +1041,14 @@
         self.machine: Machine | None = None
 
         if name is not None:
             self.name = name
         else:
             self.name = _nowuuid()
 
-        # Ensure that name is safe for use as a filename:
-        # this will raise a ValueError for us if it isn't.
-        self.runtitle_safe
-
         if protocol is None:
             self.protocol = Protocol([Stage([Step(60, 25)])])
         else:
             self.protocol = protocol
 
         if plate_setup:
             self.plate_setup = plate_setup
@@ -1262,69 +1245,53 @@
             a copy of the experiment
         """
         exp = cls(_create_xml=False)
 
         machine = exp._ensure_machine(machine)
 
         with machine.ensured_connection():
+            crt = name
+
             if move:
                 raise NotImplementedError
 
-            try:
-                z = machine.read_dir_as_zip(_safe_exp_name(name), leaf="EXP")
-            except QS_IOError:
-                try:
-                    z = machine.read_dir_as_zip(name, leaf="EXP")
-                except QS_IOError:
-                    raise ValueError(
-                        f"Could not find experiment {name} in uncollect runs on {machine}."
-                    )
+            if not crt:
+                raise ValueError("Nothing is currently running.")
+
+            z = machine.read_dir_as_zip(crt, leaf="EXP")
 
             z.extractall(exp._dir_base)
 
             exp._update_from_files()
 
         return exp
 
     @classmethod
     def from_machine_storage(cls, machine: MachineReference, name: str) -> Experiment:
-        """Create an experiment from the machine's storage.
+        """Create an experiment from the one currently running on a machine.
 
         Parameters
         ----------
         machine : Machine
-            the machine to connect to.
-
-        name: str
-            the name of the run to collect.
+            the machine to connect to
 
         Returns
         -------
         Experiment
             a copy of the experiment
         """
         exp = cls(_create_xml=False)
 
         machine = exp._ensure_machine(machine)
 
         with machine.ensured_connection():
-            o = None
-            for possible_name in [
-                _safe_exp_name(name) + ".eds",
-                _safe_exp_name(name),
-                name + ".eds",
-                name,
-            ]:
-                try:
-                    o = machine.read_file(possible_name, context="public_run_complete")
-                    break
-                except QS_IOError:
-                    continue
-            if o is None:
-                raise FileNotFoundError(f"Could not find {name} on {machine.host}.")
+            try:
+                o = machine.read_file(name + ".eds", context="public_run_complete")
+            except FileNotFoundError:
+                o = machine.read_file(name, context="public_run_complete")
 
             z = zipfile.ZipFile(io.BytesIO(o))
 
             z.extractall(exp._dir_base)
 
             exp._update_from_files()
 
@@ -1348,30 +1315,21 @@
         -------
         Experiment
             a copy of the experiment
         """
         if isinstance(machine, str):
             machine = Machine(machine)
 
-        safename = _safe_exp_name(name)
-
         with machine.ensured_connection():
-            if machine.current_run_name in [safename, name]:
+            if name == machine.current_run_name:
                 exp = cls.from_running(machine)
-                return exp
-
-            storage_runs = machine.list_runs_in_storage()
-            if (name in storage_runs) or (safename in storage_runs):
+            elif name in machine.list_runs_in_storage():
                 exp = cls.from_machine_storage(machine, name)
-                return exp
-
-            exp_runs = machine.list_files("", verbose=False, leaf="EXP")
-            if ((name + "/") in exp_runs) or ((safename + "/") in exp_runs):
+            elif name + "/" in machine.list_files("", verbose=False, leaf="EXP"):
                 exp = cls.from_uncollected(machine, name)
-
             else:
                 raise FileNotFoundError(f"Could not find run {name} on {machine.host}.")
         return exp
 
     def _update_experiment_xml(self) -> None:
         exml = ET.parse(os.path.join(self._dir_eds, "experiment.xml"))
 
@@ -1598,18 +1556,18 @@
                     stages[-1].setdefault("end_time", ts)
 
         self.stages = pd.DataFrame(stages, columns=["stage", "start_time", "end_time"])
 
         if self.activestarttime:
             self.stages["start_seconds"] = (
                 self.stages["start_time"] - self.activestarttime
-            ).astype("timedelta64[ms]").astype("int64") / 1000
+            ).astype("timedelta64[s]")
             self.stages["end_seconds"] = (
                 self.stages["end_time"] - self.activestarttime
-            ).astype("timedelta64[ms]").astype("int64") / 1000
+            ).astype("timedelta64[s]")
 
         tt = []
 
         try:
             # In normal runs, the protocol is there without the PROT command at the
             # beginning of the log as an info command, with quote.message.  Let's
             # try to grab it!
```

### Comparing `qslib-0.9.2/src/qslib/machine.py` & `qslib-1.8.2/src/qslib/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 
 from ._util import _unwrap_tags
 from .protocol import Protocol
 from .qsconnection_async import QSConnectionAsync
 
 nest_asyncio.apply()
 
-from .base import MachineStatus, RunStatus  # noqa: E402
+from .base import MachineStatus, RunStatus
 
 log = logging.getLogger(__name__)
 
 if TYPE_CHECKING:  # pragma: no cover
-    import matplotlib.pyplot as plt  # noqa: F401
+    import matplotlib.pyplot as plt
 
     from .experiment import Experiment
 
 
 def _ensure_connection(level: AccessLevel = AccessLevel.Observer) -> Any:
     def wrap(func):
         @wraps(func)
```

### Comparing `qslib-0.9.2/src/qslib/monitor.py` & `qslib-1.8.2/src/qslib/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         return n
 
     def statemsg(self, timestamp: str) -> str:
         s = f'run_state name="{self.name}"'
         if self.stage:
             s += f",stage={self.stage}i,cycle={self.cycle}i,step={self.step}i"
         else:
-            s += ",stage=0i,cycle=0i,step=0i"  # FIXME: not great
+            s += f",stage=0i,cycle=0i,step=0i"  # FIXME: not great
         s += f" {timestamp}"
         return s
 
 
 @dataclass
 class MachineState:
     zone_targets: List[float]
@@ -558,15 +558,15 @@
             self.inject(
                 f'run_action,type={action} run_name="{state.run.name}" {timestamp}'  # noqa: E501
             )
             asyncio.tasks.create_task(self.docollect(msg.opts, state, c))
         else:
             self.inject(
                 Point("run_action")
-                .tag("type", "Other")
+                .tag("type", f"Other")
                 .tag("run_name", state.run.name)
                 .field("message", " ".join(str(x) for x in contents))
                 .time(timestamp)
             )
 
         await state.run.refresh(c)
         await state.machine.refresh(c)
```

### Comparing `qslib-0.9.2/src/qslib/monitor_cli.py` & `qslib-1.8.2/src/qslib/monitor_cli.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/plate_setup.py` & `qslib-1.8.2/src/qslib/plate_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         color: Tuple[int, int, int, int] = (255, 0, 0, 255),
         properties: dict[str, str] | None = None,
         description: str | None = None,
         wells: str | list[str] | None = None,
     ) -> None:
         if properties is None:
             properties = dict()
-        if "SP_UUID" not in properties:
+        if not "SP_UUID" in properties:
             if not uuid:
                 uuid = uuid1().hex
             properties["SP_UUID"] = uuid
         if wells is None:
             wells = list()
         self.__attrs_init__(name, color, properties, description, wells=wells)  # type: ignore
 
@@ -256,19 +256,19 @@
             for ((r, c), s) in zip(_WELLALPHREF, self.well_sample)
         ]
 
     @classmethod
     def from_array(
         cls, array: Union[np.ndarray, pd.DataFrame], *, make_unique: bool = False
     ) -> PlateSetup:
-        raise NotImplementedError
+        raise NotImplemented
 
     @classmethod
     def from_tsv(cls, tsvstr: str) -> PlateSetup:
-        raise NotImplementedError
+        raise NotImplemented
 
     def to_table(
         self,
         headers: Sequence[Union[str, int]] = list(range(1, 13)),
         tablefmt: str = "orgtbl",
         showindex: Sequence[str] = tuple("ABCDEFGH"),
         **kwargs: Any,
```

### Comparing `qslib-0.9.2/src/qslib/processors.py` & `qslib-1.8.2/src/qslib/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,16 +120,16 @@
     scope: ClassVar[ScopeType] = "limited"
 
     def __attrs_post_init__(self):
         pass
 
     def ylabel(self, previous_label: str | None = None) -> str:
         if previous_label is None:
-            return "fluorescence (EMW-smoothed)"
-        return re.sub(r"\(([^)]+)\)", r"(\1, EMW-smoothed)", previous_label)
+            return f"fluorescence (EMW-smoothed)"
+        return re.sub(r"\(([^)]+)\)", rf"(\1, EMW-smoothed)", previous_label)
 
     def process_scoped(self, data: pd.DataFrame, scope: ScopeType) -> pd.DataFrame:
         if scope == self.scope:
             return self.process(data)
         else:
             return data
```

### Comparing `qslib-0.9.2/src/qslib/protocol.py` & `qslib-1.8.2/src/qslib/protocol.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,71 +51,55 @@
 
 NZONES = 6
 
 UR: pint.UnitRegistry = pint.UnitRegistry(
     autoconvert_offset_to_baseunit=True, auto_reduce_dimensions=True
 )
 
-Q_ = UR.Quantity
 
 log = logging.getLogger(__name__)
 
 
-def _check_unit_or_fail(val: pint.Quantity, unit: str | pint.Unit) -> None:
-    if not val.check(unit):
-        raise pint.DimensionalityError(val.u, unit)
-
-
 def _wrap_seconds(val: int | float | str | pint.Quantity) -> pint.Quantity:
     if isinstance(val, str):
-        uv = Q_(val)
-        _check_unit_or_fail(uv, "seconds")
+        uv = UR.Quantity(val)
+        uv.check("seconds")
     elif isinstance(val, pint.Quantity):
         uv = val
-        _check_unit_or_fail(uv, "seconds")
+        uv.check("seconds")
     else:
-        uv = Q_(val, "seconds")
+        uv = UR.Quantity(val, "seconds")
     return uv
 
 
 def _wrap_degC(val: int | float | str | pint.Quantity) -> pint.Quantity:
     if isinstance(val, str):
-        uv = Q_(val)
-        _check_unit_or_fail(uv, "degC")
+        uv = UR.Quantity(val)
+        uv.check("degC")
     elif isinstance(val, pint.Quantity):
         uv = val
-        _check_unit_or_fail(uv, "degC")
+        uv.check("degC")
     else:
-        uv = Q_(val, "degC")
+        uv = UR.Quantity(val, "degC")
     return uv
 
 
 def _wrap_delta_degC(val: int | float | str | pint.Quantity) -> pint.Quantity:
     if isinstance(val, str):
-        uv = Q_(val)
-        uv = _ensure_delta_temperature(uv)
+        uv = UR.Quantity(val)
+        uv.check("delta_degC")
     elif isinstance(val, pint.Quantity):
         uv = val
-        uv = _ensure_delta_temperature(uv)
+        uv.check("delta_degC")
     else:
-        uv = Q_(val, "delta_degC")
+        uv = UR.Quantity(val, "delta_degC")
     return uv
 
 
-def _ensure_delta_temperature(val: pint.Quantity) -> pint.Quantity:
-    _check_unit_or_fail(val, "delta_degC")
-
-    # Are we multiplicative?
-    if not UR._units[str(val.u)].is_multiplicative:
-        return Q_(val.m, "delta_" + str(val.u))
-
-    return val
-
-
-_ZEROTEMPDELTA = Q_(0.0, "delta_degC")
+_ZEROTEMPDELTA = UR.Quantity(0.0, "delta_degC")
 
 
 def _wrap_delta_degC_or_zero(
     val: int | float | str | pint.Quantity | None,
 ) -> pint.Quantity:
     if val is None:
         return _ZEROTEMPDELTA
@@ -135,34 +119,34 @@
 def _wrapunitmaybelist_degC(
     val: int
     | float
     | str
     | pint.Quantity
     | Sequence[int | float | str | pint.Quantity],
 ) -> pint.Quantity:
-    unit: pint.Unit = UR.Unit("degC")
+    unit: pint.Unit = cast(pint.Unit, UR("degC"))
 
     if isinstance(val, pint.Quantity):
         uv = val
-        _check_unit_or_fail(uv, unit)
+        uv.check(unit)
     elif isinstance(val, str):
         uv = UR(val)
-        _check_unit_or_fail(uv, unit)
+        uv.check(unit)
     elif isinstance(val, Sequence):
         m = []
         for x in val:
             if isinstance(x, pint.Quantity):
                 m.append(x.to(unit).magnitude)
             elif isinstance(x, str):
-                m.append(Q_(x).to(unit).magnitude)
+                m.append(UR.Quantity(x).to(unit).magnitude)
             else:
                 m.append(x)
-        return Q_(m, unit)
+        return UR.Quantity(m, unit)
     else:
-        uv = Q_(val, unit)
+        uv = UR.Quantity(val, unit)
     return uv
 
 
 def _durformat(time: pint.Quantity[int]) -> str:
     """Convert time in seconds to a nice string"""
     time_s: int = time.to(UR.seconds).magnitude
     s = ""
@@ -252,15 +236,15 @@
 
         return SCPICommand(
             "RAMP", *self.temperature.to("degC").magnitude, comment=None, **opts
         )
 
     @classmethod
     def from_scpicommand(cls, sc: SCPICommand) -> Ramp:
-        return Ramp(Q_(sc.args, "degC"), **sc.opts)  # type: ignore
+        return Ramp(UR.Quantity(sc.args, "degC"), **sc.opts)  # type: ignore
 
 
 @dataclass
 class Exposure(ProtoCommand):
     """Modifies exposure settings."""
 
     # We don't support persistent... it doesn't seem safe
@@ -330,15 +314,15 @@
 
 
 @dataclass
 class HoldAndCollect(ProtoCommand):
     """A protocol hold (for a time) and collect (set by HACFILT) command."""
 
     time: pint.Quantity[int]
-    increment: pint.Quantity[int] = Q_(0, "seconds")
+    increment: pint.Quantity[int] = UR.Quantity(0, "seconds")
     incrementcycle: int = 1
     incrementstep: int = 1
     tiff: bool = False
     quant: bool = True
     pcr: bool = False
     _names: ClassVar[Sequence[str]] = ("HoldAndCollect",)
 
@@ -358,23 +342,23 @@
             int(self.time.to("seconds").magnitude),
             comment=None,
             **opts,
         )
 
     @classmethod
     def from_scpicommand(cls, sc: SCPICommand) -> HoldAndCollect:
-        return HoldAndCollect(Q_(cast(int, sc.args[0]), "seconds"), **sc.opts)  # type: ignore
+        return HoldAndCollect(UR.Quantity(cast(int, sc.args[0]), "seconds"), **sc.opts)  # type: ignore
 
 
 @dataclass
 class Hold(ProtoCommand):
     """A protocol hold (for a time) command."""
 
     time: pint.Quantity[int] | None
-    increment: pint.Quantity[int] = Q_(0, "seconds")
+    increment: pint.Quantity[int] = UR.Quantity(0, "seconds")
     incrementcycle: int = 1
     incrementstep: int = 1
     _names: ClassVar[Sequence[str]] = ("HOLD",)
 
     def to_scpicommand(self, **kwargs: None) -> SCPICommand:
         opts = {}
         if self.increment != Hold.increment:
@@ -388,15 +372,15 @@
             int(self.time.to("seconds").magnitude) if self.time is not None else "",
             comment=None,
             **opts,
         )
 
     @classmethod
     def from_scpicommand(cls, sc: SCPICommand) -> Hold:
-        return Hold(Q_(cast(int, sc.args[0]), "seconds"), **sc.opts)  # type: ignore
+        return Hold(UR.Quantity(cast(int, sc.args[0]), "seconds"), **sc.opts)  # type: ignore
 
 
 class XMLable(ABC):
     @abstractmethod
     def to_xml(self, **kwargs: Any) -> ET.Element:
         ...
 
@@ -480,18 +464,18 @@
         s += "\n".join(
             f"  {i+1}. " + c.to_scpicommand().to_string()
             for i, c in enumerate(self._body)
         )
         return s
 
     def duration_at_cycle(self, cycle: int) -> pint.Quantity[int]:  # cycle from 1
-        return Q_(0, "second")
+        return UR.Quantity(0, "second")
 
     def temperatures_at_cycle(self, cycle: int) -> pint.Quantity[np.ndarray]:
-        return Q_(np.array(6 * [math.nan]), "degC")
+        return UR.Quantity(np.array(6 * [math.nan]), "degC")
 
     def total_duration(self, repeat: int = 1) -> pint.Quantity[int]:
         return 0 * UR.seconds
 
     @property
     def body(self) -> list[ProtoCommand]:
         return self._body
@@ -609,15 +593,15 @@
         default=_ZEROTEMPDELTA,
         converter=_wrap_delta_degC,
         on_setattr=attr.setters.convert,
     )
     temp_incrementcycle: int = 2
     temp_incrementpoint: int = 2
     time_increment: pint.Quantity[int] = attr.field(
-        default=Q_(0, UR.second),
+        default=UR.Quantity(0, UR.second),
         converter=_wrap_seconds,
         on_setattr=attr.setters.convert,
     )
     time_incrementcycle: int = 2
     time_incrementpoint: int = 2
     filters: Sequence[FilterSet] = attr.field(
         default=tuple(),
@@ -681,17 +665,17 @@
         tempstr = "{:.2f~}".format(temperatures_cycle1)  # type: ignore
         if (repeats > 1) and (self.temp_increment != 0.0):
             temperatures = self.temperatures_at_cycle(repeats)
             temperatures = convert_quantity_ndarray_to_scalar_if_all_equal(temperatures)
             t = "{:.2f~}".format(temperatures)  # type: ignore
             tempstr += f" to {t}"
 
-        elems = [f"{tempstr} for {self.time:~}/cycle"]
+        elems = [f"{tempstr} for {self.time}/cycle"]
         if self.temp_increment != 0.0:
-            elems.append(f"{self.temp_increment:~}/cycle")
+            elems.append(f"{self.temp_increment}°C/cycle")
             if self.temp_incrementcycle > 1:
                 elems[-1] += f" from cycle {self.temp_incrementcycle}"
         if self.time_increment != 0.0:
             elems.append(f"{_durformat(self.time_increment)}/cycle")
             if self.time_incrementcycle != 2:
                 elems[
                     -1
@@ -744,17 +728,17 @@
     def identifier(self, v: Any) -> None:
         raise ValueError
 
     @property
     def temperature_list(self) -> pint.Quantity[np.ndarray]:
         mag = self.temperature.to("degC").magnitude  # FIXME
         if isinstance(mag, np.ndarray):
-            return Q_(mag, "degC")
+            return UR.Quantity(mag, "degC")
         else:
-            return Q_(NZONES * [mag], "degC")
+            return UR.Quantity(NZONES * [mag], "degC")
 
     @property
     def body(self) -> list[ProtoCommand]:
         if self.collects:
             return [
                 Ramp(
                     self.temperature_list,
@@ -794,15 +778,15 @@
         raise ValueError
 
     @classmethod
     def from_xml(
         cls, e: ET.Element, *, etc: int = 1, ehtc: int = 1, he: bool = False
     ) -> Step:
         collect = bool(int(e.findtext("CollectionFlag") or 0))
-        ts: pint.Quantity[np.ndarray] = Q_(
+        ts: pint.Quantity[np.ndarray] = UR.Quantity(
             [float(x.text or math.nan) for x in e.findall("Temperature")], "degC"
         )
         ht: pint.Quantity[int] = int(e.findtext("HoldTime") or 0) * UR.seconds
         et: pint.Quantity[float] = (
             float(e.findtext("ExtTemperature") or 0.0) * UR.delta_degC
         )
         eht: pint.Quantity[int] = int(e.findtext("ExtHoldTime") or 0) * UR.seconds
@@ -948,164 +932,131 @@
         ):
             return False
         return self.steps == other.steps
 
     @classmethod
     def stepped_ramp(
         cls: Type[Stage],
-        from_temperature: float | str | pint.Quantity[float] | Sequence[float] | None,
+        from_temperature: float | str | pint.Quantity[float] | Sequence[float],
         to_temperature: float | str | pint.Quantity[float] | Sequence[float],
         total_time: int | str | pint.Quantity[int],
         *,
         n_steps: int | None = None,
         temperature_step: float | str | pint.Quantity[float] | None = None,
         collect: bool | None = None,
         filters: Sequence[str | FilterSet] = tuple(),
-        start_increment: bool = False,
     ) -> Stage:
         """Hold at a series of temperatures, from one to another.
 
         Parameters
         ----------
         from_temperature
-            Initial temperature/s (inclusive).  If None, uses the final temperature of
-            the previous stage.
+            Initial temperature/s (inclusive).
         to_temperature
             Final temperature/s (inclusive).
         total_time
             Total time for the stage
         n_steps
             Number of steps.  If None, uses 1.0 Δ°C steps, or, if
             doing a multi-temperature change, uses maximum step
-            of 1.0 Δ°C.  If n_steps is specified, it is the number of
-            temperature *steps* to take.  Normally, since there is
-            an initial cycle of the starting temperatures, this means
-            there will be `n_steps + 1` cycles.  If start_increment is True,
-            and the initial cycle is already stepped away from the starting
-            temperature, then there will be only `n_steps` cycles.
+            of 1.0 Δ°C.
         temperature_step
             Step temperature change (optional).  Must be None,
             or correctly match calculation, if n_steps is not
             None.  If both this and n_steps are None, default
             is 1.0 Δ°C steps.  If temperature step does not
             exactly fit range, it will be adjusted, with a warning
             if the change is more than 5%.  Sign is ignored.  If
             doing a multi-temperature change, then this is the
             maximum temperature step.
         collect
             Collect data?  If None, collects data if filters is set explicitly.
         filters
             Filters to collect.
-        start_increment
-            If False (default), start at the `from_temperature`, holding there
-            for the same hold time as every other temperature.  If True, start
-            one step away from the `from_temperature`.  This is useful, for
-            example, if the previous stage held at a particular temperature,
-            and you now want to step *away* from that temperature.  When True,
-            note the remarks about n_steps above.
 
         Returns
         -------
         Stage
             The resulting stage.
         """
 
         from_temperature = _wrapunitmaybelist_degC(from_temperature)
         to_temperature = _wrapunitmaybelist_degC(to_temperature)
 
         delta = to_temperature - from_temperature
 
         multistep = False
 
-        if hasattr(delta, "shape") and len(delta.shape) > 0:
-            max_delta = delta.max()  # type: pint.Quantity[float]
+        if hasattr(delta, "shape"):
+            if (delta != delta[0]).any():
+                multistep = True
+                max_delta = delta.max()  # type: pint.Quantity[float]
+            else:
+                max_delta = delta[0]
         else:
             max_delta = delta
 
         total_time = _wrap_seconds(total_time).to("seconds")
 
         if n_steps is None:
             if temperature_step is None:
-                temperature_step = Q_(1.0, "delta_degC")
-                autoset_step = True
+                temperature_step = UR("1.0 delta_degC")
             else:
                 temperature_step = abs(_wrap_delta_degC(temperature_step))
-                autoset_step = False
 
-            n_steps = max(
-                abs(round((max_delta / temperature_step).to("").magnitude))
-                + (0 if start_increment else 1),
-                1,
-            )
+            n_steps = abs(round((max_delta / temperature_step).to("").magnitude)) + 1
 
-            real_max_temperature_step = abs(
-                max_delta / (n_steps - (0 if start_increment else 1))
-            )
+            real_max_temperature_step = abs(max_delta / (n_steps - 1))
 
             change = (
                 ((real_max_temperature_step - temperature_step) / temperature_step)
                 .to("")
                 .magnitude
             )
 
-            if (abs(change) > 0.05) and not autoset_step:
+            if abs(change) > 0.05:
                 warnings.warn(
                     f"Desired temperature step {temperature_step} differs by {100*change}% from actual {real_max_temperature_step}."
                 )
 
         elif temperature_step is not None:
             temperature_step = abs(_wrap_delta_degC(temperature_step))
             if (
-                abs(round((max_delta / temperature_step).to("").magnitude))
-                + (0 if start_increment else 1)
+                abs(round((max_delta / temperature_step).to("").magnitude)) + 1
                 != n_steps
             ):
                 raise ValueError(
                     "Both n_steps and temperature_step set, and calculated steps don't match set steps."
                 )
 
-        temp_increment = (
-            (to_temperature - from_temperature)
-            / (n_steps - (0 if start_increment else 1))
-        ).round(4)
-
-        # If the temp_increment is entirely equal, we are not multistep, and we should
-        # have only a single temp_increment.
-
-        if hasattr(temp_increment, "shape") and len(temp_increment.shape) > 0:
-            if (temp_increment != temp_increment[0]).any():
-                multistep = True
-            else:
-                temp_increment = temp_increment[0]
+        temp_increment = ((to_temperature - from_temperature) / (n_steps - 1)).round(4)
 
         step_time = (total_time / n_steps).round()
 
         if not multistep:
             return cls(
                 [
                     Step(
                         step_time,
                         from_temperature,
                         collect=collect,
                         temp_increment=temp_increment,
                         filters=filters,
-                        temp_incrementcycle=(1 if start_increment else 2),
                     )
                 ],
                 repeat=n_steps,
             )
 
         # MULTISTEP!
 
         return cls(
             [
                 Step(
                     step_time,
-                    from_temperature
-                    + (step_i + (1 if start_increment else 0)) * temp_increment,
+                    from_temperature + step_i * temp_increment,
                     collect=collect,
                     filters=filters,
                 )
                 for step_i in range(0, n_steps)
             ]
         )
 
@@ -1381,15 +1332,15 @@
         stepstrs = [
             textwrap.indent(f"{step.info_str(i+1, self.repeat)}", "    ")
             for i, step in enumerate(self.steps)
         ]
         try:
             tot_dur = sum(
                 (x.total_duration(self.repeat) for x in self.steps),
-                Q_(0, UR.seconds),
+                UR.Quantity(0, UR.seconds),
             )
             stagestr += f" (total duration {_durformat(tot_dur)})"
         except KeyError:
             pass
         if len(stepstrs) > 1:
             stagestr += " of:\n" + "\n".join(stepstrs)
         else:
```

### Comparing `qslib-0.9.2/src/qslib/qs_is_protocol.py` & `qslib-1.8.2/src/qslib/qs_is_protocol.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import logging
 import re
 import time
 from asyncio.futures import Future
 from dataclasses import dataclass
 from typing import Any, Coroutine, Optional, Protocol, Type
 
-from .scpi_commands import AccessLevel, SCPICommand, _arglist
+from .scpi_commands import AccessLevel, SCPICommand
 
-NL_OR_Q = re.compile(rb"(?:\n|<(/?)([\w.]+)[ *]*>?)")
+NL_OR_Q = re.compile(rb"(?:\n|<(/?)([\w.]+)[ *]*>)")
+Q_ONLY = re.compile(rb"<(/?)([\w.]+)[ *]*>")
 TIMESTAMP = re.compile(rb"(\d{8,}\.\d{3})")
 
 log = logging.getLogger(__name__)
 
 
 def _validate_command_format(commandstring: bytes) -> None:
     # This is meant to validate that the command will not mess up comms
@@ -65,40 +66,20 @@
             return COM_ERRORS[m[1]].parse(command, ref_index, m[2])
         except ValueError:
             return UnparsedCommandError(command, ref_index, response)
 
 
 @dataclass
 class UnparsedCommandError(CommandError):
-    """The machine has returned an error that we are not familiar with,
-    and that we haven't parsed."""
-
     command: Optional[str]
     ref_index: Optional[str]
     response: str
 
 
 @dataclass
-class QS_IOError(CommandError):
-    command: str
-    message: str
-    data: dict[str, str]
-
-    @classmethod
-    def parse(cls, command: str, ref_index: str, message: str) -> QS_IOError:
-        m = re.match(r"(.*) --> (.*)", message)
-        if not m:
-            raise ValueError
-
-        data = _arglist.parse_string(m[1])[0].opts
-
-        return cls(command, m[2], data)
-
-
-@dataclass
 class InsufficientAccess(CommandError):
     command: str
     requiredAccess: AccessLevel
     currentAccess: AccessLevel
     message: str
 
     @classmethod
@@ -160,15 +141,14 @@
 
 COM_ERRORS: dict[str, Type[CommandError]] = {
     "InsufficientAccess": InsufficientAccess,
     "AuthError": AuthError,
     "AccessLevelExceeded": AccessLevelExceeded,
     "InvocationError": InvocationError,
     "NoMatch": NoMatch,
-    "IOError": QS_IOError,
 }
 
 
 class ReplyError(IOError):
     pass
 
 
@@ -222,15 +202,14 @@
         # setup connection.
         self.transport = transport
         self.waiting_commands = []
         self.buffer = io.BytesIO()
         self.quote_stack: list[bytes] = []
         self.topic_handlers: dict[bytes, SubHandler] = {}
         self.last_received = time.time()
-        self.unclosed_quote_pos: int | None = None
 
     async def _default_topic_handler(
         self, topic: bytes, message: bytes, timestamp: Optional[float] = None
     ) -> None:
         log.info(f"{topic.decode()} at {timestamp}: {message.decode()}")
         self.last_received = time.time()
 
@@ -284,47 +263,26 @@
         """Process received data packet from instrument, keeping track of quotes. If
         a newline occurs when the quote stack is empty, create a task to process
         the message, but continue processing. (TODO: consider threads/processes here.)
 
         :param data: bytes:
 
         """
-        log.debug(f"Received {data!r}")
-
-        # If we have an unclosed tag opener (<) in the buffer, add it to the data
-        if self.unclosed_quote_pos is not None:
-            self.buffer.write(data)
-            self.buffer.seek(self.unclosed_quote_pos)
-            data = self.buffer.read()
-            self.buffer.truncate(self.unclosed_quote_pos)
-            self.buffer.seek(self.unclosed_quote_pos)
-            self.unclosed_quote_pos = None
-            print(data)
-
         lastwrite = 0
         for m in NL_OR_Q.finditer(data):
             if m[0] == b"\n":
                 if len(self.quote_stack) == 0:
                     self.buffer.write(data[lastwrite : m.end()])
                     lastwrite = m.end()
                     asyncio.create_task(self.parse_message(self.buffer.getvalue()))
                     self.buffer = io.BytesIO()
                 # else:  # This is not actually needed
                 #     continue
             else:
-                if m[0][-1] != ord(">"):
-                    if m.end() != len(data):
-                        raise ValueError(data, m[0])
-                    # We have an unclosed tag opener (<) at the end of the data
-                    log.debug(f"Unclosed tag opener: {m[0]!r}")
-                    self.buffer.write(data[lastwrite : m.start()])
-                    self.unclosed_quote_pos = self.buffer.tell()
-                    self.buffer.write(m[0])
-                    lastwrite = m.end()
-                elif not m[1]:
+                if not m[1]:
                     self.quote_stack.append(m[2])
                 else:
                     try:
                         i = self.quote_stack.index(m[2])
                     except ValueError:
                         log.error(
                             f"Close quote {m[2]!r} did not have open in stack {self.quote_stack}. Disconnecting to avoid corruption."
```

### Comparing `qslib-0.9.2/src/qslib/qsconnection_async.py` & `qslib-1.8.2/src/qslib/qsconnection_async.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/rawquant_compat.py` & `qslib-1.8.2/src/qslib/rawquant_compat.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib/scpi_commands.py` & `qslib-1.8.2/src/qslib/scpi_commands.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/src/qslib.egg-info/PKG-INFO` & `qslib-1.8.2/src/qslib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qslib
-Version: 0.9.2
+Version: 1.8.2
 Summary: Library for communicating with and using the QuantStudio qPCR machine, intended for non-qPCR uses.
 Home-page: https://github.com/cgevans/qslib/
 Author: Constantine Evans
 Author-email: Constantine Evans <const@costi.eu>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
         Version 3, 19 November 2007
```

### Comparing `qslib-0.9.2/src/qslib.egg-info/SOURCES.txt` & `qslib-1.8.2/src/qslib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -66,12 +66,11 @@
 tests/test_accesslevel.py
 tests/test_basic.py
 tests/test_cli.py
 tests/test_experiment.py
 tests/test_experiment_file.py
 tests/test_experiment_run.py
 tests/test_fakeserver.py
-tests/test_is_protocol.py
 tests/test_protocol.py
 tests/test_real.py
 tests/test_scpicommand.py
 tests/test_util_fns.py
```

### Comparing `qslib-0.9.2/tests/test.eds` & `qslib-1.8.2/tests/test.eds`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_accesslevel.py` & `qslib-1.8.2/tests/test_accesslevel.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_basic.py` & `qslib-1.8.2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_cli.py` & `qslib-1.8.2/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # SPDX-FileCopyrightText: 2021-2022 Constantine Evans <const@costi.eu>
 # SPDX-License-Identifier: AGPL-3.0-only
 
-import sys
-
 import pytest
 from click.testing import CliRunner
 
 from qslib import Experiment, Machine
 from qslib.cli import cli
 
 
@@ -24,17 +22,14 @@
     result = runner.invoke(
         cli,
         ["info", "tests/test.eds"],
     )
     assert exp.info().rstrip() == result.output.rstrip()
 
 
-@pytest.mark.skipif(
-    sys.platform.startswith("win"), reason="HTML output not identical on Windows."
-)
 def test_html(exp, tmp_path_factory: pytest.TempPathFactory, runner: CliRunner):
     tp = tmp_path_factory.mktemp("temp_html")
     result = runner.invoke(
         cli,
         ["info-html", "-o", str(tp / "test.html"), "--no-open", "tests/test.eds"],
     )
     assert exp.info_html()[0:100] == open(tp / "test.html").read()[0:100]
```

### Comparing `qslib-0.9.2/tests/test_experiment.py` & `qslib-1.8.2/tests/test_experiment.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,13 +17,7 @@
         exp.plot_temperatures()
 
     with pytest.raises(ValueError, match="no data available"):
         exp.plot_over_time()
 
     with pytest.raises(ValueError, match="no data available"):
         exp.plot_anneal_melt()
-
-
-@pytest.mark.parametrize("ch", ["/", "!", "}"])
-def test_unsafe_names(ch):
-    with pytest.raises(ValueError, match=r"Invalid characters \(" + ch + r"\)"):
-        exp = Experiment(name=f"a{ch}b")
```

### Comparing `qslib-0.9.2/tests/test_experiment_file.py` & `qslib-1.8.2/tests/test_experiment_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,30 +46,30 @@
     assert exp.name == exp_reloaded.name
     assert exp.protocol == exp_reloaded.protocol
     assert exp.plate_setup == exp_reloaded.plate_setup
 
 
 def test_plot_ntmpw_smoothmw(exp: Experiment) -> None:
     axf, axt = exp.plot_over_time(
-        process=[SmoothWindowMean(4), NormToMeanPerWell(2)], annotate_stage_lines=False
+        process=[SmoothWindowMean(4), NormToMeanPerWell(1)], annotate_stage_lines=False
     )
     assert axf.get_ylabel() == "fluorescence (window mean 4, norm. to mean)"
 
 
 def test_plot_emw_maxperwell(exp: Experiment) -> None:
     axf, axt = exp.plot_over_time(
-        process=[SmoothEMWMean(alpha=0.1), NormToMaxPerWell(2)],
+        process=[SmoothEMWMean(alpha=0.1), NormToMaxPerWell(1)],
         annotate_stage_lines=False,
     )
     assert axf.get_ylabel() == "fluorescence (EMW-smoothed, norm. to max)"
 
 
 def test_plot_subtrbymean(exp: Experiment) -> None:
     axf, axt = exp.plot_over_time(
-        process=SubtractByMeanPerWell(2), annotate_stage_lines=False
+        process=SubtractByMeanPerWell(1), annotate_stage_lines=False
     )
     assert axf.get_ylabel() == "fluorescence (subtr. by mean)"
 
 
 def test_plots(exp: Experiment) -> None:
     axf, axt = exp.plot_over_time(
         legend=False, figure_kw={"constrained_layout": False}, annotate_stage_lines=True
```

### Comparing `qslib-0.9.2/tests/test_experiment_run.py` & `qslib-1.8.2/tests/test_experiment_run.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_fakeserver.py` & `qslib-1.8.2/tests/test_fakeserver.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_protocol.py` & `qslib-1.8.2/tests/test_protocol.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import PathLike
 
 import numpy as np
 import pytest
 
 import qslib.protocol as tc
 from qslib import Experiment
-from qslib.protocol import Q_, UR, Exposure, FilterSet, Protocol, Stage, Step
+from qslib.protocol import UR, Exposure, FilterSet, Protocol, Stage, Step
 from qslib.scpi_commands import SCPICommand  # noqa
 
 PROTSTRING = """PROTOCOL -volume=30 -runmode=standard testproto <multiline.protocol>
 \tSTAGE 1 STAGE_1 <multiline.stage>
 \t\tSTEP 1 <multiline.step>
 \t\t\tRAMP -incrementcycle=2 -incrementstep=2 80 80 80 80 80 80
 \t\t\tHOLD -incrementcycle=2 -incrementstep=2 300
@@ -238,59 +238,7 @@
     assert srstage == Stage(Step(60, 40.0, temp_increment=0.5), 41)
 
 
 def test_exposure_roundtrip():
     e = Exposure([(FilterSet(1, 4), [500, 2000])])
     s = e.to_scpicommand().to_string()
     assert SCPICommand.from_string(s).specialize() == e
-
-
-def test_stepped_ramp_multi_same_increment():
-    p1 = Protocol(
-        [
-            Stage.stepped_ramp(
-                [50, 50, 50, 40, 40, 40], [40, 40, 40, 30, 30, 30], "11 min"
-            ),
-            Stage.stepped_ramp(
-                [40, 40, 40, 30, 30, 30],
-                [30, 30, 30, 20, 20, 20.0],
-                "10 min",
-                start_increment=True,
-            ),
-            # Stage.stepped_ramp(None, [20,20,20,10,10,10], "9 min", start_increment=True), # FIXME: implement this
-        ]
-    )
-
-    s = str(p1)
-
-    p1.to_scpicommand()
-
-    assert (
-        (p1.dataframe.loc[:, "temperature_1":"temperature_6"].diff()[1:] == -1)
-        .all()
-        .all()
-    )
-    assert (p1.dataframe.start_time.diff()[1:] == 60.625).all()
-    assert (p1.dataframe.end_time.diff()[1:] == 60.625).all()
-
-
-def test_delta_unit_conversion():
-    assert (
-        Stage.stepped_ramp(
-            "50 °C", "20 °C", total_time="30 min", temperature_step="2 °C"
-        )
-        == Stage.stepped_ramp(
-            "50 °C", "20 °C", total_time="30 min", temperature_step="2 delta_degC"
-        )
-        == Stage.stepped_ramp(
-            "50 °C", "20 °C", total_time="30 min", temperature_step="3.6 degF"
-        )
-    )
-
-
-def test_hold():
-    h = Stage.hold_at("60 °C", "1 hour", "10 minutes")
-    assert h == Stage(Step("10 min", "60 °C"), 6)
-
-    assert Stage.hold_at("50 °C", total_time="1 hour").steps[0].duration_at_cycle(
-        0
-    ) == Q_("1 hour")
```

### Comparing `qslib-0.9.2/tests/test_real.py` & `qslib-1.8.2/tests/test_real.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_scpicommand.py` & `qslib-1.8.2/tests/test_scpicommand.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tests/test_util_fns.py` & `qslib-1.8.2/tests/test_util_fns.py`

 * *Files identical despite different names*

### Comparing `qslib-0.9.2/tox.ini` & `qslib-1.8.2/tox.ini`

 * *Files identical despite different names*

