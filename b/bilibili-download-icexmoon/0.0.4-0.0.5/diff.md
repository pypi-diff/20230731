# Comparing `tmp/bilibili-download-icexmoon-0.0.4.tar.gz` & `tmp/bilibili-download-icexmoon-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-download-icexmoon-0.0.4.tar", last modified: Mon Jul 31 07:03:41 2023, max compression
+gzip compressed data, was "bilibili-download-icexmoon-0.0.5.tar", last modified: Mon Jul 31 08:20:17 2023, max compression
```

## Comparing `bilibili-download-icexmoon-0.0.4.tar` & `bilibili-download-icexmoon-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.122982 bilibili-download-icexmoon-0.0.4/
--rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.4/LICENCE
--rw-rw-rw-   0        0        0     2115 2023-07-31 07:03:41.124494 bilibili-download-icexmoon-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1565 2023-07-31 06:12:41.000000 bilibili-download-icexmoon-0.0.4/README.md
--rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      893 2023-07-31 07:03:41.127021 bilibili-download-icexmoon-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:03:40.983045 bilibili-download-icexmoon-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.070138 bilibili-download-icexmoon-0.0.4/src/bilibili_download/
--rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/__init__.py
--rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/__main__.py
--rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_album.py
--rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_user.py
--rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/download_info.py
--rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/json_parse.py
--rw-rw-rw-   0        0        0     4511 2023-07-31 04:46:54.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/main.py
--rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download/map_util.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.120860 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/
--rw-rw-rw-   0        0        0     2115 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-31 07:03:40.000000 bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 07:03:41.120860 bilibili-download-icexmoon-0.0.4/tests/
--rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.4/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:20:17.669312 bilibili-download-icexmoon-0.0.5/
+-rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.5/LICENCE
+-rw-rw-rw-   0        0        0     2143 2023-07-31 08:20:17.670312 bilibili-download-icexmoon-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-07-31 07:31:20.000000 bilibili-download-icexmoon-0.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      893 2023-07-31 08:20:17.671313 bilibili-download-icexmoon-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:20:17.630104 bilibili-download-icexmoon-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 08:20:17.640250 bilibili-download-icexmoon-0.0.5/src/bilibili_download/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/__init__.py
+-rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/__main__.py
+-rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/bilibili_album.py
+-rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/bilibili_user.py
+-rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/download_info.py
+-rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/json_parse.py
+-rw-rw-rw-   0        0        0     4511 2023-07-31 04:46:54.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/main.py
+-rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download/map_util.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:20:17.668310 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-31 08:20:17.000000 bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 08:20:17.669312 bilibili-download-icexmoon-0.0.5/tests/
+-rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.5/tests/test.py
```

### Comparing `bilibili-download-icexmoon-0.0.4/LICENCE` & `bilibili-download-icexmoon-0.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.4/PKG-INFO` & `bilibili-download-icexmoon-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-download-icexmoon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Help download lot vedio from bilibili
 Home-page: https://github.com/icexmoon/bilibili-download
 Author: icexmoon
 Author-email: icexmoon@qq.com
 Project-URL: Bug Tracker, https://github.com/icexmoon/bilibili-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,15 +63,15 @@
     ],
     "apiRetryMax": 50
 }
 ```
 
 其中元素的含义为：
 
-- homeDir，下载视频保存的根目录，下载好的视频会按照专辑作为子目录进行保存。
+- homeDir，下载视频保存的根目录，下载好的视频会按照专辑 id 作为子目录进行保存，默认为当前目录。
 - users，待下载的用户信息。
 - users.id，用户id
 - users.albums，用户专辑信息
 - albums.id，专辑id
 - albums.redoTimes，专辑下载额外重试次数（接口有调用限制，单次下载部分视频会缺失），默认10
 - apiRetryMax，接口调用重试最大次数，默认50
```

### Comparing `bilibili-download-icexmoon-0.0.4/README.md` & `bilibili-download-icexmoon-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ],
     "apiRetryMax": 50
 }
 ```
 
 其中元素的含义为：
 
-- homeDir，下载视频保存的根目录，下载好的视频会按照专辑作为子目录进行保存。
+- homeDir，下载视频保存的根目录，下载好的视频会按照专辑 id 作为子目录进行保存，默认为当前目录。
 - users，待下载的用户信息。
 - users.id，用户id
 - users.albums，用户专辑信息
 - albums.id，专辑id
 - albums.redoTimes，专辑下载额外重试次数（接口有调用限制，单次下载部分视频会缺失），默认10
 - apiRetryMax，接口调用重试最大次数，默认50
```

### Comparing `bilibili-download-icexmoon-0.0.4/setup.cfg` & `bilibili-download-icexmoon-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696c 6962 696c 692d 646f 776e   = bilibili-down
 00000020: 6c6f 6164 2d69 6365 786d 6f6f 6e0d 0a76  load-icexmoon..v
-00000030: 6572 7369 6f6e 203d 2030 2e30 2e34 0d0a  ersion = 0.0.4..
+00000030: 6572 7369 6f6e 203d 2030 2e30 2e35 0d0a  ersion = 0.0.5..
 00000040: 6175 7468 6f72 203d 2069 6365 786d 6f6f  author = icexmoo
 00000050: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
 00000060: 3d20 6963 6578 6d6f 6f6e 4071 712e 636f  = icexmoon@qq.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2048 656c 7020 646f 776e 6c6f 6164 206c   Help download l
 00000090: 6f74 2076 6564 696f 2066 726f 6d20 6269  ot vedio from bi
 000000a0: 6c69 6269 6c69 0d0a 6c6f 6e67 5f64 6573  libili..long_des
```

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download/bilibili_user.py` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download/bilibili_user.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download/download_info.py` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download/download_info.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download/json_parse.py` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download/json_parse.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download/main.py` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download/main.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/PKG-INFO` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilibili-download-icexmoon
-Version: 0.0.4
+Version: 0.0.5
 Summary: Help download lot vedio from bilibili
 Home-page: https://github.com/icexmoon/bilibili-download
 Author: icexmoon
 Author-email: icexmoon@qq.com
 Project-URL: Bug Tracker, https://github.com/icexmoon/bilibili-download/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,15 +63,15 @@
     ],
     "apiRetryMax": 50
 }
 ```
 
 其中元素的含义为：
 
-- homeDir，下载视频保存的根目录，下载好的视频会按照专辑作为子目录进行保存。
+- homeDir，下载视频保存的根目录，下载好的视频会按照专辑 id 作为子目录进行保存，默认为当前目录。
 - users，待下载的用户信息。
 - users.id，用户id
 - users.albums，用户专辑信息
 - albums.id，专辑id
 - albums.redoTimes，专辑下载额外重试次数（接口有调用限制，单次下载部分视频会缺失），默认10
 - apiRetryMax，接口调用重试最大次数，默认50
```

### Comparing `bilibili-download-icexmoon-0.0.4/src/bilibili_download_icexmoon.egg-info/SOURCES.txt` & `bilibili-download-icexmoon-0.0.5/src/bilibili_download_icexmoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

