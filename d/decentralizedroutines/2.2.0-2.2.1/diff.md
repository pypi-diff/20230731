# Comparing `tmp/decentralizedroutines-2.2.0.tar.gz` & `tmp/decentralizedroutines-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.2.0.tar", last modified: Mon Jul 31 11:20:48 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.2.1.tar", last modified: Mon Jul 31 11:42:50 2023, max compression
```

## Comparing `decentralizedroutines-2.2.0.tar` & `decentralizedroutines-2.2.1.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.361207 decentralizedroutines-2.2.0/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.361207 decentralizedroutines-2.2.0/src/decentralizedroutines/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10073 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/__init__.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      623 2023-07-08 20:05:47.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/master.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1312 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/runroutines.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3281 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/schedule_sequence.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2149 2023-07-18 18:19:13.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/update_version_requirements.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8743 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/worker.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.0/src/decentralizedroutines/worker_lib.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:20:48.365207 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      665 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 11:20:48.000000 decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/decentralizedroutines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      613 2023-07-31 11:35:52.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/master.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/runroutines.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:38:35.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/worker_lib.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.2.0/LICENSE` & `decentralizedroutines-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.0/PKG-INFO` & `decentralizedroutines-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.0
+Version: 2.2.1
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.0/setup.cfg` & `decentralizedroutines-2.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = decentralizedroutines
-version = 2.2.0
+version = 2.2.1
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Master/Worker implementation of decentralized git published routines and kinesis worker pool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/DecentralizedRoutines
 project_urls =
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/RoutineScheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 from datetime import datetime
 from tzlocal import get_localzone 
 local_tz = pytz.timezone(str(get_localzone()))
 
 from SharedData.Metadata import Metadata
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSKinesis import KinesisLogStreamConsumer,KinesisStreamProducer
+from SharedData.AWSKinesis import KinesisLogStreamConsumer,KinesisStreamProducer
 
 class RoutineScheduler:
 
     def __init__(self,stream_name):
         self.consumer = KinesisLogStreamConsumer()
         self.producer = KinesisStreamProducer(stream_name)
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/master.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/master.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os,sys,json
 
 from SharedData.Logger import Logger
 logger = Logger(__file__)
-from SharedData.SharedDataAWSKinesis import KinesisStreamProducer
+from SharedData.AWSKinesis import KinesisStreamProducer
 import decentralizedroutines.defaults as defaults 
 
 producer = KinesisStreamProducer(os.environ['WORKERPOOL_STREAM'])
 
 if len(sys.argv)>=2:
     _argv = sys.argv[1:]
 else:
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/runroutines.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # PROPRIETARY LIBS
 import os,sys,time
 from decentralizedroutines.RoutineScheduler import RoutineScheduler
 from datetime import datetime
 
 import decentralizedroutines.defaults as defaults 
+from SharedData.SharedData import SharedData
+shdata = SharedData(__file__,user='master')
 from SharedData.Logger import Logger
-logger = Logger(__file__,'master')
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,KinesisStreamProducer
+from SharedData.AWSKinesis import KinesisStreamConsumer,KinesisStreamProducer
 
 
 if len(sys.argv)>=2:
     SCHEDULE_NAME = str(sys.argv[1])
 else:
     Logger.log.error('SCHEDULE_NAME not provided, please specify!')
     raise Exception('SCHEDULE_NAME not provided, please specify!')
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/update_version_requirements.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 import pandas as pd
 import numpy as np
 from pathlib import Path
 
 
 from decentralizedroutines.worker_lib import send_command
 import decentralizedroutines.defaults as defaults 
+from SharedData.SharedData import SharedData
+shdata = SharedData(__file__,user='master')
 from SharedData.Logger import Logger
-logger = Logger(__file__)
 
 
 shareddata_version='shareddata==2.0.31'
 decentralizedroutines_version='decentralizedroutines==2.0.31'
 source_folder = Path(os.environ['SOURCE_FOLDER'])
 paths = [Path(source_folder/f) for f in os.listdir(source_folder) if Path.is_dir(source_folder/f)]
 path = paths[1]
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 # SOURCE_FOLDER
 # WORKERPOOL_STREAM
 # GIT_SERVER
 # GIT_USER
 # GIT_ACRONYM
 # GIT_TOKEN
 
-import os,time
+import os,time,sys
 from importlib.metadata import version
 import numpy as np
 from threading import Thread
 
 import decentralizedroutines.defaults as defaults 
+from SharedData.SharedData import SharedData
+shdata = SharedData(r'decentralizedroutines\worker',user='worker')
 from SharedData.Logger import Logger
-logger = Logger(r'decentralizedroutines\worker',user='worker')
 
-from SharedData.SharedDataAWSKinesis import KinesisStreamConsumer,\
+from SharedData.AWSKinesis import KinesisStreamConsumer,\
     KinesisStreamProducer
 from decentralizedroutines.worker_lib import send_command,install_repo,\
     restart_program,run_routine,run_logger,run_scheduler
 
 Logger.log.info('Initializing decentralizedroutines worker version %s...' % \
     (version('decentralizedroutines')))
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.2.1/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.0
+Version: 2.2.1
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.0/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 src/decentralizedroutines/RoutineScheduler.py
 src/decentralizedroutines/__init__.py
 src/decentralizedroutines/defaults.py
 src/decentralizedroutines/master.py
 src/decentralizedroutines/runroutines.py
-src/decentralizedroutines/schedule_sequence.py
 src/decentralizedroutines/update_version_requirements.py
 src/decentralizedroutines/worker.py
 src/decentralizedroutines/worker_lib.py
 src/decentralizedroutines.egg-info/PKG-INFO
 src/decentralizedroutines.egg-info/SOURCES.txt
 src/decentralizedroutines.egg-info/dependency_links.txt
 src/decentralizedroutines.egg-info/requires.txt
```

