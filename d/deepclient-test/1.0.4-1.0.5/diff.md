# Comparing `tmp/deepclient-test-1.0.4.tar.gz` & `tmp/deepclient-test-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepclient-test-1.0.4.tar", last modified: Sun Jul 30 21:55:45 2023, max compression
+gzip compressed data, was "deepclient-test-1.0.5.tar", last modified: Mon Jul 31 00:18:32 2023, max compression
```

## Comparing `deepclient-test-1.0.4.tar` & `deepclient-test-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/deepclient/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/deepclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/deepclient/deep_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/deepclient/deep_client_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/deepclient/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/deepclient_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-30 21:55:45.000000 deepclient-test-1.0.4/deepclient_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-30 21:55:45.000000 deepclient-test-1.0.4/deepclient_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 21:55:45.000000 deepclient-test-1.0.4/deepclient_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-30 21:55:45.000000 deepclient-test-1.0.4/deepclient_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-30 21:55:45.000000 deepclient-test-1.0.4/deepclient_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 21:55:45.634216 deepclient-test-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-07-30 21:55:26.000000 deepclient-test-1.0.4/tests/test_deep_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:32.199208 deepclient-test-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 00:18:32.199208 deepclient-test-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:32.195208 deepclient-test-1.0.5/deepclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27126 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/deep_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/deep_client_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:32.195208 deepclient-test-1.0.5/deepclient/generate_gql_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/generate_gql_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/generate_gql_operations/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/generate_gql_operations/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/deepclient/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:32.195208 deepclient-test-1.0.5/deepclient_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-31 00:18:32.000000 deepclient-test-1.0.5/deepclient_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-31 00:18:32.000000 deepclient-test-1.0.5/deepclient_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:18:32.000000 deepclient-test-1.0.5/deepclient_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-31 00:18:32.000000 deepclient-test-1.0.5/deepclient_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 00:18:32.000000 deepclient-test-1.0.5/deepclient_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:18:32.199208 deepclient-test-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:32.195208 deepclient-test-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16021 2023-07-31 00:18:11.000000 deepclient-test-1.0.5/tests/test_deep_client.py
```

### Comparing `deepclient-test-1.0.4/PKG-INFO` & `deepclient-test-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepclient-test
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep Client - a way to connect your favorite language with Deep
 Home-page: https://github.com/Lotos2021/deepclient-test
 License: Unlicense
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deepclient-test-1.0.4/deepclient/deep_client.py` & `deepclient-test-1.0.5/deepclient/deep_client.py`

 * *Files identical despite different names*

### Comparing `deepclient-test-1.0.4/deepclient/deep_client_options.py` & `deepclient-test-1.0.5/deepclient/deep_client_options.py`

 * *Files identical despite different names*

### Comparing `deepclient-test-1.0.4/deepclient/query.py` & `deepclient-test-1.0.5/deepclient/query.py`

 * *Files identical despite different names*

### Comparing `deepclient-test-1.0.4/deepclient_test.egg-info/PKG-INFO` & `deepclient-test-1.0.5/deepclient_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepclient-test
-Version: 1.0.4
+Version: 1.0.5
 Summary: Deep Client - a way to connect your favorite language with Deep
 Home-page: https://github.com/Lotos2021/deepclient-test
 License: Unlicense
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deepclient-test-1.0.4/setup.py` & `deepclient-test-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="deepclient-test",
-    version="1.0.4",
+    version="1.0.5",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.8.4",
         "aiosignal==1.3.1",
         "async-timeout==4.0.2",
         "backoff==2.2.1",
         "botocore==1.29.129",
```

### Comparing `deepclient-test-1.0.4/tests/test_deep_client.py` & `deepclient-test-1.0.5/tests/test_deep_client.py`

 * *Files identical despite different names*

