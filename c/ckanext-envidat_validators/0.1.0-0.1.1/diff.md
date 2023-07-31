# Comparing `tmp/ckanext-envidat-validators-0.1.0.tar.gz` & `tmp/ckanext-envidat-validators-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-envidat-validators-0.1.0.tar", last modified: Mon Jul 31 14:16:16 2023, max compression
+gzip compressed data, was "ckanext-envidat-validators-0.1.1.tar", last modified: Mon Jul 31 15:59:47 2023, max compression
```

## Comparing `ckanext-envidat-validators-0.1.0.tar` & `ckanext-envidat-validators-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      134 2023-07-31 14:15:57.795673 ckanext-envidat-validators-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1060 2023-07-31 14:15:57.795673 ckanext-envidat-validators-0.1.0/LICENSE
--rw-r--r--   0        0        0     1015 2023-07-31 14:15:57.795673 ckanext-envidat-validators-0.1.0/README.md
--rw-r--r--   0        0        0      230 2023-07-31 14:15:57.795673 ckanext-envidat-validators-0.1.0/ckanext/__init__.py
--rw-r--r--   0        0        0      237 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/__init__.py
--rw-r--r--   0        0        0       43 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/__version__.py
--rw-r--r--   0        0        0     9943 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/logic.py
--rw-r--r--   0        0        0     1118 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/plugin.py
--rw-r--r--   0        0        0       51 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/tests/__init__.py
--rw-r--r--   0        0        0     1436 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/tests/test_plugin.py
--rw-r--r--   0        0        0     2137 2023-07-31 14:15:57.799672 ckanext-envidat-validators-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 ckanext-envidat-validators-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2023-07-31 15:59:28.690921 ckanext-envidat-validators-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1060 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1015 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/README.md
+-rw-r--r--   0        0        0      230 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/ckanext/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/__init__.py
+-rw-r--r--   0        0        0       43 2023-07-31 15:59:28.690921 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/__version__.py
+-rw-r--r--   0        0        0     9943 2023-07-31 15:59:28.690921 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/logic.py
+-rw-r--r--   0        0        0     1316 2023-07-31 15:59:28.690921 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/plugin.py
+-rw-r--r--   0        0        0       51 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/tests/__init__.py
+-rw-r--r--   0        0        0     1436 2023-07-31 13:42:19.217905 ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/tests/test_plugin.py
+-rw-r--r--   0        0        0     2137 2023-07-31 15:59:28.690921 ckanext-envidat-validators-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1846 1970-01-01 00:00:00.000000 ckanext-envidat-validators-0.1.1/PKG-INFO
```

### Comparing `ckanext-envidat-validators-0.1.0/LICENSE` & `ckanext-envidat-validators-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.1.0/README.md` & `ckanext-envidat-validators-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/logic.py` & `ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/logic.py`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.1.0/ckanext/envidat_validators/tests/test_plugin.py` & `ckanext-envidat-validators-0.1.1/ckanext/envidat_validators/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-envidat-validators-0.1.0/pyproject.toml` & `ckanext-envidat-validators-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points."ckan.plugins"]
 envidat_validators = "ckanext.envidat_validators.plugin:EnviDatValidatorsPlugin"
 
@@ -58,15 +58,15 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest-ckan>=0.0.12",
 ]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.1.0"
+version = "0.1.1"
 version_files = [
     "pyproject.toml:version",
     "ckanext/envidat_validators/__version__.py",
 ]
 
 [tool.isort]
 profile = "black"
```

### Comparing `ckanext-envidat-validators-0.1.0/PKG-INFO` & `ckanext-envidat-validators-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-envidat_validators
-Version: 0.1.0
+Version: 0.1.1
 Summary: Custom CKAN validators for EnviDat.
 License: MIT
 Keywords: CKAN,validators,schema
 Author-email: Sam Woodcock <sam.woodcock@protonmail.com>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ckanext-envidat_validators Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: ckanext-envidat_validators Version: 0.1.1 Summary:
 Custom CKAN validators for EnviDat. License: MIT Keywords:
 CKAN,validators,schema Author-email: Sam Woodcock
 woodcock@protonmail.com> Requires-Python: >=3.8 Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

