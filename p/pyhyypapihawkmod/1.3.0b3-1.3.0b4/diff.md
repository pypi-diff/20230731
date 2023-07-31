# Comparing `tmp/pyhyypapihawkmod-1.3.0b3.tar.gz` & `tmp/pyhyypapihawkmod-1.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.3.0b3.tar", last modified: Sun Jul 30 16:44:24 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.3.0b4.tar", last modified: Mon Jul 31 07:33:04 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.3.0b3.tar` & `pyhyypapihawkmod-1.3.0b4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.863539 pyhyypapihawkmod-1.3.0b3/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-30 16:44:24.862034 pyhyypapihawkmod-1.3.0b3/PKG-INFO
--rw-rw-rw-   0        0        0     3094 2023-07-30 16:43:15.000000 pyhyypapihawkmod-1.3.0b3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.841998 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      410 2023-07-30 15:49:06.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      162 2023-07-30 07:50:36.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    12324 2023-07-30 07:42:04.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    32745 2023-07-30 16:39:10.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4114 2023-07-30 16:00:32.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     1999 2023-07-30 15:55:41.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/imei.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    17749 2023-07-30 16:15:07.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-30 16:44:24.860040 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      576 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-30 16:44:24.000000 pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 16:44:24.864035 pyhyypapihawkmod-1.3.0b3/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-30 15:18:53.000000 pyhyypapihawkmod-1.3.0b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.959539 pyhyypapihawkmod-1.3.0b4/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-31 07:33:04.958027 pyhyypapihawkmod-1.3.0b4/PKG-INFO
+-rw-rw-rw-   0        0        0     3250 2023-07-31 07:29:05.000000 pyhyypapihawkmod-1.3.0b4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.941525 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      410 2023-07-30 15:49:06.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      162 2023-07-30 07:50:36.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    12324 2023-07-30 07:42:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    32743 2023-07-31 07:26:33.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4114 2023-07-30 16:00:32.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     1999 2023-07-30 15:55:41.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/imei.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    17749 2023-07-30 16:15:07.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:04.955531 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      576 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 07:33:04.000000 pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:33:04.960037 pyhyypapihawkmod-1.3.0b4/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-31 07:26:36.000000 pyhyypapihawkmod-1.3.0b4/setup.py
```

### Comparing `pyhyypapihawkmod-1.3.0b3/LICENSE.md` & `pyhyypapihawkmod-1.3.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/PKG-INFO` & `pyhyypapihawkmod-1.3.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b3
+Version: 1.3.0b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b3/README.md` & `pyhyypapihawkmod-1.3.0b4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. THis fixes the issues on newer versions of home assistant.
+This is a fork from https://github.com/RenierM26. This fork has reversed engineered the protobuf pb2 files and recompiled with version 4.21. This fixes the issues on newer versions of home assistant and incorporated several new features. See the main integration: https://github.com/hawky358/hass_ids_hyyp for more information.
 
 # pyHyypApi
 API for ADT Secure Home and IDS Hyyp. There could be more variants but it's easy to add package names to the constants.py file.
 
 
 How to use:
 
   1. Install:
 
 ```pip install pyhyypapihawkmod```
 
   2.1. Login (ADT Secure Home):
-
-
 ```
 import pyhyypapihawkmod
 import json
 client = pyhyypapihawkmod.hyypclient(email="",password="")
 client.login()
 ```
 
@@ -37,14 +35,17 @@
 
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
+1.3.0b4
+- Minor Refactoring
+
 1.3.0b3
 - Hotfix, notifications appear to go to random people. Implemented random IMEI
 
 1.3.0b2
 - Implementation of push receiver.
 
 1.3.0b1
```

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,28 +57,30 @@
         self._session = requests.session()
         self._session.headers.update(REQUEST_HEADER)
         STD_PARAMS["pkg"] = pkg
         STD_PARAMS["token"] = token
         STD_PARAMS["userId"] = userid
         STD_PARAMS["imei"] = imei
         self._timeout = timeout
-        self.callback_function_alarm_info = None
-        self.callback_function_fcm_info = None
         self.time_to_push = PUSH_DELAY
         self.forced_refresh = False
         self.alarminfos = HyypAlarmInfos(self)
         self.fcm_listener = FCMListener()
         self.fcm_register = FCMRegistration()
         self.fcm_credentials = fcm_credentials
+    
         
     def login(self) -> Any:
         """Login to ADT Secure Home API."""
 
-
-
+        if STD_PARAMS["imei"] is None:
+            _LOGGER.warning("No IMEI found, this warning should not be seen in home assistant.")
+            STD_PARAMS["imei"] = self.generate_imei()
+            _LOGGER.warning("Generated session IMEI " + str(STD_PARAMS["imei"]))
+            
         _params = STD_PARAMS.copy()
         _params["email"] = self._email
         _params["password"] = self._password
         try:
             req = self._session.get(
                 "https://" + BASE_URL + API_ENDPOINT_LOGIN,
                 allow_redirects=False,
@@ -154,68 +156,64 @@
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(
                 f"Error checking app version from api: {_json_result['error']}"
             )
 
         return _json_result
 
-    def alarm_info_push_timer(self):
+    def alarm_info_push_timer(self, callback):
         SLEEP_DELAY = 0.1
         while 1:
             if self.forced_refresh and self.time_to_push > REQUEST_PUSH_TIMEOUT:
                 self.time_to_push = REQUEST_PUSH_TIMEOUT
             while self.time_to_push > 0:
                 time.sleep(SLEEP_DELAY)
                 self.time_to_push -= SLEEP_DELAY
             alarminfo = self.load_alarm_infos()
-            self.callback_function_alarm_info(alarminfo)
+            callback(alarminfo)
             self.forced_refresh = False
             self.time_to_push = PUSH_DELAY
 
     def request_alarm_info_push_to_hass(self):
         self.forced_refresh = True
         self.time_to_push = REQUEST_PUSH_TIMEOUT
         
-    def initialize_alarm_info_push_timer(self):
-        thread.Thread(target=self.alarm_info_push_timer).start()
+    def initialize_alarm_info_push_timer(self, callback):
+        thread.Thread(target=self.alarm_info_push_timer,
+                      kwargs={"callback" : callback}).start()
 
-    def register_alarm_info_callback(self, callback_function):
-        self.callback_function_alarm_info = callback_function
+        
 
     def load_alarm_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
         forced = self.forced_refresh
         #return HyypAlarmInfos(self).status()
         return self.alarminfos.status(forced=forced)
 
-    def initialize_fcm_notification_listener(self, persistent_pids = None):
-        
+    def initialize_fcm_notification_listener(self, callback, persistent_pids = None):
         if self.fcm_credentials is None:
             _LOGGER.warning("No FCM credentials available, disabling notifications")
             return
         if "fcm" not in self.fcm_credentials:
             _LOGGER.warning("No FCM credentials available, disabling notifications")
             return
         thread.Thread(target=self.fcm_notification_thread,
-                      kwargs={'persistent_ids': persistent_pids}).start()
-        #thread.Thread(target=self.alarm_info_push_timer).start()
+                      kwargs={"persistent_ids" : persistent_pids,
+                              "callback" : callback
+                              }).start()
 
 
-    def fcm_notification_thread(self, persistent_ids = None):
+    def fcm_notification_thread(self, callback, persistent_ids = None):
         gcm_address = self.fcm_credentials["fcm"]["token"]
         self.store_gcm_registrationid(gcm_id=gcm_address)  
-        self.fcm_listener.runner(callback=self.callback_function_fcm_info,
+        self.fcm_listener.runner(callback=callback,
                                  credentials=self.fcm_credentials,
                                  persistent_ids=persistent_ids)
 
 
-    def register_fcm_info_callback(self, callback_function):
-        self.callback_function_fcm_info = callback_function
-        
-
     def get_intial_fcm_credentials(self):
         return self.fcm_register.register(sender_id=GCF_SENDER_ID)
         # error checker??
 
 
     def get_debug_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
```

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/imei.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/imei.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.3.0b3
+Version: 1.3.0b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.3.0b3/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.3.0b4/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.3.0b3/setup.py` & `pyhyypapihawkmod-1.3.0b4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.3.0b3",
+    version="1.3.0b4",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

