# Comparing `tmp/nflx-genie-client-3.6.6.tar.gz` & `tmp/nflx-genie-client-3.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nflx-genie-client-3.6.6.tar", last modified: Tue Dec  4 23:41:35 2018, max compression
+gzip compressed data, was "dist/nflx-genie-client-3.6.8.tar", last modified: Thu Jan 31 19:37:30 2019, max compression
```

## Comparing `nflx-genie-client-3.6.6.tar` & `nflx-genie-client-3.6.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     5280 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)      738 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        1 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       76 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/requires.txt
--rw-r--r--   0 travis    (2000) travis    (2000)        8 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/nflx_genie_client.egg-info/top_level.txt
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/pygenie/
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/pygenie/adapter/
--rw-r--r--   0 travis    (2000) travis    (2000)      154 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/adapter/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1709 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/adapter/adapter.py
--rw-r--r--   0 travis    (2000) travis    (2000)    11014 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/adapter/genie_2.py
--rw-r--r--   0 travis    (2000) travis    (2000)    17758 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/adapter/genie_3.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3335 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/adapter/genie_x.py
-drwxr-xr-x   0 travis    (2000) travis    (2000)        0 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/pygenie/jobs/
--rw-r--r--   0 travis    (2000) travis    (2000)      281 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)    29553 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/core.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3744 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/hadoop.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6013 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/hive.py
--rw-r--r--   0 travis    (2000) travis    (2000)     6307 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/pig.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5472 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/presto.py
--rw-r--r--   0 travis    (2000) travis    (2000)    26835 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/running.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7718 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/sqoop.py
--rw-r--r--   0 travis    (2000) travis    (2000)     7166 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/jobs/utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1392 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/__init__.py
--rw-r--r--   0 travis    (2000) travis    (2000)     3088 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/auth.py
--rw-r--r--   0 travis    (2000) travis    (2000)    52731 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/client.py
--rw-r--r--   0 travis    (2000) travis    (2000)    10612 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/conf.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1669 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/exceptions.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1290 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/genie.ini
--rw-r--r--   0 travis    (2000) travis    (2000)     6142 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/pygenie/utils.py
--rw-r--r--   0 travis    (2000) travis    (2000)     1631 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/CHANGES.txt
--rw-r--r--   0 travis    (2000) travis    (2000)     3501 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/DESCRIPTION.rst
--rw-r--r--   0 travis    (2000) travis    (2000)    11343 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/LICENSE.txt
--rw-r--r--   0 travis    (2000) travis    (2000)       28 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/MANIFEST.in
--rw-r--r--   0 travis    (2000) travis    (2000)      638 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/README.md
--rw-r--r--   0 travis    (2000) travis    (2000)     2876 2018-12-04 23:40:56.000000 nflx-genie-client-3.6.6/setup.py
--rw-r--r--   0 travis    (2000) travis    (2000)     5280 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/PKG-INFO
--rw-r--r--   0 travis    (2000) travis    (2000)       38 2018-12-04 23:41:35.000000 nflx-genie-client-3.6.6/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/pygenie/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52731 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/pygenie/jobs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3744 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/hadoop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      281 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7718 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/sqoop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26844 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/running.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    29553 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/core.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7406 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5472 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/presto.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6307 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/pig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6013 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/jobs/hive.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1290 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/genie.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1669 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3088 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/auth.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1392 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6142 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/pygenie/adapter/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1709 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/adapter/adapter.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/adapter/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17758 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/adapter/genie_3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3335 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/adapter/genie_x.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11014 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/adapter/genie_2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10612 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/pygenie/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      638 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11343 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2876 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       76 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5280 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      738 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/nflx_genie_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3501 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/DESCRIPTION.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5280 2019-01-31 19:37:30.000000 nflx-genie-client-3.6.8/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1631 2019-01-31 19:36:53.000000 nflx-genie-client-3.6.8/CHANGES.txt
```

### Comparing `nflx-genie-client-3.6.6/nflx_genie_client.egg-info/PKG-INFO` & `nflx-genie-client-3.6.8/nflx_genie_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nflx-genie-client
-Version: 3.6.6
+Version: 3.6.8
 Summary: Genie Python Client.
 Home-page: http://netflix.github.io/genie/
 Author: Netflix Inc.
 Author-email: genieoss@googlegroups.com
 License: Apache 2.0
 Description: 
         ===================
```

### Comparing `nflx-genie-client-3.6.6/nflx_genie_client.egg-info/SOURCES.txt` & `nflx-genie-client-3.6.8/nflx_genie_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/adapter/adapter.py` & `nflx-genie-client-3.6.8/pygenie/adapter/adapter.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/adapter/genie_2.py` & `nflx-genie-client-3.6.8/pygenie/adapter/genie_2.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/adapter/genie_3.py` & `nflx-genie-client-3.6.8/pygenie/adapter/genie_3.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/adapter/genie_x.py` & `nflx-genie-client-3.6.8/pygenie/adapter/genie_x.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/core.py` & `nflx-genie-client-3.6.8/pygenie/jobs/core.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/hadoop.py` & `nflx-genie-client-3.6.8/pygenie/jobs/hadoop.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/hive.py` & `nflx-genie-client-3.6.8/pygenie/jobs/hive.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/pig.py` & `nflx-genie-client-3.6.8/pygenie/jobs/pig.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/presto.py` & `nflx-genie-client-3.6.8/pygenie/jobs/presto.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/running.py` & `nflx-genie-client-3.6.8/pygenie/jobs/running.py`

 * *Files 0% similar despite different names*

```diff
@@ -639,15 +639,15 @@
         Args:
             iterator (bool, optional): Set to True if want to return as iterator.
 
         Returns:
             str or iterator.
         """
 
-        self._update_stderr()
+        self._update_stderr(**kwargs)
 
         return self._cached_stderr.split('\n') if iterator \
             else self._cached_stderr
 
     @property
     def stdout_url(self):
         """
@@ -996,8 +996,8 @@
             for entry in output_files:
                 if entry.get('name') == 'spark.log':
                     spark_log_exists = True
 
         if spark_log_exists:
             return self._adapter.get_spark_log(self._job_id,
                                                       iterator=iterator,
-                                                      **kwargs)
+                                                      **kwargs)
```

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/sqoop.py` & `nflx-genie-client-3.6.8/pygenie/jobs/sqoop.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/jobs/utils.py` & `nflx-genie-client-3.6.8/pygenie/jobs/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,18 +220,24 @@
 
 
 def is_file(path):
     """Checks if path is to a file."""
 
     path = convert_to_unicode(path)
 
-    return path is not None and \
-        (os.path.isfile(path) \
-         or path.startswith('s3://') \
-         or path.startswith('s3n://'))
+    try:
+        return path is not None and \
+            (os.path.isfile(path) \
+            or path.startswith('s3://') \
+            or path.startswith('s3n://'))
+    except (ValueError, TypeError):
+        # Py2 throws TypeError and Py3 ValueError
+        # if os.path.isfile encounters invalid path
+        # ref https://github.com/python/cpython/pull/7695
+        return False
 
 
 def reattach_job(job_id, conf=None):
     """
     Reattach to a running job.
 
     Search for a job (by job id). If found, return :py:class:`RunningJob` object.
```

### Comparing `nflx-genie-client-3.6.6/pygenie/__init__.py` & `nflx-genie-client-3.6.8/pygenie/__init__.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/auth.py` & `nflx-genie-client-3.6.8/pygenie/auth.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/client.py` & `nflx-genie-client-3.6.8/pygenie/client.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/conf.py` & `nflx-genie-client-3.6.8/pygenie/conf.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/exceptions.py` & `nflx-genie-client-3.6.8/pygenie/exceptions.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/genie.ini` & `nflx-genie-client-3.6.8/pygenie/genie.ini`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/pygenie/utils.py` & `nflx-genie-client-3.6.8/pygenie/utils.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/CHANGES.txt` & `nflx-genie-client-3.6.8/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/DESCRIPTION.rst` & `nflx-genie-client-3.6.8/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/LICENSE.txt` & `nflx-genie-client-3.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/README.md` & `nflx-genie-client-3.6.8/README.md`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/setup.py` & `nflx-genie-client-3.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `nflx-genie-client-3.6.6/PKG-INFO` & `nflx-genie-client-3.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nflx-genie-client
-Version: 3.6.6
+Version: 3.6.8
 Summary: Genie Python Client.
 Home-page: http://netflix.github.io/genie/
 Author: Netflix Inc.
 Author-email: genieoss@googlegroups.com
 License: Apache 2.0
 Description: 
         ===================
```

