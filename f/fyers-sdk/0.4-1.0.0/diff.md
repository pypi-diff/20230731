# Comparing `tmp/fyers_sdk-0.4.tar.gz` & `tmp/fyers_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-0.4.tar", last modified: Fri Jul  7 09:26:22 2023, max compression
+gzip compressed data, was "fyers_sdk-1.0.0.tar", last modified: Mon Jul 31 06:14:46 2023, max compression
```

## Comparing `fyers_sdk-0.4.tar` & `fyers_sdk-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:26:22.023001 fyers_sdk-0.4/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-06-30 14:05:35.000000 fyers_sdk-0.4/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:26:22.023001 fyers_sdk-0.4/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10390 2023-07-03 07:06:42.000000 fyers_sdk-0.4/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:26:22.019001 fyers_sdk-0.4/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10801 2023-07-07 09:26:21.000000 fyers_sdk-0.4/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      355 2023-07-07 09:26:21.000000 fyers_sdk-0.4/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-07 09:26:21.000000 fyers_sdk-0.4/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       96 2023-07-07 09:26:21.000000 fyers_sdk-0.4/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-07 09:26:21.000000 fyers_sdk-0.4/fyers_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:26:22.023001 fyers_sdk-0.4/fyerstest/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-07 09:14:06.000000 fyers_sdk-0.4/fyerstest/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7315 2023-07-07 09:24:32.000000 fyers_sdk-0.4/fyerstest/api_test.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    54530 2023-07-07 09:24:31.000000 fyers_sdk-0.4/fyerstest/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3632 2023-07-07 09:24:32.000000 fyers_sdk-0.4/fyerstest/data_ws_test.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      923 2023-06-30 09:29:39.000000 fyers_sdk-0.4/fyerstest/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    28056 2023-07-03 09:38:05.000000 fyers_sdk-0.4/fyerstest/fyers_api.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-03 12:46:12.000000 fyers_sdk-0.4/fyerstest/fyers_logger.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-07 09:26:22.023001 fyers_sdk-0.4/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)      804 2023-07-07 09:25:37.000000 fyers_sdk-0.4/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-27 04:16:48.000000 fyers_sdk-1.0.0/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-1.0.0/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.188823 fyers_sdk-1.0.0/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    58436 2023-07-31 06:14:01.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1053 2023-07-31 05:28:04.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-1.0.0/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27911 2023-07-31 06:13:16.000000 fyers_sdk-1.0.0/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-1.0.0/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-07-31 06:14:46.208823 fyers_sdk-1.0.0/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      412 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      101 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-07-31 06:14:45.000000 fyers_sdk-1.0.0/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-07-31 06:14:46.212823 fyers_sdk-1.0.0/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)      851 2023-07-31 06:12:49.000000 fyers_sdk-1.0.0/setup.py
```

### Comparing `fyers_sdk-0.4/LICENSE.txt` & `fyers_sdk-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.4/PKG-INFO` & `fyers_sdk-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 0.4
+Version: 1.0.0
 Summary: Fyers trading APIs.
-Home-page: https://github.com/
+Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # The Fyers API Python client - v2.1
@@ -101,18 +99,20 @@
     getauthToken(client_id, redirect_uri, response_type, scope, state, nonce)
     
     # Step 2: Obtain authorization code
     # Add the obtained authorization code here
     auth_code = "XXXxxx"
     
     # Step 3: Generate access token
-    access_token = generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
-    print(access_token)
+    generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
 
 
+if __name__ == '__main__':
+    main()
+    
 ```
 
 ## Getting started wih API
 
 ```Python
 
 from fyerstest.fyers_api import FyersModelv3
@@ -295,9 +295,7 @@
 # Keep the socket running to receive real-time data
 fyOrder.keep_running()
 
 
 
 
 ```
-
-
```

### Comparing `fyers_sdk-0.4/README.md` & `fyers_sdk-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,20 @@
     getauthToken(client_id, redirect_uri, response_type, scope, state, nonce)
     
     # Step 2: Obtain authorization code
     # Add the obtained authorization code here
     auth_code = "XXXxxx"
     
     # Step 3: Generate access token
-    access_token = generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
-    print(access_token)
+    generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
 
 
+if __name__ == '__main__':
+    main()
+    
 ```
 
 ## Getting started wih API
 
 ```Python
 
 from fyerstest.fyers_api import FyersModelv3
```

### Comparing `fyers_sdk-0.4/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-1.0.0/fyers_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 0.4
+Version: 1.0.0
 Summary: Fyers trading APIs.
-Home-page: https://github.com/
+Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # The Fyers API Python client - v2.1
@@ -101,18 +99,20 @@
     getauthToken(client_id, redirect_uri, response_type, scope, state, nonce)
     
     # Step 2: Obtain authorization code
     # Add the obtained authorization code here
     auth_code = "XXXxxx"
     
     # Step 3: Generate access token
-    access_token = generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
-    print(access_token)
+    generate_access_token(auth_code, client_id, redirect_uri, secret_key, grant_type)
 
 
+if __name__ == '__main__':
+    main()
+    
 ```
 
 ## Getting started wih API
 
 ```Python
 
 from fyerstest.fyers_api import FyersModelv3
@@ -295,9 +295,7 @@
 # Keep the socket running to receive real-time data
 fyOrder.keep_running()
 
 
 
 
 ```
-
-
```

### Comparing `fyers_sdk-0.4/fyerstest/data_ws.py` & `fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import base64
 import logging
 import threading
 import time
+import requests
+import urllib.parse
 import websocket
 from threading import Thread
 import struct
-from fyerstest.fyers_api import FyersModelv3
-from fyerstest import defines
+from fyers_sdk.FyersWebsocket import defines
 import json
 from typing import Optional, Callable
-from fyerstest.fyers_logger import FyersLogger
+from fyers_sdk.fyers_logger import FyersLogger
 
 
 class SymbolConversion:
     def __init__(self, access_token: str, data_type: str, log_path: str):
         """
         Initializes a SymbolConversion instance.
 
@@ -23,23 +25,24 @@
 
         """
         self.data_type = data_type
         if ":" in access_token:
             access_token = access_token.split(":")[1]
         self.access_token = access_token
         self.log_path = log_path
+        self.quotes_url = "https://api-t1.fyers.in/data/quotes"
         if log_path:
-            self.logger = FyersLogger(
+            self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
                 logger_handler=logging.FileHandler(log_path + "/fyersSocket.log"),
             )
         else:
-            self.logger = FyersLogger(
+            self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
                 logger_handler=logging.FileHandler("fyersSocket.log"),
             )
 
     def symbol_to_hsmtoken(self, symbols: list):
@@ -53,19 +56,28 @@
             tuple: A tuple containing dictionary and list.
                 - The first dictionary represents the mapping of symbols to HSM tokens.
                 - The second list represents any symbols that could not be converted.
 
         """
         try:
             symbols = ",".join(symbols)
-            fyers = FyersModelv3(token=self.access_token, is_async=False)
-            quote_data = fyers.quotes({"symbols": symbols})
+            data = {"symbols": symbols}
+            url_params = urllib.parse.urlencode(data)
+            URL = self.quotes_url + "?" + url_params
+            response = requests.get(
+                url=URL,
+                headers={
+                    "Authorization": self.access_token,
+                    "Content-Type": "application/json",
+                },
+            )
+            quote_data =response.json()
             datadict = {}
             values = {}
-            with open("fyerstest/map.json", "r") as file:
+            with open("fyers_sdk/FyersWebsocket/map.json", "r") as file:
                 # Load the JSON data into a Python object
                 mapper = json.load(file)
             index_dict = mapper["index_dict"]
             exch_seg_dict = mapper["exch_seg_dict"]
             wrong_symbol = []
             if "d" in quote_data:
                 for data in quote_data["d"]:
@@ -101,15 +113,15 @@
                         datadict[values["subSymbol"]] = values["symbol"]
                     elif data["s"] == "error":
                         wrong_symbol.append(data["n"])
 
                 return (datadict, wrong_symbol)
             return ({}, [])
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
 
 class FyersDataSocket:
 
     _instance = None
 
     def __new__(cls, *args, **kwargs):
@@ -150,36 +162,37 @@
                 Defaults to None.
             OnClose (callable, optional): Callback function to be executed when a connection is closed.
                 Defaults to None.
         """
 
         self.__url = "wss://socket.fydev.tech/hsm/v1-5/dev"
         self.__access_token = access_token
+        self.__hsm_token = ""
         self.log_path = log_path
-        self.reconnect = reconnect
         self.lite = litemode
         self.source = "PythonSDK-1.0.0"
         self.channel_num = 1
         self.channels = []
         self.running_channels = set()
         self.data_type = None
         self.OnMessage = OnMessage
         self.OnError = OnError
         self.OnOpen = OnOpen
         self.OnClose = OnClose
+        self.ack_count = 0
         self.__ws_run = None
         self.write_to_file = write_to_file
         self.background_flag = False
         self.update_count = 0
         self.literesp = {}
         self.channel_symbol = []
         self.symbol_dict = {}
         self.scrips_count = {}
         self.scrips_per_channel = {}
-        self.restart_flag = True
+        self.restart_flag = reconnect
         self.websocket_lock = threading.Lock()
         self.unsub_symbol = []
         for i in range(1, 31):
             self.scrips_per_channel[i] = []
         self.active_channel = None
         self.message = []
         self.resp = {}
@@ -191,48 +204,91 @@
         self.reconnect_attempts = 0
         self.max_reconnect_attempts = 5
         self.reconnect_delay = 5
         self.index_sym = {}
         self.scrips_sym = {}
         self.symbol_token = {}
         self.ack_bool = False
-
+        self.__init_connection()
         if log_path:
-            self.logger = FyersLogger(
+            self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
-                logger_handler=logging.FileHandler(log_path + "/fyersSocket.log"),
+                logger_handler=logging.FileHandler(log_path + "fyersSocket.log"),
             )
         else:
-            self.logger = FyersLogger(
+            self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
                 logger_handler=logging.FileHandler("fyersSocket.log"),
             )
 
-        with open("fyerstest/map.json", "r") as file:
+        with open("fyers_sdk/FyersWebsocket/map.json", "r") as file:
             # Imported json file
             mapper = json.load(file)
 
         self.data_val = mapper["data_val"]
         self.index_val = mapper["index_val"]
         self.lite_val = mapper["lite_val"]
         self.depthvalue = mapper["depthvalue"]
 
+    def access_token_to_hsmtoken(self) -> bool :
+        """
+        Decode APIv2 token to extract 'hsm_key' and check for validity.
+
+        This function decodes the APIv2 access token and extracts the 'hsm_key' from it.
+        It also verifies if the token is expired by comparing the 'exp' (expiration) claim in the
+        token's payload with the current timestamp. If the token is valid and not expired, it sets
+        the 'hsm_token' attribute and returns True. Otherwise, it raises an error and returns False.
+
+        Returns:
+            bool: True if the token is valid and not expired, False otherwise.
+        """
+        try:
+            _ , payload_b64, _ = self.__access_token.split(".")
+            # Decode the base64 encoded payload
+            decoded_payload = base64.urlsafe_b64decode(payload_b64 + "===")
+            # Convert the decoded payload to a string (assuming it's in JSON format)
+            decode_token = json.loads(decoded_payload.decode())
+            today = int(time.time())
+            if decode_token["exp"] - today  < 0:
+                self.On_error(
+                    {
+                        "code": defines.TOKEN_EXPIRED,
+                        "message": defines.TOKEN_EXPIRED_MSG,
+                        "s": defines.ERROR,
+                    }
+                )
+                return False
+            self.__hsm_token = decode_token["hsm_key"]
+            return True
+        except Exception as e:
+            self.On_error(
+                {
+                    "code": defines.INVALID_CODE,
+                    "message": defines.INVALID_TOKEN,
+                    "s": defines.ERROR,
+                }
+            )
+            self.data_logger.error(e)
+            return False
+
+
+
     def __access_token_msg(self) -> bytearray:
         """
         Create a message in bytearray for token.
 
         Returns:
             bytearray: The token message in bytearray format.
         """
         try:
-            buffer_size = 18 + len(self.__access_token) + len(self.source)
+            buffer_size = 18 + len(self.__hsm_token) + len(self.source)
 
             # Create the byte buffer
             byte_buffer = bytearray()
 
             # Pack data length into the byte buffer
             byte_buffer.extend(struct.pack("!H", buffer_size - 2))
 
@@ -269,15 +325,15 @@
             byte_buffer.extend(bytes([field4_id]))
             byte_buffer.extend(struct.pack("!H", field4_size))
             byte_buffer.extend(self.source.encode())
 
             return byte_buffer
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __lite_mode_msg(self) -> bytearray:
         """
         Create a message in bytearray for lite mode connection.
 
         Returns:
             bytearray: The lite mode message in bytearray format.
@@ -310,15 +366,15 @@
             field_2.extend(struct.pack(">H", 1))
             field_2.extend(struct.pack("B", 76))
             data.extend(field_2)
 
             return data
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __full_mode_msg(self) -> bytearray:
 
         """
         Create a message in bytearray for full mode connection.
 
         Returns:
@@ -351,15 +407,15 @@
             field_2.extend(struct.pack(">H", 1))
             field_2.extend(struct.pack("B", 70))
             data.extend(field_2)
 
             return data
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __subscription_msg(self, symbols: list) -> bytearray:
 
         """
         Create a message in bytearray for symbol subscription.
 
         Args:
@@ -395,19 +451,18 @@
             buffer_msg.extend(struct.pack(">H", len(self.scrips_data)))
             buffer_msg.extend(self.scrips_data)
 
             # Field-2
             buffer_msg.append(2)
             buffer_msg.extend(struct.pack(">H", 1))
             buffer_msg.append(self.channel_num)
-
             return buffer_msg
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __unsubscription_msg(self, symbols: list) -> bytearray:
         """
         Create a message in bytearray for unsubscription message.
 
         Args:
             symbols (list): A list of symbols to unsubscribe from.
@@ -441,17 +496,16 @@
 
             # Field-2
             buffer_msg.append(2)
             buffer_msg.extend(struct.pack(">H", 1))
             buffer_msg.append(self.channel_num)
 
             return buffer_msg
-
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __channel_resume_msg(self, channel: int) -> bytearray:
 
         """
         Create a message in bytearray for channel resume.
 
         Args:
@@ -482,15 +536,15 @@
             field_1.extend(struct.pack(">H", 8))
             field_1.extend(struct.pack(">Q", channel_bits))
             data.extend(field_1)
 
             return data
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __channel_pause_msg(self, channel: int) -> bytearray:
 
         """
         Create a message in bytearray for channel pause.
 
         Args:
@@ -521,15 +575,15 @@
             field_1.extend(struct.pack(">H", 8))
             field_1.extend(struct.pack(">Q", channel_bits))
             data.extend(field_1)
 
             return data
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __ackowledgement_msg(self, message_number: int) -> bytearray:
 
         """
         Create a message in bytearray for acknowledgement.
 
         Args:
@@ -553,15 +607,15 @@
             buffer_msg.extend(struct.pack("B", field_id))
             buffer_msg.extend(struct.pack(">H", field_size))
             buffer_msg.extend(struct.pack(">I", field_value))
 
             return buffer_msg
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __auth_resp(self, data: bytearray) -> dict:
         """
         Unpacks the authentication response from a bytearray.
 
         Args:
             data (bytearray): The authentication response message.
@@ -599,15 +653,15 @@
             offset += 1
             field_length = struct.unpack("!H", data[offset : offset + 2])[0]
             offset += 2
             self.ack_count = struct.unpack(">I", data[offset : offset + 4])[0]
             offset += 4
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __subscribe_resp(self, data: bytearray) -> dict:
         """
         Unpacks the subscription response from a bytearray.
 
         Args:
             data (bytearray): The subscription response message.
@@ -638,15 +692,15 @@
                         "code": defines.SUBS_ERROR_CODE,
                         "message": defines.SUBSCRIBE_FAIL,
                         "s": defines.ERROR,
                     }
                 )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __unsubscribe_resp(self, data: bytearray) -> dict:
 
         """
         Unpacks the unsubscription response from a bytearray.
 
         Args:
@@ -668,26 +722,37 @@
                 self.On_message(
                     {
                         "code": defines.SUCCESS_CODE,
                         "message": defines.UNSUBSCRIBE_SUCCESS,
                         "s": defines.SUCCESS,
                     }
                 )
-
+                for symbol in self.unsub_symbol:
+                    count = 0
+                    for channel in self.running_channels:
+                        if symbol in self.scrips_per_channel[channel]:
+                            count +=1 
+                        if count > 1:
+                            break
+                    if symbol in self.scrips_per_channel[self.active_channel]:
+                        self.scrips_per_channel[self.active_channel].remove(symbol)
+                    if count == 1:
+                        self.symbol_token.pop(symbol)
+                            
             else:
                 self.On_error(
                     {
                         "code": defines.UNSUBS_ERROR_CODE,
                         "message": defines.UNSUBSCRIBE_FAIL,
                         "s": defines.ERROR,
                     }
                 )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __lite_full_mode_resp(self, data: bytearray) -> dict:
 
         """
         Unpacks the lite/full mode response from a bytearray.
 
         Args:
@@ -739,15 +804,15 @@
                             "code": defines.MODE_ERROR_CODE,
                             "message": defines.MODE_CHANGE_ERROR,
                             "s": defines.ERROR,
                         }
                     )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __response_output(self, data: str, data_type: str) -> object:
 
         """
         Processes the response data and returns the output based on the specified data_type.
 
         Args:
@@ -774,55 +839,57 @@
                 if data_type == "depth":
 
                     for i, val in enumerate(self.depthvalue):
                         if val in data_resp and i < 10:
                             response[val] = data_resp[val] / (
                                 10 ** data_resp["precision"]
                             )
-                        else:
+                        elif val in data_resp:
                             response[val] = data_resp[val]
                 elif data_type == "scrips":
                     for i, val in enumerate(self.data_val):
                         if val in data_resp and i in [
                             0,
                             6,
                             7,
                             11,
                             13,
                             14,
                             17,
                             18,
                             19,
-                            20,
+                            20
                         ]:
                             response[val] = data_resp[val] / (
                                 10 ** data_resp["precision"]
                             )
-                        else:
+                        elif val in data_resp:
                             response[val] = data_resp[val]
-
+                    if "close_price" in response and "ltp" in response:
+                        response["ch"] = round((response['ltp']  - response['close_price']),2) 
+                        response["chp"] = round((response["ch"]  / response['close_price'] * 100) , 2)
                     if "OI" in response:
                         response.pop("OI")
                     if "Yhigh" in response:
                         response.pop("Yhigh")
                     if "Ylow" in response:
                         response.pop("Ylow")
                 else:
                     for i, val in enumerate(self.index_val):
                         if val in data_resp and i in [0, 1, 3, 4, 5]:
                             response[val] = data_resp[val] / (
                                 10 ** data_resp["precision"]
                             )
-                        else:
+                        elif val in data_resp:
                             response[val] = data_resp[val]
 
             self.On_message(response)
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __datafeed_resp(self, data: bytearray):
 
         """
         Unpacks and processes the data based on data_type and sends it to the __response_output function.
 
         Args:
@@ -855,14 +922,15 @@
 
                     topic_name = data[offset : offset + topic_name_len].decode("utf-8")
                     offset += topic_name_len
 
                     # Maintaining dict - topic_id : topic_name
                     if topic_name[:2] == "dp":
                         self.dp_sym[topic_id] = topic_name
+
                         self.resp[self.dp_sym[topic_id]] = {}
 
                         field_count = struct.unpack("B", data[offset : offset + 1])[0]
                         offset += 1
 
                         for index in range(field_count):
                             value = struct.unpack(">I", data[offset : offset + 4])[0]
@@ -973,15 +1041,14 @@
                             offset += 1
                             string_data = data[offset : offset + string_len].decode(
                                 "utf-8"
                             )
                             self.resp[self.scrips_sym[topic_id]][val[i]] = string_data
                             offset += string_len
                         self.resp[topic_name]["symbol"] = self.symbol_token[topic_name]
-
                         self.__response_output(
                             self.resp[self.scrips_sym[topic_id]], "scrips"
                         )
 
                 elif data_type == 85:  # Full mode datafeed
                     offset += 1
                     topic_id = struct.unpack("H", data[offset : offset + 2])[0]
@@ -990,30 +1057,30 @@
                     field_count = struct.unpack("B", data[offset : offset + 1])[0]
                     offset += 1
                     sf_flag, idx_flag, dp_flag = False, False, False
 
                     for index in range(field_count):
                         value = struct.unpack(">I", data[offset : offset + 4])[0]
                         offset += 4
-                        if field_count == 21:
+                        # if field_count == 20 or field_count == 21:
+                        if topic_id in self.scrips_sym:
                             self.resp[self.scrips_sym[topic_id]][
                                 self.data_val[index]
                             ] = value
                             sf_flag = True
-                        elif field_count == 6:
+                        elif topic_id in self.index_sym:
                             self.resp[self.index_sym[topic_id]][
                                 self.index_val[index]
                             ] = value
                             idx_flag = True
-                        else:
+                        elif topic_id in self.dp_sym:
                             self.resp[self.dp_sym[topic_id]][
                                 self.depthvalue[index]
                             ] = value
                             dp_flag = True
-
                     if sf_flag:
                         self.__response_output(
                             self.resp[self.scrips_sym[topic_id]], "scrips"
                         )
                     elif idx_flag:
 
                         self.__response_output(
@@ -1050,15 +1117,15 @@
                         )
                     elif idx_flag:
                         self.__response_output(
                             self.resp[self.index_sym[topic_id]], "index"
                         )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __resume_pause_resp(self, data: bytearray, channeltype: int) -> dict:
         """
         Unpacks and processes the resume/pause response data based on the channel type.
 
         Args:
             data (bytearray): The response data.
@@ -1110,15 +1177,15 @@
                             "code": defines.RESUME_ERROR_CODE,
                             "message": defines.CHANNEL_CHANGE_FAIL,
                             "s": defines.ERROR,
                         }
                     )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __response_msg(self, data: bytearray):
         """
         Processes the response message based on the response type and calls the corresponding function.
 
         Args:
             data (bytearray): The response data.
@@ -1142,15 +1209,15 @@
             elif resp_type == 7 or resp_type == 8:
                 self.__resume_pause_resp(data, resp_type)
 
             elif resp_type == 12:  # Full Mode Data Response
                 self.__lite_full_mode_resp(data)
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __symbol_conversion(self, symbolslst: list) -> dict:
         """
         Converts symbols to HSM symbol tokens and returns a dictionary of {hsmtoken: symbol}.
 
         Args:
             symbolslst (list): A list of symbols to convert.
@@ -1168,15 +1235,15 @@
                 len(self.scrips_per_channel[self.channel_num]) > 200
                 or total_symbols > 200
                 and len(self.scrips_per_channel[self.channel_num]) + total_symbols > 200
             ):
                 self.On_error(
                     {
                         "code": defines.LIMIT_EXCEED_CODE,
-                        "message": defines.LIMIT_EXCEED_MSG,
+                        "message": defines.LIMIT_EXCEED_MSG_200,
                         "s": defines.ERROR,
                     }
                 )
                 return None
 
             symbol_chunks = [
                 symbolslst[i : i + 50] for i in range(0, total_symbols, 50)
@@ -1198,15 +1265,15 @@
                         "symbols": wrong_symbols,
                     }
                 )
 
             return symbol_dict
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def __channel_resume_pause(self):
         """
         Pauses the active channel and resumes the specified channel if necessary.
 
         If the WebSocket object (__ws_object) is not None and there is an active channel (active_channel)
         that is different from the specified channel (channelNum), the function creates and appends a pause message
@@ -1228,56 +1295,57 @@
                 if self.channel_num in self.running_channels:
                     message = self.__channel_resume_msg(self.channel_num)
                     self.message.append(message)
             self.running_channels.add(self.channel_num)
             self.active_channel = self.channel_num
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def channel_resume(self, channel: int) -> None:
         """
         Resumes the specified channel.
 
         Args:
             channel (int): The channel number to resume.
         """
         try:
             self.channel_num = channel
             self.__channel_resume_pause()
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def On_message(self, message: dict) -> None:
         """
         Handles the received message.
 
         Args:
             message (str): The received message.
         """
 
         if self.OnMessage is not None:
             self.OnMessage(message)
         else:
             if self.write_to_file:
-                self.logger.debug(f"Response:{message}")
+                self.data_logger.debug(f"Response:{message}")
             else:
-                print(f"Received response: {message}")
+                print(f"Response:{message}")
 
     def __send_message(self, message: str) -> None:
         """
         Sends a message through the WebSocket connection.
 
         Args:
             message (str): The message to send.
         """
         with self.websocket_lock:
             if self.__ws_object is not None:
-                self.__ws_object.send(message, websocket.ABNF.OPCODE_BINARY)
+
+                self.__ws_object.send(message, opcode=websocket.ABNF.OPCODE_BINARY)
 
     def __process_message_queue(self) -> None:
         """
         Processes the message queue by sending messages sequentially.
         """
 
         while True:
@@ -1295,24 +1363,24 @@
         Args:
             message (str): The error message.
         """
         if self.OnError is not None:
             self.OnError(message)
         else:
             if self.write_to_file:
-                self.logger.debug(f"ERROR Response:{message}")
+                self.data_logger.debug(f"ERROR Response:{message}")
             else:
                 print(f"Response: {message}")
 
     def on_open(self) -> None:
         """
         Performs initialization and waits before executing further actions.
         """
         if self.__ws_object is not None:
-            self.init_connection()
+            self.__init_connection()
             time.sleep(2)
 
         if self.OnOpen:
             self.OnOpen()
 
     def on_close(self, message: dict) -> None:
         """
@@ -1362,26 +1430,27 @@
             dict: A dictionary containing the response code, message, and s.
         """
         if self.restart_flag:
             if self.reconnect_attempts < self.max_reconnect_attempts:
                 self.reconnect_attempts += 1
 
                 if self.write_to_file:
-                    self.logger.debug(
+                    self.data_logger.debug(
                         f"Response:{f'Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}...'}"
                     )
                 else:
                     print(
                         f"Attempting reconnect {self.reconnect_attempts} of {self.max_reconnect_attempts}..."
                     )
                 time.sleep(self.reconnect_delay)
-                self.on_open()
+                self.__ws_object = None
+                self.__init_connection()
             else:
                 if self.write_to_file:
-                    self.logger.debug(
+                    self.data_logger.debug(
                         f"Response:{'Max reconnect attempts reached. Connection abandoned.'}"
                     )
                 else:
                     print("Max reconnect attempts reached. Connection abandoned.")
         else:
 
             self.on_close(
@@ -1397,41 +1466,42 @@
             self.__ws_object is not None
             and self.__ws_object.sock
             and self.__ws_object.sock.connected
         ):
             self.__ws_object.send("Ping")
             time.sleep(10)
 
-    def init_connection(self):
+    def __init_connection(self):
         """
         Initializes the WebSocket connection and starts the WebSocketApp.
 
         The method creates a WebSocketApp object with the specified URL and sets the appropriate event handlers.
         It then starts the WebSocketApp in a separate thread.
         """
         try:
             if self.__ws_object is None:
-                if self.write_to_file:
-                    self.background_flag = True
-
-                ws = websocket.WebSocketApp(
-                    self.__url,
-                    on_message=lambda ws, msg: self.__response_msg(msg),
-                    on_error=lambda ws, msg: self.On_error(msg),
-                    on_close=lambda ws, close_code, close_reason: self.__on_close(
-                        ws, close_code, close_reason
-                    ),
-                    on_open=lambda ws: self.__on_open(ws),
-                )
-                self.ws_thread = Thread(target=ws.run_forever)
-                self.ws_thread.daemon = self.background_flag
-                self.ws_thread.start()
+                if self.access_token_to_hsmtoken():
+                    if self.write_to_file:
+                        self.background_flag = True
+
+                    ws = websocket.WebSocketApp(
+                        self.__url,
+                        on_message=lambda ws, msg: self.__response_msg(msg),
+                        on_error=lambda ws, msg: self.On_error(msg),
+                        on_close=lambda ws, close_code, close_reason: self.__on_close(
+                            ws, close_code, close_reason
+                        ),
+                        on_open=lambda ws: self.__on_open(ws),
+                    )
+                    self.ws_thread = Thread(target=ws.run_forever)
+                    self.ws_thread.daemon = self.background_flag
+                    self.ws_thread.start()
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def close_connection(self) -> None:
         """
         Closes the WebSocket connection 
 
         """
 
@@ -1486,50 +1556,58 @@
                 for symbols in symbol_chunks:
                     message = self.__unsubscription_msg(symbols)
                     self.message.append(message)
             else:
                 self.On_error(
                     {
                         "code": defines.INVALID_CODE,
-                        "message": defines.WRONG_CHANNEL_MSG,
+                        "message": defines.INVALID_SYMBOLS,
                         "s": defines.ERROR,
                     }
                 )
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
 
     def subscribe(
         self, symbols: list, data_type: str = "SymbolUpdate", channel: int = 1
     ):
         """
         Subscribes to real-time data updates for the specified symbols.
 
         Args:
             symbols (list): A list of symbols to subscribe to.
             data_type (str, optional): The type of data to subscribe to. Defaults to "SymbolUpdate".
             channel (int, optional): The channel to use for subscription. Defaults to 1.
         """
         try:
-            self.init_connection()
+            # self.__init_connection()
             time.sleep(2)
-
             self.data_type = data_type
             self.symbols = symbols
             self.channel_num = channel
             self.__channel_resume_pause()
             self.channel_symbol = self.__symbol_conversion(symbols)
             if self.channel_symbol is None:
                 return
+            if len(self.symbol_token) + len(self.channel_symbol) > 500:
+                self.On_error(
+                    {
+                        "code": defines.LIMIT_EXCEED_CODE,
+                        "message": defines.LIMIT_EXCEED_MSG_500,
+                        "s": defines.ERROR,
+                    }
+                )
+                return
             self.symbol_token.update(self.symbol_token, **self.channel_symbol)
             self.scrips_count[self.channel_num] = list(self.channel_symbol.keys())
             total_symbols = len(self.scrips_count[self.channel_num])
             symbol_chunks = [
                 self.scrips_count[self.channel_num][i : i + 100]
                 for i in range(0, total_symbols, 100)
             ]
             for symbols in symbol_chunks:
                 message = self.__subscription_msg(symbols)
                 self.message.append(message)
 
         except Exception as e:
-            self.logger.exception(e)
+            self.data_logger.exception(e)
```

### Comparing `fyers_sdk-0.4/fyerstest/defines.py` & `fyers_sdk-1.0.0/fyers_sdk/FyersWebsocket/defines.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,23 @@
 SUBS_ERROR_CODE = 11011
 UNSUBS_ERROR_CODE = 11012
 RESUME_ERROR_CODE = 11031
 RESUME_ERROR_CODE = 11032
 MODE_ERROR_CODE = 12001
 SUCCESS_CODE = 200
 INVALID_CODE = -300
+TOKEN_EXPIRED = -99
 LIMIT_EXCEED_CODE = -99
-LIMIT_EXCEED_MSG = "Please provide less than 200 symbols"
+LIMIT_EXCEED_MSG_200 = "Please provide less than 200 symbols"
+LIMIT_EXCEED_MSG_500 = "Please provide less than 500 symbols"
+TOKEN_EXPIRED_MSG = "Token is expired"
 WRONG_CHANNEL_MSG = (
-    "Please provide valid channel , channel does not contain this symbol"
+    "Please provide valid symbol"
 )
+INVALID_TOKEN = "Please provide valid token"
 SUCCESS = "Ok"
 ERROR = "error"
 AUTH_SUCCESS = "Authentication done"
 AUTH_FAIL = "Authentication failed"
 SUBSCRIBE_SUCCESS = "Subscribed"
 SUBSCRIBE_FAIL = "subscription failed"
 UNSUBSCRIBE_SUCCESS = "Unsubscribed"
```

### Comparing `fyers_sdk-0.4/fyerstest/fyers_api.py` & `fyers_sdk-1.0.0/fyers_sdk/fyersModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,68 @@
-moduleName = "fyersApi"
+moduleName ="fyersModel"
+try:
+	import logging
+	import urllib.parse
+	import hashlib
+	import json
+	import asyncio
+	import subprocess
+	import sys
+	import requests
+	import json
+	import urllib
+	import aiohttp
+	import asyncio
+	import json
+	from fyers_sdk.fyers_logger import FyersLogger
 
-import logging
-import urllib.parse
-import hashlib
-import json
-import asyncio
-import subprocess
-import sys
-import requests
-import json
-import urllib
-import aiohttp
-import asyncio
-import json
-from fyerstest.fyers_logger import FyersLogger
+except Exception as e:
+	print("moduleName: {}, ERR: could not import module : {}".format(moduleName,e))
 
 
 class Config:
-    # API = 'https://api-t1.fyers.in/trade/v3'
+    API = 'https://api-t1.fyers.in/api/v3'
     # API = "https://api-t1.fydev.tech/trade/dev"
-    API = "https://api.fyers.in/api/v2"
+    # API = "https://api.fyers.in/api/v2"
     HISTORY_URL = "https://api.fyers.in/data-rest/v2"
     DATA_API = "https://api-t1.fyers.in/data"
     AUTH_URL = "https://api.fyers.in/api/v2"
 
     # Endpoint
     get_profile = "/profile"
     tradebook = "/tradebook"
     positions = "/positions"
     holdings = "/holdings"
     convert_position = "/positions"
     funds = "/funds"
-    orders = "/orders/sync"
+    place_orders = "/orders/sync"
+    orderbook = "/orders"
     minquantity = "/minquantity"
     market_status = "/marketStatus"
     auth = "/generate-authcode"
     generate_access_token = "/validate-authcode"
     generate_data_token = "/data-token"
-    data_vendor_td = "truedata-ws"
-    # multi_orders = 'orders-multi'
-    sync_multi_order = "/multi-order/sync"
-    multi_orders = "/multi-order"
+    data_vendor_td = "/truedata-ws"
+    multi_orders = "/multi-order/sync"
     history = "/history"
     quotes = "/quotes"
     market_depth = "/depth"
 
 
+
+
 class FyersServiceSync:
     def __init__(self, logger):
         """
         Initializes an instance of FyersServiceSync.
 
         Args:
             logger: The logger object used for logging errors.
         """
-        self.logger = logger
+        self.api_logger = logger
         self.content = "application/json"
 
     def post_call(self, api: str, header: str, data=None) -> dict:
         """
         Makes a POST request to the specified API.
 
         Args:
@@ -73,15 +77,15 @@
             response = requests.post(
                 Config.API + api,
                 data=json.dumps(data),
                 headers={"Authorization": header, "Content-Type": self.content},
             )
             return response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
 
     def get_call(self, api: str, header: str, data=None, data_flag=False) -> dict:
         """
         Makes a GET request to the specified API.
 
         Args:
             api: The API endpoint to make the request to.
@@ -111,15 +115,15 @@
                     "Authorization": header,
                     "Content-Type": self.content,
                     "version": "2.1",
                 },
             )
             return response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
 
     def delete_call(self, api: str, header: str, data) -> dict:
         """
         Makes a DELETE request to the specified API.
 
         Args:
             api: The API endpoint to make the request to.
@@ -133,15 +137,15 @@
             response = requests.delete(
                 url=Config.API + api,
                 data=json.dumps(data),
                 headers={"Authorization": header, "Content-Type": self.content},
             )
             return response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
 
     def patch_call(self, api: str, header: str, data) -> dict:
         """
         Makes a PATCH request to the specified API.
 
         Args:
             api: The API endpoint to make the request to.
@@ -155,26 +159,26 @@
             response = requests.patch(
                 url=Config.API + api,
                 data=json.dumps(data),
                 headers={"Authorization": header, "Content-Type": self.content},
             )
             return response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
 
 
 class FyersServiceAsync:
     def __init__(self, logger):
         """
         Initializes an instance of FyersServiceAsync.
 
         Args:
             logger: The logger object used for logging errors.
         """
-        self.logger = logger
+        self.api_logger = logger
         self.content = "application/json"
 
     async def post_async_call(self, api: str, header: str, data=None) -> dict:
         """
         Makes an asynchronous POST request to the specified API.
 
         Args:
@@ -190,15 +194,15 @@
                 headers={"Authorization": header, "Content-Type": self.content}
             ) as session:
                 url = Config.API + api
                 async with session.post(url, data=json.dumps(data)) as response:
                     response = await response.json()
                     return response
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
             return response
 
     async def get_async_call(
         self, api: str, header: str, params=None, data_flag=False
     ) -> dict:
         """
         Makes an asynchronous GET request to the specified API.
@@ -228,15 +232,15 @@
                 }
             ) as session:
                 async with session.get(URL, params=params) as response:
                     response = await response.json()
                     return response
 
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
             return response
 
     async def delete_async_call(self, api: str, header: str, data) -> dict:
         """
         Makes an asynchronous DELETE request to the specified API.
 
         Args:
@@ -251,15 +255,15 @@
             async with aiohttp.ClientSession(
                 headers={"Authorization": header, "Content-Type": self.content}
             ) as session:
                 url = Config.API + api
                 async with session.delete(url, data=json.dumps(data)) as response:
                     return await response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
             return response
 
     async def patch_async_call(self, api: str, header: str, data) -> dict:
         """
         Makes an asynchronous PATCH request to the specified API.
 
         Args:
@@ -276,15 +280,15 @@
             ) as session:
                 url = Config.API + api
                 json_data = json.dumps(data).encode("utf-8")
 
                 async with session.patch(url, data=json_data) as response:
                     return await response.json()
         except Exception as e:
-            self.logger.error(e)
+            self.api_logger.error(e)
             return response
 
 
 class SessionModel:
     def __init__(
         self,
         client_id=None,
@@ -335,27 +339,15 @@
         }
         response = requests.post(
             Config.AUTH_URL + Config.generate_access_token, headers="", json=data
         )
         return response.json()
 
 
-class FyersModelv3:
-    """
-    A class that provides methods for making API calls synchronously or asynchronously.
-
-    Attributes:
-        is_async (bool): A boolean indicating whether API calls should be made asynchronously.
-        service (object): An object that provides methods for making API calls.
-        header (str): A string containing the header information for making API calls.
-        logger (Logger): The logger object used for logging.
-        client_id (str): The client ID for API authentication.
-        token (str): The token for API authentication.
-    """
-
+class FyersModel:
     def __init__(
         self,
         is_async: bool = False,
         log_path=None,
         client_id: str = "",
         token: str = "",
     ):
@@ -369,31 +361,31 @@
         """
         self.client_id = client_id
         self.token = token
         self.is_async = is_async
         self.log_path = log_path
         self.header = "{}:{}".format(self.client_id, self.token)
         if log_path:
-            self.logger = FyersLogger(
+            self.api_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=2,
                 logger_handler=logging.FileHandler(log_path + "/fyersApi.log"),
             )
         else:
-            self.logger = FyersLogger(
+            self.api_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=2,
                 logger_handler=logging.FileHandler("fyersApi.log"),
             )
         if is_async:
-            self.service = FyersServiceAsync(self.logger)
+            self.service = FyersServiceAsync(self.api_logger)
         else:
-            self.service = FyersServiceSync(self.logger)
+            self.service = FyersServiceSync(self.api_logger)
 
     def get_profile(self) -> dict:
         """
         Retrieves the user profile information.
 
         """
         if self.is_async:
@@ -417,17 +409,14 @@
             response = self.service.get_call(Config.tradebook, self.header)
         return response
 
     def funds(self) -> dict:
         """
         Retrieves funds details.
 
-        Args:
-            data: Optional data to send in the request.
-
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
                 self.service.get_async_call(Config.funds, self.header)
             )
@@ -473,33 +462,33 @@
             data: The data containing the order ID.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
-                self.service.get_async_call(Config.orders, self.header, params=data)
+                self.service.get_async_call(Config.orderbook, self.header, params=data)
             )
         else:
-            response = self.service.get_call(Config.orders, self.header, data=data)
+            response = self.service.get_call(Config.orderbook, self.header, data=data)
         return response
 
     def orderbook(self) -> dict:
         """
         Retrieves the order information.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
-                self.service.get_async_call(Config.orders, self.header)
+                self.service.get_async_call(Config.orderbook, self.header)
             )
         else:
-            response = self.service.get_call(Config.orders, self.header)
+            response = self.service.get_call(Config.orderbook, self.header)
         return response
 
     def market_status(self) -> dict:
         """
         Retrieves market status.
 
         Returns:
@@ -517,16 +506,16 @@
             )
         return response
 
     def convert_position(self, data) -> dict:
         """
         Converts positions from one product type to another based on the provided details.
 
-        Parameters:
-            symbol (str): Symbol of the positions. Eg: '119031547242'.
+        Args:
+            symbol (str): Symbol of the positions. Eg: "MCX:SILVERMIC20NOVFUT".
             positionSide (int): Side of the positions. 1 for open long positions, -1 for open short positions.
             convertQty (int): Quantity to be converted. Should be in multiples of lot size for derivatives.
             convertFrom (str): Existing product type of the positions. (CNC positions cannot be converted)
             convertTo (str): The new product type to convert the positions to.
 
         Returns:
             The response JSON as a dictionary.
@@ -582,18 +571,18 @@
             - 'offlineOrder' (bool): Specifies if the order is placed when the market is open (False) or as an AMO order (True).
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
-                self.service.post_async_call(Config.orders, self.header, data)
+                self.service.post_async_call(Config.place_orders, self.header, data)
             )
         else:
-            response = self.service.post_call(Config.orders, self.header, data)
+            response = self.service.post_call(Config.place_orders, self.header, data)
         return response
 
     def modify_order(self, data) -> dict:
         """
         Modifies the parameters of a pending order based on the provided details.
 
         Parameters:
@@ -632,17 +621,17 @@
         else:
             response = self.service.delete_call(Config.positions, self.header, data)
         return response
 
     def generate_data_token(self, data):
         allPackages = subprocess.check_output([sys.executable, "-m", "pip", "freeze"])
         installed_packages = [r.decode().split("==")[0] for r in allPackages.split()]
-        if Config.dataVendorTD not in installed_packages:
+        if Config.data_vendor_td not in installed_packages:
             print("Please install truedata package | pip install truedata-ws")
-        response = self.service.post_call(Config.generateDataToken, self.header, data)
+        response = self.service.post_call(Config.generate_data_token, self.header, data)
         return response
 
     def cancel_basket_orders(self, data):
         """
         Cancels the orders with the provided IDs.
 
         Parameters:
@@ -650,20 +639,20 @@
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
                 self.service.delete_async_call(
-                    Config.sync_multi_order, self.header, data
+                    Config.multi_orders, self.header, data
                 )
             )
         else:
             response = self.service.delete_call(
-                Config.sync_multi_order, self.header, data
+                Config.multi_orders, self.header, data
             )
         return response
 
     def place_basket_orders(self, data):
         """
         Places multiple orders based on the provided details.
 
@@ -689,15 +678,15 @@
         """
         if self.is_async:
             response = asyncio.run(
                 self.service.post_async_call(Config.multi_orders, self.header, data)
             )
         else:
             response = self.service.post_call(
-                Config.sync_multi_order, self.header, data
+                Config.multi_orders, self.header, data
             )
         return response
 
     def modify_basket_orders(self, data):
         """
         Modifies multiple pending orders based on the provided details.
 
@@ -712,20 +701,20 @@
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
                 self.service.patch_async_call(
-                    Config.sync_multi_order, self.header, data
+                    Config.multi_orders, self.header, data
                 )
             )
         else:
             response = self.service.patch_call(
-                Config.sync_multi_order, self.header, data
+                Config.multi_orders, self.header, data
             )
         return response
 
     def history(self, data=None):
         """
         Fetches candle data based on the provided parameters.
 
@@ -797,7 +786,20 @@
                 )
             )
         else:
             response = self.service.get_call(
                 Config.market_depth, self.header, data, data_flag=True
             )
         return response
+    
+
+    def minquantity(self):
+        if self.is_async:
+            response = asyncio.run(
+                self.service.get_async_call(
+                    Config.minquantity, self.header)
+            )
+        else:
+            response = self.service.get_call(
+                Config.minquantity, self.header)
+        return response
+
```

### Comparing `fyers_sdk-0.4/fyerstest/fyers_logger.py` & `fyers_sdk-1.0.0/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-0.4/setup.py` & `fyers_sdk-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='0.4',
+     version='1.0.0',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
-     url="https://github.com/",
+     url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
      install_requires=[
-            'aiohttp==3.8.4',
-            'Requests==2.31.0',
-            'websocket_client==1.2.1',
-            'websocket_client==1.2.1',
-            'websockets==8.1'
+                'requests==2.31.0',
+                'asyncio==3.4.3',
+                'aiohttp==3.8.4',
+                'aws_lambda_powertools==1.25.5',
+                'websocket-client==1.6.1'
           ],
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: MIT License",
          "Operating System :: OS Independent",
      ],
- )
+ )
```

