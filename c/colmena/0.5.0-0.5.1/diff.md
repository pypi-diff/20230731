# Comparing `tmp/colmena-0.5.0.tar.gz` & `tmp/colmena-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colmena-0.5.0.tar", last modified: Mon May 15 11:53:29 2023, max compression
+gzip compressed data, was "colmena-0.5.1.tar", last modified: Mon Jul 31 19:46:24 2023, max compression
```

## Comparing `colmena-0.5.0.tar` & `colmena-0.5.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-05-15 11:53:21.000000 colmena-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 11:53:29.131730 colmena-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-05-15 11:53:21.000000 colmena-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena/queue/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/queue/tests/test_queues.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/task_server/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/task_server/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/task_server/tests/test_parsl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/tests/test_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/thinker/
--rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.131730 colmena-0.5.0/colmena/thinker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/tests/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/thinker/tests/test_thinker.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-15 11:53:21.000000 colmena-0.5.0/colmena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:53:29.127730 colmena-0.5.0/colmena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 11:53:29.000000 colmena-0.5.0/colmena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-15 11:53:21.000000 colmena-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:53:29.131730 colmena-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.746586 colmena-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-31 19:46:16.000000 colmena-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-31 19:46:24.746586 colmena-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-31 19:46:16.000000 colmena-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/queue/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/queue/tests/test_queues.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/task_server/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/task_server/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/tests/test_globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/task_server/tests/test_parsl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/tests/test_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/thinker/
+-rw-r--r--   0 runner    (1001) docker     (123)    19328 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/thinker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13241 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/thinker/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena/thinker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/thinker/tests/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/thinker/tests/test_thinker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-31 19:46:16.000000 colmena-0.5.1/colmena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:46:24.742586 colmena-0.5.1/colmena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-31 19:46:24.000000 colmena-0.5.1/colmena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-31 19:46:24.000000 colmena-0.5.1/colmena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:46:24.000000 colmena-0.5.1/colmena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-31 19:46:24.000000 colmena-0.5.1/colmena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 19:46:24.000000 colmena-0.5.1/colmena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-31 19:46:16.000000 colmena-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:46:24.746586 colmena-0.5.1/setup.cfg
```

### Comparing `colmena-0.5.0/LICENSE.txt` & `colmena-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/PKG-INFO` & `colmena-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.5.0
+Version: 0.5.1
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,15 +213,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: globus
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Colmena
```

### Comparing `colmena-0.5.0/README.md` & `colmena-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/models.py` & `colmena-0.5.1/colmena/models.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/proxy.py` & `colmena-0.5.1/colmena/proxy.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/queue/base.py` & `colmena-0.5.1/colmena/queue/base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/queue/python.py` & `colmena-0.5.1/colmena/queue/python.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/queue/redis.py` & `colmena-0.5.1/colmena/queue/redis.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/queue/tests/test_base.py` & `colmena-0.5.1/colmena/queue/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/queue/tests/test_queues.py` & `colmena-0.5.1/colmena/queue/tests/test_queues.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,33 @@
 """Tests across different queue implementations"""
 from multiprocessing import Pool
 
 from pytest import fixture, raises, mark
+from redis import Redis, ConnectionError
 
 from colmena.exceptions import TimeoutException, KillSignalException
 from colmena.queue.base import ColmenaQueues
 from colmena.queue.python import PipeQueues
 from colmena.queue.redis import RedisQueues
 
+# Determine which classes to test
 
-@fixture(params=[PipeQueues, RedisQueues])
+has_redis = True
+try:
+    client = Redis()
+    client.ping()
+except ConnectionError:
+    has_redis = False
+
+to_test = [PipeQueues]
+if has_redis:
+    to_test.append(RedisQueues)
+
+
+@fixture(params=to_test)
 def queue(request) -> ColmenaQueues:
     return request.param(['a', 'b'])
 
 
 def test_topics(queue):
     assert queue.topics == {'default', 'a', 'b'}
```

### Comparing `colmena-0.5.0/colmena/task_server/base.py` & `colmena-0.5.1/colmena/task_server/base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/task_server/globus.py` & `colmena-0.5.1/colmena/task_server/globus.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/task_server/parsl.py` & `colmena-0.5.1/colmena/task_server/parsl.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/task_server/tests/test_base.py` & `colmena-0.5.1/colmena/task_server/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/task_server/tests/test_globus.py` & `colmena-0.5.1/colmena/task_server/tests/test_globus.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/task_server/tests/test_parsl.py` & `colmena-0.5.1/colmena/task_server/tests/test_parsl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests for the Parsl implementation of the task server"""
 from typing import Tuple, List
 
 from parsl import HighThroughputExecutor
 from parsl.config import Config
+from proxystore.connectors.file import FileConnector
 from pytest import fixture, mark
 
-from proxystore.connectors.redis import RedisConnector
 from proxystore.store import Store
 from proxystore.store import register_store
 from proxystore.store import unregister_store
 
 from colmena.queue.base import ColmenaQueues
 
 from colmena.queue.python import PipeQueues
@@ -35,25 +35,25 @@
 
 
 # Make the Parsl configuration. Use LocalThreads for Mac and Windows compatibility
 @fixture()
 def config(tmpdir):
     return Config(
         executors=[
-            HighThroughputExecutor(max_workers=1, address='localhost')
+            HighThroughputExecutor(max_workers=1)
         ],
         strategy=None,
-        run_dir=str(tmpdir),
+        run_dir=str(tmpdir / 'run'),
     )
 
 
 # Make a proxy store for larger objects
-@fixture(scope='module')
-def store():
-    connector = RedisConnector(hostname='localhost', port=6379)
+@fixture()
+def store(tmpdir):
+    connector = FileConnector(store_dir=str(tmpdir / 'proxy-store'))
     with Store('store', connector=connector, metrics=True) as store:
         register_store(store)
         yield store
         unregister_store(store.name)
 
 
 @fixture(autouse=True)
```

### Comparing `colmena-0.5.0/colmena/tests/test_model.py` & `colmena-0.5.1/colmena/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/tests/test_proxy.py` & `colmena-0.5.1/colmena/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/thinker/__init__.py` & `colmena-0.5.1/colmena/thinker/__init__.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/thinker/resources.py` & `colmena-0.5.1/colmena/thinker/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
             def _function():
                 self.reallocate(task_from, task_to, n_slots, block=True, timeout=timeout, cancel_if=cancel_if)
                 if callback is not None:
                     callback()
 
             thr = Thread(target=_function, daemon=True)
             thr.start()
-            assert thr.is_alive(), thr.join()
             return True
 
         # Pull nodes from the remaining
         with self._allocation_lock[task_from]:
             if n_slots == "all":
                 n_slots = self.allocated_slots(task_from)
             acq_success = self.acquire(task_from, n_slots, timeout, cancel_if)
```

### Comparing `colmena-0.5.0/colmena/thinker/tests/test_resources.py` & `colmena-0.5.1/colmena/thinker/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena/thinker/tests/test_thinker.py` & `colmena-0.5.1/colmena/thinker/tests/test_thinker.py`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/colmena.egg-info/PKG-INFO` & `colmena-0.5.1/colmena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colmena
-Version: 0.5.0
+Version: 0.5.1
 Summary: colmena: Intelligent Steerable Pipelines on HPC
 Author-email: Globus Labs <labs@globus.org>, Logan Ward <lward@anl.gov>, Greg Pauloski <jgpauloski@uchicago.edu>, Yadu Babuji <yadudoc1729@gmail.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -213,15 +213,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: globus
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # Colmena
```

### Comparing `colmena-0.5.0/colmena.egg-info/SOURCES.txt` & `colmena-0.5.1/colmena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colmena-0.5.0/pyproject.toml` & `colmena-0.5.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "colmena"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
     { name = "Globus Labs", email = "labs@globus.org" },
     { name = "Logan Ward", email = "lward@anl.gov" },
     { name = "Greg Pauloski", email = "jgpauloski@uchicago.edu" },
     { name = "Yadu Babuji", email = "yadudoc1729@gmail.com" },
 ]
 description = 'colmena: Intelligent Steerable Pipelines on HPC'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { file = "LICENSE.txt" }
 keywords = ["HPC", "AI", "Workflows"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

