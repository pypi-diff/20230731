# Comparing `tmp/utilix-0.7.3.tar.gz` & `tmp/utilix-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilix-0.7.3.tar", last modified: Sat Jun 24 23:05:08 2023, max compression
+gzip compressed data, was "utilix-0.7.4.tar", last modified: Mon Jul 31 20:47:35 2023, max compression
```

## Comparing `utilix-0.7.3.tar` & `utilix-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-24 23:05:08.786452 utilix-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-06-24 23:05:03.000000 utilix-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 23:05:08.786452 utilix-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-24 23:05:03.000000 utilix-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_get.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-24 23:05:03.000000 utilix-0.7.3/tests/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/utilix/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9174 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/batchq.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    23294 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/mongo_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    23315 2023-06-24 23:05:03.000000 utilix-0.7.3/utilix/rundb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 23:05:08.786452 utilix-0.7.3/utilix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 23:05:08.000000 utilix-0.7.3/utilix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:47:35.293839 utilix-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-07-31 20:47:35.293839 utilix-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10353 2023-07-31 20:47:30.000000 utilix-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:47:35.293839 utilix-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-31 20:47:30.000000 utilix-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:47:35.293839 utilix-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-31 20:47:30.000000 utilix-0.7.4/tests/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:47:35.293839 utilix-0.7.4/utilix/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/batchq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23294 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/mongo_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23315 2023-07-31 20:47:30.000000 utilix-0.7.4/utilix/rundb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:47:35.293839 utilix-0.7.4/utilix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-07-31 20:47:35.000000 utilix-0.7.4/utilix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-31 20:47:35.000000 utilix-0.7.4/utilix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:47:35.000000 utilix-0.7.4/utilix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-31 20:47:35.000000 utilix-0.7.4/utilix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 20:47:35.000000 utilix-0.7.4/utilix.egg-info/top_level.txt
```

### Comparing `utilix-0.7.3/PKG-INFO` & `utilix-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.7.3
+Version: 0.7.4
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues.
```

### Comparing `utilix-0.7.3/README.md` & `utilix-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/setup.py` & `utilix-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setup(
     name="utilix",
-    version="0.7.3",
+    version="0.7.4",
     url='https://github.com/XENONnT/utilix',
     description="User-friendly interface to various utilities for XENON users",
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=requires,
     python_requires=">=3.6",
     long_description=readme + '\n\n' + history,
```

### Comparing `utilix-0.7.3/tests/test_get.py` & `utilix-0.7.4/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/tests/test_query.py` & `utilix-0.7.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/tests/test_update.py` & `utilix-0.7.4/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/tests/test_url.py` & `utilix-0.7.4/tests/test_url.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/utilix/batchq.py` & `utilix-0.7.4/utilix/batchq.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,21 +159,14 @@
     os.makedirs(TMPDIR[partition], exist_ok=True)
     # overwrite bind to make sure dali is isolated
     bind = overwrite_dali_bind(bind, partition)
 
     # overwrite log directory if it is not on dali and you are running on dali.
     log = overwrite_dali_job_log(log, partition)
 
-    # temporary dirty fix. will remove these 3 from xenon1t soon.
-    if partition == 'xenon1t':
-        if exclude_nodes is None:
-            exclude_nodes = 'dali0[28-30]'
-        else:
-            exclude_nodes += ',dali028,dali029,dali030'
-
     if container:
         # need to wrap job into another executable
         jobstring = singularity_wrap(jobstring, container, bind, partition)
         jobstring = 'unset X509_CERT_DIR CUTAX_LOCATION\n' + 'module load singularity\n' + jobstring
 
     if not hours is None:
         hours = '#SBATCH --time={:02d}:{:02d}:{:02d}'.format(int(hours), int(hours * 60 % 60), int(hours * 60 % 60 * 60 % 60))
```

### Comparing `utilix-0.7.3/utilix/config.py` & `utilix-0.7.4/utilix/config.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/utilix/io.py` & `utilix-0.7.4/utilix/io.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/utilix/mongo_files.py` & `utilix-0.7.4/utilix/mongo_files.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/utilix/rundb.py` & `utilix-0.7.4/utilix/rundb.py`

 * *Files identical despite different names*

### Comparing `utilix-0.7.3/utilix.egg-info/PKG-INFO` & `utilix-0.7.4/utilix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilix
-Version: 0.7.3
+Version: 0.7.4
 Summary: User-friendly interface to various utilities for XENON users
 Home-page: https://github.com/XENONnT/utilix
 License: UNKNOWN
 Description: # utilix
         [![PyPI version shields.io](https://img.shields.io/pypi/v/utilix.svg)](https://pypi.python.org/pypi/utilix/)
         
         ``utilix`` is a utility package for XENON software, mainly relating to analysis. It currently has two main features: (1) a general XENON configuration framework and (2) easy access to the runsDB by wrapping python calls to a RESTful API. Eventually, we would like to include easy functions for interacting with the Midway and OSG batch queues.
```

