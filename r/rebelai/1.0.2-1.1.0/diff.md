# Comparing `tmp/rebelai-1.0.2-py2.py3-none-any.whl.zip` & `tmp/rebelai-1.1.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,19 @@
-Zip file size: 17943 bytes, number of entries: 11
--rw-r--r--  2.0 unx      129 b- defN 23-Jul-30 20:14 rebelai/__init__.py
+Zip file size: 23087 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      129 b- defN 23-Jul-31 14:47 rebelai/__init__.py
 -rw-r--r--  2.0 unx     2002 b- defN 23-Jul-30 19:36 rebelai/const.py
 -rw-r--r--  2.0 unx     3555 b- defN 23-Jul-30 19:35 rebelai/enums.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/py.typed
+-rw-r--r--  2.0 unx       81 b- defN 23-Jul-31 14:47 rebelai/ai/__init__.py
+-rw-r--r--  2.0 unx      810 b- defN 23-Jul-30 19:26 rebelai/ai/alpaca.py
+-rw-r--r--  2.0 unx     1700 b- defN 23-Jul-30 19:27 rebelai/ai/deepai.py
+-rw-r--r--  2.0 unx     4560 b- defN 23-Jul-30 19:28 rebelai/ai/gpt.py
+-rw-r--r--  2.0 unx      720 b- defN 23-Jul-30 19:28 rebelai/ai/pollinations.py
+-rw-r--r--  2.0 unx     2919 b- defN 23-Jul-30 19:29 rebelai/ai/prodia.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jul-30 19:33 rebelai/ai/py.typed
--rw-------  2.0 unx    35115 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3091 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-1.0.2.dist-info/zip-safe
--rw-rw-r--  2.0 unx      837 b- defN 23-Jul-30 20:15 rebelai-1.0.2.dist-info/RECORD
-11 files, 44848 bytes uncompressed, 16531 bytes compressed:  63.1%
+-rw-------  2.0 unx    35115 b- defN 23-Jul-31 14:53 rebelai-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3091 b- defN 23-Jul-31 14:53 rebelai-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-31 14:53 rebelai-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-31 14:53 rebelai-1.1.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-30 15:48 rebelai-1.1.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1300 b- defN 23-Jul-31 14:53 rebelai-1.1.0.dist-info/RECORD
+17 files, 56101 bytes uncompressed, 20969 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -6,29 +6,47 @@
 
 Filename: rebelai/enums.py
 Comment: 
 
 Filename: rebelai/py.typed
 Comment: 
 
+Filename: rebelai/ai/__init__.py
+Comment: 
+
+Filename: rebelai/ai/alpaca.py
+Comment: 
+
+Filename: rebelai/ai/deepai.py
+Comment: 
+
+Filename: rebelai/ai/gpt.py
+Comment: 
+
+Filename: rebelai/ai/pollinations.py
+Comment: 
+
+Filename: rebelai/ai/prodia.py
+Comment: 
+
 Filename: rebelai/ai/py.typed
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/LICENSE
+Filename: rebelai-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/METADATA
+Filename: rebelai-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/WHEEL
+Filename: rebelai-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/top_level.txt
+Filename: rebelai-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/zip-safe
+Filename: rebelai-1.1.0.dist-info/zip-safe
 Comment: 
 
-Filename: rebelai-1.0.2.dist-info/RECORD
+Filename: rebelai-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rebelai/__init__.py

```diff
@@ -1,5 +1,5 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """rebelai -- providing free ai access to everyone"""
 
-__version__: str = "1.0.2"
+__version__: str = "1.1.0"
```

## Comparing `rebelai-1.0.2.dist-info/LICENSE` & `rebelai-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rebelai-1.0.2.dist-info/METADATA` & `rebelai-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rebelai
-Version: 1.0.2
+Version: 1.1.0
 Summary: providing free access to proprietary ai models in python
 Home-page: https://ari-web.xyz/gh/rebelai
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,http-client,api,https,ai,machine learning,openai
 Classifier: Development Status :: 5 - Production/Stable
```

