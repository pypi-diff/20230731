# Comparing `tmp/amqp-mock-0.5.0.tar.gz` & `tmp/amqp-mock-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mock-0.5.0.tar", last modified: Mon Jul 31 17:24:18 2023, max compression
+gzip compressed data, was "amqp-mock-0.5.1.tar", last modified: Mon Jul 31 17:26:45 2023, max compression
```

## Comparing `amqp-mock-0.5.0.tar` & `amqp-mock-0.5.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_mock_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/amqp_server/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/http_server/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/_http_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/_http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/tests/_test_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/amqp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_delete_exchange_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_get_exchange_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_get_queue_message_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_publish_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_reset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.468674 amqp-mock-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:26:45.468674 amqp-mock-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.464674 amqp-mock-0.5.1/amqp_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/_mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.464674 amqp-mock-0.5.1/amqp_mock/amqp_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/amqp_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.464674 amqp-mock-0.5.1/amqp_mock/http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/http_server/_http_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/http_server/_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/amqp_mock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.464674 amqp-mock-0.5.1/amqp_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:26:45.000000 amqp-mock-0.5.1/amqp_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 17:26:45.000000 amqp-mock-0.5.1/amqp_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:26:45.000000 amqp-mock-0.5.1/amqp_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 17:26:45.000000 amqp-mock-0.5.1/amqp_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 17:26:45.000000 amqp-mock-0.5.1/amqp_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-31 17:26:45.468674 amqp-mock-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.468674 amqp-mock-0.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:45.468674 amqp-mock-0.5.1/tests/_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/_test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/_test_utils/amqp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/_test_utils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/_test_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/_test_utils/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_delete_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_get_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_get_queue_message_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_publish_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 17:26:25.000000 amqp-mock-0.5.1/tests/test_reset.py
```

### Comparing `amqp-mock-0.5.0/LICENSE.txt` & `amqp-mock-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/PKG-INFO` & `amqp-mock-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.5.0
+Version: 0.5.1
 Summary: Remote AMQP mock
 Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `amqp-mock-0.5.0/README.md` & `amqp-mock-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/__init__.py` & `amqp-mock-0.5.1/amqp_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/_message.py` & `amqp-mock-0.5.1/amqp_mock/_message.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/_mock_client.py` & `amqp-mock-0.5.1/amqp_mock/_mock_client.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/_mock_server.py` & `amqp-mock-0.5.1/amqp_mock/_mock_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/_storage.py` & `amqp-mock-0.5.1/amqp_mock/_storage.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_connection.py` & `amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_connection.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_server.py` & `amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_site.py` & `amqp-mock-0.5.1/amqp_mock/amqp_server/_amqp_site.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/http_server/_http_route.py` & `amqp-mock-0.5.1/amqp_mock/http_server/_http_route.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock/http_server/_http_server.py` & `amqp-mock-0.5.1/amqp_mock/http_server/_http_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/amqp_mock.egg-info/PKG-INFO` & `amqp-mock-0.5.1/amqp_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.5.0
+Version: 0.5.1
 Summary: Remote AMQP mock
 Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `amqp-mock-0.5.0/amqp_mock.egg-info/SOURCES.txt` & `amqp-mock-0.5.1/amqp_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/setup.cfg` & `amqp-mock-0.5.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.0
+current_version = 0.5.1
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `amqp-mock-0.5.0/setup.py` & `amqp-mock-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="amqp-mock",
-    version="0.5.0",
+    version="0.5.1",
     description="Remote AMQP mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7.0",
     url="https://github.com/tsv1/amqp-mock",
```

### Comparing `amqp-mock-0.5.0/tests/_test_utils/amqp_client.py` & `amqp-mock-0.5.1/tests/_test_utils/amqp_client.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/_test_utils/fixtures.py` & `amqp-mock-0.5.1/tests/_test_utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_basics.py` & `amqp-mock-0.5.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_context_manager.py` & `amqp-mock-0.5.1/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_delete_exchange_messages.py` & `amqp-mock-0.5.1/tests/test_delete_exchange_messages.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_get_exchange_messages.py` & `amqp-mock-0.5.1/tests/test_get_exchange_messages.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_get_queue_message_history.py` & `amqp-mock-0.5.1/tests/test_get_queue_message_history.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_healthcheck.py` & `amqp-mock-0.5.1/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_publish_message.py` & `amqp-mock-0.5.1/tests/test_publish_message.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_repr.py` & `amqp-mock-0.5.1/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.5.0/tests/test_reset.py` & `amqp-mock-0.5.1/tests/test_reset.py`

 * *Files identical despite different names*

