# Comparing `tmp/agora_busclient-1.1.37-py2.py3-none-any.whl.zip` & `tmp/agora_busclient-1.1.38-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 14481 bytes, number of entries: 22
+Zip file size: 14487 bytes, number of entries: 22
 -rw-r--r--  2.0 fat      261 b- defN 23-Jul-28 12:34 agora_busclient/__init__.py
 -rw-r--r--  2.0 fat     2974 b- defN 23-Jul-27 15:56 agora_busclient/base_mqtt_client.py
 -rw-r--r--  2.0 fat     3220 b- defN 23-Jul-27 16:58 agora_busclient/bus_client.py
 -rw-r--r--  2.0 fat     4272 b- defN 23-Jul-31 12:20 agora_busclient/message_queue.py
 -rw-r--r--  2.0 fat     5115 b- defN 23-May-19 17:55 agora_busclient/mqtt_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-31 12:21 agora_busclient/version.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-31 12:58 agora_busclient/version.py
 -rw-r--r--  2.0 fat      432 b- defN 23-Jul-10 22:39 agora_busclient/messages/__init__.py
--rw-r--r--  2.0 fat     1693 b- defN 23-Jul-27 17:21 agora_busclient/messages/event_msg.py
+-rw-r--r--  2.0 fat     1666 b- defN 23-Jul-31 12:37 agora_busclient/messages/event_msg.py
 -rw-r--r--  2.0 fat      233 b- defN 23-May-12 13:38 agora_busclient/messages/io_device_data.py
 -rw-r--r--  2.0 fat      678 b- defN 23-May-12 13:38 agora_busclient/messages/io_point.py
 -rw-r--r--  2.0 fat      565 b- defN 23-May-12 13:38 agora_busclient/messages/io_tag_data_dict.py
 -rw-r--r--  2.0 fat     1918 b- defN 23-May-12 13:38 agora_busclient/messages/iodatareport_message.py
 -rw-r--r--  2.0 fat      950 b- defN 23-Jul-27 17:24 agora_busclient/messages/media_data.py
 -rw-r--r--  2.0 fat      799 b- defN 23-May-12 13:38 agora_busclient/messages/message_header.py
--rw-r--r--  2.0 fat     7651 b- defN 23-Jul-31 12:09 agora_busclient/messages/msg_decoder.py
+-rw-r--r--  2.0 fat     7674 b- defN 23-Jul-31 12:57 agora_busclient/messages/msg_decoder.py
 -rw-r--r--  2.0 fat     3881 b- defN 23-Jul-31 12:09 agora_busclient/messages/msg_encoder.py
 -rw-r--r--  2.0 fat      581 b- defN 23-May-12 13:38 agora_busclient/messages/request_msg.py
 -rw-r--r--  2.0 fat      129 b- defN 23-Jul-11 16:30 agora_busclient/messages/work_flow.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.37.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.37.dist-info/WHEEL
--rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.37.dist-info/METADATA
--rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.37.dist-info/RECORD
-22 files, 38733 bytes uncompressed, 11159 bytes compressed:  71.2%
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_busclient-1.1.38.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_busclient-1.1.38.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1123 b- defN 16-Jan-01 00:00 agora_busclient-1.1.38.dist-info/METADATA
+-rw-r--r--  2.0 fat     2000 b- defN 16-Jan-01 00:00 agora_busclient-1.1.38.dist-info/RECORD
+22 files, 38729 bytes uncompressed, 11165 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: agora_busclient/messages/request_msg.py
 Comment: 
 
 Filename: agora_busclient/messages/work_flow.py
 Comment: 
 
-Filename: agora_busclient-1.1.37.dist-info/LICENSE
+Filename: agora_busclient-1.1.38.dist-info/LICENSE
 Comment: 
 
-Filename: agora_busclient-1.1.37.dist-info/WHEEL
+Filename: agora_busclient-1.1.38.dist-info/WHEEL
 Comment: 
 
-Filename: agora_busclient-1.1.37.dist-info/METADATA
+Filename: agora_busclient-1.1.38.dist-info/METADATA
 Comment: 
 
-Filename: agora_busclient-1.1.37.dist-info/RECORD
+Filename: agora_busclient-1.1.38.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_busclient/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.37'
+__version__ = '1.1.38'
```

## agora_busclient/messages/event_msg.py

```diff
@@ -4,16 +4,15 @@
 from .media_data import MediaData
 from .work_flow import WorkFlow
 from typing import List
 
 class EventMsg:
     event_id = -1
 
-    def __init__(self):
-        self.Type = ""            
+    def __init__(self):         
         if EventMsg.event_id == -1:
             EventMsg.event_id = self.__get_event_id()
         EventMsg.event_id = EventMsg.event_id + 1
         self.EventId = EventMsg.event_id        
       
         if config["GROUP_ID"] is None or config["GROUP_ID"] == "":
             self.GroupId = ""
```

## agora_busclient/messages/msg_decoder.py

```diff
@@ -122,28 +122,43 @@
             if 'MotEdgeFilename' in d:
                 ret.MotEdgeFilename = d['MotEdgeFilename']
             if 'MIMEType' in d:
                 ret.MIMEType = d['MIMEType']
             if 'AltText' in d:
                 ret.AltText = d['AltText']
             if 'RawData' in d:
-                ret.AltText = d['RawData']
+                ret.RawData = d['RawData']
             try:
                 if 'DetectedStart_tm' in d:
                     ret.DetectedStart_tm = float(str(d['DetectedStart_tm']))
             except:
                 ret.DetectedStart_tm = -1
             try:
                 if 'DetectedEnd_tm' in d:
                     ret.DetectedEnd_tm = float(str(d['DetectedEnd_tm']))
             except:
                 ret.DetectedEnd_tm = -1
             return ret
         if o == EventMsg:                     
             ret = EventMsg()  
+            try:
+                if 'Sent_tm' in d:
+                    ret.Sent_tm = float(str(d['Sent_tm']))
+            except:
+                ret.Sent_tm = -1
+            try:
+                if 'Start_tm' in d:
+                    ret.Start_tm = float(str(d['Start_tm']))
+            except:
+                ret.Start_tm = -1
+            try:
+                if 'End_tm' in d:
+                    ret.End_tm = float(str(d['End_tm']))
+            except:
+                ret.End_tm = -1
             if 'workFlow' in d:  
                 wrkflw = WorkFlow()  
                 if 'Type' in d['workFlow']:                   
                     ret.workFlow.Type = d['workFlow']['Type']     
                 if 'Properties' in d['workFlow']:                   
                      ret.workFlow.Properties = d['workFlow']['Properties']                
             if 'EventId' in d:
@@ -152,40 +167,25 @@
                 ret.GroupId = d['GROUP_ID']    
             if 'GATEWAY_ID' in d:
                 ret.GatewayId = d['GATEWAY_ID']    
             if 'DEVICE_ID' in d:
                 ret.ControllerId = d['DEVICE_ID']                   
             if 'mediaData' in d:               
                 for d in d['mediaData']:
-                    ret.mediaDataRef.append(self.__decode(d, MediaData))
-            try:
-                if 'Start_tm' in d:
-                    ret.Start_tm = float(str(d['Start_tm']))
-            except:
-                ret.Start_tm = -1
-            try:
-                if 'End_tm' in d:
-                    ret.End_tm = float(str(d['End_tm']))
-            except:
-                ret.End_tm = -1
+                    ret.mediaDataRef.append(self.__decode(d, MediaData))           
             try:
                 if 'DetectedStart_tm' in d:
                     ret.DetectedStart_tm = float(str(d['DetectedStart_tm']))
             except:
                 ret.DetectedStart_tm = -1
             try:
                 if 'DetectedEnd_tm' in d:
                     ret.DetectedEnd_tm = float(str(d['DetectedEnd_tm']))
             except:
-                ret.DetectedEnd_tm = -1
-            try:
-                if 'Sent_tm' in d:
-                    ret.Sent_tm = float(str(d['Sent_tm']))
-            except:
-                ret.Sent_tm = -1
+                ret.DetectedEnd_tm = -1            
             try:
                 if 'Created_tm' in d:
                     ret.Created_tm = float(str(d['Created_tm']))
             except:
                 ret.Created_tm = -1            
             try:
                 if 'Detected_tm' in d:
```

## Comparing `agora_busclient-1.1.37.dist-info/METADATA` & `agora_busclient-1.1.38.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: agora_busclient
-Version: 1.1.37
+Version: 1.1.38
 Summary: Bus Client libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.37
-Requires-Dist: agora_config == 1.1.37
-Requires-Dist: agora_utils == 1.1.37
+Requires-Dist: agora_logging == 1.1.38
+Requires-Dist: agora_config == 1.1.38
+Requires-Dist: agora_utils == 1.1.38
 Requires-Dist: paho-mqtt
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_busclient
 
  This package is the Bus Client library for the Agora Edge Apps SDK (Python) developed by SLB.
```

## Comparing `agora_busclient-1.1.37.dist-info/RECORD` & `agora_busclient-1.1.38.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 agora_busclient/__init__.py,sha256=u5C1uUUYJLFPg8rdFdLLUBkNZjPznbShJPz_6k7T8nc,261
 agora_busclient/base_mqtt_client.py,sha256=3TOsWL_LOfnxtj73slPj-L3I1kqc1niqW3C_m8tuSjQ,2974
 agora_busclient/bus_client.py,sha256=9SypfvNAuv_Tct1uwDMgj7dg-BdoLvk3aEWi2FpTPS0,3220
 agora_busclient/message_queue.py,sha256=McVJOphO8VvbwR7Kv4nrYedLdT3LivYeqfpCXoP8Rog,4272
 agora_busclient/mqtt_client.py,sha256=I87pojxwhaAzIrjU1HSlXOL2XkK8m-YCT2SD9mFYEFU,5115
-agora_busclient/version.py,sha256=wzQumjbBZLB6HKa1UYl1fLkDW0jP3nh0f7OOTqs5o6s,25
+agora_busclient/version.py,sha256=BPlAo_MDT13g-sG5NVbqsmNEMiY3Bh651OBWao0zlPU,25
 agora_busclient/messages/__init__.py,sha256=SXI28GSrnaOZxDpXYqH4emANTRWlGDjvKVsClgtQGqw,432
-agora_busclient/messages/event_msg.py,sha256=55cfh04jB9CeuIUZRlnUwb9wY9ijSbjtpkpJHKUmO0Y,1693
+agora_busclient/messages/event_msg.py,sha256=OP0Zb-QdhjEakeE26MOwUS0fpIzJCpOF5mThUi_hLz8,1666
 agora_busclient/messages/io_device_data.py,sha256=6-IyVdps8AquyivHUzS5LU4iIpIMIxBSdmOWZ1l187E,233
 agora_busclient/messages/io_point.py,sha256=J9nqULZ09fQxUneB1zcXNk5poOR7Uf9JwqkwrlQkFe8,678
 agora_busclient/messages/io_tag_data_dict.py,sha256=1-hmLr6RTtkeHdqfr7A8kGom3ZxkC8lHOfw3yDHk2ic,565
 agora_busclient/messages/iodatareport_message.py,sha256=u3ckr4Wx8qk-ce2pNcd6D3nBIJ09YrBlid57V1BKe1A,1918
 agora_busclient/messages/media_data.py,sha256=qjPR53XXC3WHEJeAiobNm0zeGr3dwrDI7RHBABtnga8,950
 agora_busclient/messages/message_header.py,sha256=Hk0slDisem-mIlpeosHpj1AxNSQqz7uerH8yUj6_-Jw,799
-agora_busclient/messages/msg_decoder.py,sha256=H1t5fp8g6IJ4x4ILMPw_1mb_Fz80rzKpZV-bn8yjkl4,7651
+agora_busclient/messages/msg_decoder.py,sha256=9E3LUsY3Ron_Ua4fdnUDt7kfUHG2xozTM3ZSqZkWvS0,7674
 agora_busclient/messages/msg_encoder.py,sha256=ipDoFBXu7X5GuBa-C68-zadwAmTZzF7Jsuxbw8x8ktQ,3881
 agora_busclient/messages/request_msg.py,sha256=LdtaEHkf2M4aA0I-XILzw9EQK0XNPi3H7M_O2z3AuMs,581
 agora_busclient/messages/work_flow.py,sha256=u1a7i4Inins3w9qThnz4CUkB-eYp6mkVsukJqr9x-n8,129
-agora_busclient-1.1.37.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_busclient-1.1.37.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_busclient-1.1.37.dist-info/METADATA,sha256=a3VJxFsTZLAhxBpt8CvnqNkyeVA7T2C9KH7DfO_X5CQ,1123
-agora_busclient-1.1.37.dist-info/RECORD,,
+agora_busclient-1.1.38.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_busclient-1.1.38.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_busclient-1.1.38.dist-info/METADATA,sha256=_QdyuPE_ttJOnNTEXkpJ_Ev0jOBDs8fz-t0Fr1Rld_Y,1123
+agora_busclient-1.1.38.dist-info/RECORD,,
```

