# Comparing `tmp/HAP-python-4.7.0.tar.gz` & `tmp/HAP-python-4.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HAP-python-4.7.0.tar", last modified: Sun Jun 18 12:00:48 2023, max compression
+gzip compressed data, was "HAP-python-4.7.1.tar", last modified: Mon Jul 31 19:16:35 2023, max compression
```

## Comparing `HAP-python-4.7.0.tar` & `HAP-python-4.7.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.479140 HAP-python-4.7.0/
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.473441 HAP-python-4.7.0/HAP_python.egg-info/
--rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)      691 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/SOURCES.txt
--rw-r--r--   0 ivan       (501) staff       (20)        1 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/dependency_links.txt
--rw-r--r--   0 ivan       (501) staff       (20)      101 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/requires.txt
--rw-r--r--   0 ivan       (501) staff       (20)        6 2023-06-18 12:00:48.000000 HAP-python-4.7.0/HAP_python.egg-info/top_level.txt
--rw-r--r--   0 ivan       (501) staff       (20)    12247 2023-06-18 11:42:25.000000 HAP-python-4.7.0/LICENSE
--rw-r--r--   0 ivan       (501) staff       (20)       61 2023-06-18 11:42:25.000000 HAP-python-4.7.0/MANIFEST.in
--rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-06-18 12:00:48.479205 HAP-python-4.7.0/PKG-INFO
--rw-r--r--   0 ivan       (501) staff       (20)    12362 2023-06-18 11:59:57.000000 HAP-python-4.7.0/README.md
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.478281 HAP-python-4.7.0/pyhap/
--rw-r--r--   0 ivan       (501) staff       (20)      497 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/__init__.py
--rw-r--r--   0 ivan       (501) staff       (20)    13393 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/accessory.py
--rw-r--r--   0 ivan       (501) staff       (20)    35373 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/accessory_driver.py
--rw-r--r--   0 ivan       (501) staff       (20)    34138 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/camera.py
--rw-r--r--   0 ivan       (501) staff       (20)    13435 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/characteristic.py
--rw-r--r--   0 ivan       (501) staff       (20)     2709 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/const.py
--rw-r--r--   0 ivan       (501) staff       (20)     4928 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/encoder.py
--rw-r--r--   0 ivan       (501) staff       (20)     4207 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_crypto.py
--rw-r--r--   0 ivan       (501) staff       (20)      551 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_event.py
--rw-r--r--   0 ivan       (501) staff       (20)    30302 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/hap_handler.py
--rw-r--r--   0 ivan       (501) staff       (20)    10729 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_protocol.py
--rw-r--r--   0 ivan       (501) staff       (20)     3104 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hap_server.py
--rw-r--r--   0 ivan       (501) staff       (20)     3344 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/hsrp.py
--rw-r--r--   0 ivan       (501) staff       (20)     1936 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/iid_manager.py
--rw-r--r--   0 ivan       (501) staff       (20)     2371 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/loader.py
--rw-r--r--   0 ivan       (501) staff       (20)     1254 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/params.py
-drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-06-18 12:00:48.478778 HAP-python-4.7.0/pyhap/resources/
--rw-r--r--   0 ivan       (501) staff       (20)    35625 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/characteristics.json
--rw-r--r--   0 ivan       (501) staff       (20)    14516 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/services.json
--rw-r--r--   0 ivan       (501) staff       (20)   203005 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/resources/snapshot.jpg
--rw-r--r--   0 ivan       (501) staff       (20)     4653 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/service.py
--rw-r--r--   0 ivan       (501) staff       (20)     4010 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/state.py
--rw-r--r--   0 ivan       (501) staff       (20)     2212 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyhap/tlv.py
--rw-r--r--   0 ivan       (501) staff       (20)     4156 2023-06-18 11:59:57.000000 HAP-python-4.7.0/pyhap/util.py
--rw-r--r--   0 ivan       (501) staff       (20)     2648 2023-06-18 11:42:25.000000 HAP-python-4.7.0/pyproject.toml
--rw-r--r--   0 ivan       (501) staff       (20)      107 2023-06-18 12:00:48.479519 HAP-python-4.7.0/setup.cfg
--rw-r--r--   0 ivan       (501) staff       (20)     1887 2023-06-18 11:42:25.000000 HAP-python-4.7.0/setup.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-31 19:16:35.403199 HAP-python-4.7.1/
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-31 19:16:35.398771 HAP-python-4.7.1/HAP_python.egg-info/
+-rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-07-31 19:16:35.000000 HAP-python-4.7.1/HAP_python.egg-info/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)      691 2023-07-31 19:16:35.000000 HAP-python-4.7.1/HAP_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        1 2023-07-31 19:16:35.000000 HAP-python-4.7.1/HAP_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan       (501) staff       (20)      115 2023-07-31 19:16:35.000000 HAP-python-4.7.1/HAP_python.egg-info/requires.txt
+-rw-r--r--   0 ivan       (501) staff       (20)        6 2023-07-31 19:16:35.000000 HAP-python-4.7.1/HAP_python.egg-info/top_level.txt
+-rw-r--r--   0 ivan       (501) staff       (20)    12247 2023-06-18 11:42:25.000000 HAP-python-4.7.1/LICENSE
+-rw-r--r--   0 ivan       (501) staff       (20)       61 2023-06-18 11:42:25.000000 HAP-python-4.7.1/MANIFEST.in
+-rw-r--r--   0 ivan       (501) staff       (20)    13612 2023-07-31 19:16:35.403255 HAP-python-4.7.1/PKG-INFO
+-rw-r--r--   0 ivan       (501) staff       (20)    12362 2023-06-18 11:59:57.000000 HAP-python-4.7.1/README.md
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-31 19:16:35.402426 HAP-python-4.7.1/pyhap/
+-rw-r--r--   0 ivan       (501) staff       (20)      497 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/__init__.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13393 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/accessory.py
+-rw-r--r--   0 ivan       (501) staff       (20)    35373 2023-06-18 11:59:57.000000 HAP-python-4.7.1/pyhap/accessory_driver.py
+-rw-r--r--   0 ivan       (501) staff       (20)    34149 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/camera.py
+-rw-r--r--   0 ivan       (501) staff       (20)    13435 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/characteristic.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2709 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/const.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4928 2023-06-18 11:59:57.000000 HAP-python-4.7.1/pyhap/encoder.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4494 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/hap_crypto.py
+-rw-r--r--   0 ivan       (501) staff       (20)      551 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/hap_event.py
+-rw-r--r--   0 ivan       (501) staff       (20)    30501 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/hap_handler.py
+-rw-r--r--   0 ivan       (501) staff       (20)    10729 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/hap_protocol.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3104 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/hap_server.py
+-rw-r--r--   0 ivan       (501) staff       (20)     3345 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/hsrp.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1936 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/iid_manager.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2371 2023-06-18 11:59:57.000000 HAP-python-4.7.1/pyhap/loader.py
+-rw-r--r--   0 ivan       (501) staff       (20)     1254 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/params.py
+drwxr-xr-x   0 ivan       (501) staff       (20)        0 2023-07-31 19:16:35.402840 HAP-python-4.7.1/pyhap/resources/
+-rw-r--r--   0 ivan       (501) staff       (20)    35625 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/resources/characteristics.json
+-rw-r--r--   0 ivan       (501) staff       (20)    14516 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/resources/services.json
+-rw-r--r--   0 ivan       (501) staff       (20)   203005 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/resources/snapshot.jpg
+-rw-r--r--   0 ivan       (501) staff       (20)     4653 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/service.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4010 2023-06-18 11:59:57.000000 HAP-python-4.7.1/pyhap/state.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2212 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyhap/tlv.py
+-rw-r--r--   0 ivan       (501) staff       (20)     4205 2023-07-31 19:16:09.000000 HAP-python-4.7.1/pyhap/util.py
+-rw-r--r--   0 ivan       (501) staff       (20)     2648 2023-06-18 11:42:25.000000 HAP-python-4.7.1/pyproject.toml
+-rw-r--r--   0 ivan       (501) staff       (20)      107 2023-07-31 19:16:35.403524 HAP-python-4.7.1/setup.cfg
+-rw-r--r--   0 ivan       (501) staff       (20)     1931 2023-07-31 19:16:09.000000 HAP-python-4.7.1/setup.py
```

### Comparing `HAP-python-4.7.0/HAP_python.egg-info/PKG-INFO` & `HAP-python-4.7.1/HAP_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HAP-python
-Version: 4.7.0
+Version: 4.7.1
 Summary: HomeKit Accessory Protocol implementation in python
 Home-page: https://github.com/ikalchev/HAP-python
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/ikalchev/HAP-python/issues
 Project-URL: Documentation, http://hap-python.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ikalchev/HAP-python/tree/master
 Platform: UNKNOWN
```

### Comparing `HAP-python-4.7.0/HAP_python.egg-info/SOURCES.txt` & `HAP-python-4.7.1/HAP_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/LICENSE` & `HAP-python-4.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/PKG-INFO` & `HAP-python-4.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HAP-python
-Version: 4.7.0
+Version: 4.7.1
 Summary: HomeKit Accessory Protocol implementation in python
 Home-page: https://github.com/ikalchev/HAP-python
 License: Apache License 2.0
 Project-URL: Bug Reports, https://github.com/ikalchev/HAP-python/issues
 Project-URL: Documentation, http://hap-python.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ikalchev/HAP-python/tree/master
 Platform: UNKNOWN
```

### Comparing `HAP-python-4.7.0/README.md` & `HAP-python-4.7.1/README.md`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/accessory.py` & `HAP-python-4.7.1/pyhap/accessory.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Module for the Accessory classes."""
 import itertools
 import logging
-
 from uuid import UUID
+
 from pyhap import SUPPORT_QR_CODE, util
 from pyhap.const import (
     CATEGORY_BRIDGE,
     CATEGORY_OTHER,
+    HAP_PROTOCOL_VERSION,
     HAP_REPR_AID,
     HAP_REPR_IID,
-    HAP_PROTOCOL_VERSION,
     HAP_REPR_SERVICES,
     HAP_REPR_VALUE,
     STANDALONE_AID,
 )
 from pyhap.iid_manager import IIDManager
 from pyhap.service import Service
```

### Comparing `HAP-python-4.7.0/pyhap/accessory_driver.py` & `HAP-python-4.7.1/pyhap/accessory_driver.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/camera.py` & `HAP-python-4.7.1/pyhap/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,26 +14,26 @@
 streaming.
 4. The camera starts the streaming with the above configuration.
 [5. At some point the client can reconfigure or stop the stream similarly to step 3.]
 """
 
 import asyncio
 import functools
-import os
 import ipaddress
 import logging
+import os
 import struct
 from uuid import UUID
 
-from pyhap import RESOURCE_DIR
+import async_timeout
+
+from pyhap import RESOURCE_DIR, tlv
 from pyhap.accessory import Accessory
 from pyhap.const import CATEGORY_CAMERA
-from pyhap.util import to_base64_str, byte_bool
-from pyhap import tlv
-
+from pyhap.util import byte_bool, to_base64_str
 
 SETUP_TYPES = {
     'SESSION_ID': b'\x01',
     'STATUS': b'\x02',
     'ADDRESS': b'\x03',
     'VIDEO_SRTP_PARAM': b'\x04',
     'AUDIO_SRTP_PARAM': b'\x05',
@@ -855,16 +855,16 @@
         """
         session_id = session_info['id']
         ffmpeg_process = session_info.get('process')
         if ffmpeg_process:
             logger.info('[%s] Stopping stream.', session_id)
             try:
                 ffmpeg_process.terminate()
-                _, stderr = await asyncio.wait_for(
-                    ffmpeg_process.communicate(), timeout=2.0)
+                async with async_timeout.timeout(2.0):
+                    _, stderr = await ffmpeg_process.communicate()
                 logger.debug('Stream command stderr: %s', stderr)
             except asyncio.TimeoutError:
                 logger.error(
                     'Timeout while waiting for the stream process '
                     'to terminate. Trying with kill.'
                 )
                 ffmpeg_process.kill()
```

### Comparing `HAP-python-4.7.0/pyhap/characteristic.py` & `HAP-python-4.7.1/pyhap/characteristic.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/const.py` & `HAP-python-4.7.1/pyhap/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """This module contains constants used by other modules."""
 MAJOR_VERSION = 4
 MINOR_VERSION = 7
-PATCH_VERSION = 0
+PATCH_VERSION = 1
 __short_version__ = f"{MAJOR_VERSION}.{MINOR_VERSION}"
 __version__ = f"{__short_version__}.{PATCH_VERSION}"
 REQUIRED_PYTHON_VER = (3, 7)
 
 BASE_UUID = "-0000-1000-8000-0026BB765291"
 
 # ### Misc ###
```

### Comparing `HAP-python-4.7.0/pyhap/encoder.py` & `HAP-python-4.7.1/pyhap/encoder.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/hap_crypto.py` & `HAP-python-4.7.1/pyhap/hap_crypto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """This module partially implements crypto for HAP."""
 import logging
 import struct
-
+from functools import partial
+from typing import List
+from struct import Struct
 from chacha20poly1305_reuseable import ChaCha20Poly1305Reusable as ChaCha20Poly1305
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.kdf.hkdf import HKDF
 
 logger = logging.getLogger(__name__)
 
 CRYPTO_BACKEND = default_backend()
 
+PACK_NONCE = partial(Struct("<LQ").pack, 0)
+PACK_LENGTH = Struct("H").pack
+
 
 class HAP_CRYPTO:
     HKDF_KEYLEN = 32  # bytes, length of expanded HKDF keys
     HKDF_HASH = hashes.SHA512()  # Hash function to use in key expansion
     TAG_LENGTH = 16  # ChaCha20Poly1305 tag length
     TLS_NONCE_LEN = 12  # bytes, length of TLS encryption nonce
 
@@ -70,55 +75,58 @@
     def decrypt(self) -> bytes:
         """Decrypt and return any complete blocks in the buffer as plaintext
 
         The received full cipher blocks are decrypted and returned and partial cipher
         blocks are buffered locally.
         """
         result = b""
+        crypt_in_buffer = self._crypt_in_buffer
+        length_length = self.LENGTH_LENGTH
+        tag_length = HAP_CRYPTO.TAG_LENGTH
 
-        while len(self._crypt_in_buffer) > self.MIN_BLOCK_LENGTH:
-            block_length_bytes = self._crypt_in_buffer[: self.LENGTH_LENGTH]
+        while len(crypt_in_buffer) > self.MIN_BLOCK_LENGTH:
+            block_length_bytes = crypt_in_buffer[:length_length]
             block_size = struct.unpack("H", block_length_bytes)[0]
-            block_size_with_length = (
-                self.LENGTH_LENGTH + block_size + HAP_CRYPTO.TAG_LENGTH
-            )
+            block_size_with_length = length_length + block_size + tag_length
 
-            if len(self._crypt_in_buffer) < block_size_with_length:
+            if len(crypt_in_buffer) < block_size_with_length:
                 logger.debug("Incoming buffer does not have the full block")
                 return result
 
             # Trim off the length
-            del self._crypt_in_buffer[: self.LENGTH_LENGTH]
+            del crypt_in_buffer[:length_length]
 
-            data_size = block_size + HAP_CRYPTO.TAG_LENGTH
-            nonce = pad_tls_nonce(struct.pack("Q", self._in_count))
+            data_size = block_size + tag_length
+            nonce = PACK_NONCE(self._in_count)
 
             result += self._in_cipher.decrypt(
                 nonce,
-                bytes(self._crypt_in_buffer[:data_size]),
+                bytes(crypt_in_buffer[:data_size]),
                 bytes(block_length_bytes),
             )
 
             self._in_count += 1
 
             # Now trim out the decrypted data
-            del self._crypt_in_buffer[:data_size]
+            del crypt_in_buffer[:data_size]
 
         return result
 
     def encrypt(self, data: bytes) -> bytes:
         """Encrypt and send the return bytes."""
-        result = b""
+        result: List[bytes] = []
         offset = 0
         total = len(data)
         while offset < total:
             length = min(total - offset, self.MAX_BLOCK_LENGTH)
-            length_bytes = struct.pack("H", length)
+            length_bytes = PACK_LENGTH(length)
             block = bytes(data[offset : offset + length])
-            nonce = pad_tls_nonce(struct.pack("Q", self._out_count))
-            ciphertext = length_bytes + self._out_cipher.encrypt(
-                nonce, block, length_bytes
-            )
+            nonce = PACK_NONCE(self._out_count)
+            result.append(length_bytes)
+            result.append(self._out_cipher.encrypt(nonce, block, length_bytes))
             offset += length
             self._out_count += 1
-            result += ciphertext
-        return result
+
+        # Join the result once instead of concatenating each time
+        # as this is much faster than generating an new immutable
+        # byte string each time.
+        return b"".join(result)
```

### Comparing `HAP-python-4.7.0/pyhap/hap_event.py` & `HAP-python-4.7.1/pyhap/hap_event.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/hap_handler.py` & `HAP-python-4.7.1/pyhap/hap_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import asyncio
 from http import HTTPStatus
 import logging
 from typing import TYPE_CHECKING, Dict, Optional
 from urllib.parse import ParseResult, parse_qs, urlparse
 import uuid
 
+import async_timeout
 from chacha20poly1305_reuseable import ChaCha20Poly1305Reusable as ChaCha20Poly1305
 from cryptography.exceptions import InvalidSignature, InvalidTag
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519, x25519
 import h11
 
 from pyhap import tlv
@@ -89,14 +90,20 @@
     PERMISSIONS = b"\x0B"
 
 
 class UnprivilegedRequestException(Exception):
     pass
 
 
+async def _run_with_timeout(coro, timeout: float) -> bytes:
+    """Run a coroutine with a timeout."""
+    async with async_timeout.timeout(timeout):
+        return await coro
+
+
 class HAPServerHandler:
     """Manages HAP connection state and handles incoming HTTP requests."""
 
     # Mapping from paths to methods that handle them.
     HANDLERS = {
         "POST": {
             "/pair-setup": "handle_pairing",
@@ -816,12 +823,12 @@
             coro = loop.run_in_executor(None, accessory.get_snapshot, data)
         else:
             raise ValueError(
                 "Got a request for snapshot, but the Accessory "
                 'does not define a "get_snapshot" or "async_get_snapshot" method'
             )
 
-        task = asyncio.ensure_future(asyncio.wait_for(coro, RESPONSE_TIMEOUT))
+        task = asyncio.ensure_future(_run_with_timeout(coro, RESPONSE_TIMEOUT))
         self.send_response(HTTPStatus.OK)
         self.send_header("Content-Type", "image/jpeg")
         assert self.response is not None  # nosec
         self.response.task = task
```

### Comparing `HAP-python-4.7.0/pyhap/hap_protocol.py` & `HAP-python-4.7.1/pyhap/hap_protocol.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/hap_server.py` & `HAP-python-4.7.1/pyhap/hap_server.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/hsrp.py` & `HAP-python-4.7.1/pyhap/hsrp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Server Side SRP implementation
 
 import os
+
 from .util import long_to_bytes
 
 
 def bytes_to_long(s):
     # Bytes should be interpreted from left to right, hence the byteorder
     return int.from_bytes(s, byteorder="big")
```

### Comparing `HAP-python-4.7.0/pyhap/iid_manager.py` & `HAP-python-4.7.1/pyhap/iid_manager.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/loader.py` & `HAP-python-4.7.1/pyhap/loader.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/params.py` & `HAP-python-4.7.1/pyhap/params.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/resources/characteristics.json` & `HAP-python-4.7.1/pyhap/resources/characteristics.json`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/resources/services.json` & `HAP-python-4.7.1/pyhap/resources/services.json`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/resources/snapshot.jpg` & `HAP-python-4.7.1/pyhap/resources/snapshot.jpg`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/service.py` & `HAP-python-4.7.1/pyhap/service.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/state.py` & `HAP-python-4.7.1/pyhap/state.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/tlv.py` & `HAP-python-4.7.1/pyhap/tlv.py`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/pyhap/util.py` & `HAP-python-4.7.1/pyhap/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import base64
 import functools
 import random
 import socket
 from uuid import UUID
 
+import async_timeout
 import orjson
 
 from .const import BASE_UUID
 
 ALPHANUM = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 HEX_DIGITS = "0123456789ABCDEF"
 
@@ -131,15 +132,16 @@
     :param timeout: The timeout for which to wait, in seconds.
     :type timeout: float
 
     :return: ``event.is_set()``
     :rtype: bool
     """
     try:
-        await asyncio.wait_for(event.wait(), timeout)
+        async with async_timeout.timeout(timeout):
+            await event.wait()
     except asyncio.TimeoutError:
         pass
     return event.is_set()
 
 
 @functools.lru_cache(maxsize=2048)
 def uuid_to_hap_type(uuid):
```

### Comparing `HAP-python-4.7.0/pyproject.toml` & `HAP-python-4.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `HAP-python-4.7.0/setup.py` & `HAP-python-4.7.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,22 @@
 
 MIN_PY_VERSION = ".".join(map(str, pyhap_const.REQUIRED_PYTHON_VER))
 
 with open("README.md", "r", encoding="utf-8") as f:
     README = f.read()
 
 
-REQUIRES = ["cryptography", "chacha20poly1305-reuseable", "orjson>=3.7.2", "zeroconf>=0.36.2", "h11"]
+REQUIRES = [
+    "async_timeout",
+    "cryptography",
+    "chacha20poly1305-reuseable",
+    "orjson>=3.7.2",
+    "zeroconf>=0.36.2",
+    "h11",
+]
 
 
 setup(
     name=NAME,
     version=pyhap_const.__version__,
     description=DESCRIPTION,
     long_description=README,
```

