# Comparing `tmp/airtouch5py-0.2.5.tar.gz` & `tmp/airtouch5py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.5.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.6.tar", max compression
```

## Comparing `airtouch5py-0.2.5.tar` & `airtouch5py-0.2.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/LICENSE
--rw-r--r--   0        0        0       47 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/README.md
--rw-r--r--   0        0        0     4853 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     8614 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2208 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15561 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-29 21:32:54.814858 airtouch5py-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/README.md
+-rw-r--r--   0        0        0     4853 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     9683 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2208 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15561 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.6/PKG-INFO
```

### Comparing `airtouch5py-0.2.5/LICENSE` & `airtouch5py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.6/airtouch5py/airtouch5_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.6/airtouch5py/airtouch5_simple_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,28 +150,51 @@
         return await asyncio.wait_for(_read_packets_until_match(), 5)
 
     async def _maintain_connection(self) -> None:
         """
         Read messages off the queue, reconnecting if we disconnect.
         Calls the matching callbacks.
         """
+
+        # AirTouch5 doesn't send any packets if nothing is changing.
+        # So we periodically send a packet to test if the connection is alive.
+        have_sent_keep_alive_packet = False
+
         while True:
-            # Wait for a packet, or timeout after 5 minutes
+            # Wait for a packet, send one after 4 minutes, or timeout after 4+1 minutes
             packet: DataPacket | Airtouch5ConnectionStateChange
             try:
                 packet = await asyncio.wait_for(
-                    self._client.packets_received.get(), 5 * 60
+                    self._client.packets_received.get(),
+                    1 * 60 if have_sent_keep_alive_packet else 4 * 60,
                 )
             except asyncio.TimeoutError:
-                _LOGGER.error("Timeout waiting for packet, reconnecting")
-                await self._client.disconnect()
-                # disconnect pushes a DISCONNECTED message in to the queue, so we'll reconnect
-                continue
+                if not have_sent_keep_alive_packet:
+                    # send something to test the connection
+                    try:
+                        await self._client.send_packet(
+                            self.data_packet_factory.console_version_request()
+                        )
+                        have_sent_keep_alive_packet = True
+                    except:
+                        # Ignore, send_packet will disconnect if it fails
+                        _LOGGER.info(
+                            "Failed to send keep alive packet, connection must be dead"
+                        )
+                    continue
+                else:
+                    _LOGGER.error("Timeout waiting for packet, reconnecting")
+                    await self._client.disconnect()
+                    have_sent_keep_alive_packet = False
+                    # disconnect pushes a DISCONNECTED message in to the queue, so we'll reconnect
+                    continue
 
             _LOGGER.debug(f"maintain Received packet {packet}")
+            have_sent_keep_alive_packet = False
+
             if packet is Airtouch5ConnectionStateChange.DISCONNECTED:
                 [cb(packet) for cb in self.connection_state_callbacks]
                 _LOGGER.warning("Disconnected from Airtouch 5, reconnecting")
                 while True:
                     try:
                         await self._client.connect()
                         break
```

### Comparing `airtouch5py-0.2.5/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.6/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.6/airtouch5py/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.6/airtouch5py/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packet_reader.py` & `airtouch5py-0.2.6/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.6/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.6/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.6/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.6/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.6/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.5/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.6/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

