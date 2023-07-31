# Comparing `tmp/shareddata-2.1.5.tar.gz` & `tmp/shareddata-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.1.5.tar", last modified: Thu Jul 27 17:39:10 2023, max compression
+gzip compressed data, was "shareddata-2.2.0.tar", last modified: Mon Jul 31 11:19:43 2023, max compression
```

## Comparing `shareddata-2.1.5.tar` & `shareddata-2.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.1.5/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 17:39:10.717709 shareddata-2.1.5/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.1.5/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.1.5/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-27 17:39:10.717709 shareddata-2.1.5/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.713709 shareddata-2.1.5/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1515 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4738 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1232 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11268 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.1.5/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5061 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SeriesLib.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5759 2023-07-18 17:51:31.000000 shareddata-2.1.5/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.1.5/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SharedDataAWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1817 2023-07-27 16:58:00.000000 shareddata-2.1.5/src/SharedData/SharedDataFeeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10857 2023-06-25 15:34:09.000000 shareddata-2.1.5/src/SharedData/SharedDataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15118 2023-07-27 17:37:34.000000 shareddata-2.1.5/src/SharedData/SharedDataPeriod.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3399 2023-07-22 06:17:01.000000 shareddata-2.1.5/src/SharedData/SharedDataRealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2468 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28760 2023-07-27 08:45:10.000000 shareddata-2.1.5/src/SharedData/SharedDataTable.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8776 2023-07-08 20:02:34.000000 shareddata-2.1.5/src/SharedData/SharedDataTableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.1.5/src/SharedData/SharedDataTableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    21375 2023-07-27 17:31:32.000000 shareddata-2.1.5/src/SharedData/SharedDataTimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.1.5/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-18 16:46:01.000000 shareddata-2.1.5/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.1.5/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-27 17:39:10.717709 shareddata-2.1.5/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      928 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-27 17:39:10.000000 shareddata-2.1.5/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:19:43.032148 shareddata-2.2.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 11:19:43.032148 shareddata-2.2.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.028148 shareddata-2.2.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.0/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.0/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.0/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.0/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1358 2023-07-29 20:08:45.000000 shareddata-2.2.0/src/SharedData/Feeder.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.0/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1222 2023-07-29 20:09:03.000000 shareddata-2.2.0/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11258 2023-07-29 20:08:46.000000 shareddata-2.2.0/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.0/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15066 2023-07-29 20:08:40.000000 shareddata-2.2.0/src/SharedData/Period.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.0/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2458 2023-07-29 20:09:00.000000 shareddata-2.2.0/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.0/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.2.0/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.0/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8626 2023-07-29 20:38:54.000000 shareddata-2.2.0/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.0/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.0/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16353 2023-07-31 11:18:41.000000 shareddata-2.2.0/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.0/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.0/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:19:43.032148 shareddata-2.2.0/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 11:19:43.000000 shareddata-2.2.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.1.5/LICENSE` & `shareddata-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/PKG-INFO` & `shareddata-2.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.5
+Version: 2.2.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.5/README.md` & `shareddata-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/setup.cfg` & `shareddata-2.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.1.5
+version = 2.2.0
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.1.5/src/SharedData/Defaults.py` & `shareddata-2.2.0/src/SharedData/Defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 if not 'PYTHONHASHSEED' in os.environ:
     raise Exception('PYTHONHASHSEED must be set to 0 in the environment!')
 else:
     if os.environ['PYTHONHASHSEED']!='0':
         raise Exception('PYTHONHASHSEED must be set to 0 in the environment!')
 
 if not 'DATABASE_FOLDER' in os.environ:    
-    os.environ['DATABASE_FOLDER'] = os.path.expanduser("~")+'\DB' 
+    os.environ['DATABASE_FOLDER'] = os.path.expanduser("~")+'/db'
 
 if not 'S3_BUCKET' in os.environ:    
     os.environ['S3_BUCKET'] = 's3://deepportfolio'
 
 if not 'S3_AWS_PROFILE' in os.environ:
     os.environ['S3_AWS_PROFILE'] = os.environ['AWS_PROFILE']
```

### Comparing `shareddata-2.1.5/src/SharedData/Logger.py` & `shareddata-2.2.0/src/SharedData/Logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,26 @@
 from pathlib import Path
 from datetime import datetime, timedelta
 import glob
 import pandas as pd
 from pythonjsonlogger.jsonlogger import JsonFormatter
 import boto3
 
-from importlib.metadata import version
-
-import SharedData.Defaults as Defaults 
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamHandler
 
+from SharedData.AWSKinesis import KinesisLogStreamHandler
 
 class Logger:
 
     log = None
-    user = None
+    user = 'guest'
+    source = 'unknown'
 
-    def __init__(self, source, user=None):
-        if Logger.log is None:                                
+    @staticmethod
+    def connect(source,user=None):
+        if Logger.log is None:
             if 'SOURCE_FOLDER' in os.environ:
                 try:
                     commompath = os.path.commonpath([source,os.environ['SOURCE_FOLDER']])
                     source = source.replace(commompath,'')
                 except:
                     pass
             elif 'USERPROFILE' in os.environ:
@@ -38,21 +37,18 @@
             if finds in source:
                 cutid = source.find(finds) + len(finds) + 1
                 source = source[cutid:]            
             source = source.replace('Windows\\system32\\','')
             source = source.lstrip('src').lstrip('\\src')
             source = source.lstrip('\\').lstrip('/')        
             source = source.replace('.py','')
-            self.source = source
+            Logger.source = source
             
             if not user is None:                
                 Logger.user = user
-            else:
-                user = 'guest'
-                Logger.user = 'guest'
                         
             path = Path(os.environ['DATABASE_FOLDER'])
             path = path / 'Logs'
             path = path / datetime.now().strftime('%Y%m%d')
             path = path / (os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'])        
             path = path / (source+'.log')
             if not path.parents[0].is_dir():
@@ -64,45 +60,40 @@
                     loglevel = logging.DEBUG
                 elif os.environ['LOG_LEVEL']=='INFO':
                     loglevel = logging.INFO   
             else:
                 loglevel = logging.INFO
 
             # Create Logger
-            self.log = logging.getLogger(source)
-            self.log.setLevel(logging.DEBUG)    
+            Logger.log = logging.getLogger(source)
+            Logger.log.setLevel(logging.DEBUG)    
             formatter = logging.Formatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
                 ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
                 datefmt='%Y-%m-%dT%H:%M:%S%z')
             #log screen
             handler = logging.StreamHandler()
             handler.setLevel(loglevel)    
             handler.setFormatter(formatter)
-            self.log.addHandler(handler)
-            #log file        
-            fhandler = logging.FileHandler(os.environ['LOG_PATH'], mode='a')
-            fhandler.setLevel(loglevel)    
-            fhandler.setFormatter(formatter)
-            self.log.addHandler(fhandler)
+            Logger.log.addHandler(handler)
+            # #log file        
+            # fhandler = logging.FileHandler(os.environ['LOG_PATH'], mode='a')
+            # fhandler.setLevel(loglevel)    
+            # fhandler.setFormatter(formatter)
+            # Logger.log.addHandler(fhandler)
             #log to aws kinesis
             kinesishandler = KinesisLogStreamHandler(user=Logger.user)
             kinesishandler.setLevel(logging.DEBUG)
             jsonformatter = JsonFormatter(os.environ['USERNAME']+'@'+os.environ['COMPUTERNAME'] + 
                 ';%(asctime)s;%(name)s;%(levelname)s;%(message)s',\
                 datefmt='%Y-%m-%dT%H:%M:%S%z')
             kinesishandler.setFormatter(jsonformatter)
-            self.log.addHandler(kinesishandler)
-            #assign static variable log to be used by modules
-            Logger.log = self.log
-            try:
-                Logger.log.debug('Logger initialized shareddata user %s version %s!' % \
-                    (Logger.user,version('SharedData')))
-            except:
-                Logger.log.debug('Logger initialized shareddata!')
+            Logger.log.addHandler(kinesishandler)            
+            
         
+    @staticmethod
     def readLogs(self):    
         logsdir = Path(os.environ['LOG_PATH']).parents[0]
         lenlogsdir = len(str(logsdir))
         files = glob.glob(str(logsdir) + "/**/*.log", recursive = True)   
         df = pd.DataFrame()
         # f=files[0]
         for f in files:
```

### Comparing `shareddata-2.1.5/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.2.0/src/SharedData/LoggerConsumerProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import numpy as np
 
 from SharedData.Logger import Logger
 logger = Logger(__file__,user='worker')
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer
+from SharedData.AWSKinesis import KinesisLogStreamConsumer
 
 SLEEP_TIME = 2
 
 def run():
     Logger.log.info('Starting SharedDataLogsConsumer process')
     consumer = KinesisLogStreamConsumer(user='worker')
```

### Comparing `shareddata-2.1.5/src/SharedData/Metadata.py` & `shareddata-2.2.0/src/SharedData/Metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import time
 import subprocess
 from datetime import datetime, timedelta
 import gzip,io,shutil,hashlib
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import S3Upload, S3ListFolder, S3Download, UpdateModTime
+from SharedData.AWSS3 import S3Upload, S3ListFolder, S3Download, UpdateModTime
 
 class Metadata():
     
     def __init__(self, name, mode='rw', user='master'):
         
         if Logger.log is None:
             Logger('Metadata')
```

### Comparing `shareddata-2.1.5/src/SharedData/MultiProc.py` & `shareddata-2.2.0/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/SharedData/SharedData.py` & `shareddata-2.2.0/src/SharedData/SharedData.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,116 @@
 import os, psutil
 import pandas as pd
 from multiprocessing import shared_memory
 from pathlib import Path
+from importlib.metadata import version
 
+import SharedData.Defaults as Defaults 
 from SharedData.Logger import Logger
-from SharedData.SharedDataFeeder import SharedDataFeeder
-from SharedData.Metadata import Metadata
-from SharedData.SharedDataRealTime import SharedDataRealTime
+from SharedData.Table import Table
+from SharedData.TimeseriesContainer import TimeseriesContainer
+from SharedData.TimeSeries import TimeSeries
+from SharedData.DataFrame import SharedDataFrame
+from SharedData.RealTime import SharedDataRealTime
 from SharedData.Utils import remove_shm_from_resource_tracker
 
-
-class SharedData:
-
-    INIT_MESSAGE_SENT = False
-    PERSIST_SHARED_MEMORY = True
-
-    def __init__(self, database, mode='rw', user='master'):
-
-        if Logger.log is None:
-            Logger('SharedData')
-
-        if (os.name == 'posix') & (SharedData.PERSIST_SHARED_MEMORY):
-            remove_shm_from_resource_tracker()
-
-        self.database = database
+class SharedData:    
+    
+    def __init__(self,source,user='guest'):
+        self.source = source
         self.user = user
 
-        self.s3read = False
-        self.s3write = False
-        if mode == 'r':
-            self.s3read = True
-            self.s3write = False
-        elif mode == 'w':
-            self.s3read = False
-            self.s3write = True
-        elif mode == 'rw':
-            self.s3read = True
-            self.s3write = True
-
-        if (Logger.user != 'master') & (user == 'master'):
-            self.s3write = False
-            mode = 'r'
-
-        self.save_local = (os.environ['SAVE_LOCAL'] == 'True')
-
-        self.mode = mode
-
-        # DATA DICTIONARY
-        # SharedDataTimeSeries: data[feeder][period][tag] (date x symbols)
-        # SharedDataFrame: data[feeder][period][date] (symbols x tags)
+        # DATA DICTIONARY        
         self.data = {}
+        
+        # LOGIN VARIABLES
+        self.islogged = False
+        self.source=source
+        self.user=user
+        self.mode='rw'
+
+        # S3 VARIABLES
+        self.s3read = True
+        self.s3write = True
 
-        # Symbols collections metadata
-        self.metadata = {}
+        # save files locally
+        self.save_local = (os.environ['SAVE_LOCAL'] == 'True')
 
-        # static metadata
-        self.static = pd.DataFrame([])
+        self.databases = {
+            'MarketData' : ['date','symbol'],
+            'Relationships' : ['date','symbol1','symbol2'],
+            'Portfolios' : ['date','portfolio'],
+            'Signals' : ['date','portfolio','symbol'],
+            'Risk' : ['date','portfolio','symbol'],
+            'Positions' : ['date','portfolio','symbol'],
+            'Orders' : ['date','portfolio','symbol','clordid'],
+            'Trades' : ['date','portfolio','symbol','tradeid']
+        }
+        
+        Logger.connect(self.source,self.user)
 
-        if not SharedData.INIT_MESSAGE_SENT:
-            SharedData.INIT_MESSAGE_SENT = True
-            Logger.log.debug('Initializing SharedData %s:%s DONE!' %
-                (os.environ['USERNAME'], os.environ['COMPUTERNAME']))
-
-    def __setitem__(self, feeder, value):
-        self.data[feeder] = value
-
-    def __getitem__(self, feeder):
-        if not feeder in self.data.keys():
-            self.data[feeder] = SharedDataFeeder(self, feeder)
-        return self.data[feeder]
+        if (os.name == 'posix'):
+            remove_shm_from_resource_tracker()        
+    
+        if not self.islogged:
+            self.islogged = True
+            try:
+                Logger.log.debug('%s@%s CONNECTED!\nSharedData version %s, user %s' %
+                    (os.environ['USERNAME'], os.environ['COMPUTERNAME'],version('SharedData'), self.user))
+            except:
+                Logger.log.debug('%s:%s CONNECTED!\nSharedData user %s!' %
+                    (os.environ['USERNAME'], os.environ['COMPUTERNAME'],self.user))
+            
+    ###############################################
+    ############# DATA CONTAINERS #################
+    ###############################################
+
+    ############# TABLE #################
+    def table(self,database,period,source,tablename,\
+        names=None,formats=None,size=None,value=None,user='master'):
+
+        path = user+'/'+database+'/'+period+'/'+source+'/table/'+tablename
+        if not path in self.data.keys():
+            self.data[path] = Table(self,database,period,source,\
+                tablename,records=value,names=names,formats=formats,size=size,user=user)
+        return self.data[path].records
     
-    def malloc(self,shm_name,create=False,size=None,overwrite=False,):
+    ############# TIMESERIES #################
+    def timeseries(self,database,period,source,tag=None,\
+        startDate=None,columns=None,value=None,user='master'):
+        
+        path = user+'/'+database+'/'+period+'/'+source+'/timeseries'
+        if not path in self.data.keys():
+            self.data[path] = TimeseriesContainer(self, database, period, source,user=user)
+        if tag is None:
+            return self.data[path]
+        
+        if not tag in self.data[path].tags.keys():
+            if (startDate is None) & (columns is None) & (value is None):
+                self.data[path].load()
+                if not tag in self.data[path].tags.keys():
+                    Logger.log.error('Tag %s/%s doesnt exist' % (path,tag))
+                    return None
+            else:
+                self.data[path].tags[tag] = TimeSeries(self, self.data[path],\
+                    database, period, source, tag,\
+                    value=value,startDate=startDate,columns=columns,user=user)
+                            
+        return self.data[path].tags[tag].data
+            
+    ############# DATAFRAME #################
+    def dataframe(self,database,period,source,\
+        date=None,value=None,user='master'):
+        pass
+
+    ###############################################
+    ######### SHARED MEMORY MANAGEMENT ############
+    ###############################################    
+    @staticmethod
+    def malloc(shm_name,create=False,size=None,overwrite=False):
         ismalloc = False
         shm = None        
         try:
             shm = shared_memory.SharedMemory(\
                 name = shm_name,create=False)
             ismalloc = True
         except:
@@ -86,15 +122,15 @@
             ismalloc = True
         
         elif (create) & (size is None):
             raise Exception('SharedData malloc must have a size when create=True')
         
         elif (os.name=='posix')\
             & (ismalloc) & (create) & (overwrite) & (not size is None):
-            self.free(shm_name)        
+            SharedData.free(shm_name)
             shm = shared_memory.SharedMemory(\
                 name=shm_name,create=True,size=size)
             ismalloc = True            
         
         # register process id access to memory
         if ismalloc:            
             fpath = Path(os.environ['DATABASE_FOLDER'])
@@ -104,28 +140,14 @@
             f = open(fpath, "a+")
             f.write(str(pid)+',')
             f.flush()
             f.close()
 
         return [shm, ismalloc]
     
-    def free(self,shm_name):
-        if os.name=='posix':
-            try:
-                shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=False)
-                shm.close()
-                shm.unlink()
-                fpath = Path(os.environ['DATABASE_FOLDER'])
-                fpath = fpath/('shm/'+shm_name.replace('\\','/')+'.csv')
-                if fpath.is_file():
-                    os.remove(fpath)
-            except:
-                pass
-
     @staticmethod
     def free(shm_name):
         if os.name=='posix':
             try:
                 shm = shared_memory.SharedMemory(\
                     name = shm_name,create=False)
                 shm.close()
@@ -164,9 +186,12 @@
     
     @staticmethod
     def freeall():
         shm_names = SharedData.list()
         for shm_name in shm_names.index:
             SharedData.free(shm_name)
     
-    def subscriberealtime(self):
-        SharedDataRealTime.subscribe(self)
+    ###############################################
+    ############# REAL TIME MANAGEMENT ############
+    ###############################################
+    def subscribe(database,source,period):
+        SharedDataRealTime.subscribe(database,source,period)
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.2.0/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.2.0/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataFeeder.py` & `shareddata-2.2.0/src/SharedData/Feeder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from SharedData.SharedDataPeriod import SharedDataPeriod
-from SharedData.SharedDataTable import SharedDataTable
+from SharedData.Period import SharedDataPeriod
+from SharedData.Table import SharedDataTable
 
 class SharedDataFeeder():
 
     dense_datasets = {'W1':'weekly','D1':'daily','M15':'15 min','M1':'1 min'}
     
     def __init__(self, sharedData, feeder):
         self.feeder = feeder
@@ -20,28 +20,18 @@
                 period = dataset
                 self.data[period] = value
             else:
                 self.data[dataset] = SharedDataTable(self, dataset, value)            
         return self.data[dataset]
                 
     def __getitem__(self, dataset):
-        if not dataset in self.data.keys():            
+        if not dataset in self.data.keys():
             if (dataset in SharedDataFeeder.dense_datasets.keys()):                
                 period = dataset
                 self.data[period] = SharedDataPeriod(self, period)
             else:
                 self.data[dataset] = SharedDataTable(self, dataset)
 
         if (dataset in SharedDataFeeder.dense_datasets.keys()):
             return self.data[dataset]
         else:
-            return self.data[dataset].records
-    
-    def create_table(self,dataset,names,formats,size,overwrite=False):
-        self.data[dataset] = SharedDataTable(\
-            self,dataset,names=names,formats=formats,size=size,\
-                overwrite=overwrite)
-        return self.data[dataset].records
-    
-    def load_table(self,dataset,size=None):
-        self.data[dataset] = SharedDataTable(self,dataset,size=size)
-        return self.data[dataset].records
+            return self.data[dataset].records
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataFrame.py` & `shareddata-2.2.0/src/SharedData/DataFrame.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from pandas.tseries.offsets import BDay
 from pathlib import Path
 from multiprocessing import shared_memory
 from datetime import datetime, timedelta
 
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import S3Download,S3Upload,UpdateModTime
-from SharedData.SharedDataRealTime import SharedDataRealTime
+from SharedData.AWSS3 import S3Download,S3Upload,UpdateModTime
+from SharedData.RealTime import SharedDataRealTime
 
 
 class SharedDataFrame:
 
     def __init__(self, sharedDataPeriod, tag, df=None):        
         self.sharedDataPeriod = sharedDataPeriod
         self.tag = tag
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataPeriod.py` & `shareddata-2.2.0/src/SharedData/Period.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 from pathlib import Path
 from pandas.tseries.offsets import BDay
 from threading import Thread
 
-
 from SharedData.Logger import Logger
-from SharedData.SharedDataFrame import SharedDataFrame
-from SharedData.SharedDataTimeSeries import SharedDataTimeSeries
-from SharedData.SharedDataAWSS3 import S3Upload,S3Download,UpdateModTime
+from SharedData.DataFrame import SharedDataFrame
+from SharedData.TimeSeries import SharedDataTimeSeries
+from SharedData.AWSS3 import S3Upload,S3Download,UpdateModTime
 
 class SharedDataPeriod:
 
     def __init__(self, sharedDataFeeder, period):
         self.sharedDataFeeder = sharedDataFeeder        
         self.sharedData = sharedDataFeeder.sharedData        
         self.period = period
@@ -37,38 +36,27 @@
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M1':
             self.periodSeconds = 60
             self.default_startDate = pd.Timestamp('2010-01-01')
         self.getContinousTimeIndex(self.default_startDate)
         self.loaded = False
 
-    def load(self):
-        # read if not loaded
-        shdatalist = self.sharedData.list()   
-        path, shm_name = self.get_path()
-        idx = [shm_name in str(s) for s in shdatalist.index]
-        if not np.any(idx):
-            self.read()
-        else:
-            #map
-            self.map(shm_name,shdatalist.index[idx])
-
     def __setitem__(self, tag, df):
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 self.tags[tag] = SharedDataFrame(self, tag, df)
             else:
                 self.tags[tag] = SharedDataTimeSeries(self, tag, df)
         elif isinstance(df, pd.DataFrame):
             data = self.tags[tag].data
             iidx = df.index.intersection(data.index)
             icol = df.columns.intersection(data.columns)
             data.loc[iidx, icol] = df.loc[iidx, icol].copy()
 
-    def __getitem__(self, tag):     
+    def __getitem__(self, tag):
         if not self.loaded:
             self.load()
             self.loaded=True
         if not tag in self.tags.keys():
             if isinstance(tag, pd.Timestamp):
                 df = SharedDataFrame(self, tag)
                 if not df.data.empty:
@@ -146,20 +134,30 @@
     #CREATE
     def create_timeseries(self,tag,startDate,columns,overwrite=False):
         self.tags[tag] = SharedDataTimeSeries(\
             self,tag,startDate=startDate,columns=columns,overwrite=overwrite)
         return self.tags[tag].data
 
     # READ
+    def load(self):
+        # read if not loaded
+        shdatalist = self.sharedData.list()   
+        path, shm_name = self.get_path()
+        idx = [shm_name in str(s) for s in shdatalist.index]
+        if not np.any(idx):
+            self.read()
+        else:
+            #map
+            self.map(shm_name,shdatalist.index[idx])
+
     def map(self,shm_name,shm_name_list):
         for shm in shm_name_list:
             tag = shm.replace(shm_name,'')[1:]
             self.tags[tag] = SharedDataTimeSeries(self, tag = tag)            
 
-
     def read(self):
         tini = time.time()
         datasize = 1
         path, shm_name= self.get_path()
         headpath = str(path)+'_head.bin'
         tailpath = str(path)+'_tail.bin'        
         head_io = None
@@ -215,16 +213,16 @@
         #read
         io_obj.seek(0)
         io_data = io_obj.read()
         datasize = len(io_data)
         _m = hashlib.md5(io_data[:-24]).digest()
         m = io_data[-16:]
         if (m!=_m):
-            Logger.log.error('Timeseries read_head() file %s corrupted!' % (path))
-            raise Exception('Timeseries read_head() %s corrupted!' % (path))
+            Logger.log.error('Timeseries file %s corrupted!' % (path))
+            raise Exception('Timeseries file %s corrupted!' % (path))
         io_obj.seek(0)
         separator = np.frombuffer(io_obj.read(8),dtype=np.int64)[0]        
         while (separator==1):
             _header = np.frombuffer(io_obj.read(40),dtype=np.int64)
             _tag_b = io_obj.read(int(_header[0]))
             _tag = _tag_b.decode(encoding='UTF-8',errors='ignore')
             _idx_b = io_obj.read(int(_header[1]))
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataRealTime.py` & `shareddata-2.2.0/src/SharedData/RealTime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os,boto3,time,subprocess,sys
 import pandas as pd
 import numpy as np
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSKinesis import KinesisStreamProducer
+from SharedData.AWSKinesis import KinesisStreamProducer
 
 class SharedDataRealTime:
 
     # producer dictionary
     producer = {}
 
     def broadcast(shdata,feeder,period,tag,idx,col):
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.2.0/src/SharedData/RealTimeProcess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 import numpy as np
 from pathlib import Path
 
 from SharedData.Logger import Logger
 logger = Logger(__file__)
 from SharedData.SharedData import SharedData
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer
+from SharedData.AWSKinesis import KinesisStreamConsumer
 
 
 try:
     if len(sys.argv)>=2:
         DATABASE = str(sys.argv[1])
     else:
         DATABASE = 'MarketData'
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataTable.py` & `shareddata-2.2.0/src/SharedData/Table.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,33 +6,35 @@
 import time
 from multiprocessing import shared_memory
 import gzip,io,hashlib
 from datetime import datetime
 from tqdm import tqdm
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import S3Upload,S3Download,UpdateModTime
-from SharedData.SharedDataTableIndex import SharedDataTableIndex
+from SharedData.AWSS3 import S3Upload,S3Download,UpdateModTime
+from SharedData.TableIndex import TableIndex
 from SharedData.SharedNumpy import SharedNumpy
 
 if os.name == 'posix':
     from SharedData.Utils  import cpp
 
-class SharedDataTable:
+class Table:
 
-    def __init__(self, sharedDataFeeder, dataset, records=None,\
-                 names=None,formats=None,size=None,overwrite=False):
-        self.sharedDataFeeder = sharedDataFeeder
-        self.sharedData = self.sharedDataFeeder.sharedData
-        self.feeder = self.sharedDataFeeder.feeder
-        self.dataset = dataset
+    def __init__(self, shareddata, database, period, source, tablename,\
+          records=None,names=None,formats=None,size=None,overwrite=False,user='master'):
+        self.shareddata = shareddata
+        self.user = user
+        self.database = database
+        self.period = period        
+        self.source = source
+        self.tablename = tablename
         if os.name != 'posix':
             overwrite = False
         
-        self.keys = SharedDataTableIndex(self)
+        self.keys = TableIndex(self)
         
         self.init_time = time.time()
         self.download_time = pd.NaT
                         
         # file partitioning threshold
         self.maxtailbytes = int(100*10**6)
         
@@ -67,51 +69,70 @@
             self.create_map = 'map'
         else:
             self.create_map = 'create'
 
         # initalize
         try:
             if ((self.create_map == 'create') | (overwrite)):
-                if (not names is None):
-                    # create new empty shared memory
+                if (not names is None) & (records is None):
+                    # create new shared memory empty 
                     self.create(names,formats,size)
 
                 elif (not records is None):
-                    # allocate existing data
+                    # create new shared memory set value
                     if isinstance(records,pd.DataFrame):
                         records = self.df2records(records)
                     descr = records.__array_interface__['descr']
                     names = [item[0] for item in descr]
                     formats = [item[1] for item in descr]
                     size = int(records.size*1.25)
                     self.create(names,formats,size)
                     self.records.insert(records)
 
                 elif (records is None):
-                    # read & allocate data
+                    # create new shared memory read value
                     tini = time.time()            
                     self.read(size)
                     te = time.time()-tini+0.000001
                     datasize = self.hdr['count']*self.hdr['itemsize']/1000000
                     Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-                        (self.feeder,self.dataset,datasize,te,datasize/te))
+                        (self.source,self.tablename,datasize,te,datasize/te))
                     
             elif (self.create_map == 'map'):
                 # map existing shared memory
                 self.malloc_map()
         except Exception as e:
             path, shm_name = self.get_path()
             Logger.log.error('Error initalizing %s!\n%s' % (shm_name,e))
             self.free()
 
         self.init_time = time.time() - self.init_time
-            
+        
+    def get_path(self):
+        shm_name = self.user + '/' + self.database + '/' \
+            + self.period + '/' + self.source + '/table/' + self.tablename
+        if os.name=='posix':
+            shm_name = shm_name.replace('/','\\')
+        
+        path = Path(os.environ['DATABASE_FOLDER'])
+        path = path / self.user
+        path = path / self.database
+        path = path / self.period
+        path = path / self.source
+        path = path / 'table'
+        path = path / self.tablename
+        path = Path(str(path).replace('\\','/'))
+        if self.shareddata.save_local:
+            os.makedirs(path,exist_ok=True)
+
+        return path, shm_name
+                
     def ismalloc(self):
         path, shm_name = self.get_path()
-        [self.shm, ismalloc] = self.sharedData.malloc(shm_name)
+        [self.shm, ismalloc] = self.shareddata.malloc(shm_name)
         return ismalloc
 
     def create(self, names, formats, size):        
         path, shm_name = self.get_path()
         #TODO: WRITE FILE WITH POINTER TO SHARED DATA TO KEEP TRACK OF OPENED MEMORY
         check_pkey = True
         npkeys = len(self.keys.pkeycolumns)
@@ -162,15 +183,15 @@
         nb_hdr = self.hdrdtype.itemsize # number of header bytes        
         nb_records = int(self.hdr['recordssize']*self.hdr['itemsize']) #number of data bytes
         total_size = int(nb_hdr+nb_records)
 
         # if in linux check if data exists and dispose it
         # doesnt work in windows
         [self.shm, ismalloc] = \
-            self.sharedData.malloc(shm_name,create=True,size=total_size,overwrite=True)
+            self.shareddata.malloc(shm_name,create=True,size=total_size,overwrite=True)
         if not ismalloc:
             raise Exception('Could not allocate shared memory!')
 
         # allocate header
         self.hdr['semaphore']=1 # lock semaphore memory
         self.shm.buf[0:nb_hdr] = self.hdr.tobytes()
         self.hdr = np.ndarray((1,),dtype=self.hdrdtype,buffer=self.shm.buf)[0]
@@ -203,32 +224,32 @@
         tail_io_remote_isnewer = False
         headpath = path / 'head.bin'
         tailpath = path / 'tail.bin'
         unzip_head = False
 
         # open head_io to read header
         # download remote head if its newer than local
-        if self.sharedData.s3read:
-            force_download= (not self.sharedData.save_local)     
+        if self.shareddata.s3read:
+            force_download= (not self.shareddata.save_local)     
             tini = time.time()
             [head_io_gzip, head_local_mtime, head_remote_mtime] = \
                 S3Download(str(headpath),str(headpath)+'.gzip',force_download)            
             if not head_io_gzip is None:
                 te = time.time()-tini+0.000001
                 datasize = head_io_gzip.getbuffer().nbytes/1000000
                 Logger.log.debug('download head %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-                    (self.feeder,self.dataset,datasize,te,datasize/te))
+                    (self.source,self.tablename,datasize,te,datasize/te))
                 
                 head_io_remote_isnewer = True
                 head_io_gzip.seek(0)
                 head_io = gzip.GzipFile(fileobj=head_io_gzip, mode='rb')                
                 unzip_head = True
                 
         # open head_io to read header
-        if self.sharedData.save_local:
+        if self.shareddata.save_local:
             if head_io is None:
                 if headpath.exists():
                     head_io = open(headpath, 'rb')
 
         # read header
         if not head_io is None:
             head_io.seek(0)
@@ -242,30 +263,30 @@
             nb_hdr = self.hdrdtype.itemsize            
             head_io.seek(0)
             self.hdr = np.ndarray((1,),dtype=self.hdrdtype,\
                 buffer=head_io.read(nb_hdr))[0]
             self.hdr = self.hdr.copy()
             self.hdr['semaphore']=1
             
-            if self.sharedData.s3read:
+            if self.shareddata.s3read:
                 if self.hdr['hastail']==1:
                     tini = time.time()
                     [tail_io_gzip, tail_local_mtime, tail_remote_mtime] = \
                         S3Download(str(tailpath),str(tailpath)+'.gzip',force_download)
                     if not tail_io_gzip is None:
                         te = time.time()-tini+0.000001
                         datasize = tail_io_gzip.getbuffer().nbytes/1000000
                         Logger.log.debug('download tail %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-                            (self.feeder,self.dataset,datasize,te,datasize/te))
+                            (self.source,self.tablename,datasize,te,datasize/te))
                         
                         tail_io_remote_isnewer = True
                         tail_io_gzip.seek(0)                        
                         tail_io = gzip.GzipFile(fileobj=tail_io_gzip, mode='rb')
              
-            if self.sharedData.save_local:
+            if self.shareddata.save_local:
                 if self.hdr['hastail']==1:
                     if tail_io is None:                    
                         if tailpath.exists():
                             tail_io = open(tailpath, 'rb')
 
             # read tail header if exists
             if not tail_io is None:
@@ -299,17 +320,17 @@
             self.shm.buf[0:nb_hdr] = head_io.read(nb_hdr)
             self.hdr['semaphore'] = 1 # force acquire
             
             nb_head = int(self.hdr['headsize']*self.hdr['itemsize'])
             nb_head_mb = nb_head / (1024*1024)
         
             if unzip_head:
-                message = 'Unzipping:%iMB %s/%s' % (nb_head_mb,self.feeder,self.dataset)
+                message = 'Unzipping:%iMB %s/%s' % (nb_head_mb,self.source,self.tablename)
             else:
-                message = 'Reading:%iMB %s/%s' % (nb_head_mb,self.feeder,self.dataset)
+                message = 'Reading:%iMB %s/%s' % (nb_head_mb,self.source,self.tablename)
             block_size = 100 * 1024 * 1024 # or any other block size that you prefer
             # Use a with block to manage the progress bar
             with tqdm(total=nb_head, unit='B',unit_scale=True, desc=message) as pbar:
                 read_bytes = 0
                 # Loop until we have read all the data
                 while read_bytes < nb_head:
                     # Read a block of data
@@ -335,15 +356,15 @@
             self.hdr['recordssize'] = int(self.hdr['count']*1.25) # add 25% space for growth
             
             # check if data is corrupted            
             self.hdr['md5hash'] = 0
             nb_records = self.hdr['count']*self.hdr['itemsize']
             nb_records_mb = nb_records / (1024*1024)
         
-            message = 'Verifying:%iMB %s/%s' % (nb_records_mb,self.feeder,self.dataset)
+            message = 'Verifying:%iMB %s/%s' % (nb_records_mb,self.source,self.tablename)
             block_size = 100 * 1024 * 1024 # or any other block size that you prefer
             nb_total = nb_hdr+nb_records
             read_bytes = nb_hdr
             m = hashlib.md5()                
             # Use a with block to manage the progress bar
             with tqdm(total=nb_total, unit='B',unit_scale=True, desc=message) as pbar:                    
                 # Loop until we have read all the data                    
@@ -359,15 +380,15 @@
             if md5hash != m.digest():
                 Logger.log.error('File corrupted %s!' % (path))
                 raise Exception('File corrupted %s!' % (path))
             
             self.hdr['md5hash'] = md5hash
             self.release()
 
-        if self.sharedData.save_local:
+        if self.shareddata.save_local:
             if (head_io_remote_isnewer) | (tail_io_remote_isnewer):
                 self.acquire()
                 try:
                     # create header                
                     [write_head,nb_header,nb_head,nb_tail] = self.fill_header(md5hash)
                     # save local
                     if (head_io_remote_isnewer) | (write_head):
@@ -409,32 +430,32 @@
 
             tini = time.time()
             # create header
             mtime = self.hdr['mtime']
             [write_head,nb_header,nb_head,nb_tail] = self.fill_header()
             
             # TODO: split threads write local and remote
-            if self.sharedData.s3write:
+            if self.shareddata.s3write:
                 if write_head:
                     self.upload_head(path,nb_header,nb_head,mtime)
 
                 if self.hdr['hastail']==1:        
                     self.upload_tail(path,nb_header,nb_head,nb_tail,mtime)        
                     
-            if self.sharedData.save_local:
+            if self.shareddata.save_local:
                 if write_head:
                     self.write_head(path,nb_header,nb_head,mtime)
                 
                 if self.hdr['hastail']==1:
                     self.write_tail(path,nb_header,nb_head,nb_tail,mtime)
 
             te = time.time()-tini
             datasize = self.hdr['count']*self.hdr['itemsize']/1000000
             Logger.log.debug('write %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-                (self.feeder,self.dataset,datasize,te,datasize/te))
+                (self.source,self.tablename,datasize,te,datasize/te))
         except Exception as e:
             Logger.log.error('Could not write %s\n%s!' % (path,e))
             self.release()
             return False
         
         self.release()
         return True
@@ -477,15 +498,15 @@
     def upload_head(self,path,nb_header,nb_head,mtime):
         # zip head
         gzip_io = io.BytesIO()
         with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
             gz.write(self.shm.buf[0:nb_header])
             headsize_mb = nb_head / (1000000)
             blocksize = 1024*1024*100
-            descr = 'Zipping:%iMB %s/%s' % (headsize_mb,self.feeder,self.dataset)
+            descr = 'Zipping:%iMB %s/%s' % (headsize_mb,self.source,self.tablename)
             with tqdm(total=headsize_mb, unit='B', unit_scale=True, desc=descr) as pbar:
                 written = 0
                 while written < nb_head:
                     chunk_size = min(blocksize, nb_head-written) # write in chunks of max 100 MB size
                     gz.write(self.shm.buf[nb_header+written:nb_header+written+chunk_size])
                     written += chunk_size
                     pbar.update(chunk_size)
@@ -501,16 +522,16 @@
         S3Upload(gzip_io,path/'tail.bin.gzip',mtime)
 
     def write_head(self,path,nb_header,nb_head,mtime):
         with open(path/'head.bin', 'wb') as f:
             f.write(self.shm.buf[0:nb_header])
             headsize_mb = nb_head / (1000000)
             blocksize = 1024*1024*100
-            descr = 'Writing:%iMB %s/%s' % (headsize_mb,self.feeder,self.dataset)
-            with tqdm(total=headsize_mb, unit='B', unit_scale=True, desc=descr) as pbar:
+            descr = 'Writing:%iMB %s/%s' % (headsize_mb,self.source,self.tablename)
+            with tqdm(total=nb_head, unit='B', unit_scale=True, desc=descr) as pbar:
                 written = 0
                 while written < nb_head:
                     chunk_size = min(blocksize, nb_head-written) # write in chunks of max 100 MB size
                     f.write(self.shm.buf[nb_header+written:nb_header+written+chunk_size])                                                
                     written += chunk_size
                     pbar.update(chunk_size)
             
@@ -571,61 +592,43 @@
                     try:  
                         if col in df.columns:
                             rec[col] = df[col].astype(dtypes[col])
                     except Exception as e:
                         Logger.log.error('Could not convert %s!\n%s' % (col,e))
                 
                 return rec
-        
-    def get_path(self):
-        shm_name = self.sharedData.user + '/' + self.sharedData.database + '/' \
-            + self.sharedDataFeeder.feeder + '/' + self.dataset 
-        if os.name=='posix':
-            shm_name = shm_name.replace('/','\\')
-        
-        path = Path(os.environ['DATABASE_FOLDER'])
-        path = path / self.sharedData.user
-        path = path / self.sharedData.database
-        path = path / self.sharedDataFeeder.feeder
-        path = path / self.dataset        
-        path = Path(str(path).replace('\\','/'))
-        if self.sharedData.save_local:
-            os.makedirs(path,exist_ok=True)
-
-        return path, shm_name
     
     def acquire(self,timeout=60):
         if os.name == 'posix':
             # semaphore is process safe
             telapsed = 0
             tini = time.time()
             hdrptr = self.hdr.__array_interface__['data'][0]
             semseek = 258        
             while cpp.bool_compare_and_swap(hdrptr, semseek, 0, 1)==0:
                 telapsed = time.time() - tini
                 if telapsed>timeout:
                     raise TimeoutError('Timeout waiting for semaphore')
-                time.sleep(0.001)
+                time.sleep(0.0001)
         else:
             while self.hdr['semaphore']!=0:
                 telapsed = time.time() - tini
                 if telapsed>timeout:
                     raise TimeoutError('Timeout waiting for semaphore')
-                time.sleep(0.001)
+                time.sleep(0.0001)
             self.hdr['semaphore'] = 1
             
-
     def release(self):
         if os.name == 'posix':
             hdrptr = self.hdr.__array_interface__['data'][0]
             semseek = 258
             if cpp.bool_compare_and_swap(hdrptr, semseek, 1, 0)!=1:
                 raise Exception('Tried to release semaphore without acquire!')
         else:
             self.hdr['semaphore'] = 0
         
     def free(self):
         path, shm_name = self.get_path()            
-        self.sharedData.free(shm_name)
-        self.sharedData.free(shm_name+'#pkey')
-        self.sharedData.free(shm_name+'#dateidx')
-        self.sharedData.free(shm_name+'#portidx')
+        self.shareddata.free(shm_name)
+        self.shareddata.free(shm_name+'#pkey')
+        self.shareddata.free(shm_name+'#dateidx')
+        self.shareddata.free(shm_name+'#portidx')
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataTableIndex.py` & `shareddata-2.2.0/src/SharedData/TableIndex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import numpy as np
 import time
 from multiprocessing import shared_memory
 
-import SharedData.SharedDataTableIndexJit as SharedDataTableIndexJit
-from SharedData.SharedDataTableIndexJit import *
+import SharedData.TableIndexJit as TableIndexJit
+from SharedData.TableIndexJit import *
 
 
-class SharedDataTableIndex:
+class TableIndex:
 
     def __init__(self,table):
         self.table = table
-        self.sharedData = self.table.sharedData
+        self.shareddata = self.table.shareddata
         
         self.initialized = False
 
         # primary key hash table        
-        self.pkeycolumns = SharedDataTableIndex.get_pkeycolumns(self.sharedData.database)
+        self.pkeycolumns = TableIndex.get_pkeycolumns(self.table.database)
         self.pkeystr = '_'.join(self.pkeycolumns)
         self.pkey = np.ndarray([])
         # date index
         self.dateiniidx = np.ndarray([])
         self.dateendidx = np.ndarray([])
         # date,portfolio index
         self.portiniidx = np.ndarray([]) # hash table
@@ -38,36 +38,36 @@
         # primary key & index functions
         self.create_index_func = None
         self.upsert_func = None
         self.get_loc_func = None
         
 
         create_pkey_fname = 'create_pkey_'+ self.pkeystr + '_jit'
-        if hasattr(SharedDataTableIndexJit,create_pkey_fname):
-            self.create_index_func = getattr(SharedDataTableIndexJit,create_pkey_fname)
+        if hasattr(TableIndexJit,create_pkey_fname):
+            self.create_index_func = getattr(TableIndexJit,create_pkey_fname)
         else:
             raise Exception('create_pkey function not found for database %s!' \
-                % (self.sharedData.database))
+                % (self.table.database))
 
         upsert_fname = 'upsert_'+ self.pkeystr + '_jit'
-        if hasattr(SharedDataTableIndexJit,upsert_fname):
-            self.upsert_func = getattr(SharedDataTableIndexJit,upsert_fname)
+        if hasattr(TableIndexJit,upsert_fname):
+            self.upsert_func = getattr(TableIndexJit,upsert_fname)
         else:
             raise Exception('upsert function not found for database %s!' \
-                % (self.sharedData.database))
+                % (self.table.database))
 
         get_loc_fname = 'get_loc_'+ self.pkeystr + '_jit'
-        if hasattr(SharedDataTableIndexJit,get_loc_fname):
-            self.get_loc_func = getattr(SharedDataTableIndexJit,get_loc_fname)
+        if hasattr(TableIndexJit,get_loc_fname):
+            self.get_loc_func = getattr(TableIndexJit,get_loc_fname)
         else:
             raise Exception('get_loc function not found for database %s!' \
-                % (self.sharedData.database))
+                % (self.table.database))
         
         if 'date_portfolio_' in self.pkeystr:
-            self.get_index_date_portfolio_func = getattr(SharedDataTableIndexJit,'get_index_date_portfolio_jit')
+            self.get_index_date_portfolio_func = getattr(TableIndexJit,'get_index_date_portfolio_jit')
     
     def malloc(self):
         path, shm_name = self.table.get_path()
         self.malloc_pkey(shm_name)
         if 'date' in self.pkeystr:
             self.malloc_dateidx(shm_name)
         if 'date_portfolio_' in self.pkeystr:
@@ -76,17 +76,17 @@
             self.create_index()
 
     def malloc_pkey(self,shm_name):        
         keysize = int(self.table.records.size*5)
         keysize_bytes = int(keysize * 4)
 
         iscreate = False
-        [self.pkeyshm, ismalloc] = self.sharedData.malloc(shm_name+'#pkey')
+        [self.pkeyshm, ismalloc] = self.shareddata.malloc(shm_name+'#pkey')
         if not ismalloc:
-            [self.pkeyshm, ismalloc] = self.sharedData.malloc(shm_name+'#pkey',\
+            [self.pkeyshm, ismalloc] = self.shareddata.malloc(shm_name+'#pkey',\
                 create=True,size=keysize_bytes)
             iscreate = True
 
         self.pkey = np.ndarray((keysize,),dtype=np.int32,buffer=self.pkeyshm.buf)
         if iscreate:
             self.pkey[:] = -1
                         
@@ -108,17 +108,17 @@
         elif dtunit=='ns':
             self.dateunit = 24*60*60*1000*1000*1000
         maxdate = np.datetime64('2070-01-01','D')
         dateidxsize = maxdate.astype(int)
         dateidxsize_bytes = int(dateidxsize * 4)
         
         iscreate = False        
-        [self.dateidxshm, ismalloc] = self.sharedData.malloc(shm_name+'#dateidx')
+        [self.dateidxshm, ismalloc] = self.shareddata.malloc(shm_name+'#dateidx')
         if not ismalloc:
-            [self.dateidxshm, ismalloc] = self.sharedData.malloc(shm_name+'#dateidx',\
+            [self.dateidxshm, ismalloc] = self.shareddata.malloc(shm_name+'#dateidx',\
                 create=True,size=int(dateidxsize_bytes*2))
             iscreate = True
             
         self.dateiniidx = np.ndarray((dateidxsize,),dtype=np.int32,buffer=self.dateidxshm.buf)        
         self.dateendidx = np.ndarray((dateidxsize,),dtype=np.int32,buffer=self.dateidxshm.buf,\
             offset=dateidxsize_bytes)
         
@@ -129,17 +129,17 @@
     def malloc_portfolioidx(self,shm_name):
         portlistsize = int(self.table.records.size*2)
         keysize = int(self.table.records.size*5)
         keysize_bytes = int(keysize * 4)
         portidxsize_bytes = 4 +  int(keysize_bytes*2) + int(portlistsize*4)
         
         iscreate = False
-        [self.portidxshm, ismalloc] = self.sharedData.malloc(shm_name+'#portidx')
+        [self.portidxshm, ismalloc] = self.shareddata.malloc(shm_name+'#portidx')
         if not ismalloc:        
-            [self.portidxshm, ismalloc] = self.sharedData.malloc(shm_name+'#portidx',create=True,size=portidxsize_bytes)
+            [self.portidxshm, ismalloc] = self.shareddata.malloc(shm_name+'#portidx',create=True,size=portidxsize_bytes)
             iscreate = True
             
         self.portlistcount = np.ndarray((1,),dtype=np.int32,buffer=self.portidxshm.buf)[0]
         self.portiniidx = np.ndarray((keysize,),dtype=np.int32,\
             buffer=self.portidxshm.buf,offset=4)
         self.portendidx = np.ndarray((keysize,),dtype=np.int32,\
             buffer=self.portidxshm.buf,offset=int(4+keysize_bytes))
@@ -152,28 +152,28 @@
             self.portendidx[:]=-1
             self.portlist[:]=-1
                 
     def create_index(self):
         ti = time.time()
         if self.table.records.count>0:
             print('Creating index %s/%s/%s %i lines...' % \
-                (self.sharedData.database,self.table.feeder,\
+                (self.table.database,self.table.feeder,\
                 self.table.dataset,self.table.records.count))
             time.sleep(0.001)
             arr = self.table.records
             if 'date_portfolio_' in self.pkeystr:
                 self.create_index_func(arr,self.table.records.count,\
                     self.pkey,self.dateiniidx,self.dateendidx,self.dateunit,\
                     self.portiniidx,self.portendidx,self.portlist,self.portlistcount,0)
                 self.portlistcount=self.table.records.count
             else:
                 self.create_index_func(arr,self.table.records.count,self.pkey,\
                     self.dateiniidx,self.dateendidx,self.dateunit,0)
             print('Creating index %s/%s/%s %i lines/s DONE!' % \
-                (self.sharedData.database,self.table.feeder,\
+                (self.table.database,self.table.feeder,\
                 self.table.dataset,self.table.records.count/(time.time()-ti)))
 
     def update_index(self,start):
         self.pkey[:] = -1
         self.dateiniidx[:]=-1        
         self.dateendidx[:]=-1
         arr = self.table.records[0:self.table.records.size]
```

### Comparing `shareddata-2.1.5/src/SharedData/SharedDataTableIndexJit.py` & `shareddata-2.2.0/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/SharedData/SharedNumpy.py` & `shareddata-2.2.0/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/SharedData/Utils.py` & `shareddata-2.2.0/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.1.5/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.2.0/src/shareddata.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.1.5
+Version: 2.2.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.1.5/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.2.0/src/shareddata.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
+src/SharedData/AWSKinesis.py
+src/SharedData/AWSS3.py
+src/SharedData/DataFrame.py
 src/SharedData/Defaults.py
+src/SharedData/Feeder.py
 src/SharedData/Logger.py
 src/SharedData/LoggerConsumerProcess.py
 src/SharedData/Metadata.py
 src/SharedData/MultiProc.py
-src/SharedData/SeriesLib.py
+src/SharedData/Period.py
+src/SharedData/RealTime.py
+src/SharedData/RealTimeProcess.py
 src/SharedData/SharedData.py
-src/SharedData/SharedDataAWSKinesis.py
-src/SharedData/SharedDataAWSS3.py
-src/SharedData/SharedDataFeeder.py
-src/SharedData/SharedDataFrame.py
-src/SharedData/SharedDataPeriod.py
-src/SharedData/SharedDataRealTime.py
-src/SharedData/SharedDataRealTimeProcess.py
-src/SharedData/SharedDataTable.py
-src/SharedData/SharedDataTableIndex.py
-src/SharedData/SharedDataTableIndexJit.py
-src/SharedData/SharedDataTimeSeries.py
 src/SharedData/SharedNumpy.py
+src/SharedData/Table.py
+src/SharedData/TableIndex.py
+src/SharedData/TableIndexJit.py
+src/SharedData/TimeSeries.py
+src/SharedData/TimeseriesContainer.py
 src/SharedData/Utils.py
 src/SharedData/__init__.py
 src/shareddata.egg-info/PKG-INFO
 src/shareddata.egg-info/SOURCES.txt
 src/shareddata.egg-info/dependency_links.txt
 src/shareddata.egg-info/requires.txt
 src/shareddata.egg-info/top_level.txt
```

