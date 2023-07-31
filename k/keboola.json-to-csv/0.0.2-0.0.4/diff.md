# Comparing `tmp/keboola.json-to-csv-0.0.2.tar.gz` & `tmp/keboola.json-to-csv-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keboola.json-to-csv-0.0.2.tar", last modified: Thu Sep 22 08:19:52 2022, max compression
+gzip compressed data, was "keboola.json-to-csv-0.0.4.tar", last modified: Mon Jul 31 11:48:03 2023, max compression
```

## Comparing `keboola.json-to-csv-0.0.2.tar` & `keboola.json-to-csv-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5773 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9655 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/configuration/parser_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2747 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/data_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/exception/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/exception/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    12441 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/parse_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/value_object/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/value_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/value_object/column.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-09-22 08:19:33.000000 keboola.json-to-csv-0.0.2/src/keboola/json_to_csv/value_object/key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:19:52.432714 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6549 2022-09-22 08:19:52.000000 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-09-22 08:19:52.000000 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 08:19:52.000000 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 08:19:52.000000 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-09-22 08:19:52.000000 keboola.json-to-csv-0.0.2/src/keboola.json_to_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.413680 keboola.json-to-csv-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 11:48:03.413680 keboola.json-to-csv-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.405680 keboola.json-to-csv-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.405680 keboola.json-to-csv-0.0.4/src/keboola/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22470 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/csv_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15907 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/src/keboola/json_to_csv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 11:48:03.000000 keboola.json-to-csv-0.0.4/src/keboola.json_to_csv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 11:48:03.409680 keboola.json-to-csv-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-31 11:47:50.000000 keboola.json-to-csv-0.0.4/tests/test_functional.py
```

### Comparing `keboola.json-to-csv-0.0.2/LICENSE` & `keboola.json-to-csv-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `keboola.json-to-csv-0.0.2/setup.py` & `keboola.json-to-csv-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="keboola.json-to-csv",
-    version="0.0.2",
+    version="0.0.4",
     author="Keboola KDS Team",
     setup_requires=['flake8'],
     tests_require=[],
     install_requires=[],
     author_email="support@keboola.com",
     description="General utility library for Python applications running in Keboola Connection environment",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/keboola/python-utils",
-    packages=['keboola.json_to_csv', 'keboola.json_to_csv.configuration', 'keboola.json_to_csv.exception',
-              'keboola.json_to_csv.value_object'],
+    packages=['keboola.json_to_csv'],
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     test_suite='tests',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

