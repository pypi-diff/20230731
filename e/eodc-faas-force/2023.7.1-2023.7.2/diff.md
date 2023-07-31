# Comparing `tmp/eodc_faas_force-2023.7.1.tar.gz` & `tmp/eodc_faas_force-2023.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_force-2023.7.1.tar", max compression
+gzip compressed data, was "eodc_faas_force-2023.7.2.tar", max compression
```

## Comparing `eodc_faas_force-2023.7.1.tar` & `eodc_faas_force-2023.7.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.7.1/README.md
--rw-r--r--   0        0        0       93 2023-07-26 09:23:23.152000 eodc_faas_force-2023.7.1/force_processor_bindings/__init__.py
--rw-r--r--   0        0        0     3352 2023-07-25 08:54:20.680000 eodc_faas_force-2023.7.1/force_processor_bindings/model.py
--rw-r--r--   0        0        0      610 2023-07-26 09:23:23.152000 eodc_faas_force-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 eodc_faas_force-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.7.2/README.md
+-rw-r--r--   0        0        0       93 2023-07-31 13:52:04.684000 eodc_faas_force-2023.7.2/force_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     3352 2023-07-25 08:54:20.680000 eodc_faas_force-2023.7.2/force_processor_bindings/model.py
+-rw-r--r--   0        0        0      610 2023-07-31 13:52:04.684000 eodc_faas_force-2023.7.2/pyproject.toml
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 eodc_faas_force-2023.7.2/PKG-INFO
```

### Comparing `eodc_faas_force-2023.7.1/force_processor_bindings/model.py` & `eodc_faas_force-2023.7.2/force_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_force-2023.7.1/pyproject.toml` & `eodc_faas_force-2023.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-force"
-version = "2023.7.1"
+version = "2023.7.2"
 description = "Bindings for the FORCE processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "force_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_force-2023.7.1/PKG-INFO` & `eodc_faas_force-2023.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-force
-Version: 2023.7.1
+Version: 2023.7.2
 Summary: Bindings for the FORCE processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

