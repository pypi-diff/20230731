# Comparing `tmp/bomf-0.6.0.tar.gz` & `tmp/bomf-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.6.0.tar", last modified: Mon Jul  3 13:11:25 2023, max compression
+gzip compressed data, was "bomf-0.6.1.tar", last modified: Mon Jul 31 11:03:37 2023, max compression
```

## Comparing `bomf-0.6.0.tar` & `bomf-0.6.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-03 13:11:17.000000 bomf-0.6.0/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-03 13:11:17.000000 bomf-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-03 13:11:17.000000 bomf-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 13:11:17.000000 bomf-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-03 13:11:25.608066 bomf-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-03 13:11:17.000000 bomf-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-03 13:11:17.000000 bomf-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-03 13:11:17.000000 bomf-0.6.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-03 13:11:17.000000 bomf-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-03 13:11:25.608066 bomf-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 13:11:17.000000 bomf-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17580 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 13:11:17.000000 bomf-0.6.0/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.604066 bomf-0.6.0/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 13:11:25.000000 bomf-0.6.0/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-03 13:11:17.000000 bomf-0.6.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 13:11:25.608066 bomf-0.6.0/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_list_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21270 2023-07-03 13:11:17.000000 bomf-0.6.0/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.602330 bomf-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-31 11:03:30.000000 bomf-0.6.1/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-31 11:03:30.000000 bomf-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-31 11:03:30.000000 bomf-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 11:03:30.000000 bomf-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-31 11:03:37.602330 bomf-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-31 11:03:30.000000 bomf-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-31 11:03:30.000000 bomf-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 11:03:30.000000 bomf-0.6.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 11:03:30.000000 bomf-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-31 11:03:37.602330 bomf-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-31 11:03:30.000000 bomf-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.594330 bomf-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-31 11:03:30.000000 bomf-0.6.1/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.598330 bomf-0.6.1/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-31 11:03:37.000000 bomf-0.6.1/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-31 11:03:30.000000 bomf-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:03:37.602330 bomf-0.6.1/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-31 11:03:30.000000 bomf-0.6.1/unittests/test_validation.py
```

### Comparing `bomf-0.6.0/.github/dependabot.yml` & `bomf-0.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/black.yml` & `bomf-0.6.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/codeql-analysis.yml` & `bomf-0.6.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/coverage.yml` & `bomf-0.6.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/packaging_test.yml` & `bomf-0.6.1/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/python-publish.yml` & `bomf-0.6.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/pythonlint.yml` & `bomf-0.6.1/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.github/workflows/unittests.yml` & `bomf-0.6.1/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.gitignore` & `bomf-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/.pre-commit-config.yaml` & `bomf-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/LICENSE` & `bomf-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/PKG-INFO` & `bomf-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.0
+Version: 0.6.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.0/README.md` & `bomf-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/pyproject.toml` & `bomf-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/requirements.txt` & `bomf-0.6.1/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 #
 annotated-types==0.5.0
     # via pydantic
 attrs==23.1.0
     # via -r requirements.in
 bidict==0.22.1
     # via -r requirements.in
-bo4e==0.5.0
+bo4e==0.5.3
     # via -r requirements.in
 frozendict==2.3.8
     # via -r requirements.in
-injector==0.20.1
+injector==0.21.0
     # via -r requirements.in
 iso3166==2.1.1
     # via bo4e
 networkx==3.1
     # via -r requirements.in
-pydantic==2.0
+pydantic==2.1.1
     # via
     #   -r requirements.in
     #   bo4e
-pydantic-core==2.0.1
+pydantic-core==2.4.0
     # via pydantic
 pyhumps==3.8.0
     # via bo4e
-typeguard==2.13.3
+typeguard==4.0.1
     # via -r requirements.in
-typing-extensions==4.7.0
+typing-extensions==4.7.1
     # via
     #   pydantic
     #   pydantic-core
```

### Comparing `bomf-0.6.0/setup.cfg` & `bomf-0.6.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 zip_safe = False
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	attrs
 	bo4e
 	pydantic>=2.0.0
-	typeguard==2.13.3
+	typeguard>=4.0.1
 	frozendict
 	bidict
 	networkx
 	injector
 
 [options.packages.find]
 where = src
```

### Comparing `bomf-0.6.0/src/bomf/__init__.py` & `bomf-0.6.1/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/filter/__init__.py` & `bomf-0.6.1/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.6.1/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/loader/entityloader.py` & `bomf-0.6.1/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/logging/__init__.py` & `bomf-0.6.1/src/bomf/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/mapper/__init__.py` & `bomf-0.6.1/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/model/__init__.py` & `bomf-0.6.1/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/provider/__init__.py` & `bomf-0.6.1/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/core/analysis.py` & `bomf-0.6.1/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/core/errors.py` & `bomf-0.6.1/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/core/execution.py` & `bomf-0.6.1/src/bomf/validation/core/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from collections import defaultdict
 from dataclasses import dataclass
 from datetime import timedelta
 from enum import IntEnum, StrEnum
 from typing import Generic, Iterator, Optional
 
 import networkx as nx
-from typeguard import check_type
+from typeguard import TypeCheckError, check_type
 
 from bomf.logging import logger
 from bomf.validation.core.analysis import ValidationResult
 from bomf.validation.core.errors import ErrorHandler, ValidationError
 from bomf.validation.core.types import DataSetT, MappedValidatorSyncAsync, SyncValidatorFunction
 from bomf.validation.core.validator import MappedValidator, Parameters, is_async, is_sync
 
@@ -207,19 +207,18 @@
                 custom_error_id=_CustomErrorIDS.PARAM_PROVIDER_ERRORED,
             )
             return False
         try:
             self.info.current_provided_params = params_or_exc
             for param_name, param in params_or_exc.items():
                 check_type(
-                    param.param_id,
                     param.value,
                     mapped_validator.validator.signature.parameters[param_name].annotation,
                 )
-        except TypeError as error:
+        except TypeCheckError as error:
             await self.info.error_handler.catch(
                 str(error), error, mapped_validator, self, custom_error_id=_CustomErrorIDS.PARAM_TYPE_MISMATCH
             )
             return False
         return True
 
     async def _execute_async_validator(
```

### Comparing `bomf-0.6.0/src/bomf/validation/core/types.py` & `bomf-0.6.1/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/core/utils.py` & `bomf-0.6.1/src/bomf/validation/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     splitted_path = attribute_path.split(".")
     for index, attr_name in enumerate(splitted_path):
         try:
             current_obj = getattr(current_obj, attr_name)
         except AttributeError as error:
             current_path = ".".join(splitted_path[0 : index + 1])
             raise AttributeError(f"'{current_path}' does not exist") from error
-    check_type(attribute_path, current_obj, attribute_type)
+    check_type(current_obj, attribute_type)
     return current_obj
```

### Comparing `bomf-0.6.0/src/bomf/validation/core/validator.py` & `bomf-0.6.1/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/path_map.py` & `bomf-0.6.1/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/query_map.py` & `bomf-0.6.1/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf/validation/utils.py` & `bomf-0.6.1/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/src/bomf.egg-info/PKG-INFO` & `bomf-0.6.1/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.6.0
+Version: 0.6.1
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.6.0/src/bomf.egg-info/SOURCES.txt` & `bomf-0.6.1/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/tox.ini` & `bomf-0.6.1/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_bo4e_data_set.py` & `bomf-0.6.1/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_entity_loader.py` & `bomf-0.6.1/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_filter.py` & `bomf-0.6.1/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_list_conversion.py` & `bomf-0.6.1/unittests/test_list_conversion.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_mapper.py` & `bomf-0.6.1/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_migration.py` & `bomf-0.6.1/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_source_data_provider.py` & `bomf-0.6.1/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.6.0/unittests/test_validation.py` & `bomf-0.6.1/unittests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 
     @pytest.mark.parametrize(
         ["validator", "param_map", "expected_error"],
         [
             pytest.param(
                 validator_type_check_fail_y,
                 {"x": "x", "y": "y"},
-                "type of y must be str; got int instead",
+                "int is not an instance of str",
                 id="Wrong parameter type",
             ),
         ],
     )
     async def test_type_error(
         self, validator: Validator[DataSetTest, ValidatorFunctionT], param_map: dict[str, str], expected_error: str
     ):
```

