# Comparing `tmp/zerocap_api_new_test-0.1.6.tar.gz` & `tmp/zerocap_api_new_test-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\zerocap_api_new_test-0.1.6.tar", last modified: Mon Jul 31 02:28:27 2023, max compression
+gzip compressed data, was "dist\zerocap_api_new_test-0.1.7.tar", last modified: Mon Jul 31 07:11:03 2023, max compression
```

## Comparing `zerocap_api_new_test-0.1.6.tar` & `zerocap_api_new_test-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/
--rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.6/LICENSE.txt
--rw-rw-rw-   0        0        0    19529 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     2133 2023-07-31 02:28:20.000000 zerocap_api_new_test-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/
--rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/__init__.py
--rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/
--rw-rw-rw-   0        0        0    19529 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2023-07-31 02:28:27.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 02:28:26.000000 zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/
+-rw-rw-rw-   0        0        0    11523 2023-07-26 06:34:57.000000 zerocap_api_new_test-0.1.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    19586 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15434 2023-07-31 02:13:00.000000 zerocap_api_new_test-0.1.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     2133 2023-07-31 07:11:00.000000 zerocap_api_new_test-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/
+-rw-rw-rw-   0        0        0      126 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/__init__.py
+-rw-rw-rw-   0        0        0     8154 2023-07-29 09:52:06.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/
+-rw-rw-rw-   0        0        0    19586 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 07:11:03.000000 zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_new_test-0.1.6/LICENSE.txt` & `zerocap_api_new_test-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.6/PKG-INFO` & `zerocap_api_new_test-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_api_new_test
-Version: 0.1.6
+Version: 0.1.7
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -41,16 +41,16 @@
 
 ```
 from zerocap_api_new_test import ZerocapRestClient
 import uuid
 import time
 
 # API key and secret required, 联系zerocap进行注册
-apiKey = "***" 
-apiSecret = "***"
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
 ```
 
 #### 1. Create an order
 <!--post https://dma-api.defi.wiki/orders/create_order-->
 
 ```
 
@@ -76,16 +76,16 @@
 |-----------------|-----------|-----------|-----------------|--------------|
 | symbol          | true      | string    | Instrument      | USDT/AUD     |
 | side            | true      | string    | Side            | buy sell     |
 | type            | true      | string    | Type            | market limit |
 | amount          | true      | string    | Quantity        |              |
 | price           | true      | string    | Price           |              |
 | client_order_id | true      | string    | Client order id |              |
-| note | true      | string    | Client order id |              |
-| third_identity_id | true      | string    | Client order id |              |
+| note | true      | string    | note  |              |
+| third_identity_id | true      | string    | third_identity_id |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "USDT/AUD",
@@ -260,15 +260,15 @@
 | Parameter      | required | data type | describe        | Value range |
 |----------------|----------|-----------|-----------------|-------------|
 | symbol         | true     | string    | symbol          |             |
 | start_datetime | true     | string    | start_datetime  |             |
 | end_datetime   | true     | string    | end_datetime    |             |
 | page           | true     | string    | page            |             |
 | limit          | true     | string    | limit           |             |
-| ids            | true     | string    | Transaction ids |             |
+| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
 | status         | true     | string    | status          |             |
 | sort_order     | true     | string    | sort_order      |             |
 | order_type     | true     | string    | order_type      |             |
 | side           | true     | string    | side            |             |
 
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
@@ -412,23 +412,23 @@
 {
     "type": "message",
     "channel": "dma_price_USDT/AUD",
     "data": "{
         \"sell_price\": \"1.322544321902561296\",
         \"buy_price\": \"1.668209315127094362\",
         \"datetime\": \"2023-07-28 10:03:40\",
-        \"timestamp\": \"1690538620.1056492\",
+        \"timestamp\": \"1690538620.1056492\"
         }"
 }
 
 {
     "type": "message",
     "channel": "dma_price_USDT/AUD",
     "data": "{
-        \"message\":\"Price stream unavailable.\,
+        \"message\":\"Price stream unavailable.\"
         }"
 }
 
 # Heartbeat neglect
 {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
 
 ```
@@ -529,16 +529,16 @@
         \"Note\":\"yyy_test_create_order\",
         \"Status\":\"open\",
         \"Average\":\"0\",
         \"Filled\":\"0\",
         \"Remaining\":\"1000\",
         \"Cost\":\"1000000\",
         \"ExecPrice\":\"\",
-        \"OrderFrom\":\"coinroutes\,
-    "}"
+        \"OrderFrom\":\"coinroutes\"
+    }"
 }
 
 ```
 
 channel: dma_trader_info 响应数据:
 
 
@@ -577,12 +577,12 @@
         \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
         \"type\":\"market\",
         \"side\":\"sell\",
         \"takerOrMaker\":\"taker\",
         \"price\":\"1.662902412\",
         \"amount\":\"101\",
         \"cost\":\"167.9531436\",
-        \"orderFrom\":\"coinroutes\
-    "}
-"}
+        \"orderFrom\":\"coinroutes\"
+    }"
+}
 
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: zerocap_api_new_test Version: 0.1.7 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
 from zerocap_api_new_test import ZerocapRestClient import uuid import time #
-API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "***" apiSecret
-= "***" ``` #### 1. Create an order  ``` client = ZerocapRestClient(apiKey,
-apiSecret) client_order_id = str(uuid.uuid4()) result = client.create_order
-( symbol='USDT/AUD', side='buy', type='market', amount='100', price='1000',
-client_order_id=client_order_id, note='this is test',
-third_identity_id='ZCStreamingLiquidity1') ``` è¯·æ±åæ°: | Parameter |
-required | data type | describe | Value range | |-----------------|-----------
-|-----------|-----------------|--------------| | symbol | true | string |
-Instrument | USDT/AUD | | side | true | string | Side | buy sell | | type |
-true | string | Type | market limit | | amount | true | string | Quantity | | |
-price | true | string | Price | | | client_order_id | true | string | Client
-order id | | | note | true | string | Client order id | | | third_identity_id |
-true | string | Client order id | |
+API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "coinroutes"
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ``` #### 1. Create an order
+``` client = ZerocapRestClient(apiKey, apiSecret) client_order_id = str
+(uuid.uuid4()) result = client.create_order( symbol='USDT/AUD', side='buy',
+type='market', amount='100', price='1000', client_order_id=client_order_id,
+note='this is test', third_identity_id='ZCStreamingLiquidity1') ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+---------------|-----------|-----------|-----------------|--------------| |
+symbol | true | string | Instrument | USDT/AUD | | side | true | string | Side
+| buy sell | | type | true | string | Type | market limit | | amount | true |
+string | Quantity | | | price | true | string | Price | | | client_order_id |
+true | string | Client order id | | | note | true | string | note | | |
+third_identity_id | true | string | third_identity_id | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "USDT/AUD", "side": "buy", "type": "market", "amount": "1000",
 "price": "1000", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |--------------------|---------
 -|-----------|-----------------|-------------| | id | true | long | Transaction
@@ -67,17 +67,18 @@
 3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
 client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
 describe | Value range | |----------------|----------|-----------|-------------
 ----|-------------| | symbol | true | string | symbol | | | start_datetime |
 true | string | start_datetime | | | end_datetime | true | string |
 end_datetime | | | page | true | string | page | | | limit | true | string |
-limit | | | ids | true | string | Transaction ids | | | status | true | string
-| status | | | sort_order | true | string | sort_order | | | order_type | true
-| string | order_type | | | side | true | string | side | |
+limit | | | ids | true | string | Transaction ids(null character string or
+id1,id2...) | | | status | true | string | status | | | sort_order | true |
+string | sort_order | | | order_type | true | string | order_type | | | side |
+true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
@@ -108,16 +109,16 @@
 dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
 true | string | sell price | | | data['buy_price'] | true | string | buy price
 | | | data['datetime'] | true | string | time | | | data['timestamp'] | true |
 string | time | | | message | false | string | description | Is price open |
 ååºä¾å­: ``` { "type": "message", "channel": "dma_price_USDT/AUD", "data":
 "{ \"sell_price\": \"1.322544321902561296\", \"buy_price\":
 \"1.668209315127094362\", \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\":
-\"1690538620.1056492\", }" } { "type": "message", "channel": "dma_price_USDT/
-AUD", "data": "{ \"message\":\"Price stream unavailable.\, }" } # Heartbeat
+\"1690538620.1056492\" }" } { "type": "message", "channel": "dma_price_USDT/
+AUD", "data": "{ \"message\":\"Price stream unavailable.\" }" } # Heartbeat
 neglect {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"} ``` #### 2.
 Subscribe Order updates or transaction records  ``` orders_connect =
 websocket.get_orders() while True: # Get messages message =
 websocket.get_message(orders_connect) print(f"Receiving message from server: \n
 {message}") ``` è¯·æ±åæ°: | Parameter | required | data type | describe |
 Value range | |---------------|----------|-----------|-------------------------
 |-------------| | api_key | true | string | key | | | signature | true | long |
@@ -150,15 +151,15 @@
 4256-9de3-cd37310a55da\", \"TxnAlias\":\"\", \"TransferId\":\"\", \"Symbol\":
 \"USDT/AUD\", \"Type\":\"market\", \"TimeInForce\":\"FOK\", \"Side\":\"sell\",
 \"Price\":\"1000\", \"AveragePrice\":\"\", \"Amount\":\"1000\", \"CreatedAt\":
 1690538950000, \"UpdatedAt\":1690538950000, \"AccountId\":\"1ca36d2b-2103-45c7-
 a2e3-3b90825ba1b2\", \"VaultId\":\"5175\", \"Note\":\"yyy_test_create_order\",
 \"Status\":\"open\", \"Average\":\"0\", \"Filled\":\"0\", \"Remaining\":
 \"1000\", \"Cost\":\"1000000\", \"ExecPrice\":\"\", \"OrderFrom\":
-\"coinroutes\, "}" } ``` channel: dma_trader_info ååºæ°æ®: | Parameter |
+\"coinroutes\" }" } ``` channel: dma_trader_info ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |----------------------|-------
 -----|-----------|--------------|--------------------------------| | type |
 true | long | type | | | channel | true | string | channel |
 dma_order_infoãdma_trader_info | | data | true | jsonstr | data | | | data
 ['id'] | true | str | id | | | data['timestamp'] | true | str | timestamp | | |
 data['datetime'] | true | str | datetime | | | data['symbol'] | true | str |
 symbol | | | data['order'] | true | str | order | | | data['type'] | true | str
@@ -167,8 +168,8 @@
 ['amount'] | true | str | amount | | | data['cost'] | true | str | cost | | |
 data['orderFrom'] | true | str | orderFrom | | ååºä¾å­: ``` { "type":
 "message", "pattern":null, "channel":"dma_trade_info", "data":"{ \"id\":
 \"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\", \"timestamp\":\"1690767892000\",
 \"datetime\":\"2023-07-31 01:44:52\", \"symbol\":\"USDT/AUD\", \"order\":
 \"41969863-1f32-4eaa-b679-a5b0e6fb5542\", \"type\":\"market\", \"side\":
 \"sell\", \"takerOrMaker\":\"taker\", \"price\":\"1.662902412\", \"amount\":
-\"101\", \"cost\":\"167.9531436\", \"orderFrom\":\"coinroutes\ "} "} ```
+\"101\", \"cost\":\"167.9531436\", \"orderFrom\":\"coinroutes\" }" } ```
```

### Comparing `zerocap_api_new_test-0.1.6/README.rst` & `zerocap_api_new_test-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.6/setup.py` & `zerocap_api_new_test-0.1.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         os.system('git tag v{0}'.format(about['__version__']))
         os.system('git push --tags')
 
         sys.exit()
 
 setup(
     name='zerocap_api_new_test',  # 包名
-    version='0.1.6',  # 版本号
+    version='0.1.7',  # 版本号
     description='zerocap_api',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='zerocap',
     author_email='jiayu.gao@eigen.capital',
     url='https://zerocap.com/',
     install_requires=REQUIRED,
```

### Comparing `zerocap_api_new_test-0.1.6/zerocap_api_new_test/main.py` & `zerocap_api_new_test-0.1.7/zerocap_api_new_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_api_new_test-0.1.6/zerocap_api_new_test.egg-info/PKG-INFO` & `zerocap_api_new_test-0.1.7/zerocap_api_new_test.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-api-new-test
-Version: 0.1.6
+Version: 0.1.7
 Summary: zerocap_api
 Home-page: https://zerocap.com/
 Author: zerocap
 Author-email: jiayu.gao@eigen.capital
 License: MIT
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -41,16 +41,16 @@
 
 ```
 from zerocap_api_new_test import ZerocapRestClient
 import uuid
 import time
 
 # API key and secret required, 联系zerocap进行注册
-apiKey = "***" 
-apiSecret = "***"
+apiKey = "coinroutes" 
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a"
 ```
 
 #### 1. Create an order
 <!--post https://dma-api.defi.wiki/orders/create_order-->
 
 ```
 
@@ -76,16 +76,16 @@
 |-----------------|-----------|-----------|-----------------|--------------|
 | symbol          | true      | string    | Instrument      | USDT/AUD     |
 | side            | true      | string    | Side            | buy sell     |
 | type            | true      | string    | Type            | market limit |
 | amount          | true      | string    | Quantity        |              |
 | price           | true      | string    | Price           |              |
 | client_order_id | true      | string    | Client order id |              |
-| note | true      | string    | Client order id |              |
-| third_identity_id | true      | string    | Client order id |              |
+| note | true      | string    | note  |              |
+| third_identity_id | true      | string    | third_identity_id |              |
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
 
 ```
 
 {
     "symbol": "USDT/AUD",
@@ -260,15 +260,15 @@
 | Parameter      | required | data type | describe        | Value range |
 |----------------|----------|-----------|-----------------|-------------|
 | symbol         | true     | string    | symbol          |             |
 | start_datetime | true     | string    | start_datetime  |             |
 | end_datetime   | true     | string    | end_datetime    |             |
 | page           | true     | string    | page            |             |
 | limit          | true     | string    | limit           |             |
-| ids            | true     | string    | Transaction ids |             |
+| ids            | true     | string    | Transaction ids(null character string or id1,id2...) |   |
 | status         | true     | string    | status          |             |
 | sort_order     | true     | string    | sort_order      |             |
 | order_type     | true     | string    | order_type      |             |
 | side           | true     | string    | side            |             |
 
 
 请求参数：示例（不能直接使用,需要替换自己的参数）
@@ -412,23 +412,23 @@
 {
     "type": "message",
     "channel": "dma_price_USDT/AUD",
     "data": "{
         \"sell_price\": \"1.322544321902561296\",
         \"buy_price\": \"1.668209315127094362\",
         \"datetime\": \"2023-07-28 10:03:40\",
-        \"timestamp\": \"1690538620.1056492\",
+        \"timestamp\": \"1690538620.1056492\"
         }"
 }
 
 {
     "type": "message",
     "channel": "dma_price_USDT/AUD",
     "data": "{
-        \"message\":\"Price stream unavailable.\,
+        \"message\":\"Price stream unavailable.\"
         }"
 }
 
 # Heartbeat neglect
 {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"}
 
 ```
@@ -529,16 +529,16 @@
         \"Note\":\"yyy_test_create_order\",
         \"Status\":\"open\",
         \"Average\":\"0\",
         \"Filled\":\"0\",
         \"Remaining\":\"1000\",
         \"Cost\":\"1000000\",
         \"ExecPrice\":\"\",
-        \"OrderFrom\":\"coinroutes\,
-    "}"
+        \"OrderFrom\":\"coinroutes\"
+    }"
 }
 
 ```
 
 channel: dma_trader_info 响应数据:
 
 
@@ -577,12 +577,12 @@
         \"order\":\"41969863-1f32-4eaa-b679-a5b0e6fb5542\",
         \"type\":\"market\",
         \"side\":\"sell\",
         \"takerOrMaker\":\"taker\",
         \"price\":\"1.662902412\",
         \"amount\":\"101\",
         \"cost\":\"167.9531436\",
-        \"orderFrom\":\"coinroutes\
-    "}
-"}
+        \"orderFrom\":\"coinroutes\"
+    }"
+}
 
 ```
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
-Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.6 Summary:
+Metadata-Version: 2.1 Name: zerocap-api-new-test Version: 0.1.7 Summary:
 zerocap_api Home-page: https://zerocap.com/ Author: zerocap Author-email:
 jiayu.gao@eigen.capital License: MIT Platform: all Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE.txt # zerocap-
 api-new-test # Jump_restapi # Jump_websocket ``` æè¿°ä»ç» sdk install pip
 install zerocap-api-new-test ã ã ã ``` # restapi #### æ¥å£ææ¡£ ```
 from zerocap_api_new_test import ZerocapRestClient import uuid import time #
-API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "***" apiSecret
-= "***" ``` #### 1. Create an order  ``` client = ZerocapRestClient(apiKey,
-apiSecret) client_order_id = str(uuid.uuid4()) result = client.create_order
-( symbol='USDT/AUD', side='buy', type='market', amount='100', price='1000',
-client_order_id=client_order_id, note='this is test',
-third_identity_id='ZCStreamingLiquidity1') ``` è¯·æ±åæ°: | Parameter |
-required | data type | describe | Value range | |-----------------|-----------
-|-----------|-----------------|--------------| | symbol | true | string |
-Instrument | USDT/AUD | | side | true | string | Side | buy sell | | type |
-true | string | Type | market limit | | amount | true | string | Quantity | | |
-price | true | string | Price | | | client_order_id | true | string | Client
-order id | | | note | true | string | Client order id | | | third_identity_id |
-true | string | Client order id | |
+API key and secret required, èç³»zerocapè¿è¡æ³¨å apiKey = "coinroutes"
+apiSecret = "e2d2a9b8-85fe-4a38-b9bd-60e06b58b28a" ``` #### 1. Create an order
+``` client = ZerocapRestClient(apiKey, apiSecret) client_order_id = str
+(uuid.uuid4()) result = client.create_order( symbol='USDT/AUD', side='buy',
+type='market', amount='100', price='1000', client_order_id=client_order_id,
+note='this is test', third_identity_id='ZCStreamingLiquidity1') ```
+è¯·æ±åæ°: | Parameter | required | data type | describe | Value range | |--
+---------------|-----------|-----------|-----------------|--------------| |
+symbol | true | string | Instrument | USDT/AUD | | side | true | string | Side
+| buy sell | | type | true | string | Type | market limit | | amount | true |
+string | Quantity | | | price | true | string | Price | | | client_order_id |
+true | string | Client order id | | | note | true | string | note | | |
+third_identity_id | true | string | third_identity_id | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "USDT/AUD", "side": "buy", "type": "market", "amount": "1000",
 "price": "1000", "client_order_id": "e7f80d34-0d80-4256-9de3-cd37310a55da",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |--------------------|---------
 -|-----------|-----------------|-------------| | id | true | long | Transaction
@@ -67,17 +67,18 @@
 3864, "page": "1" } ``` #### 3. Batch fetch order  ``` result =
 client.fetch_orders(symbol='USDT/AUD', start_datetime=int(time.time() * 1000 -
 86400), limit=10) ``` è¯·æ±åæ°: | Parameter | required | data type |
 describe | Value range | |----------------|----------|-----------|-------------
 ----|-------------| | symbol | true | string | symbol | | | start_datetime |
 true | string | start_datetime | | | end_datetime | true | string |
 end_datetime | | | page | true | string | page | | | limit | true | string |
-limit | | | ids | true | string | Transaction ids | | | status | true | string
-| status | | | sort_order | true | string | sort_order | | | order_type | true
-| string | order_type | | | side | true | string | side | |
+limit | | | ids | true | string | Transaction ids(null character string or
+id1,id2...) | | | status | true | string | status | | | sort_order | true |
+string | sort_order | | | order_type | true | string | order_type | | | side |
+true | string | side | |
 è¯·æ±åæ°ï¼ç¤ºä¾ï¼ä¸è½ç´æ¥ä½¿ç¨,éè¦æ¿æ¢èªå·±çåæ°ï¼ ```
 { "symbol": "", "start_datetime": 0, "end_datetime": 0, "page": 0, "limit": 0,
 "ids": "", "status": "", "sort_order": "", "order_type": "", "side": "",
 "account_vault": { "third_identity_id": "918d7125916c13191f3674e", "api_key":
 "***", "signature": "***", "note": "" } } ``` ååºæ°æ® æ¥å£æ¥é å¾å®:
 | Parameter | required | data type | describe | Value range | |---------------
 |----------|-----------|----------------|-------------| | id | true | string |
@@ -108,16 +109,16 @@
 dma_price_USDT/AUD | | data | true | jsonstr | data | | | data['sell_price'] |
 true | string | sell price | | | data['buy_price'] | true | string | buy price
 | | | data['datetime'] | true | string | time | | | data['timestamp'] | true |
 string | time | | | message | false | string | description | Is price open |
 ååºä¾å­: ``` { "type": "message", "channel": "dma_price_USDT/AUD", "data":
 "{ \"sell_price\": \"1.322544321902561296\", \"buy_price\":
 \"1.668209315127094362\", \"datetime\": \"2023-07-28 10:03:40\", \"timestamp\":
-\"1690538620.1056492\", }" } { "type": "message", "channel": "dma_price_USDT/
-AUD", "data": "{ \"message\":\"Price stream unavailable.\, }" } # Heartbeat
+\"1690538620.1056492\" }" } { "type": "message", "channel": "dma_price_USDT/
+AUD", "data": "{ \"message\":\"Price stream unavailable.\" }" } # Heartbeat
 neglect {"type":"message","channel":"","data":"{\"ok\": \"ok\"}"} ``` #### 2.
 Subscribe Order updates or transaction records  ``` orders_connect =
 websocket.get_orders() while True: # Get messages message =
 websocket.get_message(orders_connect) print(f"Receiving message from server: \n
 {message}") ``` è¯·æ±åæ°: | Parameter | required | data type | describe |
 Value range | |---------------|----------|-----------|-------------------------
 |-------------| | api_key | true | string | key | | | signature | true | long |
@@ -150,15 +151,15 @@
 4256-9de3-cd37310a55da\", \"TxnAlias\":\"\", \"TransferId\":\"\", \"Symbol\":
 \"USDT/AUD\", \"Type\":\"market\", \"TimeInForce\":\"FOK\", \"Side\":\"sell\",
 \"Price\":\"1000\", \"AveragePrice\":\"\", \"Amount\":\"1000\", \"CreatedAt\":
 1690538950000, \"UpdatedAt\":1690538950000, \"AccountId\":\"1ca36d2b-2103-45c7-
 a2e3-3b90825ba1b2\", \"VaultId\":\"5175\", \"Note\":\"yyy_test_create_order\",
 \"Status\":\"open\", \"Average\":\"0\", \"Filled\":\"0\", \"Remaining\":
 \"1000\", \"Cost\":\"1000000\", \"ExecPrice\":\"\", \"OrderFrom\":
-\"coinroutes\, "}" } ``` channel: dma_trader_info ååºæ°æ®: | Parameter |
+\"coinroutes\" }" } ``` channel: dma_trader_info ååºæ°æ®: | Parameter |
 required | data type | describe | Value range | |----------------------|-------
 -----|-----------|--------------|--------------------------------| | type |
 true | long | type | | | channel | true | string | channel |
 dma_order_infoãdma_trader_info | | data | true | jsonstr | data | | | data
 ['id'] | true | str | id | | | data['timestamp'] | true | str | timestamp | | |
 data['datetime'] | true | str | datetime | | | data['symbol'] | true | str |
 symbol | | | data['order'] | true | str | order | | | data['type'] | true | str
@@ -167,8 +168,8 @@
 ['amount'] | true | str | amount | | | data['cost'] | true | str | cost | | |
 data['orderFrom'] | true | str | orderFrom | | ååºä¾å­: ``` { "type":
 "message", "pattern":null, "channel":"dma_trade_info", "data":"{ \"id\":
 \"60e2e941-070c-40e3-b2ef-4a8f6ad9f316\", \"timestamp\":\"1690767892000\",
 \"datetime\":\"2023-07-31 01:44:52\", \"symbol\":\"USDT/AUD\", \"order\":
 \"41969863-1f32-4eaa-b679-a5b0e6fb5542\", \"type\":\"market\", \"side\":
 \"sell\", \"takerOrMaker\":\"taker\", \"price\":\"1.662902412\", \"amount\":
-\"101\", \"cost\":\"167.9531436\", \"orderFrom\":\"coinroutes\ "} "} ```
+\"101\", \"cost\":\"167.9531436\", \"orderFrom\":\"coinroutes\" }" } ```
```

