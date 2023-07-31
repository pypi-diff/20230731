# Comparing `tmp/fyers_sdk-1.0.7.tar.gz` & `tmp/fyers_sdk-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-1.0.7.tar", last modified: Mon Jul 31 09:39:09 2023, max compression
+gzip compressed data, was "fyers_sdk-1.0.8.tar", last modified: Mon Jul 31 10:15:08 2023, max compression
```

## Comparing `fyers_sdk-1.0.7.tar` & `fyers_sdk-1.0.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 09:39:09.505196 fyers_sdk-1.0.7/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.7/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 09:39:09.505196 fyers_sdk-1.0.7/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.7/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 09:39:09.457197 fyers_sdk-1.0.7/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 09:39:09.505196 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58550 2023-07-31 07:03:59.000000 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.7/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-1.0.7/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.7/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 09:39:09.477197 fyers_sdk-1.0.7/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 09:39:09.000000 fyers_sdk-1.0.7/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 09:39:09.000000 fyers_sdk-1.0.7/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 09:39:09.000000 fyers_sdk-1.0.7/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 09:39:09.000000 fyers_sdk-1.0.7/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 09:39:09.000000 fyers_sdk-1.0.7/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 09:39:09.505196 fyers_sdk-1.0.7/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 09:38:57.000000 fyers_sdk-1.0.7/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:15:08.416310 fyers_sdk-1.0.8/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.8/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       54 2023-07-31 10:14:46.000000 fyers_sdk-1.0.8/MANIFEST.in
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:15:08.416310 fyers_sdk-1.0.8/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.8/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:15:08.392311 fyers_sdk-1.0.8/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:15:08.416310 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58550 2023-07-31 07:03:59.000000 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.8/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-1.0.8/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.8/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 10:15:08.412310 fyers_sdk-1.0.8/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 10:15:08.000000 fyers_sdk-1.0.8/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      458 2023-07-31 10:15:08.000000 fyers_sdk-1.0.8/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 10:15:08.000000 fyers_sdk-1.0.8/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 10:15:08.000000 fyers_sdk-1.0.8/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 10:15:08.000000 fyers_sdk-1.0.8/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 10:15:08.416310 fyers_sdk-1.0.8/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 10:14:54.000000 fyers_sdk-1.0.8/setup.py
```

### Comparing `fyers_sdk-1.0.7/LICENSE.txt` & `fyers_sdk-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/PKG-INFO` & `fyers_sdk-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.7/README.md` & `fyers_sdk-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/map.json` & `fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/map.json`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-1.0.8/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/fyersModel.py` & `fyers_sdk-1.0.8/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk/fyers_logger.py` & `fyers_sdk-1.0.8/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.7/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-1.0.8/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 1.0.7
+Version: 1.0.8
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.7/setup.py` & `fyers_sdk-1.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='1.0.7',
+     version='1.0.8',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

