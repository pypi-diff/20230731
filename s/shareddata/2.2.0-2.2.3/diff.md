# Comparing `tmp/shareddata-2.2.0.tar.gz` & `tmp/shareddata-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.2.0.tar", last modified: Mon Jul 31 11:19:43 2023, max compression
+gzip compressed data, was "shareddata-2.2.3.tar", last modified: Mon Jul 31 11:52:37 2023, max compression
```

## Comparing `shareddata-2.2.0.tar` & `shareddata-2.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.0/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:19:43.032148 shareddata-2.2.0/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.0/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.0/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 11:19:43.032148 shareddata-2.2.0/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.028148 shareddata-2.2.0/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.0/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.0/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.0/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.0/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1358 2023-07-29 20:08:45.000000 shareddata-2.2.0/src/SharedData/Feeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.0/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1222 2023-07-29 20:09:03.000000 shareddata-2.2.0/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11258 2023-07-29 20:08:46.000000 shareddata-2.2.0/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.0/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15066 2023-07-29 20:08:40.000000 shareddata-2.2.0/src/SharedData/Period.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.0/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2458 2023-07-29 20:09:00.000000 shareddata-2.2.0/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.0/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.2.0/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.0/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8626 2023-07-29 20:38:54.000000 shareddata-2.2.0/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.0/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.0/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16353 2023-07-31 11:18:41.000000 shareddata-2.2.0/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.0/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.0/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.3/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:52:37.242063 shareddata-2.2.3/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.3/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.3/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 11:52:37.242063 shareddata-2.2.3/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.3/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.3/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.3/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.3/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1358 2023-07-29 20:08:45.000000 shareddata-2.2.3/src/SharedData/Feeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.3/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.3/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11195 2023-07-31 11:51:26.000000 shareddata-2.2.3/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.3/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15066 2023-07-29 20:08:40.000000 shareddata-2.2.3/src/SharedData/Period.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.3/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.3/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.3/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.2.3/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.3/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8626 2023-07-29 20:38:54.000000 shareddata-2.2.3/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.3/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.3/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16353 2023-07-31 11:18:41.000000 shareddata-2.2.3/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.3/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.3/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.2.0/LICENSE` & `shareddata-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/PKG-INFO` & `shareddata-2.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.0
+Version: 2.2.3
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.0/README.md` & `shareddata-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/setup.cfg` & `shareddata-2.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.2.0
+version = 2.2.3
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.2.0/src/SharedData/AWSKinesis.py` & `shareddata-2.2.3/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/AWSS3.py` & `shareddata-2.2.3/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/DataFrame.py` & `shareddata-2.2.3/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Defaults.py` & `shareddata-2.2.3/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Feeder.py` & `shareddata-2.2.3/src/SharedData/Feeder.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Logger.py` & `shareddata-2.2.3/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.2.3/src/SharedData/LoggerConsumerProcess.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import time
 import numpy as np
 
+
+from SharedData.SharedData import SharedData
+shdata = SharedData(__file__,user='worker')
 from SharedData.Logger import Logger
-logger = Logger(__file__,user='worker')
 from SharedData.AWSKinesis import KinesisLogStreamConsumer
 
 SLEEP_TIME = 2
 
 def run():
     Logger.log.info('Starting SharedDataLogsConsumer process')
     consumer = KinesisLogStreamConsumer(user='worker')
```

### Comparing `shareddata-2.2.0/src/SharedData/Metadata.py` & `shareddata-2.2.3/src/SharedData/Metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 
 from SharedData.Logger import Logger
 from SharedData.AWSS3 import S3Upload, S3ListFolder, S3Download, UpdateModTime
 
 class Metadata():
     
     def __init__(self, name, mode='rw', user='master'):
-        
-        if Logger.log is None:
-            Logger('Metadata')
-        
+                
         self.user = user
         
         self.s3read = False
         self.s3write = False
         if mode == 'r':
             self.s3read = True
             self.s3write = False
```

### Comparing `shareddata-2.2.0/src/SharedData/MultiProc.py` & `shareddata-2.2.3/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Period.py` & `shareddata-2.2.3/src/SharedData/Period.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/RealTime.py` & `shareddata-2.2.3/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/RealTimeProcess.py` & `shareddata-2.2.3/src/SharedData/RealTimeProcess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os,time,sys
 import pandas as pd
 import numpy as np
 from pathlib import Path
 
-from SharedData.Logger import Logger
-logger = Logger(__file__)
 from SharedData.SharedData import SharedData
+shdata = SharedData(__file__,user='worker')
+from SharedData.Logger import Logger
 from SharedData.AWSKinesis import KinesisStreamConsumer
 
 
 try:
     if len(sys.argv)>=2:
         DATABASE = str(sys.argv[1])
     else:
```

### Comparing `shareddata-2.2.0/src/SharedData/SharedData.py` & `shareddata-2.2.3/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/SharedNumpy.py` & `shareddata-2.2.3/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Table.py` & `shareddata-2.2.3/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/TableIndex.py` & `shareddata-2.2.3/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/TableIndexJit.py` & `shareddata-2.2.3/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/TimeSeries.py` & `shareddata-2.2.3/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/TimeseriesContainer.py` & `shareddata-2.2.3/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/SharedData/Utils.py` & `shareddata-2.2.3/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.2.3/src/shareddata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.0
+Version: 2.2.3
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.0/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.2.3/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

