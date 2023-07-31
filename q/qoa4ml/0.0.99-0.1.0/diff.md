# Comparing `tmp/qoa4ml-0.0.99.tar.gz` & `tmp/qoa4ml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.99.tar", last modified: Mon Jul 31 17:59:00 2023, max compression
+gzip compressed data, was "qoa4ml-0.1.0.tar", last modified: Mon Jul 31 20:13:09 2023, max compression
```

## Comparing `qoa4ml-0.0.99.tar` & `qoa4ml-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.187764 qoa4ml-0.0.99/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.99/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.99/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.99/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 17:59:00.187301 qoa4ml-0.0.99/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.99/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2023-07-31 17:58:53.000000 qoa4ml-0.0.99/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.99/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.178972 qoa4ml-0.0.99/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13534 2023-07-31 17:56:43.000000 qoa4ml-0.0.99/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.99/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.181501 qoa4ml-0.0.99/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.99/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.99/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.184653 qoa4ml-0.0.99/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.99/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.99/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.99/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.99/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.99/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.99/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.186217 qoa4ml-0.0.99/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.99/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.99/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7689 2023-07-31 16:37:47.000000 qoa4ml-0.0.99/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 17:35:19.000000 qoa4ml-0.0.99/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 17:59:00.180593 qoa4ml-0.0.99/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 17:59:00.000000 qoa4ml-0.0.99/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 17:59:00.000000 qoa4ml-0.0.99/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 17:59:00.000000 qoa4ml-0.0.99/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 17:59:00.000000 qoa4ml-0.0.99/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 17:59:00.000000 qoa4ml-0.0.99/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.99/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 17:59:00.188141 qoa4ml-0.0.99/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.99/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.726326 qoa4ml-0.1.0/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.1.0/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.1.0/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.1.0/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-07-31 20:13:09.726061 qoa4ml-0.1.0/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6845 2023-07-31 20:11:46.000000 qoa4ml-0.1.0/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        5 2023-07-31 20:12:59.000000 qoa4ml-0.1.0/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.1.0/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.719854 qoa4ml-0.1.0/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    14812 2023-07-31 19:42:41.000000 qoa4ml-0.1.0/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.1.0/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.721851 qoa4ml-0.1.0/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.1.0/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.1.0/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.724839 qoa4ml-0.1.0/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.1.0/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.1.0/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.1.0/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.1.0/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.1.0/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.1.0/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.725680 qoa4ml-0.1.0/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6842 2023-07-31 19:42:51.000000 qoa4ml-0.1.0/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4977 2023-07-31 19:51:07.000000 qoa4ml-0.1.0/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6094 2023-07-31 19:07:19.000000 qoa4ml-0.1.0/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11814 2023-07-31 18:03:09.000000 qoa4ml-0.1.0/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 20:13:09.721328 qoa4ml-0.1.0/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7678 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 20:13:09.000000 qoa4ml-0.1.0/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      249 2023-07-31 18:03:45.000000 qoa4ml-0.1.0/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 20:13:09.726412 qoa4ml-0.1.0/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.1.0/setup.py
```

### Comparing `qoa4ml-0.0.99/CHANGELOG.txt` & `qoa4ml-0.1.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/LICENCE.txt` & `qoa4ml-0.1.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/PKG-INFO` & `qoa4ml-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.99
+Version: 0.1.0
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -66,15 +66,15 @@
         - `set`: set the value to a given number.
 
 ## [QoA4ML Reports](https://github.com/rdsea/QoA4ML/blob/main/qoa4ml_lib/qoa4ml/reports.py)
 
 This module defines ``QoA_Report``, an object that provide functions to export monitored metric to the following schema:
 ```json
 {
-    "execution_graph":{
+    "computationGraph":{
         "instances":{
             "@instance_id":{
                 "instance_name": "@name_of_instance",
                 "method": "@method/task/function",
                 "previous_instance":["@list_of_previous_instance"]
             },
             ...
@@ -85,15 +85,15 @@
         "data":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
-        "service":{
+        "performance":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
         "inference":{
```

### Comparing `qoa4ml-0.0.99/README.md` & `qoa4ml-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         - `set`: set the value to a given number.
 
 ## [QoA4ML Reports](https://github.com/rdsea/QoA4ML/blob/main/qoa4ml_lib/qoa4ml/reports.py)
 
 This module defines ``QoA_Report``, an object that provide functions to export monitored metric to the following schema:
 ```json
 {
-    "execution_graph":{
+    "computationGraph":{
         "instances":{
             "@instance_id":{
                 "instance_name": "@name_of_instance",
                 "method": "@method/task/function",
                 "previous_instance":["@list_of_previous_instance"]
             },
             ...
@@ -74,15 +74,15 @@
         "data":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
-        "service":{
+        "performance":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
         "inference":{
```

### Comparing `qoa4ml-0.0.99/qoa4ml/QoaClient.py` & `qoa4ml-0.1.0/qoa4ml/QoaClient.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from threading import Thread
 import time, uuid, requests
 from datetime import datetime
 import logging
 import os, sys, traceback
 from .utils import get_proc_cpu, get_proc_mem, load_config
 from .reports import QoaReport
+from .probes.dataquality import eva_duplicate, eva_erronous, eva_missing, eva_none, image_quality
+from .probes.mlquality import *
 
 headers = {
     'Content-Type': 'application/json'
 }
 
 class QoaClient(object):
     # Init QoA Client
@@ -284,15 +286,44 @@
         report[infID]["instance_id"] = self.instanceID
 
         report[infID][metric_name] = {}
         report[infID][metric_name]["value"] = value
         
         self.qoaReport.observeInferenceMetric(report,dependency=dependency)
         return infID
-
+    
+    def observeErronous(self, data, errors=None):
+        results = eva_erronous(data, errors=errors)
+        if results != None:
+            for key in results:
+                self.observeMetric(key,results[key],1)
+
+    def observeDuplicate(self, data):
+        results = eva_duplicate(data)
+        if results != None:
+            for key in results:
+                self.observeMetric(key,results[key],1)
+    
+    def observeMissing(self, data, null_count=True, correlations=False, predict=False, random_state=0):
+        results = eva_missing(data, null_count=null_count, correlations=correlations, predict=predict, random_state=random_state)
+        if results != None:
+            for key in results:
+                self.observeMetric(key,results[key],1)
+    
+    def observeImgQuality(self, image):
+        results = image_quality(image)
+        if results != None:
+            for key in results:
+                self.observeMetric(key,results[key],1)
+
+    def observeNone(self, data):
+        results = eva_none(data)
+        if results != None:
+            for key in results:
+                self.observeMetric(key,results[key],1)
 
 
         # self.qoaReport = QoA_Report()
         # self.start_time = time.time()
         # self.clientConf = client_conf
         # self.metricList = {}
         # self.connectorList = {}
```

### Comparing `qoa4ml-0.0.99/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.1.0/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.1.0/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.1.0/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.1.0/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.1.0/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/metric.py` & `qoa4ml-0.1.0/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/qoa4ml/probes/dataquality.py` & `qoa4ml-0.1.0/qoa4ml/probes/dataquality.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This library is built based on ydata_quality: https://github.com/ydataai/ydata-quality
 import pandas as pd 
 import numpy as np
-import traceback, sys
+import traceback, sys, logging
 from ydata_quality.erroneous_data import ErroneousDataIdentifier
 from ydata_quality.missings import MissingsProfiler
 from ydata_quality.labelling import LabelInspector
 from ydata_quality.duplicates import DuplicateChecker
 from PIL import Image
 import PIL, io
 import utils
@@ -13,81 +13,84 @@
 # Define metric names, return formats: dictionary {metric name} {sub-element}
 # Return error/debugging
 ################################################ DATA QUALITY ########################################################
 
 
 
 
-def eva_erronous(data, errors=None, ratio=False, sum=True):
+def eva_erronous(data, errors=None):
     """
     Return number/percentage of error data
     data: numpy array or pandas data frame
     errors: list of item considered as error
     ratio: return percentage if set to True
-    sum: sumarize the result if set to True, otherwise return errors following the categories in list of 'errors'
+    sum: sum the result if set to True, otherwise return errors following the categories in list of 'errors'
     """
     try:
         if utils.is_numpyarray(data):
             data = pd.DataFrame(data)
         if utils.is_pddataframe(data):
             if errors and isinstance(errors, list):
                 eva_err =  ErroneousDataIdentifier(df=data,ed_extensions=errors) 
             else:
                 eva_err = ErroneousDataIdentifier(df=data) 
             error_df = eva_err.predefined_erroneous_data()
-            if ratio:
-                total_count = data.count().to_numpy().flatten().sum()
-                error_df.to_numpy().flatten().sum()
-                error_df = 100*error_df/total_count
-            if sum:
-                error_df = error_df.to_numpy().flatten().sum()
-            return error_df
+            
+            total_count = data.count().to_numpy().flatten().sum()
+            results = {}
+            results["Total Errors"] = error_df.to_numpy().flatten().sum()
+            results["Error Ratio"] = 100*error_df/total_count
+            return results
         else:
-            return {"Error": "Unsupported data: {}".format(type(data))}
+            logging.warning("Unsupported data: {}".format(type(data)))
+            return None
     except Exception as e:
         print("[ERROR] - Error {} in eva_erronous: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
-def eva_duplicate(data, ratio=False):
+def eva_duplicate(data):
     """
     Return data/percentage of duplicate
     data: numpy array or pandas data frame
     ratio: return percentage if set to True
     """
     try:
         if utils.is_numpyarray(data):
             data = pd.DataFrame(data)
         if utils.is_pddataframe(data):
             dc = DuplicateChecker(df=data)
-            result = dc.exact_duplicates()
-            if ratio:
-                result = {"duplicate": 100*len(result.index)/len(data.index)}
-            return result
+            dcEva = dc.exact_duplicates()
+            results = {}
+            results["Duplicate Ratio"] = 100*len(dcEva.index)/len(data.index)
+            results["Total Duplicate"] = len(dcEva.index)
+            return results
         else:
-            return {"Error": "Unsupported data: {}".format(type(data))}
+            logging.warning("Unsupported data: {}".format(type(data)))
+            return None
     except Exception as e:
         print("[ERROR] - Error {} in eva_duplicate: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
 def eva_missing(data, null_count=True, correlations=False, predict=False, random_state=0):
     try:
         if utils.is_numpyarray(data):
             data = pd.DataFrame(data)
         if utils.is_pddataframe(data):
             mp = MissingsProfiler(df=data, random_state=random_state)
             results ={}
             if null_count:
-                results["null_count"] = mp.null_count()
+                results["Null Count"] = mp.null_count()
             if correlations:
-                results["correlations"] = mp.missing_correlations()
+                results["Correlations"] = mp.missing_correlations()
             if predict:
-                results["missing_prediction"]= mp.predict_missings()
+                results["Missing Prediction"]= mp.predict_missings()
             return results
         else:
-            return {"Error":  "Unsupported data: {}".format(type(data))}
+            logging.warning("Unsupported data: {}".format(type(data)))
+            return None
     except Exception as e:
         print("[ERROR] - Error {} in eva_erronous: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
 
 class Outlier_Detector(object):
     def __init__(self, data):
         self.data = None
@@ -135,28 +138,32 @@
     quality = {}
     if isinstance(image,bytes):
         image = Image.open(io.BytesIO(image))
     if isinstance(image,np.ndarray):
         image = Image.fromarray(image)
     if isinstance(image,PIL.JpegImagePlugin.JpegImageFile) or isinstance(image,PIL.Image.Image):
         # print(dir(image))
-        quality["image_quality"] = {}
-        quality["image_quality"]["width"] = image.width
-        quality["image_quality"]["height"] = image.height
-        quality["image_quality"]["size"] = image.size
-        quality["image_quality"]["mode"] = image.mode
-        quality["image_quality"]["channel"] = len(image.getbands())
+        quality["Image Width"] = image.width
+        quality["Image Height"] = image.height
+        quality["Image Size"] = image.size
+        quality["Color Mode"] = image.mode
+        quality["Color Channel"] = len(image.getbands())
     return quality
 
 def eva_none(data):
     try:
         if utils.is_pddataframe(data):
             data = data.to_numpy()
         if utils.is_numpyarray(data):
             valid_count = np.count_nonzero(~np.isnan(data))
             none_count = np.count_nonzero(np.isnan(data))
-            return valid_count/(valid_count+none_count)
+            results = {}
+            results["Total Valid"] = valid_count
+            results["Total None"] = none_count
+            results["None Ratio"] = valid_count/(valid_count+none_count)
+            return results
         else:
-            return {"Error":  "Unsupported data: {}".format(type(data))}
+            logging.warning("Unsupported data: {}".format(type(data)))
+            return None
     except Exception as e:
         print("[ERROR] - Error {} in eva_none: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
```

### Comparing `qoa4ml-0.0.99/qoa4ml/probes/mlquality.py` & `qoa4ml-0.1.0/qoa4ml/probes/mlquality.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,95 +18,107 @@
         print("[ERROR] - Error {} when querying timeseries model metrics: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get metrics"}
 
 def ts_inference_metric(model,name):
     try:
         metrics = timeseries_metric(model)
+        results = {}
         if name in metrics:
-            return metrics[name]
+            results[name] = metrics[name]
         if "Error" in metrics:
-            return metrics
+            results["Error"] = metrics["Error"]
+        return results
     except Exception as e:
         print("[ERROR] - Error {} when querying timeseries {}: {}".format(type(e),name,e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model {}".format(name)}
     
 def ts_inference_MAE(model):
     try:
         metrics = ts_inference_metric(model, "mean_absolute_error")
-        return metrics
+        return {"MAE":metrics}
     except Exception as e:
         print("[ERROR] - Error {} when querying timeseries mean absolute error: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model mean absolute error"}
     
 def ts_inference_loss(model):
     try:
         metrics = ts_inference_metric(model, "loss")
-        return metrics
+        return {"Loss":metrics}
     except Exception as e:
         print("[ERROR] - Error {} when querying timeseries mean absolute error: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get model mean absolute error"}
     
 
 def training_metric(model):
     try:
         if isinstance(model, tf.keras.Sequential):
             return model.history.history
+        else:
+            return None
     except Exception as e:
         print("[ERROR] - Error {} when querying training metrics: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get training metrics"}
     
 def training_loss(model):
     try:
         if isinstance(model, tf.keras.Sequential):
-            return model.history.history["loss"]
+            return {"Training Loss":model.history.history["loss"]}
+        else:
+            return None
     except Exception as e:
         print("[ERROR] - Error {} when querying training loss: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get training loss"}
     
 def training_val_accuracy(model):
     try:
         if isinstance(model, tf.keras.Sequential):
-            return model.history.history["val_accuracy"]
+            return {"Evaluate Accuracy":model.history.history["val_accuracy"]}
+        else:
+            return None
     except Exception as e:
         print("[ERROR] - Error {} when querying training validation accuracy: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get validation accuracy"}
 
 def training_accuracy(model):
     try:
         if isinstance(model, tf.keras.Sequential):
-            return model.history.history["accuracy"]
+            return {"Train Accuracy": model.history.history["accuracy"]}
+        else:
+            return None
     except Exception as e:
         print("[ERROR] - Error {} when querying training accuracy: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get accuracy"}
     
 def training_val_loss(model):
     try:
         if isinstance(model, tf.keras.Sequential):
-            return model.history.history["val_loss"]
+            return {"Evaluate Loss":model.history.history["val_loss"]}
+        else:
+            return None
     except Exception as e:
         print("[ERROR] - Error {} when querying training validation loss: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get validation loss"}
 
 def classification_confidence(data, score=True):
     try:
         if score:
-            return 100 * np.max(data)
+            return {"Confidence": 100 * np.max(data)}
         else:
             if is_numpyarray(data):
                 scores = tf.nn.softmax(data[0])
-                return 100 * np.max(scores)
+                return {"Confidence":100 * np.max(scores)}
             else:
                 return {"Error": "Unsupported data: {}".format(type(data))}
     except Exception as e:
         print("[ERROR] - Error {} in extracting classification confidence: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
         return {"Error": "Unable to get classification confidence"}
```

### Comparing `qoa4ml-0.0.99/qoa4ml/reports.py` & `qoa4ml-0.1.0/qoa4ml/reports.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self.computationGraph = {}
         self.report = {}
 
     def import_report_from_file(self, file_path):
         report = load_config(file_path)
         self.qualityReport = report["quality"]
         self.computationGraph = report["computationGraph"]
+        self.metadata = report["metadata"]
     
     def processPReport(self, pReport):
         report = copy.deepcopy(pReport)
         self.reportList.append(report)
         self.previousReportInstance.append(report["computationGraph"]["last_instance"])
         if "inference" in report["quality"]:
             self.previousInference.append(report["quality"]["inference"]["last_inference"])
@@ -110,74 +111,30 @@
         else:
             infReport[key]["source"] = self.previousInference
         if "inference" not in self.qualityReport:
             self.qualityReport["inference"] = {}
         self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],infReport)
         self.qualityReport["inference"]["last_inference"] = key
 
-class Report(object):
-    def __init__(self, report:dict=None):
-        self.report = report
-        if report:
-            self.load_metadata()
-        self.t_report = self.report.copy()
-    
-    def set_report(self, report:dict):
-        self.report = report
-        self.t_report = self.report.copy()
-        self.load_metadata()
-
-    def load_metadata(self):
-        self.application = self.report["application"]
-        self.client_id = self.report["client_id"]
-        self.instance_name = self.report["instance_name"]
-        self.stageID = self.report["stage_id"]
-        self.method = self.report["method"]
-        self.roles = self.report["roles"]
-        self.timestamp = self.report["timestamp"]
-        self.runtime = self.report["runtime"]
-    
-    def load_computationGraph(self):
-        self.computationGraph = self.report["computationGraph"]
+    def sortComputationGraph(self):
+        instanceList = {}
+        source = [self.computationGraph["last_instance"]]
+        rank = 0
+        while len(source) != 0:
+            new_source = []
+            for ikey in source:
+                instanceList.update({ikey:rank})
+                new_source.extend(self.computationGraph["instances"][ikey]["previous_instance"])
+            source = new_source
+            rank += 1
+        return instanceList
 
-    def load_metric(self):
-        if self.t_report:
-            pass
-
-    def getMetric(self, metric_name, data_quality=False, service_quality=False, inference_quality=False):
-        if data_quality:
-            return self.get_data_quality(metric_name)
-        elif service_quality:
-            return self.get_service_quality(metric_name)
-        elif inference_quality:
-            return self.get_inference_quality(metric_name)
-        else:
-            return self.get_data_quality(metric_name)
 
-    def get_responsetime_list(self, sum=True):
-        if self.t_report:
-            data = self.t_report["quality"]["data"]
-            result = 0
-            responsetimes = []
-            for stage in data:
-                stage_i = data[stage]
-                if "Response Time" in stage_i:
-                    dict_res = stage_i.pop("Response Time")
-                    for instance in dict_res:
-                        res = dict_res[instance]
-                        res["instance_id"] = instance
-                        responsetimes.append(res)
-
-    def get_data_quality(self, metric_name):
-        if self.t_report:
-            data = self.t_report["quality"]["data"]
-        else:
-            return None
 
-    def get_service_quality(self, metric_name):
-        if self.t_report:
-            data = self.t_report["quality"]["service"]
-        else:
-            return None
 
-    def get_inference_quality(self, metric_name):
-        pass
+    def getMetric(self, metric_name):
+        metricReport = []
+        for stage in self.qualityReport:
+            if metric_name in self.qualityReport[stage]:
+                pass
+            # Todo 
+
```

### Comparing `qoa4ml-0.0.99/qoa4ml/utils.py` & `qoa4ml-0.1.0/qoa4ml/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ###################### COMMON USED FUNCTION ######################
 def load_config(file_path:str, format=0)->dict:
     """
     file_path: file path to load config
     format:
         0 - json
-        1 - ymal
+        1 - yaml
         other - To Do
     """
     try:
         if format == 0:
             with open(file_path, "r") as f:
                 return json.load(f)
         elif format == 1:
```

### Comparing `qoa4ml-0.0.99/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.1.0/qoa4ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.99
+Version: 0.1.0
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
@@ -66,15 +66,15 @@
         - `set`: set the value to a given number.
 
 ## [QoA4ML Reports](https://github.com/rdsea/QoA4ML/blob/main/qoa4ml_lib/qoa4ml/reports.py)
 
 This module defines ``QoA_Report``, an object that provide functions to export monitored metric to the following schema:
 ```json
 {
-    "execution_graph":{
+    "computationGraph":{
         "instances":{
             "@instance_id":{
                 "instance_name": "@name_of_instance",
                 "method": "@method/task/function",
                 "previous_instance":["@list_of_previous_instance"]
             },
             ...
@@ -85,15 +85,15 @@
         "data":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
-        "service":{
+        "performance":{
             "@stage_id":{
                 "@metric_name":{
                     "@instance_id": "@value"
                 }
             }
         },
         "inference":{
```

### Comparing `qoa4ml-0.0.99/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.1.0/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.99/setup.py` & `qoa4ml-0.1.0/setup.py`

 * *Files identical despite different names*

