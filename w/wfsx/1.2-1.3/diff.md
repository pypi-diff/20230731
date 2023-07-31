# Comparing `tmp/wfsx-1.2-py3-none-any.whl.zip` & `tmp/wfsx-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 31395 bytes, number of entries: 19
+Zip file size: 32617 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat      413 b- defN 23-Jun-06 11:13 wfsx/CONST_j.py
 -rw-rw-rw-  2.0 fat     5163 b- defN 23-Jul-28 14:45 wfsx/Excel_x.py
 -rw-rw-rw-  2.0 fat     5280 b- defN 23-Jul-28 14:45 wfsx/Report.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-06 11:13 wfsx/__init__.py
 -rw-rw-rw-  2.0 fat     6310 b- defN 23-Jul-28 14:31 wfsx/api.py
 -rw-rw-rw-  2.0 fat     6019 b- defN 23-Jun-15 14:25 wfsx/apivalid.py
 -rw-rw-rw-  2.0 fat    16574 b- defN 23-Jul-28 14:41 wfsx/apivalidation.py
 -rw-rw-rw-  2.0 fat    20705 b- defN 23-Jul-28 16:02 wfsx/common.py
 -rw-rw-rw-  2.0 fat    12039 b- defN 23-Jul-31 14:22 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1395 b- defN 23-Jul-31 14:22 wfsx-1.2.dist-info/RECORD
-19 files, 129288 bytes uncompressed, 29189 bytes compressed:  77.4%
+-rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/RECORD
+20 files, 133692 bytes uncompressed, 30285 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -36,23 +36,26 @@
 
 Filename: wfsx/plite.py
 Comment: 
 
 Filename: wfsx/results_validate.py
 Comment: 
 
-Filename: wfsx-1.2.dist-info/LICENSE
+Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.2.dist-info/METADATA
+Filename: wfsx-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.2.dist-info/WHEEL
+Filename: wfsx-1.3.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.2.dist-info/top_level.txt
+Filename: wfsx-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.2.dist-info/RECORD
+Filename: wfsx-1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: wfsx-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wfsx-1.2.dist-info/LICENSE` & `wfsx-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.2.dist-info/METADATA` & `wfsx-1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.2
+Version: 1.3
 Summary: api automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfsx/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
@@ -24,13 +24,13 @@
 Requires-Dist: urllib3
 Requires-Dist: ijson
 Requires-Dist: pandas
 Requires-Dist: SQLAlchemy
 Requires-Dist: configparser
 Requires-Dist: numpy
 Requires-Dist: selenium
-Requires-Dist: cdxg (==1.1)
+Requires-Dist: cdxg (==1.2)
 Requires-Dist: CXRunner (==1.0.6)
 
 # Accelerate API Generic functions
 Automation Framework desgined to test api's.
 * API functionality to be tested
```

