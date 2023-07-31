# Comparing `tmp/healdata_utils-0.1.4a0.tar.gz` & `tmp/healdata_utils-0.1.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "healdata_utils-0.1.4a0.tar", last modified: Fri Jul 21 13:43:11 2023, max compression
+gzip compressed data, was "healdata_utils-0.1.6a0.tar", last modified: Mon Jul 31 15:31:12 2023, max compression
```

## Comparing `healdata_utils-0.1.4a0.tar` & `healdata_utils-0.1.6a0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/types/typesets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/src/healdata_utils/validators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/frictionless.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/jsonschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/src/healdata_utils/validators/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.017076 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 13:43:11.000000 healdata_utils-0.1.4a0/src/healdata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 13:43:11.021076 healdata_utils-0.1.4a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-21 13:43:01.000000 healdata_utils-0.1.4a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.622150 healdata_utils-0.1.6a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-31 15:31:12.622150 healdata_utils-0.1.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:31:12.622150 healdata_utils-0.1.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.606150 healdata_utils-0.1.6a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.610150 healdata_utils-0.1.6a0/src/healdata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.614150 healdata_utils-0.1.6a0/src/healdata_utils/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/schemas/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155418 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/schemas/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.614150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.614150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvdata/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.614150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/frictionless/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/frictionless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/frictionless/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/readstat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/readstat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/readstat/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/types/typesets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.618150 healdata_utils-0.1.6a0/src/healdata_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/validators/frictionless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/validators/jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/src/healdata_utils/validators/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.614150 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 15:31:12.000000 healdata_utils-0.1.6a0/src/healdata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:31:12.622150 healdata_utils-0.1.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10039 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-31 15:31:00.000000 healdata_utils-0.1.6a0/tests/test_utils.py
```

### Comparing `healdata_utils-0.1.4a0/PKG-INFO` & `healdata_utils-0.1.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata_utils
-Version: 0.1.4a0
+Version: 0.1.6a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.1.4a0/README.md` & `healdata_utils-0.1.6a0/README.md`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/setup.py` & `healdata_utils-0.1.6a0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 os.chdir(Path(__file__).parent)
 def generate_long_description():
     return Path("README.md").read_text()
 
 def get_install_requirements():
     return '''petl==1.7.12
 jsonschema==4.17.3
-requests==2.28.2
+# requests==2.28.2
 PyYaml==6.0
 #frictionless==4.40.8
+pandas==1.4
 pyreadstat==1.2.0
 charset_normalizer==2.1
 visions== 0.7.5
 click==8.1.3'''
 
-
 setup(
     name='healdata_utils',
-    version='0.1.4-alpha',
+    version='0.1.6-alpha',
     author='Michael Kranz',
     author_email='kranz-michael@norc.org',
     long_description=generate_long_description(),
     long_description_content_type="text/markdown",    
     description='Data packaging tools for the HEAL data ecosystem',
     #TODO: change url to HEAL once migrated.
     url='https://github.com/norc-heal/healdata-utils',
```

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/cli.py` & `healdata_utils-0.1.6a0/src/healdata_utils/cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/io.py` & `healdata_utils-0.1.6a0/src/healdata_utils/io.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/schemas.py` & `healdata_utils-0.1.6a0/src/healdata_utils/schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvdata/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvdata/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/csvtemplate/mappings.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/csvtemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/frictionless/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/frictionless/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/jsontemplate/mappings.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/jsontemplate/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/readstat/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/readstat/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/conversion.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/conversion.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/headers.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/headers.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/mappings.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/mappings.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/transforms/redcapcsv/schema.py` & `healdata_utils-0.1.6a0/src/healdata_utils/transforms/redcapcsv/schema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/types/typesets.py` & `healdata_utils-0.1.6a0/src/healdata_utils/types/typesets.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,19 +94,25 @@
     df,typepaths,_ = typeset.infer(df) # typepaths is list of the visions graph traversal - last item is casted type
     fields = []
 
     for col,typepath in typepaths.items():
         field = {"name":col}
         type_final = str(typepath[-1])
         if type_final=="Categorical":
+            # TODO: see visions PR https://github.com/dylan-profiler/visions/issues/160 -- best way 
+            # would probably be to use networkx graph. seems like this may be a good feature to add
+            # to visions package
             type_second_to_final = str(typepath[-2])
             field["type"] = typeset_mapping.get(type_second_to_final,"any")
             # enums for inferred categoricals
             field["constraints"] = {"enum":list(df[col].cat.categories)}       
         else:
             field["type"] = typeset_mapping.get(str(type_final),"any")
 
+        
+        if field["type"]=="any":
+            print(field["name"])
         fields.append(field)
 
         
     
     return fields
```

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/utils.py` & `healdata_utils-0.1.6a0/src/healdata_utils/utils.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/validators/jsonschema.py` & `healdata_utils-0.1.6a0/src/healdata_utils/validators/jsonschema.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils/validators/validate.py` & `healdata_utils-0.1.6a0/src/healdata_utils/validators/validate.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils.egg-info/PKG-INFO` & `healdata_utils-0.1.6a0/src/healdata_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: healdata-utils
-Version: 0.1.4a0
+Version: 0.1.6a0
 Summary: Data packaging tools for the HEAL data ecosystem
 Home-page: https://github.com/norc-heal/healdata-utils
 Author: Michael Kranz
 Author-email: kranz-michael@norc.org
 Description-Content-Type: text/markdown
 
 --8<-- [start:intro]
```

### Comparing `healdata_utils-0.1.4a0/src/healdata_utils.egg-info/SOURCES.txt` & `healdata_utils-0.1.6a0/src/healdata_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 src/healdata_utils/utils.py
 src/healdata_utils.egg-info/PKG-INFO
 src/healdata_utils.egg-info/SOURCES.txt
 src/healdata_utils.egg-info/dependency_links.txt
 src/healdata_utils.egg-info/entry_points.txt
 src/healdata_utils.egg-info/requires.txt
 src/healdata_utils.egg-info/top_level.txt
+src/healdata_utils/schemas/__init__.py
+src/healdata_utils/schemas/frictionless.py
+src/healdata_utils/schemas/jsonschema.py
 src/healdata_utils/transforms/__init__.py
 src/healdata_utils/transforms/csvdata/conversion.py
 src/healdata_utils/transforms/csvtemplate/__init__.py
 src/healdata_utils/transforms/csvtemplate/conversion.py
 src/healdata_utils/transforms/csvtemplate/mappings.py
 src/healdata_utils/transforms/frictionless/__init__.py
 src/healdata_utils/transforms/frictionless/conversion.py
```

### Comparing `healdata_utils-0.1.4a0/tests/test_cli.py` & `healdata_utils-0.1.6a0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/tests/test_schemas.py` & `healdata_utils-0.1.6a0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `healdata_utils-0.1.4a0/tests/test_utils.py` & `healdata_utils-0.1.6a0/tests/test_utils.py`

 * *Files identical despite different names*

