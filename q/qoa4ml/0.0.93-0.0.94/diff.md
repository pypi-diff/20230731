# Comparing `tmp/qoa4ml-0.0.93.tar.gz` & `tmp/qoa4ml-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.93.tar", last modified: Mon Jul 31 15:11:42 2023, max compression
+gzip compressed data, was "qoa4ml-0.0.94.tar", last modified: Mon Jul 31 15:17:48 2023, max compression
```

## Comparing `qoa4ml-0.0.93.tar` & `qoa4ml-0.0.94.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.705559 qoa4ml-0.0.93/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.93/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.93/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.93/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:11:42.705289 qoa4ml-0.0.93/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.93/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:11:34.000000 qoa4ml-0.0.93/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.93/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.700162 qoa4ml-0.0.93/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.93/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.93/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.702556 qoa4ml-0.0.93/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.93/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.93/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.704266 qoa4ml-0.0.93/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.93/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.93/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.93/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.93/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.93/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.93/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.704884 qoa4ml-0.0.93/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.93/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.93/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 14:45:04.000000 qoa4ml-0.0.93/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11257 2023-07-31 15:11:24.000000 qoa4ml-0.0.93/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:11:42.701689 qoa4ml-0.0.93/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:11:42.000000 qoa4ml-0.0.93/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:11:42.000000 qoa4ml-0.0.93/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:11:42.000000 qoa4ml-0.0.93/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:11:42.000000 qoa4ml-0.0.93/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:11:42.000000 qoa4ml-0.0.93/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.93/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:11:42.705765 qoa4ml-0.0.93/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.93/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.469022 qoa4ml-0.0.94/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.94/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.94/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.94/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:17:48.468755 qoa4ml-0.0.94/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.94/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:17:22.000000 qoa4ml-0.0.94/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.94/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.462174 qoa4ml-0.0.94/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.94/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.94/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.465666 qoa4ml-0.0.94/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.94/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.94/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.467678 qoa4ml-0.0.94/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.94/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.94/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.94/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.94/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.94/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.94/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.468347 qoa4ml-0.0.94/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.94/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.94/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7606 2023-07-31 15:17:15.000000 qoa4ml-0.0.94/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11185 2023-07-31 15:15:24.000000 qoa4ml-0.0.94/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:17:48.464775 qoa4ml-0.0.94/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:17:48.000000 qoa4ml-0.0.94/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:17:48.000000 qoa4ml-0.0.94/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:17:48.000000 qoa4ml-0.0.94/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:17:48.000000 qoa4ml-0.0.94/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:17:48.000000 qoa4ml-0.0.94/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.94/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:17:48.469241 qoa4ml-0.0.94/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.94/setup.py
```

### Comparing `qoa4ml-0.0.93/CHANGELOG.txt` & `qoa4ml-0.0.94/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/LICENCE.txt` & `qoa4ml-0.0.94/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/PKG-INFO` & `qoa4ml-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.93
+Version: 0.0.94
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.93/README.md` & `qoa4ml-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/QoaClient.py` & `qoa4ml-0.0.94/qoa4ml/QoaClient.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.94/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.94/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.94/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.94/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.94/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/metric.py` & `qoa4ml-0.0.94/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/probes/dataquality.py` & `qoa4ml-0.0.94/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/probes/mlquality.py` & `qoa4ml-0.0.94/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/qoa4ml/reports.py` & `qoa4ml-0.0.94/qoa4ml/reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         key,value = get_dict_at(infReport)
         if dependency != None:
             infReport[key]["source"] = dependency
         else:
             infReport[key]["source"] = self.previousInference
         if "inference" not in self.qualityReport:
             self.qualityReport["inference"] = {}
-        self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],infReport)
+        # self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],infReport)
         self.qualityReport["inference"]["last_inference"] = key
 
 class Report(object):
     def __init__(self, report:dict=None):
         self.report = report
         if report:
             self.load_metadata()
```

### Comparing `qoa4ml-0.0.93/qoa4ml/utils.py` & `qoa4ml-0.0.94/qoa4ml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,19 +276,17 @@
 def docker_monitor(client, interval:int, metrics: dict = None, detail=False):
     if (metrics == None):
         metrics = default_docker_metric
     sub_thread = Thread(target=docker_report, args=(client, interval, metrics,detail))
     sub_thread.start()
 
 
-def mergeReport(fReport, iReport, prio=True):
+def mergeReport(f_report, i_report, prio=True):
     try:
-        if isinstance(fReport, dict) and isinstance(iReport, dict):
-            f_report = fReport.copy()
-            i_report = iReport.copy()
+        if isinstance(f_report, dict) and isinstance(i_report, dict):
             for key in f_report:
                 if key in i_report:
                     f_report[key] = mergeReport(f_report[key],i_report[key],prio)
                     i_report.pop(key)
             f_report.update(i_report)
         else:
             if f_report != i_report:
```

### Comparing `qoa4ml-0.0.93/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.0.94/qoa4ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.93
+Version: 0.0.94
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.93/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.94/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.93/setup.py` & `qoa4ml-0.0.94/setup.py`

 * *Files identical despite different names*

