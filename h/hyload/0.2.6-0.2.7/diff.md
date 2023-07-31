# Comparing `tmp/hyload-0.2.6-py3-none-any.whl.zip` & `tmp/hyload-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 27493 bytes, number of entries: 17
--rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-19 05:41 hyload/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-25 10:57 hyload/cfg.py
--rw-rw-rw-  2.0 fat    19401 b- defN 23-Jul-23 00:11 hyload/httpclient.py
--rw-rw-rw-  2.0 fat     2627 b- defN 23-Jul-23 00:12 hyload/logger.py
--rw-rw-rw-  2.0 fat    11771 b- defN 23-Jul-23 23:50 hyload/stats.py
+Zip file size: 27559 bytes, number of entries: 17
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-31 00:52 hyload/__init__.py
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-31 01:21 hyload/cfg.py
+-rw-rw-rw-  2.0 fat    19401 b- defN 23-Jul-31 00:52 hyload/httpclient.py
+-rw-rw-rw-  2.0 fat     2627 b- defN 23-Jul-31 00:52 hyload/logger.py
+-rw-rw-rw-  2.0 fat    11771 b- defN 23-Jul-31 00:52 hyload/stats.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Jul-08 14:54 hyload/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-08 14:54 hyload/tools/__init__.py
 -rw-rw-rw-  2.0 fat     3667 b- defN 23-Jul-08 14:54 hyload/tools/plotperf.py
 -rw-rw-rw-  2.0 fat     2802 b- defN 23-Jul-08 14:54 hyload/tools/plotresource.py
 -rw-rw-rw-  2.0 fat    39521 b- defN 23-Jul-08 14:54 hyload/tools/puttyagents.py
--rw-rw-rw-  2.0 fat     4007 b- defN 23-Jul-21 06:07 hyload/tools/remoteop.py
+-rw-rw-rw-  2.0 fat     4303 b- defN 23-Jul-31 01:20 hyload/tools/remoteop.py
 -rw-rw-rw-  2.0 fat     7493 b- defN 23-Jul-14 12:12 hyload/tools/statshub.py
--rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1509 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-25 10:58 hyload-0.2.6.dist-info/RECORD
-17 files, 96475 bytes uncompressed, 25369 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1509 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-31 01:22 hyload-0.2.7.dist-info/RECORD
+17 files, 96771 bytes uncompressed, 25435 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: hyload/tools/remoteop.py
 Comment: 
 
 Filename: hyload/tools/statshub.py
 Comment: 
 
-Filename: hyload-0.2.6.dist-info/LICENSE.txt
+Filename: hyload-0.2.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hyload-0.2.6.dist-info/METADATA
+Filename: hyload-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: hyload-0.2.6.dist-info/WHEEL
+Filename: hyload-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: hyload-0.2.6.dist-info/top_level.txt
+Filename: hyload-0.2.7.dist-info/top_level.txt
 Comment: 
 
-Filename: hyload-0.2.6.dist-info/RECORD
+Filename: hyload-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyload/cfg.py

```diff
@@ -1 +1 @@
-Version = '0.2.6'
+Version = '0.2.7'
```

## hyload/tools/remoteop.py

```diff
@@ -147,8 +147,20 @@
     #     print ("\n!!uncompress tar file failed with 7z.exe, errCode = %s" % ret)
     #     return
     # else:
     #     print ('unpackage record file successfully.')
     # 
     # import subprocess
     # subprocess.Popen(rf'explorer "{localDir}"') 
-    
+    
+
+
+
+def  testSSHConnection_using_password(HOST,PORT,USER, PASSWD):
+    
+    ssh = paramiko.SSHClient()
+
+    ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+   
+    ssh.connect(HOST,PORT,username=USER, password=PASSWD, look_for_keys=False)
+     
+    print('* ssh login ok *')
```

## Comparing `hyload-0.2.6.dist-info/LICENSE.txt` & `hyload-0.2.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hyload-0.2.6.dist-info/METADATA` & `hyload-0.2.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyload
-Version: 0.2.6
+Version: 0.2.7
 Summary: Framework for load testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hyload
 Author: baiyueheiyu 白月黑羽
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hyload loadtesting
```

## Comparing `hyload-0.2.6.dist-info/RECORD` & `hyload-0.2.7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hyload/__init__.py,sha256=wXjdLCvcOlQV8a7Mku2cQbyWRXheGf7dGkHfjvBqKu8,171
-hyload/cfg.py,sha256=o9buJSZqLK87y7pzqM6v4uXwbX6dEUO6vdeGbsg4uBc,17
+hyload/cfg.py,sha256=GIdgtOLuSXpL0hEOWZyX4Nrxm6xhf1EIwSc8bGhSh3A,17
 hyload/httpclient.py,sha256=8fjF_T6i8q4Y1HEVKv97Qdn14SgdpqFBnDbup3RtAr4,19401
 hyload/logger.py,sha256=CfxUQM7oPiWuiuXmtiQiD5ViXkdY1t5yo8-SvRWO1q8,2627
 hyload/stats.py,sha256=1BCif-2OTVWEPvSMEIxY_WoJQ0v7I2WxJlkLAXDoIxA,11771
 hyload/util.py,sha256=lNKVVW4vYFueXcvOC4HoIMIiXFUz6skR9shSA7iPsWU,979
 hyload/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hyload/tools/plotperf.py,sha256=H1OszxmfgAYAxX4YEp-_aX66w6slynz9tjDGdpraMMo,3667
 hyload/tools/plotresource.py,sha256=9ydos2xFSA__ANhQ4b_fr5ORJPwWVLCgXoYnYdO5cA4,2802
 hyload/tools/puttyagents.py,sha256=NvL3VhYYka69kh7QTdRzjm7dLN3dB5MuU__K1GmGsW8,39521
-hyload/tools/remoteop.py,sha256=eJ7gSwJNzNIZfOU--5F_MNiy8laA9EBqIXtsuE83ZH8,4007
+hyload/tools/remoteop.py,sha256=IzpeYMIk-zmNGJD-U_h_N9bSD6FDHy87kH6zgKzg7rA,4303
 hyload/tools/statshub.py,sha256=bPyj9h6eewxRJSJmQpqtkx3DFbvoYbQsWpcFvATFang,7493
-hyload-0.2.6.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
-hyload-0.2.6.dist-info/METADATA,sha256=JwVE1kkckhxtR9Lqese-ClWYoZOAToF0ft_V2Onkkhw,1509
-hyload-0.2.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hyload-0.2.6.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
-hyload-0.2.6.dist-info/RECORD,,
+hyload-0.2.7.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
+hyload-0.2.7.dist-info/METADATA,sha256=K40sjgOlvHizeoVZ-IotBLXIfJ8c8H2zyxie7NQbZFQ,1509
+hyload-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hyload-0.2.7.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
+hyload-0.2.7.dist-info/RECORD,,
```

