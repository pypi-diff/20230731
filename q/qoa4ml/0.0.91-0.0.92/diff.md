# Comparing `tmp/qoa4ml-0.0.91.tar.gz` & `tmp/qoa4ml-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoa4ml-0.0.91.tar", last modified: Mon Jul 31 14:57:07 2023, max compression
+gzip compressed data, was "qoa4ml-0.0.92.tar", last modified: Mon Jul 31 15:06:06 2023, max compression
```

## Comparing `qoa4ml-0.0.91.tar` & `qoa4ml-0.0.92.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.788037 qoa4ml-0.0.91/
--rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.91/CHANGELOG.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.91/LICENCE.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.91/MANIFEST.in
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:57:07.787769 qoa4ml-0.0.91/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.91/README.md
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:57:02.000000 qoa4ml-0.0.91/VERSION
--rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.91/pyproject.toml
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.780470 qoa4ml-0.0.91/qoa4ml/
--rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.91/qoa4ml/QoaClient.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.91/qoa4ml/__init__.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.783089 qoa4ml-0.0.91/qoa4ml/collector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.91/qoa4ml/collector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.91/qoa4ml/collector/amqp_collector.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.785832 qoa4ml-0.0.91/qoa4ml/connector/
--rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.91/qoa4ml/connector/__init__.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.91/qoa4ml/connector/amqp_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.91/qoa4ml/connector/mess_logging.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.91/qoa4ml/connector/mqtt_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.91/qoa4ml/connector/prom_connector.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.91/qoa4ml/metric.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.786988 qoa4ml-0.0.91/qoa4ml/probes/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.91/qoa4ml/probes/dataquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.91/qoa4ml/probes/mlquality.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 14:45:04.000000 qoa4ml-0.0.91/qoa4ml/reports.py
--rw-r--r--   0 tringuyen   (501) wheel        (0)    11185 2023-07-31 13:24:11.000000 qoa4ml-0.0.91/qoa4ml/utils.py
-drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 14:57:07.782363 qoa4ml-0.0.91/qoa4ml.egg-info/
--rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/PKG-INFO
--rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/SOURCES.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/dependency_links.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/requires.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 14:57:07.000000 qoa4ml-0.0.91/qoa4ml.egg-info/top_level.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.91/requirements.txt
--rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 14:57:07.788260 qoa4ml-0.0.91/setup.cfg
--rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.91/setup.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.863457 qoa4ml-0.0.92/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      563 2023-05-22 14:23:36.000000 qoa4ml-0.0.92/CHANGELOG.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1047 2022-03-23 13:04:50.000000 qoa4ml-0.0.92/LICENCE.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       39 2023-07-31 12:17:09.000000 qoa4ml-0.0.92/MANIFEST.in
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:06:06.863165 qoa4ml-0.0.92/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6840 2023-07-31 10:28:13.000000 qoa4ml-0.0.92/README.md
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:05:59.000000 qoa4ml-0.0.92/VERSION
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       84 2022-09-02 11:22:46.000000 qoa4ml-0.0.92/pyproject.toml
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.856790 qoa4ml-0.0.92/qoa4ml/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    13237 2023-07-31 14:56:45.000000 qoa4ml-0.0.92/qoa4ml/QoaClient.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2023-07-31 13:14:03.000000 qoa4ml-0.0.92/qoa4ml/__init__.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.858713 qoa4ml-0.0.92/qoa4ml/collector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:26.000000 qoa4ml-0.0.92/qoa4ml/collector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2120 2023-01-30 17:43:18.000000 qoa4ml-0.0.92/qoa4ml/collector/amqp_collector.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.861446 qoa4ml-0.0.92/qoa4ml/connector/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        0 2022-03-23 14:05:29.000000 qoa4ml-0.0.92/qoa4ml/connector/__init__.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2093 2023-01-30 16:55:55.000000 qoa4ml-0.0.92/qoa4ml/connector/amqp_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1379 2022-03-23 09:27:48.000000 qoa4ml-0.0.92/qoa4ml/connector/mess_logging.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     1611 2022-03-23 09:32:08.000000 qoa4ml-0.0.92/qoa4ml/connector/mqtt_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     2189 2022-03-23 09:33:14.000000 qoa4ml-0.0.92/qoa4ml/connector/prom_connector.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4181 2023-07-31 13:38:41.000000 qoa4ml-0.0.92/qoa4ml/metric.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.862492 qoa4ml-0.0.92/qoa4ml/probes/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     6691 2023-07-18 06:51:33.000000 qoa4ml-0.0.92/qoa4ml/probes/dataquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     4587 2023-05-31 13:54:44.000000 qoa4ml-0.0.92/qoa4ml/probes/mlquality.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7604 2023-07-31 14:45:04.000000 qoa4ml-0.0.92/qoa4ml/reports.py
+-rw-r--r--   0 tringuyen   (501) wheel        (0)    11251 2023-07-31 15:05:25.000000 qoa4ml-0.0.92/qoa4ml/utils.py
+drwxr-xr-x   0 tringuyen   (501) wheel        (0)        0 2023-07-31 15:06:06.858211 qoa4ml-0.0.92/qoa4ml.egg-info/
+-rw-r--r--   0 tringuyen   (501) wheel        (0)     7674 2023-07-31 15:06:06.000000 qoa4ml-0.0.92/qoa4ml.egg-info/PKG-INFO
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      622 2023-07-31 15:06:06.000000 qoa4ml-0.0.92/qoa4ml.egg-info/SOURCES.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        1 2023-07-31 15:06:06.000000 qoa4ml-0.0.92/qoa4ml.egg-info/dependency_links.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 15:06:06.000000 qoa4ml-0.0.92/qoa4ml.egg-info/requires.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)        7 2023-07-31 15:06:06.000000 qoa4ml-0.0.92/qoa4ml.egg-info/top_level.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      235 2023-07-31 13:04:18.000000 qoa4ml-0.0.92/requirements.txt
+-rw-r--r--   0 tringuyen   (501) wheel        (0)       38 2023-07-31 15:06:06.863685 qoa4ml-0.0.92/setup.cfg
+-rw-r--r--   0 tringuyen   (501) wheel        (0)      711 2023-07-31 12:17:09.000000 qoa4ml-0.0.92/setup.py
```

### Comparing `qoa4ml-0.0.91/CHANGELOG.txt` & `qoa4ml-0.0.92/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/LICENCE.txt` & `qoa4ml-0.0.92/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/PKG-INFO` & `qoa4ml-0.0.92/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.91
+Version: 0.0.92
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.91/README.md` & `qoa4ml-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/QoaClient.py` & `qoa4ml-0.0.92/qoa4ml/QoaClient.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/collector/amqp_collector.py` & `qoa4ml-0.0.92/qoa4ml/collector/amqp_collector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/connector/amqp_connector.py` & `qoa4ml-0.0.92/qoa4ml/connector/amqp_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/connector/mess_logging.py` & `qoa4ml-0.0.92/qoa4ml/connector/mess_logging.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/connector/mqtt_connector.py` & `qoa4ml-0.0.92/qoa4ml/connector/mqtt_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/connector/prom_connector.py` & `qoa4ml-0.0.92/qoa4ml/connector/prom_connector.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/metric.py` & `qoa4ml-0.0.92/qoa4ml/metric.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/probes/dataquality.py` & `qoa4ml-0.0.92/qoa4ml/probes/dataquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/probes/mlquality.py` & `qoa4ml-0.0.92/qoa4ml/probes/mlquality.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/reports.py` & `qoa4ml-0.0.92/qoa4ml/reports.py`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/qoa4ml/utils.py` & `qoa4ml-0.0.92/qoa4ml/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,16 +276,18 @@
 def docker_monitor(client, interval:int, metrics: dict = None, detail=False):
     if (metrics == None):
         metrics = default_docker_metric
     sub_thread = Thread(target=docker_report, args=(client, interval, metrics,detail))
     sub_thread.start()
 
 
-def mergeReport(f_report, i_report, prio=True):
+def mergeReport(fReport, iReport, prio=True):
     try:
+        f_report = fReport.copy()
+        i_report = iReport.copy()
         if isinstance(f_report, dict) and isinstance(i_report, dict):
             for key in f_report:
                 if key in i_report:
                     f_report[key] = mergeReport(f_report[key],i_report[key],prio)
                     i_report.pop(key)
             f_report.update(i_report)
         else:
```

### Comparing `qoa4ml-0.0.91/qoa4ml.egg-info/PKG-INFO` & `qoa4ml-0.0.92/qoa4ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoa4ml
-Version: 0.0.91
+Version: 0.0.92
 Summary: Quality of Analysis for Machine Learning
 Home-page: https://rdsea.github.io/
 Author: AaltoSEA
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `qoa4ml-0.0.91/qoa4ml.egg-info/SOURCES.txt` & `qoa4ml-0.0.92/qoa4ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoa4ml-0.0.91/setup.py` & `qoa4ml-0.0.92/setup.py`

 * *Files identical despite different names*

