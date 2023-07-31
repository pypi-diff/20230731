# Comparing `tmp/qsharp-core-0.28.291393b1.tar.gz` & `tmp/qsharp-core-0.28.291394.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsharp-core-0.28.291393b1.tar", last modified: Fri Jul 28 04:12:56 2023, max compression
+gzip compressed data, was "qsharp-core-0.28.291394.tar", last modified: Fri Jul 28 04:09:59 2023, max compression
```

## Comparing `qsharp-core-0.28.291393b1.tar` & `qsharp-core-0.28.291394.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.323932 qsharp-core-0.28.291393b1/
--rw-rw-rw-   0        0        0     2722 2023-07-28 04:12:56.323932 qsharp-core-0.28.291393b1/PKG-INFO
--rw-rw-rw-   0        0        0     2234 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.308342 qsharp-core-0.28.291393b1/qsharp/
--rw-rw-rw-   0        0        0     7076 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/__init__.py
--rw-rw-rw-   0        0        0     7940 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/azure.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.308342 qsharp-core-0.28.291393b1/qsharp/clients/
--rw-rw-rw-   0        0        0     2214 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/clients/__init__.py
--rw-rw-rw-   0        0        0    13962 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/clients/iqsharp.py
--rw-rw-rw-   0        0        0     3023 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/clients/mock.py
--rw-rw-rw-   0        0        0     1718 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/config.py
--rw-rw-rw-   0        0        0      785 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/experimental.py
--rw-rw-rw-   0        0        0     1270 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/ipython_magic.py
--rw-rw-rw-   0        0        0    10472 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/loader.py
--rw-rw-rw-   0        0        0    23551 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/noise_model.py
--rw-rw-rw-   0        0        0     1458 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/packages.py
--rw-rw-rw-   0        0        0     1376 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/projects.py
--rw-rw-rw-   0        0        0     3627 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/qobj.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.308342 qsharp-core-0.28.291393b1/qsharp/results/
--rw-rw-rw-   0        0        0        0 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/results/__init__.py
--rw-rw-rw-   0        0        0    11153 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/results/resource_estimator.py
--rw-rw-rw-   0        0        0     2696 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/serialization.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.323932 qsharp-core-0.28.291393b1/qsharp/tests/
--rw-rw-rw-   0        0        0        0 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/__init__.py
--rw-rw-rw-   0        0        0     6094 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/test_azure.py
--rw-rw-rw-   0        0        0    11603 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/test_iqsharp.py
--rw-rw-rw-   0        0        0     1050 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/test_loader.py
--rw-rw-rw-   0        0        0     2520 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/test_qir.py
--rw-rw-rw-   0        0        0     3075 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/test_serialization.py
--rw-rw-rw-   0        0        0      845 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tests/utils.py
--rw-rw-rw-   0        0        0     2329 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/tomography.py
--rw-rw-rw-   0        0        0     1144 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/types.py
--rw-rw-rw-   0        0        0     1190 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/qsharp/utils.py
--rw-rw-rw-   0        0        0      272 2023-07-28 04:12:54.000000 qsharp-core-0.28.291393b1/qsharp/version.py
-drwxrwxrwx   0        0        0        0 2023-07-28 04:12:56.323932 qsharp-core-0.28.291393b1/qsharp_core.egg-info/
--rw-rw-rw-   0        0        0     2722 2023-07-28 04:12:55.000000 qsharp-core-0.28.291393b1/qsharp_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      809 2023-07-28 04:12:55.000000 qsharp-core-0.28.291393b1/qsharp_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 04:12:55.000000 qsharp-core-0.28.291393b1/qsharp_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-28 04:12:55.000000 qsharp-core-0.28.291393b1/qsharp_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-28 04:12:55.000000 qsharp-core-0.28.291393b1/qsharp_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 04:12:56.323932 qsharp-core-0.28.291393b1/setup.cfg
--rw-rw-rw-   0        0        0     2020 2023-07-28 03:56:50.000000 qsharp-core-0.28.291393b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.570813 qsharp-core-0.28.291394/
+-rw-rw-rw-   0        0        0     2720 2023-07-28 04:09:59.570813 qsharp-core-0.28.291394/PKG-INFO
+-rw-rw-rw-   0        0        0     2234 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.555131 qsharp-core-0.28.291394/qsharp/
+-rw-rw-rw-   0        0        0     7076 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/__init__.py
+-rw-rw-rw-   0        0        0     7940 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/azure.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.555131 qsharp-core-0.28.291394/qsharp/clients/
+-rw-rw-rw-   0        0        0     2214 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/clients/__init__.py
+-rw-rw-rw-   0        0        0    13962 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/clients/iqsharp.py
+-rw-rw-rw-   0        0        0     3023 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/clients/mock.py
+-rw-rw-rw-   0        0        0     1718 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/config.py
+-rw-rw-rw-   0        0        0      785 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/experimental.py
+-rw-rw-rw-   0        0        0     1270 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/ipython_magic.py
+-rw-rw-rw-   0        0        0    10472 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/loader.py
+-rw-rw-rw-   0        0        0    23551 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/noise_model.py
+-rw-rw-rw-   0        0        0     1458 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/packages.py
+-rw-rw-rw-   0        0        0     1376 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/projects.py
+-rw-rw-rw-   0        0        0     3627 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/qobj.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.555131 qsharp-core-0.28.291394/qsharp/results/
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/results/__init__.py
+-rw-rw-rw-   0        0        0    11153 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/results/resource_estimator.py
+-rw-rw-rw-   0        0        0     2696 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/serialization.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.555131 qsharp-core-0.28.291394/qsharp/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/__init__.py
+-rw-rw-rw-   0        0        0     6094 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/test_azure.py
+-rw-rw-rw-   0        0        0    11603 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/test_iqsharp.py
+-rw-rw-rw-   0        0        0     1050 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/test_loader.py
+-rw-rw-rw-   0        0        0     2520 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/test_qir.py
+-rw-rw-rw-   0        0        0     3075 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/test_serialization.py
+-rw-rw-rw-   0        0        0      845 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tests/utils.py
+-rw-rw-rw-   0        0        0     2329 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/tomography.py
+-rw-rw-rw-   0        0        0     1144 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/types.py
+-rw-rw-rw-   0        0        0     1190 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/qsharp/utils.py
+-rw-rw-rw-   0        0        0      268 2023-07-28 04:09:58.000000 qsharp-core-0.28.291394/qsharp/version.py
+drwxrwxrwx   0        0        0        0 2023-07-28 04:09:59.570813 qsharp-core-0.28.291394/qsharp_core.egg-info/
+-rw-rw-rw-   0        0        0     2720 2023-07-28 04:09:59.000000 qsharp-core-0.28.291394/qsharp_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      809 2023-07-28 04:09:59.000000 qsharp-core-0.28.291394/qsharp_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 04:09:59.000000 qsharp-core-0.28.291394/qsharp_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-28 04:09:59.000000 qsharp-core-0.28.291394/qsharp_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-28 04:09:59.000000 qsharp-core-0.28.291394/qsharp_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 04:09:59.570813 qsharp-core-0.28.291394/setup.cfg
+-rw-rw-rw-   0        0        0     2020 2023-07-28 03:52:59.000000 qsharp-core-0.28.291394/setup.py
```

### Comparing `qsharp-core-0.28.291393b1/PKG-INFO` & `qsharp-core-0.28.291394/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-core
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python client for Q#, a domain-specific quantum programming language
 Home-page: https://github.com/microsoft/iqsharp
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-core-0.28.291393b1/README.md` & `qsharp-core-0.28.291394/README.md`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/__init__.py` & `qsharp-core-0.28.291394/qsharp/__init__.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/azure.py` & `qsharp-core-0.28.291394/qsharp/azure.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/clients/__init__.py` & `qsharp-core-0.28.291394/qsharp/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/clients/iqsharp.py` & `qsharp-core-0.28.291394/qsharp/clients/iqsharp.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/clients/mock.py` & `qsharp-core-0.28.291394/qsharp/clients/mock.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/config.py` & `qsharp-core-0.28.291394/qsharp/config.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/experimental.py` & `qsharp-core-0.28.291394/qsharp/experimental.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/ipython_magic.py` & `qsharp-core-0.28.291394/qsharp/ipython_magic.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/loader.py` & `qsharp-core-0.28.291394/qsharp/loader.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/noise_model.py` & `qsharp-core-0.28.291394/qsharp/noise_model.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/packages.py` & `qsharp-core-0.28.291394/qsharp/packages.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/projects.py` & `qsharp-core-0.28.291394/qsharp/projects.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/qobj.py` & `qsharp-core-0.28.291394/qsharp/qobj.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/results/resource_estimator.py` & `qsharp-core-0.28.291394/qsharp/results/resource_estimator.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/serialization.py` & `qsharp-core-0.28.291394/qsharp/serialization.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/test_azure.py` & `qsharp-core-0.28.291394/qsharp/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/test_iqsharp.py` & `qsharp-core-0.28.291394/qsharp/tests/test_iqsharp.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/test_loader.py` & `qsharp-core-0.28.291394/qsharp/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/test_qir.py` & `qsharp-core-0.28.291394/qsharp/tests/test_qir.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/test_serialization.py` & `qsharp-core-0.28.291394/qsharp/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tests/utils.py` & `qsharp-core-0.28.291394/qsharp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/tomography.py` & `qsharp-core-0.28.291394/qsharp/tomography.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/types.py` & `qsharp-core-0.28.291394/qsharp/types.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp/utils.py` & `qsharp-core-0.28.291394/qsharp/utils.py`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/qsharp_core.egg-info/PKG-INFO` & `qsharp-core-0.28.291394/qsharp_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-core
-Version: 0.28.291393b1
+Version: 0.28.291394
 Summary: Python client for Q#, a domain-specific quantum programming language
 Home-page: https://github.com/microsoft/iqsharp
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-core-0.28.291393b1/qsharp_core.egg-info/SOURCES.txt` & `qsharp-core-0.28.291394/qsharp_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsharp-core-0.28.291393b1/setup.py` & `qsharp-core-0.28.291394/setup.py`

 * *Files identical despite different names*

