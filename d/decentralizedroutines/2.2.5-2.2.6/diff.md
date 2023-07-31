# Comparing `tmp/decentralizedroutines-2.2.5.tar.gz` & `tmp/decentralizedroutines-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decentralizedroutines-2.2.5.tar", last modified: Mon Jul 31 13:09:38 2023, max compression
+gzip compressed data, was "decentralizedroutines-2.2.6.tar", last modified: Mon Jul 31 18:16:01 2023, max compression
```

## Comparing `decentralizedroutines-2.2.5.tar` & `decentralizedroutines-2.2.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.5/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.5/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.5/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/src/decentralizedroutines/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/RoutineScheduler.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/__init__.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      699 2023-07-31 11:46:47.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/master.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/runroutines.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:43:01.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/update_version_requirements.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/worker.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.5/src/decentralizedroutines/worker_lib.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 13:09:38.714558 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 13:09:38.000000 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-07-31 13:09:38.000000 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 13:09:38.000000 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 13:09:38.000000 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 13:09:38.000000 decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 18:16:01.645127 decentralizedroutines-2.2.6/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.6/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 18:16:01.645127 decentralizedroutines-2.2.6/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      487 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.6/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.6/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      832 2023-07-31 18:16:01.645127 decentralizedroutines-2.2.6/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 18:16:01.641127 decentralizedroutines-2.2.6/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 18:16:01.641127 decentralizedroutines-2.2.6/src/decentralizedroutines/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10063 2023-07-31 11:35:56.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/RoutineScheduler.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/__init__.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      625 2023-06-24 22:45:00.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      699 2023-07-31 11:46:47.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/master.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1356 2023-07-31 11:35:02.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/runroutines.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2212 2023-07-31 11:43:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/update_version_requirements.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8786 2023-07-31 11:42:19.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/worker.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10328 2023-06-30 14:17:28.000000 decentralizedroutines-2.2.6/src/decentralizedroutines/worker_lib.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-07-31 18:16:01.645127 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1126 2023-07-31 18:16:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      618 2023-07-31 18:16:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-07-31 18:16:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       45 2023-07-31 18:16:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       22 2023-07-31 18:16:01.000000 decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/top_level.txt
```

### Comparing `decentralizedroutines-2.2.5/LICENSE` & `decentralizedroutines-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/PKG-INFO` & `decentralizedroutines-2.2.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.5
+Version: 2.2.6
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.5/setup.cfg` & `decentralizedroutines-2.2.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = decentralizedroutines
-version = 2.2.5
+version = 2.2.6
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Master/Worker implementation of decentralized git published routines and kinesis worker pool
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/DecentralizedRoutines
 project_urls = 
@@ -16,15 +16,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.9
 install_requires = 
-	shareddata==2.2.5
+	shareddata==2.2.6
 	psutil==5.9.5
 	tzlocal==4.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
```

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/RoutineScheduler.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/RoutineScheduler.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/defaults.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/defaults.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/master.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/master.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/runroutines.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/runroutines.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/update_version_requirements.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/update_version_requirements.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/worker.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/worker.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines/worker_lib.py` & `decentralizedroutines-2.2.6/src/decentralizedroutines/worker_lib.py`

 * *Files identical despite different names*

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/PKG-INFO` & `decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decentralizedroutines
-Version: 2.2.5
+Version: 2.2.6
 Summary: Master/Worker implementation of decentralized git published routines and kinesis worker pool
 Home-page: https://github.com/jcarlitooliveira/DecentralizedRoutines
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/DecentralizedRoutines/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `decentralizedroutines-2.2.5/src/decentralizedroutines.egg-info/SOURCES.txt` & `decentralizedroutines-2.2.6/src/decentralizedroutines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

