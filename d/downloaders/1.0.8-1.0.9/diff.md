# Comparing `tmp/downloaders-1.0.8.tar.gz` & `tmp/downloaders-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/downloaders-1.0.8.tar", last modified: Fri Jan  8 10:34:22 2021, max compression
+gzip compressed data, was "dist/downloaders-1.0.9.tar", last modified: Fri Jan  8 10:45:06 2021, max compression
```

## Comparing `downloaders-1.0.8.tar` & `downloaders-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:34:22.000000 downloaders-1.0.8/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2020-12-19 08:20:06.000000 downloaders-1.0.8/MANIFEST.in
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4983 2021-01-08 10:34:22.000000 downloaders-1.0.8/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3767 2020-12-24 08:33:17.000000 downloaders-1.0.8/README.rst
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:34:22.000000 downloaders-1.0.8/downloaders/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      136 2020-12-23 13:04:32.000000 downloaders-1.0.8/downloaders/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       67 2021-01-08 10:33:48.000000 downloaders-1.0.8/downloaders/__version__.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:34:22.000000 downloaders-1.0.8/downloaders/downloaders/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      141 2020-12-23 13:04:09.000000 downloaders-1.0.8/downloaders/downloaders/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)    13300 2021-01-08 10:32:51.000000 downloaders-1.0.8/downloaders/downloaders/base_downloader.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:34:22.000000 downloaders-1.0.8/downloaders/extractors/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      122 2020-12-19 15:32:39.000000 downloaders-1.0.8/downloaders/extractors/__init__.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     3206 2021-01-08 10:17:00.000000 downloaders-1.0.8/downloaders/extractors/auto_extractor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4266 2020-12-23 15:30:27.000000 downloaders-1.0.8/downloaders/extractors/base_extractor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1684 2020-12-23 09:47:49.000000 downloaders-1.0.8/downloaders/extractors/gzip_extractor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1577 2020-12-23 09:49:05.000000 downloaders-1.0.8/downloaders/extractors/targz_extractor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1525 2020-12-24 08:52:14.000000 downloaders-1.0.8/downloaders/extractors/utils.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1628 2020-12-23 09:49:11.000000 downloaders-1.0.8/downloaders/extractors/xz_extractor.py
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1559 2020-12-23 09:49:16.000000 downloaders-1.0.8/downloaders/extractors/zip_extraction.py
-drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:34:22.000000 downloaders-1.0.8/downloaders.egg-info/
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     4983 2021-01-08 10:34:21.000000 downloaders-1.0.8/downloaders.egg-info/PKG-INFO
--rw-r--r--   0 lucacappelletti   (501) staff       (20)      647 2021-01-08 10:34:21.000000 downloaders-1.0.8/downloaders.egg-info/SOURCES.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-01-08 10:34:21.000000 downloaders-1.0.8/downloaders.egg-info/dependency_links.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       86 2021-01-08 10:34:21.000000 downloaders-1.0.8/downloaders.egg-info/requires.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       12 2021-01-08 10:34:21.000000 downloaders-1.0.8/downloaders.egg-info/top_level.txt
--rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-01-08 10:34:22.000000 downloaders-1.0.8/setup.cfg
--rw-r--r--   0 lucacappelletti   (501) staff       (20)     1740 2020-12-23 20:38:47.000000 downloaders-1.0.8/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:45:06.000000 downloaders-1.0.9/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        0 2020-12-19 08:20:06.000000 downloaders-1.0.9/MANIFEST.in
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4983 2021-01-08 10:45:06.000000 downloaders-1.0.9/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3767 2020-12-24 08:33:17.000000 downloaders-1.0.9/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      136 2020-12-23 13:04:32.000000 downloaders-1.0.9/downloaders/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       67 2021-01-08 10:45:01.000000 downloaders-1.0.9/downloaders/__version__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders/downloaders/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      141 2020-12-23 13:04:09.000000 downloaders-1.0.9/downloaders/downloaders/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    13447 2021-01-08 10:44:00.000000 downloaders-1.0.9/downloaders/downloaders/base_downloader.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders/extractors/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      122 2020-12-19 15:32:39.000000 downloaders-1.0.9/downloaders/extractors/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     3206 2021-01-08 10:17:00.000000 downloaders-1.0.9/downloaders/extractors/auto_extractor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4266 2020-12-23 15:30:27.000000 downloaders-1.0.9/downloaders/extractors/base_extractor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1684 2020-12-23 09:47:49.000000 downloaders-1.0.9/downloaders/extractors/gzip_extractor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1577 2020-12-23 09:49:05.000000 downloaders-1.0.9/downloaders/extractors/targz_extractor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1525 2020-12-24 08:52:14.000000 downloaders-1.0.9/downloaders/extractors/utils.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1628 2020-12-23 09:49:11.000000 downloaders-1.0.9/downloaders/extractors/xz_extractor.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1559 2020-12-23 09:49:16.000000 downloaders-1.0.9/downloaders/extractors/zip_extraction.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      199 2021-01-08 10:42:54.000000 downloaders-1.0.9/downloaders/utils.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     4983 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      668 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       86 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       12 2021-01-08 10:45:06.000000 downloaders-1.0.9/downloaders.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2021-01-08 10:45:06.000000 downloaders-1.0.9/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1740 2020-12-23 20:38:47.000000 downloaders-1.0.9/setup.py
```

### Comparing `downloaders-1.0.8/PKG-INFO` & `downloaders-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downloaders
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package to handle download of multiple types of files.
 Home-page: https://github.com/LucaCappelletti94/downloaders
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: downloaders
         =========================================================================================
```

### Comparing `downloaders-1.0.8/README.rst` & `downloaders-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/downloaders/base_downloader.py` & `downloaders-1.0.9/downloaders/downloaders/base_downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Union, List, Dict
 import requests
 from tqdm.auto import tqdm
 from multiprocessing import Pool, cpu_count
 import os
 import pandas as pd
 from ..extractors import AutoExtractor
+from ..utils import is_iterable
 
 
 class BaseDownloader:
     """Base class for making downloaders."""
 
     def __init__(
         self,
@@ -16,15 +17,15 @@
         block_size: int = 32768,
         auto_extract: bool = True,
         delete_original_after_extraction: bool = True,
         max_description_size: int = 50,
         cache: bool = True,
         target_directory: str = "downloads",
         description_pattern="Downloading to {}",
-        crash_early: bool = True,
+        crash_early: bool = False,
         verbose: int = 1
     ):
         """Create new BaseDownloader.
 
         Parameters
         ------------------
         process_number: int = -1,
@@ -40,15 +41,15 @@
             Maximum length of the description in the loading bar.
         cache: bool = True,
             Wether to use cache or not.
         target_directory: str = "downloads",
             Position where to store the downloaded files.
         description_pattern="Downloading to {}",
             Pattern to use for the loading bar description.
-        crash_early: bool = True,
+        crash_early: bool = False,
             Wether if the download should stop at the earliest crash.
         verbose: int = 1
             The level of verbosity.
             With level 1, the overall loading bar is showed.
             With level 2, also the download of each element is showed.
         """
         if not isinstance(process_number, int) or process_number == 0:
@@ -277,18 +278,22 @@
         ValueError,
             If the request has not a status code 200 (success).
 
         Returns
         ----------------------
         Dataframe with report on the operations executed.
         """
-        if not isinstance(urls, list):
+        if isinstance(urls, str):
             urls = [urls]
-        if paths is not None and not isinstance(paths, list):
+        if is_iterable(urls):
+            urls = list(urls)
+        if paths is not None and isinstance(paths, str):
             paths = [paths]
+        if is_iterable(paths):
+            paths = list(paths)
         if isinstance(urls, list) and isinstance(paths, list) and len(urls) != len(paths):
             raise ValueError(
                 "The urls and paths lists must have the same length."
             )
         # Use the minimum amount of processes.
         process_number = min(len(urls), self._process_number)
         # Create the tasks generator
```

### Comparing `downloaders-1.0.8/downloaders/extractors/auto_extractor.py` & `downloaders-1.0.9/downloaders/extractors/auto_extractor.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/base_extractor.py` & `downloaders-1.0.9/downloaders/extractors/base_extractor.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/gzip_extractor.py` & `downloaders-1.0.9/downloaders/extractors/gzip_extractor.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/targz_extractor.py` & `downloaders-1.0.9/downloaders/extractors/targz_extractor.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/utils.py` & `downloaders-1.0.9/downloaders/extractors/utils.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/xz_extractor.py` & `downloaders-1.0.9/downloaders/extractors/xz_extractor.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders/extractors/zip_extraction.py` & `downloaders-1.0.9/downloaders/extractors/zip_extraction.py`

 * *Files identical despite different names*

### Comparing `downloaders-1.0.8/downloaders.egg-info/PKG-INFO` & `downloaders-1.0.9/downloaders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: downloaders
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python package to handle download of multiple types of files.
 Home-page: https://github.com/LucaCappelletti94/downloaders
 Author: LucaCappelletti94
 Author-email: cappelletti.luca94@gmail.com
 License: MIT
 Description: downloaders
         =========================================================================================
```

### Comparing `downloaders-1.0.8/downloaders.egg-info/SOURCES.txt` & `downloaders-1.0.9/downloaders.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 README.rst
 setup.py
 downloaders/__init__.py
 downloaders/__version__.py
+downloaders/utils.py
 downloaders.egg-info/PKG-INFO
 downloaders.egg-info/SOURCES.txt
 downloaders.egg-info/dependency_links.txt
 downloaders.egg-info/requires.txt
 downloaders.egg-info/top_level.txt
 downloaders/downloaders/__init__.py
 downloaders/downloaders/base_downloader.py
```

### Comparing `downloaders-1.0.8/setup.py` & `downloaders-1.0.9/setup.py`

 * *Files identical despite different names*

