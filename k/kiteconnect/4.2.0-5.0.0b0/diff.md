# Comparing `tmp/kiteconnect-4.2.0.tar.gz` & `tmp/kiteconnect-5.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiteconnect-4.2.0.tar", last modified: Mon Jan  9 08:19:16 2023, max compression
+gzip compressed data, was "kiteconnect-5.0.0b0.tar", last modified: Mon Jul 31 10:39:29 2023, max compression
```

## Comparing `kiteconnect-4.2.0.tar` & `kiteconnect-5.0.0b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:19:16.647333 kiteconnect-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-01-09 08:19:16.647333 kiteconnect-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6103 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:19:16.647333 kiteconnect-4.2.0/kiteconnect/
--rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/kiteconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/kiteconnect/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36086 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/kiteconnect/connect.py
--rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/kiteconnect/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    32586 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/kiteconnect/ticker.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-09 08:19:16.647333 kiteconnect-4.2.0/kiteconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7181 2023-01-09 08:19:16.000000 kiteconnect-4.2.0/kiteconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      332 2023-01-09 08:19:16.000000 kiteconnect-4.2.0/kiteconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-09 08:19:16.000000 kiteconnect-4.2.0/kiteconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-01-09 08:19:16.000000 kiteconnect-4.2.0/kiteconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-01-09 08:19:16.000000 kiteconnect-4.2.0/kiteconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-01-09 08:19:16.647333 kiteconnect-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1920 2023-01-09 08:18:58.000000 kiteconnect-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 10:39:29.912924 kiteconnect-5.0.0b0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     7736 2023-07-31 10:39:29.912924 kiteconnect-5.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6706 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 10:39:29.912924 kiteconnect-5.0.0b0/kiteconnect/
+-rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/kiteconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/kiteconnect/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36468 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/kiteconnect/connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2574 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/kiteconnect/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32586 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/kiteconnect/ticker.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 10:39:29.912924 kiteconnect-5.0.0b0/kiteconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7736 2023-07-31 10:39:29.000000 kiteconnect-5.0.0b0/kiteconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-07-31 10:39:29.000000 kiteconnect-5.0.0b0/kiteconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 10:39:29.000000 kiteconnect-5.0.0b0/kiteconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-07-31 10:39:29.000000 kiteconnect-5.0.0b0/kiteconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-31 10:39:29.000000 kiteconnect-5.0.0b0/kiteconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-31 10:39:29.912924 kiteconnect-5.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-07-31 10:39:01.000000 kiteconnect-5.0.0b0/setup.py
```

### Comparing `kiteconnect-4.2.0/LICENSE` & `kiteconnect-5.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiteconnect-4.2.0/PKG-INFO` & `kiteconnect-5.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: kiteconnect
-Version: 4.2.0
+Version: 5.0.0b0
 Summary: The official Python client for the Kite Connect trading API
 Home-page: https://kite.trade
 Download-URL: https://github.com/zerodhatech/pykiteconnect
 Author: Zerodha Technology Pvt. Ltd. (India)
 Author-email: talk@zerodha.tech
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
@@ -40,16 +39,22 @@
 ## Documentation
 
 - [Python client documentation](https://kite.trade/docs/pykiteconnect/v4)
 - [Kite Connect HTTP API documentation](https://kite.trade/docs/connect/v3)
 
 ## v4 - Breaking changes
 
-* Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
-* Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+- Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
+- Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+
+## v5 - Breaking changes
+
+- **Drop Support for Python 2.7**: Starting from version v5, support for Python 2.7 has been discontinued. This decision was made due to the [announcement](https://github.com/actions/setup-python/issues/672) by `setup-python`, which stopped supporting Python 2.x since May 2023.
+
+- **For Python 2.x Users**: If you are using Python 2.x, you can continue using the `kiteconnect` library, but please stick to the <= 4.x.x versions of the library. You can find the previous releases on the [PyKiteConnect GitHub Releases](https://github.com/zerodha/pykiteconnect/releases) page.
 
 ## Installing the client
 
 You can install the pre release via pip
 
 ```
 pip install --upgrade kiteconnect
```

### Comparing `kiteconnect-4.2.0/README.md` & `kiteconnect-5.0.0b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,22 @@
 ## Documentation
 
 - [Python client documentation](https://kite.trade/docs/pykiteconnect/v4)
 - [Kite Connect HTTP API documentation](https://kite.trade/docs/connect/v3)
 
 ## v4 - Breaking changes
 
-* Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
-* Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+- Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
+- Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+
+## v5 - Breaking changes
+
+- **Drop Support for Python 2.7**: Starting from version v5, support for Python 2.7 has been discontinued. This decision was made due to the [announcement](https://github.com/actions/setup-python/issues/672) by `setup-python`, which stopped supporting Python 2.x since May 2023.
+
+- **For Python 2.x Users**: If you are using Python 2.x, you can continue using the `kiteconnect` library, but please stick to the <= 4.x.x versions of the library. You can find the previous releases on the [PyKiteConnect GitHub Releases](https://github.com/zerodha/pykiteconnect/releases) page.
 
 ## Installing the client
 
 You can install the pre release via pip
 
 ```
 pip install --upgrade kiteconnect
```

### Comparing `kiteconnect-4.2.0/kiteconnect/__init__.py` & `kiteconnect-5.0.0b0/kiteconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `kiteconnect-4.2.0/kiteconnect/connect.py` & `kiteconnect-5.0.0b0/kiteconnect/connect.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,16 @@
         "gtt.place": "/gtt/triggers",
         "gtt.info": "/gtt/triggers/{trigger_id}",
         "gtt.modify": "/gtt/triggers/{trigger_id}",
         "gtt.delete": "/gtt/triggers/{trigger_id}",
 
         # Margin computation endpoints
         "order.margins": "/margins/orders",
-        "order.margins.basket": "/margins/basket"
+        "order.margins.basket": "/margins/basket",
+        "order.contract_note": "/charges/orders",
     }
 
     def __init__(self,
                  api_key,
                  access_token=None,
                  root=None,
                  debug=False,
@@ -782,14 +783,23 @@
         - `mode` is margin response mode type. compact - Compact mode will only give the total margins
         """
         return self._post("order.margins.basket",
                           params=params,
                           is_json=True,
                           query_params={'consider_positions': consider_positions, 'mode': mode})
 
+    def get_virtual_contract_note(self, params):
+        """
+        Calculates detailed charges order-wise for the order book
+        - `params` is list of orders to fetch charges detail
+        """
+        return self._post("order.contract_note",
+                          params=params,
+                          is_json=True)
+
     def _warn(self, message):
         """ Add deprecation warning message """
         warnings.simplefilter('always', DeprecationWarning)
         warnings.warn(message, DeprecationWarning)
 
     def _parse_instruments(self, data):
         # decode to string for Python 3
```

### Comparing `kiteconnect-4.2.0/kiteconnect/exceptions.py` & `kiteconnect-5.0.0b0/kiteconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `kiteconnect-4.2.0/kiteconnect/ticker.py` & `kiteconnect-5.0.0b0/kiteconnect/ticker.py`

 * *Files identical despite different names*

### Comparing `kiteconnect-4.2.0/kiteconnect.egg-info/PKG-INFO` & `kiteconnect-5.0.0b0/kiteconnect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: kiteconnect
-Version: 4.2.0
+Version: 5.0.0b0
 Summary: The official Python client for the Kite Connect trading API
 Home-page: https://kite.trade
 Download-URL: https://github.com/zerodhatech/pykiteconnect
 Author: Zerodha Technology Pvt. Ltd. (India)
 Author-email: talk@zerodha.tech
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Programming Language :: Python
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
@@ -40,16 +39,22 @@
 ## Documentation
 
 - [Python client documentation](https://kite.trade/docs/pykiteconnect/v4)
 - [Kite Connect HTTP API documentation](https://kite.trade/docs/connect/v3)
 
 ## v4 - Breaking changes
 
-* Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
-* Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+- Renamed ticker fields as per [kite connect doc](https://kite.trade/docs/connect/v3/websocket/#quote-packet-structure)
+- Renamed `bsecds` to `bcd` in `ticker.EXCHANGE_MAP`
+
+## v5 - Breaking changes
+
+- **Drop Support for Python 2.7**: Starting from version v5, support for Python 2.7 has been discontinued. This decision was made due to the [announcement](https://github.com/actions/setup-python/issues/672) by `setup-python`, which stopped supporting Python 2.x since May 2023.
+
+- **For Python 2.x Users**: If you are using Python 2.x, you can continue using the `kiteconnect` library, but please stick to the <= 4.x.x versions of the library. You can find the previous releases on the [PyKiteConnect GitHub Releases](https://github.com/zerodha/pykiteconnect/releases) page.
 
 ## Installing the client
 
 You can install the pre release via pip
 
 ```
 pip install --upgrade kiteconnect
```

### Comparing `kiteconnect-4.2.0/setup.py` & `kiteconnect-5.0.0b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Programming Language :: Python",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Topic :: Office/Business :: Financial :: Investment",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries"
     ],
```

