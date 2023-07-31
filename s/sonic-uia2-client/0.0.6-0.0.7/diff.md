# Comparing `tmp/sonic-uia2-client-0.0.6.tar.gz` & `tmp/sonic-uia2-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.6.tar", last modified: Mon Jul 24 03:02:12 2023, max compression
+gzip compressed data, was "sonic-uia2-client-0.0.7.tar", last modified: Mon Jul 31 02:24:39 2023, max compression
```

## Comparing `sonic-uia2-client-0.0.6.tar` & `sonic-uia2-client-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/client/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/android_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/client/uia_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/common/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/resp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/common/sonic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-24 03:02:12.000000 sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.026600 sonic-uia2-client-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/tests/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 03:02:12.030600 sonic-uia2-client-0.0.6/uia2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/uia2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-24 03:01:56.000000 sonic-uia2-client-0.0.6/uia2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.269989 sonic-uia2-client-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-31 02:24:39.269989 sonic-uia2-client-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.265989 sonic-uia2-client-0.0.7/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/client/android_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/client/uia_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.265989 sonic-uia2-client-0.0.7/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/resp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/common/sonic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 02:24:39.269989 sonic-uia2-client-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.265989 sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-31 02:24:39.000000 sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-31 02:24:39.000000 sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 02:24:39.000000 sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 02:24:39.000000 sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.265989 sonic-uia2-client-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/tests/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 02:24:39.269989 sonic-uia2-client-0.0.7/uia2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/uia2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-31 02:24:29.000000 sonic-uia2-client-0.0.7/uia2/driver.py
```

### Comparing `sonic-uia2-client-0.0.6/LICENSE` & `sonic-uia2-client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/PKG-INFO` & `sonic-uia2-client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.6/README.md` & `sonic-uia2-client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/client/android_element.py` & `sonic-uia2-client-0.0.7/client/android_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,16 @@
         self.uia_client.check_session_id()
         b = self.uia_client.get_resp_handler().get_resp(
             HttpUtil.create_get(
                 f"{self.uia_client.remote_url}/session/{self.uia_client.get_session_id()}/element/{self.id}/rect"
             )
         )
         if b.err is None:
-            element_rect = ElementRect(**json.loads(b.value))
+            rect = b.value if isinstance(b.value, dict) else json.loads(b.value)
+            element_rect = ElementRect(**rect)
             self.logger.info(f"get {self.id} rect {element_rect}.")
             return element_rect
         else:
             self.logger.error(f"get {self.id} rect failed.")
             raise SonicRespException(b.err.message)
 
     def screenshot(self) -> bytes:
```

### Comparing `sonic-uia2-client-0.0.6/client/uia_client.py` & `sonic-uia2-client-0.0.7/client/uia_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import time
 from base64 import b64decode, b64encode
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Union
 
 from client.android_element import AndroidElement
 from common.http_client import HttpUtil, HttpRequest
 from common.logger import Logger
 from common.models import BaseResp, Method, WindowSize
 from common.resp_handler import RespHandler
 from common.sonic_exception import SonicRespException
@@ -285,7 +285,52 @@
             ).body(json.dumps(data))
         )
         if b.err is None:
             self.logger.info("set appium settings %s.", json.dumps(settings))
         else:
             self.logger.error("set appium settings failed.")
             raise SonicRespException(b.err.message)
+
+    def tap(self, x: int, y: int):
+        self.check_session_id()
+        data = {"x": x, "y": y}
+        b = self.resp_handler.get_resp(
+            HttpUtil.create_post(
+                self._remote_url + "/session/" + self.session_id + "/appium/tap"
+            ).body(json.dumps(data))
+        )
+        if b.err is None:
+            self.logger.info("perform tap action %s.", json.dumps(data))
+        else:
+            self.logger.error("perform tap action failed.")
+            raise SonicRespException(b.err.message)
+
+    def long_press(self, x: Union[int, float], y: Union[int, float], duration_ms: Union[int, float]):
+        self.check_session_id()
+        touch_event_params = {"x": x, "y": y, "duration": duration_ms}
+        data = {"params": touch_event_params}
+        b = self.resp_handler.get_resp(
+            HttpUtil.create_post(
+                self._remote_url + "/session/" + self.session_id + "/touch/longclick"
+            ).body(json.dumps(data))
+        )
+        if b.err is None:
+            self.logger.info("perform long_press action %s.", json.dumps(data))
+        else:
+            self.logger.error("perform long_press action failed.")
+            raise SonicRespException(b.err.message)
+
+    def swipe(self, start_x: Union[int, float], start_y: Union[int, float], end_x: Union[int, float],
+              end_y: Union[int, float], duration_ms: Union[int, float]):
+        self.check_session_id()
+        steps = int(duration_ms / 5) if duration_ms else 100
+        data = {"startX": start_x, "startY": start_y, "endX": end_x, "endY": end_y, "steps": steps}
+        b = self.resp_handler.get_resp(
+            HttpUtil.create_post(
+                self._remote_url + "/session/" + self.session_id + "/touch/perform"
+            ).body(json.dumps(data))
+        )
+        if b.err is None:
+            self.logger.info("perform swipe action %s.", json.dumps(data))
+        else:
+            self.logger.error("perform swipe action failed.")
+            raise SonicRespException(b.err.message)
```

### Comparing `sonic-uia2-client-0.0.6/common/http_client.py` & `sonic-uia2-client-0.0.7/common/http_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/common/logger.py` & `sonic-uia2-client-0.0.7/common/logger.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/common/models.py` & `sonic-uia2-client-0.0.7/common/models.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/common/resp_handler.py` & `sonic-uia2-client-0.0.7/common/resp_handler.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.6/setup.py` & `sonic-uia2-client-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 6
+PATCH = 7
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 setup(
     name="sonic-uia2-client",
     version=VERSION,
     author="SonicCloudOrg",
     author_email="soniccloudorg@163.com",
```

### Comparing `sonic-uia2-client-0.0.6/sonic_uia2_client.egg-info/PKG-INFO` & `sonic-uia2-client-0.0.7/sonic_uia2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.6/tests/test_driver.py` & `sonic-uia2-client-0.0.7/tests/test_driver.py`

 * *Files identical despite different names*

