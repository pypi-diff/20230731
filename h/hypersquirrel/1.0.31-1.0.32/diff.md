# Comparing `tmp/hypersquirrel-1.0.31.tar.gz` & `tmp/hypersquirrel-1.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersquirrel-1.0.31.tar", last modified: Thu Jul 27 16:46:33 2023, max compression
+gzip compressed data, was "hypersquirrel-1.0.32.tar", last modified: Mon Jul 31 13:53:25 2023, max compression
```

## Comparing `hypersquirrel-1.0.31.tar` & `hypersquirrel-1.0.32.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreter/ph.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/literalinterpreterfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/hypersquirrel/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/buondua.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/cosplayporntube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/drts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/fseg.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/googleimagesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hcos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hellp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/hnlg.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/lgbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/nlgs.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/opendir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/sbgx.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/v2ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/vg.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/xh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/xv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraper/youtubeapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/scraperfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/hypersquirrel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.282415 hypersquirrel-1.0.31/hypersquirrel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 16:46:33.000000 hypersquirrel-1.0.31/hypersquirrel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-27 16:46:17.000000 hypersquirrel-1.0.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:33.286415 hypersquirrel-1.0.31/ytdlwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/ytdlwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-27 16:46:16.000000 hypersquirrel-1.0.31/ytdlwrapper/ytdlpscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.967520 hypersquirrel-1.0.32/hypersquirrel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.971520 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreterfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.975520 hypersquirrel-1.0.32/hypersquirrel/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/buondua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/cosplayporntube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/drts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/fseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/googleimagesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hellp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hnlg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/lgbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/nlgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/opendir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/sbgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/v2ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/vg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/xh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/xv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/youtubeapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraperfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.971520 hypersquirrel-1.0.32/hypersquirrel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/ytdlwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/ytdlwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/ytdlwrapper/ytdlpscrape.py
```

### Comparing `hypersquirrel-1.0.31/LICENSE` & `hypersquirrel-1.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/PKG-INFO` & `hypersquirrel-1.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.31
+Version: 1.0.32
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.31/hypersquirrel/core.py` & `hypersquirrel-1.0.32/hypersquirrel/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import sys
 from dataclasses import dataclass, field
 from typing import Iterator, Callable
 
 
 @dataclass
 class Watchlist:
-    url: str
+    url: str = field(default=None)
     max_items: int = field(default=None)
     page_min: int = field(default=1)
     page_max: int = field(default=1)
+    html: str = field(default=None)
 
     @property
     def is_multipage(self):
         return "${page}" in self.url
 
     def __post_init__(self):
-        assert self.url
-        if self.is_multipage:
+        assert self.url or self.html
+        if self.url and self.is_multipage:
             assert isinstance(self.page_min, int)
             assert isinstance(self.page_max, int)
             assert self.page_min < self.page_max
 
     def scrape(self, scraper: Callable[[str], Iterator[dict]], url=None):
         def generate():
             for page in range(self.page_min, self.page_max + 1):
```

### Comparing `hypersquirrel-1.0.31/hypersquirrel/entry.py` & `hypersquirrel-1.0.32/hypersquirrel/entry.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/literalinterpreterfactory.py` & `hypersquirrel-1.0.32/hypersquirrel/literalinterpreterfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/buondua.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/buondua.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/cosplayporntube.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/cosplayporntube.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/drts.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/drts.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/ehen.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/ehen.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/fseg.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/fseg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/hcos.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/hcos.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/hellp.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/hellp.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/hnlg.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/hnlg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/lgbb.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/lgbb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/nh.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/nh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/nlgs.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/nlgs.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/reddit.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/reddit.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/sb.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/sb.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 from commmons import get_host_url
 from lxml import html
+from pydash import head
 
+from hypersquirrel.core import Watchlist
 
-def scrape(url):
-    def get_body_with_ytdl() -> str:
-        from yt_dlp import YoutubeDL
-        ytdl = YoutubeDL()
-        ie = ytdl.get_info_extractor("SpankBang")
-        mobj = ie._match_valid_url(url)
-        video_id = mobj.group('id') or mobj.group('id_2')
-        return ie._download_webpage(
-            url.replace('/%s/embed' % video_id, '/%s/video' % video_id),
-            video_id, headers={'Cookie': 'country=US'})
-
-    tree = html.fromstring(get_body_with_ytdl())
-    host_url = get_host_url(url)
 
+def _scrape(tree, host_url):
     divs = tree.xpath("//div[contains(@class, 'video-item')]")
     for div in divs:
         if "data-id" not in div.attrib:
             continue
 
         dataid = div.attrib["data-id"]
         atags = div.xpath("./a")
@@ -36,7 +26,40 @@
 
         yield {
             "fileid": "sb" + dataid,
             "sourceurl": host_url + atag.attrib["href"],
             "filename": img.attrib["alt"],
             "thumbnailurl": img.attrib["data-src"]
         }
+
+
+def scrape(url):
+    def get_body_with_ytdl() -> str:
+        from yt_dlp import YoutubeDL
+        ytdl = YoutubeDL()
+        ie = ytdl.get_info_extractor("SpankBang")
+        mobj = ie._match_valid_url(url)
+        video_id = mobj.group('id') or mobj.group('id_2')
+        return ie._download_webpage(
+            url.replace('/%s/embed' % video_id, '/%s/video' % video_id),
+            video_id, headers={'Cookie': 'country=US'})
+
+    tree = html.fromstring(get_body_with_ytdl())
+    host_url = get_host_url(url)
+    yield from _scrape(tree, host_url)
+
+
+def scrape_html(w: Watchlist):
+    assert w.html
+    tree = html.fromstring(w.html)
+    yield from _scrape(tree, "https://spankbang.com")
+
+
+def is_sb_html(w: Watchlist):
+    if w.html:
+        tree = html.fromstring(w.html)
+        title = head(tree.xpath("//head/title"))
+
+        if title is not None and "SpankBang" in title.text:
+            return True
+
+    return False
```

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/sbgx.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/sbgx.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/v2ph.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/v2ph.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/vg.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/vg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/xh.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/xh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/xv.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/xv.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraper/youtubeapi.py` & `hypersquirrel-1.0.32/hypersquirrel/scraper/youtubeapi.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel/scraperfactory.py` & `hypersquirrel-1.0.32/hypersquirrel/scraperfactory.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .scraper.hcos import scrape_hcos
 from .scraper.hnlg import scrape_hnlg
 from .scraper.lgbb import scrape_lgbb
 from .scraper.nh import scrape as scrape_nh_html
 from .scraper.nlgs import scrape_uulg, scrape_nlgs, scrape_lgcx
 from .scraper.opendir import scrape as scrape_opendir
 from .scraper.reddit import scrape_reddit_rss, scrape_reddit_json
-from .scraper.sb import scrape as scrape_sb_html
+from .scraper.sb import scrape as scrape_sb_url, scrape_html as scrape_sb_html, is_sb_html
 from .scraper.sbgx import scrape_sbgx
 from .scraper.v2ph import scrape_v2ph
 from .scraper.vg import scrape_vipergirls as scrape_vg_html
 from .scraper.xh import scrape as scrape_xh_html
 from .scraper.xv import scrape as scrape_xv_html
 from .scraper.hellp import scrape as scrape_hellp
 
@@ -47,15 +47,15 @@
 get_scraper = _wsf.get_scraper
 register_scraper = _wsf.register_scraper
 
 register_scraper(lambda w: "pornhub.com" in w.url, scrape_nh_html)
 register_scraper(lambda w: "vipergirls" in w.url, scrape_vg_html)
 register_scraper(lambda w: "xhamster" in w.url, scrape_xh_html)
 register_scraper(lambda w: "xvideos.com" in w.url, scrape_xv_html)
-register_scraper(lambda w: "spankbang.com" in w.url, scrape_sb_html)
+register_scraper(lambda w: "spankbang.com" in w.url, scrape_sb_url)
 register_scraper(lambda w: "reddit" in w.url and "json?feed" in w.url, scrape_reddit_json)
 register_scraper(lambda w: "reddit" in w.url, scrape_reddit_rss)
 register_scraper(lambda w: "v2ph" in w.url, scrape_v2ph)
 register_scraper(lambda w: "hentai-cosplays" in w.url, scrape_hcos)
 register_scraper(lambda w: "buondua" in w.url, scrape_buondua)
 register_scraper(lambda w: "e-hentai" in w.url, scrape_ehen)
 register_scraper(lambda w: "cosplayporntube" in w.url, scrape_cpt)
@@ -68,7 +68,10 @@
 register_scraper(lambda w: "superbeautygirlx" in w.url, scrape_sbgx)
 register_scraper(lambda w: "porn-images-xxx" in w.url, scrape_hcos)
 register_scraper(lambda w: "hentai-img" in w.url, scrape_hcos)
 register_scraper(lambda w: "google" in w.url, scrape_gimg)
 register_scraper(lambda w: "dirtyship" in w.url, scrape_drts)
 register_scraper(lambda w: "hellporno" in w.url, scrape_hellp)
 register_scraper(lambda w: "youtube" in w.url, youtubeapi.scrape_youtubeapi)
+
+# html-based scrapers at the as they cost a lot
+register_scraper(is_sb_html, scrape_sb_html)
```

### Comparing `hypersquirrel-1.0.31/hypersquirrel/util.py` & `hypersquirrel-1.0.32/hypersquirrel/util.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/hypersquirrel.egg-info/PKG-INFO` & `hypersquirrel-1.0.32/hypersquirrel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.31
+Version: 1.0.32
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.31/hypersquirrel.egg-info/SOURCES.txt` & `hypersquirrel-1.0.32/hypersquirrel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.31/setup.py` & `hypersquirrel-1.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hypersquirrel",
-    version="v1.0.31",
+    version="v1.0.32",
     author="vka",
     description="Scrapes posts from various websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `hypersquirrel-1.0.31/ytdlwrapper/ytdlpscrape.py` & `hypersquirrel-1.0.32/ytdlwrapper/ytdlpscrape.py`

 * *Files identical despite different names*

