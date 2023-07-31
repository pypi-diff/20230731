# Comparing `tmp/flxtrd-0.2.3.tar.gz` & `tmp/flxtrd-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.2.3.tar", max compression
+gzip compressed data, was "flxtrd-0.2.4.tar", max compression
```

## Comparing `flxtrd-0.2.3.tar` & `flxtrd-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.3/LICENSE
--rw-r--r--   0        0        0     8976 2023-07-04 11:25:04.503836 flxtrd-0.2.3/README.md
--rw-r--r--   0        0        0     2211 2023-07-04 11:25:29.191836 flxtrd-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     7470 2023-07-04 06:14:54.745883 flxtrd-0.2.3/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      580 2023-07-04 11:24:10.475838 flxtrd-0.2.3/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.3/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.3/src/flxtrd/core/types.py
--rw-r--r--   0        0        0     1581 2023-07-04 11:25:18.687836 flxtrd-0.2.3/src/flxtrd/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0    10763 2023-07-04 06:17:45.849878 flxtrd-0.2.3/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.3/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     9718 1970-01-01 00:00:00.000000 flxtrd-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.4/LICENSE
+-rw-r--r--   0        0        0     8726 2023-07-04 12:36:56.071698 flxtrd-0.2.4/README.md
+-rw-r--r--   0        0        0     2211 2023-07-31 11:11:53.329826 flxtrd-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     7470 2023-07-04 06:14:54.745883 flxtrd-0.2.4/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-07-04 11:24:10.475838 flxtrd-0.2.4/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.4/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.4/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     1788 2023-07-31 07:51:31.956598 flxtrd-0.2.4/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10790 2023-07-31 11:10:01.081832 flxtrd-0.2.4/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     9468 1970-01-01 00:00:00.000000 flxtrd-0.2.4/PKG-INFO
```

### Comparing `flxtrd-0.2.3/LICENSE` & `flxtrd-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/README.md` & `flxtrd-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,40 +39,20 @@
     MyClient --> CustomPlugins
     FlexAPIClient --> APIProtocols
     FlexAPIClient --> FlexPlugins
 ```
 
 ## Quickstart Guide
 
-Create virtual environment
-
-```sh
-python3 -m venv venv
-```
-
-Activate virtual environment
-
-```sh
-source venv/bin/activate
-```
-
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
 
-Update GLocalFlexTrade Python package to latest version
-
-```sh
-pip install --upgrade flxtrd
-# or
-pip install -U flxtrd
-```
-
 ### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
 from logging import ERROR, INFO
 import sys
```

### Comparing `flxtrd-0.2.3/pyproject.toml` & `flxtrd-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.2.3"
+version = "0.2.4"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
```

### Comparing `flxtrd-0.2.3/src/flxtrd/__init__.py` & `flxtrd-0.2.4/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/api_client.py` & `flxtrd-0.2.4/src/flxtrd/core/api_client.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/logger.py` & `flxtrd-0.2.4/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.2.4/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.2.4/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/types.py` & `flxtrd-0.2.4/src/flxtrd/core/types.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/src/flxtrd/core/utils.py` & `flxtrd-0.2.4/src/flxtrd/core/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,52 +14,57 @@
     """
 
     dt = datetime.fromtimestamp(milliseconds / MILLI, tz=timezone.utc)
     return dt.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
 
 
 def seconds_to_min(seconds: int):
+    """Convert seconds to minutes"""
     if seconds == 0:
         log(ERROR, "Duration is zero")
         return 0
     return round(seconds / 60)
 
 
 def milliseconds_to_min(seconds: int):
+    """Convert milliseconds to minutes"""
     if seconds == 0:
         log(ERROR, "Duration is zero")
         return 0
     return round(seconds / 60 / MILLI)
 
 
 def utc_timestamp_ms() -> float:
-    # Get current UTC timestamp in seconds
+    """ Get current UTC timestamp in milliseconds"""
     timestamp = datetime.now(tz=timezone.utc).timestamp()
     # Convert seconds to milliseconds
     return int(timestamp * MILLI)
 
 
 def utc_timestamp_s() -> float:
-    # Get current UTC timestamp in seconds
+    """Get current UTC timestamp in seconds"""
     timestamp = datetime.now(tz=timezone.utc).timestamp()
     return int(timestamp)
 
 
 def min_to_ms(minutes: int):
+    """Convert minutes to milliseconds"""
     if minutes == 0:
         log(ERROR, "Minutes can not be zero")
         return 0
     return minutes * 60 * 1000
 
 
 def min_to_hour(minutes: int):
+    """Convert minutes to hours"""
     if minutes == 0:
         log(ERROR, "Minutes can not be zero")
         return 0
     return minutes / 60
 
 
 def min_to_s(minutes: int):
+    """Convert minutes to seconds"""
     if minutes == 0:
         log(ERROR, "Minutes can not be zero")
         return 0
     return minutes * 60
```

### Comparing `flxtrd-0.2.3/src/flxtrd/protocols/ampq.py` & `flxtrd-0.2.4/src/flxtrd/protocols/ampq.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     FlexBroker,
     FlexError,
     FlexMarket,
     FlexResource,
     FlexUser,
     MarketOrder,
     OrderType,
+    utils
 )
 from flxtrd.protocols.base import BaseAPI
 
 
 def create_line_message(user: FlexUser, flexibility: FlexResource, marketOrder: MarketOrder):
     """Create a line protocol message for InfluxDB that is the payload in the AMQP message
 
@@ -38,15 +39,15 @@
         pricename = "biddingprice"
     else:
         raise FlexError(f"Order type {marketOrder.order_type} not supported")
 
     order_type = marketOrder.order_type
     application_key = user.app_key
     wattage = flexibility.power_w
-    duration = flexibility.duration_min
+    duration = utils.min_to_ms(flexibility.duration_min)
     starttime = flexibility.start_time_epoch_ms
     totalenergy = flexibility.energy_wh
     orderprice = marketOrder.price_eur
     expirationtime = flexibility.expiration_time_epoch_ms
 
     lineordermsg = (
         f"{order_type.value},"
```

### Comparing `flxtrd-0.2.3/src/flxtrd/protocols/restapi.py` & `flxtrd-0.2.4/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.3/PKG-INFO` & `flxtrd-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.2.3
+Version: 0.2.4
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,40 +57,20 @@
     MyClient --> CustomPlugins
     FlexAPIClient --> APIProtocols
     FlexAPIClient --> FlexPlugins
 ```
 
 ## Quickstart Guide
 
-Create virtual environment
-
-```sh
-python3 -m venv venv
-```
-
-Activate virtual environment
-
-```sh
-source venv/bin/activate
-```
-
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
 
-Update GLocalFlexTrade Python package to latest version
-
-```sh
-pip install --upgrade flxtrd
-# or
-pip install -U flxtrd
-```
-
 ### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
 from logging import ERROR, INFO
 import sys
```

