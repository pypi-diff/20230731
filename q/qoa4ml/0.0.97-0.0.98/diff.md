# Comparing `tmp/qoa4ml-0.0.97.tar.gz` & `tmp/qoa4ml-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.97.tar", last modified: Mon Jul 31 15:48:05 2023, max compression
+gzip compressed data, was "qoa4ml-0.0.98.tar", last modified: Mon Jul 31 16:38:02 2023, max compression
```

## Comparing `qoa4ml-0.0.97.tar` & `qoa4ml-0.0.98.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.841874 qoa4ml-0.0.97/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.97/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.97/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.97/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:48:05.841629 qoa4ml-0.0.97/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.97/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:48:02.000000 qoa4ml-0.0.97/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.97/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.837398 qoa4ml-0.0.97/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.97/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.97/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.839354 qoa4ml-0.0.97/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.97/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.97/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.840675 qoa4ml-0.0.97/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.97/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.97/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.97/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.97/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.97/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.97/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.841243 qoa4ml-0.0.97/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.97/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.97/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7651 2023-07-31 15:46:59.000000 qoa4ml-0.0.97/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11282 2023-07-31 15:39:00.000000 qoa4ml-0.0.97/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:48:05.838853 qoa4ml-0.0.97/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:48:05.000000 qoa4ml-0.0.97/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:48:05.000000 qoa4ml-0.0.97/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:48:05.000000 qoa4ml-0.0.97/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:48:05.000000 qoa4ml-0.0.97/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:48:05.000000 qoa4ml-0.0.97/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.97/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:48:05.842087 qoa4ml-0.0.97/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.97/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.176354 qoa4ml-0.0.98/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.98/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.98/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.98/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 16:38:02.176089 qoa4ml-0.0.98/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.98/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        6 2023-07-31 16:37:56.000000 qoa4ml-0.0.98/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.98/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.167337 qoa4ml-0.0.98/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.98/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.98/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.170640 qoa4ml-0.0.98/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.98/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.98/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.173918 qoa4ml-0.0.98/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.98/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.98/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.98/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.98/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.98/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.98/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.175296 qoa4ml-0.0.98/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.98/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.98/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7689 2023-07-31 16:37:47.000000 qoa4ml-0.0.98/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11231 2023-07-31 16:35:57.000000 qoa4ml-0.0.98/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 16:38:02.169562 qoa4ml-0.0.98/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 16:38:02.000000 qoa4ml-0.0.98/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 16:38:02.000000 qoa4ml-0.0.98/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 16:38:02.000000 qoa4ml-0.0.98/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 16:38:02.000000 qoa4ml-0.0.98/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 16:38:02.000000 qoa4ml-0.0.98/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.98/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 16:38:02.176577 qoa4ml-0.0.98/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.98/setup.py
```

### Comparing `qoa4ml-0.0.97/CHANGELOG.txt` & `qoa4ml-0.0.98/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/LICENCE.txt` & `qoa4ml-0.0.98/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/PKG-INFO` & `qoa4ml-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.97
+Version: 0.0.98
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.97/README.md` & `qoa4ml-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/QoaClient.py` & `qoa4ml-0.0.98/qoa4ml/QoaClient.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.98/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.98/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.98/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.98/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.98/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/metric.py` & `qoa4ml-0.0.98/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/probes/dataquality.py` & `qoa4ml-0.0.98/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/probes/mlquality.py` & `qoa4ml-0.0.98/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/qoa4ml/reports.py` & `qoa4ml-0.0.98/qoa4ml/reports.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import List
 from .connector.amqp_connector import Amqp_Connector
 from .connector.mqtt_connector import Mqtt_Connector
 from .connector.prom_connector import Prom_Connector
 from .metric import Gauge, Counter, Summary, Histogram
-import json, uuid, time, traceback,sys
+import json, uuid, time, traceback,sys, copy
 from .utils import mergeReport, get_dict_at, load_config
 
 
 class QoaReport(object):
     # Init QoA Client
     def __init__(self, clientConfig):
-        self.clientConfig = clientConfig.copy()
+        self.clientConfig = copy.deepcopy(clientConfig)
         self.reset()
         self.initTime = time.time()
 
     def reset(self):
         self.reportList = []
         self.previousReportInstance = []
         self.previousInference = []
@@ -24,15 +24,15 @@
 
     def import_report_from_file(self, file_path):
         report = load_config(file_path)
         self.qualityReport = report["quality"]
         self.computationGraph = report["computationGraph"]
     
     def processPReport(self, pReport):
-        report = pReport.copy()
+        report = copy.deepcopy(pReport)
         self.reportList.append(report)
         self.previousReportInstance.append(report["computationGraph"]["last_instance"])
         if "inference" in report["quality"]:
             self.previousInference.append(report["quality"]["inference"]["last_inference"])
 
     def importPReport(self, reports):
         try:
@@ -68,18 +68,18 @@
             self.qualityReport = mergeReport(self.qualityReport,i_quality)
         return self.qualityReport
 
     def generateReport(self, metric:list=None,reset=True):
         # Todo: only report on specific metrics
         self.report["computationGraph"] = self.buildComputationGraph()
         self.report["quality"] = self.buildQualityReport()
-        self.report["metadata"] = self.clientConfig.copy()
+        self.report["metadata"] = copy.deepcopy(self.clientConfig)
         self.report["metadata"]["timestamp"] = time.time()
         self.report["metadata"]["runtime"] = self.report["metadata"]["timestamp"] - self.initTime
-        report = self.report.copy()
+        report = copy.deepcopy(self.report)
         if reset:
             self.reset()
         return report
     
     def observeMetric(self, metric):
         metricReport = {}
         metricReport[self.clientConfig["stage_id"]] = {}
```

### Comparing `qoa4ml-0.0.97/qoa4ml/utils.py` & `qoa4ml-0.0.98/qoa4ml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,34 +278,31 @@
         metrics = default_docker_metric
     sub_thread = Thread(target=docker_report, args=(client, interval, metrics,detail))
     sub_thread.start()
 
 
 def mergeReport(f_report, i_report, prio=True):
     try:
-        report = {}
         if isinstance(f_report, dict) and isinstance(i_report, dict):
-            for key in f_report:
-                report[key] = {}
+            key_list = tuple(f_report.keys())
+            for key in key_list:
                 if key in i_report:
-                    report[key] = mergeReport(f_report[key],i_report[key],prio)
+                    f_report[key] = mergeReport(f_report[key],i_report[key],prio)
                     i_report.pop(key)
-            report.update(i_report)
+            f_report.update(i_report)
         else:
             if f_report != i_report:
                 if prio == True:
                     return f_report
                 else:
                     return i_report
-            else:
-                return f_report
     except Exception as e:
         print("[ERROR] - Error {} in mergeReport: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
-    return report
+    return f_report
 
 def get_dict_at(dict, i=0):
     try:
         keys = list(dict.keys())
         return  keys[i], dict[keys[i]]
     except Exception as e:
         print("[ERROR] - Error {} in get_dict_at: {}".format(type(e),e.__traceback__))
```

### Comparing `qoa4ml-0.0.97/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.0.98/qoa4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.97
+Version: 0.0.98
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.97/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.98/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.97/setup.py` & `qoa4ml-0.0.98/setup.py`

 * *Files identical despite different names*

