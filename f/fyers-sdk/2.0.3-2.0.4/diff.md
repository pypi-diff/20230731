# Comparing `tmp/fyers_sdk-2.0.3.tar.gz` & `tmp/fyers_sdk-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.0.3.tar", last modified: Mon Jul 31 10:31:00 2023, max compression
+gzip compressed data, was "fyers_sdk-2.0.4.tar", last modified: Mon Jul 31 10:39:01 2023, max compression
```

## Comparing `fyers_sdk-2.0.3.tar` & `fyers_sdk-2.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:31:00.760362 fyers_sdk-2.0.3/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.0.3/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:31:00.760362 fyers_sdk-2.0.3/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.0.3/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:31:00.736362 fyers_sdk-2.0.3/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:31:00.760362 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58416 2023-07-31 10:30:39.000000 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 10:17:48.000000 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.0.3/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.0.3/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.0.3/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:31:00.756362 fyers_sdk-2.0.3/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:31:00.000000 fyers_sdk-2.0.3/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 10:31:00.000000 fyers_sdk-2.0.3/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 10:31:00.000000 fyers_sdk-2.0.3/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 10:31:00.000000 fyers_sdk-2.0.3/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 10:31:00.000000 fyers_sdk-2.0.3/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 10:31:00.760362 fyers_sdk-2.0.3/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 10:30:46.000000 fyers_sdk-2.0.3/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.0.4/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.0.4/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.187518 fyers_sdk-2.0.4/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58588 2023-07-31 10:36:58.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 10:17:48.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.0.4/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.0.4/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.0.4/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:39:01.207518 fyers_sdk-2.0.4/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 10:39:01.000000 fyers_sdk-2.0.4/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 10:39:01.211518 fyers_sdk-2.0.4/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 10:37:07.000000 fyers_sdk-2.0.4/setup.py
```

### Comparing `fyers_sdk-2.0.3/LICENSE.txt` & `fyers_sdk-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/PKG-INFO` & `fyers_sdk-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.0.3
+Version: 2.0.4
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.3/README.md` & `fyers_sdk-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import base64
 import logging
 import threading
 import time
+from pkg_resources import resource_filename
 import requests
 import urllib.parse
 import websocket
 from threading import Thread
 import struct
 from fyers_sdk.FyersWebsocket import defines
 import json
@@ -69,15 +70,16 @@
                     "Authorization": self.access_token,
                     "Content-Type": "application/json",
                 },
             )
             quote_data =response.json()
             datadict = {}
             values = {}
-            with open("FyersWebsocket/map.json", "r") as file:
+            file_path = resource_filename('fyers_sdk.FyersWebsocket', 'map.json')
+            with open(file_path, "r") as file:
                 # Load the JSON data into a Python object
                 mapper = json.load(file)
             index_dict = mapper["index_dict"]
             exch_seg_dict = mapper["exch_seg_dict"]
             wrong_symbol = []
             if "d" in quote_data:
                 for data in quote_data["d"]:
@@ -219,16 +221,17 @@
         else:
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
                 logger_handler=logging.FileHandler("fyersSocket.log"),
             )
+        file_path = resource_filename('fyers_sdk.FyersWebsocket', 'map.json')
 
-        with open("FyersWebsocket/map.json", "r") as file:
+        with open(file_path, "r") as file:
             # Imported json file
             mapper = json.load(file)
 
         self.data_val = mapper["data_val"]
         self.index_val = mapper["index_val"]
         self.lite_val = mapper["lite_val"]
         self.depthvalue = mapper["depthvalue"]
```

### Comparing `fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.0.4/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk/fyersModel.py` & `fyers_sdk-2.0.4/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.0.4/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.0.3/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.0.4/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.0.3
+Version: 2.0.4
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.0.3/setup.py` & `fyers_sdk-2.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.0.3',
+     version='2.0.4',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

