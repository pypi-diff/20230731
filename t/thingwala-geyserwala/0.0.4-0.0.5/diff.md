# Comparing `tmp/thingwala_geyserwala-0.0.4-py3-none-any.whl.zip` & `tmp/thingwala_geyserwala-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 7492 bytes, number of entries: 13
+Zip file size: 7570 bytes, number of entries: 13
 -rw-r--r--  2.0 unx      255 b- defN 23-Jul-14 20:03 thingwala/geyserwala/__init__.py
--rw-r--r--  2.0 unx      664 b- defN 23-Jul-14 20:03 thingwala/geyserwala/const.py
+-rw-r--r--  2.0 unx      736 b- defN 23-Jul-31 16:59 thingwala/geyserwala/const.py
 -rw-r--r--  2.0 unx      564 b- defN 23-Jul-14 20:03 thingwala/geyserwala/errors.py
 -rw-r--r--  2.0 unx      255 b- defN 23-Jul-14 20:03 thingwala/geyserwala/aio/__init__.py
 -rw-r--r--  2.0 unx     2538 b- defN 23-Jul-14 20:03 thingwala/geyserwala/aio/cli.py
--rw-r--r--  2.0 unx     9292 b- defN 23-Jul-29 09:37 thingwala/geyserwala/aio/client.py
+-rw-r--r--  2.0 unx     9491 b- defN 23-Jul-31 17:12 thingwala/geyserwala/aio/client.py
 -rw-r--r--  2.0 unx     1494 b- defN 23-Jul-14 20:03 thingwala/geyserwala/aio/discovery.py
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx      294 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       64 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1182 b- defN 23-Jul-29 16:57 thingwala_geyserwala-0.0.4.dist-info/RECORD
-13 files, 17770 bytes uncompressed, 5470 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx      294 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       64 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1182 b- defN 23-Jul-31 17:34 thingwala_geyserwala-0.0.5.dist-info/RECORD
+13 files, 18041 bytes uncompressed, 5548 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: thingwala/geyserwala/aio/client.py
 Comment: 
 
 Filename: thingwala/geyserwala/aio/discovery.py
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/LICENSE
+Filename: thingwala_geyserwala-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/METADATA
+Filename: thingwala_geyserwala-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/WHEEL
+Filename: thingwala_geyserwala-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/entry_points.txt
+Filename: thingwala_geyserwala-0.0.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/top_level.txt
+Filename: thingwala_geyserwala-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: thingwala_geyserwala-0.0.4.dist-info/RECORD
+Filename: thingwala_geyserwala-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## thingwala/geyserwala/const.py

```diff
@@ -13,7 +13,9 @@
     GEYSERWALA_MODE_SOLAR,
     GEYSERWALA_MODE_HOLIDAY,
     GEYSERWALA_MODE_STANDBY,
 ]
 
 GEYSERWALA_SETPOINT_TEMP_MAX = 65
 GEYSERWALA_SETPOINT_TEMP_MIN = 30
+GEYSERWALA_AUTOMATION_TEMP_MAX = 75
+GEYSERWALA_AUTOMATION_TEMP_MIN = 30
```

## thingwala/geyserwala/aio/client.py

```diff
@@ -14,14 +14,16 @@
     GEYSERWALA_MODE_SETPOINT,
     GEYSERWALA_MODE_TIMER,
     GEYSERWALA_MODE_SOLAR,
     GEYSERWALA_MODE_HOLIDAY,
     GEYSERWALA_MODE_STANDBY,
     GEYSERWALA_SETPOINT_TEMP_MAX,
     GEYSERWALA_SETPOINT_TEMP_MIN,
+    GEYSERWALA_AUTOMATION_TEMP_MAX,
+    GEYSERWALA_AUTOMATION_TEMP_MIN,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 class GeyserwalaClientAsync:
@@ -119,20 +121,23 @@
                     json=json,
                     timeout=self._rest_timeout,
                 ) as rsp:
                     status = rsp.status
                     if status == 200:
                         json_blob = await rsp.json()
                         return json_blob
+        except asyncio.TimeoutError as ex:
+            raise RequestError from ex
         except (
             aiohttp.ClientError,
             aiohttp.http_exceptions.HttpProcessingError,
         ) as ex:
-            logger.error(
-                "aiohttp exception on %s %s [%s]: %s",
+            logger.warn(
+                "aiohttp exception %s on %s %s [%s]: %s",
+                ex.__class__.__name__,
                 method,
                 url,
                 getattr(ex, "status", None),
                 getattr(ex, "message", None),
             )
             raise RequestError() from ex
         except Exception as ex:
@@ -254,15 +259,15 @@
         return await self._set_value("external-demand", on)
 
     @property
     def external_setpoint(self):
         return self._status.get("external-setpoint", None)
 
     async def set_external_setpoint(self, external_setpoint: int):
-        if GEYSERWALA_SETPOINT_TEMP_MIN <= external_setpoint <= GEYSERWALA_SETPOINT_TEMP_MAX:
+        if GEYSERWALA_AUTOMATION_TEMP_MIN <= external_setpoint <= GEYSERWALA_AUTOMATION_TEMP_MAX:
             return await self._set_value("external-setpoint", external_setpoint)
         return False
 
     @property
     def lowpower_enable(self):
         return self._status.get("lowpower-enable", None)
```

## Comparing `thingwala_geyserwala-0.0.4.dist-info/LICENSE` & `thingwala_geyserwala-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `thingwala_geyserwala-0.0.4.dist-info/RECORD` & `thingwala_geyserwala-0.0.5.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 thingwala/geyserwala/__init__.py,sha256=qj4bLIyK36U1ivt7PWoFK42RCva4mKumbH87ANxqW-E,255
-thingwala/geyserwala/const.py,sha256=BIZNCcTpvc1_aJ9mgP2fhbnRArzGuNy2zBhpmgcyOX8,664
+thingwala/geyserwala/const.py,sha256=gTgE8IMItY5jbTu05Rt7XjxCz1cB652sl4oHs8kJOG4,736
 thingwala/geyserwala/errors.py,sha256=IyI4bUxTVplzSRbjr7tu7m4jR8oK6IIlbOD1GAFJP88,564
 thingwala/geyserwala/aio/__init__.py,sha256=qj4bLIyK36U1ivt7PWoFK42RCva4mKumbH87ANxqW-E,255
 thingwala/geyserwala/aio/cli.py,sha256=NN2gEzR7o5Jj2922C_OXb2exXvJbO76vjO3W3Z2-BM4,2538
-thingwala/geyserwala/aio/client.py,sha256=00iiFse0n-oZ1_oWvSxs5iF8Icz2bx-OVIO23YOTZ-Q,9292
+thingwala/geyserwala/aio/client.py,sha256=irWpLbouvEibTvJpLqS9qljMrxcPztWkGvKFAEC8f9E,9491
 thingwala/geyserwala/aio/discovery.py,sha256=VfNGOsKJVZCuiUj_kNAFr7vtTvgXLIsH6-0QAAy8-GQ,1494
-thingwala_geyserwala-0.0.4.dist-info/LICENSE,sha256=gyF__UD4feLqEiQaCB5ak8jdc8-1UZOBFKEL-Pf8Y6o,1066
-thingwala_geyserwala-0.0.4.dist-info/METADATA,sha256=NRktQnLRim6CdAfq5EHUNqldhlcilByfkRYuu6xL6l8,294
-thingwala_geyserwala-0.0.4.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-thingwala_geyserwala-0.0.4.dist-info/entry_points.txt,sha256=i-4-nYc2EWKZgp2OkdhunSjYOe7_7pkwsJ5B8bswt_M,64
-thingwala_geyserwala-0.0.4.dist-info/top_level.txt,sha256=n6rcs8stkw-UrgrGzIobTwxPz9yrId1tHNvUkdN94F4,10
-thingwala_geyserwala-0.0.4.dist-info/RECORD,,
+thingwala_geyserwala-0.0.5.dist-info/LICENSE,sha256=gyF__UD4feLqEiQaCB5ak8jdc8-1UZOBFKEL-Pf8Y6o,1066
+thingwala_geyserwala-0.0.5.dist-info/METADATA,sha256=rJ0e9IYRKsdEYxd8YX9fFL8xYg3q7eLEiYunqVyMqH4,294
+thingwala_geyserwala-0.0.5.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+thingwala_geyserwala-0.0.5.dist-info/entry_points.txt,sha256=i-4-nYc2EWKZgp2OkdhunSjYOe7_7pkwsJ5B8bswt_M,64
+thingwala_geyserwala-0.0.5.dist-info/top_level.txt,sha256=n6rcs8stkw-UrgrGzIobTwxPz9yrId1tHNvUkdN94F4,10
+thingwala_geyserwala-0.0.5.dist-info/RECORD,,
```

