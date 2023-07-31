# Comparing `tmp/barcodes_uc-0.6.0.tar.gz` & `tmp/barcodes_uc-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barcodes_uc-0.6.0.tar", max compression
+gzip compressed data, was "barcodes_uc-0.6.1.tar", max compression
```

## Comparing `barcodes_uc-0.6.0.tar` & `barcodes_uc-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       81 2023-07-27 08:53:47.149695 barcodes_uc-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.6.0/barcodes_uc/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.6.0/barcodes_uc/barcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.6.0/barcodes_uc/barcodes/__main__.py
--rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.6.0/barcodes_uc/qrcodes/__init__.py
--rw-r--r--   0        0        0        0 2023-07-12 09:46:23.049740 barcodes_uc-0.6.0/barcodes_uc/qrcodes/__main__.py
--rw-r--r--   0        0        0    13170 2023-07-30 17:06:37.851607 barcodes_uc-0.6.0/barcodes_uc/qrcodes/qrgenerator.py
--rw-r--r--   0        0        0    40363 2023-07-30 07:58:05.620515 barcodes_uc-0.6.0/barcodes_uc/qrcodes/qrutils.py
--rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.6.0/data/GF256.csv
--rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.6.0/data/alignment_locations.csv
--rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.6.0/data/capabilities.csv
--rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.6.0/data/error_correction_table.csv
--rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.6.0/data/format_table.csv
--rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.6.0/data/version_table.csv
--rw-r--r--   0        0        0      470 2023-07-31 06:14:57.938735 barcodes_uc-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10174 2023-07-30 21:54:01.391050 barcodes_uc-0.6.0/requirements.txt
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 barcodes_uc-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-07-27 08:53:47.149695 barcodes_uc-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 21:52:22.989605 barcodes_uc-0.6.1/barcodes_uc/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:12.077870 barcodes_uc-0.6.1/barcodes_uc/barcodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:46:15.448895 barcodes_uc-0.6.1/barcodes_uc/barcodes/__main__.py
+-rw-r--r--   0        0        0        0 2023-07-09 21:53:18.670296 barcodes_uc-0.6.1/barcodes_uc/qrcodes/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-12 09:46:23.049740 barcodes_uc-0.6.1/barcodes_uc/qrcodes/__main__.py
+-rw-r--r--   0        0        0    13170 2023-07-30 17:06:37.851607 barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrgenerator.py
+-rw-r--r--   0        0        0    40363 2023-07-30 07:58:05.620515 barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrutils.py
+-rw-r--r--   0        0        0     1843 2023-07-14 14:45:54.180606 barcodes_uc-0.6.1/data/GF256.csv
+-rw-r--r--   0        0        0      664 2023-07-18 09:25:40.467529 barcodes_uc-0.6.1/data/alignment_locations.csv
+-rw-r--r--   0        0        0    10948 2023-07-14 13:23:50.352025 barcodes_uc-0.6.1/data/capabilities.csv
+-rw-r--r--   0        0        0     3824 2023-07-14 14:37:48.262264 barcodes_uc-0.6.1/data/error_correction_table.csv
+-rw-r--r--   0        0        0      766 2023-07-26 21:12:31.179696 barcodes_uc-0.6.1/data/format_table.csv
+-rw-r--r--   0        0        0      780 2023-07-26 08:54:25.882026 barcodes_uc-0.6.1/data/version_table.csv
+-rw-r--r--   0        0        0      442 2023-07-31 21:52:02.948955 barcodes_uc-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    10174 2023-07-30 21:54:01.391050 barcodes_uc-0.6.1/requirements.txt
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 barcodes_uc-0.6.1/PKG-INFO
```

### Comparing `barcodes_uc-0.6.0/barcodes_uc/qrcodes/qrgenerator.py` & `barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrgenerator.py`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/barcodes_uc/qrcodes/qrutils.py` & `barcodes_uc-0.6.1/barcodes_uc/qrcodes/qrutils.py`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/GF256.csv` & `barcodes_uc-0.6.1/data/GF256.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/alignment_locations.csv` & `barcodes_uc-0.6.1/data/alignment_locations.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/capabilities.csv` & `barcodes_uc-0.6.1/data/capabilities.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/error_correction_table.csv` & `barcodes_uc-0.6.1/data/error_correction_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/format_table.csv` & `barcodes_uc-0.6.1/data/format_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/data/version_table.csv` & `barcodes_uc-0.6.1/data/version_table.csv`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/requirements.txt` & `barcodes_uc-0.6.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `barcodes_uc-0.6.0/PKG-INFO` & `barcodes_uc-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barcodes-uc
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library to generate barcodes
 Author: Pedro Juan Royo
 Author-email: pedro.juan.royo@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

