# Comparing `tmp/wfsx-1.3-py3-none-any.whl.zip` & `tmp/wfsx-1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -10,13 +10,13 @@
 -rw-rw-rw-  2.0 fat    12039 b- defN 23-Jul-31 14:22 wfsx/dataextract.py
 -rw-rw-rw-  2.0 fat     2808 b- defN 23-Jun-06 11:13 wfsx/excel_json_reader.py
 -rw-rw-rw-  2.0 fat     4189 b- defN 23-Jun-16 15:41 wfsx/ghelper.py
 -rw-rw-rw-  2.0 fat     5407 b- defN 23-Jun-06 11:13 wfsx/parseexcel.py
 -rw-rw-rw-  2.0 fat     7022 b- defN 23-Jun-13 11:44 wfsx/plite.py
 -rw-rw-rw-  2.0 fat    23242 b- defN 23-Jul-28 14:45 wfsx/results_validate.py
 -rw-rw-rw-  2.0 fat     4322 b- defN 23-Jul-27 11:01 wfsx/inix/endpointapi.ini
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1477 b- defN 23-Jul-31 14:31 wfsx-1.3.dist-info/RECORD
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 14:54 wfsx-1.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1260 b- defN 23-Jul-31 14:54 wfsx-1.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 14:54 wfsx-1.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-31 14:54 wfsx-1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1477 b- defN 23-Jul-31 14:54 wfsx-1.4.dist-info/RECORD
 20 files, 133692 bytes uncompressed, 30285 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: wfsx/results_validate.py
 Comment: 
 
 Filename: wfsx/inix/endpointapi.ini
 Comment: 
 
-Filename: wfsx-1.3.dist-info/LICENSE
+Filename: wfsx-1.4.dist-info/LICENSE
 Comment: 
 
-Filename: wfsx-1.3.dist-info/METADATA
+Filename: wfsx-1.4.dist-info/METADATA
 Comment: 
 
-Filename: wfsx-1.3.dist-info/WHEEL
+Filename: wfsx-1.4.dist-info/WHEEL
 Comment: 
 
-Filename: wfsx-1.3.dist-info/top_level.txt
+Filename: wfsx-1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: wfsx-1.3.dist-info/RECORD
+Filename: wfsx-1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wfsx-1.3.dist-info/LICENSE` & `wfsx-1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfsx-1.3.dist-info/METADATA` & `wfsx-1.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfsx
-Version: 1.3
+Version: 1.4
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
-Requires-Dist: cdxg (==1.2)
+Requires-Dist: cdxg (==1.3)
 Requires-Dist: CXRunner (==1.0.6)
 
 # Accelerate API Generic functions
 Automation Framework desgined to test api's.
 * API functionality to be tested
```

## Comparing `wfsx-1.3.dist-info/RECORD` & `wfsx-1.4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 wfsx/dataextract.py,sha256=C5lm_ZV1QmkfKK9VbzFwKSaGo44SduJl7DfA9ZJWjzI,12039
 wfsx/excel_json_reader.py,sha256=z4vQkNRLKCO7x3UAeI8EVd9vjY5GDTEYDOVTj2jqICA,2808
 wfsx/ghelper.py,sha256=oYgGDv8YZOKAX6vg4gel0kjpaAwZ40137AQhAFDFnW8,4189
 wfsx/parseexcel.py,sha256=uXXUcI9AiDHqdaKd8oGAxu_3OXFmuw66CLRXvJRXHtc,5407
 wfsx/plite.py,sha256=d2yNK_XkO17OFQbr4Ecf_OSkDgys9vzdefnm03Lm3Ck,7022
 wfsx/results_validate.py,sha256=Jzx6xUHcbrTQuKhc9q48vKR7BXmSrEbD8T7SB45c_NM,23242
 wfsx/inix/endpointapi.ini,sha256=0NfMZyTdLlBseaPlWWtzLFShX2qGODskfJ7PVUVnK34,4322
-wfsx-1.3.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfsx-1.3.dist-info/METADATA,sha256=Aufz6UKNdxA4rhREdd6Iq8DxLVn2tdTZwSZECy9GKdY,1260
-wfsx-1.3.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfsx-1.3.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
-wfsx-1.3.dist-info/RECORD,,
+wfsx-1.4.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfsx-1.4.dist-info/METADATA,sha256=Qu67dJDO0XWA86f_TC_flQQMB4iBct_ysRQer1xSx0c,1260
+wfsx-1.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfsx-1.4.dist-info/top_level.txt,sha256=ylpSMw0AVSmfULYBvc6iiXmLKtra7xinB3IPH0sBALs,5
+wfsx-1.4.dist-info/RECORD,,
```

