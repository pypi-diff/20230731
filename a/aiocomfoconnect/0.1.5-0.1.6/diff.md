# Comparing `tmp/aiocomfoconnect-0.1.5.tar.gz` & `tmp/aiocomfoconnect-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocomfoconnect-0.1.5.tar", max compression
+gzip compressed data, was "aiocomfoconnect-0.1.6.tar", max compression
```

## Comparing `aiocomfoconnect-0.1.5.tar` & `aiocomfoconnect-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.5/LICENSE
--rw-r--r--   0        0        0     5764 2022-12-16 21:29:08.419287 aiocomfoconnect-0.1.5/README.md
--rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.5/aiocomfoconnect/__init__.py
--rw-r--r--   0        0        0     7863 2022-12-16 21:38:22.901771 aiocomfoconnect-0.1.5/aiocomfoconnect/__main__.py
--rw-r--r--   0        0        0    20119 2022-12-16 20:56:56.207639 aiocomfoconnect-0.1.5/aiocomfoconnect/bridge.py
--rw-r--r--   0        0        0    19319 2022-12-16 21:36:32.618442 aiocomfoconnect-0.1.5/aiocomfoconnect/comfoconnect.py
--rw-r--r--   0        0        0     9341 2022-12-16 20:52:49.305149 aiocomfoconnect-0.1.5/aiocomfoconnect/const.py
--rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.5/aiocomfoconnect/discovery.py
--rw-r--r--   0        0        0     1184 2022-12-16 20:52:19.762650 aiocomfoconnect-0.1.5/aiocomfoconnect/exceptions.py
--rw-r--r--   0        0        0     1129 2022-12-16 21:20:35.038454 aiocomfoconnect-0.1.5/aiocomfoconnect/properties.py
--rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.5/aiocomfoconnect/protobuf/nanopb_pb2.py
--rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.5/aiocomfoconnect/protobuf/zehnder_pb2.py
--rw-r--r--   0        0        0     9977 2022-12-16 20:52:33.152649 aiocomfoconnect-0.1.5/aiocomfoconnect/sensors.py
--rw-r--r--   0        0        0     1203 2022-12-16 19:25:07.186887 aiocomfoconnect-0.1.5/aiocomfoconnect/util.py
--rw-r--r--   0        0        0     2394 2022-12-16 21:44:55.566768 aiocomfoconnect-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     6791 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.5/setup.py
--rw-r--r--   0        0        0     6520 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1133 2022-11-14 19:35:15.185394 aiocomfoconnect-0.1.6/LICENSE
+-rw-r--r--   0        0        0     5826 2023-07-31 09:48:20.130139 aiocomfoconnect-0.1.6/README.md
+-rw-r--r--   0        0        0      263 2022-12-16 20:50:33.736818 aiocomfoconnect-0.1.6/aiocomfoconnect/__init__.py
+-rw-r--r--   0        0        0     9118 2023-07-31 09:48:20.130139 aiocomfoconnect-0.1.6/aiocomfoconnect/__main__.py
+-rw-r--r--   0        0        0    20942 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.6/aiocomfoconnect/bridge.py
+-rw-r--r--   0        0        0    19319 2023-04-06 04:27:11.595081 aiocomfoconnect-0.1.6/aiocomfoconnect/comfoconnect.py
+-rw-r--r--   0        0        0     9341 2022-12-16 20:52:49.305149 aiocomfoconnect-0.1.6/aiocomfoconnect/const.py
+-rw-r--r--   0        0        0     2796 2022-12-16 20:52:49.294316 aiocomfoconnect-0.1.6/aiocomfoconnect/discovery.py
+-rw-r--r--   0        0        0     1297 2023-04-11 07:07:54.292758 aiocomfoconnect-0.1.6/aiocomfoconnect/exceptions.py
+-rw-r--r--   0        0        0     1129 2022-12-16 21:20:35.038454 aiocomfoconnect-0.1.6/aiocomfoconnect/properties.py
+-rw-r--r--   0        0        0     2776 2022-12-16 19:59:11.317713 aiocomfoconnect-0.1.6/aiocomfoconnect/protobuf/nanopb_pb2.py
+-rw-r--r--   0        0        0    29853 2022-11-08 09:06:10.920864 aiocomfoconnect-0.1.6/aiocomfoconnect/protobuf/zehnder_pb2.py
+-rw-r--r--   0        0        0     9977 2023-04-06 04:55:14.628771 aiocomfoconnect-0.1.6/aiocomfoconnect/sensors.py
+-rw-r--r--   0        0        0     1203 2022-12-16 19:25:07.186887 aiocomfoconnect-0.1.6/aiocomfoconnect/util.py
+-rw-r--r--   0        0        0     2394 2023-07-31 09:47:48.640141 aiocomfoconnect-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     6582 1970-01-01 00:00:00.000000 aiocomfoconnect-0.1.6/PKG-INFO
```

### Comparing `aiocomfoconnect-0.1.5/LICENSE` & `aiocomfoconnect-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/README.md` & `aiocomfoconnect-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 $ python -m aiocomfoconnect discover
 
 $ python -m aiocomfoconnect register --host 192.168.1.213
 
 $ python -m aiocomfoconnect set-speed away --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed low --host 192.168.1.213
+$ python -m aiocomfoconnect set-mode auto --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed medium --host 192.168.1.213
 $ python -m aiocomfoconnect set-speed high --host 192.168.1.213
 
 $ python -m aiocomfoconnect show-sensors --host 192.168.1.213
 $ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213
 ```
 
@@ -136,15 +137,15 @@
 
 - [ComfoConnect LAN C Protocol](docs/PROTOCOL.md)
 - [PDO Sensors](docs/PROTOCOL-PDO.md)
 - [RMI commands](docs/PROTOCOL-RMI.md)
 
 ### Decode network traffic
 
-You can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C. 
+You can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C.
 Make sure that the first TCP session in the capture is the connection between the bridge and the app. It's therefore recommended to start the capture before you open the app.
 
 ```shell
 $ sudo tcpdump -i any -s 0 -w /tmp/capture.pcap tcp and port 56747
 $ python scripts/decode_pcap.py /tmp/capture.pcap
 ```
```

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/__main__.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Literal
 
 from aiocomfoconnect import DEFAULT_NAME, DEFAULT_PIN, DEFAULT_UUID
 from aiocomfoconnect.comfoconnect import ComfoConnect
 from aiocomfoconnect.discovery import discover_bridges
 from aiocomfoconnect.exceptions import (
     AioComfoConnectNotConnected,
+    AioComfoConnectTimeout,
     ComfoConnectNotAllowed,
 )
 from aiocomfoconnect.sensors import SENSORS
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -27,14 +28,17 @@
 
     elif args.action == "register":
         await run_register(args.host, args.uuid, args.name, args.pin)
 
     elif args.action == "set-speed":
         await run_set_speed(args.host, args.uuid, args.speed)
 
+    elif args.action == "set-mode":
+        await run_set_mode(args.host, args.uuid, args.mode)
+
     elif args.action == "show-sensors":
         await run_show_sensors(args.host, args.uuid)
 
     elif args.action == "show-sensor":
         await run_show_sensor(args.host, args.uuid, args.sensor)
 
     else:
@@ -105,14 +109,34 @@
         sys.exit(1)
 
     await comfoconnect.set_speed(speed)
 
     await comfoconnect.disconnect()
 
 
+async def run_set_mode(host: str, uuid: str, mode: Literal["auto", "manual"]):
+    """Connect to a bridge."""
+    # Discover bridge so we know the UUID
+    bridges = await discover_bridges(host)
+    if not bridges:
+        raise Exception("No bridge found")
+
+    # Connect to the bridge
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid)
+    try:
+        await comfoconnect.connect(uuid)
+    except ComfoConnectNotAllowed:
+        print("Could not connect to bridge. Please register first.")
+        sys.exit(1)
+
+    await comfoconnect.set_mode(mode)
+
+    await comfoconnect.disconnect()
+
+
 async def run_show_sensors(host: str, uuid: str):
     """Connect to a bridge."""
     # Discover bridge so we know the UUID
     bridges = await discover_bridges(host)
     if not bridges:
         raise Exception("No bridge found")
 
@@ -136,23 +160,28 @@
 
     # Register all sensors
     for sensor in SENSORS.values():
         await comfoconnect.register_sensor(sensor)
 
     try:
         while True:
-            # Wait for updates and send a keepalive every 60 seconds
-            await asyncio.sleep(60)
+            # Wait for updates and send a keepalive every 30 seconds
+            await asyncio.sleep(30)
 
             try:
                 print("Sending keepalive...")
-                await comfoconnect.cmd_keepalive()
-            except AioComfoConnectNotConnected:
+                # Use cmd_time_request as a keepalive since cmd_keepalive doesn't send back a reply we can wait for
+                await comfoconnect.cmd_time_request()
+
+            except (AioComfoConnectNotConnected, AioComfoConnectTimeout):
                 # Reconnect when connection has been dropped
-                await comfoconnect.connect(uuid)
+                try:
+                    await comfoconnect.connect(uuid)
+                except AioComfoConnectTimeout:
+                    _LOGGER.warning("Connection timed out. Retrying later...")
 
     except KeyboardInterrupt:
         pass
 
     print("Disconnecting...")
     await comfoconnect.disconnect()
 
@@ -167,16 +196,15 @@
         raise Exception("No bridge found")
 
     def sensor_callback(sensor_, value):
         """Print sensor update."""
         result.set_result(value)
 
     # Connect to the bridge
-    # Increase sensor_delay if you get 0 values. This is a bug in the firmware.
-    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid, sensor_callback=sensor_callback, sensor_delay=0)
+    comfoconnect = ComfoConnect(bridges[0].host, bridges[0].uuid, sensor_callback=sensor_callback)
     try:
         await comfoconnect.connect(uuid)
     except ComfoConnectNotAllowed:
         print("Could not connect to bridge. Please register first.")
         sys.exit(1)
 
     if not sensor in SENSORS:
@@ -208,14 +236,19 @@
     p_register.add_argument("--name", help="Name of this app", default=DEFAULT_NAME)
 
     p_set_speed = subparsers.add_parser("set-speed", help="set the fan speed")
     p_set_speed.add_argument("speed", help="Fan speed", choices=["low", "medium", "high", "away"])
     p_set_speed.add_argument("--host", help="Host address of the bridge")
     p_set_speed.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
+    p_set_mode = subparsers.add_parser("set-mode", help="set operation mode")
+    p_set_mode.add_argument("mode", help="Operation mode", choices=["auto", "manual"])
+    p_set_mode.add_argument("--host", help="Host address of the bridge")
+    p_set_mode.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
+
     p_sensors = subparsers.add_parser("show-sensors", help="show the sensor values")
     p_sensors.add_argument("--host", help="Host address of the bridge")
     p_sensors.add_argument("--uuid", help="UUID of this app", default=DEFAULT_UUID)
 
     p_sensor = subparsers.add_parser("show-sensor", help="show a single sensor value")
     p_sensor.add_argument("sensor", help="The ID of the sensor", type=int)
     p_sensor.add_argument("--host", help="Host address of the bridge")
```

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/bridge.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/bridge.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """ ComfoConnect Bridge API """
 from __future__ import annotations
 
 import asyncio
 import logging
 import struct
 from asyncio import IncompleteReadError, StreamReader, StreamWriter
+from typing import Awaitable
 
 from google.protobuf.message import DecodeError
 from google.protobuf.message import Message as ProtobufMessage
 
 from .exceptions import (
     AioComfoConnectNotConnected,
+    AioComfoConnectTimeout,
     ComfoConnectBadRequest,
     ComfoConnectError,
     ComfoConnectInternalError,
     ComfoConnectNoResources,
     ComfoConnectNotAllowed,
     ComfoConnectNotExist,
     ComfoConnectNotReachable,
     ComfoConnectOtherSession,
     ComfoConnectRmiError,
 )
 from .protobuf import zehnder_pb2
 
 _LOGGER = logging.getLogger(__name__)
 
+TIMEOUT = 5
+
 
 class EventBus:
     """An event bus for async replies."""
 
     def __init__(self):
         self.listeners = {}
 
@@ -83,44 +87,55 @@
 
     def set_alarm_callback(self, callback: callable):
         """Set a callback to be called when an alarm is received."""
         self.__alarm_callback_fn = callback
 
     async def connect(self, uuid: str):
         """Connect to the bridge."""
+        await self.disconnect()
+
         _LOGGER.debug("Connecting to bridge %s", self.host)
-        self._reader, self._writer = await asyncio.open_connection(self.host, self.PORT)
+        try:
+            self._reader, self._writer = await asyncio.wait_for(asyncio.open_connection(self.host, self.PORT), TIMEOUT)
+        except asyncio.TimeoutError as exc:
+            raise AioComfoConnectTimeout() from exc
+
         self._reference = 1
         self._local_uuid = uuid
         self._event_bus = EventBus()
 
         # We are connected, start the background task
         self._read_task = self._loop.create_task(self._read_messages())
 
+        _LOGGER.debug("Connected to bridge %s", self.host)
+
     async def disconnect(self):
         """Disconnect from the bridge."""
         _LOGGER.debug("Disconnecting from bridge %s", self.host)
 
-        # Cancel the background task
-        self._read_task.cancel()
+        if self._read_task:
+            # Cancel the background task
+            self._read_task.cancel()
+
+            # Wait for background task to finish
+            try:
+                await self._read_task
+            except asyncio.CancelledError:
+                pass
 
-        # Disconnect
-        await self.cmd_close_session()
+        if self._writer:
+            self._writer.close()
 
-        # Wait for background task to finish
-        try:
-            await self._read_task
-        except asyncio.CancelledError:
-            pass
+        _LOGGER.debug("Disconnected from bridge %s", self.host)
 
     def is_connected(self) -> bool:
         """Returns True if the bridge is connected."""
         return self._writer is not None and not self._writer.is_closing()
 
-    def _send(self, request, request_type, params: dict = None, reply: bool = True) -> Message:
+    async def _send(self, request, request_type, params: dict = None, reply: bool = True) -> Message:
         """Sends a command and wait for a response if the request is known to return a result."""
         # Check if we are actually connected
         if not self.is_connected():
             raise AioComfoConnectNotConnected()
 
         # Construct the message
         cmd = zehnder_pb2.GatewayOperation()  # pylint: disable=no-member
@@ -145,15 +160,19 @@
         # Send the message
         _LOGGER.debug("TX %s", message)
         self._writer.write(message.encode())
 
         # Increase message reference for next message
         self._reference += 1
 
-        return fut
+        try:
+            return await asyncio.wait_for(fut, TIMEOUT)
+        except asyncio.TimeoutError as exc:
+            _LOGGER.warning("Timeout while waiting for response from bridge")
+            raise AioComfoConnectTimeout from exc
 
     async def _read(self) -> Message:
         # Read packet size
         msg_len_buf = await self._reader.readexactly(4)
 
         # Read rest of packet
         msg_len = int.from_bytes(msg_len_buf, byteorder="big")
@@ -233,111 +252,109 @@
             except ComfoConnectError as exc:
                 if exc.message.cmd.reference:
                     self._event_bus.emit(exc.message.cmd.reference, exc)
 
             except DecodeError as exc:
                 _LOGGER.error("Failed to decode message: %s", exc)
 
-    def cmd_start_session(self, take_over: bool = False):
+    def cmd_start_session(self, take_over: bool = False) -> Awaitable[Message]:
         """Starts the session on the device by logging in and optionally disconnecting an already existing session."""
         _LOGGER.debug("StartSessionRequest")
         # pylint: disable=no-member
-        result = self._send(
+        return self._send(
             zehnder_pb2.StartSessionRequest,
             zehnder_pb2.GatewayOperation.StartSessionRequestType,
             {"takeover": take_over},
         )
-        return result
 
-    def cmd_close_session(self):
+    def cmd_close_session(self) -> Awaitable[Message]:
         """Stops the current session."""
         _LOGGER.debug("CloseSessionRequest")
         # pylint: disable=no-member
-        result = self._send(
+        return self._send(
             zehnder_pb2.CloseSessionRequest,
             zehnder_pb2.GatewayOperation.CloseSessionRequestType,
             reply=False,  # Don't wait for a reply
         )
-        return result
 
-    def cmd_list_registered_apps(self):
+    def cmd_list_registered_apps(self) -> Awaitable[Message]:
         """Returns a list of all the registered clients."""
         _LOGGER.debug("ListRegisteredAppsRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.ListRegisteredAppsRequest,
             zehnder_pb2.GatewayOperation.ListRegisteredAppsRequestType,
         )
 
-    def cmd_register_app(self, uuid: str, device_name: str, pin: int):
+    def cmd_register_app(self, uuid: str, device_name: str, pin: int) -> Awaitable[Message]:
         """Register a new app by specifying our own uuid, device_name and pin code."""
         _LOGGER.debug("RegisterAppRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.RegisterAppRequest,
             zehnder_pb2.GatewayOperation.RegisterAppRequestType,
             {
                 "uuid": bytes.fromhex(uuid),
                 "devicename": device_name,
                 "pin": int(pin),
             },
         )
 
-    def cmd_deregister_app(self, uuid: str):
+    def cmd_deregister_app(self, uuid: str) -> Awaitable[Message]:
         """Remove the specified app from the registration list."""
         _LOGGER.debug("DeregisterAppRequest")
         if uuid == self._local_uuid:
             raise Exception("You should not deregister yourself.")
 
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.DeregisterAppRequest,
             zehnder_pb2.GatewayOperation.DeregisterAppRequestType,
             {"uuid": bytes.fromhex(uuid)},
         )
 
-    def cmd_version_request(self):
+    def cmd_version_request(self) -> Awaitable[Message]:
         """Returns version information."""
         _LOGGER.debug("VersionRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.VersionRequest,
             zehnder_pb2.GatewayOperation.VersionRequestType,
         )
 
-    def cmd_time_request(self):
+    def cmd_time_request(self) -> Awaitable[Message]:
         """Returns the current time on the device."""
         _LOGGER.debug("CnTimeRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.CnTimeRequest,
             zehnder_pb2.GatewayOperation.CnTimeRequestType,
         )
 
-    def cmd_rmi_request(self, message, node_id: int = 1):
+    def cmd_rmi_request(self, message, node_id: int = 1) -> Awaitable[Message]:
         """Sends a RMI request."""
         _LOGGER.debug("CnRmiRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.CnRmiRequest,
             zehnder_pb2.GatewayOperation.CnRmiRequestType,
             {"nodeId": node_id or 1, "message": message},
         )
 
-    def cmd_rpdo_request(self, pdid: int, pdo_type: int = 1, zone: int = 1, timeout=None):
+    def cmd_rpdo_request(self, pdid: int, pdo_type: int = 1, zone: int = 1, timeout=None) -> Awaitable[Message]:
         """Register a RPDO request."""
         _LOGGER.debug("CnRpdoRequest")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.CnRpdoRequest,
             zehnder_pb2.GatewayOperation.CnRpdoRequestType,
             {"pdid": pdid, "type": pdo_type, "zone": zone or 1, "timeout": timeout},
         )
 
-    def cmd_keepalive(self):
+    def cmd_keepalive(self) -> Awaitable[Message]:
         """Sends a keepalive."""
         _LOGGER.debug("KeepAlive")
         # pylint: disable=no-member
         return self._send(
             zehnder_pb2.KeepAlive,
             zehnder_pb2.GatewayOperation.KeepAliveType,
             reply=False,  # Don't wait for a reply
```

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/comfoconnect.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/comfoconnect.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/const.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/const.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/discovery.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/discovery.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/exceptions.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,8 +38,12 @@
 
 
 class ComfoConnectRmiError(ComfoConnectError):
     """The RMI failed, the message contains the error response."""
 
 
 class AioComfoConnectNotConnected(Exception):
-    """An error occured because the bridge is not connected."""
+    """An error occurred because the bridge is not connected."""
+
+
+class AioComfoConnectTimeout(Exception):
+    """An error occurred because the bridge didn't reply in time."""
```

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/properties.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/properties.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/protobuf/nanopb_pb2.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/protobuf/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/protobuf/zehnder_pb2.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/protobuf/zehnder_pb2.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/sensors.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/sensors.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/aiocomfoconnect/util.py` & `aiocomfoconnect-0.1.6/aiocomfoconnect/util.py`

 * *Files identical despite different names*

### Comparing `aiocomfoconnect-0.1.5/pyproject.toml` & `aiocomfoconnect-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiocomfoconnect"
-version = "0.1.5"
+version = "0.1.6"
 description = "aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system"
 authors = ["Michaël Arnauts <michael.arnauts@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/michaelarnauts/aiocomfoconnect"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `aiocomfoconnect-0.1.5/setup.py` & `aiocomfoconnect-0.1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,177 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aiocomfoconnect
+Version: 0.1.6
+Summary: aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system
+Home-page: https://github.com/michaelarnauts/aiocomfoconnect
+Author: Michaël Arnauts
+Author-email: michael.arnauts@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
+Requires-Dist: nanopb (>=0.4.6,<0.5.0)
+Requires-Dist: protobuf (>=4.21.9,<5.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['aiocomfoconnect', 'aiocomfoconnect.protobuf']
+# aiocomfoconnect
 
-package_data = \
-{'': ['*']}
+`aiocomfoconnect` is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system. It's the successor of
+[comfoconnect](https://github.com/michaelarnauts/comfoconnect).
 
-install_requires = \
-['aiohttp>=3.8.0,<4.0.0', 'nanopb>=0.4.6,<0.5.0', 'protobuf>=4.21.9,<5.0.0']
-
-setup_kwargs = {
-    'name': 'aiocomfoconnect',
-    'version': '0.1.5',
-    'description': 'aiocomfoconnect is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system',
-    'long_description': '# aiocomfoconnect\n\n`aiocomfoconnect` is an asyncio Python 3 library for communicating with a Zehnder ComfoAir Q350/450/600 ventilation system. It\'s the successor of\n[comfoconnect](https://github.com/michaelarnauts/comfoconnect).\n\nIt\'s compatible with Python 3.8 and higher.\n\n## Installation\n\n```shell\npip3 install aiocomfoconnect\n```\n\n## CLI Usage\n\n```shell\n$ python -m aiocomfoconnect --help\n\n$ python -m aiocomfoconnect discover\n\n$ python -m aiocomfoconnect register --host 192.168.1.213\n\n$ python -m aiocomfoconnect set-speed away --host 192.168.1.213\n$ python -m aiocomfoconnect set-speed low --host 192.168.1.213\n$ python -m aiocomfoconnect set-speed medium --host 192.168.1.213\n$ python -m aiocomfoconnect set-speed high --host 192.168.1.213\n\n$ python -m aiocomfoconnect show-sensors --host 192.168.1.213\n$ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213\n```\n\n## Available methods\n\n- `async connect()`: Connect to the bridge.\n- `async disconnect()`: Disconnect from the bridge.\n- `async register_sensor(sensor)`: Register a sensor.\n- `async deregister_sensor(sensor)`: Deregister a sensor.\n- `async get_mode()`: Get the ventilation mode.\n- `async set_mode(mode)`: Set the ventilation mode. (auto / manual)\n- `async get_speed()`: Get the ventilation speed.\n- `async set_speed(speed)`: Set the ventilation speed. (away / low / medium / high)\n- `async get_bypass()`: Get the bypass mode.\n- `async set_bypass(mode, timeout=-1)`: Set the bypass mode. (auto / on / off)\n- `async get_balance_mode()`: Get the balance mode.\n- `async set_balance_mode(mode, timeout=-1)`: Set the balance mode. (balance / supply only / exhaust only)\n- `async get_boost()`: Get the boost mode.\n- `async set_boost(mode, timeout=-1)`: Set the boost mode. (boolean)\n- `async get_away()`: Get the away mode.\n- `async set_away(mode, timeout=-1)`: Set the away mode. (boolean)\n- `async get_temperature_profile()`: Get the temperature profile.\n- `async set_temperature_profile(profile)`: Set the temperature profile. (warm / normal / cool)\n- `async get_sensor_ventmode_temperature_passive()`: Get the sensor based ventilation passive temperature control setting.\n- `async set_sensor_ventmode_temperature_passive(mode)`: Set the sensor based ventilation passive temperature control setting. (auto / on / off)\n- `async get_sensor_ventmode_humidity_comfort()`: Get the sensor based ventilation humidity comfort setting.\n- `async set_sensor_ventmode_humidity_comfort(mode)`: Set the sensor based ventilation humidity comfort setting. (auto / on / off)\n- `async get_sensor_ventmode_humidity_protection()`: Get the sensor based ventilation humidity protection setting.\n- `async set_sensor_ventmode_humidity_protection(mode)`: Set the sensor based ventilation humidity protection setting. (auto / on / off)\n\n### Low-level API\n\n- `async cmd_start_session()`: Start a session.\n- `async cmd_close_session()`: Close a session.\n- `async cmd_list_registered_apps()`: List registered apps.\n- `async cmd_register_app(uuid, device_name, pin)`: Register an app.\n- `async cmd_deregister_app(uuid)`: Deregister an app.\n- `async cmd_version_request()`: Request the bridge\'s version.\n- `async cmd_time_request()`: Request the bridge\'s time.\n- `async cmd_rmi_request(message, node_id)`: Send a RMI request.\n- `async cmd_rpdo_request(pdid, type, zone, timeout)`: Send a RPDO request.\n- `async cmd_keepalive()`: Send a keepalive message.\n\n## Examples\n\n### Discovery of ComfoConnect LAN C Bridges\n\n```python\nimport asyncio\n\nfrom aiocomfoconnect import discover_bridges\n\n\nasync def main():\n    """ ComfoConnect LAN C Bridge discovery example."""\n\n    # Discover all ComfoConnect LAN C Bridges on the subnet.\n    bridges = await discover_bridges()\n    print(bridges)\n\n\nif __name__ == "__main__":\n    asyncio.run(main())\n```\n\n### Basic Example\n\n```python\nimport asyncio\n\nfrom aiocomfoconnect import ComfoConnect\nfrom aiocomfoconnect.const import VentilationSpeed\nfrom aiocomfoconnect.sensors import SENSORS\n\n\nasync def main(local_uuid, host, uuid):\n    """ Basic example."""\n\n    def sensor_callback(sensor, value):\n        """ Print sensor updates. """\n        print(f"{sensor.name} = {value}")\n\n    # Connect to the Bridge\n    comfoconnect = ComfoConnect(host, uuid, sensor_callback=sensor_callback)\n    await comfoconnect.connect(local_uuid)\n\n    # Register all sensors\n    for key in SENSORS:\n        await comfoconnect.register_sensor(SENSORS[key])\n\n    # Set speed to LOW\n    await comfoconnect.set_speed(VentilationSpeed.LOW)\n\n    # Wait 2 minutes so we can see some sensor updates\n    await asyncio.sleep(120)\n\n    # Disconnect from the bridge\n    await comfoconnect.disconnect()\n\n\nif __name__ == "__main__":\n    asyncio.run(main(local_uuid=\'00000000000000000000000000001337\', host=\'192.168.1.20\', uuid=\'00000000000000000000000000000055\'))  # Replace with your bridge\'s IP and UUID\n```\n\n## Development Notes\n\n### Protocol Documentation\n\n- [ComfoConnect LAN C Protocol](docs/PROTOCOL.md)\n- [PDO Sensors](docs/PROTOCOL-PDO.md)\n- [RMI commands](docs/PROTOCOL-RMI.md)\n\n### Decode network traffic\n\nYou can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C. \nMake sure that the first TCP session in the capture is the connection between the bridge and the app. It\'s therefore recommended to start the capture before you open the app.\n\n```shell\n$ sudo tcpdump -i any -s 0 -w /tmp/capture.pcap tcp and port 56747\n$ python scripts/decode_pcap.py /tmp/capture.pcap\n```\n\n### Generate zehnder_pb2.py file\n\n```shell\npip3 install grpcio-tools\npython3 -m grpc_tools.protoc -Iprotobuf protobuf/nanopb.proto --python_out=aiocomfoconnect/protobuf\npython3 -m grpc_tools.protoc -Iprotobuf protobuf/zehnder.proto --python_out=aiocomfoconnect/protobuf\n```\n',
-    'author': 'Michaël Arnauts',
-    'author_email': 'michael.arnauts@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/michaelarnauts/aiocomfoconnect',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+It's compatible with Python 3.8 and higher.
 
+## Installation
+
+```shell
+pip3 install aiocomfoconnect
+```
+
+## CLI Usage
+
+```shell
+$ python -m aiocomfoconnect --help
+
+$ python -m aiocomfoconnect discover
+
+$ python -m aiocomfoconnect register --host 192.168.1.213
+
+$ python -m aiocomfoconnect set-speed away --host 192.168.1.213
+$ python -m aiocomfoconnect set-speed low --host 192.168.1.213
+$ python -m aiocomfoconnect set-mode auto --host 192.168.1.213
+$ python -m aiocomfoconnect set-speed medium --host 192.168.1.213
+$ python -m aiocomfoconnect set-speed high --host 192.168.1.213
+
+$ python -m aiocomfoconnect show-sensors --host 192.168.1.213
+$ python -m aiocomfoconnect show-sensor 276 --host 192.168.1.213
+```
+
+## Available methods
+
+- `async connect()`: Connect to the bridge.
+- `async disconnect()`: Disconnect from the bridge.
+- `async register_sensor(sensor)`: Register a sensor.
+- `async deregister_sensor(sensor)`: Deregister a sensor.
+- `async get_mode()`: Get the ventilation mode.
+- `async set_mode(mode)`: Set the ventilation mode. (auto / manual)
+- `async get_speed()`: Get the ventilation speed.
+- `async set_speed(speed)`: Set the ventilation speed. (away / low / medium / high)
+- `async get_bypass()`: Get the bypass mode.
+- `async set_bypass(mode, timeout=-1)`: Set the bypass mode. (auto / on / off)
+- `async get_balance_mode()`: Get the balance mode.
+- `async set_balance_mode(mode, timeout=-1)`: Set the balance mode. (balance / supply only / exhaust only)
+- `async get_boost()`: Get the boost mode.
+- `async set_boost(mode, timeout=-1)`: Set the boost mode. (boolean)
+- `async get_away()`: Get the away mode.
+- `async set_away(mode, timeout=-1)`: Set the away mode. (boolean)
+- `async get_temperature_profile()`: Get the temperature profile.
+- `async set_temperature_profile(profile)`: Set the temperature profile. (warm / normal / cool)
+- `async get_sensor_ventmode_temperature_passive()`: Get the sensor based ventilation passive temperature control setting.
+- `async set_sensor_ventmode_temperature_passive(mode)`: Set the sensor based ventilation passive temperature control setting. (auto / on / off)
+- `async get_sensor_ventmode_humidity_comfort()`: Get the sensor based ventilation humidity comfort setting.
+- `async set_sensor_ventmode_humidity_comfort(mode)`: Set the sensor based ventilation humidity comfort setting. (auto / on / off)
+- `async get_sensor_ventmode_humidity_protection()`: Get the sensor based ventilation humidity protection setting.
+- `async set_sensor_ventmode_humidity_protection(mode)`: Set the sensor based ventilation humidity protection setting. (auto / on / off)
+
+### Low-level API
+
+- `async cmd_start_session()`: Start a session.
+- `async cmd_close_session()`: Close a session.
+- `async cmd_list_registered_apps()`: List registered apps.
+- `async cmd_register_app(uuid, device_name, pin)`: Register an app.
+- `async cmd_deregister_app(uuid)`: Deregister an app.
+- `async cmd_version_request()`: Request the bridge's version.
+- `async cmd_time_request()`: Request the bridge's time.
+- `async cmd_rmi_request(message, node_id)`: Send a RMI request.
+- `async cmd_rpdo_request(pdid, type, zone, timeout)`: Send a RPDO request.
+- `async cmd_keepalive()`: Send a keepalive message.
+
+## Examples
+
+### Discovery of ComfoConnect LAN C Bridges
+
+```python
+import asyncio
+
+from aiocomfoconnect import discover_bridges
+
+
+async def main():
+    """ ComfoConnect LAN C Bridge discovery example."""
+
+    # Discover all ComfoConnect LAN C Bridges on the subnet.
+    bridges = await discover_bridges()
+    print(bridges)
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
+### Basic Example
+
+```python
+import asyncio
+
+from aiocomfoconnect import ComfoConnect
+from aiocomfoconnect.const import VentilationSpeed
+from aiocomfoconnect.sensors import SENSORS
+
+
+async def main(local_uuid, host, uuid):
+    """ Basic example."""
+
+    def sensor_callback(sensor, value):
+        """ Print sensor updates. """
+        print(f"{sensor.name} = {value}")
+
+    # Connect to the Bridge
+    comfoconnect = ComfoConnect(host, uuid, sensor_callback=sensor_callback)
+    await comfoconnect.connect(local_uuid)
+
+    # Register all sensors
+    for key in SENSORS:
+        await comfoconnect.register_sensor(SENSORS[key])
+
+    # Set speed to LOW
+    await comfoconnect.set_speed(VentilationSpeed.LOW)
+
+    # Wait 2 minutes so we can see some sensor updates
+    await asyncio.sleep(120)
+
+    # Disconnect from the bridge
+    await comfoconnect.disconnect()
+
+
+if __name__ == "__main__":
+    asyncio.run(main(local_uuid='00000000000000000000000000001337', host='192.168.1.20', uuid='00000000000000000000000000000055'))  # Replace with your bridge's IP and UUID
+```
+
+## Development Notes
+
+### Protocol Documentation
+
+- [ComfoConnect LAN C Protocol](docs/PROTOCOL.md)
+- [PDO Sensors](docs/PROTOCOL-PDO.md)
+- [RMI commands](docs/PROTOCOL-RMI.md)
+
+### Decode network traffic
+
+You can use the `scripts/decode_pcap.py` file to decode network traffic between the Mobile App and the ComfoConnect LAN C.
+Make sure that the first TCP session in the capture is the connection between the bridge and the app. It's therefore recommended to start the capture before you open the app.
+
+```shell
+$ sudo tcpdump -i any -s 0 -w /tmp/capture.pcap tcp and port 56747
+$ python scripts/decode_pcap.py /tmp/capture.pcap
+```
+
+### Generate zehnder_pb2.py file
+
+```shell
+pip3 install grpcio-tools
+python3 -m grpc_tools.protoc -Iprotobuf protobuf/nanopb.proto --python_out=aiocomfoconnect/protobuf
+python3 -m grpc_tools.protoc -Iprotobuf protobuf/zehnder.proto --python_out=aiocomfoconnect/protobuf
+```
 
-setup(**setup_kwargs)
```

