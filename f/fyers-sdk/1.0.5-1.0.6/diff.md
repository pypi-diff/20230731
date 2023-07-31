# Comparing `tmp/fyers_sdk-1.0.5.tar.gz` & `tmp/fyers_sdk-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-1.0.5.tar", last modified: Mon Jul 31 07:01:36 2023, max compression
+gzip compressed data, was "fyers_sdk-1.0.6.tar", last modified: Mon Jul 31 07:04:12 2023, max compression
```

## Comparing `fyers_sdk-1.0.5.tar` & `fyers_sdk-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.5/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.5/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.327673 fyers_sdk-1.0.5/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.5/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.5/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.5/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.347674 fyers_sdk-1.0.5/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 07:01:13.000000 fyers_sdk-1.0.5/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:04:12.326667 fyers_sdk-1.0.6/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.6/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:04:12.326667 fyers_sdk-1.0.6/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.6/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:04:12.298667 fyers_sdk-1.0.6/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:04:12.326667 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58550 2023-07-31 07:03:59.000000 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.6/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.6/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.6/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:04:12.322667 fyers_sdk-1.0.6/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:04:12.000000 fyers_sdk-1.0.6/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 07:04:12.000000 fyers_sdk-1.0.6/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 07:04:12.000000 fyers_sdk-1.0.6/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 07:04:12.000000 fyers_sdk-1.0.6/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 07:04:12.000000 fyers_sdk-1.0.6/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 07:04:12.326667 fyers_sdk-1.0.6/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 07:04:09.000000 fyers_sdk-1.0.6/setup.py
```

### Comparing `fyers_sdk-1.0.5/LICENSE.txt` & `fyers_sdk-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/PKG-INFO` & `fyers_sdk-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.5/README.md` & `fyers_sdk-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                     "Authorization": self.access_token,
                     "Content-Type": "application/json",
                 },
             )
             quote_data =response.json()
             datadict = {}
             values = {}
-            with open("fyers_sdk/FyersWebsocket/map.json", "r") as file:
+            with open("/home/vinay/Documents/API-V3/apiv2-with-HSM/fyers-api-py/fyers_sdk/FyersWebsocket/map.json", "r") as file:
                 # Load the JSON data into a Python object
                 mapper = json.load(file)
             index_dict = mapper["index_dict"]
             exch_seg_dict = mapper["exch_seg_dict"]
             wrong_symbol = []
             if "d" in quote_data:
                 for data in quote_data["d"]:
@@ -220,15 +220,15 @@
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
                 logger_handler=logging.FileHandler("fyersSocket.log"),
             )
 
-        with open("fyers_sdk/FyersWebsocket/map.json", "r") as file:
+        with open("/home/vinay/Documents/API-V3/apiv2-with-HSM/fyers-api-py/fyers_sdk/FyersWebsocket/map.json", "r") as file:
             # Imported json file
             mapper = json.load(file)
 
         self.data_val = mapper["data_val"]
         self.index_val = mapper["index_val"]
         self.lite_val = mapper["lite_val"]
         self.depthvalue = mapper["depthvalue"]
```

### Comparing `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-1.0.6/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk/fyersModel.py` & `fyers_sdk-1.0.6/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk/fyers_logger.py` & `fyers_sdk-1.0.6/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.5/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-1.0.6/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 1.0.5
+Version: 1.0.6
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.5/setup.py` & `fyers_sdk-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='1.0.5',
+     version='1.0.6',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

