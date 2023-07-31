# Comparing `tmp/bilibili-download-icexmoon-0.0.1.tar.gz` & `tmp/bilibili-download-icexmoon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilibili-download-icexmoon-0.0.1.tar", last modified: Mon Jul 31 04:31:32 2023, max compression
+gzip compressed data, was "bilibili-download-icexmoon-0.0.2.tar", last modified: Mon Jul 31 05:06:20 2023, max compression
```

## Comparing `bilibili-download-icexmoon-0.0.1.tar` & `bilibili-download-icexmoon-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:32.351347 bilibili-download-icexmoon-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      571 2023-07-31 04:31:32.351347 bilibili-download-icexmoon-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       21 2023-07-31 04:24:38.000000 bilibili-download-icexmoon-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      882 2023-07-31 04:31:32.359059 bilibili-download-icexmoon-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:32.309929 bilibili-download-icexmoon-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:32.319908 bilibili-download-icexmoon-0.0.1/src/bilibili_download/
--rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/__init__.py
--rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/__main__.py
--rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/bilibili_album.py
--rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/bilibili_user.py
--rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/download_info.py
--rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/json_parse.py
--rw-rw-rw-   0        0        0     4448 2023-07-31 04:07:38.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/main.py
--rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download/map_util.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:32.350645 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/
--rw-rw-rw-   0        0        0      571 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-31 04:31:32.000000 bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 04:31:32.351347 bilibili-download-icexmoon-0.0.1/tests/
--rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:06:20.499326 bilibili-download-icexmoon-0.0.2/
+-rw-rw-rw-   0        0        0     1100 2023-07-31 01:30:45.000000 bilibili-download-icexmoon-0.0.2/LICENCE
+-rw-rw-rw-   0        0        0     2129 2023-07-31 05:06:20.499326 bilibili-download-icexmoon-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2023-07-31 05:04:02.000000 bilibili-download-icexmoon-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-31 01:31:02.000000 bilibili-download-icexmoon-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      882 2023-07-31 05:06:20.501325 bilibili-download-icexmoon-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-07-31 01:49:08.000000 bilibili-download-icexmoon-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:06:20.443217 bilibili-download-icexmoon-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:06:20.464382 bilibili-download-icexmoon-0.0.2/src/bilibili_download/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:56:19.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/__init__.py
+-rw-rw-rw-   0        0        0      173 2023-07-31 02:01:09.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/__main__.py
+-rw-rw-rw-   0        0        0      370 2023-07-31 03:27:53.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/bilibili_album.py
+-rw-rw-rw-   0        0        0      529 2023-07-31 02:33:07.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/bilibili_user.py
+-rw-rw-rw-   0        0        0      604 2023-07-31 03:25:16.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/download_info.py
+-rw-rw-rw-   0        0        0     2574 2023-07-31 04:14:53.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/json_parse.py
+-rw-rw-rw-   0        0        0     4511 2023-07-31 04:46:54.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/main.py
+-rw-rw-rw-   0        0        0      434 2023-07-31 03:05:23.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download/map_util.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:06:20.497310 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/
+-rw-rw-rw-   0        0        0     2129 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-31 05:06:20.000000 bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 05:06:20.498318 bilibili-download-icexmoon-0.0.2/tests/
+-rw-rw-rw-   0        0        0      151 2023-07-31 04:03:37.000000 bilibili-download-icexmoon-0.0.2/tests/test.py
```

### Comparing `bilibili-download-icexmoon-0.0.1/LICENCE` & `bilibili-download-icexmoon-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.1/setup.cfg` & `bilibili-download-icexmoon-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696c 6962 696c 692d 646f 776e   = bilibili-down
 00000020: 6c6f 6164 2d69 6365 786d 6f6f 6e0d 0a76  load-icexmoon..v
-00000030: 6572 7369 6f6e 203d 2030 2e30 2e31 0d0a  ersion = 0.0.1..
+00000030: 6572 7369 6f6e 203d 2030 2e30 2e32 0d0a  ersion = 0.0.2..
 00000040: 6175 7468 6f72 203d 2069 6365 786d 6f6f  author = icexmoo
 00000050: 6e0d 0a61 7574 686f 725f 656d 6169 6c20  n..author_email 
 00000060: 3d20 6963 6578 6d6f 6f6e 4071 712e 636f  = icexmoon@qq.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2048 656c 7020 646f 776e 6c6f 6164 206c   Help download l
 00000090: 6f74 2076 6564 696f 2066 726f 6d20 6269  ot vedio from bi
 000000a0: 6c69 6269 6c69 0d0a 6c6f 6e67 5f64 6573  libili..long_des
```

### Comparing `bilibili-download-icexmoon-0.0.1/src/bilibili_download/bilibili_user.py` & `bilibili-download-icexmoon-0.0.2/src/bilibili_download/bilibili_user.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.1/src/bilibili_download/download_info.py` & `bilibili-download-icexmoon-0.0.2/src/bilibili_download/download_info.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.1/src/bilibili_download/json_parse.py` & `bilibili-download-icexmoon-0.0.2/src/bilibili_download/json_parse.py`

 * *Files identical despite different names*

### Comparing `bilibili-download-icexmoon-0.0.1/src/bilibili_download/main.py` & `bilibili-download-icexmoon-0.0.2/src/bilibili_download/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,9 +94,10 @@
         url = "https://www.bilibili.com/video/{}".format(bvid)
         # cmd = "you-get -o {} https://www.bilibili.com/video/{}".format(
         #     path, bvid)
         # print("exec you-get, cmd[{}]".format(cmd))
         # subprocess.call(cmd, shell=True)
         print("begin downlod vedio [{}]".format(url))
         result = subprocess.run(["you-get", "-o", path, url], shell=True)
+        # os.system('you-get "{}" -o "{}"'.format(url, path))
         # print(result.stdout.decode("GBK"))
         time.sleep(5)
```

### Comparing `bilibili-download-icexmoon-0.0.1/src/bilibili_download_icexmoon.egg-info/SOURCES.txt` & `bilibili-download-icexmoon-0.0.2/src/bilibili_download_icexmoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

