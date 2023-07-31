# Comparing `tmp/scratchattach-1.2.9.tar.gz` & `tmp/scratchattach-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchattach-1.2.9.tar", last modified: Mon Jul 31 11:58:54 2023, max compression
+gzip compressed data, was "scratchattach-1.3.0.tar", last modified: Mon Jul 31 12:16:01 2023, max compression
```

## Comparing `scratchattach-1.2.9.tar` & `scratchattach-1.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:58:54.344886 scratchattach-1.2.9/
--rw-rw-rw-   0        0        0    22121 2023-07-31 11:58:54.344886 scratchattach-1.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 11:58:54.325965 scratchattach-1.2.9/scratchattach/
--rw-rw-rw-   0        0        0      167 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/__init__.py
--rw-rw-rw-   0        0        0    15465 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_cloud.py
--rw-rw-rw-   0        0        0    18518 2023-07-31 11:58:31.000000 scratchattach-1.2.9/scratchattach/_cloud_requests.py
--rw-rw-rw-   0        0        0     1797 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_encoder.py
--rw-rw-rw-   0        0        0      888 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_exceptions.py
--rw-rw-rw-   0        0        0     6558 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_forum.py
--rw-rw-rw-   0        0        0    18239 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_project.py
--rw-rw-rw-   0        0        0    17986 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_session.py
--rw-rw-rw-   0        0        0     9728 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_studio.py
--rw-rw-rw-   0        0        0    25434 2023-07-30 15:45:18.000000 scratchattach-1.2.9/scratchattach/_user.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:58:54.342884 scratchattach-1.2.9/scratchattach.egg-info/
--rw-rw-rw-   0        0        0    22121 2023-07-31 11:58:54.000000 scratchattach-1.2.9/scratchattach.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-07-31 11:58:54.000000 scratchattach-1.2.9/scratchattach.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:58:54.000000 scratchattach-1.2.9/scratchattach.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-31 11:58:54.000000 scratchattach-1.2.9/scratchattach.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 11:58:54.000000 scratchattach-1.2.9/scratchattach.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 11:58:54.344886 scratchattach-1.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-07-31 11:58:46.000000 scratchattach-1.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:16:01.001222 scratchattach-1.3.0/
+-rw-rw-rw-   0        0        0    22121 2023-07-31 12:16:01.000222 scratchattach-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    20795 2023-07-04 18:52:48.000000 scratchattach-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 12:16:00.984507 scratchattach-1.3.0/scratchattach/
+-rw-rw-rw-   0        0        0      167 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/__init__.py
+-rw-rw-rw-   0        0        0    15465 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_cloud.py
+-rw-rw-rw-   0        0        0    18518 2023-07-31 12:07:52.000000 scratchattach-1.3.0/scratchattach/_cloud_requests.py
+-rw-rw-rw-   0        0        0     1797 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_encoder.py
+-rw-rw-rw-   0        0        0      888 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_exceptions.py
+-rw-rw-rw-   0        0        0     6558 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_forum.py
+-rw-rw-rw-   0        0        0    18239 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_project.py
+-rw-rw-rw-   0        0        0    17986 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_session.py
+-rw-rw-rw-   0        0        0     9728 2023-07-30 15:45:18.000000 scratchattach-1.3.0/scratchattach/_studio.py
+-rw-rw-rw-   0        0        0    25440 2023-07-31 12:15:07.000000 scratchattach-1.3.0/scratchattach/_user.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:16:00.999222 scratchattach-1.3.0/scratchattach.egg-info/
+-rw-rw-rw-   0        0        0    22121 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 12:16:00.000000 scratchattach-1.3.0/scratchattach.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:16:01.001222 scratchattach-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-07-31 12:15:22.000000 scratchattach-1.3.0/setup.py
```

### Comparing `scratchattach-1.2.9/PKG-INFO` & `scratchattach-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.9
+Version: 1.3.0
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.2.9/README.md` & `scratchattach-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_cloud.py` & `scratchattach-1.3.0/scratchattach/_cloud.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_cloud_requests.py` & `scratchattach-1.3.0/scratchattach/_cloud_requests.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_encoder.py` & `scratchattach-1.3.0/scratchattach/_encoder.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_exceptions.py` & `scratchattach-1.3.0/scratchattach/_exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_forum.py` & `scratchattach-1.3.0/scratchattach/_forum.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_project.py` & `scratchattach-1.3.0/scratchattach/_project.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_session.py` & `scratchattach-1.3.0/scratchattach/_session.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_studio.py` & `scratchattach-1.3.0/scratchattach/_studio.py`

 * *Files identical despite different names*

### Comparing `scratchattach-1.2.9/scratchattach/_user.py` & `scratchattach-1.3.0/scratchattach/_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,18 +175,18 @@
     def following_names(self, *, limit=40, offset=0):
         return [i.name for i in self.following(limit=limit, offset=offset)]
 
     '''def get_comments(self, *, page=1):
         response = requests.get(f"https://scratch.mit.edu/site-api/comments/user/{self.z}/?page=1")'''
 
     def is_following(self, user):
-        return requests.get(f"https://following-check.1tim.repl.co/api/{self.username}/?following={user}").json()["following"]
+        return requests.get(f"http://explodingstar.pythonanywhere.com/api/{self.username}/?following={user}").json()["following"]
 
     def is_followed_by(self, user):
-        return requests.get(f"https://following-check.1tim.repl.co/api/{user}/?following={self.username}").json()["following"]
+        return requests.get(f"http://explodingstar.pythonanywhere.com/api/{user}/?following={self.username}").json()["following"]
 
     def project_count(self):
         text = requests.get(
             f"https://scratch.mit.edu/users/{self.username}/projects/",
             headers = {
                 "x-csrftoken": "a",
                 "x-requested-with": "XMLHttpRequest",
```

### Comparing `scratchattach-1.2.9/scratchattach.egg-info/PKG-INFO` & `scratchattach-1.3.0/scratchattach.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchattach
-Version: 1.2.9
+Version: 1.3.0
 Summary: An Scratch API Wrapper for scratch.mit.edu
 Home-page: https://github.com/TimMcCool/scratchattach
 Author: TimMcCool
 Author-email: timmccool.scratch@gmail.com
 Keywords: scratch api,scratchattach,scratch api python,scratch python,scratch for python,scratch,scratch cloud,scratch cloud variables,scratch bot
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchattach-1.2.9/setup.py` & `scratchattach-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.2.9'
+VERSION = '1.3.0'
 DESCRIPTION = 'An Scratch API Wrapper for scratch.mit.edu'
 LONG_DESCRIPTION = DESCRIPTION
 
 # Setting up
 setup(
     name="scratchattach",
     version=VERSION,
```

