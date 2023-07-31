# Comparing `tmp/zerocap_api_new_test-0.1.5.tar.gz` & `tmp/zerocap_api_new_test-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zerocap_api_new_test-0.1.5.tar", last modified: Mon Jul 31 02:24:53 2023, max compression
+gzip compressed data, was "dist\zerocap_api_new_test-0.1.6.tar", last modified: Mon Jul 31 02:28:27 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.5.tar` & `zerocap_api_new_test-0.1.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/
--rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    18303 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-07-31 02:24:49.000000 zerocap_api_new_test-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/
--rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/__init__.py
--rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/
--rw-rw-rw-   0        0        0    18303 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 02:24:53.000000 zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/
+-rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    19529 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2133 2023-07-31 02:28:20.000000 zerocap_api_new_test-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/
+-rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/__init__.py
+-rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/
+-rw-rw-rw-   0        0        0    19529 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.5/LICENSE.txt` & `zerocap_api_new_test-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.5/PKG-INFO` & `zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap_api_new_test
-Version: 0.1.5
+Name: zerocap-api-new-test
+Version: 0.1.6
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -209,15 +209,42 @@
 | id            | true     | string    | Transaction ID |             |
 
 
 响应例子:
 
 ```
 
-{}
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
 
 ```
 
 
 #### 3. Batch fetch order
 <!--post https://dma-api.defi.wiki/orders/fetch_orders-->
 
@@ -280,15 +307,42 @@
 
 
 
 响应例子:
 
 ```
 
-{}
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
 
 ```
 
 
 
 ## <span id='test'>websocket</span>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.6 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -53,33 +53,47 @@
 ID | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "account_vault":
 { "third_identity_id": "918d7125916c13191f3674e", "api_key": "***",
 "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®: |
 Parameter | required | data type | describe | Value range | |---------------|--
 --------|-----------|----------------|-------------| | id | true | string |
-Transaction ID | | ååºä¾å­: ``` {} ``` #### 3. Batch fetch order  ```
-result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time()
-* 1000 - 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type
-| describe | Value range | |----------------|----------|-----------|-----------
-------|-------------| | symbol | true | string | symbol | | | start_datetime |
+Transaction ID | | ååºä¾å­: ``` { "order_list": [ { "id": "476b0262-8689-
+4bc4-b5ff-380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-
+cd37310a55da", "datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
+"last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
+AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
+"average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
+"transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
+3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
+client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
+86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
+describe | Value range | |----------------|----------|-----------|-------------
+----|-------------| | symbol | true | string | symbol | | | start_datetime |
 true | string | start_datetime | | | end_datetime | true | string |
 end_datetime | | | page | true | string | page | | | limit | true | string |
 limit | | | ids | true | string | Transaction ids | | | status | true | string
 | status | | | sort_order | true | string | sort_order | | | order_type | true
 | string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
 Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` ## websocket ``` from zerocap_api_new_test import
+ååºä¾å­: ``` { "order_list": [ { "id": "476b0262-8689-4bc4-b5ff-
+380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+"datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
+"last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
+AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
+"average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
+"transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
+3864, "page": "1" } ``` ## websocket ``` from zerocap_api_new_test import
 ZerocapWebsocketClient # API key and secret required, èç³»zerocapè¿è¡æ³¨å
 apiKey = "***" apiSecret = "***" signature = hmac.new(apiSecret.encode("utf-
 8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest() ``` #### 1. Subscribe
 to Market data  ``` market_connect = websocket.get_market() while True: # Get
 messages message = websocket.get_message(market_connect) print(f"Receiving
 message from server: \n{message}") ``` è¯·æ±åæ°: | Parameter | required |
 data type | describe | Value range | |---------------|----------|-----------|--
```

### Comparing `zerocap_api_new_test-0.1.5/README.rst` & `zerocap_api_new_test-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.5/setup.py` & `zerocap_api_new_test-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 setup(
     name='zerocap_api_new_test',  # 包名
-    version='0.1.5',  # 版本号
+    version='0.1.6',  # 版本号
     description='zerocap_api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zerocap',
     author_email='jiayu.gao@eigen.capital',
     url='https://zerocap.com/',
     install_requires=REQUIRED,
```

### Comparing `zerocap_api_new_test-0.1.5/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.6/zerocap_api_new_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.5/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap-api-new-test
-Version: 0.1.5
+Name: zerocap_api_new_test
+Version: 0.1.6
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -209,15 +209,42 @@
 | id            | true     | string    | Transaction ID |             |
 
 
 响应例子:
 
 ```
 
-{}
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
 
 ```
 
 
 #### 3. Batch fetch order
 <!--post https://dma-api.defi.wiki/orders/fetch_orders-->
 
@@ -280,15 +307,42 @@
 
 
 
 响应例子:
 
 ```
 
-{}
+{
+	"order_list": [
+		{
+			"id": "476b0262-8689-4bc4-b5ff-380bb4ccc5e1",
+			"client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+			"datatime": "2023-07-31 02:12:23",
+			"timestamp": "1690516007000",
+			"last_trade_timestamp": "1690516007000",
+			"status": "rejected",
+			"symbol": "USDT/AUD",
+			"type": "market",
+			"time_in_force": "FOK",
+			"side": "buy",
+			"price": "1000",
+			"average": "",
+			"amount": "1000",
+			"filled": "",
+			"remaining": "",
+			"cost": "",
+			"transfer_id": "",
+			"fee": "",
+			"trades": []
+		}
+	],
+	"status": "success",
+	"total": 3864,
+	"page": "1"
+}
 
 ```
 
 
 
 ## <span id='test'>websocket</span>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.5 Summary:
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.6 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
@@ -53,33 +53,47 @@
 ID | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "id": "16ef58d1-677e-489c-8fe0-5acc4a680b6e", "account_vault":
 { "third_identity_id": "918d7125916c13191f3674e", "api_key": "***",
 "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®: |
 Parameter | required | data type | describe | Value range | |---------------|--
 --------|-----------|----------------|-------------| | id | true | string |
-Transaction ID | | ååºä¾å­: ``` {} ``` #### 3. Batch fetch order  ```
-result = client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time()
-* 1000 - 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type
-| describe | Value range | |----------------|----------|-----------|-----------
-------|-------------| | symbol | true | string | symbol | | | start_datetime |
+Transaction ID | | ååºä¾å­: ``` { "order_list": [ { "id": "476b0262-8689-
+4bc4-b5ff-380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-
+cd37310a55da", "datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
+"last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
+AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
+"average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
+"transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
+3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
+client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
+86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
+describe | Value range | |----------------|----------|-----------|-------------
+----|-------------| | symbol | true | string | symbol | | | start_datetime |
 true | string | start_datetime | | | end_datetime | true | string |
 end_datetime | | | page | true | string | page | | | limit | true | string |
 limit | | | ids | true | string | Transaction ids | | | status | true | string
 | status | | | sort_order | true | string | sort_order | | | order_type | true
 | string | order_type | | | side | true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
 Transaction ID | | | account_vault | true | json | accountVault | |
-ååºä¾å­: ``` {} ``` ## websocket ``` from zerocap_api_new_test import
+ååºä¾å­: ``` { "order_list": [ { "id": "476b0262-8689-4bc4-b5ff-
+380bb4ccc5e1", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
+"datatime": "2023-07-31 02:12:23", "timestamp": "1690516007000",
+"last_trade_timestamp": "1690516007000", "status": "rejected", "symbol": "USDT/
+AUD", "type": "market", "time_in_force": "FOK", "side": "buy", "price": "1000",
+"average": "", "amount": "1000", "filled": "", "remaining": "", "cost": "",
+"transfer_id": "", "fee": "", "trades": [] } ], "status": "success", "total":
+3864, "page": "1" } ``` ## websocket ``` from zerocap_api_new_test import
 ZerocapWebsocketClient # API key and secret required, èç³»zerocapè¿è¡æ³¨å
 apiKey = "***" apiSecret = "***" signature = hmac.new(apiSecret.encode("utf-
 8"), apiKey.encode("utf-8"), hashlib.sha256).hexdigest() ``` #### 1. Subscribe
 to Market data  ``` market_connect = websocket.get_market() while True: # Get
 messages message = websocket.get_message(market_connect) print(f"Receiving
 message from server: \n{message}") ``` è¯·æ±åæ°: | Parameter | required |
 data type | describe | Value range | |---------------|----------|-----------|--
```

