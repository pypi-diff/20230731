# Comparing `tmp/scratchattach-1.2.7.tar.gz` & `tmp/scratchattach-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.7.tar", last modified: Tue Jul  4 18:53:41 2023, max compression
+gzip compressed data, was "scratchattach-1.2.8.tar", last modified: Mon Jul 31 11:50:01 2023, max compression
```

## Comparing `scratchattach-1.2.7.tar` & `scratchattach-1.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.479739 scratchattach-1.2.7/
--rw-rw-rw-   0        0        0    22121 2023-07-04 18:53:41.478742 scratchattach-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.441054 scratchattach-1.2.7/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-06-10 15:02:36.000000 scratchattach-1.2.7/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    15465 2023-07-04 18:39:44.000000 scratchattach-1.2.7/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18499 2023-06-18 14:33:59.000000 scratchattach-1.2.7/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-06-10 15:02:49.000000 scratchattach-1.2.7/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-06-10 15:02:52.000000 scratchattach-1.2.7/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-06-10 15:02:54.000000 scratchattach-1.2.7/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-06-10 15:02:57.000000 scratchattach-1.2.7/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-06-10 16:04:19.000000 scratchattach-1.2.7/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-06-10 15:02:59.000000 scratchattach-1.2.7/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-06-10 15:03:05.000000 scratchattach-1.2.7/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-07-04 18:53:41.476264 scratchattach-1.2.7/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22121 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-04 18:53:40.000000 scratchattach-1.2.7/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 18:53:41.479739 scratchattach-1.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-07-04 18:52:57.000000 scratchattach-1.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.399992 scratchattach-1.2.8/
+-rw-rw-rw-   0        0        0    22121 2023-07-31 11:50:01.399992 scratchattach-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.382493 scratchattach-1.2.8/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    15465 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18513 2023-07-31 11:49:08.000000 scratchattach-1.2.8/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25434 2023-07-30 15:45:18.000000 scratchattach-1.2.8/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.398992 scratchattach-1.2.8/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22121 2023-07-31 11:49:58.000000 scratchattach-1.2.8/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-31 11:50:01.000000 scratchattach-1.2.8/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:49:58.000000 scratchattach-1.2.8/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-31 11:49:58.000000 scratchattach-1.2.8/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 11:49:58.000000 scratchattach-1.2.8/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:50:01.399992 scratchattach-1.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-07-31 11:49:30.000000 scratchattach-1.2.8/setup.py
```

### Comparing `scratchattach-1.2.7/PKG-INFO` & `scratchattach-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.7
+Version: 1.2.8
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.2.7/README.md` & `scratchattach-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_cloud.py` & `scratchattach-1.2.8/scratchattach/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_cloud_requests.py` & `scratchattach-1.2.8/scratchattach/_cloud_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,16 +430,16 @@
                     if req_obj["thread"]:
                         Thread(target=self.call_request,
                                args=(request_id, req_obj, arguments)).start()
                     else:
                         self.call_request(request_id, req_obj, arguments)
 
             #Send outputs
-            output_ids = list(self.outputs.keys())
-            while len(output_ids) > 0:
+            while list(self.outputs.keys()) > 0:
+                output_ids = list(self.outputs.keys())
                 for request_id in output_ids:
                     output = self.outputs[request_id]["output"]
                     request = self.outputs[request_id]["request"]["name"]
                     req_obj = self.outputs[request_id]["request"]
                     self._parse_output(output, request, req_obj, request_id)
                     self.outputs.pop(request_id)
```

### Comparing `scratchattach-1.2.7/scratchattach/_encoder.py` & `scratchattach-1.2.8/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_exceptions.py` & `scratchattach-1.2.8/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_forum.py` & `scratchattach-1.2.8/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_project.py` & `scratchattach-1.2.8/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_session.py` & `scratchattach-1.2.8/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_studio.py` & `scratchattach-1.2.8/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach/_user.py` & `scratchattach-1.2.8/scratchattach/_user.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.7/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.2.8/scratchattach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.7
+Version: 1.2.8
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.2.7/setup.py` & `scratchattach-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.7'
+VERSION = '1.2.8'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

