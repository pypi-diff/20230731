# Comparing `tmp/ezcx-0.0.0.tar.gz` & `tmp/ezcx-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcx-0.0.0.tar", last modified: Mon Jul 31 14:30:04 2023, max compression
+gzip compressed data, was "ezcx-0.0.1.tar", last modified: Mon Jul 31 14:51:15 2023, max compression
```

## Comparing `ezcx-0.0.0.tar` & `ezcx-0.0.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:30:04.215236 ezcx-0.0.0/
--rw-r--r--   0 developer  (1001) developer  (1002)    11343 2023-07-31 13:45:28.000000 ezcx-0.0.0/LICENSE
--rw-r--r--   0 developer  (1001) developer  (1002)       70 2023-07-31 14:30:04.215236 ezcx-0.0.0/PKG-INFO
-drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:30:04.211236 ezcx-0.0.0/ezcx/
--rw-r--r--   0 developer  (1001) developer  (1002)      184 2023-07-31 13:38:08.000000 ezcx-0.0.0/ezcx/__init__.py
-drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:30:04.215236 ezcx-0.0.0/ezcx/server/
--rw-r--r--   0 developer  (1001) developer  (1002)      121 2023-07-29 23:56:17.000000 ezcx-0.0.0/ezcx/server/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1002)     1953 2023-07-31 13:47:32.000000 ezcx-0.0.0/ezcx/server/server.py
-drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:30:04.215236 ezcx-0.0.0/ezcx/webhooks/
--rw-r--r--   0 developer  (1001) developer  (1002)       99 2023-07-29 23:54:27.000000 ezcx-0.0.0/ezcx/webhooks/__init__.py
--rw-r--r--   0 developer  (1001) developer  (1002)      768 2023-07-29 22:50:41.000000 ezcx-0.0.0/ezcx/webhooks/request.py
--rw-r--r--   0 developer  (1001) developer  (1002)     2309 2023-07-29 22:49:09.000000 ezcx-0.0.0/ezcx/webhooks/response.py
-drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:30:04.215236 ezcx-0.0.0/ezcx.egg-info/
--rw-r--r--   0 developer  (1001) developer  (1002)       70 2023-07-31 14:30:04.000000 ezcx-0.0.0/ezcx.egg-info/PKG-INFO
--rw-r--r--   0 developer  (1001) developer  (1002)      283 2023-07-31 14:30:04.000000 ezcx-0.0.0/ezcx.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (1001) developer  (1002)        1 2023-07-31 14:30:04.000000 ezcx-0.0.0/ezcx.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (1001) developer  (1002)        5 2023-07-31 14:30:04.000000 ezcx-0.0.0/ezcx.egg-info/top_level.txt
--rw-r--r--   0 developer  (1001) developer  (1002)      497 2023-07-31 14:19:06.000000 ezcx-0.0.0/pyproject.toml
--rw-r--r--   0 developer  (1001) developer  (1002)       38 2023-07-31 14:30:04.215236 ezcx-0.0.0/setup.cfg
--rw-r--r--   0 developer  (1001) developer  (1002)       48 2023-07-31 14:06:25.000000 ezcx-0.0.0/setup.py
+drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:51:15.725304 ezcx-0.0.1/
+-rw-r--r--   0 developer  (1001) developer  (1002)    11343 2023-07-31 13:45:28.000000 ezcx-0.0.1/LICENSE
+-rw-r--r--   0 developer  (1001) developer  (1002)      425 2023-07-31 14:51:15.725304 ezcx-0.0.1/PKG-INFO
+drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:51:15.725304 ezcx-0.0.1/ezcx/
+-rw-r--r--   0 developer  (1001) developer  (1002)      184 2023-07-31 13:38:08.000000 ezcx-0.0.1/ezcx/__init__.py
+drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:51:15.725304 ezcx-0.0.1/ezcx/server/
+-rw-r--r--   0 developer  (1001) developer  (1002)      121 2023-07-29 23:56:17.000000 ezcx-0.0.1/ezcx/server/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1002)     1953 2023-07-31 13:47:32.000000 ezcx-0.0.1/ezcx/server/server.py
+drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:51:15.725304 ezcx-0.0.1/ezcx/webhooks/
+-rw-r--r--   0 developer  (1001) developer  (1002)       99 2023-07-29 23:54:27.000000 ezcx-0.0.1/ezcx/webhooks/__init__.py
+-rw-r--r--   0 developer  (1001) developer  (1002)      768 2023-07-29 22:50:41.000000 ezcx-0.0.1/ezcx/webhooks/request.py
+-rw-r--r--   0 developer  (1001) developer  (1002)     2309 2023-07-29 22:49:09.000000 ezcx-0.0.1/ezcx/webhooks/response.py
+drwxr-xr-x   0 developer  (1001) developer  (1002)        0 2023-07-31 14:51:15.725304 ezcx-0.0.1/ezcx.egg-info/
+-rw-r--r--   0 developer  (1001) developer  (1002)      425 2023-07-31 14:51:15.000000 ezcx-0.0.1/ezcx.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (1001) developer  (1002)      310 2023-07-31 14:51:15.000000 ezcx-0.0.1/ezcx.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (1001) developer  (1002)        1 2023-07-31 14:51:15.000000 ezcx-0.0.1/ezcx.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (1001) developer  (1002)       37 2023-07-31 14:51:15.000000 ezcx-0.0.1/ezcx.egg-info/requires.txt
+-rw-r--r--   0 developer  (1001) developer  (1002)        5 2023-07-31 14:51:15.000000 ezcx-0.0.1/ezcx.egg-info/top_level.txt
+-rw-r--r--   0 developer  (1001) developer  (1002)      573 2023-07-31 14:51:08.000000 ezcx-0.0.1/pyproject.toml
+-rw-r--r--   0 developer  (1001) developer  (1002)       38 2023-07-31 14:51:15.725304 ezcx-0.0.1/setup.cfg
+-rw-r--r--   0 developer  (1001) developer  (1002)       49 2023-07-31 14:41:43.000000 ezcx-0.0.1/setup.py
```

### Comparing `ezcx-0.0.0/LICENSE` & `ezcx-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcx-0.0.0/ezcx/server/server.py` & `ezcx-0.0.1/ezcx/server/server.py`

 * *Files identical despite different names*

### Comparing `ezcx-0.0.0/ezcx/webhooks/request.py` & `ezcx-0.0.1/ezcx/webhooks/request.py`

 * *Files identical despite different names*

### Comparing `ezcx-0.0.0/ezcx/webhooks/response.py` & `ezcx-0.0.1/ezcx/webhooks/response.py`

 * *Files identical despite different names*

