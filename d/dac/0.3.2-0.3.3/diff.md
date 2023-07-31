# Comparing `tmp/dac-0.3.2.tar.gz` & `tmp/dac-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dac-0.3.2.tar", last modified: Mon Jul 31 15:03:06 2023, max compression
+gzip compressed data, was "dac-0.3.3.tar", last modified: Mon Jul 31 15:19:56 2023, max compression
```

## Comparing `dac-0.3.2.tar` & `dac-0.3.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.887693 dac-0.3.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.891693 dac-0.3.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-31 15:02:42.000000 dac-0.3.2/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 15:02:42.000000 dac-0.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 15:02:42.000000 dac-0.3.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 15:02:42.000000 dac-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 15:02:42.000000 dac-0.3.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 15:02:42.000000 dac-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 15:03:06.899693 dac-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 15:02:42.000000 dac-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.891693 dac-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 15:02:42.000000 dac-0.3.2/docs/examples.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.891693 dac-0.3.2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-07-31 15:02:42.000000 dac-0.3.2/docs/img/logo.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-07-31 15:02:42.000000 dac-0.3.2/docs/img/motto.png
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-31 15:02:42.000000 dac-0.3.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 15:02:42.000000 dac-0.3.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-31 15:02:42.000000 dac-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 15:02:42.000000 dac-0.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 15:02:42.000000 dac-0.3.2/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 15:02:42.000000 dac-0.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:03:06.899693 dac-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.887693 dac-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.891693 dac-0.3.2/src/dac/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_file_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.895693 dac-0.3.2/src/dac/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/_config_pydantic_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/_config_pydantic_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/_pyproject_pydantic_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/_pyproject_pydantic_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_input/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-31 15:02:42.000000 dac-0.3.2/src/dac/_pyproject_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.895693 dac-0.3.2/src/dac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 15:03:06.000000 dac-0.3.2/src/dac.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.895693 dac-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-31 15:02:42.000000 dac-0.3.2/test/cli_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 15:02:42.000000 dac-0.3.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.895693 dac-0.3.2/test/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.895693 dac-0.3.2/test/data/load/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/missing_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/missing_load_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/missing_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/parquet_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/return_wrong_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/load/self_contained_as_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/pack_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/data/parquet/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/parquet/sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/data/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/requirements/parquet_as_pandas.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/data/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/schema/incompatible_with_sample_df.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/schema/invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/schema/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/schema/self_contained.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:02:42.000000 dac-0.3.2/test/data/schema/wrong_syntax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/integration_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/integration_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 15:02:42.000000 dac-0.3.2/test/integration_test/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/unit_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/unit_test/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_cli/help_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_cli/info_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_cli/pack_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/unit_test/_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_input/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_input/pyproject_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:03:06.899693 dac-0.3.2/test/unit_test/_packing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_packing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_packing/build_wheel_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_packing/data_as_code_project_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 15:02:42.000000 dac-0.3.2/test/unit_test/_packing/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.805431 dac-0.3.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.793431 dac-0.3.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.797431 dac-0.3.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-07-31 15:19:36.000000 dac-0.3.3/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-31 15:19:36.000000 dac-0.3.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 15:19:36.000000 dac-0.3.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-31 15:19:36.000000 dac-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 15:19:36.000000 dac-0.3.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 15:19:36.000000 dac-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 15:19:56.805431 dac-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-31 15:19:36.000000 dac-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.797431 dac-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 15:19:36.000000 dac-0.3.3/docs/examples.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.797431 dac-0.3.3/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   206100 2023-07-31 15:19:36.000000 dac-0.3.3/docs/img/logo.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    45811 2023-07-31 15:19:36.000000 dac-0.3.3/docs/img/motto.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-31 15:19:36.000000 dac-0.3.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 15:19:36.000000 dac-0.3.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-31 15:19:36.000000 dac-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 15:19:36.000000 dac-0.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 15:19:36.000000 dac-0.3.3/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 15:19:36.000000 dac-0.3.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:19:56.805431 dac-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.797431 dac-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.797431 dac-0.3.3/src/dac/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_file_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/src/dac/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/_config_pydantic_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/_config_pydantic_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/_pyproject_pydantic_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/_pyproject_pydantic_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_input/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-31 15:19:36.000000 dac-0.3.3/src/dac/_pyproject_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/src/dac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-31 15:19:56.000000 dac-0.3.3/src/dac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-31 15:19:36.000000 dac-0.3.3/test/cli_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-31 15:19:36.000000 dac-0.3.3/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/data/load/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/missing_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/missing_load_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/missing_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/parquet_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/return_wrong_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/load/self_contained_as_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/pack_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/data/parquet/
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/parquet/sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/data/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/requirements/parquet_as_pandas.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/data/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/schema/incompatible_with_sample_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/schema/invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/schema/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/schema/self_contained.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-31 15:19:36.000000 dac-0.3.3/test/data/schema/wrong_syntax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/integration_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/integration_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-07-31 15:19:36.000000 dac-0.3.3/test/integration_test/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/unit_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/unit_test/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_cli/help_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_cli/info_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_cli/pack_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.801431 dac-0.3.3/test/unit_test/_input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_input/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_input/pyproject_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:56.805431 dac-0.3.3/test/unit_test/_packing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_packing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_packing/build_wheel_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_packing/data_as_code_project_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 15:19:36.000000 dac-0.3.3/test/unit_test/_packing/pack_test.py
```

### Comparing `dac-0.3.2/.github/workflows/actions.yml` & `dac-0.3.3/.github/workflows/actions.yml`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/.gitlab-ci.yml` & `dac-0.3.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/.pre-commit-config.yaml` & `dac-0.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/CHANGELOG.md` & `dac-0.3.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 **IMPORTANT**: Currently the project is in the initial development phase, this is why releases are marked as `0.z.y`.
 (following [semantic versioning 2.0.0](https://semver.org/): "Major version zero (0.y.z) is for initial development.
 Anything MAY change at any time. The public API SHOULD NOT be considered stable.").
 While in this phase, we will denote breaking changes with a minor increase.
 
+## 0.3.3
+
+### Fixed
+
+* Cleanup
+
 ## 0.3.2
 
 ### Changed
 
 * Extend compatibility to pydantic v1. Now `dac` works with both v1 and v2 of pydantic
 
 ## 0.3.1
```

### Comparing `dac-0.3.2/LICENSE` & `dac-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/PKG-INFO` & `dac-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
```

### Comparing `dac-0.3.2/README.md` & `dac-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/docs/img/logo.jpg` & `dac-0.3.3/docs/img/logo.jpg`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/docs/img/motto.png` & `dac-0.3.3/docs/img/motto.png`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/docs/index.md` & `dac-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/mkdocs.yml` & `dac-0.3.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/pyproject.toml` & `dac-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_cli.py` & `dac-0.3.3/src/dac/_cli.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_input/_config_pydantic_v1.py` & `dac-0.3.3/src/dac/_input/_config_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_input/_config_pydantic_v2.py` & `dac-0.3.3/src/dac/_input/_config_pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_input/_pyproject_pydantic_v1.py` & `dac-0.3.3/src/dac/_input/_pyproject_pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_input/_pyproject_pydantic_v2.py` & `dac-0.3.3/src/dac/_input/_pyproject_pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_packing.py` & `dac-0.3.3/src/dac/_packing.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac/_pyproject_factory.py` & `dac-0.3.3/src/dac/_pyproject_factory.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/src/dac.egg-info/PKG-INFO` & `dac-0.3.3/src/dac.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dac
-Version: 0.3.2
+Version: 0.3.3
 Summary: Tool to distribute data as code
 Author-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 Maintainer-email: Francesco Calcavecchia <francesco.calcavecchia@gmail.com>
 License: MIT
 Project-URL: homepage, https://data-as-code.github.io/dac/
 Project-URL: documentation, https://data-as-code.github.io/dac/
 Project-URL: repository, https://github.com/data-as-code/dac
```

### Comparing `dac-0.3.2/src/dac.egg-info/SOURCES.txt` & `dac-0.3.3/src/dac.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/cli_utilities.py` & `dac-0.3.3/test/cli_utilities.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/conftest.py` & `dac-0.3.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/data/__init__.py` & `dac-0.3.3/test/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/data/pack_input.py` & `dac-0.3.3/test/data/pack_input.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/data/parquet/sample.parquet` & `dac-0.3.3/test/data/parquet/sample.parquet`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/integration_test/pack_test.py` & `dac-0.3.3/test/integration_test/pack_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_cli/pack_test.py` & `dac-0.3.3/test/unit_test/_cli/pack_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_input/config_test.py` & `dac-0.3.3/test/unit_test/_input/config_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_input/pyproject_test.py` & `dac-0.3.3/test/unit_test/_input/pyproject_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_packing/build_wheel_test.py` & `dac-0.3.3/test/unit_test/_packing/build_wheel_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_packing/data_as_code_project_test.py` & `dac-0.3.3/test/unit_test/_packing/data_as_code_project_test.py`

 * *Files identical despite different names*

### Comparing `dac-0.3.2/test/unit_test/_packing/pack_test.py` & `dac-0.3.3/test/unit_test/_packing/pack_test.py`

 * *Files identical despite different names*

