# Comparing `tmp/access_logs_local-0.0.3.tar.gz` & `tmp/access_logs_local-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_logs_local-0.0.3.tar", last modified: Mon Jul 31 13:23:47 2023, max compression
+gzip compressed data, was "access_logs_local-0.0.4.tar", last modified: Mon Jul 31 13:43:22 2023, max compression
```

## Comparing `access_logs_local-0.0.3.tar` & `access_logs_local-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:23:47.655847 access_logs_local-0.0.3/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1225 2023-07-28 16:31:41.000000 access_logs_local-0.0.3/LICENSE
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1440 2023-07-31 13:23:47.651847 access_logs_local-0.0.3/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      954 2023-07-28 16:32:11.000000 access_logs_local-0.0.3/README.rst
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      632 2023-07-28 16:37:05.000000 access_logs_local-0.0.3/pyproject.toml
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-07-31 13:23:47.655847 access_logs_local-0.0.3/setup.cfg
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:23:47.627847 access_logs_local-0.0.3/src/
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:23:47.639847 access_logs_local-0.0.3/src/access_logs_local.egg-info/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1440 2023-07-31 13:23:47.000000 access_logs_local-0.0.3/src/access_logs_local.egg-info/PKG-INFO
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      492 2023-07-31 13:23:47.000000 access_logs_local-0.0.3/src/access_logs_local.egg-info/SOURCES.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-07-31 13:23:47.000000 access_logs_local-0.0.3/src/access_logs_local.egg-info/dependency_links.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       23 2023-07-31 13:23:47.000000 access_logs_local-0.0.3/src/access_logs_local.egg-info/requires.txt
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       25 2023-07-31 13:23:47.000000 access_logs_local-0.0.3/src/access_logs_local.egg-info/top_level.txt
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:23:47.643847 access_logs_local-0.0.3/src/access_logs_local_driver/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       79 2023-07-28 16:31:41.000000 access_logs_local-0.0.3/src/access_logs_local_driver/__init__.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      967 2023-07-31 13:09:51.000000 access_logs_local-0.0.3/src/access_logs_local_driver/geolookup.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     8058 2023-07-28 16:31:41.000000 access_logs_local-0.0.3/src/access_logs_local_driver/logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      876 2023-07-28 16:31:41.000000 access_logs_local-0.0.3/src/access_logs_local_driver/process_download_logs.py
-drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:23:47.647847 access_logs_local-0.0.3/tests/
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    28563 2023-07-31 13:12:42.000000 access_logs_local-0.0.3/tests/test_logdata.py
--rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     4272 2023-07-31 13:09:24.000000 access_logs_local-0.0.3/tests/test_process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1225 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/LICENSE
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1538 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1052 2023-07-31 13:40:04.000000 access_logs_local-0.0.4/README.rst
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      632 2023-07-31 13:40:22.000000 access_logs_local-0.0.4/pyproject.toml
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       38 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/setup.cfg
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.078181 access_logs_local-0.0.4/src/
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.078181 access_logs_local-0.0.4/src/access_logs_local.egg-info/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     1538 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/PKG-INFO
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      492 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)        1 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       23 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/requires.txt
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       25 2023-07-31 13:43:22.000000 access_logs_local-0.0.4/src/access_logs_local.egg-info/top_level.txt
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/src/access_logs_local_driver/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)       79 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/__init__.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      967 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/geolookup.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     8058 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)      876 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/src/access_logs_local_driver/process_download_logs.py
+drwxrwxr-x   0 cristiangarcia  (1000) cristiangarcia  (1000)        0 2023-07-31 13:43:22.082181 access_logs_local-0.0.4/tests/
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)    28563 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/tests/test_logdata.py
+-rw-rw-r--   0 cristiangarcia  (1000) cristiangarcia  (1000)     4272 2023-07-31 13:39:05.000000 access_logs_local-0.0.4/tests/test_process_download_logs.py
```

### Comparing `access_logs_local-0.0.3/LICENSE` & `access_logs_local-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.3/PKG-INFO` & `access_logs_local-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_logs_local
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -22,14 +22,20 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.4] - 2023-07-31
+
+Changed:
+    * Update file structure and name of the driver
+
+Release Notes:
 [0.0.3] - 2023-07-25
 
 Changed:
     * Update requirements
     * Update using a pyproject.toml file as well as the new deployment structure
```

### Comparing `access_logs_local-0.0.3/README.rst` & `access_logs_local-0.0.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.4] - 2023-07-31
+
+Changed:
+    * Update file structure and name of the driver
+
+Release Notes:
 [0.0.3] - 2023-07-25
 
 Changed:
     * Update requirements
     * Update using a pyproject.toml file as well as the new deployment structure
```

### Comparing `access_logs_local-0.0.3/pyproject.toml` & `access_logs_local-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "access_logs_local"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Cristian Garcia", email="cristian.garcia@ubiquitypress.com" },
 ]
 description = "Functions required by the access-logs-local-driver"
 readme = "README.rst" 
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `access_logs_local-0.0.3/src/access_logs_local.egg-info/PKG-INFO` & `access_logs_local-0.0.4/src/access_logs_local.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-logs-local
-Version: 0.0.3
+Version: 0.0.4
 Summary: Functions required by the access-logs-local-driver
 Author-email: Cristian Garcia <cristian.garcia@ubiquitypress.com>
 Project-URL: Homepage, https://github.com/hirmeos/access_logs_driver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -22,14 +22,20 @@
 We strip out entries where the same (IP address * user agent) pair has accessed
 a URL within the last `SESSION_TIMEOUT` (e.g. half-hour)
 
 Additionally, we convert the URLs to ISBNs and collate request data by date,
 outputting a CSV for ingest via the stats system.
 
 Release Notes:
+[0.0.4] - 2023-07-31
+
+Changed:
+    * Update file structure and name of the driver
+
+Release Notes:
 [0.0.3] - 2023-07-25
 
 Changed:
     * Update requirements
     * Update using a pyproject.toml file as well as the new deployment structure
```

### Comparing `access_logs_local-0.0.3/src/access_logs_local_driver/geolookup.py` & `access_logs_local-0.0.4/src/access_logs_local_driver/geolookup.py`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.3/src/access_logs_local_driver/logdata.py` & `access_logs_local-0.0.4/src/access_logs_local_driver/logdata.py`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.3/src/access_logs_local_driver/process_download_logs.py` & `access_logs_local-0.0.4/src/access_logs_local_driver/process_download_logs.py`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.3/tests/test_logdata.py` & `access_logs_local-0.0.4/tests/test_logdata.py`

 * *Files identical despite different names*

### Comparing `access_logs_local-0.0.3/tests/test_process_download_logs.py` & `access_logs_local-0.0.4/tests/test_process_download_logs.py`

 * *Files identical despite different names*

