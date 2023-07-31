# Comparing `tmp/wfs-1.1.8-py3-none-any.whl.zip` & `tmp/wfs-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 35511 bytes, number of entries: 23
+Zip file size: 35517 bytes, number of entries: 23
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/__init__.py
 -rw-rw-rw-  2.0 fat     3819 b- defN 23-Jul-26 15:23 wfs/cli.py
 -rw-rw-rw-  2.0 fat    22389 b- defN 23-Jul-26 18:16 wfs/fgen.py
 -rw-rw-rw-  2.0 fat     2786 b- defN 23-Jul-25 08:46 wfs/mproxy.py
 -rw-rw-rw-  2.0 fat     2978 b- defN 23-Jul-25 13:31 wfs/proxy.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/pages/__init__.py
 -rw-rw-rw-  2.0 fat     5448 b- defN 23-Jul-25 08:46 wfs/pages/action_step.py
@@ -12,14 +12,14 @@
 -rw-rw-rw-  2.0 fat    15519 b- defN 23-Jul-26 16:50 wfs/pages/object_repo_page.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-25 08:46 wfs/utils/__init__.py
 -rw-rw-rw-  2.0 fat    19870 b- defN 23-Jul-26 16:50 wfs/utils/action_test_item.py
 -rw-rw-rw-  2.0 fat     6924 b- defN 23-Jul-26 16:50 wfs/utils/assertions.py
 -rw-rw-rw-  2.0 fat    10320 b- defN 23-Jul-26 16:50 wfs/utils/common.py
 -rw-rw-rw-  2.0 fat     4608 b- defN 23-Jul-26 08:27 wfs/utils/confapp.py
 -rw-rw-rw-  2.0 fat     5991 b- defN 23-Jul-25 08:46 wfs/utils/parseexcel.py
--rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1348 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       99 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1764 b- defN 23-Jul-26 18:18 wfs-1.1.8.dist-info/RECORD
-23 files, 142590 bytes uncompressed, 32707 bytes compressed:  77.1%
+-rw-rw-rw-  2.0 fat    11365 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1373 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       99 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1764 b- defN 23-Jul-31 15:22 wfs-1.1.9.dist-info/RECORD
+23 files, 142615 bytes uncompressed, 32713 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -45,26 +45,26 @@
 
 Filename: wfs/utils/confapp.py
 Comment: 
 
 Filename: wfs/utils/parseexcel.py
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/LICENSE
+Filename: wfs-1.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/METADATA
+Filename: wfs-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/WHEEL
+Filename: wfs-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/entry_points.txt
+Filename: wfs-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/top_level.txt
+Filename: wfs-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wfs-1.1.8.dist-info/RECORD
+Filename: wfs-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `wfs-1.1.8.dist-info/LICENSE` & `wfs-1.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wfs-1.1.8.dist-info/METADATA` & `wfs-1.1.9.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wfs
-Version: 1.1.8
+Version: 1.1.9
 Summary: fms automation testing framework based on unittest.
 Home-page: https://github.com/saasaa831/wfs/
 Author: saasaa
 Author-email: saasaa@saa.com
 License: Apache 2.0
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: MacOS :: MacOS X
@@ -24,14 +24,15 @@
 Requires-Dist: openpyxl
 Requires-Dist: xlrd
 Requires-Dist: ffmpeg
 Requires-Dist: pyautogui
 Requires-Dist: poium
 Requires-Dist: waiting
 Requires-Dist: mitmproxy
-Requires-Dist: cdxg (==1.1)
+Requires-Dist: selenium
+Requires-Dist: cdxg (==1.3)
 Requires-Dist: CXRunner (==1.0.6)
 Requires-Dist: configparser (==5.3.0)
 
 # Accelerate Framework
 Automation Framework desgined to test web, mobile and desktop applications.
 * UI functionality to be tested for web, mobile or desktop applications
```

## Comparing `wfs-1.1.8.dist-info/RECORD` & `wfs-1.1.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 wfs/pages/object_repo_page.py,sha256=Cjq_cQuoWykTOHjFKlOxm2DPn6yjloKmnfbxG5x1fMM,15519
 wfs/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wfs/utils/action_test_item.py,sha256=LIJQrZTQE7VfzX5rX3S6I94BIO--t2xCakgExuwB8f0,19870
 wfs/utils/assertions.py,sha256=avIcgxQB844_IXooPuMrnPUI3pPs6IlLmfxcsKrP84U,6924
 wfs/utils/common.py,sha256=bWBrpKXtJTfm__oIPoOYZXxkIeJEmBgxFbSkcOoy2oI,10320
 wfs/utils/confapp.py,sha256=ecPJK6BELeIr6qGC2nTzjPwvuJ-xz-LrBPD2M8p8y6E,4608
 wfs/utils/parseexcel.py,sha256=HvXDdAbFByHUKqi-V4f_Vo1l5DdvdBa_iuC6mhLMf2U,5991
-wfs-1.1.8.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
-wfs-1.1.8.dist-info/METADATA,sha256=r7lbsi8JUNvXDr8ZaJa17HMmgVpHKysBgoZoA8iqRvU,1348
-wfs-1.1.8.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wfs-1.1.8.dist-info/entry_points.txt,sha256=7FtgvgAvRY5Fu3NUkE8PIqCoJ0aqnPlT3NfO7_1Mhiw,99
-wfs-1.1.8.dist-info/top_level.txt,sha256=SvDSVst_ygBLSCxkPHGmSU8tKuPQRVd_ttWw9nVzEwY,4
-wfs-1.1.8.dist-info/RECORD,,
+wfs-1.1.9.dist-info/LICENSE,sha256=O6YYwBy5W9D4kClOvrHiQlSfu479SgduHM03YRmz8mE,11365
+wfs-1.1.9.dist-info/METADATA,sha256=4mJfGy2BD0MZesyIPgwG2WrpEERtMXm2CgpnuBJzTBw,1373
+wfs-1.1.9.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wfs-1.1.9.dist-info/entry_points.txt,sha256=7FtgvgAvRY5Fu3NUkE8PIqCoJ0aqnPlT3NfO7_1Mhiw,99
+wfs-1.1.9.dist-info/top_level.txt,sha256=SvDSVst_ygBLSCxkPHGmSU8tKuPQRVd_ttWw9nVzEwY,4
+wfs-1.1.9.dist-info/RECORD,,
```

