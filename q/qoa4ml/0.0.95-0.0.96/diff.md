# Comparing `tmp/qoa4ml-0.0.95.tar.gz` & `tmp/qoa4ml-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.95.tar", last modified: Mon Jul 31 15:24:36 2023, max compression
+gzip compressed data, was "qoa4ml-0.0.96.tar", last modified: Mon Jul 31 15:41:20 2023, max compression
```

## Comparing `qoa4ml-0.0.95.tar` & `qoa4ml-0.0.96.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.412269 qoa4ml-0.0.95/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.95/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.95/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.95/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:24:36.412003 qoa4ml-0.0.95/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.95/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:24:33.000000 qoa4ml-0.0.95/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.95/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.407516 qoa4ml-0.0.95/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.95/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.95/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.409600 qoa4ml-0.0.95/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.95/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.95/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.410995 qoa4ml-0.0.95/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.95/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.95/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.95/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.95/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.95/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.95/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.411610 qoa4ml-0.0.95/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.95/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.95/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7793 2023-07-31 15:24:25.000000 qoa4ml-0.0.95/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11185 2023-07-31 15:15:24.000000 qoa4ml-0.0.95/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:24:36.409073 qoa4ml-0.0.95/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:24:36.000000 qoa4ml-0.0.95/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:24:36.000000 qoa4ml-0.0.95/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:24:36.000000 qoa4ml-0.0.95/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:24:36.000000 qoa4ml-0.0.95/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:24:36.000000 qoa4ml-0.0.95/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.95/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:24:36.412484 qoa4ml-0.0.95/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.95/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.204602 qoa4ml-0.0.96/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.96/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.96/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.96/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:41:20.204342 qoa4ml-0.0.96/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.96/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:41:15.000000 qoa4ml-0.0.96/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.96/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.197835 qoa4ml-0.0.96/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.96/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.96/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.201034 qoa4ml-0.0.96/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.96/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.96/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.203182 qoa4ml-0.0.96/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.96/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.96/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.96/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.96/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.96/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.96/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.203911 qoa4ml-0.0.96/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.96/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.96/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 15:28:14.000000 qoa4ml-0.0.96/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11282 2023-07-31 15:39:00.000000 qoa4ml-0.0.96/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:41:20.200084 qoa4ml-0.0.96/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:41:20.000000 qoa4ml-0.0.96/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:41:20.000000 qoa4ml-0.0.96/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:41:20.000000 qoa4ml-0.0.96/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:41:20.000000 qoa4ml-0.0.96/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:41:20.000000 qoa4ml-0.0.96/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.96/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:41:20.204875 qoa4ml-0.0.96/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.96/setup.py
```

### Comparing `qoa4ml-0.0.95/CHANGELOG.txt` & `qoa4ml-0.0.96/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/LICENCE.txt` & `qoa4ml-0.0.96/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/PKG-INFO` & `qoa4ml-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.95
+Version: 0.0.96
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.95/README.md` & `qoa4ml-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/QoaClient.py` & `qoa4ml-0.0.96/qoa4ml/QoaClient.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.96/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.96/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.96/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.96/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.96/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/metric.py` & `qoa4ml-0.0.96/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/probes/dataquality.py` & `qoa4ml-0.0.96/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/probes/mlquality.py` & `qoa4ml-0.0.96/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/qoa4ml/reports.py` & `qoa4ml-0.0.96/qoa4ml/reports.py`

 * *Files 5% similar despite different names*

```diff
@@ -75,51 +75,46 @@
         self.report["metadata"]["timestamp"] = time.time()
         self.report["metadata"]["runtime"] = self.report["metadata"]["timestamp"] - self.initTime
         report = self.report.copy()
         if reset:
             self.reset()
         return report
     
-    def mergeReport(self, fReport, iReport):
-        f_report = fReport.copy()
-        i_report = iReport.copy()
-        return mergeReport(f_report,i_report)
-
     def observeMetric(self, metric):
         metricReport = {}
         metricReport[self.clientConfig["stage_id"]] = {}
         metricReport[self.clientConfig["stage_id"]][metric.name] = {}
         metricReport[self.clientConfig["stage_id"]][metric.name][self.clientConfig["instances_id"]] = metric.value
 
         if metric.category == 0:
             if "performance" not in self.qualityReport:
                 self.qualityReport["performance"] = {}
-            self.qualityReport["performance"] = self.mergeReport(self.qualityReport["performance"],metricReport)
+            self.qualityReport["performance"] = mergeReport(self.qualityReport["performance"],metricReport)
         elif metric.category == 1:
             if "data" not in self.qualityReport:
                 self.qualityReport["data"] = {}
-            self.qualityReport["data"] = self.mergeReport(self.qualityReport["data"],metricReport)
-        # elif metric.category == 2:
-        #     key,value = get_dict_at(metricReport)
-        #     metricReport[key]["source"] = self.previousInference
-        #     if "inference" not in self.qualityReport:
-        #         self.qualityReport["inference"] = {}
-        #     self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],metricReport)
-        #     self.qualityReport["inference"]["last_inference"] = key
+            self.qualityReport["data"] = mergeReport(self.qualityReport["data"],metricReport)
+        elif metric.category == 2:
+            key,value = get_dict_at(metricReport)
+            metricReport[key]["source"] = self.previousInference
+            if "inference" not in self.qualityReport:
+                self.qualityReport["inference"] = {}
+            self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],metricReport)
+            self.qualityReport["inference"]["last_inference"] = key
 
     def observeInferenceMetric(self, infReport, dependency=None):
 
         key,value = get_dict_at(infReport)
         if dependency != None:
             infReport[key]["source"] = dependency
         else:
             infReport[key]["source"] = self.previousInference
         if "inference" not in self.qualityReport:
             self.qualityReport["inference"] = {}
-        self.qualityReport["inference"] = self.mergeReport(self.qualityReport["inference"],infReport)
+        self.qualityReport["inference"] = mergeReport(self.qualityReport["inference"],infReport)
         self.qualityReport["inference"]["last_inference"] = key
 
 class Report(object):
     def __init__(self, report:dict=None):
         self.report = report
         if report:
             self.load_metadata()
```

### Comparing `qoa4ml-0.0.95/qoa4ml/utils.py` & `qoa4ml-0.0.96/qoa4ml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,30 +278,34 @@
         metrics = default_docker_metric
     sub_thread = Thread(target=docker_report, args=(client, interval, metrics,detail))
     sub_thread.start()
 
 
 def mergeReport(f_report, i_report, prio=True):
     try:
+        report = {}
         if isinstance(f_report, dict) and isinstance(i_report, dict):
             for key in f_report:
+                report[key] = {}
                 if key in i_report:
-                    f_report[key] = mergeReport(f_report[key],i_report[key],prio)
+                    report[key] = mergeReport(f_report[key],i_report[key],prio)
                     i_report.pop(key)
-            f_report.update(i_report)
+            report.update(i_report)
         else:
             if f_report != i_report:
                 if prio == True:
                     return f_report
                 else:
                     return i_report
+            else:
+                return f_report
     except Exception as e:
         print("[ERROR] - Error {} in mergeReport: {}".format(type(e),e.__traceback__))
         traceback.print_exception(*sys.exc_info())
-    return f_report
+    return report
 
 def get_dict_at(dict, i=0):
     try:
         keys = list(dict.keys())
         return  keys[i], dict[keys[i]]
     except Exception as e:
         print("[ERROR] - Error {} in get_dict_at: {}".format(type(e),e.__traceback__))
```

### Comparing `qoa4ml-0.0.95/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.0.96/qoa4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.95
+Version: 0.0.96
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.95/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.96/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.95/setup.py` & `qoa4ml-0.0.96/setup.py`

 * *Files identical despite different names*

