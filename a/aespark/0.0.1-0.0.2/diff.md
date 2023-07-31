# Comparing `tmp/aespark-0.0.1.tar.gz` & `tmp/aespark-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespark-0.0.1.tar", last modified: Mon Jul 31 13:30:38 2023, max compression
+gzip compressed data, was "aespark-0.0.2.tar", last modified: Mon Jul 31 14:03:12 2023, max compression
```

## Comparing `aespark-0.0.1.tar` & `aespark-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 13:30:38.149294 aespark-0.0.1/
--rw-rw-rw-   0        0        0       97 2023-07-31 13:27:02.000000 aespark-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-07-31 13:30:38.149294 aespark-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 13:30:37.977436 aespark-0.0.1/aespark/
--rw-rw-rw-   0        0        0        0 2023-07-31 13:20:07.000000 aespark-0.0.1/aespark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:30:38.008678 aespark-0.0.1/aespark/aespark/
--rw-rw-rw-   0        0        0        0 2023-07-31 13:20:07.000000 aespark-0.0.1/aespark/aespark/__init__.py
--rw-rw-rw-   0        0        0    16080 2023-07-31 13:14:43.000000 aespark-0.0.1/aespark/aespark/aespark.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:30:38.149294 aespark-0.0.1/aespark/aespark/static/
--rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.1/aespark/aespark/static/ip.txt
--rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.1/aespark/aespark/static/材料模板.docx
-drwxrwxrwx   0        0        0        0 2023-07-31 13:30:37.993054 aespark-0.0.1/aespark.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 13:30:37.000000 aespark-0.0.1/aespark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 13:30:38.149294 aespark-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      982 2023-07-31 13:27:38.000000 aespark-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:12.572008 aespark-0.0.2/
+-rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2023-07-31 14:03:12.572008 aespark-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:12.446714 aespark-0.0.2/aespark/
+-rw-rw-rw-   0        0        0      702 2023-07-31 13:59:30.000000 aespark-0.0.2/aespark/__init__.py
+-rw-rw-rw-   0        0        0    16080 2023-07-31 13:14:43.000000 aespark-0.0.2/aespark/aespark.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:12.572008 aespark-0.0.2/aespark/static/
+-rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.2/aespark/static/ip.txt
+-rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.2/aespark/static/材料模板.docx
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:12.462338 aespark-0.0.2/aespark.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      325 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 14:03:12.000000 aespark-0.0.2/aespark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:03:12.572008 aespark-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-07-31 14:02:49.000000 aespark-0.0.2/setup.py
```

### Comparing `aespark-0.0.1/PKG-INFO` & `aespark-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `aespark-0.0.1/aespark/aespark/aespark.py` & `aespark-0.0.2/aespark/aespark.py`

 * *Files identical despite different names*

### Comparing `aespark-0.0.1/aespark/aespark/static/ip.txt` & `aespark-0.0.2/aespark/static/ip.txt`

 * *Files identical despite different names*

### Comparing `aespark-0.0.1/aespark/aespark/static/材料模板.docx` & `aespark-0.0.2/aespark/static/材料模板.docx`

 * *Files identical despite different names*

### Comparing `aespark-0.0.1/aespark.egg-info/PKG-INFO` & `aespark-0.0.2/aespark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

