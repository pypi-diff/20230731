# Comparing `tmp/testflows.github.runners-1.3.230731.1154931.tar.gz` & `tmp/testflows.github.runners-1.3.230731.1173142.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230731.1154931.tar", last modified: Mon Jul 31 15:49:31 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230731.1173142.tar", last modified: Mon Jul 31 17:31:42 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230731.1154931.tar` & `testflows.github.runners-1.3.230731.1173142.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    48447 2023-07-31 15:49:25.000000 testflows.github.runners-1.3.230731.1154931/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.399552 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5122 2023-07-29 20:55:15.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1154931/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 15:49:31.395552 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 15:49:31.000000 testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    48447 2023-07-31 15:49:25.000000 testflows.github.runners-1.3.230731.1173142/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.328390 testflows.github.runners-1.3.230731.1173142/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.328390 testflows.github.runners-1.3.230731.1173142/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    23381 2023-07-31 15:15:18.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-07-31 15:16:54.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10814 2023-07-29 23:14:39.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16903 2023-07-31 15:02:38.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230731.1173142/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-31 17:31:42.332390 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    49039 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1154 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-31 17:31:42.000000 testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230731.1154931/LICENSE` & `testflows.github.runners-1.3.230731.1173142/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/PKG-INFO` & `testflows.github.runners-1.3.230731.1173142/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230731.1154931
+Version: 1.3.230731.1173142
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230731.1154931/README.rst` & `testflows.github.runners-1.3.230731.1173142/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/setup.py` & `testflows.github.runners-1.3.230731.1173142/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230731.1154931",
+    version="1.3.230731.1173142",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230731.1154931"
+__version__ = "1.3.230731.1173142"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     command += f" --workers {config.workers}"
     command += f" --default-type {config.default_server_type.name}"
     command += (
         f" --default-location {config.default_location.name}"
         if config.default_location
         else ""
     )
-    command += f" --default-image {config.default_image.type}:{config.default_image.name or config.default_image.description}"
+    command += f" --default-image {config.default_image.architecture}:{config.default_image.type}:{config.default_image.name or config.default_image.description}"
     command += f" --max-runners {config.max_runners}" if config.max_runners else ""
     command += f" --setup-script {config.setup_script}" if config.setup_script else ""
     command += (
         f" --startup-x64-script {config.startup_x64_script}"
         if config.startup_x64_script
         else ""
     )
```

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230731.1173142/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230731.1154931
+Version: 1.3.230731.1173142
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.3.230731.1154931/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230731.1173142/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

