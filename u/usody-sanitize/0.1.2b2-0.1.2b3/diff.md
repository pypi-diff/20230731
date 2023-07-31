# Comparing `tmp/usody_sanitize-0.1.2b2.tar.gz` & `tmp/usody_sanitize-0.1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usody_sanitize-0.1.2b2.tar", max compression
+gzip compressed data, was "usody_sanitize-0.1.2b3.tar", max compression
```

## Comparing `usody_sanitize-0.1.2b2.tar` & `usody_sanitize-0.1.2b3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      277 2023-07-31 03:49:31.258774 usody_sanitize-0.1.2b2/CHANGELOG.md
--rw-r--r--   0        0        0    18092 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/LICENSE
--rwxr-xr-x   0        0        0     1224 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/README.md
--rwxr-xr-x   0        0        0      778 2023-07-31 03:49:31.166772 usody_sanitize-0.1.2b2/pyproject.toml
--rwxr-xr-x   0        0        0       28 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/__init__.py
--rw-r--r--   0        0        0     3108 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/cmd_client.py
--rwxr-xr-x   0        0        0     4147 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b2/usody_sanitize/commands.py
--rwxr-xr-x   0        0        0     2859 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/erasure.py
--rw-r--r--   0        0        0     4049 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/methods.py
--rw-r--r--   0        0        0     9893 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/sanitize.py
--rw-r--r--   0        0        0      217 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/__init__.py
--rw-r--r--   0        0        0     1880 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/definition.py
--rw-r--r--   0        0        0      955 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/devices.py
--rw-r--r--   0        0        0     3905 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/export_data.py
--rw-r--r--   0        0        0     4186 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/schemas/sanitize.py
--rwxr-xr-x   0        0        0     6891 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/steps.py
--rw-r--r--   0        0        0     1522 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b2/usody_sanitize/utils.py
--rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 usody_sanitize-0.1.2b2/PKG-INFO
+-rw-r--r--   0        0        0      277 2023-07-31 03:55:30.384376 usody_sanitize-0.1.2b3/CHANGELOG.md
+-rw-r--r--   0        0        0    18092 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b3/LICENSE
+-rwxr-xr-x   0        0        0     1224 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b3/README.md
+-rwxr-xr-x   0        0        0      778 2023-07-31 03:55:30.304373 usody_sanitize-0.1.2b3/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b3/usody_sanitize/__init__.py
+-rw-r--r--   0        0        0     3108 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b3/usody_sanitize/cmd_client.py
+-rwxr-xr-x   0        0        0     4147 2023-07-31 02:49:51.881167 usody_sanitize-0.1.2b3/usody_sanitize/commands.py
+-rwxr-xr-x   0        0        0     2859 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/erasure.py
+-rw-r--r--   0        0        0     4049 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/methods.py
+-rw-r--r--   0        0        0     9893 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/sanitize.py
+-rw-r--r--   0        0        0      217 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/schemas/__init__.py
+-rw-r--r--   0        0        0     1880 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/schemas/definition.py
+-rw-r--r--   0        0        0      955 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/schemas/devices.py
+-rw-r--r--   0        0        0     3905 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/schemas/export_data.py
+-rw-r--r--   0        0        0     4186 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/schemas/sanitize.py
+-rwxr-xr-x   0        0        0     6891 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/steps.py
+-rw-r--r--   0        0        0     1522 2023-07-31 02:49:51.885167 usody_sanitize-0.1.2b3/usody_sanitize/utils.py
+-rw-r--r--   0        0        0     2234 1970-01-01 00:00:00.000000 usody_sanitize-0.1.2b3/PKG-INFO
```

### Comparing `usody_sanitize-0.1.2b2/LICENSE` & `usody_sanitize-0.1.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/README.md` & `usody_sanitize-0.1.2b3/README.md`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/pyproject.toml` & `usody_sanitize-0.1.2b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usody-sanitize"
-version = "0.1.2-beta2"
+version = "0.1.2-beta3"
 
 description = "A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process."
 repository = "https://github.com/usody/sanitize"
 authors = ["blkpws <me@blkpws.xyz>"]
 readme = ["CHANGELOG.md", "README.md"]
 license = "GNU"
```

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/cmd_client.py` & `usody_sanitize-0.1.2b3/usody_sanitize/cmd_client.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/commands.py` & `usody_sanitize-0.1.2b3/usody_sanitize/commands.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/erasure.py` & `usody_sanitize-0.1.2b3/usody_sanitize/erasure.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/methods.py` & `usody_sanitize-0.1.2b3/usody_sanitize/methods.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/sanitize.py` & `usody_sanitize-0.1.2b3/usody_sanitize/sanitize.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/schemas/definition.py` & `usody_sanitize-0.1.2b3/usody_sanitize/schemas/definition.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/schemas/devices.py` & `usody_sanitize-0.1.2b3/usody_sanitize/schemas/devices.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/schemas/export_data.py` & `usody_sanitize-0.1.2b3/usody_sanitize/schemas/export_data.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/schemas/sanitize.py` & `usody_sanitize-0.1.2b3/usody_sanitize/schemas/sanitize.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/steps.py` & `usody_sanitize-0.1.2b3/usody_sanitize/steps.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/usody_sanitize/utils.py` & `usody_sanitize-0.1.2b3/usody_sanitize/utils.py`

 * *Files identical despite different names*

### Comparing `usody_sanitize-0.1.2b2/PKG-INFO` & `usody_sanitize-0.1.2b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usody-sanitize
-Version: 0.1.2b2
+Version: 0.1.2b3
 Summary: A tool to securely erase/wipe data on disks HDD and SSD with a proper sanitization process.
 Home-page: https://github.com/usody/sanitize
 License: GNU
 Author: blkpws
 Author-email: me@blkpws.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

