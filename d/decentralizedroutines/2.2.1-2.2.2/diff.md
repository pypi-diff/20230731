# Comparing `tmp/decentralizedroutines-2.2.1.tar.gz` & `tmp/decentralizedroutines-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.2.1.tar", last modified: Mon Jul 31 11:42:50 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.2.2.tar", last modified: Mon Jul 31 11:46:59 2023, max compression
```

## Comparing `decentralizedroutines-2.2.1.tar` & `decentralizedroutines-2.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/decentralizedroutines/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/__init__.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      613 2023-07-31 11:35:52.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/master.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/runroutines.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:38:35.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/update_version_requirements.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/worker.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.1/src/decentralizedroutines/worker_lib.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:42:50.940756 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 11:42:50.000000 decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.2/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.2/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.2/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/src/decentralizedroutines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      699 2023-07-31 11:46:47.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/master.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/runroutines.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:43:01.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.2/src/decentralizedroutines/worker_lib.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 11:46:59.738608 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 11:46:59.000000 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-07-31 11:46:59.000000 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 11:46:59.000000 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 11:46:59.000000 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 11:46:59.000000 decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.2.1/LICENSE` & `decentralizedroutines-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/PKG-INFO` & `decentralizedroutines-2.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.1
+Version: 2.2.2
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.1/setup.cfg` & `decentralizedroutines-2.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = decentralizedroutines
-version = 2.2.1
+version = 2.2.2
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Master/Worker implementation of decentralized git published routines and kinesis worker pool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/DecentralizedRoutines
 project_urls =
```

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/RoutineScheduler.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/runroutines.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/update_version_requirements.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from decentralizedroutines.worker_lib import send_command
 import decentralizedroutines.defaults as defaults 
 from SharedData.SharedData import SharedData
 shdata = SharedData(__file__,user='master')
 from SharedData.Logger import Logger
 
 
-shareddata_version='shareddata==2.0.31'
-decentralizedroutines_version='decentralizedroutines==2.0.31'
+shareddata_version='shareddata==2.0.35'
+decentralizedroutines_version='decentralizedroutines==2.0.35'
 source_folder = Path(os.environ['SOURCE_FOLDER'])
 paths = [Path(source_folder/f) for f in os.listdir(source_folder) if Path.is_dir(source_folder/f)]
 path = paths[1]
 for path in paths:
     req_path = path/'requirements.txt'
     if (req_path).is_file():
         print(req_path)
```

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/worker.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.2.2/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.1
+Version: 2.2.2
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.1/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.2.2/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

