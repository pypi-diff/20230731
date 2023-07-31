# Comparing `tmp/SlyYTDAPI-0.2.0.tar.gz` & `tmp/SlyYTDAPI-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SlyYTDAPI-0.2.0.tar", last modified: Wed Mar  1 10:59:26 2023, max compression
+gzip compressed data, was "SlyYTDAPI-0.3.0.tar", last modified: Mon Jul 31 05:54:05 2023, max compression
```

## Comparing `SlyYTDAPI-0.2.0.tar` & `SlyYTDAPI-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 10:59:26.586097 SlyYTDAPI-0.2.0/
--rw-rw-rw-   0        0        0     1088 2023-02-24 12:14:33.000000 SlyYTDAPI-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     3372 2023-03-01 10:59:26.585068 SlyYTDAPI-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1658 2023-03-01 10:58:44.000000 SlyYTDAPI-0.2.0/README.md
--rw-rw-rw-   0        0        0      897 2023-03-01 10:50:16.000000 SlyYTDAPI-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-01 10:59:26.586097 SlyYTDAPI-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-01 10:59:26.547072 SlyYTDAPI-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 10:59:26.557068 SlyYTDAPI-0.2.0/src/SlyYTDAPI/
--rw-rw-rw-   0        0        0      155 2023-03-01 10:55:49.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI/__init__.py
--rw-rw-rw-   0        0        0      558 2023-03-01 10:56:48.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI/__main__.py
--rw-rw-rw-   0        0        0     4740 2023-03-01 10:38:06.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI/members.py
--rw-rw-rw-   0        0        0    10798 2023-03-01 10:57:10.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI/ytdapi.py
-drwxrwxrwx   0        0        0        0 2023-03-01 10:59:26.577067 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/
--rw-rw-rw-   0        0        0     3372 2023-03-01 10:59:26.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      423 2023-03-01 10:59:26.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 10:59:26.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2023-03-01 10:59:26.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-01 10:59:26.000000 SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-01 10:59:26.583072 SlyYTDAPI-0.2.0/test/
--rw-rw-rw-   0        0        0      199 2023-03-01 10:47:52.000000 SlyYTDAPI-0.2.0/test/test_channels.py
--rw-rw-rw-   0        0        0      328 2023-03-01 10:45:44.000000 SlyYTDAPI-0.2.0/test/test_members.py
--rw-rw-rw-   0        0        0      354 2023-03-01 10:47:13.000000 SlyYTDAPI-0.2.0/test/test_playlists.py
--rw-rw-rw-   0        0        0      512 2023-03-01 10:46:43.000000 SlyYTDAPI-0.2.0/test/test_readme.py
--rw-rw-rw-   0        0        0      313 2023-03-01 10:46:56.000000 SlyYTDAPI-0.2.0/test/test_search.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:05.575524 SlyYTDAPI-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2023-02-24 12:14:33.000000 SlyYTDAPI-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     3372 2023-07-31 05:54:05.574524 SlyYTDAPI-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1658 2023-03-01 10:58:44.000000 SlyYTDAPI-0.3.0/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-31 05:49:49.000000 SlyYTDAPI-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:54:05.575524 SlyYTDAPI-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:05.562513 SlyYTDAPI-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:05.567517 SlyYTDAPI-0.3.0/src/SlyYTDAPI/
+-rw-rw-rw-   0        0        0      155 2023-03-01 10:55:49.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-03-17 05:48:35.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI/__main__.py
+-rw-rw-rw-   0        0        0      814 2023-03-17 08:41:40.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI/livechat.py
+-rw-rw-rw-   0        0        0     4740 2023-03-01 10:38:06.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI/members.py
+-rw-rw-rw-   0        0        0    11900 2023-07-31 03:54:33.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI/ytdapi.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:05.570520 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/
+-rw-rw-rw-   0        0        0     3372 2023-07-31 05:54:05.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2023-07-31 05:54:05.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:54:05.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-31 05:54:05.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 05:54:05.000000 SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 05:54:05.574524 SlyYTDAPI-0.3.0/test/
+-rw-rw-rw-   0        0        0      261 2023-07-31 03:39:11.000000 SlyYTDAPI-0.3.0/test/test_channels.py
+-rw-rw-rw-   0        0        0      382 2023-07-31 03:39:19.000000 SlyYTDAPI-0.3.0/test/test_members.py
+-rw-rw-rw-   0        0        0      406 2023-07-31 03:39:33.000000 SlyYTDAPI-0.3.0/test/test_playlists.py
+-rw-rw-rw-   0        0        0      365 2023-07-31 03:39:48.000000 SlyYTDAPI-0.3.0/test/test_search.py
+-rw-rw-rw-   0        0        0      565 2023-07-31 03:40:12.000000 SlyYTDAPI-0.3.0/test/test_yt_readme.py
```

### Comparing `SlyYTDAPI-0.2.0/LICENSE` & `SlyYTDAPI-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SlyYTDAPI-0.2.0/PKG-INFO` & `SlyYTDAPI-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SlyYTDAPI
-Version: 0.2.0
+Version: 0.3.0
 Summary: No-boilerplate, async and typed YouTube Data API access.
 Author: Dunkyl 🔣🔣
 License: The MIT License
         
         Copyright © 2021 Maroue Reus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `SlyYTDAPI-0.2.0/README.md` & `SlyYTDAPI-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SlyYTDAPI-0.2.0/pyproject.toml` & `SlyYTDAPI-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "SlyYTDAPI"
-version = "0.2.0"
+version = "0.3.0"
 description = "No-boilerplate, async and typed YouTube Data API access."
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file="LICENSE" }
 authors = [{name="Dunkyl 🔣🔣"}]
-dependencies = [ 'SlyAPI >= 0.4.3' ]
+dependencies = [ 'SlyAPI >= 0.5.0' ]
 
 [project.optional-dependencies]
 dev = [
     # testing
     'pytest',
     'pytest-asyncio',
```

### Comparing `SlyYTDAPI-0.2.0/src/SlyYTDAPI/__main__.py` & `SlyYTDAPI-0.3.0/src/SlyYTDAPI/__main__.py`

 * *Files identical despite different names*

### Comparing `SlyYTDAPI-0.2.0/src/SlyYTDAPI/members.py` & `SlyYTDAPI-0.3.0/src/SlyYTDAPI/members.py`

 * *Files identical despite different names*

### Comparing `SlyYTDAPI-0.2.0/src/SlyYTDAPI/ytdapi.py` & `SlyYTDAPI-0.3.0/src/SlyYTDAPI/ytdapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from enum import Enum
 from datetime import datetime
 from typing import TypeVar, Any
+from warnings import warn
 from SlyAPI import *
 
 SCOPES_ROOT = 'https://www.googleapis.com/auth/youtube'
 
 class Scope:
     READONLY     = F"{SCOPES_ROOT}.readonly"
     MEMBERS      = F"{SCOPES_ROOT}.channel-memberships.creator"
@@ -39,46 +40,54 @@
 class CommentOrder(Enum):
     RELEVANCE    = 'relevance'
     TIME         = 'time'
 
 ISO8601_PERIOD = re.compile(r'P(\d+)?T(?:(\d{1,2})H)?(?:(\d{1,2})M)?(\d{1,2})S')
 
 def yt_date(date: str) -> datetime:
-    return datetime.strptime(date, '%Y-%m-%dT%H:%M:%SZ')
+    try:
+        return datetime.strptime(date, '%Y-%m-%dT%H:%M:%S.%fZ')
+    except ValueError:
+        return datetime.strptime(date, '%Y-%m-%dT%H:%M:%SZ')
 
 W = TypeVar('W')
 T = TypeVar('T')
 
 def get_dict_path(d: dict[str, Any], *keys: str) -> Any:
     for key in keys:
         if key not in d:
             return None
         d = d[key]
     return d
     
 class Comment:
     id: str
     # part: snippet
-    author_name: str
+    author_display_name: str
     author_channel_id: str
     body: str
     created_at: datetime
     # part: replies
     replies: list['Comment']|None
 
+    @property
+    def author_name(self):
+        warn("author_name is deprecated, please use author_display_name")
+        return self.author_display_name
+
     def __init__(self, source: dict[str, Any]):
         # case of top-level comment
         if tlc := source.get('snippet', {}).get('topLevelComment'):
             replies: list[Any] = source.get('replies', {}).get('comments', [])
             self.replies = [Comment(r) for r in replies]
             source = tlc
             
         self.id = source['id']
         if snippet := source.get('snippet'):
-            self.author_name = snippet['authorDisplayName']
+            self.display_name = snippet['authorDisplayName']
             self.author_channel_id = snippet['authorChannelId']['value']
             self.body = snippet['textDisplay']
             self.created_at = yt_date(snippet['publishedAt'])
         
 
 
 class Video:
@@ -160,50 +169,61 @@
         return F"https://www.youtube.com/playlist?list={self.id}"
 
 class Channel:
     _youtube: 'YouTubeData'
     id: str
 
     # part: snippet
-    name: str
+    display_name: str
     description: str
     created_at: datetime
+    at_username: str
     profile_image_url: str|None = None
-    custom_url: str|None = None
 
     # part: contentDetails
     uploads_playlist: Playlist
 
     # part: statistics
     view_count: int
     subscriber_count: int
     video_count: int
 
+    @property
+    def custom_url(self):
+        warn("custom_url is deprecated, please use at_username")
+        return self.at_username
+
+    
+    @property
+    def name(self):
+        warn("name is deprecated, please use display_name")
+        return self.display_name
+
     def __init__(self, source: dict[str, Any], yt: 'YouTubeData'):
         self._youtube = yt
 
         self.id = source['id']
         if snippet := source.get('snippet'):
-            self.name = snippet['title']
+            self.display_name = snippet['title']
             self.description = snippet['description']
             self.created_at = yt_date(snippet['publishedAt'])
             self.profile_image_url = snippet.get('thumbnails', {}).get('default', {}).get('url')
-            self.custom_url = snippet.get('customUrl')
+            self.at_username = snippet.get('customUrl')
 
         if details := source.get('contentDetails'):
             self.uploads_playlist = Playlist(details['relatedPlaylists']['uploads'], yt)
 
         if stats := source.get('statistics'):
             self.view_count = int(stats['viewCount'])
             self.subscriber_count = int(stats['subscriberCount'])
             self.video_count = int(stats['videoCount'])
 
     def link(self) -> str:
-        if self.custom_url:
-            return F"https://www.youtube.com/c/{self.custom_url}"
+        if self.at_username:
+            return F"https://www.youtube.com/c/{self.at_username}"
         else:
             return F"https://www.youtube.com/channels/{self.id}"
 
     async def update(self):
         new = await self._youtube.channel(self.id)
         self.__dict__.update(new.__dict__)
 
@@ -233,23 +253,31 @@
     def _channels_list(self,
         channel_ids: list[str]|None=None,
         mine: bool=False,
         parts: Part|set[Part]=Part.SNIPPET,
         limit: int|None=None) -> AsyncTrans[Channel]:
         if mine==bool(channel_ids):
             raise ValueError("Must specify exactly one of channel id or mine in channel list query")
-        params = {
-            'part': parts,
-            'mine': mine if mine else None,
-            'id': ','.join(channel_ids) if channel_ids else None,
-            'maxResults': min(50, limit) if limit else None,
-        }
-        return self.paginated(
-            '/channels', params, limit
-            ).map(lambda r: Channel(r, self))
+        maxResults = min(50, limit) if limit else None # per-page limit
+        params = { 'part': parts, 'maxResults': maxResults }
+        if channel_ids:
+            channel_ids = list(set(channel_ids or [])) # deduplicate IDs
+            channels_chunks50 = [
+                channel_ids[i: i + 50] for i in range(0, len(channel_ids), 50)
+            ]
+            async def page_chunks():
+                for ids in channels_chunks50:
+                    p = params | { 'id': ','.join(ids) }
+                    async for c in self.paginated('/channels', p, limit):
+                        yield c
+            return AsyncLazy(page_chunks()).map(lambda r: Channel(r, self))
+        else: # mine
+            return self.paginated(
+                '/channels', params | { 'mine': True }, limit
+                ).map(lambda r: Channel(r, self))
 
     def videos(self,
         video_ids: list[str],
         parts: Part|set[Part]={Part.ID,Part.SNIPPET}) -> AsyncTrans[Video]:
         params = {
             'part': parts,
             'id': ','.join(video_ids),
```

### Comparing `SlyYTDAPI-0.2.0/src/SlyYTDAPI.egg-info/PKG-INFO` & `SlyYTDAPI-0.3.0/src/SlyYTDAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SlyYTDAPI
-Version: 0.2.0
+Version: 0.3.0
 Summary: No-boilerplate, async and typed YouTube Data API access.
 Author: Dunkyl 🔣🔣
 License: The MIT License
         
         Copyright © 2021 Maroue Reus
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `SlyYTDAPI-0.2.0/test/test_readme.py` & `SlyYTDAPI-0.3.0/test/test_yt_readme.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import os
 from SlyYTDAPI import *
-
+test_dir = os.path.dirname(__file__)
 async def test_readme():
-    yt = YouTubeData(open('./test/api_key.txt').read())
+    yt = YouTubeData(open(F'{test_dir}/api_key.txt').read())
 
     my_video = await yt.video('dQw4w9WgXcQ')
     print(F"Check this out!\n{my_video.link()}")
 
     # keep it simple
     all_comments = await my_video.comments(limit=10) # list[Comment]
 
     # or opt in to generators
     print('\n---\n'.join([
-        F"{c.author_name} > {c.body}"
+        F"{c.display_name} > {c.body}"
         async for c in my_video.comments(limit=10)
     ]))
 
     # ---
 
     assert len(all_comments) > 0
```

