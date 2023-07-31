# Comparing `tmp/airtouch5py-0.2.6.tar.gz` & `tmp/airtouch5py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.6.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.7.tar", max compression
```

## Comparing `airtouch5py-0.2.6.tar` & `airtouch5py-0.2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/LICENSE
--rw-r--r--   0        0        0       47 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/README.md
--rw-r--r--   0        0        0     4853 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     9683 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2208 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15561 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-31 02:19:02.844680 airtouch5py-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/LICENSE
+-rw-r--r--   0        0        0       47 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/README.md
+-rw-r--r--   0        0        0     4986 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     9683 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2208 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20400 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15561 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.7/PKG-INFO
```

### Comparing `airtouch5py-0.2.6/LICENSE` & `airtouch5py-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.7/airtouch5py/airtouch5_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import binascii
 import logging
 from enum import Enum
 
 from airtouch5py.data_packet_factory import DataPacketFactory
 
 from airtouch5py.packet_encoder import PacketEncoder
 from airtouch5py.packet_reader import PacketReader
@@ -109,14 +110,15 @@
         reader = self._reader
         if reader is None:
             raise Exception("Reader is None")
 
         try:
             while reader.at_eof() == False:
                 read = await reader.read(1024)
+                _LOGGER.debug(f"Received data: {binascii.hexlify(read)}")
                 packets = self._packet_reader.read(read)
                 for packet in packets:
                     self.packets_received.put_nowait(packet)
         except Exception as e:
             _LOGGER.error(f"Exception in reader task: {e}")
 
         # If we've finished reading for some reason, we should disconnect
@@ -129,15 +131,16 @@
         Send the given packet to the airtouch 5.
         Throws if we aren't connected or if there is a connection issue
         """
         writer = self._writer
         if writer is None:
             raise Exception("Writer is None")
 
-        _LOGGER.debug(f"Sending packet {packet}")
         try:
-            writer.write(self._encoder.encode(packet))
+            data = self._encoder.encode(packet)
+            _LOGGER.debug(f"Sending data: {binascii.hexlify(data)}")
+            writer.write(data)
             await writer.drain()
         except Exception as e:
             _LOGGER.error(f"Exception when sending packet: {e}")
             await self.disconnect()
             raise e
```

### Comparing `airtouch5py-0.2.6/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.7/airtouch5py/airtouch5_simple_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.7/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.7/airtouch5py/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.7/airtouch5py/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packet_reader.py` & `airtouch5py-0.2.7/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.7/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.7/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.7/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.7/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.7/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.6/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.7/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

