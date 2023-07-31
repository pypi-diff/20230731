# Comparing `tmp/KolejkaClient-0.1.202307311426-py3-none-any.whl.zip` & `tmp/KolejkaClient-0.1.202307311914-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6536 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426-nspkg.pth
+Zip file size: 6542 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      544 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914-nspkg.pth
 -rw-rw-r--  2.0 unx     1032 b- defN 23-Jan-19 17:32 kolejka/client/__init__.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-13 18:28 kolejka/client/__nonpath__.py
--rw-rw-r--  2.0 unx    18662 b- defN 23-Jul-31 14:28 kolejka/client/client.py
--rw-rw-r--  2.0 unx      535 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/WHEEL
--rw-rw-r--  2.0 unx       56 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/namespace_packages.txt
--rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      937 b- defN 23-Jul-31 14:29 KolejkaClient-0.1.202307311426.dist-info/RECORD
-10 files, 21874 bytes uncompressed, 4884 bytes compressed:  77.7%
+-rw-rw-r--  2.0 unx    18676 b- defN 23-Jul-31 19:16 kolejka/client/client.py
+-rw-rw-r--  2.0 unx      535 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       56 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/namespace_packages.txt
+-rw-rw-r--  2.0 unx        8 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      937 b- defN 23-Jul-31 19:17 KolejkaClient-0.1.202307311914.dist-info/RECORD
+10 files, 21888 bytes uncompressed, 4890 bytes compressed:  77.7%
```

## zipnote {}

```diff
@@ -1,31 +1,31 @@
-Filename: KolejkaClient-0.1.202307311426-nspkg.pth
+Filename: KolejkaClient-0.1.202307311914-nspkg.pth
 Comment: 
 
 Filename: kolejka/client/__init__.py
 Comment: 
 
 Filename: kolejka/client/__nonpath__.py
 Comment: 
 
 Filename: kolejka/client/client.py
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/METADATA
+Filename: KolejkaClient-0.1.202307311914.dist-info/METADATA
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/WHEEL
+Filename: KolejkaClient-0.1.202307311914.dist-info/WHEEL
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/entry_points.txt
+Filename: KolejkaClient-0.1.202307311914.dist-info/entry_points.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/namespace_packages.txt
+Filename: KolejkaClient-0.1.202307311914.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/top_level.txt
+Filename: KolejkaClient-0.1.202307311914.dist-info/top_level.txt
 Comment: 
 
-Filename: KolejkaClient-0.1.202307311426.dist-info/RECORD
+Filename: KolejkaClient-0.1.202307311914.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kolejka/client/client.py

```diff
@@ -10,15 +10,15 @@
 import requests
 import shutil
 import sys
 import time
 
 from kolejka.common import kolejka_config, client_config
 from kolejka.common import KolejkaTask, KolejkaResult, KolejkaLimits
-from kolejka.common import MemoryAction, TimeAction
+from kolejka.common import MemoryAction, TimeAction, BigIntAction
 
 class KolejkaClientError(Exception):
     pass
 
 class KolejkaClientAuthorizationError(KolejkaClientError):
     pass
```

## Comparing `KolejkaClient-0.1.202307311426-nspkg.pth` & `KolejkaClient-0.1.202307311914-nspkg.pth`

 * *Files identical despite different names*

## Comparing `KolejkaClient-0.1.202307311426.dist-info/METADATA` & `KolejkaClient-0.1.202307311914.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KolejkaClient
-Version: 0.1.202307311426
+Version: 0.1.202307311914
 Summary: Kolejka Client
 Home-page: https://github.com/kolejka/kolejka
 Author: KOLEJKA
 Author-email: kolejka@matinf.uj.edu.pl
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

## Comparing `KolejkaClient-0.1.202307311426.dist-info/RECORD` & `KolejkaClient-0.1.202307311914.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-KolejkaClient-0.1.202307311426-nspkg.pth,sha256=ymghxcR0SaoJPJNC5JQSPrO2foeCxLaTaJ0CvL2Q_H4,544
+KolejkaClient-0.1.202307311914-nspkg.pth,sha256=ymghxcR0SaoJPJNC5JQSPrO2foeCxLaTaJ0CvL2Q_H4,544
 kolejka/client/__init__.py,sha256=OuNTzofl-2FGuC55nfxqNeZsqCiE-J6szRN-gGEB7xA,1032
 kolejka/client/__nonpath__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-kolejka/client/client.py,sha256=4s8UaYg4myTs5e-OsmqVX48Z62iR-keGBtns-t4TRQk,18662
-KolejkaClient-0.1.202307311426.dist-info/METADATA,sha256=BVWDU8OxmBLM2fxEqdWhCg3oOrpJzBsQBzLZ0fsODtw,535
-KolejkaClient-0.1.202307311426.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-KolejkaClient-0.1.202307311426.dist-info/entry_points.txt,sha256=S_LbdlFa8PWwuIrcnQN6g5mhUVHJml-uvP5AsqKm9BE,56
-KolejkaClient-0.1.202307311426.dist-info/namespace_packages.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
-KolejkaClient-0.1.202307311426.dist-info/top_level.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
-KolejkaClient-0.1.202307311426.dist-info/RECORD,,
+kolejka/client/client.py,sha256=APNzis6bkrwjutqU0w9zwfHSc-_8YTSUK5NLRB41WoA,18676
+KolejkaClient-0.1.202307311914.dist-info/METADATA,sha256=iMnaUm0uwWdK6iW5gdEFhXEabdwGAyw91_ONN8FtDRY,535
+KolejkaClient-0.1.202307311914.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+KolejkaClient-0.1.202307311914.dist-info/entry_points.txt,sha256=S_LbdlFa8PWwuIrcnQN6g5mhUVHJml-uvP5AsqKm9BE,56
+KolejkaClient-0.1.202307311914.dist-info/namespace_packages.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
+KolejkaClient-0.1.202307311914.dist-info/top_level.txt,sha256=JRltIMS23djVkt75McrNZpEyfqHwicCBrIZYwdn_g98,8
+KolejkaClient-0.1.202307311914.dist-info/RECORD,,
```

