# Comparing `tmp/agora_config-1.1.37-py2.py3-none-any.whl.zip` & `tmp/agora_config-1.1.38-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 8009 bytes, number of entries: 13
+Zip file size: 8008 bytes, number of entries: 13
 -rw-r--r--  2.0 fat      105 b- defN 23-May-12 13:38 agora_config/__init__.py
 -rw-r--r--  2.0 fat     5994 b- defN 23-Jun-30 14:21 agora_config/agora_config.py
 -rw-r--r--  2.0 fat      540 b- defN 23-May-12 13:38 agora_config/command_line_provider.py
 -rw-r--r--  2.0 fat     2283 b- defN 23-May-12 13:38 agora_config/dict_of_dict.py
 -rw-r--r--  2.0 fat      410 b- defN 23-May-12 13:38 agora_config/environment_variable_provider.py
 -rw-r--r--  2.0 fat     3164 b- defN 23-May-12 13:38 agora_config/file_key_provider.py
 -rw-r--r--  2.0 fat     1974 b- defN 23-May-18 11:05 agora_config/file_provider.py
 -rw-r--r--  2.0 fat      550 b- defN 23-May-12 13:38 agora_config/last_value_callbacks.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-31 12:21 agora_config/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.37.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.37.dist-info/WHEEL
--rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.37.dist-info/METADATA
--rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.37.dist-info/RECORD
-13 files, 18232 bytes uncompressed, 6141 bytes compressed:  66.3%
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-31 12:58 agora_config/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.38.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.38.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.38.dist-info/METADATA
+-rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.38.dist-info/RECORD
+13 files, 18232 bytes uncompressed, 6140 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: agora_config/last_value_callbacks.py
 Comment: 
 
 Filename: agora_config/version.py
 Comment: 
 
-Filename: agora_config-1.1.37.dist-info/LICENSE
+Filename: agora_config-1.1.38.dist-info/LICENSE
 Comment: 
 
-Filename: agora_config-1.1.37.dist-info/WHEEL
+Filename: agora_config-1.1.38.dist-info/WHEEL
 Comment: 
 
-Filename: agora_config-1.1.37.dist-info/METADATA
+Filename: agora_config-1.1.38.dist-info/METADATA
 Comment: 
 
-Filename: agora_config-1.1.37.dist-info/RECORD
+Filename: agora_config-1.1.38.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_config/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.37'
+__version__ = '1.1.38'
```

## Comparing `agora_config-1.1.37.dist-info/METADATA` & `agora_config-1.1.38.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: agora_config
-Version: 1.1.37
+Version: 1.1.38
 Summary: Configuration libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.37
+Requires-Dist: agora_logging == 1.1.38
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_config
 
 This package is the Configuration library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
```

## Comparing `agora_config-1.1.37.dist-info/RECORD` & `agora_config-1.1.38.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 agora_config/agora_config.py,sha256=dOmvUDU6BGF6uqeXpRbomKV9eeDz3OvrH0oR9QBKrgs,5994
 agora_config/command_line_provider.py,sha256=TivZe91P_K6FbGbRtZpl9es_cNi2EmTeZBvp4cwW37I,540
 agora_config/dict_of_dict.py,sha256=aSN3xpEAWCXSO6elkVbn9IJ1hNzJAp6c7gQMHIwPKlg,2283
 agora_config/environment_variable_provider.py,sha256=K-zWy9radHQK2zR2paPWE9pA-yAZkgCmCaHx7AyKRbY,410
 agora_config/file_key_provider.py,sha256=NJH4M9sF3zhxZiMbaWQGP2HpSQxps2S0_eoFrHXTdqg,3164
 agora_config/file_provider.py,sha256=-NoYILq7yjhCkImY6k0Izs7HSPe6WSoqb9wlqIa3FKk,1974
 agora_config/last_value_callbacks.py,sha256=3linM0LqWB92D0gFn0_YX0m1B7otSQ22sMv49uiBABw,550
-agora_config/version.py,sha256=wzQumjbBZLB6HKa1UYl1fLkDW0jP3nh0f7OOTqs5o6s,25
-agora_config-1.1.37.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_config-1.1.37.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_config-1.1.37.dist-info/METADATA,sha256=41cy74e3IrrJND705IeapcTAuEyzD6eFKMMuhe1oXGY,1847
-agora_config-1.1.37.dist-info/RECORD,,
+agora_config/version.py,sha256=BPlAo_MDT13g-sG5NVbqsmNEMiY3Bh651OBWao0zlPU,25
+agora_config-1.1.38.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_config-1.1.38.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_config-1.1.38.dist-info/METADATA,sha256=euwxPZN-FE8I3vmGu6FtyzGm_vympEgBM6_3QY5ny34,1847
+agora_config-1.1.38.dist-info/RECORD,,
```

