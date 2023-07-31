# Comparing `tmp/dac-0.3.0.tar.gz` & `tmp/dac-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dac-0.3.0.tar", last modified: Wed Apr 12 12:22:14 2023, max compression
+gzip compressed data, was "dac-0.3.1.tar", last modified: Mon Jul 31 13:44:40 2023, max compression
```

## Comparing `dac-0.3.0.tar` & `dac-0.3.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.780995 dac-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.756995 dac-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-12 12:21:44.000000 dac-0.3.0/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-12 12:21:44.000000 dac-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-12 12:21:44.000000 dac-0.3.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-12 12:21:44.000000 dac-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-12 12:21:44.000000 dac-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-12 12:21:44.000000 dac-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 12:22:14.776996 dac-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-12 12:21:44.000000 dac-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-12 12:21:44.000000 dac-0.3.0/docs/examples.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-04-12 12:21:44.000000 dac-0.3.0/docs/img/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-04-12 12:21:44.000000 dac-0.3.0/docs/img/motto.png
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-04-12 12:21:44.000000 dac-0.3.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-12 12:21:44.000000 dac-0.3.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-12 12:21:44.000000 dac-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-12 12:21:44.000000 dac-0.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 12:22:14.780995 dac-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.756995 dac-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.764995 dac-0.3.0/src/dac/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_file_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/src/dac/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_input/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-12 12:21:44.000000 dac-0.3.0/src/dac/_pyproject_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/src/dac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-12 12:22:14.000000 dac-0.3.0/src/dac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.768995 dac-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-12 12:21:44.000000 dac-0.3.0/test/cli_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-12 12:21:44.000000 dac-0.3.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_load_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/missing_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/parquet_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/return_wrong_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/load/self_contained_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/pack_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/parquet/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/parquet/sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.772996 dac-0.3.0/test/data/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/requirements/parquet_as_pandas.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/data/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/incompatible_with_sample_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/self_contained.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-12 12:21:44.000000 dac-0.3.0/test/data/schema/wrong_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/integration_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-12 12:21:44.000000 dac-0.3.0/test/integration_test/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/help_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_cli/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_input/pyproject_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 12:22:14.776996 dac-0.3.0/test/unit_test/_packing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/build_wheel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/data_as_code_project_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-12 12:21:44.000000 dac-0.3.0/test/unit_test/_packing/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.461265 dac-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.453265 dac-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.453265 dac-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-31 13:44:19.000000 dac-0.3.1/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 13:44:19.000000 dac-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 13:44:19.000000 dac-0.3.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 13:44:19.000000 dac-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-31 13:44:19.000000 dac-0.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 13:44:19.000000 dac-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 13:44:40.461265 dac-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 13:44:19.000000 dac-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.453265 dac-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 13:44:19.000000 dac-0.3.1/docs/examples.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.453265 dac-0.3.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-07-31 13:44:19.000000 dac-0.3.1/docs/img/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-07-31 13:44:19.000000 dac-0.3.1/docs/img/motto.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-31 13:44:19.000000 dac-0.3.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 13:44:19.000000 dac-0.3.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-31 13:44:19.000000 dac-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 13:44:19.000000 dac-0.3.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 13:44:19.000000 dac-0.3.1/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 13:44:19.000000 dac-0.3.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:44:40.461265 dac-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.453265 dac-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/src/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_file_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/src/dac/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_input/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_input/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-31 13:44:19.000000 dac-0.3.1/src/dac/_pyproject_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/src/dac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 13:44:40.000000 dac-0.3.1/src/dac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-31 13:44:19.000000 dac-0.3.1/test/cli_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 13:44:19.000000 dac-0.3.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/data/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/missing_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/missing_load_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/missing_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/parquet_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/return_wrong_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/load/self_contained_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/pack_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/data/parquet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/parquet/sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/data/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/requirements/parquet_as_pandas.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/schema/incompatible_with_sample_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/schema/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/schema/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/schema/self_contained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 13:44:19.000000 dac-0.3.1/test/data/schema/wrong_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/integration_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 13:44:19.000000 dac-0.3.1/test/integration_test/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.457265 dac-0.3.1/test/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.461265 dac-0.3.1/test/unit_test/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_cli/help_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_cli/info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_cli/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.461265 dac-0.3.1/test/unit_test/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_input/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_input/pyproject_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:40.461265 dac-0.3.1/test/unit_test/_packing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_packing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_packing/build_wheel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_packing/data_as_code_project_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 13:44:19.000000 dac-0.3.1/test/unit_test/_packing/pack_test.py
```

### Comparing `dac-0.3.0/.github/workflows/actions.yml` & `dac-0.3.1/.github/workflows/actions.yml`

 * *Files 5% similar despite different names*

```diff
@@ -59,24 +59,22 @@
         pytest test --run-slow
 
   docs:
     needs: [test, check-style]
     if: ${{ github.ref == 'refs/heads/main' }}
     runs-on: ubuntu-latest
     steps:
-      - name: Checkout 🔖
-        uses: actions/checkout@v3
-      - name: Setup python 🐍
-        uses: actions/setup-python@v4
-        with:
-          python-version: "3.11"
-      - name: Build and push docs 📔🚀
-        run: |
-          pip install -r requirements-docs.txt
-          mkdocs gh-deploy --force
+    - name: Checkout 🔖
+      uses: actions/checkout@v3
+    - name: Deploy docs
+      uses: mhausenblas/mkdocs-deploy-gh-pages@master
+      env:
+        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        CONFIG_FILE: mkdocs.yml
+        REQUIREMENTS: requirements-docs.txt
 
   pypi-release:
     needs: [test, check-style]
     if: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags/v') }}
     runs-on: ubuntu-latest
     steps:
     - name: Checkout 🔖
```

### Comparing `dac-0.3.0/.gitlab-ci.yml` & `dac-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/.pre-commit-config.yaml` & `dac-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/CHANGELOG.md` & `dac-0.3.1/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 # Changelog
+
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
+## 0.3.1
+
+### Changed
+
+* Update code to be compatible with pydantic v2 (no retro-compatibility with v1)
 
 ## 0.3.0
+
 ### Changed
+
 * Dependencies passed in CLI `--pkg-dependencies` or `PyProjectConfig` must be separated by `;` or newline (previously was `,` or newline)
 
 ## 0.2.0
+
 ### Added
+
 * First release of `dac`
```

### Comparing `dac-0.3.0/LICENSE` & `dac-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/PKG-INFO` & `dac-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
@@ -33,35 +33,38 @@
 </div>
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
-
 ## 📔 [User documentation](https://data-as-code.github.io/dac/)
 
-
 ## Setup development environment (for contributors only)
 
 * Create a virtual environment and activate it
+
   ```shell
   python -m venv venv
   . venv/bin/activate
   ```
 
 * Install the developer dependencies
+
   ```shell
   python -m pip install -U pip wheel setuptools
   python -m pip install -r requirements-dev.txt
   ```
 
 * Enable the pre-commits
+
   ```shell
   pre-commit install
   ```
 
 * To run all the tests
+
   ```shell
   pytest --run-slow
   ```
+
   (omit `--run-slow` to run only the fast unit tests)
```

### Comparing `dac-0.3.0/README.md` & `dac-0.3.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -11,35 +11,38 @@
 </div>
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
-
 ## 📔 [User documentation](https://data-as-code.github.io/dac/)
 
-
 ## Setup development environment (for contributors only)
 
 * Create a virtual environment and activate it
+
   ```shell
   python -m venv venv
   . venv/bin/activate
   ```
 
 * Install the developer dependencies
+
   ```shell
   python -m pip install -U pip wheel setuptools
   python -m pip install -r requirements-dev.txt
   ```
 
 * Enable the pre-commits
+
   ```shell
   pre-commit install
   ```
 
 * To run all the tests
+
   ```shell
   pytest --run-slow
   ```
+
   (omit `--run-slow` to run only the fast unit tests)
```

### Comparing `dac-0.3.0/docs/img/logo.jpg` & `dac-0.3.1/docs/img/logo.jpg`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/docs/img/motto.png` & `dac-0.3.1/docs/img/motto.png`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/docs/index.md` & `dac-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/mkdocs.yml` & `dac-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/pyproject.toml` & `dac-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "License :: OSI Approved :: MIT License",
   "Topic :: Scientific/Engineering",
   "Operating System :: OS Independent"
 ]
 
 dependencies = [
   "build~=0.9",
-  "pydantic~=1.10",
+  "pydantic~=2.1",
   "toml~=0.10",
   "typer[all]~=0.7",
   "wheel~=0.38"
 ]
 
 # [project.optional-dependencies]
 #
```

### Comparing `dac-0.3.0/src/dac/_cli.py` & `dac-0.3.1/src/dac/_cli.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/src/dac/_input/config.py` & `dac-0.3.1/src/dac/_input/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import importlib
 import inspect
 import sys
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 
 import pandera as pa
-from pydantic import BaseModel, root_validator, validator
+from pydantic import BaseModel, field_validator, model_validator
 
 from dac._file_helper import temporarily_copied_file
 from dac._input.pyproject import PyProjectConfig
 
 
 class PackConfig(BaseModel):
     data_path: Optional[Path] = None
     load_path: Path
     schema_path: Path
     wheel_dir: Path
     pyproject: PyProjectConfig
 
-    @validator("data_path", "load_path", "schema_path", "wheel_dir")
+    @field_validator("data_path", "load_path", "schema_path", "wheel_dir")
+    @classmethod
     def path_exists(cls, path: Path) -> Path:  # pylint: disable=no-self-argument,no-self-use
         if path is not None and not path.exists():
             raise ValueError((f"Path {path.as_posix()} is not valid"))
         return path
 
-    @validator("load_path")
+    @field_validator("load_path")
+    @classmethod
     def load_contains_expected_function(cls, path: Path) -> Path:  # pylint: disable=no-self-argument,no-self-use
         try:
             sys.path.append(path.parent.as_posix())
             pkg = importlib.import_module(name=path.stem)
         except Exception as e:
             raise ValueError(
                 (
@@ -42,15 +44,16 @@
         try:
             signature = inspect.getfullargspec(pkg.load)
             assert signature.args == []
         except Exception as e:
             raise ValueError((f"{path.as_posix()} does not contain the required `def load()`")) from e
         return path
 
-    @validator("schema_path")
+    @field_validator("schema_path")
+    @classmethod
     def schema_contains_expected_class(cls, path: Path) -> Path:  # pylint: disable=no-self-argument,no-self-use
         try:
             sys.path.append(path.parent.as_posix())
             pkg = importlib.import_module(name=path.stem)
         except Exception as e:
             raise ValueError(
                 (
@@ -63,48 +66,44 @@
 
         try:
             issubclass(pkg.Schema, pa.SchemaModel)
         except Exception as e:
             raise ValueError((f"{path.as_posix()} does not contain the required `class Schema(pa.SchemaModel)`")) from e
         return path
 
-    @root_validator
-    def schema_match_data(  # pylint: disable=no-self-argument,no-self-use
-        cls, values: Dict[str, Path]
-    ) -> Dict[str, Path]:
+    @model_validator(mode="after")
+    def schema_match_data(self) -> "PackConfig":
         try:
-            sys.path.append(values["load_path"].parent.as_posix())
-            load_module = importlib.import_module(name=values["load_path"].stem)
+            sys.path.append(self.load_path.parent.as_posix())
+            load_module = importlib.import_module(name=self.load_path.stem)
         except Exception as e:
             raise ValueError(
                 "Validation of the schema against the data has failed because the load module could not be imported"
             ) from e
 
         try:
-            if values.get("data_path", None) is not None:
-                with temporarily_copied_file(
-                    src=values["data_path"], dst=values["load_path"].parent / values["data_path"].name
-                ):
+            if self.data_path is not None:
+                with temporarily_copied_file(src=self.data_path, dst=self.load_path.parent / self.data_path.name):
                     data = load_module.load()
             else:
                 data = load_module.load()
         except Exception as e:
             raise ValueError("`load()` failed due to the following error:" "\n" f"{e}") from e
 
         try:
-            sys.path.append(values["schema_path"].parent.as_posix())
-            schema_module = importlib.import_module(name=values["schema_path"].stem)
+            sys.path.append(self.schema_path.parent.as_posix())
+            schema_module = importlib.import_module(name=self.schema_path.stem)
         except Exception as e:
             raise ValueError(
                 "Validation of the schema against the data has failed because the schema module could not be imported"
             ) from e
 
         try:
             schema_module.Schema.validate(data, lazy=True)
         except pa.errors.SchemaErrors as e:
             raise ValueError("Validation of the schema against the data has failed:" "\n" f"{e.failure_cases}") from e
         except Exception as e:
             raise ValueError(
                 "Validation of the schema against the data has failed for unexpected reasons:" "\n" f"{e}"
             ) from e
 
-        return values
+        return self
```

### Comparing `dac-0.3.0/src/dac/_input/pyproject.py` & `dac-0.3.1/src/dac/_input/pyproject.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import List
 
 import toml  # type: ignore
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, field_validator
 
 
 class PyProjectConfig(BaseModel):
     project_name: str
     project_version: str
     project_dependencies: str
 
-    @validator("project_name")
+    @field_validator("project_name")
+    @classmethod
     def valid_project_name(cls, name: str) -> str:  # pylint: disable=no-self-argument,no-self-use
         if not name.isidentifier() or "\xb7" in name:
             raise ValueError(f"Invalid project name: {name} (hint: only '_' are allowed, no '-')")
         return name
 
     def generate_pyproject_toml(self) -> str:
         return toml.dumps(
```

### Comparing `dac-0.3.0/src/dac/_packing.py` & `dac-0.3.1/src/dac/_packing.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/src/dac/_pyproject_factory.py` & `dac-0.3.1/src/dac/_pyproject_factory.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/src/dac.egg-info/PKG-INFO` & `dac-0.3.1/src/dac.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
@@ -33,35 +33,38 @@
 </div>
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
-
 ## 📔 [User documentation](https://data-as-code.github.io/dac/)
 
-
 ## Setup development environment (for contributors only)
 
 * Create a virtual environment and activate it
+
   ```shell
   python -m venv venv
   . venv/bin/activate
   ```
 
 * Install the developer dependencies
+
   ```shell
   python -m pip install -U pip wheel setuptools
   python -m pip install -r requirements-dev.txt
   ```
 
 * Enable the pre-commits
+
   ```shell
   pre-commit install
   ```
 
 * To run all the tests
+
   ```shell
   pytest --run-slow
   ```
+
   (omit `--run-slow` to run only the fast unit tests)
```

### Comparing `dac-0.3.0/src/dac.egg-info/SOURCES.txt` & `dac-0.3.1/src/dac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/cli_utilities.py` & `dac-0.3.1/test/cli_utilities.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/conftest.py` & `dac-0.3.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/data/__init__.py` & `dac-0.3.1/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/data/pack_input.py` & `dac-0.3.1/test/data/pack_input.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/data/parquet/sample.parquet` & `dac-0.3.1/test/data/parquet/sample.parquet`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/integration_test/pack_test.py` & `dac-0.3.1/test/integration_test/pack_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/unit_test/_cli/pack_test.py` & `dac-0.3.1/test/unit_test/_cli/pack_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     get_path_to_wrong_syntax_schema,
 )
 from test.data.pack_input import input_with_local_data, input_with_self_contained_data
 from unittest.mock import MagicMock, patch
 
 import pytest
 from click.testing import Result
-
 from dac._input.config import PackConfig
 
 
 @pytest.fixture(autouse=True)
 def fixture_ensure_pack_signautre():
     pack_signature = signature(import_module("dac._cli").py_api_pack)
     assert len(pack_signature.parameters) == 1
@@ -56,19 +55,20 @@
 def test_if_load_requires_missing_requirement_then_error_contains_meaningful_info():
     result = invoke_dac_pack(load=get_path_to_missing_requirement_load().as_posix())
     assert result.exit_code != 0
     error_message = str(result.exception)
     assert "No module named 'modin'" in error_message
 
 
-def test_if_load_returns_wrong_type_then_error_contains_meningful_info():
+def test_if_load_returns_wrong_type_then_error_contains_meaningful_info():
     result = invoke_dac_pack(load=get_path_to_return_wrong_type_load().as_posix())
     assert result.exit_code != 0
     error_message = str(result.exception)
-    assert "expected pd.DataFrame, got <class 'NoneType'>" in error_message
+    assert "Backend not found for backend" in error_message
+    assert "pandas" in error_message
 
 
 def test_if_load_miss_credentials_then_error_contains_meaningful_info():
     result = invoke_dac_pack(load=get_path_to_sample_load_failing_because_of_missing_credentials().as_posix())
     assert result.exit_code != 0
     error_message = str(result.exception)
     assert "Missing credentials" in error_message
```

### Comparing `dac-0.3.0/test/unit_test/_input/config_test.py` & `dac-0.3.1/test/unit_test/_input/config_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/unit_test/_input/pyproject_test.py` & `dac-0.3.1/test/unit_test/_input/pyproject_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/unit_test/_packing/build_wheel_test.py` & `dac-0.3.1/test/unit_test/_packing/build_wheel_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/unit_test/_packing/data_as_code_project_test.py` & `dac-0.3.1/test/unit_test/_packing/data_as_code_project_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.0/test/unit_test/_packing/pack_test.py` & `dac-0.3.1/test/unit_test/_packing/pack_test.py`

 * *Files identical despite different names*

