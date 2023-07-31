# Comparing `tmp/astarte-device-sdk-0.11.0.tar.gz` & `tmp/astarte-device-sdk-0.12.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astarte-device-sdk-0.11.0.tar", last modified: Thu Mar 16 14:47:44 2023, max compression
+gzip compressed data, was "astarte-device-sdk-0.12.0.tar", last modified: Mon Jul 31 09:39:05 2023, max compression
```

## Comparing `astarte-device-sdk-0.11.0.tar` & `astarte-device-sdk-0.12.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:47:44.581349 astarte-device-sdk-0.11.0/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-16 14:47:44.581349 astarte-device-sdk-0.11.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:47:44.577349 astarte-device-sdk-0.11.0/astarte/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:47:44.577349 astarte-device-sdk-0.11.0/astarte/device/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    29086 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/astarte/device/pairing_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:47:44.577349 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-16 14:47:44.000000 astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 14:47:44.581349 astarte-device-sdk-0.11.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-03-16 14:47:34.000000 astarte-device-sdk-0.11.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:39:05.318323 astarte-device-sdk-0.12.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-31 09:39:05.318323 astarte-device-sdk-0.12.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:39:05.314324 astarte-device-sdk-0.12.0/astarte/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:39:05.314324 astarte-device-sdk-0.12.0/astarte/device/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33053 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11885 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/astarte/device/pairing_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:39:05.318323 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 09:39:05.000000 astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 09:39:05.318323 astarte-device-sdk-0.12.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-31 09:38:54.000000 astarte-device-sdk-0.12.0/setup.py
```

### Comparing `astarte-device-sdk-0.11.0/PKG-INFO` & `astarte-device-sdk-0.12.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,91 @@
-Metadata-Version: 2.1
-Name: astarte-device-sdk
-Version: 0.11.0
-Summary: Astarte Device SDK for Python
-Home-page: https://github.com/astarte-platform/astarte-device-sdk-python
-Author: Francesco Vaiani
-Author-email: francesco.vaiani@secomind.com
-License: License :: OSI Approved :: Apache Software License
-Description: # Astarte Python Device SDK
-        
-        Python Device SDK for [Astarte](https://github.com/astarte-platform/astarte). Create Astarte Devices
-        and Simulators with Python3.
-        It integrates with asyncio to ensure a smooth developer experience and to hide complex details
-        regarding threading and MQTT interactions.
-        
-        ## How to get with Pip
-        
-        The Astarte device SDK can be obtained by running:
-        ```
-        pip install astarte-device-sdk
-        ```
-        
-        ## Basic usage
-        
-        ### Create a device
-        
-        Initializing an instance of a device can be performed in three steps, as seen below.
-        ```python
-        from astarte.device import Device
-        
-        # Create the device instance
-        device = Device(
-            device_id="device id",
-            realm="realm",
-            credentials_secret="credentials secret",
-            pairing_base_url="pairing url",
-            persistency_dir=".",
-            loop=None,
-            ignore_ssl_errors=False,
-        )
-        # Add all the interfaces for this device
-        for interface in interfaces:
-            device.add_interface(interface)
-        # Connect to Astarte
-        device.connect()
-        ```
-        
-        ### Publish data from device
-        
-        Publishing new values can be performed using the `send` and `send_aggregate` functions.
-        ```python
-        from astarte.device import Device
-        from datetime import datetime, timezone
-        
-        # ... Create a device and connect it to Astarte ...
-        
-        # Send an individual datastream or a property
-        device.send(
-            interface_name="datastream_interface",
-            interface_path=f"/path/name",
-            payload="payload",
-            timestamp=None,
-        )
-        
-        # Send an aggregated object datastream
-        payload = {"endpoint1": "value1", "endpoint2": 42}
-        device.send_aggregate(
-            interface_name="aggregate_interface",
-            interface_path=f"/path/name",
-            payload=payload,
-            timestamp=datetime.now(tz=timezone.utc),
-        )
-        ```
-        
-        ### Receive a server publication
-        
-        The device automatically polls for new messages. The user can use a call back function to process
-        received data. Callback functions are also available for connect/disconnect events.
-        ```python
-        from astarte.device import Device
-        
-        def my_callback(device: Device, name: str, path: str, payload: dict):
-            print(f"Received message for {name}{path}: {payload}")
-        
-        # ... Create a device and connect it to Astarte ...
-        
-        # Setup the callback
-        device.on_data_received = my_callback
-        
-        # Keep the program running
-        while True:
-            pass
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: e2e
+<!--
+Copyright 2023 SECO Mind Srl
+
+SPDX-License-Identifier: Apache-2.0
+-->
+
+# Astarte Python Device SDK
+
+Python Device SDK for [Astarte](https://github.com/astarte-platform/astarte). Create Astarte Devices
+and Simulators with Python3.
+It integrates with asyncio to ensure a smooth developer experience and to hide complex details
+regarding threading and MQTT interactions.
+
+## How to get with Pip
+
+The Astarte device SDK can be obtained by running:
+```
+pip install astarte-device-sdk
+```
+
+## Basic usage
+
+### Create a device
+
+Initializing an instance of a device can be performed in three steps, as seen below.
+```python
+from astarte.device import Device
+
+# Create the device instance
+device = Device(
+    device_id="device id",
+    realm="realm",
+    credentials_secret="credentials secret",
+    pairing_base_url="pairing url",
+    persistency_dir=".",
+    loop=None,
+    ignore_ssl_errors=False,
+)
+# Add a single interface from a .json file
+device.add_interface_from_file(Path("interfaces/path/file.json"))
+# Use `device.add_interfaces_from_dir(Path("interfaces/path"))` instead to add all the interfaces in a directory
+# Connect to Astarte
+device.connect()
+```
+
+### Publish data from device
+
+Publishing new values can be performed using the `send` and `send_aggregate` functions.
+```python
+from astarte.device import Device
+from datetime import datetime, timezone
+
+# ... Create a device and connect it to Astarte ...
+
+# Send an individual datastream or a property
+device.send(
+    interface_name="datastream_interface",
+    interface_path=f"/path/name",
+    payload="payload",
+    timestamp=None,
+)
+
+# Send an aggregated object datastream
+payload = {"endpoint1": "value1", "endpoint2": 42}
+device.send_aggregate(
+    interface_name="aggregate_interface",
+    interface_path=f"/path/name",
+    payload=payload,
+    timestamp=datetime.now(tz=timezone.utc),
+)
+```
+
+### Receive a server publication
+
+The device automatically polls for new messages. The user can use a call back function to process
+received data. Callback functions are also available for connect/disconnect events.
+```python
+from astarte.device import Device
+
+def my_callback(device: Device, name: str, path: str, payload: dict):
+    print(f"Received message for {name}{path}: {payload}")
+
+# ... Create a device and connect it to Astarte ...
+
+# Setup the callback
+device.on_data_received = my_callback
+
+# Keep the program running
+while True:
+    pass
+```
```

### Comparing `astarte-device-sdk-0.11.0/README.md` & `astarte-device-sdk-0.12.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: astarte-device-sdk
+Version: 0.12.0
+Summary: Astarte Device SDK for Python
+Home-page: https://github.com/astarte-platform/astarte-device-sdk-python
+Author: Simone Orru
+Author-email: simone.orru@secomind.com
+License: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: static
+Provides-Extra: unit
+Provides-Extra: e2e
+
+<!--
+Copyright 2023 SECO Mind Srl
+
+SPDX-License-Identifier: Apache-2.0
+-->
+
 # Astarte Python Device SDK
 
 Python Device SDK for [Astarte](https://github.com/astarte-platform/astarte). Create Astarte Devices
 and Simulators with Python3.
 It integrates with asyncio to ensure a smooth developer experience and to hide complex details
 regarding threading and MQTT interactions.
 
@@ -26,17 +49,17 @@
     realm="realm",
     credentials_secret="credentials secret",
     pairing_base_url="pairing url",
     persistency_dir=".",
     loop=None,
     ignore_ssl_errors=False,
 )
-# Add all the interfaces for this device
-for interface in interfaces:
-    device.add_interface(interface)
+# Add a single interface from a .json file
+device.add_interface_from_file(Path("interfaces/path/file.json"))
+# Use `device.add_interfaces_from_dir(Path("interfaces/path"))` instead to add all the interfaces in a directory
 # Connect to Astarte
 device.connect()
 ```
 
 ### Publish data from device
 
 Publishing new values can be performed using the `send` and `send_aggregate` functions.
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/__init__.py` & `astarte-device-sdk-0.12.0/astarte/device/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-# Copyright 2020-2022 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
+# SPDX-License-Identifier: Apache-2.0
 
 # Version of the module
-__version__ = "0.11.0"
+__version__ = "0.12.0"
 
 # Export what we care about
 from .device import Device
 from .introspection import Introspection
 from .interface import Interface
 from .mapping import Mapping
 from .pairing_handler import (
@@ -28,8 +31,14 @@
     generate_random_device_id,
 )
 from .exceptions import (
     AstarteError,
     DeviceAlreadyRegisteredError,
     AuthorizationError,
     APIError,
+    ValidationError,
+    PersistencyDirectoryNotFoundError,
+    InterfaceFileNotFoundError,
+    InterfaceFileDecodeError,
+    InterfaceNotFoundError,
+    JWTGenerationError,
 )
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/crypto.py` & `astarte-device-sdk-0.12.0/astarte/device/crypto.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-# Copyright 2020-2021 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
+#
+# SPDX-License-Identifier: Apache-2.0
 
 from datetime import datetime
 from os import path
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import ec
 from cryptography.x509.oid import NameOID
 
 
 def generate_csr(realm: str, device_id: str, crypto_store_dir: str) -> bytes:
@@ -42,52 +44,60 @@
     bytes
         The device certificate signing request file
     """
     key = None
     # Do we need to generate a keypair?
     if not path.exists(path.join(crypto_store_dir, "device.key")):
         # Generate our key
-        key = ec.generate_private_key(curve=ec.SECP256R1(), backend=default_backend())
+        key = ec.generate_private_key(curve=ec.SECP256R1())
         # Write our key to disk for safe keeping
         with open(path.join(crypto_store_dir, "device.key"), "wb") as f:
             f.write(
                 key.private_bytes(
                     encoding=serialization.Encoding.PEM,
                     format=serialization.PrivateFormat.TraditionalOpenSSL,
                     encryption_algorithm=serialization.NoEncryption(),
                 )
             )
     else:
         # Load the key
         with open(path.join(crypto_store_dir, "device.key"), "rb") as key_file:
-            key = serialization.load_pem_private_key(
-                key_file.read(), password=None, backend=default_backend()
-            )
+            key = serialization.load_pem_private_key(key_file.read(), password=None)
 
     csr = (
-        x509.CertificateSigningRequestBuilder()
-        .subject_name(
+        x509.CertificateSigningRequestBuilder().subject_name(
             x509.Name(
                 [
                     # Provide various details about who we are.
                     x509.NameAttribute(NameOID.ORGANIZATION_NAME, "Devices"),
                     x509.NameAttribute(NameOID.COMMON_NAME, f"{realm}/{device_id}"),
-                    # Sign the CSR with our private key.
                 ]
             )
         )
-        .sign(key, hashes.SHA256(), default_backend())
+        # Sign the CSR with our private key.
+        .sign(key, hashes.SHA256())
     )
 
     # Return the CSR
     return csr.public_bytes(serialization.Encoding.PEM)
 
 
 def import_device_certificate(client_crt: str, crypto_store_dir: str) -> None:
-    certificate = x509.load_pem_x509_certificate(client_crt.encode("ascii"), default_backend())
+    """
+    Deserialize a client certificate and store the public information permanently in the file system
+
+    Parameters
+    ----------
+    client_crt: str
+        Serialized client certificate
+    crypto_store_dir: str
+        Directory where to store the public bytes of the certificate
+
+    """
+    certificate = x509.load_pem_x509_certificate(client_crt.encode("ascii"))
 
     # Store the certificate
     with open(path.join(crypto_store_dir, "device.crt"), "wb") as f:
         f.write(certificate.public_bytes(encoding=serialization.Encoding.PEM))
 
 
 def device_has_certificate(crypto_store_dir: str) -> bool:
@@ -129,12 +139,12 @@
 
     """
     cert_path = path.join(crypto_store_dir, "device.crt")
     with open(cert_path, "r", encoding="utf-8") as file:
         data = file.read()
     if data:
         try:
-            certificate = x509.load_pem_x509_certificate(data.encode("ascii"), default_backend())
+            certificate = x509.load_pem_x509_certificate(data.encode("ascii"))
         except ValueError:
             return False
         return certificate.not_valid_before < datetime.utcnow() < certificate.not_valid_after
     return False
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/device.py` & `astarte-device-sdk-0.12.0/astarte/device/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,52 @@
-# Copyright 2020-2021 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import logging
 import asyncio
 import collections.abc
 import os
 import ssl
 import json
+import zlib
 from pathlib import Path
 from collections.abc import Callable
 from datetime import datetime
 from urllib.parse import urlparse
 
 import bson
 import paho.mqtt.client as mqtt
 from astarte.device import crypto, pairing_handler
+from astarte.device.interface import Interface
 from astarte.device.introspection import Introspection
+from astarte.device.database import AstarteDatabaseSQLite, AstarteDatabase
+from astarte.device.exceptions import (
+    ValidationError,
+    PersistencyDirectoryNotFoundError,
+    InterfaceFileNotFoundError,
+    InterfaceFileDecodeError,
+    InterfaceNotFoundError,
+)
 
 
 class Device:  # pylint: disable=too-many-instance-attributes
     """
     Basic class to define an Astarte Device.
 
     Device represents an Astarte Device. It is the base class used for managing the Device
@@ -72,14 +87,15 @@
     def __init__(
         self,
         device_id: str,
         realm: str,
         credentials_secret: str,
         pairing_base_url: str,
         persistency_dir: str,
+        database: AstarteDatabase | None = None,
         loop: asyncio.AbstractEventLoop | None = None,
         ignore_ssl_errors: bool = False,
     ):
         """
         Parameters
         ----------
         device_id : str
@@ -93,54 +109,75 @@
             :py:func:`register_device_with_private_key`.
         pairing_base_url : str
             The Base URL of Pairing API of the Astarte Instance the Device will connect to.
         persistency_dir : str
             Path to an existing directory which will be used for holding persistency for this
             device: certificates, caching and more. It doesn't have to be unique per device,
             a subdirectory for the given Device ID will be created.
-        loop : asyncio.loop, optional
+        database : AstarteDatabase (optional)
+            User instantiated database to use for caching properties. When None, a native SQLite
+            database will be created and used in the persistency_dir.
+        loop : asyncio.loop (optional)
             An optional loop which will be used for invoking callbacks. When this is not none,
             Device will call any specified callback through loop.call_soon_threadsafe, ensuring
             that the callbacks will be run in thread the loop belongs to. Usually, you want
             to set this to get_running_loop(). When not sent, callbacks will be invoked as a
             standard function - keep in mind this means your callbacks might create deadlocks.
         ignore_ssl_errors: bool (optional)
             Useful if you're using the Device to connect to a test instance of Astarte with
             self-signed certificates, it is not recommended to leave this `true` in production.
             Defaults to `false`, if `true` the device will ignore SSL errors during connection.
+        Raises
+        ------
+        PersistencyDirectoryNotFoundError
+            If the provided persistency directory does not exists.
         """
+        if not os.path.isdir(persistency_dir):
+            raise PersistencyDirectoryNotFoundError(f"{persistency_dir} is not a directory")
+
+        if not os.path.isdir(os.path.join(persistency_dir, device_id)):
+            os.mkdir(os.path.join(persistency_dir, device_id))
+
+        crypto_dir = os.path.join(persistency_dir, device_id, "crypto")
+        if not os.path.isdir(crypto_dir):
+            os.mkdir(crypto_dir)
+
+        caching_dir = os.path.join(persistency_dir, device_id, "caching")
+        if not database and not os.path.isdir(caching_dir):
+            os.mkdir(caching_dir)
+
+        # Define private and public attributes
         self.__device_id = device_id
         self.__realm = realm
         self.__pairing_base_url = pairing_base_url
-        self.__persistency_dir = persistency_dir
+        self.__crypto_dir = crypto_dir
+        self.__prop_database = (
+            database
+            if database
+            else AstarteDatabaseSQLite(Path(os.path.join(caching_dir, "astarte.db")))
+        )
         self.__credentials_secret = credentials_secret
         # TODO: Implement device registration using token on connect
         # self.__jwt_token: str | None = None
         self.__is_crypto_setup = False
         self.__introspection = Introspection()
         self.__is_connected = False
         self.__loop = loop
         self.__ignore_ssl_errors = ignore_ssl_errors
 
         self.on_connected: Callable[Device, None] | None = None
         self.on_disconnected: Callable[[Device, int], None] | None = None
         self.on_data_received: Callable[[Device, str, str, object], None] | None = None
 
-        # Check if the persistency dir exists
-        if not os.path.isdir(persistency_dir):
-            raise FileNotFoundError(f"{persistency_dir} is not a directory")
-
-        if not os.path.isdir(os.path.join(persistency_dir, device_id)):
-            os.mkdir(os.path.join(persistency_dir, device_id))
-
-        if not os.path.isdir(os.path.join(persistency_dir, device_id, "crypto")):
-            os.mkdir(os.path.join(persistency_dir, device_id, "crypto"))
         self.__setup_mqtt_client()
 
     def __setup_mqtt_client(self) -> None:
+        """
+        Utility function used to setup an MQTT client
+        """
         self.__mqtt_client = mqtt.Client()
         self.__mqtt_client.on_connect = self.__on_connect
         self.__mqtt_client.on_disconnect = self.__on_disconnect
         self.__mqtt_client.on_message = self.__on_message
 
     def add_interface(self, interface_definition: dict) -> None:
         """
@@ -166,26 +203,28 @@
 
         Parameters
         ----------
         interface_file : Path
             An absolute path to an Astarte interface json file.
         Raises
         ------
-        FileNotFoundError
-            If specified file does not exists.
-        TypeError
-            If speficied file is not a .json file.
+        InterfaceFileNotFoundError
+            If the provided interface file does not exists.
+        InterfaceFileDecodeError
+            If speficied file is not a parsable .json file.
         """
         if not interface_file.is_file():
-            raise FileNotFoundError(f'"{interface_file}" does not exist or is not a file')
+            raise InterfaceFileNotFoundError(f'"{interface_file}" does not exist or is not a file')
         try:
             with open(interface_file, "r", encoding="utf-8") as interface_fp:
                 self.__introspection.add_interface(json.load(interface_fp))
         except json.JSONDecodeError as exc:
-            raise TypeError(f'"{interface_file}" is not a parsable json file') from exc
+            raise InterfaceFileDecodeError(
+                f'"{interface_file}" is not a parsable json file'
+            ) from exc
 
     def add_interfaces_from_dir(self, interfaces_dir: Path):
         """
         Adds a series of interfaces to the device
 
         This will add all the interfaces contained in the provided folder to the device.
         It has to be called before :py:func:`connect`, as it will be used for building the device
@@ -193,23 +232,21 @@
 
         Parameters
         ----------
         interfaces_dir : Path
             An absolute path to an a folder containing some Astarte interface .json files.
         Raises
         ------
-        FileNotFoundError
+        InterfaceFileNotFoundError
             If specified directory does not exists.
-        NotADirectoryError
-            If speficied directory exists but it's not a directory.
         """
         if not interfaces_dir.exists():
-            raise FileNotFoundError(f'"{interfaces_dir}" does not exist')
+            raise InterfaceFileNotFoundError(f'"{interfaces_dir}" does not exist')
         if not interfaces_dir.is_dir():
-            raise NotADirectoryError(f'"{interfaces_dir}" is not a directory')
+            raise InterfaceFileNotFoundError(f'"{interfaces_dir}" is not a directory')
         for interface_file in [i for i in interfaces_dir.iterdir() if i.suffix == ".json"]:
             self.add_interface_from_file(interface_file)
 
     def remove_interface(self, interface_name: str) -> None:
         """
         Removes an Interface from the Device
 
@@ -231,60 +268,62 @@
         -------
         str
             The Id of the device
         """
         return self.__device_id
 
     def __setup_crypto(self) -> None:
+        """
+        Utility function used to setup cytptography
+        """
         if self.__is_crypto_setup:
             return
 
-        if not crypto.device_has_certificate(
-            os.path.join(self.__persistency_dir, self.__device_id, "crypto")
-        ):
+        if not crypto.device_has_certificate(self.__crypto_dir):
             pairing_handler.obtain_device_certificate(
                 self.__device_id,
                 self.__realm,
                 self.__credentials_secret,
                 self.__pairing_base_url,
-                os.path.join(self.__persistency_dir, self.__device_id, "crypto"),
+                self.__crypto_dir,
                 self.__ignore_ssl_errors,
             )
         # Initialize MQTT Client
         if self.__ignore_ssl_errors:
             cert_reqs = ssl.CERT_NONE
         else:
             cert_reqs = ssl.CERT_REQUIRED
 
         self.__mqtt_client.tls_set(
             ca_certs=None,
-            certfile=os.path.join(self.__persistency_dir, self.__device_id, "crypto", "device.crt"),
-            keyfile=os.path.join(self.__persistency_dir, self.__device_id, "crypto", "device.key"),
+            certfile=os.path.join(self.__crypto_dir, "device.crt"),
+            keyfile=os.path.join(self.__crypto_dir, "device.key"),
             cert_reqs=cert_reqs,
             tls_version=ssl.PROTOCOL_TLS,
             ciphers=None,
         )
         self.__mqtt_client.tls_insecure_set(self.__ignore_ssl_errors)
 
+        self.__is_crypto_setup = True
+
     def connect(self) -> None:
         """
         Connects the Device asynchronously.
 
         When calling connect, a new connection thread is spawned and the Device will start a
         connection routine. The function might return before the Device connects: you want to
         use the on_connected callback to ensure you are notified upon connection.
 
         In case the Device gets disconnected unexpectedly, it will try to reconnect indefinitely
         until disconnect() is called.
         """
         if self.__is_connected:
             return
 
-        if not self.__is_crypto_setup:
-            self.__setup_crypto()
+        self.__setup_crypto()
 
         transport_info = pairing_handler.obtain_device_transport_information(
             self.__device_id,
             self.__realm,
             self.__credentials_secret,
             self.__pairing_base_url,
             self.__ignore_ssl_errors,
@@ -314,14 +353,15 @@
         code parameter: if it is 0, it means the disconnection happened following an explicit
         disconnection request.
         """
         if not self.__is_connected:
             return
 
         self.__mqtt_client.disconnect()
+        self.__mqtt_client.loop_stop(force=False)
 
     def is_connected(self) -> bool:
         """
         Returns whether the Device is currently connected.
 
         Returns
         -------
@@ -351,49 +391,45 @@
             interface path.
         timestamp : datetime, optional
             If sending a Datastream with explicit_timestamp, you can specify a datetime object
             which will be registered as the timestamp for the value.
 
         Raises
         ------
-        TypeError
+        InterfaceNotFoundError
+            If the interface is not declared in the introspection
+        ValidationError
             If the interface or the payload are not compatible.
         """
-        if self.__is_interface_aggregate(interface_name):
-            raise TypeError(
+        interface = self.__introspection.get_interface(interface_name)
+        if not interface:
+            raise InterfaceNotFoundError(
+                f"Interface {interface_name} not declared in introspection"
+            )
+        if interface.is_aggregation_object():
+            raise ValidationError(
                 f"Interface {interface_name} is an aggregate interface. You should use "
                 f"send_aggregate."
             )
 
         if isinstance(payload, collections.abc.Mapping):
-            raise TypeError("Payload for individual interfaces should not be a dictionary")
-
-        (validation_success, validation_error_message) = self.__validate_data(
-            interface_name, interface_path, payload, timestamp
-        )
-        if not validation_success:
-            raise TypeError(validation_error_message)
-
-        object_payload = {"v": payload}
-        if timestamp:
-            object_payload["t"] = timestamp
-
-        qos = self._get_qos(interface_name, interface_path)
+            raise ValidationError("Payload for individual interfaces should not be a dictionary")
 
         self.__send_generic(
-            f"{self.__get_base_topic()}/{interface_name}{interface_path}",
-            object_payload,
-            qos=qos,
+            interface,
+            interface_path,
+            payload,
+            timestamp,
         )
 
     def send_aggregate(
         self,
         interface_name: str,
         interface_path: str,
-        payload: dict,
+        payload: collections.abc.Mapping,
         timestamp: datetime | None = None,
     ) -> None:
         """
         Sends an aggregate message to an interface
 
         Parameters
         ----------
@@ -405,36 +441,37 @@
             A dictionary containing the path:value map for the aggregate.
         timestamp : datetime, optional
             If the Datastream has explicit_timestamp, you can specify a datetime object which
             will be registered as the timestamp for the value.
 
         Raises
         ------
-        TypeError
+        InterfaceNotFoundError
+            If the interface is not declared in the introspection
+        ValidationError
             If the interface or the payload are not compatible.
         """
-        if not self.__is_interface_aggregate(interface_name):
-            raise TypeError(
+        interface = self.__introspection.get_interface(interface_name)
+        if not interface:
+            raise InterfaceNotFoundError(
+                f"Interface {interface_name} not declared in introspection"
+            )
+        if not interface.is_aggregation_object():
+            raise ValidationError(
                 f"Interface {interface_name} is not an aggregate interface. You should use send."
             )
 
         if not isinstance(payload, collections.abc.Mapping):
-            raise TypeError("Payload for aggregate interfaces should be a dictionary")
-
-        # The payload should carry the aggregate object
-        object_payload = {"v": payload}
-        if timestamp:
-            object_payload["t"] = timestamp
-
-        qos = self._get_qos(interface_name)
+            raise ValidationError("Payload for aggregate interfaces should be a dictionary")
 
         self.__send_generic(
-            f"{self.__get_base_topic()}/{interface_name}{interface_path}",
-            object_payload,
-            qos=qos,
+            interface,
+            interface_path,
+            payload,
+            timestamp,
         )
 
     def unset_property(self, interface_name: str, interface_path: str) -> None:
         """
         Unset the specified property on an interface.
 
         Parameters
@@ -442,85 +479,98 @@
         interface_name : str
             The name of the Interface where the property to unset is located.
         interface_path : str
             The path on the Interface to unset.
 
         Raises
         ------
-        TypeError
+        InterfaceNotFoundError
+            If the interface is not declared in the introspection
+        ValidationError
             If the interface is of type datastream.
         """
-        if not self.__is_interface_type_properties(interface_name):
-            raise TypeError(
+
+        interface = self.__introspection.get_interface(interface_name)
+        if not interface:
+            raise InterfaceNotFoundError(
+                f"Interface {interface_name} not declared in introspection"
+            )
+        if not interface.is_type_properties():
+            raise ValidationError(
                 f"Interface {interface_name} is a datastream interface. You can only unset a "
                 f"property."
             )
 
-        qos = self._get_qos(interface_name)
-
         self.__send_generic(
-            f"{self.__get_base_topic()}/{interface_name}{interface_path}", None, qos=qos
+            interface,
+            interface_path,
+            None,
+            None,
         )
 
-    def __send_generic(self, topic: str, object_payload: dict | None, qos=2) -> None:
-        if object_payload:
-            payload = bson.dumps(object_payload)
-        else:
-            payload = b""
-        self.__mqtt_client.publish(topic, payload, qos=qos)
-
-    def __is_interface_aggregate(self, interface_name: str) -> bool:
-        """
-        Utility Function used to check if an interface is of type datastream and object aggregated
-
-        Parameters
-        ----------
-        interface_name: str
-            The name of the interface to check
-
-        Returns
-        -------
-        bool
-            True if the interface has aggregation "object", False otherwise
-
-        Raises
-        ------
-        FileNotFoundError
-            If the interface is not declared in the introspection
-        """
-        interface = self.__introspection.get_interface(interface_name)
-        if not interface:
-            raise FileNotFoundError(f"Interface {interface_name} not declared in introspection")
-
-        return interface.is_aggregation_object()
-
-    def __is_interface_type_properties(self, interface_name: str) -> bool:
+    def __send_generic(
+        self,
+        interface: Interface,
+        path: str,
+        payload: object | collections.abc.Mapping | None,
+        timestamp: datetime | None,
+    ) -> None:
         """
-        Utility Function used to check if an interface is of type "Properties"
+        Utility function used to publish a generic payload to an Astarte interface.
 
         Parameters
         ----------
-        interface_name: str
-            The name of the interface to check
-
-        Returns
-        -------
-        bool
-            True if the interface is of type "Properties", False otherwise
+        interface : Interface
+            The Interface to send data to.
+        path: str
+            The endpoint to send the data to
+        payload : object, collections.abc.Mapping, optional
+            The payload to send if present.
+        timestamp : datetime, optional
+            If the Datastream has explicit_timestamp, you can specify a datetime object which
+            will be registered as the timestamp for the value.
 
         Raises
         ------
-        FileNotFoundError
-            If the interface is not declared in the introspection
-        """
-        interface = self.__introspection.get_interface(interface_name)
-        if not interface:
-            raise FileNotFoundError(f"Interface {interface_name} not declared in introspection")
+        ValidationError
+            When:
+            - Attempting to send to a server owned interface.
+            - Sending to an endpoint that is not present in the interface.
+            - The payload validation fails.
+        """
+        # Check the interface has device ownership
+        if interface.is_server_owned():
+            raise ValidationError(f"The interface {interface.name} is not owned by the device.")
+
+        bson_payload = b""
+        if payload is not None:
+            validation_result = interface.validate(path, payload, timestamp)
+            if validation_result:
+                raise validation_result
+
+            object_payload = {"v": payload}
+            if timestamp:
+                object_payload["t"] = timestamp
+            bson_payload = bson.dumps(object_payload)
+        elif not interface.get_mapping(path):
+            raise ValidationError(f"Path {path} not in the {interface.name} interface.")
+
+        if interface.is_type_properties():
+            self.__prop_database.store_prop(
+                interface.name,
+                interface.version_major,
+                path,
+                payload,
+            )
 
-        return interface.is_type_properties()
+        self.__mqtt_client.publish(
+            f"{self.__get_base_topic()}/{interface.name}{path}",
+            bson_payload,
+            qos=interface.get_reliability(path),
+        )
 
     def __get_base_topic(self) -> str:
         """
         Utility function that returns the composition between realm and device id as often used
         in astarte API URLs
 
         Returns
@@ -534,33 +584,34 @@
         """
         Callback function for MQTT connection
 
         Parameters
         ----------
         flags: dict
             it contains response flags from the broker:
-            flags[‘session present’] - this flag is only useful for clients that are using
+            flags['session present'] - this flag is only useful for clients that are using
             [clean session] set to 0. If a client with [clean session] = 0 reconnects to a broker
             to which it has been connected previously, this flag indicates whether the broker still
             has the session information of the client. If 1, the session still exists.
         rc: int
             the connection result
 
         """
         if rc:
-            print("Error while connecting: " + str(rc))
+            logging.error("Connection failed! %s", rc)
+            return
 
         self.__is_connected = True
 
         if not flags["session present"]:
-            # Setup subscription
+            logging.debug("Session flag is not present, performing a clean session procedure")
             self.__setup_subscriptions()
-            # Send the introspection
             self.__send_introspection()
             self.__send_empty_cache()
+            self.__send_device_owned_properties()
 
         if self.on_connected:
             if self.__loop:
                 # Use threadsafe, as we're in a different thread here
                 self.__loop.call_soon_threadsafe(self.on_connected, self)
             else:
                 self.on_connected(self)
@@ -592,17 +643,15 @@
                 self.on_disconnected(self, rc)
 
         # If rc was explicit, stop the loop (after the callback)
         if not rc:
             self.__mqtt_client.loop_stop()
         # Else check certificate expiration and try reconnection
         # TODO: check for MQTT_ERR_TLS when Paho correctly returns it
-        elif not crypto.certificate_is_valid(
-            os.path.join(self.__persistency_dir, self.__device_id, "crypto")
-        ):
+        elif not crypto.certificate_is_valid(self.__crypto_dir):
             self.__mqtt_client.loop_stop()
             # If the certificate must be regenerated, old mqtt client is no longer valid as it is
             # bound to the wrong TLS params and paho does not allow to replace them a second time
             self.__setup_mqtt_client()
             self.connect()
 
     def __on_message(self, _client, _userdata, msg):
@@ -615,161 +664,194 @@
             an instance of MQTTMessage.
             This is a class with members topic, payload, qos, retain.
 
         Returns
         -------
 
         """
+        # Check correct base topic
         if not msg.topic.startswith(self.__get_base_topic()):
-            print(f"Received unexpected message on topic {msg.topic}, {msg.payload}")
+            logging.warning("Received unexpected message on topic %s, %s", msg.topic, msg.payload)
             return
+
+        # Parse control message in a separate function
         if msg.topic == f"{self.__get_base_topic()}/control/consumer/properties":
-            print(f"Received control message: {msg.payload}")
+            logging.info("Received purge properties control message.")
+            self.__purge_server_properties(payload=msg.payload)
             return
 
+        # Check if callback is set
         if not self.on_data_received:
             return
 
-        real_topic = msg.topic.replace(f"{self.__get_base_topic()}/", "")
-        topic_tokens = real_topic.split("/")
+        # Get interface name and path
+        topic_tokens = msg.topic.replace(f"{self.__get_base_topic()}/", "").split("/")
         interface_name = topic_tokens[0]
-        if not self.__introspection.get_interface(interface_name):
-            print(
-                f"Received unexpected message for unregistered interface {interface_name}:"
-                f" {msg.topic}, {msg.payload}"
+        interface_path = "/" + "/".join(topic_tokens[1:])
+
+        # Check if interface name is correct
+        interface = self.__introspection.get_interface(interface_name)
+        if not interface:
+            logging.warning(
+                "Received unexpected message for unregistered interface %s: %s, %s",
+                interface_name,
+                msg.topic,
+                msg.payload,
             )
             return
 
-        interface_path = "/" + "/".join(topic_tokens[1:])
+        # Check over ownership of the interface
+        if not interface.is_server_owned():
+            logging.warning(
+                "Received unexpected message for device owned interface %s: %s, %s",
+                interface_name,
+                msg.topic,
+                msg.payload,
+            )
+            return
+
+        # Extract payload from BSON
         data_payload = None
         if msg.payload:
             payload_object = bson.loads(msg.payload)
-            if "v" not in payload_object:
-                print(f"Received unexpected BSON Object on topic {msg.topic}, {payload_object}")
+            data_payload = payload_object.get("v")
+            if not data_payload:
+                logging.warning(
+                    "Received unexpected BSON Object on topic %s, %s", msg.topic, payload_object
+                )
                 return
-            data_payload = payload_object["v"]
+        # Ensure that an empty payload is only for resettable properties
+        elif not interface.is_property_endpoint_resettable(interface_path):
+            logging.warning(
+                "Received empty payload for non property interface %s or non resettable %s endpoint",
+                interface_name,
+                interface_path,
+            )
+            return
+
+        # Check the received path corresponds to the one in the interface
+        if interface.validate_path(interface_path, data_payload):
+            logging.warning(
+                "Received message on incorrect endpoint for interface %s: %s, %s",
+                interface_name,
+                msg.topic,
+                msg.payload,
+            )
+            return
+
+        # Check the payload matches with the interface
+        if data_payload:
+            if interface.validate_payload(interface_path, data_payload):
+                logging.warning(
+                    "Received incompatible payload for interface %s: %s, %s",
+                    interface_name,
+                    msg.topic,
+                    payload_object,
+                )
+                return
+
+        # For properties, store them in the properties database
+        if interface.is_type_properties():
+            self.__prop_database.store_prop(
+                interface.name, interface.version_major, interface_path, data_payload
+            )
 
         if self.__loop:
             # Use threadsafe, as we're in a different thread here
             self.__loop.call_soon_threadsafe(
                 self.on_data_received,
                 self,
                 interface_name,
                 interface_path,
                 data_payload,
             )
         else:
             self.on_data_received(self, interface_name, interface_path, data_payload)
 
+    def __setup_subscriptions(self) -> None:
+        """
+        Utility function used to subscribe to the server owned interfaces
+        """
+        self.__mqtt_client.subscribe(
+            f"{self.__get_base_topic()}/control/consumer/properties", qos=2
+        )
+        for interface in self.__introspection.get_all_server_owned_interfaces():
+            self.__mqtt_client.subscribe(f"{self.__get_base_topic()}/{interface.name}/#", qos=2)
+
     def __send_introspection(self) -> None:
         """
         Utility function used to send the introspection to Astarte
         """
 
         # Build the introspection message
         introspection_message = ""
         for interface in self.__introspection.get_all_interfaces():
             introspection_message += (
                 f"{interface.name}:{interface.version_major}:{interface.version_minor};"
             )
         introspection_message = introspection_message[:-1]
         self.__mqtt_client.publish(self.__get_base_topic(), introspection_message, 2)
 
-    def __setup_subscriptions(self) -> None:
-        """
-        Utility function used to subscribe to the server owned interfaces
-        """
-        self.__mqtt_client.subscribe(
-            f"{self.__get_base_topic()}/control/consumer/properties", qos=2
-        )
-        for interface in self.__introspection.get_all_server_owned_interfaces():
-            interface_qos = self._get_qos(interface.name)
-            self.__mqtt_client.subscribe(
-                f"{self.__get_base_topic()}/{interface.name}/#", qos=interface_qos
-            )
-
     def __send_empty_cache(self) -> None:
         """
         Utility function used to send the "empty cache" message to Astarte
         """
         self.__mqtt_client.publish(
             f"{self.__get_base_topic()}/control/emptyCache",
             payload=b"1",
             retain=False,
             qos=2,
         )
 
-    def _get_qos(self, interface_name, path=None) -> int:
+    def __send_device_owned_properties(self) -> None:
         """
-        Deduce the QoS to be used, based on the reliability of the interface.
-
-        Parameters
-        ----------
-        interface_name : str
-            The interface name to deduce QoS for.
-        path : str
-            The path on the Interface to deduce QoS for.
-
-        Returns
-        -------
-        int
-            The deduced QoS, one of [0,1,2], default is 2
-
-        Raises
-        ------
-        FileNotFoundError
-            If the interface is not declared in the introspection
+        Utility function used to send all the device properties present in the database to Astarte.
+        It also sends the purge properties message to Astarte.
         """
-        interface = self.__introspection.get_interface(interface_name)
-        if not interface:
-            raise FileNotFoundError(f"Interface {interface_name} not declared in introspection")
+        interfaces_list = []
+        for interface_name, _, interface_path, value in self.__prop_database.load_all_props():
+            interface = self.__introspection.get_interface(interface_name)
+            if not interface:
+                self.__prop_database.delete_prop(interface_name, interface_path)
+            elif not interface.is_server_owned():
+                self.__send_generic(interface, interface_path, value, timestamp=None)
+                interfaces_list += [interface_name + interface_path]
+        interfaces_str = ";".join(interfaces_list)
+        payload = bytearray(len(interfaces_str).to_bytes(4, byteorder="little"))
+        payload.extend(zlib.compress(interfaces_str.encode("utf-8")))
 
-        # When aggregation object there is no need to specify the path as every map have the same
-        # QoS
-        if path:
-            mapping = interface.get_mapping(path)
-            if not mapping:
-                raise FileNotFoundError(f"Path {path} not declared in {interface_name}")
-        else:
-            mapping = list(interface.mappings.values())[0]
-
-        return mapping.reliability
+        self.__mqtt_client.publish(
+            f"{self.__get_base_topic()}/control/producer/properties",
+            payload=payload,
+            retain=False,
+            qos=2,
+        )
 
-    def __validate_data(
-        self,
-        interface_name: str,
-        interface_path: str,
-        payload: object,
-        timestamp: datetime | None,
-    ) -> tuple[bool, str]:
+    def __purge_server_properties(self, payload) -> None:
         """
-        Verifies the data corresponds with the interface.
+        Purges the server owned properties not contained in the payload.
 
         Parameters
         ----------
-        interface_name : str
-            The name of an the Interface to send data to.
-        interface_path : str
-            The path on the Interface to send data to.
-        payload : object
-            The value to be sent. The type should be compatible to the one specified in the
-            interface path.
-        timestamp : datetime, optional
-            If sending a Datastream with explicit_timestamp, you can specify a datetime object
-            which will be registered as the timestamp for the value.
-
-        Returns
-        -------
-        bool
-            Success of the validation operation
-        str
-            Error message if success is False
-        Raises
-        ------
-        FileNotFoundError
-            If the interface is not declared in the introspection
-        """
-        interface = self.__introspection.get_interface(interface_name)
-        if not interface:
-            raise FileNotFoundError(f"Interface {interface_name} not declared in introspection")
-
-        return interface.validate(interface_path, payload, timestamp)
+        payload : str
+            The purge properties message payload, contains a list of properties to save from
+            purging.
+        """
+        allowed_properties = []
+        decompressed_payload = zlib.decompress(payload[4:]).decode("utf-8")
+        if decompressed_payload:
+            # Parse the received list of set properties.
+            for full_path in [p.split("/") for p in decompressed_payload.split(";")]:
+                interface_name = full_path[0]
+                if not self.__introspection.get_interface(interface_name):
+                    logging.debug("Purge list entry %s missing from introspection.", interface_name)
+                    continue
+                allowed_properties.append((interface_name, "/" + "/".join(full_path[1:])))
+
+        # Delete all the properties not in the received list.
+        for interface_name, _, interface_path, _ in self.__prop_database.load_all_props():
+            if (
+                self.__introspection.get_interface(interface_name).is_server_owned()
+                and (interface_name, interface_path) not in allowed_properties
+            ):
+                logging.debug("Removing the property at: %s/%s.", interface_name, interface_path)
+                self.__prop_database.delete_prop(interface_name, interface_path)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/introspection.py` & `astarte-device-sdk-0.12.0/astarte/device/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-# Copyright 2020-2021 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
+
 from __future__ import annotations
 
 from astarte.device.interface import Interface
 
 
 class Introspection:
     """
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/mapping.py` & `astarte-device-sdk-0.12.0/astarte/device/mapping.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,34 @@
-# Copyright 2020-2021 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from datetime import datetime
 from math import isfinite
+from re import sub, match
 from typing import Union, List
 
+from astarte.device.exceptions import ValidationError, InterfaceFileDecodeError
+
 # Astarte Types definition
 IntList = List[int]
 FloatList = List[float]
 StringList = List[str]
 BsonList = List[bytes]
 BoolList = List[bool]
 DatetimeList = List[datetime]
@@ -54,15 +61,15 @@
     "doublearray": list,
     "stringarray": list,
     "binaryblobarray": list,
     "booleanarray": list,
     "datetimearray": list,
 }
 
-""" Mapping quality of service """
+# Mapping quality of service
 QOS_MAP = {"unreliable": 0, "guaranteed": 1, "unique": 2}
 
 
 class Mapping:
     """
     Class that represent a data Mapping
     Mappings are designed around REST controller semantics: each mapping describes an endpoint
@@ -75,41 +82,41 @@
     Attributes
     ----------
     endpoint: str
         Path of the Mapping
     type: str
         Type of the Mapping (see notes)
     explicit_timestamp: bool
-        Flag that defines if the Mapping requires a timestamp associated to the Payload before send
+        Flag that defines if the Mapping requires a timestamp associated to the Payload before send.
     reliability:
         Reliability level of the Mapping (see notes)
 
     Notes
     -----
         **Supported data types**
 
         The following types are supported:
 
         * double: A double-precision floating-point number as specified by binary64, by the IEEE
-        754 standard (NaNs and other non-numerical values are not supported).
+            754 standard (NaNs and other non-numerical values are not supported).
         * integer: A signed 32 bit integer.
         * boolean: Either true or false, adhering to JSON boolean type.
         * longinteger: A signed 64-bit integer (please note that longinteger is represented as a
-        string by default in JSON-based APIs.).
+            string by default in JSON-based APIs.).
         * string: An UTF-8 string, at most 65536 bytes long.
         * binaryblob: An arbitrary sequence of any byte that should be shorter than 64 KiB. (
-        binaryblob is represented as a base64 string by default in JSON-based APIs.).
+            binaryblob is represented as a base64 string by default in JSON-based APIs.).
         * datetime: A UTC timestamp, internally represented as milliseconds since 1st Jan 1970
-        using a signed 64 bits integer. (datetime is represented as an ISO 8601 string by default
-        in JSON based APIs.)
+            using a signed 64 bits integer. (datetime is represented as an ISO 8601 string by
+            default in JSON based APIs.)
         * doublearray, integerarray, booleanarray, longintegerarray, stringarray,
-        binaryblobarray, datetimearray: A list of values, represented as a JSON Array.
-        Arrays can have up to 1024 items and each item must respect the limits of its scalar type
-        (i.e. each string in a stringarray must be at most 65535 bytes long, each binary blob in
-        a binaryblobarray must be shorter than 64 KiB.)
+            binaryblobarray, datetimearray: A list of values, represented as a JSON Array.
+            Arrays can have up to 1024 items and each item must respect the limits of its scalar
+            type (i.e. each string in a stringarray must be at most 65535 bytes long, each binary
+            blob in a binaryblobarray must be shorter than 64 KiB.)
 
         **Quality of Service**
 
         Data messages QoS is chosen according to mapping settings, such as reliability.
         Properties are always published using QoS 2.
 
         ============== ============== ===
@@ -125,78 +132,119 @@
     def __init__(self, mapping_definition: dict, interface_type: str):
         """
         Parameters
         ----------
         mapping_definition: dict
             Mapping from the mappings array of an Astarte Interface definition in the form of a
             Python dictionary. Usually obtained by using json.loads() on an Interface file.
-        interface_type:
+        interface_type: str
             Type of the parent Interface, used to determine the default reliability
         """
-        self.endpoint: str = mapping_definition["endpoint"]
-        self.type: str = mapping_definition["type"]
-        self.__actual_type = type_strings.get(mapping_definition["type"])
+        self.endpoint: str = mapping_definition.get("endpoint")
+        self.type: str = mapping_definition.get("type")
+        self.__actual_type = type_strings.get(mapping_definition.get("type"))
         self.explicit_timestamp = mapping_definition.get("explicit_timestamp", False)
-        self.reliability = 2
-        if interface_type == "datastream":
-            if "reliability" in mapping_definition:
-                self.reliability = QOS_MAP[mapping_definition["reliability"]]
-            else:
-                self.reliability = 0
+        default_reliability = "unreliable" if interface_type == "datastream" else "unique"
+        self.reliability = QOS_MAP.get(mapping_definition.get("reliability", default_reliability))
+        self.allow_unset = mapping_definition.get("allow_unset", False)
+
+        if not (isinstance(self.endpoint, str) and self.__actual_type):
+            raise InterfaceFileDecodeError("Error parsing the mapping.")
+        if (interface_type != "datastream") and any(
+            k in mapping_definition for k in ("explicit_timestamp", "reliability")
+        ):
+            raise InterfaceFileDecodeError(
+                "Fields 'reliability' and 'explicit_timestamp' have no meaning for properties."
+            )
+        if ("allow_unset" in mapping_definition) and (interface_type != "properties"):
+            raise InterfaceFileDecodeError("Field 'allow_unset' have no meaning for datastreams.")
 
-    def validate(self, payload: MapType, timestamp: datetime) -> tuple[bool, str]:
+    def validate_path(self, path: str) -> ValidationError | None:
         """
         Mapping data validation
 
         Parameters
         ----------
-        payload: MapType
-            Data to validate
+        path: Str
+            Path to validate.
+
+        Returns
+        -------
+        ValidationError or None
+            None in case of successful validation, ValidationError otherwise
+        """
+        regex = sub(r"%{\w+}", r"[^/+#]+", self.endpoint)
+        if not match(regex + "$", path):
+            return ValidationError(f"Path {path} does not match the endpoint {self.endpoint}")
+        return None
+
+    def validate_timestamp(self, timestamp: datetime | None) -> ValidationError | None:
+        """
+        Mapping timestamp validation
+
+        Parameters
+        ----------
         timestamp: datetime or None
             Timestamp associated to the payload
 
         Returns
         -------
-        bool
-            Success of the validation operation
-        str
-            Error message if success is False
+        ValidationError or None
+            None in case of successful validation, ValidationError otherwise
+        """
+        if self.explicit_timestamp and not timestamp:
+            return ValidationError(f"Timestamp required for {self.endpoint}")
+        if not self.explicit_timestamp and timestamp:
+            return ValidationError(f"It's not possible to set the timestamp for {self.endpoint}")
+        return None
+
+    def validate_payload(self, payload: MapType) -> ValidationError | None:
+        """
+        Mapping data validation
+
+        Parameters
+        ----------
+        payload: MapType
+            Data to validate
+
+        Returns
+        -------
+        ValidationError or None
+            None in case of successful validation, ValidationError otherwise
         """
         min_supported_int = -2147483648
         max_supported_int = 2147483647
+        if payload in [None, []]:
+            return ValidationError(f"Attempting to validate an empty payload for {self.endpoint}")
         # Check if the interface has explicit_timestamp when a timestamp is given (and viceversa)
-        if self.explicit_timestamp and not timestamp:
-            return False, f"Timestamp required for {self.endpoint}"
-        if not self.explicit_timestamp and timestamp:
-            return False, f"It's not possible to set the timestamp for {self.endpoint}"
         # Check the type of data is valid for that endpoint
-        if not isinstance(payload, self.__actual_type):
-            return (
-                False,
-                f"{self.endpoint} is {self.type} but {type(payload)} was provided",
+        # pylint: disable-next=unidiomatic-typecheck
+        if not type(payload) is self.__actual_type:
+            return ValidationError(
+                f"{self.endpoint} is {self.type} but {type(payload)} was provided"
             )
         # Must return False when trying to send an integer outside allowed interval.
         if self.type == "integer" and not min_supported_int <= payload <= max_supported_int:
-            return False, f"Value out of int32 range for {self.endpoint}"
+            return ValidationError(f"Value out of int32 range for {self.endpoint}")
         # Must return False when trying to send a double value which is not a number
         if self.type == "double" and not isfinite(payload):
-            return False, f"Invalid float value for {self.endpoint}"
+            return ValidationError(f"Invalid float value for {self.endpoint}")
         # Check types of all element in a list
         if self.__actual_type == list:
             # Check coherence
-            if any(not isinstance(elem, type(payload[0])) for elem in payload):
-                return False, "Type incoherence in payload elements"
+            if any(not type(elem) is type(payload[0]) for elem in payload):
+                return ValidationError("Type incoherence in payload elements")
             subtype: type = type_strings.get(self.type.replace("array", ""))
-            if not isinstance(payload[0], subtype):
-                return (
-                    False,
-                    f"{self.endpoint} is {self.type} but {type(payload)} was provided",
+            # pylint: disable-next=unidiomatic-typecheck
+            if not type(payload[0]) is subtype:
+                return ValidationError(
+                    f"{self.endpoint} is {self.type} but a list of {type(payload[0])} was provided"
                 )
             # Must return False when trying to send an integer outside allowed interval.
             if self.type == "integerarray" and any(
                 elem < min_supported_int or elem > max_supported_int for elem in payload
             ):
-                return False, f"Value out of int32 range for {self.endpoint}"
+                return ValidationError(f"Value out of int32 range for {self.endpoint}")
             # Must return False when trying to send a double value which is not a number
             if self.type == "doublearray" and any(not isfinite(elem) for elem in payload):
-                return False, f"Invalid float value for {self.endpoint}"
-        return True, ""
+                return ValidationError(f"Invalid float value for {self.endpoint}")
+        return None
```

### Comparing `astarte-device-sdk-0.11.0/astarte/device/pairing_handler.py` & `astarte-device-sdk-0.12.0/astarte/device/pairing_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-# Copyright 2020-2021 SECO Mind S.r.l.
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
-# http://www.apache.org/licenses/LICENSE-2.0
+#    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 import datetime
 import http
 from base64 import urlsafe_b64encode
 from uuid import UUID, uuid5, uuid4
@@ -329,25 +333,27 @@
     Returns
     -------
     dict
         The Authorization Header dict.
 
     Raises
     ------
-    TypeError
+    JWTGenerationError
         If there is an error generating the token from the certificate
     """
     headers = {}
     try:
         headers[
             "Authorization"
         ] = f'Bearer {__generate_token(private_key_file, key_type="pairing")}'
         return headers
-    except Exception as exc:
-        raise TypeError("Supplied Realm Key could not be used to generate a valid Token.") from exc
+    except jwt.exceptions.PyJWTError as exc:
+        raise exceptions.JWTGenerationError("Error encoding or decoding the JWT token.") from exc
+    except IOError as exc:
+        raise exceptions.JWTGenerationError("Error opening the private key file.") from exc
 
 
 def __register_device_headers_with_jwt_token(jwt_token: str) -> dict:
     """
     Private utility function that generates the Authorization header for astarte HTTP APIs
 
     Parameters
```

### Comparing `astarte-device-sdk-0.11.0/astarte_device_sdk.egg-info/PKG-INFO` & `astarte-device-sdk-0.12.0/astarte_device_sdk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,101 +1,108 @@
 Metadata-Version: 2.1
 Name: astarte-device-sdk
-Version: 0.11.0
+Version: 0.12.0
 Summary: Astarte Device SDK for Python
 Home-page: https://github.com/astarte-platform/astarte-device-sdk-python
-Author: Francesco Vaiani
-Author-email: francesco.vaiani@secomind.com
+Author: Simone Orru
+Author-email: simone.orru@secomind.com
 License: License :: OSI Approved :: Apache Software License
-Description: # Astarte Python Device SDK
-        
-        Python Device SDK for [Astarte](https://github.com/astarte-platform/astarte). Create Astarte Devices
-        and Simulators with Python3.
-        It integrates with asyncio to ensure a smooth developer experience and to hide complex details
-        regarding threading and MQTT interactions.
-        
-        ## How to get with Pip
-        
-        The Astarte device SDK can be obtained by running:
-        ```
-        pip install astarte-device-sdk
-        ```
-        
-        ## Basic usage
-        
-        ### Create a device
-        
-        Initializing an instance of a device can be performed in three steps, as seen below.
-        ```python
-        from astarte.device import Device
-        
-        # Create the device instance
-        device = Device(
-            device_id="device id",
-            realm="realm",
-            credentials_secret="credentials secret",
-            pairing_base_url="pairing url",
-            persistency_dir=".",
-            loop=None,
-            ignore_ssl_errors=False,
-        )
-        # Add all the interfaces for this device
-        for interface in interfaces:
-            device.add_interface(interface)
-        # Connect to Astarte
-        device.connect()
-        ```
-        
-        ### Publish data from device
-        
-        Publishing new values can be performed using the `send` and `send_aggregate` functions.
-        ```python
-        from astarte.device import Device
-        from datetime import datetime, timezone
-        
-        # ... Create a device and connect it to Astarte ...
-        
-        # Send an individual datastream or a property
-        device.send(
-            interface_name="datastream_interface",
-            interface_path=f"/path/name",
-            payload="payload",
-            timestamp=None,
-        )
-        
-        # Send an aggregated object datastream
-        payload = {"endpoint1": "value1", "endpoint2": 42}
-        device.send_aggregate(
-            interface_name="aggregate_interface",
-            interface_path=f"/path/name",
-            payload=payload,
-            timestamp=datetime.now(tz=timezone.utc),
-        )
-        ```
-        
-        ### Receive a server publication
-        
-        The device automatically polls for new messages. The user can use a call back function to process
-        received data. Callback functions are also available for connect/disconnect events.
-        ```python
-        from astarte.device import Device
-        
-        def my_callback(device: Device, name: str, path: str, payload: dict):
-            print(f"Received message for {name}{path}: {payload}")
-        
-        # ... Create a device and connect it to Astarte ...
-        
-        # Setup the callback
-        device.on_data_received = my_callback
-        
-        # Keep the program running
-        while True:
-            pass
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: static
+Provides-Extra: unit
 Provides-Extra: e2e
+
+<!--
+Copyright 2023 SECO Mind Srl
+
+SPDX-License-Identifier: Apache-2.0
+-->
+
+# Astarte Python Device SDK
+
+Python Device SDK for [Astarte](https://github.com/astarte-platform/astarte). Create Astarte Devices
+and Simulators with Python3.
+It integrates with asyncio to ensure a smooth developer experience and to hide complex details
+regarding threading and MQTT interactions.
+
+## How to get with Pip
+
+The Astarte device SDK can be obtained by running:
+```
+pip install astarte-device-sdk
+```
+
+## Basic usage
+
+### Create a device
+
+Initializing an instance of a device can be performed in three steps, as seen below.
+```python
+from astarte.device import Device
+
+# Create the device instance
+device = Device(
+    device_id="device id",
+    realm="realm",
+    credentials_secret="credentials secret",
+    pairing_base_url="pairing url",
+    persistency_dir=".",
+    loop=None,
+    ignore_ssl_errors=False,
+)
+# Add a single interface from a .json file
+device.add_interface_from_file(Path("interfaces/path/file.json"))
+# Use `device.add_interfaces_from_dir(Path("interfaces/path"))` instead to add all the interfaces in a directory
+# Connect to Astarte
+device.connect()
+```
+
+### Publish data from device
+
+Publishing new values can be performed using the `send` and `send_aggregate` functions.
+```python
+from astarte.device import Device
+from datetime import datetime, timezone
+
+# ... Create a device and connect it to Astarte ...
+
+# Send an individual datastream or a property
+device.send(
+    interface_name="datastream_interface",
+    interface_path=f"/path/name",
+    payload="payload",
+    timestamp=None,
+)
+
+# Send an aggregated object datastream
+payload = {"endpoint1": "value1", "endpoint2": 42}
+device.send_aggregate(
+    interface_name="aggregate_interface",
+    interface_path=f"/path/name",
+    payload=payload,
+    timestamp=datetime.now(tz=timezone.utc),
+)
+```
+
+### Receive a server publication
+
+The device automatically polls for new messages. The user can use a call back function to process
+received data. Callback functions are also available for connect/disconnect events.
+```python
+from astarte.device import Device
+
+def my_callback(device: Device, name: str, path: str, payload: dict):
+    print(f"Received message for {name}{path}: {payload}")
+
+# ... Create a device and connect it to Astarte ...
+
+# Setup the callback
+device.on_data_received = my_callback
+
+# Keep the program running
+while True:
+    pass
+```
```

### Comparing `astarte-device-sdk-0.11.0/setup.py` & `astarte-device-sdk-0.12.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,38 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# For a fully annotated version of this file and what it does, see
-# https://github.com/pypa/sampleproject/blob/master/setup.py
-
-# To upload this file to PyPI you must build it then upload it:
-# python setup.py sdist bdist_wheel  # build in 'dist' folder
-# python-m twine upload dist/*  # 'twine' must be installed: 'pip install twine'
-
+# This file is part of Astarte.
+#
+# Copyright 2023 SECO Mind Srl
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#    http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+# SPDX-License-Identifier: Apache-2.0
 
 import ast
 import io
 import re
 import os
 from setuptools import find_namespace_packages, setup
 
-DEPENDENCIES = ["requests>=2.22.0", "paho-mqtt", "cryptography", "bson", "PyJWT>=1.7.0"]
+DEPENDENCIES = [
+    "requests>=2.22.0",
+    "paho-mqtt",
+    "cryptography",
+    "bson",
+    "PyJWT>=1.7.0",
+]
 EXCLUDE_FROM_PACKAGES = ["contrib", "docs", "tests*", "venv"]
 CURDIR = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(CURDIR, "README.md"), "r", encoding="utf-8") as f:
     README = f.read()
 
 
@@ -31,31 +44,33 @@
         version = match.group("version") if match is not None else '"unknown"'
     return str(ast.literal_eval(version))
 
 
 setup(
     name="astarte-device-sdk",
     version=get_version(),
-    author="Francesco Vaiani",
-    author_email="francesco.vaiani@secomind.com",
+    author="Simone Orru",
+    author_email="simone.orru@secomind.com",
     description="Astarte Device SDK for Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/astarte-platform/astarte-device-sdk-python",
-    packages=find_namespace_packages(include=['astarte.*'], exclude=EXCLUDE_FROM_PACKAGES),
+    packages=find_namespace_packages(include=["astarte.*"], exclude=EXCLUDE_FROM_PACKAGES),
     include_package_data=True,
     keywords=[],
     scripts=[],
     zip_safe=False,
     install_requires=DEPENDENCIES,
     extras_require={
-        "e2e": ["termcolor", "python-dateutil"]
+        "static": ["black", "pylint"],
+        "unit": ["setuptools", "pytest", "pytest-cov"],
+        "e2e": ["termcolor", "python-dateutil"],
     },
     test_suite="tests.test_project",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     # license and classifier list:
     # https://pypi.org/pypi?%3Aaction=list_classifiers
     license="License :: OSI Approved :: Apache Software License",
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

