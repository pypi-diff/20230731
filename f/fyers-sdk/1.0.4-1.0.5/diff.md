# Comparing `tmp/fyers_sdk-1.0.4.tar.gz` & `tmp/fyers_sdk-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-1.0.4.tar", last modified: Mon Jul 31 06:47:19 2023, max compression
+gzip compressed data, was "fyers_sdk-1.0.5.tar", last modified: Mon Jul 31 07:01:36 2023, max compression
```

## Comparing `fyers_sdk-1.0.4.tar` & `fyers_sdk-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:47:19.486189 fyers_sdk-1.0.4/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.4/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:47:19.486189 fyers_sdk-1.0.4/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.4/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:47:19.462189 fyers_sdk-1.0.4/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:47:19.486189 fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.4/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.4/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.4/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:47:19.482189 fyers_sdk-1.0.4/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:47:19.000000 fyers_sdk-1.0.4/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      412 2023-07-31 06:47:19.000000 fyers_sdk-1.0.4/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 06:47:19.000000 fyers_sdk-1.0.4/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 06:47:19.000000 fyers_sdk-1.0.4/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 06:47:19.000000 fyers_sdk-1.0.4/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 06:47:19.486189 fyers_sdk-1.0.4/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 06:47:16.000000 fyers_sdk-1.0.4/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.5/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.5/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.327673 fyers_sdk-1.0.5/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     7442 2023-07-28 07:06:27.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.5/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.5/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.5/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 07:01:36.347674 fyers_sdk-1.0.5/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 07:01:36.000000 fyers_sdk-1.0.5/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 07:01:36.359674 fyers_sdk-1.0.5/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1030 2023-07-31 07:01:13.000000 fyers_sdk-1.0.5/setup.py
```

### Comparing `fyers_sdk-1.0.4/LICENSE.txt` & `fyers_sdk-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/PKG-INFO` & `fyers_sdk-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.4/README.md` & `fyers_sdk-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-1.0.5/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk/fyersModel.py` & `fyers_sdk-1.0.5/fyers_sdk/fyersModel.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk/fyers_logger.py` & `fyers_sdk-1.0.5/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-1.0.4/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-1.0.5/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 1.0.4
+Version: 1.0.5
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-1.0.4/setup.py` & `fyers_sdk-1.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='1.0.4',
+     version='1.0.5',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
      package_data={  
-         'fyerstest': ['/home/vinay/Documents/API-V3/apiv2-with-HSM/fyers-api-py/fyers_sdk/FyersWebsocket/map.json']
+         'fyers_sdk': ['/home/vinay/Documents/API-V3/apiv2-with-HSM/fyers-api-py/fyers_sdk/FyersWebsocket/map.json']
      },
      include_package_data=True,
      install_requires=[
                 'requests==2.31.0',
                 'asyncio==3.4.3',
                 'aiohttp==3.8.4',
                 'aws_lambda_powertools==1.25.5',
```

