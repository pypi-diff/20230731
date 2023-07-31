# Comparing `tmp/st-supabase-connection-0.0.1.tar.gz` & `tmp/st-supabase-connection-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-supabase-connection-0.0.1.tar", last modified: Mon Jul 31 19:39:52 2023, max compression
+gzip compressed data, was "st-supabase-connection-0.0.2.tar", last modified: Mon Jul 31 19:48:54 2023, max compression
```

## Comparing `st-supabase-connection-0.0.1.tar` & `st-supabase-connection-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.419790 st-supabase-connection-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.419790 st-supabase-connection-0.0.1/src/st_supabase_connection/
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/src/st_supabase_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/st_supabase_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-07-31 19:48:43.000000 st-supabase-connection-0.0.2/src/st_supabase_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:48:54.866883 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:48:54.000000 st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/top_level.txt
```

### Comparing `st-supabase-connection-0.0.1/LICENSE` & `st-supabase-connection-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-0.0.1/PKG-INFO` & `st-supabase-connection-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-supabase-connection
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit connection component for Supabase.
 Home-page: https://github.com/SiddhantSadangi/st_supabase_connection
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Homepage, https://github.com/SiddhantSadangi/st_supabase_connection
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_supabase_connection/blob/main/README.md
 Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
```

### Comparing `st-supabase-connection-0.0.1/README.md` & `st-supabase-connection-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-0.0.1/setup.py` & `st-supabase-connection-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-0.0.1/src/st_supabase_connection/__init__.py` & `st-supabase-connection-0.0.2/src/st_supabase_connection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from io import BytesIO
 from typing import Optional, Union
 
 from streamlit.connections import ExperimentalBaseConnection
-from supabase import create_client
+from supabase import Client, create_client
 
 # TODO: Update demo app
 # TODO: Update README (highlight benefits 1. same methods as the supabase API 2. built on postgrest-py and storage3, the backend behnd the supaabse API
 # 3. less code when using upload and download)
 # TODO: Add docstrings and example usage
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 class SupabaseConnection(ExperimentalBaseConnection[Client]):
     """Connects a streamlit app to Supabase
 
     Attributes
     ----------
```

### Comparing `st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/PKG-INFO` & `st-supabase-connection-0.0.2/src/st_supabase_connection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-supabase-connection
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit connection component for Supabase.
 Home-page: https://github.com/SiddhantSadangi/st_supabase_connection
 Author: Siddhant Sadangi
 Author-email: siddhant.sadangi@gmail.com
 Project-URL: Homepage, https://github.com/SiddhantSadangi/st_supabase_connection
 Project-URL: Documentation, https://github.com/SiddhantSadangi/st_supabase_connection/blob/main/README.md
 Project-URL: Funding, https://www.buymeacoffee.com/siddhantsadangi
```

