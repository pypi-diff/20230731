# Comparing `tmp/wikichangewatcher-0.0.3-py3-none-any.whl.zip` & `tmp/wikichangewatcher-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 10196 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-30 21:36 wikichangewatcher/__init__.py
--rw-rw-rw-  2.0 fat    10132 b- defN 23-Jul-30 21:33 wikichangewatcher/wikichangewatcher.py
--rw-rw-rw-  2.0 fat    10761 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9936 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      618 b- defN 23-Jul-30 21:36 wikichangewatcher-0.0.3.dist-info/RECORD
-7 files, 32043 bytes uncompressed, 9090 bytes compressed:  71.6%
+Zip file size: 11713 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      486 b- defN 23-Jul-31 03:08 wikichangewatcher/__init__.py
+-rw-rw-rw-  2.0 fat    10526 b- defN 23-Jul-31 01:46 wikichangewatcher/wikichangewatcher.py
+-rw-rw-rw-  2.0 fat    10761 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    16417 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      619 b- defN 23-Jul-31 03:11 wikichangewatcher-0.1.0.dist-info/RECORD
+7 files, 38919 bytes uncompressed, 10607 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: wikichangewatcher/__init__.py
 Comment: 
 
 Filename: wikichangewatcher/wikichangewatcher.py
 Comment: 
 
-Filename: wikichangewatcher-0.0.3.dist-info/LICENSE
+Filename: wikichangewatcher-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: wikichangewatcher-0.0.3.dist-info/METADATA
+Filename: wikichangewatcher-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: wikichangewatcher-0.0.3.dist-info/WHEEL
+Filename: wikichangewatcher-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: wikichangewatcher-0.0.3.dist-info/top_level.txt
+Filename: wikichangewatcher-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: wikichangewatcher-0.0.3.dist-info/RECORD
+Filename: wikichangewatcher-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wikichangewatcher/__init__.py

```diff
@@ -1,7 +1,7 @@
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 
 from wikichangewatcher.wikichangewatcher import FieldFilter, FilterCollection, IpV4Filter, WikiChangeWatcher, MatchType
 from wikichangewatcher.wikichangewatcher import FieldStringFilter, FieldRegexMatchFilter, FieldRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import UsernameFilter, UsernameRegexMatchFilter, UsernameRegexSearchFilter
 from wikichangewatcher.wikichangewatcher import PageUrlFilter, PageUrlRegexMatchFilter, PageUrlRegexSearchFilter
```

## wikichangewatcher/wikichangewatcher.py

```diff
@@ -253,14 +253,22 @@
     """
     def __init__(self, *filters):
         self._thread = None
         self._stop_event = threading.Event()
         self._filters = filters
         self._session = requests.Session()
         self._client = SSEClient(WIKIMEDIA_URL, session=self._session)
+        self._on_edit_handler = None
+
+    def on_edit(self, on_edit_handler: Callable[[dict], None]) -> Self:
+        """
+        Sets handler to run whenever any edit event is received (before any filters are processed)
+        """
+        self._on_edit_handler = on_edit_handler
+        return self
 
     def add_filter(self, fltr: Type[FieldFilter]) -> Self:
         """
         Add a new filter to the list of active filters
         """
         self._filters.append(fltr)
         return self
@@ -307,10 +315,13 @@
 
             if event.event == "message":
                 try:
                     change = json.loads(event.data)
                 except ValueError:
                     continue
 
+                if self._on_edit_handler:
+                    self._on_edit_handler(change)
+
                 for f in self._filters:
                     if f.check_match(change):
                         f.run_on_match(change)
```

## Comparing `wikichangewatcher-0.0.3.dist-info/LICENSE` & `wikichangewatcher-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `wikichangewatcher-0.0.3.dist-info/METADATA` & `wikichangewatcher-0.1.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikichangewatcher
-Version: 0.0.3
+Version: 0.1.0
 Summary: Real-time monitoring/filtering of global Wikipedia page edits
 Home-page: http://github.com/eriknyquist/wikichangewatcher
 Author: Erik Nyquist
 Author-email: eknyquist@gmail.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -23,26 +23,30 @@
 Requires-Dist: sseclient
 
 WikiChangeWatcher
 =================
 
 .. contents:: Table of Contents
 
+.. image:: https://github.com/eriknyquist/wikichangewatcher/blob/80ffe25fd4d0d694bba545bd46dcc31a37d664e7/images/wikiwatcher_logo.png
+
 Introduction
 ============
 
 Wikipedia provides an `SSE Stream <https://en.wikipedia.org/wiki/Server-sent_events>`_  of
 all edits made to any page across Wikipedia, which allows you to watch all edits made to all wikipedia
 pages in real time.
 
-``WikiChangeWatcher`` is just a thin wrapper around an SSE client, pointed at the URL for
-the SSE stream for wikipedia edits, with some filtering features that allow you to watch for page edit
-events with specific attributes (e.g. `"anonymous" <https://en.wikipedia.org/wiki/Wikipedia:IP_edits_are_not_anonymous>`_
-edits with IP addresses in specific ranges, or edits made by a wikipedia user whose username matches
-a specific regular expression).
+``WikiChangeWatcher`` is an SSE client that watches the SSE stream of wikipedia page edits,
+with some filtering features that allow you to watch for page edit events with specific attributes
+(e.g. `"anonymous" <https://en.wikipedia.org/wiki/Wikipedia:IP_edits_are_not_anonymous>`_
+edits with IP addresses in specific ranges, or edits made to a specific page, or edits made by a wikipedia
+user whose username matches a specific regular expression).
+
+This package is inspired by `Tom Scott's WikiParliament project <https://www.tomscott.com/wikiparliament/>`_.
 
 Install
 =======
 
 Install using ``pip``.
 
 ::
@@ -250,7 +254,155 @@
 
     # Watch for page edits forever until KeyboardInterrupt
     try:
         while True:
             time.sleep(0.1)
     except KeyboardInterrupt:
         wc.stop()
+
+Monitoring "anonymous" edits made from IP address ranges owned by US government depts./agencies
+-----------------------------------------------------------------------------------------------
+
+The following example watches for anonymous page edits to *any* wikipedia page,
+from IP address ranges that were found to be publicly listed as owned by various
+US government department and agencies (mostly California, some federal).
+
+If you want to look up some IP addresses owned by your local governments, or companies, it's pretty easy,
+I just went to ``https://ip-netblocks.whoisxmlapi.com/`` and searched for "california department of"
+as the company name.
+
+.. code:: python
+
+    # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
+    # wikipedia page from IP address ranges that are publicly listed as being owned by various US government departments
+
+    import time
+    from wikichangewatcher import WikiChangeWatcher, IpV4Filter, FilterCollection, MatchType
+
+    # Callback function to run whenever an event matching one of our IPv4 address ranges is seen
+    def match_handler(json_data):
+        """
+        json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
+        as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
+        """
+        print("{user} edited {title_url}".format(**json_data))
+
+    filters = [
+        IpV4Filter("136.200.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of water resources
+        IpV4Filter("151.143.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of technology
+        IpV4Filter("160.88.0-255.0-255").on_match(match_handler),   # IP range assigned to CA dept. of insurance
+        IpV4Filter("192.56.110.0-255").on_match(match_handler),     # IP range #1 assigned to CA dept. of corrections
+        IpV4Filter("153.48.0-255.0-255").on_match(match_handler),   # IP range #2 assigned to CA dept. of corrections
+        IpV4Filter("149.136.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of transportation
+        IpV4Filter("192.251.92.0-255").on_match(match_handler),     # IP range assigned to CA dept. of general services
+        IpV4Filter("159.145.0-255.0-255").on_match(match_handler),  # IP range assigned to CA dept. of consumer affairs
+        IpV4Filter("167.10.0-255.0-255").on_match(match_handler),   # IP range assigned to CA dept. of justice
+        IpV4Filter("192.58.200-203.0-255").on_match(match_handler)  # IP range assigned to Bureau of Justice Statistics in WA
+    ]
+
+    wc = WikiChangeWatcher(*filters)
+
+    wc.run()
+
+    # Watch for page edits forever until KeyboardInterrupt
+    try:
+        while True:
+            time.sleep(0.1)
+    except KeyboardInterrupt:
+        wc.stop()
+
+
+Calculating a running average of page-edits-per-minute for all of wikipedia
+---------------------------------------------------------------------------
+
+The following example watches for any edit to any wikipedia page, and updates a
+running average of the rate of page edits per minute, which is printed to stdout
+once every 5 seconds.
+
+.. code:: python
+
+    # Example script showing how to use WikiChangeWatcher to watch for "anonymous" edits to any
+    # wikipedia page from specific IP address ranges
+
+    import time
+    import statistics
+    import queue
+    from typing import Callable, Self
+
+    from wikichangewatcher import WikiChangeWatcher
+
+
+    # Max. number of samples in the averaging window
+    MAX_WINDOW_LEN = 6
+
+    # Interval between new samples for the averaging window, in seconds
+    INTERVAL_SECS = 5
+
+
+    class EditRateCounter():
+        """
+        Tracks total number of page edits per minute across all of wikipedia,
+        using a simple averaging window
+        """
+        def __init__(self, interval_secs=INTERVAL_SECS):
+            self._edit_count = 0
+            self._start_time = None
+            self._interval_secs = interval_secs
+            self._queue = queue.Queue()
+            self._window = []
+
+        # Callback function to run whenever an edit event is seen
+        def edit_handler(self, json_data):
+            """
+            json_data is a JSON-encoded event from the WikiMedia "recent changes" event stream,
+            as described here: https://www.mediawiki.org/wiki/Manual:RCFeed
+            """
+            self._edit_count += 1
+
+        # Add an edit rate sample to the averaging window, and return the new average
+        def _add_to_window(self, edits_per_min):
+            self._window.append(edits_per_min)
+            if len(self._window) > MAX_WINDOW_LEN:
+                self._window.pop(0)
+
+            return statistics.mean(self._window)
+
+        def run(self):
+            if self._start_time is None:
+                self._start_time = time.time()
+
+            if (time.time() - self._start_time) >= self._interval_secs:
+                # interval is up, calculate new rate and put it on the queue
+                edits_per_min = float(self._edit_count) * (60.0 / self._interval_secs)
+                self._queue.put((self._add_to_window(edits_per_min), self._edit_count))
+                self._edit_count = 0
+                self._start_time = time.time()
+
+        def get_rate(self):
+            ret = None
+
+            try:
+                ret = self._queue.get(block=False)
+            except queue.Empty:
+                pass
+
+            return ret
+
+
+    # Create rate counter class to monitor page edit rate over time
+    ratecounter = EditRateCounter()
+
+    # Create a watcher with no filters-- we want to see every single edit
+    wc = WikiChangeWatcher().on_edit(ratecounter.edit_handler)
+
+    wc.run()
+
+    # Watch for page edits forever until KeyboardInterrupt
+    try:
+        while True:
+            ratecounter.run()
+            new_rate = ratecounter.get_rate()
+            if new_rate:
+                rate, since_last = new_rate
+                print(f"{rate:.2f} avg. page edits per min. ({since_last} in the last {INTERVAL_SECS} secs)")
+    except KeyboardInterrupt:
+        wc.stop()
```

