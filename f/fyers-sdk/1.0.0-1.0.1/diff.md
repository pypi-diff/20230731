# Comparing `tmp/fyers_sdk-1.0.0.tar.gz` & `tmp/fyers_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-1.0.0.tar", last modified: Mon Jul 31 06:14:46 2023, max compression
+gzip compressed data, was "fyers_sdk-1.0.1.tar", last modified: Mon Jul 31 06:39:44 2023, max compression
```

## Comparing `fyers_sdk-1.0.0.tar` & `fyers_sdk-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.0/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.0/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.188823 fyers_sdk-1.0.0/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.0/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.0/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.0/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.208823 fyers_sdk-1.0.0/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      412 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      851 2023-07-31 06:12:49.000000 fyers_sdk-1.0.0/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:39:44.182392 fyers_sdk-1.0.1/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.1/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:39:44.182392 fyers_sdk-1.0.1/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.1/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:39:44.154392 fyers_sdk-1.0.1/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:39:44.178392 fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.1/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.1/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.1/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:39:44.178392 fyers_sdk-1.0.1/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:39:44.000000 fyers_sdk-1.0.1/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      412 2023-07-31 06:39:44.000000 fyers_sdk-1.0.1/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 06:39:44.000000 fyers_sdk-1.0.1/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 06:39:44.000000 fyers_sdk-1.0.1/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 06:39:44.000000 fyers_sdk-1.0.1/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 06:39:44.182392 fyers_sdk-1.0.1/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      941 2023-07-31 06:39:41.000000 fyers_sdk-1.0.1/setup.py
```

### Comparing `fyers_sdk-1.0.0/LICENSE.txt` & `fyers_sdk-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/PKG-INFO` & `fyers_sdk-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.0/README.md` & `fyers_sdk-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-1.0.1/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk/fyersModel.py` & `fyers_sdk-1.0.1/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk/fyers_logger.py` & `fyers_sdk-1.0.1/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.0/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-1.0.1/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

