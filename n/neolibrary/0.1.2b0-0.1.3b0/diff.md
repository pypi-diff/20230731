# Comparing `tmp/neolibrary-0.1.2b0.tar.gz` & `tmp/neolibrary-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neolibrary-0.1.2b0.tar", max compression
+gzip compressed data, was "neolibrary-0.1.3b0.tar", max compression
```

## Comparing `neolibrary-0.1.2b0.tar` & `neolibrary-0.1.3b0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/LICENSE
--rw-r--r--   0        0        0      437 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/README.md
--rw-r--r--   0        0        0      445 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/src/neolibrary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/src/neolibrary/monitoring/__init__.py
--rw-r--r--   0        0        0      770 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/src/neolibrary/monitoring/config/config.py
--rw-r--r--   0        0        0     3711 2023-07-31 10:22:20.588745 neolibrary-0.1.2b0/src/neolibrary/monitoring/logger.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 neolibrary-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/LICENSE
+-rw-r--r--   0        0        0      448 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/README.md
+-rw-r--r--   0        0        0      445 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/__init__.py
+-rw-r--r--   0        0        0      770 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/config/config.py
+-rw-r--r--   0        0        0     3711 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/monitoring/logger.py
+-rw-r--r--   0        0        0      714 2023-07-31 11:40:39.700573 neolibrary-0.1.3b0/src/neolibrary/utils.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 neolibrary-0.1.3b0/PKG-INFO
```

### Comparing `neolibrary-0.1.2b0/LICENSE` & `neolibrary-0.1.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.2b0/src/neolibrary/monitoring/config/config.py` & `neolibrary-0.1.3b0/src/neolibrary/monitoring/config/config.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.2b0/src/neolibrary/monitoring/logger.py` & `neolibrary-0.1.3b0/src/neolibrary/monitoring/logger.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.1.2b0/PKG-INFO` & `neolibrary-0.1.3b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neolibrary
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: The general utils library for neomedsys development
 License: Apache-2.0 license
 Author: Martin Soria Røvang
 Author-email: martinrovang@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,13 +13,13 @@
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Description-Content-Type: text/markdown
 
 # neolib
 
 
 ![Python 3.10](https://img.shields.io/badge/python-3.10.0-blue.svg)
-![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)[![Publish to PyPI](https://github.com/NeoMedSys/neolibrary/actions/workflows/pippackaging.yml/badge.svg?branch=main)](https://github.com/NeoMedSys/neolibrary/actions/workflows/pippackaging.yml)
+![PyPI status](https://img.shields.io/pypi/status/ansicolortags.svg)[![Publish to PyPI](https://github.com/NeoMedSys/neolibrary/actions/workflows/pippackaging.yml/badge.svg?branch=main&event=push)](https://github.com/NeoMedSys/neolibrary/actions/workflows/pippackaging.yml)
 
 
 The neolib is a library for the common functions that is used in the NeoMedSystem projects.
```

