# Comparing `tmp/hypersquirrel-1.0.32.tar.gz` & `tmp/hypersquirrel-1.0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypersquirrel-1.0.32.tar", last modified: Mon Jul 31 13:53:25 2023, max compression
+gzip compressed data, was "hypersquirrel-1.0.33.tar", last modified: Mon Jul 31 15:23:12 2023, max compression
```

## Comparing `hypersquirrel-1.0.32.tar` & `hypersquirrel-1.0.33.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.967520 hypersquirrel-1.0.32/hypersquirrel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.971520 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/instagram.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreter/ph.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/literalinterpreterfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.975520 hypersquirrel-1.0.32/hypersquirrel/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/buondua.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/cosplayporntube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/drts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/ehen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/fseg.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/googleimagesearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hcos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hellp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/hnlg.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/lgbb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/nh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/nlgs.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/opendir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/sb.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/sbgx.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/v2ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/vg.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/xh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/xv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraper/youtubeapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/scraperfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/hypersquirrel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.971520 hypersquirrel-1.0.32/hypersquirrel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 13:53:25.000000 hypersquirrel-1.0.32/hypersquirrel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:25.979520 hypersquirrel-1.0.32/ytdlwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/ytdlwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 13:53:12.000000 hypersquirrel-1.0.32/ytdlwrapper/ytdlpscrape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.933056 hypersquirrel-1.0.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 15:23:12.933056 hypersquirrel-1.0.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.929056 hypersquirrel-1.0.33/hypersquirrel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.929056 hypersquirrel-1.0.33/hypersquirrel/literalinterpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/literalinterpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/literalinterpreter/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/literalinterpreter/instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/literalinterpreter/ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/literalinterpreterfactory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.933056 hypersquirrel-1.0.33/hypersquirrel/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/buondua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/cosplayporntube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/drts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/ehen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/fseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/googleimagesearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/hcos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/hellp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/hnlg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/lgbb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/nh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/nlgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/opendir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/sb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/sbgx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/v2ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/vg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/xh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/xv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraper/youtubeapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/scraperfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/hypersquirrel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.929056 hypersquirrel-1.0.33/hypersquirrel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-31 15:23:12.000000 hypersquirrel-1.0.33/hypersquirrel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-31 15:23:12.000000 hypersquirrel-1.0.33/hypersquirrel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:23:12.000000 hypersquirrel-1.0.33/hypersquirrel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-31 15:23:12.000000 hypersquirrel-1.0.33/hypersquirrel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-31 15:23:12.000000 hypersquirrel-1.0.33/hypersquirrel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:23:12.933056 hypersquirrel-1.0.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:12.933056 hypersquirrel-1.0.33/ytdlwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/ytdlwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 15:23:00.000000 hypersquirrel-1.0.33/ytdlwrapper/ytdlpscrape.py
```

### Comparing `hypersquirrel-1.0.32/LICENSE` & `hypersquirrel-1.0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/PKG-INFO` & `hypersquirrel-1.0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.32
+Version: 1.0.33
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.32/hypersquirrel/core.py` & `hypersquirrel-1.0.33/hypersquirrel/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,14 @@
     def __post_init__(self):
         assert self.url or self.html
         if self.url and self.is_multipage:
             assert isinstance(self.page_min, int)
             assert isinstance(self.page_max, int)
             assert self.page_min < self.page_max
 
-    def scrape(self, scraper: Callable[[str], Iterator[dict]], url=None):
+    def scrape_by_url(self, scraper: Callable[[str], Iterator[dict]]):
         def generate():
             for page in range(self.page_min, self.page_max + 1):
-                substituted_url = (url or self.url).replace("${page}", str(page))
+                substituted_url = self.url.replace("${page}", str(page))
                 yield from scraper(substituted_url)
 
         yield from itertools.islice(generate(), self.max_items or sys.maxsize)
```

### Comparing `hypersquirrel-1.0.32/hypersquirrel/entry.py` & `hypersquirrel-1.0.33/hypersquirrel/entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,22 @@
     return Watchlist(
         url=url,
         max_items=max_items
     )
 
 
 def scrape(w: Watchlist) -> Iterator[dict]:
-    return w.scrape(get_scraper(w))
+    """"
+    Returns a generator to grab 'file' objects
+    """
+    scraper = get_scraper(w)
+    if w.html:
+        return scraper(w.html)
+
+    return w.scrape_by_url(scraper)
 
 
 def scrape_literal_urls(urls: List[str]) -> dict:
     for url in set(urls):
         interpreter = get_interpreter(url)
         if interpreter:
             yield from interpreter(url)
```

### Comparing `hypersquirrel-1.0.32/hypersquirrel/literalinterpreterfactory.py` & `hypersquirrel-1.0.33/hypersquirrel/literalinterpreterfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/buondua.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/buondua.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/cosplayporntube.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/cosplayporntube.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/drts.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/drts.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/ehen.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/ehen.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/fseg.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/fseg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/hcos.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/hcos.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/hellp.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/hellp.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/hnlg.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/hnlg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/lgbb.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/lgbb.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/nh.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/nh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/nlgs.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/nlgs.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/reddit.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/reddit.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/sb.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/sb.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,17 @@
             video_id, headers={'Cookie': 'country=US'})
 
     tree = html.fromstring(get_body_with_ytdl())
     host_url = get_host_url(url)
     yield from _scrape(tree, host_url)
 
 
-def scrape_html(w: Watchlist):
-    assert w.html
-    tree = html.fromstring(w.html)
+def scrape_html(html_string: str):
+    assert html_string
+    tree = html.fromstring(html_string)
     yield from _scrape(tree, "https://spankbang.com")
 
 
 def is_sb_html(w: Watchlist):
     if w.html:
         tree = html.fromstring(w.html)
         title = head(tree.xpath("//head/title"))
```

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/sbgx.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/sbgx.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/v2ph.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/v2ph.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/vg.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/vg.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/xh.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/xh.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/xv.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/xv.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraper/youtubeapi.py` & `hypersquirrel-1.0.33/hypersquirrel/scraper/youtubeapi.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/scraperfactory.py` & `hypersquirrel-1.0.33/hypersquirrel/scraperfactory.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel/util.py` & `hypersquirrel-1.0.33/hypersquirrel/util.py`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/hypersquirrel.egg-info/PKG-INFO` & `hypersquirrel-1.0.33/hypersquirrel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypersquirrel
-Version: 1.0.32
+Version: 1.0.33
 Summary: Scrapes posts from various websites
 Home-page: UNKNOWN
 Author: vka
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `hypersquirrel-1.0.32/hypersquirrel.egg-info/SOURCES.txt` & `hypersquirrel-1.0.33/hypersquirrel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypersquirrel-1.0.32/setup.py` & `hypersquirrel-1.0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hypersquirrel",
-    version="v1.0.32",
+    version="v1.0.33",
     author="vka",
     description="Scrapes posts from various websites",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=("test",)),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `hypersquirrel-1.0.32/ytdlwrapper/ytdlpscrape.py` & `hypersquirrel-1.0.33/ytdlwrapper/ytdlpscrape.py`

 * *Files identical despite different names*

