# Comparing `tmp/usody_sanitize-0.1.1b1.tar.gz` & `tmp/usody_sanitize-0.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usody_sanitize-0.1.1b1.tar", max compression
+gzip compressed data, was "usody_sanitize-0.1.2b2.tar", max compression
```

## Comparing `usody_sanitize-0.1.1b1.tar` & `usody_sanitize-0.1.2b2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    18092 2023-02-19 02:19:59.000000 usody_sanitize-0.1.1b1/LICENSE
--rwxr-xr-x   0        0        0     1224 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/README.md
--rwxr-xr-x   0        0        0      744 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/pyproject.toml
--rwxr-xr-x   0        0        0       28 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/__init__.py
--rw-r--r--   0        0        0     3108 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/cmd_client.py
--rwxr-xr-x   0        0        0     4147 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/commands.py
--rwxr-xr-x   0        0        0     2859 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/erasure.py
--rw-r--r--   0        0        0     4049 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/methods.py
--rw-r--r--   0        0        0     9898 2023-07-22 06:24:49.998969 usody_sanitize-0.1.1b1/usody_sanitize/sanitize.py
--rw-r--r--   0        0        0      217 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/__init__.py
--rw-r--r--   0        0        0     1880 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/definition.py
--rw-r--r--   0        0        0      955 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/devices.py
--rw-r--r--   0        0        0     3905 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/export_data.py
--rw-r--r--   0        0        0     4186 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/schemas/sanitize.py
--rwxr-xr-x   0        0        0     6891 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/steps.py
--rw-r--r--   0        0        0     1522 2023-07-22 06:24:49.999969 usody_sanitize-0.1.1b1/usody_sanitize/utils.py
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 usody_sanitize-0.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0      277 2023-07-31 03:49:31.258774 usody_sanitize-0.1.2b2/CHANGELOG.md
+-rw-r--r--   0        0        0    18092 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/LICENSE
+-rwxr-xr-x   0        0        0     1224 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/README.md
+-rwxr-xr-x   0        0        0      778 2023-07-31 03:49:31.166772 usody_sanitize-0.1.2b2/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/__init__.py
+-rw-r--r--   0        0        0     3108 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/cmd_client.py
+-rwxr-xr-x   0        0        0     4147 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/commands.py
+-rwxr-xr-x   0        0        0     2859 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/erasure.py
+-rw-r--r--   0        0        0     4049 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/methods.py
+-rw-r--r--   0        0        0     9893 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/sanitize.py
+-rw-r--r--   0        0        0      217 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/definition.py
+-rw-r--r--   0        0        0      955 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/devices.py
+-rw-r--r--   0        0        0     3905 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/export_data.py
+-rw-r--r--   0        0        0     4186 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/sanitize.py
+-rwxr-xr-x   0        0        0     6891 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/steps.py
+-rw-r--r--   0        0        0     1522 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/utils.py
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 usody_sanitize-0.1.2b2/PKG-INFO
```

### Comparing `usody_sanitize-0.1.1b1/LICENSE` & `usody_sanitize-0.1.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/README.md` & `usody_sanitize-0.1.2b2/README.md`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/pyproject.toml` & `usody_sanitize-0.1.2b2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "usody-sanitize"
-version = "0.1.1-beta1"
+version = "0.1.2-beta2"
 
 description = "A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process."
 repository = "https://github.com/usody/sanitize"
 authors = ["blkpws <me@blkpws.xyz>"]
-readme = "README.md"
+readme = ["CHANGELOG.md", "README.md"]
+license = "GNU"
 
 [tool.poetry_bumpversion.file."usody_sanitize/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.2"
```

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/cmd_client.py` & `usody_sanitize-0.1.2b2/usody_sanitize/cmd_client.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/commands.py` & `usody_sanitize-0.1.2b2/usody_sanitize/commands.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/erasure.py` & `usody_sanitize-0.1.2b2/usody_sanitize/erasure.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/methods.py` & `usody_sanitize-0.1.2b2/usody_sanitize/methods.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/sanitize.py` & `usody_sanitize-0.1.2b2/usody_sanitize/sanitize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import logging
-import sys
 from pathlib import Path
 from typing import Union, Optional
 
 from usody_sanitize import schemas, steps, commands, utils
 from usody_sanitize.methods import (
     BASIC,
     CRYPTOGRAPHIC_ATA,  # SSD
@@ -153,15 +152,15 @@
     async def _pre_validation(self):
         """Check if the disk is not mounted and if it is not a
         read-only device.
 
         :return:
         """
         if self.blk.phy_sec != self.smart.logical_block_size:
-            sys.exit("Information missmatch, can not continue.")
+            logger.warning("Information missmatch, can not continue.")
 
         bs = self.smart.logical_block_size
         max_sector = self.smart.user_capacity.bytes // bs
         sectors = utils.get_spaced_numbers(max_sector, 10)
 
         def _successful_command(
                 _cmd: schemas.Exec,
```

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/schemas/definition.py` & `usody_sanitize-0.1.2b2/usody_sanitize/schemas/definition.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/schemas/devices.py` & `usody_sanitize-0.1.2b2/usody_sanitize/schemas/devices.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/schemas/export_data.py` & `usody_sanitize-0.1.2b2/usody_sanitize/schemas/export_data.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/schemas/sanitize.py` & `usody_sanitize-0.1.2b2/usody_sanitize/schemas/sanitize.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/steps.py` & `usody_sanitize-0.1.2b2/usody_sanitize/steps.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/usody_sanitize/utils.py` & `usody_sanitize-0.1.2b2/usody_sanitize/utils.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.1b1/PKG-INFO` & `usody_sanitize-0.1.2b2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,44 @@
 Metadata-Version: 2.1
 Name: usody-sanitize
-Version: 0.1.1b1
+Version: 0.1.2b2
 Summary: A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process.
 Home-page: https://github.com/usody/sanitize
+License: GNU
 Author: blkpws
 Author-email: me@blkpws.xyz
 Requires-Python: >=3.8,<4.0
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: Repository, https://github.com/usody/sanitize
 Description-Content-Type: text/markdown
 
+# Changelog
+
+## [unreleased]
+
+### Features
+
+- Info mismatch just shows a warning instead of exit
+- Auto build release packages
+- Builds on new debian 11 machine
+
+## [0.1.1-beta1] - 2023-07-22
+
+### Features
+
+- Confirm before erase
+- Newest changes with support for MNVe (PCIe)
+
+
 # Usody Sanitize
 
 > Under development.
 
 This tool securely erases disks by performing a certificate-based validation of
 the wipe process. It ensures that the data on the disk is completely and 
 irrecoverably erased, protecting sensitive information from being recovered.
```

