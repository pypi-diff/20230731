# Comparing `tmp/shareddata-2.2.3.tar.gz` & `tmp/shareddata-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.2.3.tar", last modified: Mon Jul 31 11:52:37 2023, max compression
+gzip compressed data, was "shareddata-2.2.4.tar", last modified: Mon Jul 31 12:48:21 2023, max compression
```

## Comparing `shareddata-2.2.3.tar` & `shareddata-2.2.4.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.3/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:52:37.242063 shareddata-2.2.3/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.3/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.3/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 11:52:37.242063 shareddata-2.2.3/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.3/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.3/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.3/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.3/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1358 2023-07-29 20:08:45.000000 shareddata-2.2.3/src/SharedData/Feeder.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.3/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.3/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11195 2023-07-31 11:51:26.000000 shareddata-2.2.3/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.3/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    15066 2023-07-29 20:08:40.000000 shareddata-2.2.3/src/SharedData/Period.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.3/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.3/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.3/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9036 2023-07-07 13:16:24.000000 shareddata-2.2.3/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.3/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8626 2023-07-29 20:38:54.000000 shareddata-2.2.3/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.3/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.3/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16353 2023-07-31 11:18:41.000000 shareddata-2.2.3/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.3/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.3/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:52:37.242063 shareddata-2.2.3/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 11:52:37.000000 shareddata-2.2.3/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 12:48:21.333915 shareddata-2.2.4/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.4/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 12:48:21.333915 shareddata-2.2.4/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.4/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.4/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-07-31 12:48:21.333915 shareddata-2.2.4/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 12:48:21.329915 shareddata-2.2.4/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 12:48:21.329915 shareddata-2.2.4/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.4/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.4/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.4/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.4/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.4/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.4/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11195 2023-07-31 11:51:26.000000 shareddata-2.2.4/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.4/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.4/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.4/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.4/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-07-31 12:46:43.000000 shareddata-2.2.4/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.4/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8630 2023-07-31 12:47:07.000000 shareddata-2.2.4/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.4/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.4/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16353 2023-07-31 11:18:41.000000 shareddata-2.2.4/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.4/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.4/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 12:48:21.333915 shareddata-2.2.4/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-07-31 12:48:21.000000 shareddata-2.2.4/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-07-31 12:48:21.000000 shareddata-2.2.4/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 12:48:21.000000 shareddata-2.2.4/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-07-31 12:48:21.000000 shareddata-2.2.4/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-07-31 12:48:21.000000 shareddata-2.2.4/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.2.3/LICENSE` & `shareddata-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/PKG-INFO` & `shareddata-2.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.3
+Version: 2.2.4
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.3/README.md` & `shareddata-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/setup.cfg` & `shareddata-2.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.2.3
+version = 2.2.4
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.2.3/src/SharedData/AWSKinesis.py` & `shareddata-2.2.4/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/AWSS3.py` & `shareddata-2.2.4/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/DataFrame.py` & `shareddata-2.2.4/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/Defaults.py` & `shareddata-2.2.4/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/Logger.py` & `shareddata-2.2.4/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.2.4/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/Metadata.py` & `shareddata-2.2.4/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/MultiProc.py` & `shareddata-2.2.4/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/Period.py` & `shareddata-2.2.4/src/SharedData/TimeseriesContainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,228 +1,233 @@
 import os,io,hashlib,gzip,shutil,time
 import pandas as pd
 import numpy as np
 from datetime import datetime, timedelta
 from pathlib import Path
 from pandas.tseries.offsets import BDay
 from threading import Thread
+from tqdm import tqdm
 
 from SharedData.Logger import Logger
 from SharedData.DataFrame import SharedDataFrame
-from SharedData.TimeSeries import SharedDataTimeSeries
+from SharedData.TimeSeries import TimeSeries
 from SharedData.AWSS3 import S3Upload,S3Download,UpdateModTime
 
-class SharedDataPeriod:
+class TimeseriesContainer:
 
-    def __init__(self, sharedDataFeeder, period):
-        self.sharedDataFeeder = sharedDataFeeder        
-        self.sharedData = sharedDataFeeder.sharedData        
+    def __init__(self, shareddata, database, period, source,\
+        user='master'):
+
+        self.shareddata = shareddata
+        self.user = user
+        self.database = database
         self.period = period
+        self.source = source
             
         # DATA DICTIONARY
         # tags[tag]
-        self.tags = {}        
+        self.tags = {}
 
         # TIME INDEX
         self.timeidx = {}
         self.ctimeidx = {}        
         if self.period=='W1':
-            self.periodSeconds = 7*60*60*24
+            self.periodseconds = 7*60*60*24
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='D1':
-            self.periodSeconds = 60*60*24       
+            self.periodseconds = 60*60*24       
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M15':
-            self.periodSeconds = 60*15
+            self.periodseconds = 60*15
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M1':
-            self.periodSeconds = 60
-            self.default_startDate = pd.Timestamp('2010-01-01')
-        self.getContinousTimeIndex(self.default_startDate)
-        self.loaded = False
+            self.periodseconds = 60
+            self.default_startDate = pd.Timestamp('2010-01-01')        
 
-    def __setitem__(self, tag, df):
-        if not tag in self.tags.keys():
-            if isinstance(tag, pd.Timestamp):
-                self.tags[tag] = SharedDataFrame(self, tag, df)
-            else:
-                self.tags[tag] = SharedDataTimeSeries(self, tag, df)
-        elif isinstance(df, pd.DataFrame):
-            data = self.tags[tag].data
-            iidx = df.index.intersection(data.index)
-            icol = df.columns.intersection(data.columns)
-            data.loc[iidx, icol] = df.loc[iidx, icol].copy()
-
-    def __getitem__(self, tag):
-        if not self.loaded:
-            self.load()
-            self.loaded=True
-        if not tag in self.tags.keys():
-            if isinstance(tag, pd.Timestamp):
-                df = SharedDataFrame(self, tag)
-                if not df.data.empty:
-                    self.tags[tag] = df
-                else:
-                    return pd.DataFrame([])
-            else:                
-                ts = SharedDataTimeSeries(self, tag)                
-                if not ts.data.empty:
-                    self.tags[tag] = ts
-                else:
-                    return pd.DataFrame([])
-        return self.tags[tag].data
+        # self.getContinousTimeIndex(self.default_startDate)
+        self.loaded = False
 
     def getTimeIndex(self, startDate):
         if not startDate in self.timeidx.keys():
             nextsaturday = datetime.today() + BDay(21)\
                 + timedelta((12 - datetime.today().weekday()) % 7)
                         
             if self.period=='D1':
                 self.timeidx[startDate] = pd.Index(\
                     pd.bdate_range(start=startDate,\
                     end=np.datetime64(nextsaturday)))
-                self.periodSeconds = 60*60*24
+                self.periodseconds = 60*60*24
             
             elif self.period=='M15':
                 self.timeidx[startDate] = pd.Index(\
                     pd.bdate_range(start=startDate,\
                     end=np.datetime64(nextsaturday),freq='15min'))                    
                 idx = (self.timeidx[startDate].hour>8) 
                 idx = (idx) & (self.timeidx[startDate].hour<19)
                 idx = (idx) & (self.timeidx[startDate].day_of_week<5)
                 self.timeidx[startDate] = self.timeidx[startDate][idx]
-                self.periodSeconds = 60*15
+                self.periodseconds = 60*15
 
             elif self.period=='M1':
                 self.timeidx[startDate] = pd.Index(\
                     pd.bdate_range(start=startDate,\
                     end=np.datetime64(nextsaturday),freq='1min'))                    
                 idx = (self.timeidx[startDate].hour>8) 
                 idx = (idx) & (self.timeidx[startDate].hour<19)
                 idx = (idx) & (self.timeidx[startDate].day_of_week<5)
                 self.timeidx[startDate] = self.timeidx[startDate][idx]
-                self.periodSeconds = 60
+                self.periodseconds = 60
                 
         return self.timeidx[startDate]
                 
     def getContinousTimeIndex(self, startDate):
         if not startDate in self.ctimeidx.keys():            
             _timeidx = self.getTimeIndex(startDate)
             nsec = (_timeidx - startDate).astype(np.int64)
-            periods = (nsec/(10**9)/self.periodSeconds).astype(np.int64)
+            periods = (nsec/(10**9)/self.periodseconds).astype(np.int64)
             self.ctimeidx[startDate] = np.empty(max(periods)+1)
             self.ctimeidx[startDate][:] = np.nan
             self.ctimeidx[startDate][periods.values] = np.arange(len(periods))        
         return self.ctimeidx[startDate]
 
-    def get_path(self):        
-        shm_name = self.sharedData.user + '/' + self.sharedData.database + '/' \
-            + self.sharedDataFeeder.feeder + '/' + self.period
+    def get_path(self):
+        shm_name = self.user + '/' + self.database + '/' \
+            + self.period + '/' + self.source + '/timeseries'
         if os.name=='posix':
             shm_name = shm_name.replace('/','\\')
-
+            
         path = Path(os.environ['DATABASE_FOLDER'])
-        path = path / self.sharedData.user
-        path = path / self.sharedData.database
-        path = path / self.sharedDataFeeder.feeder
+        path = path / self.user
+        path = path / self.database
         path = path / self.period
+        path = path / self.source
+        path = path / 'timeseries'
         path = Path(str(path).replace('\\','/'))
-        if self.sharedData.save_local:
+        if self.shareddata.save_local:
             if not os.path.isdir(path.parent):
                 os.makedirs(path.parent)
-        return path , shm_name
-
-    #CREATE
-    def create_timeseries(self,tag,startDate,columns,overwrite=False):
-        self.tags[tag] = SharedDataTimeSeries(\
-            self,tag,startDate=startDate,columns=columns,overwrite=overwrite)
-        return self.tags[tag].data
+        
+        return path, shm_name    
 
     # READ
     def load(self):
         # read if not loaded
-        shdatalist = self.sharedData.list()   
+        shdatalist = self.shareddata.list()   
         path, shm_name = self.get_path()
         idx = [shm_name in str(s) for s in shdatalist.index]
         if not np.any(idx):
             self.read()
         else:
             #map
             self.map(shm_name,shdatalist.index[idx])
 
     def map(self,shm_name,shm_name_list):
         for shm in shm_name_list:
             tag = shm.replace(shm_name,'')[1:]
-            self.tags[tag] = SharedDataTimeSeries(self, tag = tag)            
+            self.tags[tag] = TimeSeries(self.shareddata, self, self.database,\
+                    self.period, self.source, tag = tag)
 
     def read(self):
         tini = time.time()
         datasize = 1
         path, shm_name= self.get_path()
         headpath = str(path)+'_head.bin'
         tailpath = str(path)+'_tail.bin'        
         head_io = None
         tail_io = None
-        if self.sharedData.s3read:
-            force_download= (not self.sharedData.save_local)
+        if self.shareddata.s3read:
+            force_download= (not self.shareddata.save_local)
             
             [head_io_gzip, head_local_mtime, head_remote_mtime] = \
                 S3Download(str(headpath),str(headpath)+'.gzip',force_download)
-            if not head_io_gzip is None:
+            if not head_io_gzip is None:                
                 head_io = io.BytesIO()
+                
+                total_size = head_io_gzip.seek(0, 2)
                 head_io_gzip.seek(0)
                 with gzip.GzipFile(fileobj=head_io_gzip, mode='rb') as gz:
-                    shutil.copyfileobj(gz,head_io)
-                if self.sharedData.save_local:
-                    SharedDataPeriod.write_file(head_io,headpath,mtime=head_remote_mtime)
+                    with tqdm(total=total_size, unit='B', unit_scale=True, \
+                        desc='Unzipping %s' % (shm_name), dynamic_ncols=True) as pbar:
+                        chunk_size = int(1024*1024)  
+                        while True:
+                            chunk = gz.read(chunk_size)
+                            if not chunk:
+                                break
+                            head_io.write(chunk)
+                            pbar.update(len(chunk))
+
+                if self.shareddata.save_local:
+                    TimeseriesContainer.write_file(head_io,headpath,mtime=head_remote_mtime,shm_name=shm_name)
                     UpdateModTime(headpath,head_remote_mtime)
                     
             
             [tail_io_gzip, tail_local_mtime, tail_remote_mtime] = \
                 S3Download(str(tailpath),str(tailpath)+'.gzip',force_download)
             if not tail_io_gzip is None:
                 tail_io = io.BytesIO()
                 tail_io_gzip.seek(0)
                 with gzip.GzipFile(fileobj=tail_io_gzip, mode='rb') as gz:
                     shutil.copyfileobj(gz,tail_io)
-                if self.sharedData.save_local:
-                    SharedDataPeriod.write_file(tail_io,tailpath,mtime=tail_remote_mtime)
+                if self.shareddata.save_local:
+                    TimeseriesContainer.write_file(tail_io,tailpath,mtime=tail_remote_mtime,shm_name=shm_name)
                     UpdateModTime(tailpath,tail_remote_mtime)
 
-        if (head_io is None) & (self.sharedData.save_local):
+        if (head_io is None) & (self.shareddata.save_local):
             # read local
             if os.path.isfile(str(headpath)):
                 head_io = open(str(headpath),'rb')            
             
-        if (tail_io is None) & (self.sharedData.save_local):
+        if (tail_io is None) & (self.shareddata.save_local):
             if os.path.isfile(str(tailpath)):
                 tail_io = open(str(tailpath),'rb')
 
         if not head_io is None:
-            datasize += self.read_io(head_io,headpath)
+            datasize += self.read_io(head_io,headpath,shm_name)
 
         if not tail_io is None:
-            datasize += self.read_io(tail_io,tailpath)
+            datasize += self.read_io(tail_io,tailpath,shm_name)
 
         te = time.time()-tini+0.000001   
         datasize = datasize/(1024*1024)
         Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
-            (self.sharedDataFeeder,self.period,datasize,te,datasize/te))
+            (self.source,self.period,datasize,te,datasize/te))
 
-    def read_io(self,io_obj,path):
+    def read_io(self,io_obj,path,shm_name):
         datasize = 0        
         #read
         io_obj.seek(0)
         io_data = io_obj.read()
-        datasize = len(io_data)
-        _m = hashlib.md5(io_data[:-24]).digest()
+        _io_data = io_data[:-24]
+        datasize = len(_io_data)
+        datasizemb = datasize/(1024*1024)
+        if datasizemb>100:
+            message = 'Verifying:%iMB %s' % (datasizemb,shm_name)
+            block_size = 100 * 1024 * 1024 # or any other block size that you prefer
+            nb_total = datasize
+            read_bytes = 0
+            _m = hashlib.md5()                
+            # Use a with block to manage the progress bar
+            with tqdm(total=nb_total, unit='B',unit_scale=True, desc=message) as pbar:
+                # Loop until we have read all the data                    
+                while read_bytes < nb_total:
+                    # Read a block of data
+                    chunk_size = min(block_size, nb_total-read_bytes)
+                    # Update the shared memory buffer with the newly read data
+                    _m.update(_io_data[read_bytes:read_bytes+chunk_size])
+                    read_bytes += chunk_size # update the total number of bytes read so far
+                    # Update the progress bar
+                    pbar.update( chunk_size )
+            _m = _m.digest()
+        else:
+            _m = hashlib.md5(io_data[:-24]).digest()
+        # _m = hashlib.md5(io_data[:-24]).digest()
         m = io_data[-16:]
         if (m!=_m):
-            Logger.log.error('Timeseries file %s corrupted!' % (path))
-            raise Exception('Timeseries file %s corrupted!' % (path))
+            Logger.log.error('Timeseries file %s corrupted!' % (shm_name))
+            raise Exception('Timeseries file %s corrupted!' % (shm_name))
         io_obj.seek(0)
         separator = np.frombuffer(io_obj.read(8),dtype=np.int64)[0]        
         while (separator==1):
             _header = np.frombuffer(io_obj.read(40),dtype=np.int64)
             _tag_b = io_obj.read(int(_header[0]))
             _tag = _tag_b.decode(encoding='UTF-8',errors='ignore')
             _idx_b = io_obj.read(int(_header[1]))
@@ -232,15 +237,16 @@
             _cols = _colscsv.split(',')
             r = _header[3]
             c = _header[4]
             total_bytes = int(r*c*8)
             _data = np.frombuffer(io_obj.read(total_bytes),dtype=np.float64).reshape((r,c))
             df = pd.DataFrame(_data,index=_idx,columns=_cols)
             if not _tag in self.tags.keys():
-                self.tags[_tag] = SharedDataTimeSeries(self, tag = _tag, value = df)
+                self.tags[_tag] = TimeSeries(self.shareddata, self, self.database,\
+                    self.period, self.source, tag = _tag, value = df)
             else:
                 data = self.tags[_tag].data
                 iidx = df.index.intersection(data.index)
                 icol = df.columns.intersection(data.columns)
                 data.loc[iidx, icol] = df.loc[iidx, icol].copy()
             separator = np.frombuffer(io_obj.read(8),dtype=np.int64)[0]
         io_obj.close()
@@ -252,44 +258,44 @@
         path , shm_name= self.get_path()                
         mtime = datetime.now().timestamp()
         partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
         firstdate = pd.Timestamp('1970-01-01')
         if not startDate is None:
             firstdate = startDate        
         if firstdate<partdate:
-            self.write_head(path,partdate,mtime)
+            self.write_head(path,partdate,mtime,shm_name)
         
-        self.write_tail(path,partdate,mtime)
+        self.write_tail(path,partdate,mtime,shm_name)
 
-    def write_head(self,path,partdate,mtime):
+    def write_head(self,path,partdate,mtime,shm_name):
         io_obj = self.create_head_io(partdate)
         
         threads=[]
-        if self.sharedData.s3write:
+        if self.shareddata.s3write:
             io_obj.seek(0)
             gzip_io = io.BytesIO()
             with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
                 shutil.copyfileobj(io_obj, gz)            
             threads = [*threads , Thread(target=S3Upload,\
                 args=(gzip_io, str(path)+'_head.bin.gzip', mtime) )]
 
-        if self.sharedData.save_local:
-            threads = [*threads , Thread(target=SharedDataPeriod.write_file, \
-                args=(io_obj, str(path)+'_head.bin', mtime) )]
+        if self.shareddata.save_local:
+            threads = [*threads , Thread(target=TimeseriesContainer.write_file, \
+                args=(io_obj, str(path)+'_head.bin', mtime, shm_name) )]
         
         for i in range(len(threads)):
             threads[i].start()
 
         for i in range(len(threads)):
             threads[i].join()         
 
     def create_head_io(self,partdate):
         io_obj = io.BytesIO()
         for tag in self.tags.keys():
-            dftag = self[tag].loc[:partdate]
+            dftag = self.tags[tag].data.loc[:partdate]
             startdate = dftag.index[0]
             #create binary df    
             df = dftag.dropna(how='all',axis=0).copy()
             # insert first line to maintain startdate
             df.loc[startdate,:] = dftag.loc[startdate,:]
             r, c = df.shape
             tag_b = str.encode(tag,encoding='UTF-8',errors='ignore')
@@ -309,40 +315,40 @@
             io_obj.write(np.ascontiguousarray(df.values.astype(np.float64)))
 
         m = hashlib.md5(io_obj.getvalue()).digest()
         io_obj.write(np.array([0]).astype(int))
         io_obj.write(m)
         return io_obj
 
-    def write_tail(self,path,partdate,mtime):
+    def write_tail(self,path,partdate,mtime,shm_name):
         io_obj = self.create_tail_io(partdate)
         
         threads=[]
-        if self.sharedData.s3write:
+        if self.shareddata.s3write:
             io_obj.seek(0)
             gzip_io = io.BytesIO()
             with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
                 shutil.copyfileobj(io_obj, gz)            
             threads = [*threads , Thread(target=S3Upload,\
                 args=(gzip_io, str(path)+'_tail.bin.gzip', mtime) )]
 
-        if self.sharedData.save_local:
-            threads = [*threads , Thread(target=SharedDataPeriod.write_file, \
-                args=(io_obj, str(path)+'_tail.bin', mtime) )]
+        if self.shareddata.save_local:
+            threads = [*threads , Thread(target=TimeseriesContainer.write_file, \
+                args=(io_obj, str(path)+'_tail.bin', mtime, shm_name) )]
         
         for i in range(len(threads)):
             threads[i].start()
 
         for i in range(len(threads)):
             threads[i].join()         
 
     def create_tail_io(self,partdate):
         io_obj = io.BytesIO()
         for tag in self.tags.keys():
-            dftag = self[tag].loc[partdate:]
+            dftag = self.tags[tag].data.loc[partdate:]
             #create binary df    
             df = dftag.dropna(how='all',axis=0)            
             r, c = df.shape
             tag_b = str.encode(tag,encoding='UTF-8',errors='ignore')
             idx = (df.index.astype(np.int64))
             idx_b = idx.values.tobytes()
             cols = df.columns.values
@@ -359,12 +365,26 @@
             io_obj.write(np.ascontiguousarray(df.values.astype(np.float64)))
 
         m = hashlib.md5(io_obj.getvalue()).digest()
         io_obj.write(np.array([0]).astype(int))
         io_obj.write(m)
         return io_obj
 
-    def write_file(io_obj,path,mtime):
+    @staticmethod
+    def write_file(io_obj,path,mtime,shm_name):
         with open(path, 'wb') as f:
-            f.write(io_obj.getbuffer())
-            f.flush()
+            nb = len(io_obj.getbuffer())
+            size_mb = nb / (1024*1024)
+            if size_mb>100:
+                blocksize = 1024*1024*100
+                descr = 'Writing:%iMB %s' % (size_mb,shm_name)    
+                with tqdm(total=nb, unit='B', unit_scale=True, desc=descr) as pbar:
+                    written = 0
+                    while written < nb:
+                        chunk_size = min(blocksize, nb-written) # write in chunks of max 100 MB size
+                        f.write(io_obj.getbuffer()[written:written+chunk_size])
+                        written += chunk_size
+                        pbar.update(chunk_size)
+            else:
+                f.write(io_obj.getbuffer())
+            f.flush()            
         os.utime(path, (mtime, mtime))
```

### Comparing `shareddata-2.2.3/src/SharedData/RealTime.py` & `shareddata-2.2.4/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/RealTimeProcess.py` & `shareddata-2.2.4/src/SharedData/RealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/SharedData.py` & `shareddata-2.2.4/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/SharedNumpy.py` & `shareddata-2.2.4/src/SharedData/SharedNumpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                     new_records['mtime'][nidx] = time.time_ns()
 
                 arr = super().__getitem__(slice(0, self.size))
                 arr[_count:_count+nrec] = new_records
                 self.count = _count + nrec
                 self.mtime = datetime.now().timestamp()
             else:
-                Logger.log.error('Dataset max size reached!')
+                Logger.log.error('Table max size reached!')
         except Exception as e:
             Logger.log.error('Error inserting records!\n%s' % (e))
 
         self.table.release()
 
     def overwrite(self, new_records):
         self.table.acquire()
@@ -68,15 +68,15 @@
             if (_count + nrec <= self.size):
                 arr = super().__getitem__(slice(0, self.size))
                 arr[_count:_count+nrec] = new_records
                 self.count = _count + nrec
                 self.minchgid = _count
                 self.mtime = datetime.now().timestamp()
             else:
-                Logger.log.error('Dataset max size reached!')
+                Logger.log.error('Table max size reached!')
         except Exception as e:
             Logger.log.error('Error overwriting records!\n%s' % (e))
 
         self.table.release()
 
     ############################## PRIMARY KEY OPERATIONS ########################################
     def upsert(self, new_records):
@@ -113,18 +113,18 @@
                         self.keys.portiniidx,self.keys.portendidx,self.keys.portlist,self.keys.portlistcount)
                     self.keys.portlistcount = self.count
                 else:
                     self.count, minchgid = self.keys.upsert_func(
                         arr, self.count, new_records, self.pkey,\
                         self.keys.dateiniidx,self.keys.dateendidx,self.keys.dateunit)
 
-                # dataset full
+                # table full
                 if self.count == self.size:
-                    Logger.log.warning('Dataset %s/%s is full!' %
-                                    (self.table.feeder, self.table.dataset))
+                    Logger.log.warning('Table %s/%s is full!' %
+                                    (self.table.source, self.table.tablename))
                 minchgid = int(minchgid)
                 self.minchgid = minchgid
                 self.mtime = datetime.now().timestamp()
             except Exception as e:
                 Logger.log.error('Error upserting records!\n%s' % (e))
 
             self.table.release()
```

### Comparing `shareddata-2.2.3/src/SharedData/Table.py` & `shareddata-2.2.4/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/TableIndex.py` & `shareddata-2.2.4/src/SharedData/TableIndex.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,29 +152,29 @@
             self.portendidx[:]=-1
             self.portlist[:]=-1
                 
     def create_index(self):
         ti = time.time()
         if self.table.records.count>0:
             print('Creating index %s/%s/%s %i lines...' % \
-                (self.table.database,self.table.feeder,\
-                self.table.dataset,self.table.records.count))
+                (self.table.database,self.table.source,\
+                self.table.tablename,self.table.records.count))
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
-                (self.table.database,self.table.feeder,\
-                self.table.dataset,self.table.records.count/(time.time()-ti)))
+                (self.table.database,self.table.source,\
+                self.table.tablename,self.table.records.count/(time.time()-ti)))
 
     def update_index(self,start):
         self.pkey[:] = -1
         self.dateiniidx[:]=-1        
         self.dateendidx[:]=-1
         arr = self.table.records[0:self.table.records.size]        
         if 'date_portfolio_' in self.pkeystr:
```

### Comparing `shareddata-2.2.3/src/SharedData/TableIndexJit.py` & `shareddata-2.2.4/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/TimeSeries.py` & `shareddata-2.2.4/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/SharedData/Utils.py` & `shareddata-2.2.4/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.3/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.2.4/src/shareddata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.3
+Version: 2.2.4
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.3/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.2.4/src/shareddata.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 README.md
 pyproject.toml
 setup.cfg
 src/SharedData/AWSKinesis.py
 src/SharedData/AWSS3.py
 src/SharedData/DataFrame.py
 src/SharedData/Defaults.py
-src/SharedData/Feeder.py
 src/SharedData/Logger.py
 src/SharedData/LoggerConsumerProcess.py
 src/SharedData/Metadata.py
 src/SharedData/MultiProc.py
-src/SharedData/Period.py
 src/SharedData/RealTime.py
 src/SharedData/RealTimeProcess.py
 src/SharedData/SharedData.py
 src/SharedData/SharedNumpy.py
 src/SharedData/Table.py
 src/SharedData/TableIndex.py
 src/SharedData/TableIndexJit.py
```

