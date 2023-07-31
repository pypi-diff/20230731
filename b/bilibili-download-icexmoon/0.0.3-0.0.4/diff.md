# Comparing `tmp/bilibili-download-icexmoon-0.0.3.tar.gz` & `tmp/bilibili-download-icexmoon-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-download-icexmoon-0.0.3.tar", last modified: Mon Jul 31 06:13:52 2023, max compression
+gzip compressed data, was "bilibili-download-icexmoon-0.0.4.tar", last modified: Mon Jul 31 07:03:41 2023, max compression
```

## Comparing `bilibili-download-icexmoon-0.0.3.tar` & `bilibili-download-icexmoon-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:13:52.323372 bilibili-download-icexmoon-0.0.3/
--rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.3/LICENCE
--rw-rw-rw-   0        0        0     2115 2023-07-31 06:13:52.323372 bilibili-download-icexmoon-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1565 2023-07-31 06:12:41.000000 bilibili-download-icexmoon-0.0.3/README.md
--rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      882 2023-07-31 06:13:52.332261 bilibili-download-icexmoon-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:13:52.273900 bilibili-download-icexmoon-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 06:13:52.293512 bilibili-download-icexmoon-0.0.3/src/bilibili_download/
--rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/__init__.py
--rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/__main__.py
--rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/bilibili_album.py
--rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/bilibili_user.py
--rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/download_info.py
--rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/json_parse.py
--rw-rw-rw-   0        0        0     4511 2023-07-31 04:46:54.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/main.py
--rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download/map_util.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:13:52.321367 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/
--rw-rw-rw-   0        0        0     2115 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-31 06:13:52.000000 bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 06:13:52.322368 bilibili-download-icexmoon-0.0.3/tests/
--rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.122982 bilibili-download-icexmoon-0.0.4/
+-rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.4/LICENCE
+-rw-rw-rw-   0        0        0     2115 2023-07-31 07:03:41.124494 bilibili-download-icexmoon-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1565 2023-07-31 06:12:41.000000 bilibili-download-icexmoon-0.0.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-31 07:03:41.127021 bilibili-download-icexmoon-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:03:40.983045 bilibili-download-icexmoon-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.070138 bilibili-download-icexmoon-0.0.4/src/bilibili_download/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/__init__.py
+-rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/__main__.py
+-rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_album.py
+-rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_user.py
+-rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/download_info.py
+-rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/json_parse.py
+-rw-rw-rw-   0        0        0     4511 2023-07-31 04:46:54.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/main.py
+-rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/map_util.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.120860 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/
+-rw-rw-rw-   0        0        0     2115 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.120860 bilibili-download-icexmoon-0.0.4/tests/
+-rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.4/tests/test.py
```

### Comparing `bilibili-download-icexmoon-0.0.3/LICENCE` & `bilibili-download-icexmoon-0.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/PKG-INFO` & `bilibili-download-icexmoon-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-download-icexmoon
-Version: 0.0.3
+Version: 0.0.4
 Summary: Help download lot vedio from bilibili
 Home-page: https://github.com/icexmoon/bilibili-download
 Author: icexmoon
 Author-email: icexmoon@qq.com
 Project-URL: Bug Tracker, https://github.com/icexmoon/bilibili-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bilibili-download-icexmoon-0.0.3/README.md` & `bilibili-download-icexmoon-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/setup.cfg` & `bilibili-download-icexmoon-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696c 6962 696c 692d 646f 776e   = bilibili-down
 00000020: 6c6f 6164 2d69 6365 786d 6f6f 6e0d 0a76  load-icexmoon..v
-00000030: 6572 7369 6f6e 203d 2030 2e30 2e33 0d0a  ersion = 0.0.3..
+00000030: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
 00000040: 6175 7468 6f72 203d 2069 6365 786d 6f6f  author = icexmoo
 00000050: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
 00000060: 3d20 6963 6578 6d6f 6f6e 4071 712e 636f  = icexmoon@qq.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2048 656c 7020 646f 776e 6c6f 6164 206c   Help download l
 00000090: 6f74 2076 6564 696f 2066 726f 6d20 6269  ot vedio from bi
 000000a0: 6c69 6269 6c69 0d0a 6c6f 6e67 5f64 6573  libili..long_des
@@ -35,22 +35,22 @@
 00000220: 6163 6b61 6765 5f64 6174 6120 3d20 4661  ackage_data = Fa
 00000230: 6c73 650d 0a70 6163 6b61 6765 5f64 6972  lse..package_dir
 00000240: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
 00000250: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
 00000260: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
 00000270: 203e 3d33 2e31 302e 350d 0a69 6e73 7461   >=3.10.5..insta
 00000280: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000290: 0979 6f75 2d67 6574 0d0a 0d0a 5b6f 7074  .you-get....[opt
-000002a0: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-000002b0: 615d 0d0a 2a20 3d20 2a2e 696e 666f 0d0a  a]..* = *.info..
-000002c0: 0d0a 5b6f 7074 696f 6e73 2e70 6163 6b61  ..[options.packa
-000002d0: 6765 732e 6669 6e64 5d0d 0a77 6865 7265  ges.find]..where
-000002e0: 203d 2073 7263 0d0a 0d0a 5b6f 7074 696f   = src....[optio
-000002f0: 6e73 2e65 6e74 7279 5f70 6f69 6e74 735d  ns.entry_points]
-00000300: 0d0a 636f 6e73 6f6c 655f 7363 7269 7074  ..console_script
-00000310: 7320 3d20 0d0a 0962 622d 646f 776e 6c6f  s = ...bb-downlo
-00000320: 6164 203d 2062 696c 6962 696c 695f 646f  ad = bilibili_do
-00000330: 776e 6c6f 6164 2e5f 5f6d 6169 6e5f 5f3a  wnload.__main__:
-00000340: 6d61 696e 0d0a 0d0a 5b65 6767 5f69 6e66  main....[egg_inf
-00000350: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000360: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000370: 0d0a                                     ..
+00000290: 0979 6f75 2d67 6574 0d0a 0972 6571 7565  .you-get...reque
+000002a0: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
+000002b0: 7061 636b 6167 655f 6461 7461 5d0d 0a2a  package_data]..*
+000002c0: 203d 202a 2e69 6e66 6f0d 0a0d 0a5b 6f70   = *.info....[op
+000002d0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
+000002e0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
+000002f0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  c....[options.en
+00000300: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+00000310: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+00000320: 0a09 6262 2d64 6f77 6e6c 6f61 6420 3d20  ..bb-download = 
+00000330: 6269 6c69 6269 6c69 5f64 6f77 6e6c 6f61  bilibili_downloa
+00000340: 642e 5f5f 6d61 696e 5f5f 3a6d 6169 6e0d  d.__main__:main.
+00000350: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000360: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000370: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download/bilibili_user.py` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_user.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download/download_info.py` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download/download_info.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download/json_parse.py` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download/json_parse.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download/main.py` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download/main.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/PKG-INFO` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-download-icexmoon
-Version: 0.0.3
+Version: 0.0.4
 Summary: Help download lot vedio from bilibili
 Home-page: https://github.com/icexmoon/bilibili-download
 Author: icexmoon
 Author-email: icexmoon@qq.com
 Project-URL: Bug Tracker, https://github.com/icexmoon/bilibili-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bilibili-download-icexmoon-0.0.3/src/bilibili_download_icexmoon.egg-info/SOURCES.txt` & `bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

