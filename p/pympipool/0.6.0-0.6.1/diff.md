# Comparing `tmp/pympipool-0.6.0.tar.gz` & `tmp/pympipool-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.6.0.tar", last modified: Sun Jul 30 15:42:18 2023, max compression
+gzip compressed data, was "pympipool-0.6.1.tar", last modified: Mon Jul 31 01:02:59 2023, max compression
```

## Comparing `pympipool-0.6.0.tar` & `pympipool-0.6.1.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-30 15:42:15.000000 pympipool-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-30 15:42:15.000000 pympipool-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-30 15:42:18.830976 pympipool-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-30 15:42:15.000000 pympipool-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/backend/mpiexec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/taskbroker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/interfaces/taskexecutor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/backend/mpipool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/interfaces/pool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool/legacy/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/legacy/shared/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/taskexecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-30 15:42:15.000000 pympipool-0.6.0/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.826976 pympipool-0.6.0/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-30 15:42:18.000000 pympipool-0.6.0/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-30 15:42:18.830976 pympipool-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-30 15:42:18.000000 pympipool-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 15:42:18.830976 pympipool-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_communicator_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_future.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_parse_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_worker_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-30 15:42:15.000000 pympipool-0.6.0/tests/test_zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-30 15:42:15.000000 pympipool-0.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-31 01:02:53.000000 pympipool-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 01:02:53.000000 pympipool-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-31 01:02:59.159087 pympipool-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-07-31 01:02:53.000000 pympipool-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/backend/mpiexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/fluxbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/taskbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/interfaces/taskexecutor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/backend/mpipool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8788 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/interfaces/pool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool/legacy/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/legacy/shared/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/taskexecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-31 01:02:53.000000 pympipool-0.6.1/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.155087 pympipool-0.6.1/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 01:02:59.000000 pympipool-0.6.1/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 01:02:59.159087 pympipool-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-31 01:02:58.000000 pympipool-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:02:59.159087 pympipool-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_communicator_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_parse_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_worker_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-31 01:02:53.000000 pympipool-0.6.1/tests/test_zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-31 01:02:53.000000 pympipool-0.6.1/versioneer.py
```

### Comparing `pympipool-0.6.0/LICENSE` & `pympipool-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/PKG-INFO` & `pympipool-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.6.0
+Version: 0.6.1
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.6.0/README.md` & `pympipool-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/__init__.py` & `pympipool-0.6.1/pympipool/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     interface_connect,
     interface_bootup,
     interface_send,
     interface_shutdown,
     interface_receive,
 )
 from pympipool.interfaces.taskbroker import HPCExecutor
+from pympipool.interfaces.fluxbroker import PyFluxExecutor
 from pympipool.interfaces.taskexecutor import Executor
 from pympipool.legacy.interfaces.executor import PoolExecutor
 from pympipool.legacy.interfaces.pool import Pool, MPISpawnPool
 from pympipool.shared.thread import RaisingThread
 from pympipool.shared.taskexecutor import cancel_items_in_queue
 
 from ._version import get_versions
```

### Comparing `pympipool-0.6.0/pympipool/backend/mpiexec.py` & `pympipool-0.6.1/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/interfaces/taskbroker.py` & `pympipool-0.6.1/pympipool/legacy/interfaces/executor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-from concurrent.futures import Executor as FutureExecutor, Future
-import queue
-
+from pympipool.interfaces.base import ExecutorBase
 from pympipool.shared.thread import RaisingThread
-from pympipool.shared.broker import executor_broker
-from pympipool.shared.taskexecutor import cancel_items_in_queue
+from pympipool.legacy.shared.interface import execute_serial_tasks
+from pympipool.shared.taskexecutor import cloudpickle_register
+
 
+class PoolExecutor(ExecutorBase):
+    """
+    To combine the functionality of the pympipool.Pool and the pympipool.Executor the pympipool.PoolExecutor again
+    connects to the mpi4py.futures.MPIPoolExecutor. Still in contrast to the pympipool.Pool it does not implement the
+    map() and starmap() functions but rather the submit() function based on the concurrent.futures.Executor interface.
+    In this case the load balancing happens internally and the maximum number of workers max_workers defines the maximum
+    number of parallel tasks. But only serial python tasks can be executed in contrast to the pympipool.Executor which
+    can also execute MPI parallel python tasks.
+
+    Args:
+        max_workers (int): defines the total number of MPI ranks to use
+        gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
+        oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only) - default False
+        enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
+        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+        cwd (str/None): current working directory where the parallel python task is executed
+        sleep_interval (float):
+        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
+        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
+
+    Simple example:
+        ```
+        from pympipool import PoolExecutor
+
+        def calc(i, j):
+            return i + j
+
+        with PoolExecutor(max_workers=2) as p:
+            fs1 = p.submit(calc, 1, 2)
+            fs2 = p.submit(calc, 3, 4)
+            fs3 = p.submit(calc, 5, 6)
+            fs4 = p.submit(calc, 7, 8)
+            print(fs1.result(), fs2.result(), fs3.result(), fs4.result()
+        ```
+    """
 
-class HPCExecutor(FutureExecutor):
     def __init__(
         self,
-        max_workers,
-        cores_per_worker=1,
-        gpus_per_worker=0,
+        max_workers=1,
+        gpus_per_task=0,
         oversubscribe=False,
         enable_flux_backend=False,
         enable_slurm_backend=False,
-        init_function=None,
         cwd=None,
         sleep_interval=0.1,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
-        self._future_queue = queue.Queue()
+        super().__init__()
         self._process = RaisingThread(
-            target=executor_broker,
+            target=execute_serial_tasks,
             kwargs={
                 "future_queue": self._future_queue,
-                "max_workers": max_workers,
-                "cores_per_worker": cores_per_worker,
-                "gpus_per_worker": gpus_per_worker,
+                "cores": max_workers,
+                "gpus_per_task": gpus_per_task,
                 "oversubscribe": oversubscribe,
                 "enable_flux_backend": enable_flux_backend,
                 "enable_slurm_backend": enable_slurm_backend,
-                "init_function": init_function,
                 "cwd": cwd,
                 "sleep_interval": sleep_interval,
                 "queue_adapter": queue_adapter,
                 "queue_adapter_kwargs": queue_adapter_kwargs,
             },
         )
         self._process.start()
-
-    def submit(self, fn, *args, **kwargs):
-        """Submits a callable to be executed with the given arguments.
-
-        Schedules the callable to be executed as fn(*args, **kwargs) and returns
-        a Future instance representing the execution of the callable.
-
-        Returns:
-            A Future representing the given call.
-        """
-        f = Future()
-        self._future_queue.put({"fn": fn, "args": args, "kwargs": kwargs, "future": f})
-        return f
-
-    def shutdown(self, wait=True, *, cancel_futures=False):
-        """Clean-up the resources associated with the Executor.
-
-        It is safe to call this method several times. Otherwise, no other
-        methods can be called after this one.
-
-        Args:
-            wait: If True then shutdown will not return until all running
-                futures have finished executing and the resources used by the
-                parallel_executors have been reclaimed.
-            cancel_futures: If True then shutdown will cancel all pending
-                futures. Futures that are completed or running will not be
-                cancelled.
-        """
-        if cancel_futures:
-            cancel_items_in_queue(que=self._future_queue)
-        self._future_queue.put({"shutdown": True, "wait": wait})
-        self._process.join()
+        cloudpickle_register(ind=3)
```

### Comparing `pympipool-0.6.0/pympipool/legacy/backend/mpipool.py` & `pympipool-0.6.1/pympipool/legacy/backend/mpipool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/legacy/interfaces/executor.py` & `pympipool-0.6.1/pympipool/interfaces/taskexecutor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-from pympipool.interfaces.taskexecutor import ExecutorBase
+from pympipool.interfaces.base import ExecutorBase
 from pympipool.shared.thread import RaisingThread
-from pympipool.legacy.shared.interface import execute_serial_tasks
+from pympipool.shared.taskexecutor import (
+    execute_parallel_tasks,
+    cloudpickle_register,
+)
 
 
-class PoolExecutor(ExecutorBase):
+class Executor(ExecutorBase):
     """
-    To combine the functionality of the pympipool.Pool and the pympipool.Executor the pympipool.PoolExecutor again
-    connects to the mpi4py.futures.MPIPoolExecutor. Still in contrast to the pympipool.Pool it does not implement the
-    map() and starmap() functions but rather the submit() function based on the concurrent.futures.Executor interface.
-    In this case the load balancing happens internally and the maximum number of workers max_workers defines the maximum
-    number of parallel tasks. But only serial python tasks can be executed in contrast to the pympipool.Executor which
-    can also execute MPI parallel python tasks.
+    The pympipool.Executor behaves like the concurrent.futures.Executor but it uses mpi4py to execute parallel tasks.
+    In contrast to the mpi4py.futures.MPIPoolExecutor the pympipool.Executor can be executed in a serial python process
+    and does not require the python script to be executed with MPI. Still internally the pympipool.Executor uses the
+    mpi4py.futures.MPIPoolExecutor, consequently it is primarily an abstraction of its functionality to improve the
+    usability in particular when used in combination with Jupyter notebooks.
 
     Args:
-        max_workers (int): defines the total number of MPI ranks to use
+        cores (int): defines the number of MPI ranks to use for each function call
         gpus_per_task (int): number of GPUs per MPI rank - defaults to 0
         oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI only) - default False
         enable_flux_backend (bool): use the flux-framework as backend rather than just calling mpiexec
         enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
+        init_function (None): optional function to preset arguments for functions which are submitted later
         cwd (str/None): current working directory where the parallel python task is executed
-        sleep_interval (float):
         queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
         queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
 
     Simple example:
         ```
-        from pympipool import PoolExecutor
+        import numpy as np
+        from pympipool import Executor
 
-        def calc(i, j):
-            return i + j
+        def calc(i, j, k):
+            from mpi4py import MPI
+            size = MPI.COMM_WORLD.Get_size()
+            rank = MPI.COMM_WORLD.Get_rank()
+            return np.array([i, j, k]), size, rank
+
+        def init_k():
+            return {"k": 3}
+
+        with Executor(cores=2, init_function=init_k) as p:
+            fs = p.submit(calc, 2, j=4)
+            print(fs.result())
 
-        with PoolExecutor(max_workers=2) as p:
-            fs1 = p.submit(calc, 1, 2)
-            fs2 = p.submit(calc, 3, 4)
-            fs3 = p.submit(calc, 5, 6)
-            fs4 = p.submit(calc, 7, 8)
-            print(fs1.result(), fs2.result(), fs3.result(), fs4.result()
+        >>> [(array([2, 4, 3]), 2, 0), (array([2, 4, 3]), 2, 1)]
         ```
     """
 
     def __init__(
         self,
-        max_workers=1,
+        cores,
         gpus_per_task=0,
         oversubscribe=False,
         enable_flux_backend=False,
         enable_slurm_backend=False,
+        init_function=None,
         cwd=None,
-        sleep_interval=0.1,
         queue_adapter=None,
         queue_adapter_kwargs=None,
     ):
         super().__init__()
         self._process = RaisingThread(
-            target=execute_serial_tasks,
+            target=execute_parallel_tasks,
             kwargs={
                 "future_queue": self._future_queue,
-                "cores": max_workers,
+                "cores": cores,
                 "gpus_per_task": gpus_per_task,
                 "oversubscribe": oversubscribe,
                 "enable_flux_backend": enable_flux_backend,
                 "enable_slurm_backend": enable_slurm_backend,
                 "cwd": cwd,
-                "sleep_interval": sleep_interval,
                 "queue_adapter": queue_adapter,
                 "queue_adapter_kwargs": queue_adapter_kwargs,
             },
         )
         self._process.start()
+        if init_function is not None:
+            self._future_queue.put(
+                {"init": True, "fn": init_function, "args": (), "kwargs": {}}
+            )
+        cloudpickle_register(ind=3)
```

### Comparing `pympipool-0.6.0/pympipool/legacy/interfaces/pool.py` & `pympipool-0.6.1/pympipool/legacy/interfaces/pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/legacy/shared/backend.py` & `pympipool-0.6.1/pympipool/legacy/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/legacy/shared/interface.py` & `pympipool-0.6.1/pympipool/legacy/shared/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import queue
+import sys
 import time
 
 from pympipool.shared.communication import interface_bootup
 
 
 def execute_serial_tasks(
     future_queue,
@@ -53,20 +54,20 @@
 
 
 def get_pool_command(cores_total, ranks_per_task=1):
     executable = os.path.abspath(
         os.path.join(__file__, "..", "..", "backend", "mpipool.py")
     )
     if ranks_per_task == 1:
-        command_lst = ["python", "-m", "mpi4py.futures", executable]
+        command_lst = [sys.executable, "-m", "mpi4py.futures", executable]
         cores = cores_total
     else:
         # Running MPI parallel tasks within the map() requires mpi4py to use mpi spawn:
         # https://github.com/mpi4py/mpi4py/issues/324
-        command_lst = ["python", executable]
+        command_lst = [sys.executable, executable]
         cores = 1
     command_lst += [
         "--cores-per-task",
         str(ranks_per_task),
         "--cores-total",
         str(cores_total),
     ]
```

### Comparing `pympipool-0.6.0/pympipool/shared/backend.py` & `pympipool-0.6.1/pympipool/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/shared/broker.py` & `pympipool-0.6.1/pympipool/shared/broker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/shared/communication.py` & `pympipool-0.6.1/pympipool/shared/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool/shared/connections.py` & `pympipool-0.6.1/pympipool/shared/connections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC
+import os
 import subprocess
 
 
 class BaseInterface(ABC):
     def __init__(self, cwd, cores=1, gpus_per_core=0, oversubscribe=False):
         self._cwd = cwd
         self._cores = cores
@@ -167,29 +168,36 @@
         if self._oversubscribe:
             raise ValueError(
                 "Oversubscribing is currently not supported for the Flux adapter."
             )
         if self._executor is None:
             self._executor = flux.job.FluxExecutor()
         jobspec = flux.job.JobspecV1.from_command(
-            command=" ".join(command_lst),
-            num_tasks=1,
-            cores_per_task=self._cores,
+            command=command_lst,
+            num_tasks=self._cores,
+            cores_per_task=1,
             gpus_per_task=self._gpus_per_core,
             num_nodes=None,
             exclusive=False,
         )
-        jobspec.cwd = self._cwd
+        jobspec.environment = dict(os.environ)
+        if self._cwd is not None:
+            jobspec.cwd = self._cwd
         self._future = self._executor.submit(jobspec)
 
     def shutdown(self, wait=True):
-        self._executor.shutdown(wait=wait)
+        if self.poll():
+            self._future.cancel()
+        # The flux future objects are not instantly updated,
+        # still showing running after cancel was called,
+        # so we wait until the execution is completed.
+        self._future.result()
 
     def poll(self):
-        return self._executor is not None
+        return self._future is not None and not self._future.done()
 
 
 def generate_slurm_command(cores, cwd, gpus_per_core=0, oversubscribe=False):
     command_prepend_lst = ["srun", "-n", str(cores), "-D", cwd]
     if gpus_per_core > 0:
         command_prepend_lst += ["--gpus-per-task=" + str(gpus_per_core)]
     if oversubscribe:
```

### Comparing `pympipool-0.6.0/pympipool/shared/taskexecutor.py` & `pympipool-0.6.1/pympipool/shared/taskexecutor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import os
 import queue
+import sys
 
 import cloudpickle
 
 from pympipool.shared.communication import interface_bootup
 
 
 def cancel_items_in_queue(que):
@@ -67,15 +68,15 @@
        enable_flux_backend (bool): enable the flux-framework as backend - defaults to False
        enable_slurm_backend (bool): enable the SLURM queueing system as backend - defaults to False
        cwd (str/None): current working directory where the parallel python task is executed
        queue_adapter (pysqa.queueadapter.QueueAdapter): generalized interface to various queuing systems
        queue_adapter_kwargs (dict/None): keyword arguments for the submit_job() function of the queue adapter
     """
     command_lst = [
-        "python",
+        sys.executable,
         os.path.abspath(os.path.join(__file__, "..", "..", "backend", "mpiexec.py")),
     ]
     interface = interface_bootup(
         command_lst=command_lst,
         cwd=cwd,
         cores=cores,
         gpus_per_core=gpus_per_task,
```

### Comparing `pympipool-0.6.0/pympipool/shared/thread.py` & `pympipool-0.6.1/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/pympipool.egg-info/PKG-INFO` & `pympipool-0.6.1/pympipool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.6.0
+Version: 0.6.1
 Summary: pympipool - scale python functions over multiple compute nodes
 Home-page: https://github.com/jan-janssen/pympipool
 Author-email: jan.janssen@outlook.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pympipool-0.6.0/pympipool.egg-info/SOURCES.txt` & `pympipool-0.6.1/pympipool.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 pympipool.egg-info/SOURCES.txt
 pympipool.egg-info/dependency_links.txt
 pympipool.egg-info/requires.txt
 pympipool.egg-info/top_level.txt
 pympipool/backend/__init__.py
 pympipool/backend/mpiexec.py
 pympipool/interfaces/__init__.py
+pympipool/interfaces/base.py
+pympipool/interfaces/fluxbroker.py
 pympipool/interfaces/taskbroker.py
 pympipool/interfaces/taskexecutor.py
 pympipool/legacy/__init__.py
 pympipool/legacy/backend/__init__.py
 pympipool/legacy/backend/mpipool.py
 pympipool/legacy/interfaces/__init__.py
 pympipool/legacy/interfaces/executor.py
@@ -31,14 +33,15 @@
 pympipool/shared/communication.py
 pympipool/shared/connections.py
 pympipool/shared/taskexecutor.py
 pympipool/shared/thread.py
 tests/test_communicator_split.py
 tests/test_connection.py
 tests/test_executor.py
+tests/test_flux.py
 tests/test_future.py
 tests/test_interface.py
 tests/test_meta.py
 tests/test_multitask.py
 tests/test_parse.py
 tests/test_parse_legacy.py
 tests/test_pool.py
```

### Comparing `pympipool-0.6.0/setup.py` & `pympipool-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_communicator_split.py` & `pympipool-0.6.1/tests/test_communicator_split.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_connection.py` & `pympipool-0.6.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_executor.py` & `pympipool-0.6.1/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_future.py` & `pympipool-0.6.1/tests/test_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_interface.py` & `pympipool-0.6.1/tests/test_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 
 import numpy as np
 import unittest
 from pympipool.shared.communication import SocketInterface
 from pympipool.shared.taskexecutor import cloudpickle_register
 from pympipool.shared.connections import MpiExecInterface
 
@@ -20,14 +21,14 @@
                 cwd=None,
                 cores=1,
                 gpus_per_core=0,
                 oversubscribe=False
             )
         )
         interface.bootup(command_lst=[
-            "python",
+            sys.executable,
             os.path.abspath(os.path.join(__file__, "..", "..", "pympipool", "backend", "mpiexec.py")),
             "--zmqport",
             str(interface.bind_to_random_port()),
         ])
         self.assertEqual(interface.send_and_receive_dict(input_dict=task_dict), np.array(4))
         interface.shutdown(wait=True)
```

### Comparing `pympipool-0.6.0/tests/test_meta.py` & `pympipool-0.6.1/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_multitask.py` & `pympipool-0.6.1/tests/test_multitask.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_parse.py` & `pympipool-0.6.1/tests/test_parse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import sys
 import unittest
 from pympipool.shared.backend import parse_arguments
 from pympipool.shared.connections import MpiExecInterface, FluxCmdInterface, SlurmSubprocessInterface
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
@@ -10,41 +11,41 @@
             'host': 'localhost',
             'zmqport': '22',
         }
         command_lst = [
             'mpiexec',
             '-n', '2',
             '--oversubscribe',
-            'python', '/',
+            sys.executable, '/',
             '--zmqport', result_dict['zmqport']
         ]
         interface = MpiExecInterface(cwd=None, cores=2, gpus_per_core=0, oversubscribe=True)
         self.assertEqual(
             command_lst,
-            interface.generate_command(command_lst=['python', '/', '--zmqport', result_dict['zmqport']])
+            interface.generate_command(command_lst=[sys.executable, '/', '--zmqport', result_dict['zmqport']])
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
 
     def test_command_flux(self):
         result_dict = {
             'host': "127.0.0.1",
             'zmqport': '22',
         }
         command_lst = [
             'flux', 'run', '-n', '2',
             "--cwd=" + os.path.abspath("."),
             '--gpus-per-task=1',
-            'python', '/',
+            sys.executable, '/',
             '--host', result_dict['host'],
             '--zmqport', result_dict['zmqport']
         ]
         interface = FluxCmdInterface(cwd=os.path.abspath("."), cores=2, gpus_per_core=1, oversubscribe=False)
         self.assertEqual(
             command_lst,
-            interface.generate_command(command_lst=['python', '/', '--host', result_dict['host'], '--zmqport', result_dict['zmqport']])
+            interface.generate_command(command_lst=[sys.executable, '/', '--host', result_dict['host'], '--zmqport', result_dict['zmqport']])
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
 
     def test_mpiexec_gpu(self):
         interface = MpiExecInterface(cwd=os.path.abspath("."), cores=2, gpus_per_core=1, oversubscribe=True)
         with self.assertRaises(ValueError):
             interface.bootup(command_lst=[])
@@ -55,17 +56,17 @@
             'zmqport': '22',
         }
         command_lst = [
             'srun', '-n', '2',
             "-D", os.path.abspath("."),
             '--gpus-per-task=1',
             '--oversubscribe',
-            'python', '/',
+            sys.executable, '/',
             '--host', result_dict['host'],
             '--zmqport', result_dict['zmqport']
         ]
         interface = SlurmSubprocessInterface(cwd=os.path.abspath("."), cores=2, gpus_per_core=1, oversubscribe=True)
         self.assertEqual(
             command_lst,
-            interface.generate_command(command_lst=['python', '/', '--host', result_dict['host'], '--zmqport', result_dict['zmqport']])
+            interface.generate_command(command_lst=[sys.executable, '/', '--host', result_dict['host'], '--zmqport', result_dict['zmqport']])
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
```

### Comparing `pympipool-0.6.0/tests/test_parse_legacy.py` & `pympipool-0.6.1/tests/test_parse_legacy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import unittest
 import os
+import sys
+
 from pympipool.legacy.shared.backend import parse_arguments
 from pympipool.shared.connections import MpiExecInterface, FluxCmdInterface
 
 
 class TestParser(unittest.TestCase):
     def test_command_local(self):
         result_dict = {
@@ -12,30 +14,30 @@
             'zmqport': '22',
             'cores_per_task': '1'
         }
         command_lst = [
             'mpiexec',
             '-n', result_dict['total_cores'],
             '--oversubscribe',
-            'python', '-m', 'mpi4py.futures', '/',
+            sys.executable, '-m', 'mpi4py.futures', '/',
             '--zmqport', result_dict['zmqport'],
             '--cores-per-task', result_dict['cores_per_task'],
             '--cores-total', result_dict['total_cores']
         ]
         interface = MpiExecInterface(
             cwd=None,
             cores=2,
             gpus_per_core=0,
             oversubscribe=True
         )
         self.assertEqual(
             command_lst,
             interface.generate_command(
                 command_lst=[
-                    'python', '-m', 'mpi4py.futures', '/',
+                    sys.executable, '-m', 'mpi4py.futures', '/',
                     '--zmqport', result_dict['zmqport'],
                     '--cores-per-task', '1', '--cores-total', '2'
                 ]
             )
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
 
@@ -45,15 +47,15 @@
             'total_cores': '2',
             'zmqport': '22',
             'cores_per_task': '2'
         }
         command_lst = [
             'flux', 'run', '-n', '1',
             "--cwd=" + os.path.abspath("."),
-            'python', '/',
+            sys.executable, '/',
             '--host', result_dict['host'],
             '--zmqport', result_dict['zmqport'],
             '--cores-per-task', result_dict['cores_per_task'],
             '--cores-total', result_dict['total_cores']
         ]
         interface = FluxCmdInterface(
             cwd=os.path.abspath("."),
@@ -61,14 +63,14 @@
             gpus_per_core=0,
             oversubscribe=False
         )
         self.assertEqual(
             command_lst,
             interface.generate_command(
                 command_lst=[
-                    'python', '/', '--host', result_dict['host'],
+                    sys.executable, '/', '--host', result_dict['host'],
                     '--zmqport', result_dict['zmqport'],
                     '--cores-per-task', '2', '--cores-total', '2'
                 ]
             )
         )
         self.assertEqual(result_dict, parse_arguments(command_lst))
```

### Comparing `pympipool-0.6.0/tests/test_pool.py` & `pympipool-0.6.1/tests/test_pool.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_queue.py` & `pympipool-0.6.1/tests/test_queue.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_task.py` & `pympipool-0.6.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_worker.py` & `pympipool-0.6.1/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_worker_memory.py` & `pympipool-0.6.1/tests/test_worker_memory.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/tests/test_zmq.py` & `pympipool-0.6.1/tests/test_zmq.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.6.0/versioneer.py` & `pympipool-0.6.1/versioneer.py`

 * *Files identical despite different names*

