# Comparing `tmp/qoa4ml-0.0.90.tar.gz` & `tmp/qoa4ml-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.90.tar", last modified: Mon Jul 31 14:54:16 2023, max compression
+gzip compressed data, was "qoa4ml-0.0.91.tar", last modified: Mon Jul 31 14:57:07 2023, max compression
```

## Comparing `qoa4ml-0.0.90.tar` & `qoa4ml-0.0.91.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.852946 qoa4ml-0.0.90/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.90/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.90/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.90/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:54:16.852512 qoa4ml-0.0.90/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.90/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:54:14.000000 qoa4ml-0.0.90/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.90/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.843463 qoa4ml-0.0.90/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13246 2023-07-31 14:54:06.000000 qoa4ml-0.0.90/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.90/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.846309 qoa4ml-0.0.90/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.90/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.90/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.849674 qoa4ml-0.0.90/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.90/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.90/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.90/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.90/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.90/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.90/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.851333 qoa4ml-0.0.90/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.90/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.90/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 14:45:04.000000 qoa4ml-0.0.90/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11185 2023-07-31 13:24:11.000000 qoa4ml-0.0.90/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:54:16.845549 qoa4ml-0.0.90/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:54:16.000000 qoa4ml-0.0.90/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 14:54:16.000000 qoa4ml-0.0.90/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 14:54:16.000000 qoa4ml-0.0.90/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 14:54:16.000000 qoa4ml-0.0.90/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:54:16.000000 qoa4ml-0.0.90/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.90/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 14:54:16.853385 qoa4ml-0.0.90/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.90/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.788037 qoa4ml-0.0.91/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.91/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.91/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.91/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:57:07.787769 qoa4ml-0.0.91/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.91/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:57:02.000000 qoa4ml-0.0.91/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.91/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.780470 qoa4ml-0.0.91/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.91/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.91/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.783089 qoa4ml-0.0.91/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.91/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.91/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.785832 qoa4ml-0.0.91/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.91/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.91/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.91/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.91/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.91/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.91/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.786988 qoa4ml-0.0.91/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.91/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.91/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 14:45:04.000000 qoa4ml-0.0.91/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11185 2023-07-31 13:24:11.000000 qoa4ml-0.0.91/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.782363 qoa4ml-0.0.91/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.91/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 14:57:07.788260 qoa4ml-0.0.91/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.91/setup.py
```

### Comparing `qoa4ml-0.0.90/CHANGELOG.txt` & `qoa4ml-0.0.91/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/LICENCE.txt` & `qoa4ml-0.0.91/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/PKG-INFO` & `qoa4ml-0.0.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.90
+Version: 0.0.91
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.90/README.md` & `qoa4ml-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/QoaClient.py` & `qoa4ml-0.0.91/qoa4ml/QoaClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         self.lock.release()
 
     def report(self, metrics:list=None, report: dict = None, connectors:list=None, submit=False,reset=True):
         if (report == None):
             report = self.qoaReport.generateReport(metrics, reset=reset)
         if submit:
             if self.default_connector != None:
-                sub_thread = Thread(target=self.asyn_report, args=(metrics, report, connectors))
+                sub_thread = Thread(target=self.asyn_report, args=(report, connectors))
                 sub_thread.start()
             else:
                 logging.warning("No connector available")
         return report
 
     def observeInferenceMetric(self, metric_name, value, new_inf=False, inference_id=None, dependency=None):
         report = {}
```

### Comparing `qoa4ml-0.0.90/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.91/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.91/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.91/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.91/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.91/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/metric.py` & `qoa4ml-0.0.91/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/probes/dataquality.py` & `qoa4ml-0.0.91/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/probes/mlquality.py` & `qoa4ml-0.0.91/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/reports.py` & `qoa4ml-0.0.91/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml/utils.py` & `qoa4ml-0.0.91/qoa4ml/utils.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.0.91/qoa4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.90
+Version: 0.0.91
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.90/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.91/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.90/setup.py` & `qoa4ml-0.0.91/setup.py`

 * *Files identical despite different names*

