# Comparing `tmp/bondzai.gateway-sdk-0.0.8.tar.gz` & `tmp/bondzai.gateway-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-sdk-0.0.8.tar", last modified: Tue Jul 11 18:22:54 2023, max compression
+gzip compressed data, was "bondzai.gateway-sdk-0.0.9.tar", last modified: Mon Jul 31 12:28:48 2023, max compression
```

## Comparing `bondzai.gateway-sdk-0.0.8.tar` & `bondzai.gateway-sdk-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.648080 bondzai.gateway-sdk-0.0.8/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-11 18:22:54.648179 bondzai.gateway-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      155 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/README.md
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.639413 bondzai.gateway-sdk-0.0.8/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.646008 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/
--rw-r--r--   0 theo       (501) staff       (20)      139 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)    10475 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/agent.py
--rw-r--r--   0 theo       (501) staff       (20)     2593 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/commands.py
--rw-r--r--   0 theo       (501) staff       (20)      255 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/config.py
--rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:22:45.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     6937 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/events.py
--rw-r--r--   0 theo       (501) staff       (20)     4429 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/gateway.py
--rw-r--r--   0 theo       (501) staff       (20)     3288 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/message.py
--rw-r--r--   0 theo       (501) staff       (20)      810 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/request.py
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/responses.py
--rw-r--r--   0 theo       (501) staff       (20)      771 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/timer.py
--rw-r--r--   0 theo       (501) staff       (20)     1396 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/transcode.py
--rw-r--r--   0 theo       (501) staff       (20)      738 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:54.647874 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      770 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)       61 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:54.000000 bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)    21241 2023-07-11 18:21:06.000000 bondzai.gateway-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-11 18:22:54.648746 bondzai.gateway-sdk-0.0.8/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:48.406235 bondzai.gateway-sdk-0.0.9/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-31 12:26:37.000000 bondzai.gateway-sdk-0.0.9/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-31 12:28:48.406388 bondzai.gateway-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      155 2023-07-31 12:26:37.000000 bondzai.gateway-sdk-0.0.9/README.md
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:48.396963 bondzai.gateway-sdk-0.0.9/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:48.403384 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/
+-rw-r--r--   0 theo       (501) staff       (20)      139 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)    10618 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/agent.py
+-rw-r--r--   0 theo       (501) staff       (20)     2593 2023-07-31 12:26:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/commands.py
+-rw-r--r--   0 theo       (501) staff       (20)      255 2023-07-31 12:26:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/config.py
+-rw-r--r--   0 theo       (501) staff       (20)     7572 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     7569 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/events.py
+-rw-r--r--   0 theo       (501) staff       (20)     5220 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/gateway.py
+-rw-r--r--   0 theo       (501) staff       (20)     3288 2023-07-31 12:26:38.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/message.py
+-rw-r--r--   0 theo       (501) staff       (20)      970 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/request.py
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-31 12:26:38.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/responses.py
+-rw-r--r--   0 theo       (501) staff       (20)      771 2023-07-31 12:26:38.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/timer.py
+-rw-r--r--   0 theo       (501) staff       (20)     1817 2023-07-31 12:28:37.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/transcode.py
+-rw-r--r--   0 theo       (501) staff       (20)      738 2023-07-31 12:26:38.000000 bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:48.405912 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      604 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      770 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)       61 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:48.000000 bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)    21241 2023-07-31 12:26:38.000000 bondzai.gateway-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-31 12:28:48.407505 bondzai.gateway-sdk-0.0.9/setup.cfg
```

### Comparing `bondzai.gateway-sdk-0.0.8/NOTICE` & `bondzai.gateway-sdk-0.0.9/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/PKG-INFO` & `bondzai.gateway-sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/agent.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,28 +46,30 @@
                     self._wait_response[msg_id] = data
 
             if typ == MessageType.EVENT:
                 operation = EventOperationID(msg['header']['op'])
                 if mod == MessageModule.LOG:
                     if operation == EventOperationID.EVT_EXT_LOG:
                         content = data.get("msg", "")
-                        if content == "EVT_INT_TRAIN_DONE":
-                            for callback in self._on_train_done_handlers.values():
-                                callback(self, data)
-                        else:
-                            for callback in self._on_log_handlers.values():
+                        for callback in self._on_log_handlers.values():
                                 callback(self, content)
                 else:
                     data_transcode = transcode(operation, data)
                     if operation == EventOperationID.EVT_EXT_VM_RESULT:
                         for callback in self._on_infer_done_handlers.values():
                             callback(self, data_transcode)
                     elif operation == EventOperationID.EVT_EXT_ASL_RESULT:
                         for callback in self._on_final_process_done.values():
                             callback(self, data_transcode)
+                    elif operation == EventOperationID.EVT_EXT_PROCESS_ACK:
+                        evt_id = data_transcode.get("evt_id", None)
+                        if evt_id == EventOperationID.EVT_INT_TRAIN_DONE:
+                            for callback in self._on_train_done_handlers.values():
+                                        callback(self, data_transcode)
+
                     for callback in self._on_event_handlers.values():
                         callback(self, operation, data)
 
     def remove_observer(self, dict_obj_name, idx):
         if not hasattr(self, dict_obj_name):
             return
         dict_obj = getattr(self, dict_obj_name)
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/commands.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/commands.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/enums.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class EventOperationID(Enum):
     EVT_EXT_EXCEPTION = 0x00
     EVT_EXT_DATA_IN = 0x01
     EVT_EXT_CMD_STATUS = 0x100
     EVT_EXT_LOG = 0x101
     EVT_EXT_VM_RESULT = 0x200
     EVT_EXT_ASL_RESULT = 0x201
+    EVT_EXT_PROCESS_ACK = 0x210
     EVT_EXT_SET_MODE = 0x300
     EVT_EXT_CORRECTION = 0x301
     EVT_EXT_TRIGGER = 0x302
     EVT_EXT_CUSTOM_1 = 0xF00
     EVT_EXT_CUSTOM_2 = 0xF01
     EVT_EXT_CUSTOM_3 = 0xF02
     EVT_EXT_CUSTOM_4 = 0xF03
@@ -78,35 +79,40 @@
     APP_AI_TYPE_CLASSIFICATION = 0
     APP_AI_TYPE_REGRESSION = 1
 
 
 class PPOperationUID(Enum):
     OPS_ID_EXT = 0x80000000
     OPS_ID = 0x00000000
+    OP_CUST_MIN = OPS_ID_EXT
+    OP_CUST_FIRST = 0x80000100
     OPS_MISC = 0x00000000
     OPS_MATH = 0x01000000
     OPS_DSP = 0x02000000
     OPS_IMG = 0x03000000
     OPS_STR = 0x04000000
     OPS_DBM = 0x05000000
     OPS_PST = 0x0E000000
     OPS_DIST = 0x0F000000
-    OPS_UID_NOP = 0x00
-    OPS_UID_NOPEND = 0x01
     OPS_UID_CP1D = 0x02
     OPS_UID_CP2D = 0x03
     OPS_UID_CP2X1D = 0x04
     OPS_UID_RMNFIRST1D_F32 = 0x05
     OPS_UID_LOGANF32 = 0x1000001
     OPS_UID_LOGA10F32 = 0x1000002
     OPS_UID_MEANF32 = 0x1000011
     OPS_UID_VARF32 = 0x1000012
     OPS_UID_RESHAPEF32 = 0x1000013
     OPS_UID_HISTOGRAMF32 = 0x1000014
-    OPS_UID_SLICEF32 = 0x1000015
+    OPS_UID_VECTORMATRIX_PRODUCTF32 = 0x1000015
+    OPS_UID_FLATTENMATRIXF32 = 0x1000016
+    OPS_UID_TRANSPOSEMATRIXF32 = 0x1000017
+    OPS_UID_SLICEF32 = 0x1000018
+    OPS_UID_SLICEMATRIXROWSF32 = 0x1000019
+    OPS_UID_SLICEMATRIXCOLSF32 = 0x100001A
     OPS_UID_FFT2048F32 = 0x2000011
     OPS_UID_FFT1024F32 = 0x2000012
     OPS_UID_FFT16F32 = 0x2000018
     OPS_UID_MFCC2048F32 = 0x2000019
     OPS_UID_MFCC1024F32 = 0x200001A
     OPS_UID_MEL2048F32 = 0x2000021
     OPS_UID_MEL1024F32 = 0x2000022
@@ -114,14 +120,16 @@
     OPS_UID_DCT2048F32 = 0x2000031
     OPS_UID_DCT1024F32 = 0x2000032
     OPS_UID_DCT512F32 = 0x2000033
     OPS_UID_DCT256F32 = 0x2000034
     OPS_UID_DCT128F32 = 0x2000035
     OPS_UID_NOISEMIXF32 = 0x2000061
     OPS_UID_PWSPANF32 = 0x2000062
+    OPS_UID_DCT2D = 0x3000001
+    OPS_UID_RGB_TO_GRAYF32 = 0x3000002
     OPS_UID_PUSHSIG2DBM = 0x5000001
     OPS_UID_PST_BYPASS = 0xE000001
     OPS_UID_PST_EXT = 0x8E000001
 
 
 class CommandOperationID(Enum):
     CMD_OPEN_SESSION = 0x00
@@ -162,14 +170,15 @@
     DBM_IMPORT_ROW = 0x201
     DBM_DELETE_ROW = 0x202
     DBM_CHECK_POINT = 0x300
     DBM_RESTORE = 0x301
     DBM_DEL_CHECK_POINT = 0x302
     DBM_GET_CHECK_POINT = 0x303
     DBM_CREATE_TABLE = 0x400
+    DBM_DELETE_TABLE = 0x401
 
 
 class DBMTable(Enum):
     DBM_VM = 0x00
     DBM_LBL = 0x01
     DBM_DAT = 0x02
     DBM_KEY = 0x03
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/events.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,26 +271,53 @@
     def to_array(self) -> list:
         return [self.data]
 
     @classmethod
     def from_dict(cls, data: dict) -> "EventCustom":
         return EventCustom(data.get("data"))
 
+@dataclass
+class EventProcessAck:
+    evt_id: int
+    process_state: int
+    step: int
+    app_id: int
+    meta: bytes
+
+    def to_dict(self) -> str:
+        return {
+            "evt_id": self.evt_id,
+            "process_state": self.process_state,
+            "step": self.step,
+            "app_id": self.app_id,
+            "meta": self.meta
+        }
+
+    def to_array(self) -> list:
+        return [
+            self.evt_id,
+            self.process_state,
+            self.step,
+            self.app_id,
+            self.meta
+        ]
+
 
 EventPayloadType = Union[
     EventCMDStatus,
     EventCustom,
     EventDataIn,
     EventException,
     EventLog,
     EventAslResult,
     EventInferResult,
     EventSetMode,
     EventCorrection,
-    EventTrigger
+    EventTrigger,
+    EventProcessAck
 ]
 
 OP_TO_EVENT_TYPES = {
     EventOperationID.EVT_EXT_EXCEPTION.value: EventException,
     EventOperationID.EVT_EXT_DATA_IN.value: EventDataIn,
     EventOperationID.EVT_EXT_CMD_STATUS.value: EventCMDStatus,
     EventOperationID.EVT_EXT_LOG.value: EventLog,
@@ -304,13 +331,14 @@
     EventOperationID.EVT_EXT_CUSTOM_3.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_4.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_5.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_6.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_7.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_8.value: EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_9.value: EventCustom,
-    EventOperationID.EVT_EXT_CUSTOM_10.value: EventCustom
+    EventOperationID.EVT_EXT_CUSTOM_10.value: EventCustom,
+    EventOperationID.EVT_EXT_PROCESS_ACK.value: EventProcessAck,
 }
 
 
 def get_event_class(event_type_id: EventOperationID):
     return OP_TO_EVENT_TYPES.get(event_type_id.value, None)
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/gateway.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/gateway.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from typing import Any
 import json
 import time
 import threading
 from collections.abc import Callable
 from websocket import WebSocketApp, setdefaulttimeout
 
 from .request import Request, RequestActions
@@ -13,14 +14,15 @@
 
 class Gateway:
     def __init__(self, host: str, port: int, secure: bool = False, config: Configuration = None) -> None: 
         self.config = config if config is not None else Configuration()
         
         self._host = host
         self._port = port
+        self._auth_token = None
 
         host_parts = host.split("/")
         url = f"{'wss' if secure else 'ws'}://{host_parts.pop(0)}:{port}"
         if len(host_parts):
             url = f"{url}/{'/'.join(host_parts)}"
 
         self.wss = WebSocketApp(
@@ -33,14 +35,15 @@
 
         self.is_connected = False
         self.thread = None
 
         self._on_connect_callbacks: list[Callable[[None], None]] = []
         self._on_close_callbacks: list[Callable[[int, str], None]] = []
         self._on_error_callbacks: list[Callable[[Exception], None]] = []
+        self._on_client_msg_callbacks: list[Callable[[Any], None]] = []
 
         self._agents: dict[str, Agent] = {}
 
     def _on_connection_open(self, _: WebSocketApp):
         self.is_connected = True
         for cb_func in self._on_connect_callbacks:
             cb_func()
@@ -74,17 +77,25 @@
 
                 elif data["action"] == RequestActions.EVT_ON_DEVICE_MSG.value:
                     device_name = data.get("device_name")
                     msg = data.get("message", "")
 
                     if device_name in self._agents:
                         self._agents[device_name].handle_message(msg)
+
+                elif data["action"] == RequestActions.EVT_ON_CLIENT_MSG.value:
+                    msg = data.get("message", "")
+                    for cb in self._on_client_msg_callbacks:
+                        cb(msg)
         except Exception as err:
             self._on_error(wsa, err)
 
+    def set_auth_token(self, token: str):
+        self._auth_token = token
+
     def connect(self, wait_for_connection: bool = True, connection_timeout_sec: int = 10) -> None:
         try:
             setdefaulttimeout(connection_timeout_sec)
 
             self.thread = threading.Thread(target=self.wss.run_forever)
             self.thread.start()
             
@@ -99,18 +110,23 @@
             raise err
 
     def close(self) -> None:
         if self.is_connected:
             self.wss.close()
         self.thread.join()
 
+    def on_client_msg(self, callback: Callable[[Any], None]) -> None:
+        self._on_client_msg_callbacks.append(callback)
+
     def on_error(self, callback: Callable[[Exception], None]) -> None:
         self._on_error_callbacks.append(callback)
 
     def send(self, request: Request) -> None:
+        if self._auth_token:
+            request.token = self._auth_token
         self.wss.send(request.to_json())
 
     def request_agent_list(self) -> None:
         self.send(Request(RequestActions.ACT_GET_DEVICES_LIST))
 
     def wait_for_agent(self, timeout_sec: int = 30) -> list[Agent]:
         if not self._agents.keys():
@@ -120,7 +136,13 @@
         while not self._agents.keys():
             Timer.wait(0.001)
             now_time = time.time()
             if now_time - start_time > timeout_sec:
                 break
 
         return list(self._agents.values())
+
+    def send_to_clients(self, msg: Any) -> None:
+        self.send(Request(
+            RequestActions.ACT_TRANSFERS_TO_WS_CLIENTS,
+            data=msg
+        ))
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/message.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/message.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/timer.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/transcode.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/transcode.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,9 +35,21 @@
         else:
             transcode_data = {
                 "ai_type": data["ai_type"],
                 "label_type": data["label_type"],
                 "step": data["step"],
                 "regression": data["result"]
             }
-
+    elif op == EventOperationID.EVT_EXT_PROCESS_ACK:
+        # convert
+        try : 
+            evt_id = EventOperationID(data["evt_id"])
+        except Exception as e :
+            evt_id = None
+        transcode_data = {
+            "evt_id": evt_id,
+            "process_state": data["process_state"],
+            "step": data["step"],
+            "app_id": data["app_id"],
+            "meta": data["meta"]
+        }
     return transcode_data
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai/gateway_sdk/utils.py` & `bondzai.gateway-sdk-0.0.9/bondzai/gateway_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/PKG-INFO` & `bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bondzai Gateway SDK
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-sdk-0.0.8/bondzai.gateway_sdk.egg-info/SOURCES.txt` & `bondzai.gateway-sdk-0.0.9/bondzai.gateway_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/pyproject.toml` & `bondzai.gateway-sdk-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-sdk-0.0.8/setup.cfg` & `bondzai.gateway-sdk-0.0.9/setup.cfg`

 * *Files identical despite different names*

