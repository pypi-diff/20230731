# Comparing `tmp/volt_client_web-0.1.8.tar.gz` & `tmp/volt_client_web-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volt_client_web-0.1.8.tar", max compression
+gzip compressed data, was "volt_client_web-0.1.9.tar", max compression
```

## Comparing `volt_client_web-0.1.8.tar` & `volt_client_web-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     9139 2023-05-12 11:38:50.050175 volt_client_web-0.1.8/README.md
--rw-r--r--   0        0        0      574 2023-07-31 08:57:15.582203 volt_client_web-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      769 2023-05-12 11:38:50.050175 volt_client_web-0.1.8/volt_client_web/__init__.py
--rw-r--r--   0        0        0    11484 2023-05-12 11:38:50.050175 volt_client_web-0.1.8/volt_client_web/crypto_utils.py
--rw-r--r--   0        0        0    22815 2023-07-10 09:44:26.246204 volt_client_web-0.1.8/volt_client_web/volt_client.py
--rw-r--r--   0        0        0     8750 2023-07-25 15:29:31.353977 volt_client_web-0.1.8/volt_client_web/websocket_rpc.py
--rw-r--r--   0        0        0    10168 1970-01-01 00:00:00.000000 volt_client_web-0.1.8/setup.py
--rw-r--r--   0        0        0     9893 1970-01-01 00:00:00.000000 volt_client_web-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     9139 2023-05-12 11:38:50.050175 volt_client_web-0.1.9/README.md
+-rw-r--r--   0        0        0      574 2023-07-31 12:40:55.324651 volt_client_web-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      769 2023-05-12 11:38:50.050175 volt_client_web-0.1.9/volt_client_web/__init__.py
+-rw-r--r--   0        0        0    11484 2023-05-12 11:38:50.050175 volt_client_web-0.1.9/volt_client_web/crypto_utils.py
+-rw-r--r--   0        0        0    22815 2023-07-10 09:44:26.246204 volt_client_web-0.1.9/volt_client_web/volt_client.py
+-rw-r--r--   0        0        0     8655 2023-07-31 12:40:35.064834 volt_client_web-0.1.9/volt_client_web/websocket_rpc.py
+-rw-r--r--   0        0        0     9893 1970-01-01 00:00:00.000000 volt_client_web-0.1.9/PKG-INFO
```

### Comparing `volt_client_web-0.1.8/README.md` & `volt_client_web-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `volt_client_web-0.1.8/pyproject.toml` & `volt_client_web-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "volt-client-web"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python websocket client API"
 authors = ["Ash Setter <ash@nquiringminds.com>"]
 license = "UNLISENCED"
 readme = "README.md"
 packages = [{include = "volt_client_web"}]
 
 [tool.poetry.dependencies]
```

### Comparing `volt_client_web-0.1.8/volt_client_web/__init__.py` & `volt_client_web-0.1.9/volt_client_web/__init__.py`

 * *Files identical despite different names*

### Comparing `volt_client_web-0.1.8/volt_client_web/crypto_utils.py` & `volt_client_web-0.1.9/volt_client_web/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `volt_client_web-0.1.8/volt_client_web/volt_client.py` & `volt_client_web-0.1.9/volt_client_web/volt_client.py`

 * *Files identical despite different names*

### Comparing `volt_client_web-0.1.8/volt_client_web/websocket_rpc.py` & `volt_client_web-0.1.9/volt_client_web/websocket_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,15 @@
     
     async def on_message(self):
         """
         Coroutine that listens for incoming messages from the server.
         """
         while not self.complete:
             try:
-                # message = await self.websocket.recv(timeout=1)
-                message = await asyncio.wait_for(self.websocket.recv(), timeout=10)
+                message = await self.websocket.recv()
                 # TODO: remove need for the below sleep command
                 # sleep for receive_delay after processing received message
                 # this is to avoid receiving another message while the last message is still being processed
                 await asyncio.sleep(self.receive_delay)
             except Exception as err:
                 print("Exception in on message here: ", err)
                 self.emit("error", err)
```

### Comparing `volt_client_web-0.1.8/setup.py` & `volt_client_web-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,204 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: volt-client-web
+Version: 0.1.9
+Summary: Python websocket client API
+License: UNLISENCED
+Author: Ash Setter
+Author-email: ash@nquiringminds.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: base58 (>=2.1.1,<3.0.0)
+Requires-Dist: cryptography (>=40.0.1,<41.0.0)
+Requires-Dist: jsonrpcclient (>=4.0.3,<5.0.0)
+Requires-Dist: pyee (>=9.0.4,<10.0.0)
+Requires-Dist: pytest-asyncio (>=0.21.0,<0.22.0)
+Requires-Dist: websockets (>=11.0.2,<12.0.0)
+Description-Content-Type: text/markdown
+
+[![PyPI version](https://badge.fury.io/py/volt_client_web.svg)](https://badge.fury.io/py/volt_client_web)
+
+# TDX volt python websocket client API.
+
+## Configuration
+
+In order to be able to initialise a connection to a Volt, you will need to obtain a [client configuration](https://docs.tdxvolt.com/en/reference/connection).
+
+Example client connection object, obtained from the **fusebox** identity dialog:
+
+```python
+BobsConfig = {
+  "client_name": "Bob",
+  "credential": {
+    "client_id": "25d050b9-5270-441e-920b-de07578394a9",
+    "key": "-----BEGIN ENCRYPTED PRIVATE KEY-----\nMIIFHDBOBgkqhkiG9w0BBQ0wQTApBgkqhkiG9w0BBQwwHAQIRalkrxf/Lt0CAggA\nMAwGCCqGSIb3DQIJBQAwFAYIKoZIhvcNAwcECADS3HqZSdqbBIIEyFH7ooxVlpVn\nxVWA/e32E322VDc/FnlDlUkBm7C4haHdbgIsLSa0AhbazAgI45ibCg9PapD4uKQO\nx1X8NyyxwqsFTYHtX3cxtgY7I3Q2iM7jvyDlvjzc68Q0o0eE7Xk7Et4hEd4aiD3I\nt9EgIsNnSIHXbnXKTYrYD3P939AyQE5wECgKrmEXq/6ymbeBkTcYRg6tqcW9otjs\nuvRgfl5+QFpxE9rydMn0Yjm+wp5L6j2oD/yVTPVNkEKBgefngeqaj3cCsPDxFVOa\n/zBBFb17Kyn6eGga4pUNyg0xKi8TjYHcH5k7GzN6MHjaIVlls0TbbBHk1/tfrfF3\nSL26162J2qHmR4vosOtTzPCNYVlT85NVL3PO/xN1OTsoz6mjP5sScgoTnzi48B1s\nqyl4BMjpkK7j/KwsaVnEdNog+UVO/4lSbrM86KzwH9O6Xuv4WeIIC3sET+v8nQwq\nVNc3vXjDleRJbPONollHt/CLErkhh2sh6CguDFqqJlr+HYyDhbVBzw57jLEmE51M\npeK+LyaX/N2TxrXlIF774TOuEV6NzbPldIn0I4XcCXZhXN0stTiH6LPKS3CMdZTy\nKNgyRAsFXRfQ3F0A9MPqbRcxmyA7v/kLtukZ6ib33B6eY049SlduhbI0eKWt1jqs\nv05o6gDiLyYsyAzzMzl+OvRsPXyRZ6xVhI59uWBM9/EW8JKWwZ09mJGJ1A3tEpT4\nidka0Vfvy3XYL3KZKYD6u/NqpqfS7KW37C4iwtXHWUCLuFsA0HLD4SZOCen2b8fZ\nTNcbfR+brR5KqCrkK40NuejheQWlQi/eLYsCooTHRfpXPF2mQZJRgKxefoPFD6MZ\nWtoW97u10lRCWB1vuTlkq79uwyY+sqY0qTuWxeBdD9zmJeBJkR/QpdTlBUwRTlaQ\nMw529N/5N0haA3PJfwDwEV1Gv5BMNGIda8zx8BG+qv3plvWSUS0YTTGRBTl8GLQ5\nHKMbmTP41544UpcFHKCTtlUKO04rM8U9y4tLSxQp4Xw84fVw4MFNYyd8MLtYqc9j\nH93MGjHY3jx8PedEE8EaSX+JAh3cRYkD9+k9CswDnWxeQ0SIvLz0qL7Y82davVdO\nyOvkvCM7WzuvgMjfIZDGEVsoh4zI7PmVluUXW5SNtrQJhcLn8DsA4FCAXYaWGKXR\ndTupWI9kfCA+7f31ZNkrGUQ+CQFIrDozZzLbNqFv+QODirMIGYNsgeiqbSo1CXHR\n+/L5dc5ZtCK5AWKglgXOgWo2qxTEq9LaYWa6MiPaH3rwMqp9/r7HVsxfDJI0v1z2\n0hGfSkO47NnhHKsjTHfHCoDi7vC3a+w9T4tS/zm1VL9+Ay9uHi4Svq9KVexKYv5J\nim4a91CSIxfsMhN4t3UiciZz8NgU8mfbaZOcL6T1NDFZhT+1HngifCoM8g/Al0J7\nILiT8qNx7e0+TSRKreeGiWSUCJrRykx5Wk/8dCKsKx4hNrXTDlTA6w/ByduO4zKq\n/lXQQfRik1rVSj2Vkt1Jp15hwTL9o7OarmqgpWB5P4iBchEg9hSB70BSM7axK1wS\nxX58fGAQaws4NvNquUxSG3QGuxA2I6AfZeYuyH8x/Vy2MjBtOEopmxVVWHpdGPzW\nf42MsgXLVz6+SBAIc+beTw==\n-----END ENCRYPTED PRIVATE KEY-----\n",
+  },
+  "volt": {
+    "id": "9a5944eb-1942-406e-a553-39b4220cbf94",
+    "display_name": "Bob's Volt",
+    "address": "192.168.1.194:50393",
+    "public_key":
+      "-----BEGIN PUBLIC KEY-----\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAshZ/IqKr1y0TeMgT4l4f\nc/LrCCjg+lIXD4FE9Na3kL0kRTSwda6FsGM4EmuU0NVK+UZ6ViFEhrgA4DCbMf8h\nefuFcWWfHq17zzkdI65vI1Lh9qdKzYNK0FZ3pKoVQyXtpdomZ8rChosFpdDRm1gS\nmV4sTPvKzsFHSTxcOlHRZ/CMtuS09cPvWuuJ4Lm3VmIr70wYSVfC/78SxJYHGYDj\nwkaBqqBwNxIamxO4dwJ8azpdNLnBEeSnhzt2OP2dLu82l1IdjzJlbEWWlL3R1pdG\n55lf/Y9CySAMQyupbiKX1sOPZ1MWWsweAZNMChQtt8hup67vJV4/MOuLeLEF8em9\ncwIDAQAB\n-----END PUBLIC KEY-----\n",
+    "fingerprint": "5M1aCpnijWbmibq748AHnyG1qgpHMFmLi5UUeaGBGo8t",
+    "ca_pem":
+      "-----BEGIN CERTIFICATE-----\nMIIDojCCAoqgAwIBAgIEG/pk5zANBgkqhkiG9w0BAQsFADBxMQswCQYDVQQGEwJH\nQjEUMBIGA1UEBwwLU291dGhhbXB0b24xGjAYBgNVBAoMEW5xdWlyaW5nTWluZHMg\nTHRkMTAwLgYDVQQDDCdjYS45YTU5NDRlYi0xOTQyLTQwNmUtYTU1My0zOWI0MjIw\nY2JmOTQwHhcNMjIwOTE1MTQxNDI1WhcNMjMwOTE1MTQxNDI2WjBxMQswCQYDVQQG\nEwJHQjEUMBIGA1UEBwwLU291dGhhbXB0b24xGjAYBgNVBAoMEW5xdWlyaW5nTWlu\nZHMgTHRkMTAwLgYDVQQDDCdjYS45YTU5NDRlYi0xOTQyLTQwNmUtYTU1My0zOWI0\nMjIwY2JmOTQwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQCyFn8ioqvX\nLRN4yBPiXh9z8usIKOD6UhcPgUT01reQvSRFNLB1roWwYzgSa5TQ1Ur5RnpWIUSG\nuADgMJsx/yF5+4VxZZ8erXvPOR0jrm8jUuH2p0rNg0rQVnekqhVDJe2l2iZnysKG\niwWl0NGbWBKZXixM+8rOwUdJPFw6UdFn8Iy25LT1w+9a64ngubdWYivvTBhJV8L/\nvxLElgcZgOPCRoGqoHA3EhqbE7h3AnxrOl00ucER5KeHO3Y4/Z0u7zaXUh2PMmVs\nRZaUvdHWl0bnmV/9j0LJIAxDK6luIpfWw49nUxZazB4Bk0wKFC23yG6nru8lXj8w\n64t4sQXx6b1zAgMBAAGjQjBAMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQD\nAgEGMB0GA1UdDgQWBBQNruu/5F1KEvJYHz5hmlfyryQhOjANBgkqhkiG9w0BAQsF\nAAOCAQEAm7mtXgQTftbcN05wQlStJ9IY+PaKkrvXJbJyl9PXOVgw5XNb9qTBzRl+\nTuEdK9N054jxHmkH9bqXObCLp/mo2xbQoavG87tILGMilv2VxEyKKzUaYc2IshYR\nY3zGT+QqC7IIfZHjVOgdc3+wwgm8ntRCYS23Z10+sE5o4lZGxiUkrGod1kjEKOaD\n5AiJ9bC3rI/tAapn14GemzsCagvVY8WzP8GW6WVz+pQCoJvy9jsHkQIq9djpzx29\nJ0hg12H9d2InnsJ8QdUIzbSPwyD8H+upKVtQZ/fVcZd3NtAuR6xo2yG3aSumdhmV\nrBJ5F7SB7WXo5/z0aXxYvCcrUqLgxA==\n-----END CERTIFICATE-----\n",
+  },
+}
+```
 
-packages = \
-['volt_client_web']
+## Connection
 
-package_data = \
-{'': ['*']}
+Create a **tdx Volt** instance to enable Bob to connect to the Volt:
 
-install_requires = \
-['base58>=2.1.1,<3.0.0',
- 'cryptography>=40.0.1,<41.0.0',
- 'jsonrpcclient>=4.0.3,<5.0.0',
- 'pyee>=9.0.4,<10.0.0',
- 'pytest-asyncio>=0.21.0,<0.22.0',
- 'websockets>=11.0.2,<12.0.0']
-
-setup_kwargs = {
-    'name': 'volt-client-web',
-    'version': '0.1.8',
-    'description': 'Python websocket client API',
-    'long_description': '[![PyPI version](https://badge.fury.io/py/volt_client_web.svg)](https://badge.fury.io/py/volt_client_web)\n\n# TDX volt python websocket client API.\n\n## Configuration\n\nIn order to be able to initialise a connection to a Volt, you will need to obtain a [client configuration](https://docs.tdxvolt.com/en/reference/connection).\n\nExample client connection object, obtained from the **fusebox** identity dialog:\n\n```python\nBobsConfig = {\n  "client_name": "Bob",\n  "credential": {\n    "client_id": "25d050b9-5270-441e-920b-de07578394a9",\n    "key": "-----BEGIN ENCRYPTED PRIVATE KEY-----\\nMIIFHDBOBgkqhkiG9w0BBQ0wQTApBgkqhkiG9w0BBQwwHAQIRalkrxf/Lt0CAggA\\nMAwGCCqGSIb3DQIJBQAwFAYIKoZIhvcNAwcECADS3HqZSdqbBIIEyFH7ooxVlpVn\\nxVWA/e32E322VDc/FnlDlUkBm7C4haHdbgIsLSa0AhbazAgI45ibCg9PapD4uKQO\\nx1X8NyyxwqsFTYHtX3cxtgY7I3Q2iM7jvyDlvjzc68Q0o0eE7Xk7Et4hEd4aiD3I\\nt9EgIsNnSIHXbnXKTYrYD3P939AyQE5wECgKrmEXq/6ymbeBkTcYRg6tqcW9otjs\\nuvRgfl5+QFpxE9rydMn0Yjm+wp5L6j2oD/yVTPVNkEKBgefngeqaj3cCsPDxFVOa\\n/zBBFb17Kyn6eGga4pUNyg0xKi8TjYHcH5k7GzN6MHjaIVlls0TbbBHk1/tfrfF3\\nSL26162J2qHmR4vosOtTzPCNYVlT85NVL3PO/xN1OTsoz6mjP5sScgoTnzi48B1s\\nqyl4BMjpkK7j/KwsaVnEdNog+UVO/4lSbrM86KzwH9O6Xuv4WeIIC3sET+v8nQwq\\nVNc3vXjDleRJbPONollHt/CLErkhh2sh6CguDFqqJlr+HYyDhbVBzw57jLEmE51M\\npeK+LyaX/N2TxrXlIF774TOuEV6NzbPldIn0I4XcCXZhXN0stTiH6LPKS3CMdZTy\\nKNgyRAsFXRfQ3F0A9MPqbRcxmyA7v/kLtukZ6ib33B6eY049SlduhbI0eKWt1jqs\\nv05o6gDiLyYsyAzzMzl+OvRsPXyRZ6xVhI59uWBM9/EW8JKWwZ09mJGJ1A3tEpT4\\nidka0Vfvy3XYL3KZKYD6u/NqpqfS7KW37C4iwtXHWUCLuFsA0HLD4SZOCen2b8fZ\\nTNcbfR+brR5KqCrkK40NuejheQWlQi/eLYsCooTHRfpXPF2mQZJRgKxefoPFD6MZ\\nWtoW97u10lRCWB1vuTlkq79uwyY+sqY0qTuWxeBdD9zmJeBJkR/QpdTlBUwRTlaQ\\nMw529N/5N0haA3PJfwDwEV1Gv5BMNGIda8zx8BG+qv3plvWSUS0YTTGRBTl8GLQ5\\nHKMbmTP41544UpcFHKCTtlUKO04rM8U9y4tLSxQp4Xw84fVw4MFNYyd8MLtYqc9j\\nH93MGjHY3jx8PedEE8EaSX+JAh3cRYkD9+k9CswDnWxeQ0SIvLz0qL7Y82davVdO\\nyOvkvCM7WzuvgMjfIZDGEVsoh4zI7PmVluUXW5SNtrQJhcLn8DsA4FCAXYaWGKXR\\ndTupWI9kfCA+7f31ZNkrGUQ+CQFIrDozZzLbNqFv+QODirMIGYNsgeiqbSo1CXHR\\n+/L5dc5ZtCK5AWKglgXOgWo2qxTEq9LaYWa6MiPaH3rwMqp9/r7HVsxfDJI0v1z2\\n0hGfSkO47NnhHKsjTHfHCoDi7vC3a+w9T4tS/zm1VL9+Ay9uHi4Svq9KVexKYv5J\\nim4a91CSIxfsMhN4t3UiciZz8NgU8mfbaZOcL6T1NDFZhT+1HngifCoM8g/Al0J7\\nILiT8qNx7e0+TSRKreeGiWSUCJrRykx5Wk/8dCKsKx4hNrXTDlTA6w/ByduO4zKq\\n/lXQQfRik1rVSj2Vkt1Jp15hwTL9o7OarmqgpWB5P4iBchEg9hSB70BSM7axK1wS\\nxX58fGAQaws4NvNquUxSG3QGuxA2I6AfZeYuyH8x/Vy2MjBtOEopmxVVWHpdGPzW\\nf42MsgXLVz6+SBAIc+beTw==\\n-----END ENCRYPTED PRIVATE KEY-----\\n",\n  },\n  "volt": {\n    "id": "9a5944eb-1942-406e-a553-39b4220cbf94",\n    "display_name": "Bob\'s Volt",\n    "address": "192.168.1.194:50393",\n    "public_key":\n      "-----BEGIN PUBLIC KEY-----\\nMIIBIjANBgkqhkiG9w0BAQEFAAOCAQ8AMIIBCgKCAQEAshZ/IqKr1y0TeMgT4l4f\\nc/LrCCjg+lIXD4FE9Na3kL0kRTSwda6FsGM4EmuU0NVK+UZ6ViFEhrgA4DCbMf8h\\nefuFcWWfHq17zzkdI65vI1Lh9qdKzYNK0FZ3pKoVQyXtpdomZ8rChosFpdDRm1gS\\nmV4sTPvKzsFHSTxcOlHRZ/CMtuS09cPvWuuJ4Lm3VmIr70wYSVfC/78SxJYHGYDj\\nwkaBqqBwNxIamxO4dwJ8azpdNLnBEeSnhzt2OP2dLu82l1IdjzJlbEWWlL3R1pdG\\n55lf/Y9CySAMQyupbiKX1sOPZ1MWWsweAZNMChQtt8hup67vJV4/MOuLeLEF8em9\\ncwIDAQAB\\n-----END PUBLIC KEY-----\\n",\n    "fingerprint": "5M1aCpnijWbmibq748AHnyG1qgpHMFmLi5UUeaGBGo8t",\n    "ca_pem":\n      "-----BEGIN CERTIFICATE-----\\nMIIDojCCAoqgAwIBAgIEG/pk5zANBgkqhkiG9w0BAQsFADBxMQswCQYDVQQGEwJH\\nQjEUMBIGA1UEBwwLU291dGhhbXB0b24xGjAYBgNVBAoMEW5xdWlyaW5nTWluZHMg\\nTHRkMTAwLgYDVQQDDCdjYS45YTU5NDRlYi0xOTQyLTQwNmUtYTU1My0zOWI0MjIw\\nY2JmOTQwHhcNMjIwOTE1MTQxNDI1WhcNMjMwOTE1MTQxNDI2WjBxMQswCQYDVQQG\\nEwJHQjEUMBIGA1UEBwwLU291dGhhbXB0b24xGjAYBgNVBAoMEW5xdWlyaW5nTWlu\\nZHMgTHRkMTAwLgYDVQQDDCdjYS45YTU5NDRlYi0xOTQyLTQwNmUtYTU1My0zOWI0\\nMjIwY2JmOTQwggEiMA0GCSqGSIb3DQEBAQUAA4IBDwAwggEKAoIBAQCyFn8ioqvX\\nLRN4yBPiXh9z8usIKOD6UhcPgUT01reQvSRFNLB1roWwYzgSa5TQ1Ur5RnpWIUSG\\nuADgMJsx/yF5+4VxZZ8erXvPOR0jrm8jUuH2p0rNg0rQVnekqhVDJe2l2iZnysKG\\niwWl0NGbWBKZXixM+8rOwUdJPFw6UdFn8Iy25LT1w+9a64ngubdWYivvTBhJV8L/\\nvxLElgcZgOPCRoGqoHA3EhqbE7h3AnxrOl00ucER5KeHO3Y4/Z0u7zaXUh2PMmVs\\nRZaUvdHWl0bnmV/9j0LJIAxDK6luIpfWw49nUxZazB4Bk0wKFC23yG6nru8lXj8w\\n64t4sQXx6b1zAgMBAAGjQjBAMA8GA1UdEwEB/wQFMAMBAf8wDgYDVR0PAQH/BAQD\\nAgEGMB0GA1UdDgQWBBQNruu/5F1KEvJYHz5hmlfyryQhOjANBgkqhkiG9w0BAQsF\\nAAOCAQEAm7mtXgQTftbcN05wQlStJ9IY+PaKkrvXJbJyl9PXOVgw5XNb9qTBzRl+\\nTuEdK9N054jxHmkH9bqXObCLp/mo2xbQoavG87tILGMilv2VxEyKKzUaYc2IshYR\\nY3zGT+QqC7IIfZHjVOgdc3+wwgm8ntRCYS23Z10+sE5o4lZGxiUkrGod1kjEKOaD\\n5AiJ9bC3rI/tAapn14GemzsCagvVY8WzP8GW6WVz+pQCoJvy9jsHkQIq9djpzx29\\nJ0hg12H9d2InnsJ8QdUIzbSPwyD8H+upKVtQZ/fVcZd3NtAuR6xo2yG3aSumdhmV\\nrBJ5F7SB7WXo5/z0aXxYvCcrUqLgxA==\\n-----END CERTIFICATE-----\\n",\n  },\n}\n```\n\n## Connection\n\nCreate a **tdx Volt** instance to enable Bob to connect to the Volt:\n\n```python\nimport asyncio # needed for async / await calls\nfrom volt_client_web import VoltClient\n\nconfig = ...\n\nvolt_client = VoltClient(config)\n```\n\nNow attempt to initialise the **tdx Volt** connection, to run async code in a python script you will need to create an async function and run it using asyncio:\n\n```python\nimport asyncio # needed for async / await calls\nfrom volt_client_web import VoltClient\n\nconfig = ...\n\nasync def main():\n  volt_client = VoltClient(config)\n  await volt_client.initialise()\n\nasyncio.run(main())\n```\n\nIf initialisation fails, an error will be thrown.\n\n## API call\n\nOnce initialised successfully, you can issue any API call.\n\nRefer to the [API documentation](https://docs.tdxvolt.com/en/api/volt_api) for details of the method names and corresponding request and response messages. Each API method expects a dictionary representing the request(s) as input, and returns a dictionary as indicated by the response message type. The dictionary of the protobuf message format is intuitive.\n\nIn the example below, we retrieve the resource associated with Bob’s home folder:\n\n```python\nimport asyncio # needed for async / await calls\nfrom volt_client_web import VoltClient\n\nconfig = ...\n\nasync def main():\n    volt_client = VoltClient(config)\n    await volt_client.initialise()\n    result = await volt_client.getResource({ "resourceId": config["credential"]["client_id"] })\n    print(result["resource"])\n\nasyncio.run(main())\n```\n\n## Unary calls\n\nAll unary calls return a promise that will either resolve with a dictionary matching that defined by the API protobuf, or reject if there is a problem with the grpc transport or an error status on the response object. The above API call example is a unary call.\n\n## Streaming calls\nThe promise model does not fit well with streaming calls since they are long-lived.\n\nFor this reason, all streaming calls (client streaming, server streaming, and bi-directional streaming) return a call object that is used to manage the call.\n\nThe call object emits events as interactions with the underlying websocket occur, and there are 3 events of interest:\n\n- “error” emitted when an error occurs on the call\n- “data” emitted when a response is received from the Volt\n- “end” emitted when the call ends\n\n### Server streaming calls\n\nThe example below shows execution of an SQL statement on a database, the data event will be emitted for each row of data in the result set.\n\nThe end event is emitted when the call ends.\n\n```python\nimport asyncio # needed for async / await calls\nfrom volt_client_web import VoltClient\n\nconfig = ...\n\nasync def main():\n    volt_client = VoltClient(config)\n    await volt_client.initialise()\n\n    call = await volt_client.sqlExecute(\n        {\n            "database_id": "fc17c5a1-a858-45c6-804b-7e16af7c968d",\n            "statement": "SELECT * FROM NETFLIX LIMIT 100"\n        }\n    )\n    @call.on("error")\n    def error_handler(error):\n        print(error)\n    \n    @call.on("data")\n    def data_handler(response):\n        print(response)\n\n    @call.on("end")\n    def end_handler():\n        print("complete")\n\nasyncio.run(main())\n```\n\n### Client streaming calls\nClient streaming calls have a similar syntax to server streaming calls, although the data event should only be emitted once rather than multiple times.\n\nClients can use the send method on the returned call object to send requests to the server (see bi-direction example below).\n\nClients use the end method of the returned call object to indicate to the server that the call has ended.\n\n### Bi-directional streaming calls\nAs expected, bi-directional calls are a combination of client and server streaming calls, whereby the data event is emitted for each response from the server, and the client can send multiple requests using the call object send method.\n\n```python\nimport asyncio # needed for async / await calls\nfrom volt_client_web import VoltClient\n\nconfig = ...\n\nasync def main():\n    volt_client = VoltClient(config)\n    await volt_client.initialise()\n\n    sub = await volt_client.subscribeWire(\n        {\n        "wire_id": "59dceb36-fafb-4c9e-a4c7-710cd16e9188",\n        }\n    )\n\n    @sub.on("error")\n    def error_handler(error):\n        print("error: ", error)\n    \n    @sub.on("data")\n    def data_handler(payload):\n        print("data: ", payload)\n\n    @sub.on("end")\n    def end_handler():\n        print("end reached")\n\n    #\n    # ...\n    #\n    \n    # Some time later, ask the server to end the subscription\n    await sub.send({"stop": True})\n\nasyncio.run(main())\n```\n',
-    'author': 'Ash Setter',
-    'author_email': 'ash@nquiringminds.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+```python
+import asyncio # needed for async / await calls
+from volt_client_web import VoltClient
+
+config = ...
+
+volt_client = VoltClient(config)
+```
+
+Now attempt to initialise the **tdx Volt** connection, to run async code in a python script you will need to create an async function and run it using asyncio:
+
+```python
+import asyncio # needed for async / await calls
+from volt_client_web import VoltClient
+
+config = ...
+
+async def main():
+  volt_client = VoltClient(config)
+  await volt_client.initialise()
+
+asyncio.run(main())
+```
+
+If initialisation fails, an error will be thrown.
+
+## API call
+
+Once initialised successfully, you can issue any API call.
+
+Refer to the [API documentation](https://docs.tdxvolt.com/en/api/volt_api) for details of the method names and corresponding request and response messages. Each API method expects a dictionary representing the request(s) as input, and returns a dictionary as indicated by the response message type. The dictionary of the protobuf message format is intuitive.
+
+In the example below, we retrieve the resource associated with Bob’s home folder:
+
+```python
+import asyncio # needed for async / await calls
+from volt_client_web import VoltClient
+
+config = ...
+
+async def main():
+    volt_client = VoltClient(config)
+    await volt_client.initialise()
+    result = await volt_client.getResource({ "resourceId": config["credential"]["client_id"] })
+    print(result["resource"])
+
+asyncio.run(main())
+```
+
+## Unary calls
+
+All unary calls return a promise that will either resolve with a dictionary matching that defined by the API protobuf, or reject if there is a problem with the grpc transport or an error status on the response object. The above API call example is a unary call.
+
+## Streaming calls
+The promise model does not fit well with streaming calls since they are long-lived.
+
+For this reason, all streaming calls (client streaming, server streaming, and bi-directional streaming) return a call object that is used to manage the call.
+
+The call object emits events as interactions with the underlying websocket occur, and there are 3 events of interest:
+
+- “error” emitted when an error occurs on the call
+- “data” emitted when a response is received from the Volt
+- “end” emitted when the call ends
+
+### Server streaming calls
+
+The example below shows execution of an SQL statement on a database, the data event will be emitted for each row of data in the result set.
+
+The end event is emitted when the call ends.
+
+```python
+import asyncio # needed for async / await calls
+from volt_client_web import VoltClient
+
+config = ...
+
+async def main():
+    volt_client = VoltClient(config)
+    await volt_client.initialise()
+
+    call = await volt_client.sqlExecute(
+        {
+            "database_id": "fc17c5a1-a858-45c6-804b-7e16af7c968d",
+            "statement": "SELECT * FROM NETFLIX LIMIT 100"
+        }
+    )
+    @call.on("error")
+    def error_handler(error):
+        print(error)
+    
+    @call.on("data")
+    def data_handler(response):
+        print(response)
+
+    @call.on("end")
+    def end_handler():
+        print("complete")
+
+asyncio.run(main())
+```
+
+### Client streaming calls
+Client streaming calls have a similar syntax to server streaming calls, although the data event should only be emitted once rather than multiple times.
+
+Clients can use the send method on the returned call object to send requests to the server (see bi-direction example below).
+
+Clients use the end method of the returned call object to indicate to the server that the call has ended.
+
+### Bi-directional streaming calls
+As expected, bi-directional calls are a combination of client and server streaming calls, whereby the data event is emitted for each response from the server, and the client can send multiple requests using the call object send method.
+
+```python
+import asyncio # needed for async / await calls
+from volt_client_web import VoltClient
+
+config = ...
+
+async def main():
+    volt_client = VoltClient(config)
+    await volt_client.initialise()
+
+    sub = await volt_client.subscribeWire(
+        {
+        "wire_id": "59dceb36-fafb-4c9e-a4c7-710cd16e9188",
+        }
+    )
+
+    @sub.on("error")
+    def error_handler(error):
+        print("error: ", error)
+    
+    @sub.on("data")
+    def data_handler(payload):
+        print("data: ", payload)
+
+    @sub.on("end")
+    def end_handler():
+        print("end reached")
+
+    #
+    # ...
+    #
+    
+    # Some time later, ask the server to end the subscription
+    await sub.send({"stop": True})
 
+asyncio.run(main())
+```
 
-setup(**setup_kwargs)
```

