# Comparing `tmp/best_bottrop_garbage_collection_dates-0.0.26.tar.gz` & `tmp/best_bottrop_garbage_collection_dates-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "best_bottrop_garbage_collection_dates-0.0.26.tar", last modified: Thu Jul 27 17:23:02 2023, max compression
+gzip compressed data, was "best_bottrop_garbage_collection_dates-0.0.27.tar", last modified: Mon Jul 31 18:31:15 2023, max compression
```

## Comparing `best_bottrop_garbage_collection_dates-0.0.26.tar` & `best_bottrop_garbage_collection_dates-0.0.27.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.981380 best_bottrop_garbage_collection_dates-0.0.26/
--rw-r--r--   0 denis      (501) staff       (20)     1062 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/LICENSE
--rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-27 17:23:02.981439 best_bottrop_garbage_collection_dates-0.0.26/PKG-INFO
--rw-r--r--   0 denis      (501) staff       (20)      188 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/README.md
--rw-r--r--   0 denis      (501) staff       (20)      103 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/pyproject.toml
--rw-r--r--   0 denis      (501) staff       (20)      710 2023-07-27 17:23:02.982081 best_bottrop_garbage_collection_dates-0.0.26/setup.cfg
-drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.969448 best_bottrop_garbage_collection_dates-0.0.26/src/
-drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.974651 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/
--rw-r--r--   0 denis      (501) staff       (20)      167 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/__init__.py
--rw-r--r--   0 denis      (501) staff       (20)     2673 2023-07-27 17:18:26.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py
--rw-r--r--   0 denis      (501) staff       (20)    26841 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/const.py
-drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.979779 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/
--rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO
--rw-r--r--   0 denis      (501) staff       (20)      509 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/SOURCES.txt
--rw-r--r--   0 denis      (501) staff       (20)        1 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/dependency_links.txt
--rw-r--r--   0 denis      (501) staff       (20)       38 2023-07-27 17:23:02.000000 best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/top_level.txt
-drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-27 17:23:02.981037 best_bottrop_garbage_collection_dates-0.0.26/tests/
--rw-r--r--   0 denis      (501) staff       (20)     2899 2023-07-27 16:56:31.000000 best_bottrop_garbage_collection_dates-0.0.26/tests/test_best.py
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-31 18:31:15.980699 best_bottrop_garbage_collection_dates-0.0.27/
+-rw-r--r--   0 denis      (501) staff       (20)     1062 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.27/LICENSE
+-rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-31 18:31:15.980769 best_bottrop_garbage_collection_dates-0.0.27/PKG-INFO
+-rw-r--r--   0 denis      (501) staff       (20)      188 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.27/README.md
+-rw-r--r--   0 denis      (501) staff       (20)      103 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.27/pyproject.toml
+-rw-r--r--   0 denis      (501) staff       (20)      710 2023-07-31 18:31:15.982269 best_bottrop_garbage_collection_dates-0.0.27/setup.cfg
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-31 18:31:15.974092 best_bottrop_garbage_collection_dates-0.0.27/src/
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-31 18:31:15.976945 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/
+-rw-r--r--   0 denis      (501) staff       (20)      167 2023-07-31 18:27:40.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/__init__.py
+-rw-r--r--   0 denis      (501) staff       (20)     2747 2023-07-31 18:25:47.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py
+-rw-r--r--   0 denis      (501) staff       (20)    26841 2023-07-27 16:24:20.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/const.py
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-31 18:31:15.979864 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/
+-rw-r--r--   0 denis      (501) staff       (20)      774 2023-07-31 18:31:15.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO
+-rw-r--r--   0 denis      (501) staff       (20)      509 2023-07-31 18:31:15.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/SOURCES.txt
+-rw-r--r--   0 denis      (501) staff       (20)        1 2023-07-31 18:31:15.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/dependency_links.txt
+-rw-r--r--   0 denis      (501) staff       (20)       38 2023-07-31 18:31:15.000000 best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/top_level.txt
+drwxr-xr-x   0 denis      (501) staff       (20)        0 2023-07-31 18:31:15.980334 best_bottrop_garbage_collection_dates-0.0.27/tests/
+-rw-r--r--   0 denis      (501) staff       (20)     2899 2023-07-27 16:56:31.000000 best_bottrop_garbage_collection_dates-0.0.27/tests/test_best.py
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/LICENSE` & `best_bottrop_garbage_collection_dates-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/PKG-INFO` & `best_bottrop_garbage_collection_dates-0.0.27/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best_bottrop_garbage_collection_dates
-Version: 0.0.26
+Version: 0.0.27
 Summary: A package to find the garbage collection dates in the city of Bottrop, Germany
 Home-page: https://github.com/Nazze/best_bottrop_garbage_collection_dates
 Author: Nazze
 Project-URL: Bug Tracker, https://github.com/Nazze/best_bottrop_garbage_collection_dates/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/setup.cfg` & `best_bottrop_garbage_collection_dates-0.0.27/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = best_bottrop_garbage_collection_dates
-version = 0.0.26
+version = 0.0.27
 author = Nazze
 description = A package to find the garbage collection dates in the city of Bottrop, Germany
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Nazze/best_bottrop_garbage_collection_dates
 project_urls = 
 	Bug Tracker = https://github.com/Nazze/best_bottrop_garbage_collection_dates/issues
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py` & `best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/best_bottrop_garbage_collection_dates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from .const import STREET_ID_DICT
-import enum
-import requests
-import datetime
 import aiohttp
 import asyncio
+import enum
+import datetime
+import logging
+import requests
+
+_LOGGER = logging.getLogger(__name__)
 
 @dataclass
 class BESTBottropGarbageCollectionDates:
     """ Class for managing connection and data to the BEST Bottrop garbage collection dates"""
 
     trash_types_json : list[dict] = ""
     session_timeout = aiohttp.ClientTimeout (total = 10)
@@ -39,32 +42,31 @@
     async def get_trash_types (self):
         # Load the trashtypes
         try:
             async with aiohttp.ClientSession(timeout = self.session_timeout) as session:
                 async with session.get('https://www.best-bottrop.de/api/trashtype') as trash_types_response:
                     self.trash_types_json = await trash_types_response.json()
         except (aiohttp.ClientError, aiohttp.ClientConnectionError, TimeoutError) as e:
-            print ("Could not load dates! Exception: {0}".format(e))
+            _LOGGER.debug ("Could not load dates due to exception: %s", type(e).__name__)
             raise e
-            return ""
 
     async def get_dates_as_json(self, street_code, number) -> list[dict]:
         # Get the BEST street id code for a given street
         #street_code = STREET_ID_DICT.get(street)
 
         dates_json = ""
 
         if (street_code != None and self.trash_types_json != None):
             try:
                 async with aiohttp.ClientSession(timeout = self.session_timeout) as session:
                     async with session.get('https://www.best-bottrop.de/api/street/{0}/house/{1}/collection'.format(street_code, number)) as dates:
                         dates_json = await dates.json()
                         dates_json = list(filter(self._today_or_later, dates_json))
             except (aiohttp.ClientError, aiohttp.ClientConnectionError, TimeoutError) as e:
-                print ("Could not load dates! Exception: {0}".format(e))
+                _LOGGER.debug ("Could not load dates due to exception: %s", type(e).__name__)
                 raise e
 
             for date_item in dates_json:
                 date_item.update({"trashType": self._get_name_for_id(date_item.get("trashType"), self.trash_types_json)})
 
         return dates_json
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates/const.py` & `best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates/const.py`

 * *Files identical despite different names*

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO` & `best_bottrop_garbage_collection_dates-0.0.27/src/best_bottrop_garbage_collection_dates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: best-bottrop-garbage-collection-dates
-Version: 0.0.26
+Version: 0.0.27
 Summary: A package to find the garbage collection dates in the city of Bottrop, Germany
 Home-page: https://github.com/Nazze/best_bottrop_garbage_collection_dates
 Author: Nazze
 Project-URL: Bug Tracker, https://github.com/Nazze/best_bottrop_garbage_collection_dates/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `best_bottrop_garbage_collection_dates-0.0.26/tests/test_best.py` & `best_bottrop_garbage_collection_dates-0.0.27/tests/test_best.py`

 * *Files identical despite different names*

