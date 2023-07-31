# Comparing `tmp/bondzai.gateway-0.0.7.tar.gz` & `tmp/bondzai.gateway-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bondzai.gateway-0.0.7.tar", last modified: Tue Jul 11 18:22:34 2023, max compression
+gzip compressed data, was "bondzai.gateway-0.0.8.tar", last modified: Mon Jul 31 12:28:29 2023, max compression
```

## Comparing `bondzai.gateway-0.0.7.tar` & `bondzai.gateway-0.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.456060 bondzai.gateway-0.0.7/
--rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/NOTICE
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-11 18:22:34.456163 bondzai.gateway-0.0.7/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/README.rst
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.438880 bondzai.gateway-0.0.7/bondzai/
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.442073 bondzai.gateway-0.0.7/bondzai/gateway/
--rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/config.yml
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.445293 bondzai.gateway-0.0.7/bondzai/gateway/core/
--rw-r--r--   0 theo       (501) staff       (20)     7995 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/application.py
--rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/device.py
--rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/events.py
--rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/fsm.py
--rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/logger.py
--rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/manager.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.449072 bondzai.gateway-0.0.7/bondzai/gateway/core/message/
--rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/command.py
--rw-r--r--   0 theo       (501) staff       (20)     7213 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/enums.py
--rw-r--r--   0 theo       (501) staff       (20)     6771 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/event.py
--rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/payload.py
--rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/process_dbm.py
--rw-r--r--   0 theo       (501) staff       (20)     9408 2023-07-11 18:22:25.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/response.py
--rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/message/utils.py
--rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.451662 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/
--rw-r--r--   0 theo       (501) staff       (20)     1768 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/client.py
--rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/connector.py
--rw-r--r--   0 theo       (501) staff       (20)     1731 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/request.py
--rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/utils.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.452992 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/
--rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/base.py
--rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/serial.py
--rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/socket_server.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.453596 bondzai.gateway-0.0.7/bondzai/gateway/tests/
--rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/tests/__init__.py
--rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/bondzai/gateway/tests/test_observer.py
-drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-11 18:22:34.455831 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/
--rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/PKG-INFO
--rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/SOURCES.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/dependency_links.txt
--rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/entry_points.txt
--rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/namespace_packages.txt
--rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/requires.txt
--rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/top_level.txt
--rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-11 18:22:34.000000 bondzai.gateway-0.0.7/bondzai.gateway.egg-info/zip-safe
--rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-11 18:20:57.000000 bondzai.gateway-0.0.7/pyproject.toml
--rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-11 18:22:34.456781 bondzai.gateway-0.0.7/setup.cfg
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.511279 bondzai.gateway-0.0.8/
+-rw-r--r--   0 theo       (501) staff       (20)      547 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/NOTICE
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-31 12:28:29.511500 bondzai.gateway-0.0.8/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)      195 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/README.rst
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.496926 bondzai.gateway-0.0.8/bondzai/
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.499224 bondzai.gateway-0.0.8/bondzai/gateway/
+-rw-r--r--   0 theo       (501) staff       (20)      775 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)      843 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/config.yml
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.501467 bondzai.gateway-0.0.8/bondzai/gateway/core/
+-rw-r--r--   0 theo       (501) staff       (20)     8525 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/application.py
+-rw-r--r--   0 theo       (501) staff       (20)      328 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/device.py
+-rw-r--r--   0 theo       (501) staff       (20)      577 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/events.py
+-rw-r--r--   0 theo       (501) staff       (20)      833 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/fsm.py
+-rw-r--r--   0 theo       (501) staff       (20)     2127 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/logger.py
+-rw-r--r--   0 theo       (501) staff       (20)     2590 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/manager.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.504448 bondzai.gateway-0.0.8/bondzai/gateway/core/message/
+-rw-r--r--   0 theo       (501) staff       (20)     5391 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4968 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/command.py
+-rw-r--r--   0 theo       (501) staff       (20)     7572 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/enums.py
+-rw-r--r--   0 theo       (501) staff       (20)     7382 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/event.py
+-rw-r--r--   0 theo       (501) staff       (20)      337 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/payload.py
+-rw-r--r--   0 theo       (501) staff       (20)     6821 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/process_dbm.py
+-rw-r--r--   0 theo       (501) staff       (20)     9408 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/response.py
+-rw-r--r--   0 theo       (501) staff       (20)      942 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/message/utils.py
+-rw-r--r--   0 theo       (501) staff       (20)     2276 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.505865 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/
+-rw-r--r--   0 theo       (501) staff       (20)     1749 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/client.py
+-rw-r--r--   0 theo       (501) staff       (20)     2652 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/connector.py
+-rw-r--r--   0 theo       (501) staff       (20)     2370 2023-07-31 12:28:18.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/request.py
+-rw-r--r--   0 theo       (501) staff       (20)      171 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/utils.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.507171 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/
+-rw-r--r--   0 theo       (501) staff       (20)      201 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/base.py
+-rw-r--r--   0 theo       (501) staff       (20)     4426 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/serial.py
+-rw-r--r--   0 theo       (501) staff       (20)     7630 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/socket_server.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.507844 bondzai.gateway-0.0.8/bondzai/gateway/tests/
+-rw-r--r--   0 theo       (501) staff       (20)        0 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/tests/__init__.py
+-rw-r--r--   0 theo       (501) staff       (20)     2280 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/bondzai/gateway/tests/test_observer.py
+drwxr-xr-x   0 theo       (501) staff       (20)        0 2023-07-31 12:28:29.510879 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/
+-rw-r--r--   0 theo       (501) staff       (20)      596 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/PKG-INFO
+-rw-r--r--   0 theo       (501) staff       (20)     1382 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 theo       (501) staff       (20)       57 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/entry_points.txt
+-rw-r--r--   0 theo       (501) staff       (20)        8 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/namespace_packages.txt
+-rw-r--r--   0 theo       (501) staff       (20)      117 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/requires.txt
+-rw-r--r--   0 theo       (501) staff       (20)       13 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/top_level.txt
+-rw-r--r--   0 theo       (501) staff       (20)        1 2023-07-31 12:28:29.000000 bondzai.gateway-0.0.8/bondzai.gateway.egg-info/zip-safe
+-rw-r--r--   0 theo       (501) staff       (20)       71 2023-07-31 12:26:30.000000 bondzai.gateway-0.0.8/pyproject.toml
+-rw-r--r--   0 theo       (501) staff       (20)      913 2023-07-31 12:28:29.512547 bondzai.gateway-0.0.8/setup.cfg
```

### Comparing `bondzai.gateway-0.0.7/NOTICE` & `bondzai.gateway-0.0.8/NOTICE`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/PKG-INFO` & `bondzai.gateway-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/__init__.py` & `bondzai.gateway-0.0.8/bondzai/gateway/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import signal
 from pathlib import Path
 
 from .core.application import Application, CONFIG_DEFAULT_PATH
 
 
 CMD_NAME = "bondzai.gateway"
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 
 
 def run():
     parser = argparse.ArgumentParser(
         prog=CMD_NAME,
         description="Davinsy Gateway"
     )
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/config.yml` & `bondzai.gateway-0.0.8/bondzai/gateway/config.yml`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/application.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/application.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from .manager import Manager
 from .message.base import Message
 from .websocket.utils import ws_client_serialize
 from .events import DeviceEvents, WebsocketEvents
 from .observer import dispatcher
 from .websocket.connector import WebSocketConnector
 from .websocket.client import WebsocketClient
-from .websocket.request import ACT_GET_DEVICES_LIST, ACT_SEND_TO_DEVICE, ACT_SUB_TO_DEVICE, ACT_UNSUB_FROM_DEVUCE, WebsocketRequest
+from .websocket.request import ACT_GET_DEVICES_LIST, ACT_SEND_TO_DEVICE, ACT_SUB_TO_DEVICE, ACT_UNSUB_FROM_DEVUCE, \
+            ACT_TRANSFERS_TO_WS_CLIENTS, EVT_ON_CLIENT_MSG, EVT_ON_DEVICE_MSG, WebsocketRequest
 from .fsm import get_files
 
 from ..device_connectors.base import DeviceConnector
 
 
 CONFIG_DEFAULT_PATH: Path = Path(__file__).parent.parent / "config.yml"
 CONNECTORS_PATH: Path = Path(__file__).parent.parent / "device_connectors"
@@ -136,14 +137,16 @@
 
         if request.action == ACT_SUB_TO_DEVICE:
             Manager.SubToDeviceEvents(request.device_name, client)
         elif request.action == ACT_UNSUB_FROM_DEVUCE:
             Manager.UnsubFromDeviceEvents(request.device_name, client)
         elif request.action == ACT_GET_DEVICES_LIST:
             self.send_device_list_to_clients(client)
+        elif request.action == ACT_TRANSFERS_TO_WS_CLIENTS:
+            self.transfers_msg_to_clients(request.message, client.id)
         elif request.action == ACT_SEND_TO_DEVICE:
             device = Manager.GetDevice(request.device_name)
             if device:
                 msg = Message.from_json(request.message)
                 device.send(msg.to_msgpack())
 
     def send_device_list_to_clients(self, client: WebsocketClient = None) -> None:
@@ -154,14 +157,22 @@
             "action": ACT_GET_DEVICES_LIST,
             "devices": device_list
         })
 
         for client in clients:
             client.send(msg)
 
+    def transfers_msg_to_clients(self, msg: str, from_client_id) -> None:
+        for client in Manager.GetClients():
+            if client.id != from_client_id:
+                client.send(ws_client_serialize({
+                    "action": EVT_ON_CLIENT_MSG,
+                    "message": msg
+                }))
+
     # Callback for Device event CONNECTED
     def on_device_connected(self, device: Device) -> None:
         log(f"New device connected {device.name}")
         Manager.RegisterDevice(device)
         self.send_device_list_to_clients()
 
     # Callback for Device event DISCONNECTED
@@ -174,15 +185,15 @@
     def on_device_message(self, device: Device, msg: Message) -> None:
         # TODO : Handle msg
         # TMP : For now send msg to every subscribed websocket clients
         log(f"Application On Device Message {device.name}")
         for client in Manager.GetDeviceEventSubs(device.name):
             log(f"Application Forward")
             client.send(ws_client_serialize({ 
-                "action": "on-device-msg",
+                "action": EVT_ON_DEVICE_MSG,
                 "device_name": device.name,
                 "message": msg.to_dict()
             }))
 
     # Callback when a websocket client is connected
     def on_websocket_client_connected(self, client: WebsocketClient) -> None:
         Manager.RegisterClient(client)
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/events.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/events.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/fsm.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/fsm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/logger.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/logger.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/manager.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/manager.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/base.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/base.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/command.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/command.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/enums.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/enums.py`

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

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/event.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/event.py`

 * *Files 3% similar despite different names*

```diff
@@ -223,14 +223,39 @@
 
     def to_dict(self) -> str:
         return { "data": B2B64(self.data) }
 
     def to_array(self) -> list:
         return [ self.data ]
     
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
 
 OP_TO_EVENT_TYPES = {
     EventOperationID.EVT_EXT_EXCEPTION.value:     EventException,
     EventOperationID.EVT_EXT_DATA_IN.value:       EventDataIn,
     EventOperationID.EVT_EXT_CMD_STATUS.value:    EventCMDStatus,
     EventOperationID.EVT_EXT_LOG.value:           EventLog,
     EventOperationID.EVT_EXT_ASL_RESULT.value:    EventAslResult, 
@@ -243,15 +268,16 @@
     EventOperationID.EVT_EXT_CUSTOM_3.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_4.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_5.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_6.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_7.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_8.value:      EventCustom,
     EventOperationID.EVT_EXT_CUSTOM_9.value:      EventCustom,
-    EventOperationID.EVT_EXT_CUSTOM_10.value:     EventCustom
+    EventOperationID.EVT_EXT_CUSTOM_10.value:     EventCustom,
+    EventOperationID.EVT_EXT_PROCESS_ACK.value:   EventProcessAck
 }
 
 
 def GetEventClass(event_type_id: int):
     return OP_TO_EVENT_TYPES.get(event_type_id, None)
 
 class EventMessagePayload(MessagePayload):
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/process_dbm.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/process_dbm.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/response.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/response.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/message/utils.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/message/utils.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/observer.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/client.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.socket = socket
         self.id = uuid4()
 
     async def _do_send(self, msg: str) -> None:
         await self.socket.send(msg)
 
     def send(self, msg: str) -> None:
-        log(f"Sending message coming from device to client, msg = {msg}")
+        log(f"Sending message to client, msg = {msg}")
 
         new_loop = False
         try:
             loop = asyncio.get_event_loop()
             if not loop.is_running():
                 # if the loop is not running we do as if there is none.
                 raise
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/connector.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/connector.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/core/websocket/request.py` & `bondzai.gateway-0.0.8/bondzai/gateway/core/websocket/request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,62 @@
+import os
+
 from dataclasses import dataclass
 
 from ..manager import Manager
 
 
 ACT_SUB_TO_DEVICE = "sub-to-device"
 ACT_UNSUB_FROM_DEVUCE = "unsub-from-device"
 ACT_SEND_TO_DEVICE = "send-to-device"
 ACT_GET_DEVICES_LIST = "get-device-list"
+ACT_TRANSFERS_TO_WS_CLIENTS = "transfers-to-ws-clients"
+
+EVT_ON_DEVICE_MSG = "on-device-msg"
+EVT_ON_CLIENT_MSG = "on-client-msg"
 
 VALID_ACTIONS = [
     ACT_GET_DEVICES_LIST,
     ACT_SEND_TO_DEVICE,
     ACT_UNSUB_FROM_DEVUCE,
-    ACT_SUB_TO_DEVICE
+    ACT_SUB_TO_DEVICE,
+    ACT_TRANSFERS_TO_WS_CLIENTS
 ]
 
 
 @dataclass
 class WebsocketRequest:
     action: str
     device_name: str
     message: str
+    token: str
 
-    def __init__(self, action: str, device_name: str = None, message: str = None) -> None:
+    def __init__(self, action: str, device_name: str = None, message: str = None, token: str = None) -> None:
         self.action = action
         self.device_name = device_name
         self.message = message
+        self.token = token
 
     def is_valid(self) -> bool:
+        # If there is an WS AUTH TOKEN, we check that the request has the token
+        auth_token = os.environ.get("GATEWAY_WS_AUTH_TOKEN", None)
+        if auth_token and auth_token != self.token:
+            return False
+
         # not valid if action is not in valid actions list
         if self.action not in VALID_ACTIONS:
             return False
         
         # if action is get device list, we don't need more arguments, so it's valid
         if self.action == ACT_GET_DEVICES_LIST:
             return True
+        
+        # Action is transfers msg to other ws clients so we need a message
+        if self.action == ACT_TRANSFERS_TO_WS_CLIENTS and self.message:
+            return True
 
         # if the device required is not registered it's not valid
         device = Manager.GetDevice(self.device_name)
         if not device:
             return False
 
         # if the action is send to device and there is no message, it's not valid
```

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/serial.py` & `bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/serial.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/device_connectors/socket_server.py` & `bondzai.gateway-0.0.8/bondzai/gateway/device_connectors/socket_server.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai/gateway/tests/test_observer.py` & `bondzai.gateway-0.0.8/bondzai/gateway/tests/test_observer.py`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/bondzai.gateway.egg-info/PKG-INFO` & `bondzai.gateway-0.0.8/bondzai.gateway.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bondzai.gateway
-Version: 0.0.7
+Version: 0.0.8
 Summary: Bondzai Gateway
 Home-page: UNKNOWN
 Author: Bondzai
 License: Apache License 2.0
 Keywords: davinsy,bondzai,gateway
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bondzai.gateway-0.0.7/bondzai.gateway.egg-info/SOURCES.txt` & `bondzai.gateway-0.0.8/bondzai.gateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bondzai.gateway-0.0.7/setup.cfg` & `bondzai.gateway-0.0.8/setup.cfg`

 * *Files identical despite different names*

