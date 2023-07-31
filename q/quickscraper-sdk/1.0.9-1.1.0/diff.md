# Comparing `tmp/quickscraper_sdk-1.0.9-py3-none-any.whl.zip` & `tmp/quickscraper_sdk-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6398 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat     8851 b- defN 23-Apr-11 05:19 quickscraper_sdk/__init__.py
--rw-rw-rw-  2.0 fat      272 b- defN 23-Apr-11 05:19 quickscraper_sdk/constant.py
+Zip file size: 6394 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat     8851 b- defN 23-Apr-11 05:23 quickscraper_sdk/__init__.py
+-rw-rw-rw-  2.0 fat      272 b- defN 23-Jul-31 06:39 quickscraper_sdk/constant.py
 -rw-rw-rw-  2.0 fat       70 b- defN 23-Mar-31 09:41 tests/__init__.py
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Mar-31 09:41 tests/constant.py
 -rw-rw-rw-  2.0 fat     5250 b- defN 23-Mar-31 09:41 tests/test_cases.py
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4126 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      821 b- defN 23-Apr-11 05:20 quickscraper_sdk-1.0.9.dist-info/RECORD
-10 files, 20789 bytes uncompressed, 4990 bytes compressed:  76.0%
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jul-31 08:37 quickscraper_sdk-1.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4126 b- defN 23-Jul-31 08:37 quickscraper_sdk-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 08:37 quickscraper_sdk-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jul-31 08:37 quickscraper_sdk-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      821 b- defN 23-Jul-31 08:37 quickscraper_sdk-1.1.0.dist-info/RECORD
+10 files, 20789 bytes uncompressed, 4986 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: tests/constant.py
 Comment: 
 
 Filename: tests/test_cases.py
 Comment: 
 
-Filename: quickscraper_sdk-1.0.9.dist-info/LICENSE
+Filename: quickscraper_sdk-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: quickscraper_sdk-1.0.9.dist-info/METADATA
+Filename: quickscraper_sdk-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: quickscraper_sdk-1.0.9.dist-info/WHEEL
+Filename: quickscraper_sdk-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: quickscraper_sdk-1.0.9.dist-info/top_level.txt
+Filename: quickscraper_sdk-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: quickscraper_sdk-1.0.9.dist-info/RECORD
+Filename: quickscraper_sdk-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quickscraper_sdk/constant.py

```diff
@@ -1,10 +1,10 @@
 import os
 
 
 BASE_URL = os.environ.get('QS_BASE_URL') or 'https://api.quickscraper.co/'
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 
 
 # from importlib.metadata import version
 # VERSION = version('quickscraper-sdk')
 # Not working this approach with pytest, so version is defined statically
```

## Comparing `quickscraper_sdk-1.0.9.dist-info/LICENSE` & `quickscraper_sdk-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `quickscraper_sdk-1.0.9.dist-info/METADATA` & `quickscraper_sdk-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickscraper-sdk
-Version: 1.0.9
+Version: 1.1.0
 Summary: https://quickscraper.co
 Home-page: https://quickscraper.co/
 Author: QuickScraper
 Author-email: app@quickscraper.co
 License: BSD
 Keywords: quickscraper
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `quickscraper_sdk-1.0.9.dist-info/RECORD` & `quickscraper_sdk-1.1.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 quickscraper_sdk/__init__.py,sha256=m8TF4hZaCvVNWddAjmvFCmKCudzrxxdHixKGbPgijiQ,8851
-quickscraper_sdk/constant.py,sha256=qdecmtVe3tbYkB1Ac3flZFLoJJiNnILJ9HR7h21H3Rs,272
+quickscraper_sdk/constant.py,sha256=1Hsf1baOPSktx8hZvupb_bVAoe8U9oPb8VSUnsW_oUU,272
 tests/__init__.py,sha256=FspmhViTO62HL15bC5o4qXWEALYaCRXsIaPi6Suj_Ls,70
 tests/constant.py,sha256=2r5201gu1BXxBJgSddaIK8vKhAdLUxkhnG_veOpv0_Q,192
 tests/test_cases.py,sha256=mrO6M4vbqp4Sekt4uHUnOPKyyhyVxPyVX1xjN3fhMzk,5250
-quickscraper_sdk-1.0.9.dist-info/LICENSE,sha256=DfrJyVjirZSu1qGS0tb7LR8OFpCVBJqaUM27NSvA9Ug,1092
-quickscraper_sdk-1.0.9.dist-info/METADATA,sha256=pGEcQqD9RLJzofDKuiOyRqQVO1GWqwWtP92J4rNaqmA,4126
-quickscraper_sdk-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-quickscraper_sdk-1.0.9.dist-info/top_level.txt,sha256=QkNMMYAEdAj6OURlUcHxYLG5ZMoiRfYfyNPgxD8JLFY,23
-quickscraper_sdk-1.0.9.dist-info/RECORD,,
+quickscraper_sdk-1.1.0.dist-info/LICENSE,sha256=DfrJyVjirZSu1qGS0tb7LR8OFpCVBJqaUM27NSvA9Ug,1092
+quickscraper_sdk-1.1.0.dist-info/METADATA,sha256=iv6jj_jxkAnoO2yvTQ_WMrWbjGAIDSfRHBO6HMFNlnU,4126
+quickscraper_sdk-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+quickscraper_sdk-1.1.0.dist-info/top_level.txt,sha256=QkNMMYAEdAj6OURlUcHxYLG5ZMoiRfYfyNPgxD8JLFY,23
+quickscraper_sdk-1.1.0.dist-info/RECORD,,
```

