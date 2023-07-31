# Comparing `tmp/redb-odm-1.3.2.tar.gz` & `tmp/redb-odm-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.3.2.tar", last modified: Thu Jul 27 21:28:08 2023, max compression
+gzip compressed data, was "redb-odm-1.3.3.tar", last modified: Mon Jul 31 14:21:16 2023, max compression
```

## Comparing `redb-odm-1.3.2.tar` & `redb-odm-1.3.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.120695 redb-odm-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 21:27:52.000000 redb-odm-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 21:28:08.120695 redb-odm-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 21:27:52.000000 redb-odm-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.112695 redb-odm-1.3.2/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-27 21:27:52.000000 redb-odm-1.3.2/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.116695 redb-odm-1.3.2/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 21:28:08.000000 redb-odm-1.3.2/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-27 21:27:52.000000 redb-odm-1.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 21:28:08.120695 redb-odm-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-27 21:27:52.000000 redb-odm-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 21:28:08.120695 redb-odm-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_soft_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-27 21:27:52.000000 redb-odm-1.3.2/tests/test_unique_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.351161 redb-odm-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 14:20:58.000000 redb-odm-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-31 14:21:16.351161 redb-odm-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 14:20:58.000000 redb-odm-1.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.335160 redb-odm-1.3.3/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.339160 redb-odm-1.3.3/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.339160 redb-odm-1.3.3/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14501 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.343160 redb-odm-1.3.3/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.343160 redb-odm-1.3.3/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.343160 redb-odm-1.3.3/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.347160 redb-odm-1.3.3/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-31 14:20:58.000000 redb-odm-1.3.3/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.347160 redb-odm-1.3.3/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-31 14:21:16.000000 redb-odm-1.3.3/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-31 14:21:16.000000 redb-odm-1.3.3/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:21:16.000000 redb-odm-1.3.3/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-31 14:21:16.000000 redb-odm-1.3.3/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 14:21:16.000000 redb-odm-1.3.3/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 14:20:58.000000 redb-odm-1.3.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 14:20:58.000000 redb-odm-1.3.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-31 14:20:58.000000 redb-odm-1.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:21:16.351161 redb-odm-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-31 14:20:58.000000 redb-odm-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:21:16.351161 redb-odm-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-31 14:20:58.000000 redb-odm-1.3.3/tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.3.2/redb/behaviors/i_remember.py` & `redb-odm-1.3.3/redb/behaviors/i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/behaviors/soft_deletion.py` & `redb-odm-1.3.3/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/core/base.py` & `redb-odm-1.3.3/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/core/document.py` & `redb-odm-1.3.3/redb/core/document.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/core/instance.py` & `redb-odm-1.3.3/redb/core/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,20 @@
 
         elif backend == "mongo" or (
             backend is None and check_config(config, MongoConfig)
         ):
             from redb.mongo_system import MongoClient
 
             cls._clients = [MongoClient(config)]
-            cls._uris = {config.database_uri: 0}
+            if isinstance(config, dict):
+                database_uri = config["database_uri"]
+            else:
+                database_uri = config.database_uri
+
+            cls._uris = {database_uri: 0}
             cls._client_name = "mongo"
 
         elif backend == "migo" or (
             backend is None and check_config(config, MigoConfig)
         ):
             from redb.migo_system import MigoClient
```

### Comparing `redb-odm-1.3.2/redb/core/mixins.py` & `redb-odm-1.3.3/redb/core/mixins.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/core/transaction.py` & `redb-odm-1.3.3/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/core/utils.py` & `redb-odm-1.3.3/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/client.py` & `redb-odm-1.3.3/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/collection.py` & `redb-odm-1.3.3/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/configs.py` & `redb-odm-1.3.3/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/database.py` & `redb-odm-1.3.3/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/errors.py` & `redb-odm-1.3.3/redb/interface/errors.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/fields.py` & `redb-odm-1.3.3/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/interface/results.py` & `redb-odm-1.3.3/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/json_system/client.py` & `redb-odm-1.3.3/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/json_system/collection.py` & `redb-odm-1.3.3/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/json_system/database.py` & `redb-odm-1.3.3/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/migo_system/client.py` & `redb-odm-1.3.3/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/migo_system/collection.py` & `redb-odm-1.3.3/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/migo_system/database.py` & `redb-odm-1.3.3/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/mongo_system/client.py` & `redb-odm-1.3.3/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/mongo_system/collection.py` & `redb-odm-1.3.3/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb/mongo_system/database.py` & `redb-odm-1.3.3/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.3.3/redb_odm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/setup.py` & `redb-odm-1.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_bson_objs.py` & `redb-odm-1.3.3/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_hashing.py` & `redb-odm-1.3.3/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_i_remember.py` & `redb-odm-1.3.3/tests/test_i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_json_client.py` & `redb-odm-1.3.3/tests/test_json_client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_mongo_system.py` & `redb-odm-1.3.3/tests/test_mongo_system.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_return_cls.py` & `redb-odm-1.3.3/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_soft_deletion.py` & `redb-odm-1.3.3/tests/test_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.3.2/tests/test_unique_constraints.py` & `redb-odm-1.3.3/tests/test_unique_constraints.py`

 * *Files identical despite different names*

