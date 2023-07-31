# Comparing `tmp/amqp-mock-0.4.0.tar.gz` & `tmp/amqp-mock-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mock-0.4.0.tar", last modified: Thu Jun  9 15:37:49 2022, max compression
+gzip compressed data, was "amqp-mock-0.5.0.tar", last modified: Mon Jul 31 17:24:18 2023, max compression
```

## Comparing `amqp-mock-0.4.0.tar` & `amqp-mock-0.5.0.tar`

### file list

```diff
@@ -1,37 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6396 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.674281 amqp-mock-0.4.0/amqp_mock/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/_mock_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3219 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/_mock_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2648 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/amqp_mock/amqp_server/
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/amqp_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12935 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     3676 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_site.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/amqp_mock/http_server/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/http_server/_http_route.py
--rw-r--r--   0 runner    (1001) docker     (121)     2315 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/http_server/_http_server.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/amqp_mock/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/amqp_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-06-09 15:37:49.000000 amqp-mock-0.4.0/amqp_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-06-09 15:37:49.000000 amqp-mock-0.4.0/amqp_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 15:37:49.000000 amqp-mock-0.4.0/amqp_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-09 15:37:49.000000 amqp-mock-0.4.0/amqp_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 15:37:49.000000 amqp-mock-0.4.0/amqp_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.674281 amqp-mock-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:49.678281 amqp-mock-0.4.0/tests/_test_utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/tests/_test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4984 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/tests/_test_utils/amqp_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/tests/_test_utils/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/tests/_test_utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-06-09 15:37:36.000000 amqp-mock-0.4.0/tests/_test_utils/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_mock_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/amqp_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock/http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/_http_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/http_server/_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/amqp_mock/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.280056 amqp-mock-0.5.0/amqp_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 17:24:18.000000 amqp-mock-0.5.0/amqp_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:18.284056 amqp-mock-0.5.0/tests/_test_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/amqp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/_test_utils/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_delete_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_get_exchange_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_get_queue_message_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_publish_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 17:24:05.000000 amqp-mock-0.5.0/tests/test_reset.py
```

### Comparing `amqp-mock-0.4.0/LICENSE.txt` & `amqp-mock-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/PKG-INFO` & `amqp-mock-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.4.0
+Version: 0.5.0
 Summary: Remote AMQP mock
-Home-page: https://github.com/nikitanovosibirsk/amqp-mock
+Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # AMQP Mock
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/amqp-mock)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/amqp-mock)
 [![PyPI](https://img.shields.io/pypi/v/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/amqp-mock?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![Python Version](https://img.shields.io/pypi/pyversions/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 
 * [Installation](#installation)
 * [Overview](#overview)
   * [Test Publishing](#test-publishing)
@@ -54,15 +55,15 @@
     publish_message([1, 2, 3], "exchange")
 
     # 3. Test message has been published
     messages = await mock.client.get_exchange_messages("exchange")
     assert messages[0].value == [1, 2, 3]
 ```
 
-Full code available here: [`./examples/publish_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/publish_example.py)
+Full code available here: [`./examples/publish_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/publish_example.py)
 
 ### Test Consuming
 
 ```python
 from amqp_mock import create_amqp_mock, Message, MessageStatus
 
 # 1. Start AMQP mock server
@@ -74,15 +75,15 @@
     consume_message("queue")
 
     # 4. Test message has been consumed
     history = await mock.client.get_queue_message_history("queue")
     assert history[0].status == MessageStatus.ACKED
 ```
 
-Full code available here: [`./examples/consume_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/consume_example.py)
+Full code available here: [`./examples/consume_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/consume_example.py)
 
 ## Mock Server
 
 ### Start server
 
 ```python
 import asyncio
@@ -99,15 +100,15 @@
 
 asyncio.run(run())
 ```
 
 or via docker
 
 ```shell
-docker run -p 8080:80 -p 5672:5672 nikitanovosibirsk/amqp-mock
+docker run -p 8080:80 -p 5672:5672 tsv1/amqp-mock
 ```
 
 ### Publish message
 
 `POST /queues/{queue}/messages`
 
 ```js
```

### Comparing `amqp-mock-0.4.0/README.md` & `amqp-mock-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # AMQP Mock
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/amqp-mock)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/amqp-mock)
 [![PyPI](https://img.shields.io/pypi/v/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/amqp-mock?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![Python Version](https://img.shields.io/pypi/pyversions/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 
 * [Installation](#installation)
 * [Overview](#overview)
   * [Test Publishing](#test-publishing)
@@ -36,15 +36,15 @@
     publish_message([1, 2, 3], "exchange")
 
     # 3. Test message has been published
     messages = await mock.client.get_exchange_messages("exchange")
     assert messages[0].value == [1, 2, 3]
 ```
 
-Full code available here: [`./examples/publish_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/publish_example.py)
+Full code available here: [`./examples/publish_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/publish_example.py)
 
 ### Test Consuming
 
 ```python
 from amqp_mock import create_amqp_mock, Message, MessageStatus
 
 # 1. Start AMQP mock server
@@ -56,15 +56,15 @@
     consume_message("queue")
 
     # 4. Test message has been consumed
     history = await mock.client.get_queue_message_history("queue")
     assert history[0].status == MessageStatus.ACKED
 ```
 
-Full code available here: [`./examples/consume_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/consume_example.py)
+Full code available here: [`./examples/consume_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/consume_example.py)
 
 ## Mock Server
 
 ### Start server
 
 ```python
 import asyncio
@@ -81,15 +81,15 @@
 
 asyncio.run(run())
 ```
 
 or via docker
 
 ```shell
-docker run -p 8080:80 -p 5672:5672 nikitanovosibirsk/amqp-mock
+docker run -p 8080:80 -p 5672:5672 tsv1/amqp-mock
 ```
 
 ### Publish message
 
 `POST /queues/{queue}/messages`
 
 ```js
```

### Comparing `amqp-mock-0.4.0/amqp_mock/__init__.py` & `amqp-mock-0.5.0/amqp_mock/__init__.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/_message.py` & `amqp-mock-0.5.0/amqp_mock/_message.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/_mock_client.py` & `amqp-mock-0.5.0/amqp_mock/_mock_client.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/_mock_server.py` & `amqp-mock-0.5.0/amqp_mock/_mock_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/_storage.py` & `amqp-mock-0.5.0/amqp_mock/_storage.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_connection.py` & `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import logging
 from asyncio import CancelledError, Task, create_task, gather
 from asyncio.streams import StreamReader, StreamWriter
 from typing import Any, AsyncGenerator, Awaitable, Callable, Dict, Optional, Tuple, Union
 
 from pamqp import base, commands
 from pamqp.body import ContentBody
+from pamqp.constants import FRAME_END
 from pamqp.exceptions import UnmarshalingException
-from pamqp.frame import marshal, unmarshal
+from pamqp.frame import FrameTypes, marshal, unmarshal
 from pamqp.header import ContentHeader, ProtocolHeader
 from pamqp.heartbeat import Heartbeat
 
 from .._message import Message
 
 __all__ = ("AmqpConnection",)
 
@@ -95,23 +96,34 @@
 
         self._stream_reader.feed_eof()
         await self._reader
 
         if self._on_close:
             await self._on_close(self)
 
+    async def _unmarshal(self, buffer: bytes) -> Tuple[int, int, FrameTypes]:
+        # Workaround for pamqp bug:
+        #   Heartbeat can be unmarshaled successfully even without FRAME_END.
+        #   this shouldn't happen according to spec
+
+        byte_count, channel_id, frame = unmarshal(buffer)
+        if frame.name == Heartbeat.name and buffer[-1] != FRAME_END:
+            raise UnmarshalingException()
+
+        return byte_count, channel_id, frame
+
     async def _reader_task(self, reader: StreamReader) -> None:
         buffer = b""
         while not reader.at_eof():
             chunk = await reader.read(1)
             if not chunk:
                 break
             buffer += chunk
             try:
-                byte_count, channel_id, frame = unmarshal(buffer)
+                byte_count, channel_id, frame = await self._unmarshal(buffer)
             except UnmarshalingException:
                 continue
             else:
                 buffer = b""
 
             _logger.debug(f"<- {frame.name} {channel_id}")
             await self.dispatch_frame(frame, channel_id)
@@ -138,15 +150,15 @@
             header = ContentHeader(body_size=len(encoded), properties=properties)
             body = ContentBody(encoded)
             await self._send_frame(channel_id, header)
             await self._send_frame(channel_id, body)
 
     async def dispatch_frame(self, frame: AnyFrame, channel_id: int) -> Any:
         handlers: Dict[str, Callable[[int, Any], Any]] = {
-            Heartbeat.name: self._do_nothing,
+            Heartbeat.name: self._send_heartbeat,
             ProtocolHeader.name: self._send_connection_start,
             ContentHeader.name: self._handle_content_header,
             ContentBody.name: self._handle_content_body,
             commands.Connection.StartOk.name: self._send_connection_tune,
             commands.Connection.TuneOk.name: self._do_nothing,
             commands.Connection.Open.name: self._send_connection_open_ok,
             commands.Connection.Close.name: self._send_connection_close_ok,
@@ -170,15 +182,15 @@
 
     async def _send_frame(self, channel_id: int, frame: AnyFrame) -> None:
         _logger.debug(f"-> {frame.name}")
         self._stream_writer.write(bytes(marshal(frame, channel_id)))
         await self._stream_writer.drain()
 
     async def _do_nothing(self, channel_id: int, frame_in: AnyFrame) -> None:
-        _logger.debug("-> DoNothing")
+        _logger.debug(f"-> DoNothing with {frame_in} on {channel_id}")
 
     async def _send_connection_start(self, channel_id: int, frame_in: base.Frame) -> None:
         frame_out = commands.Connection.Start(
             version_major=0,
             version_minor=9,
             server_properties=self._server_properties,
             mechanisms="PLAIN",
@@ -187,14 +199,19 @@
         return await self._send_frame(channel_id, frame_out)
 
     async def _send_connection_tune(self, channel_id: int,
                                     frame_in: commands.Connection.StartOk) -> None:
         frame_out = commands.Connection.Tune(channel_max=0, frame_max=0, heartbeat=0)
         return await self._send_frame(channel_id, frame_out)
 
+    async def _send_heartbeat(self, channel_id: int, frame_in: AnyFrame) -> None:
+        frame_out = Heartbeat()
+        await self._send_frame(channel_id, frame_out)
+        _logger.debug(f"-> Send heartbeat in response with {frame_in} on {channel_id}")
+
     async def _send_connection_open_ok(self, channel_id: int,
                                        frame_in: commands.Connection.Open) -> None:
         frame_out = commands.Connection.OpenOk()
         await self._send_frame(channel_id, frame_out)
 
     async def _send_channel_open_ok(self, channel_id: int,
                                     frame_in: commands.Channel.Open) -> None:
```

### Comparing `amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_server.py` & `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/amqp_server/_amqp_site.py` & `amqp-mock-0.5.0/amqp_mock/amqp_server/_amqp_site.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,9 +22,10 @@
     async def start(self) -> None:
         await super().start()
         callback = cast(Callable[[StreamReader, StreamWriter], Any], self._runner.server)
         self._server = await start_server(callback, host=self._host, port=self._port)
         if self._server.sockets is not None and len(self._server.sockets) > 0:
             self._port = self._server.sockets[0].getsockname()[1]
 
+    @property
     def name(self) -> str:
-        return "ampq://{host}:{port}".format(host=self._host, port=self._port)
+        return "amqp://{host}:{port}".format(host=self._host, port=self._port)
```

### Comparing `amqp-mock-0.4.0/amqp_mock/http_server/_http_route.py` & `amqp-mock-0.5.0/amqp_mock/http_server/_http_route.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock/http_server/_http_server.py` & `amqp-mock-0.5.0/amqp_mock/http_server/_http_server.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/amqp_mock.egg-info/PKG-INFO` & `amqp-mock-0.5.0/amqp_mock.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: amqp-mock
-Version: 0.4.0
+Version: 0.5.0
 Summary: Remote AMQP mock
-Home-page: https://github.com/nikitanovosibirsk/amqp-mock
+Home-page: https://github.com/tsv1/amqp-mock
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # AMQP Mock
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/amqp-mock)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/amqp-mock/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/amqp-mock)
 [![PyPI](https://img.shields.io/pypi/v/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/amqp-mock?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 [![Python Version](https://img.shields.io/pypi/pyversions/amqp-mock.svg?style=flat-square)](https://pypi.python.org/pypi/amqp-mock)
 
 * [Installation](#installation)
 * [Overview](#overview)
   * [Test Publishing](#test-publishing)
@@ -54,15 +55,15 @@
     publish_message([1, 2, 3], "exchange")
 
     # 3. Test message has been published
     messages = await mock.client.get_exchange_messages("exchange")
     assert messages[0].value == [1, 2, 3]
 ```
 
-Full code available here: [`./examples/publish_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/publish_example.py)
+Full code available here: [`./examples/publish_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/publish_example.py)
 
 ### Test Consuming
 
 ```python
 from amqp_mock import create_amqp_mock, Message, MessageStatus
 
 # 1. Start AMQP mock server
@@ -74,15 +75,15 @@
     consume_message("queue")
 
     # 4. Test message has been consumed
     history = await mock.client.get_queue_message_history("queue")
     assert history[0].status == MessageStatus.ACKED
 ```
 
-Full code available here: [`./examples/consume_example.py`](https://github.com/nikitanovosibirsk/amqp-mock/blob/master/examples/consume_example.py)
+Full code available here: [`./examples/consume_example.py`](https://github.com/tsv1/amqp-mock/blob/master/examples/consume_example.py)
 
 ## Mock Server
 
 ### Start server
 
 ```python
 import asyncio
@@ -99,15 +100,15 @@
 
 asyncio.run(run())
 ```
 
 or via docker
 
 ```shell
-docker run -p 8080:80 -p 5672:5672 nikitanovosibirsk/amqp-mock
+docker run -p 8080:80 -p 5672:5672 tsv1/amqp-mock
 ```
 
 ### Publish message
 
 `POST /queues/{queue}/messages`
 
 ```js
```

### Comparing `amqp-mock-0.4.0/amqp_mock.egg-info/SOURCES.txt` & `amqp-mock-0.5.0/amqp_mock.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -18,12 +18,21 @@
 amqp_mock/amqp_server/_amqp_connection.py
 amqp_mock/amqp_server/_amqp_runner.py
 amqp_mock/amqp_server/_amqp_server.py
 amqp_mock/amqp_server/_amqp_site.py
 amqp_mock/http_server/__init__.py
 amqp_mock/http_server/_http_route.py
 amqp_mock/http_server/_http_server.py
+tests/test_basics.py
+tests/test_context_manager.py
+tests/test_delete_exchange_messages.py
+tests/test_get_exchange_messages.py
+tests/test_get_queue_message_history.py
+tests/test_healthcheck.py
+tests/test_publish_message.py
+tests/test_repr.py
+tests/test_reset.py
 tests/_test_utils/__init__.py
 tests/_test_utils/amqp_client.py
 tests/_test_utils/fixtures.py
 tests/_test_utils/helpers.py
 tests/_test_utils/steps.py
```

### Comparing `amqp-mock-0.4.0/setup.cfg` & `amqp-mock-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.4.0
+current_version = 0.5.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `amqp-mock-0.4.0/setup.py` & `amqp-mock-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="amqp-mock",
-    version="0.4.0",
+    version="0.5.0",
     description="Remote AMQP mock",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7.0",
-    url="https://github.com/nikitanovosibirsk/amqp-mock",
+    url="https://github.com/tsv1/amqp-mock",
     license="Apache-2.0",
     packages=find_packages(exclude=("tests",)),
     package_data={"amqp_mock": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

### Comparing `amqp-mock-0.4.0/tests/_test_utils/amqp_client.py` & `amqp-mock-0.5.0/tests/_test_utils/amqp_client.py`

 * *Files identical despite different names*

### Comparing `amqp-mock-0.4.0/tests/_test_utils/fixtures.py` & `amqp-mock-0.5.0/tests/_test_utils/fixtures.py`

 * *Files identical despite different names*

