# Comparing `tmp/drukarnia-api-1.1.1.tar.gz` & `tmp/drukarnia-api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drukarnia-api-1.1.1.tar", last modified: Mon Jul 24 13:13:17 2023, max compression
+gzip compressed data, was "drukarnia-api-1.1.2.tar", last modified: Sun Jul 30 22:32:57 2023, max compression
```

## Comparing `drukarnia-api-1.1.1.tar` & `drukarnia-api-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.512018 drukarnia-api-1.1.1/drukarnia_api/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.516018 drukarnia-api-1.1.1/drukarnia_api/network/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/cookie.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/network/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/drukarnia_api/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/article.py
--rw-r--r--   0 runner    (1001) docker     (123)    18934 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/objects/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/drukarnia_api/shortcuts/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/shortcuts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/drukarnia_api/shortcuts/class_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 13:13:17.512018 drukarnia-api-1.1.1/drukarnia_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 13:13:17.000000 drukarnia-api-1.1.1/drukarnia_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 13:13:17.520018 drukarnia-api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-24 13:13:03.000000 drukarnia-api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.507790 drukarnia-api-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-30 22:32:57.507790 drukarnia-api-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.503790 drukarnia-api-1.1.2/drukarnia_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.503790 drukarnia-api-1.1.2/drukarnia_api/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/cookie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/network/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.503790 drukarnia-api-1.1.2/drukarnia_api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/article.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/objects/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.507790 drukarnia-api-1.1.2/drukarnia_api/shortcuts/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/shortcuts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/drukarnia_api/shortcuts/class_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:32:57.503790 drukarnia-api-1.1.2/drukarnia_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-30 22:32:57.000000 drukarnia-api-1.1.2/drukarnia_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-30 22:32:57.000000 drukarnia-api-1.1.2/drukarnia_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:32:57.000000 drukarnia-api-1.1.2/drukarnia_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-30 22:32:57.000000 drukarnia-api-1.1.2/drukarnia_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-30 22:32:57.000000 drukarnia-api-1.1.2/drukarnia_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:32:57.507790 drukarnia-api-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-30 22:32:46.000000 drukarnia-api-1.1.2/setup.py
```

### Comparing `drukarnia-api-1.1.1/LICENSE` & `drukarnia-api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/PKG-INFO` & `drukarnia-api-1.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,17 @@
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
     search = Search()
     
     async with search:
-        cupomanka, *_ = await search.find_author('cupomanka') 
+        search_res = await search.find_author('cupomanka')
+        # most probable
+        cupomanka = search_res[0]
 
         # Collect all data about the user
         await cupomanka.collect_data()
 
         # Get user articles
         articles = await cupomanka.articles
```

### Comparing `drukarnia-api-1.1.1/README.md` & `drukarnia-api-1.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
     search = Search()
     
     async with search:
-        cupomanka, *_ = await search.find_author('cupomanka') 
+        search_res = await search.find_author('cupomanka')
+        # most probable
+        cupomanka = search_res[0]
 
         # Collect all data about the user
         await cupomanka.collect_data()
 
         # Get user articles
         articles = await cupomanka.articles
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/network/connection.py` & `drukarnia-api-1.1.2/drukarnia_api/network/connection.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/network/cookie.py` & `drukarnia-api-1.1.2/drukarnia_api/network/cookie.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/network/exceptions.py` & `drukarnia-api-1.1.2/drukarnia_api/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/network/headers.py` & `drukarnia-api-1.1.2/drukarnia_api/network/headers.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/network/utils.py` & `drukarnia-api-1.1.2/drukarnia_api/network/utils.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/article.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/article.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from warnings import warn
 from aiohttp import ClientSession
 
 from drukarnia_api.objects.base_object import DrukarniaElement
 from drukarnia_api.shortcuts import data2authors, data2articles, data2tags, data2comments
 
-from typing import TYPE_CHECKING, Tuple, Dict
+from typing import TYPE_CHECKING, Tuple, Dict, Union
 
 if TYPE_CHECKING:  # always False, used for type hints
     from drukarnia_api.objects.author import Author
     from drukarnia_api.objects.tag import Tag
     from drukarnia_api.objects.comment import Comment
 
 
@@ -85,15 +85,15 @@
             raise ValueError('section_id must be passed for bookmarking')
 
         else:
             await self.request('post', '/api/articles/bookmarks',
                                data={"article": await self.article_id, "list": section_id})
 
     @DrukarniaElement.requires_attributes(['slug'])
-    async def collect_data(self, return_: bool = False) -> Dict or None:
+    async def collect_data(self, return_: bool = False) -> Union[Dict, None]:
         """
         Collects the article's data and updates the object's attributes.
 
         Parameters:
         - return_ (bool): If True, returns the collected data.
 
         Returns:
@@ -325,15 +325,15 @@
         if any(map(lambda el: isinstance(el, str), tags)):
             warn("Tag's data is incomplete, use collect_data method before in order to obtain whole data.")
             tags = map(lambda el: {'_id': el}, tags)
 
         return await data2tags(tags, self.session)
 
     @property
-    async def main_article_tag(self) -> 'Tag' or None:
+    async def main_article_tag(self) -> Union['Tag', None]:
         """
         Retrieves the main tag of the article.
 
         Returns:
         - 'Tag' or None: The main tag of the article if available, otherwise None.
         """
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/author.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/author.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, Tuple, List
+from typing import Dict, Tuple, List, Union
 from aiohttp import ClientSession
 
 from drukarnia_api.objects.base_object import DrukarniaElement
 from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
 
 from typing import TYPE_CHECKING
 
@@ -40,15 +40,15 @@
         """
 
         await self.cookies.login(email, password, self)
         self._update_data(self.cookies.owner['user'])
 
     @DrukarniaElement.requires_attributes(['author_id'])
     async def get_followers(self, create_authors: bool = True, offset: int = 0, results_per_page: int = 20,
-                            n_collect: int = None, *args, **kwargs) -> Tuple['Author'] or Tuple[Dict]:
+                            n_collect: int = None, *args, **kwargs) -> Union[Tuple['Author'], Tuple[Dict]]:
         """
         Get the followers of the author.
 
         Parameters:
             create_authors (bool, optional): Whether to create Author objects for followers. Defaults to True.
             offset (int, optional): Offset for pagination. Defaults to 0.
             results_per_page (int, optional): Number of results per page for pagination. Defaults to 20.
@@ -67,15 +67,15 @@
         if create_authors:
             followers = await data2authors(followers, self.session)
 
         return followers
 
     @DrukarniaElement.requires_attributes(['author_id'])
     async def get_followings(self, create_authors: bool = True, offset: int = 0, results_per_page: int = 20,
-                             n_collect: int = None, *args, **kwargs) -> Tuple['Author'] or Tuple[Dict]:
+                             n_collect: int = None, *args, **kwargs) -> Union[Tuple['Author'], Tuple[Dict]]:
         """
         Get the followings of the author.
 
         Parameters:
             create_authors (bool, optional): Whether to create Author objects for followings. Defaults to True.
             offset (int, optional): Offset for pagination. Defaults to 0.
             results_per_page (int, optional): Number of results per page for pagination. Defaults to 20.
@@ -113,15 +113,15 @@
         """
         return await self.multi_page_request('/api/notifications',
                                              offset, results_per_page, n_collect,
                                              *args, **kwargs)
 
     async def get_reads_history(self, create_articles: bool = True, offset: int = 0,
                                 results_per_page: int = 20, n_collect: int = None,
-                                *args, **kwargs) -> List[Dict] or List['Article']:
+                                *args, **kwargs) -> Union[List[Dict], List['Article']]:
         """
         Get the reading history of the author.
 
         Parameters:
             create_articles (bool, optional): Whether to create Article objects for read history. Defaults to True.
             offset (int, optional): Offset for pagination. Defaults to 0.
             results_per_page (int, optional): Number of results per page for pagination. Defaults to 20.
@@ -218,15 +218,15 @@
 
         if unblock:
             await self.request('patch', f'/api/relationships/block/{await self.author_id}')
             return None
 
         await self.request('put', f'/api/relationships/block/{await self.author_id}')
 
-    async def get_blocked(self, create_authors: bool = False) -> List[Dict] or Tuple['Author']:
+    async def get_blocked(self, create_authors: bool = False) -> Union[List[Dict], Tuple['Author']]:
         """
         Get the authors blocked by the current author.
 
         Parameters:
             create_authors (bool, optional): Whether to create Author objects for blocked authors. Defaults to False.
 
         Returns:
@@ -294,15 +294,15 @@
             None
         """
         await self.request('patch', f'/api/users/login/email',
                            data={"currentPassword": current_password, "newEmail": new_email},
                            **kwargs)
 
     @DrukarniaElement.requires_attributes(['username'], solution='provide username while initializing Author.')
-    async def collect_data(self, return_: bool = False) -> Dict or None:
+    async def collect_data(self, return_: bool = False) -> Union[Dict, None]:
         """
         Collect the author's data and update the object's attributes.
 
         Parameters:
             return_ (bool, optional): Whether to return the collected data. Defaults to False.
 
         Returns:
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/base_object.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/base_object.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/comment.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from aiohttp import ClientSession
 
 from drukarnia_api.objects.base_object import DrukarniaElement
 from drukarnia_api.shortcuts import data2authors, data2comments
 
 from datetime import datetime
-from typing import TYPE_CHECKING, Tuple, Dict
+from typing import TYPE_CHECKING, Tuple, Dict, Union
 
 if TYPE_CHECKING:  # always False, used for type hints
     from drukarnia_api.objects.author import Author
 
 
 class Comment(DrukarniaElement):
     async def reply(self, comment_text: str) -> str:
@@ -44,15 +44,15 @@
 
         await self.request(
             'delete',
             f'/api/articles/{await self.article_id}/comments/{await self.comment_id}')
 
     @DrukarniaElement.requires_attributes(['article_id', 'comment_id'])
     async def get_replies(self,
-                          create_comments: bool = True) -> Tuple['Comment'] or Tuple[Dict]:
+                          create_comments: bool = True) -> Union[Tuple['Comment'], Tuple[Dict]]:
         """
         Deletes a comment from the article.
         """
 
         replies = await self.request(
             'get',
             f'/api/articles/{await self.article_id}/comments/{await self.comment_id}/replies',
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/search.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from drukarnia_api.objects.base_object import DrukarniaElement
 from drukarnia_api.shortcuts import data2authors, data2articles, data2tags
 
-from typing import TYPE_CHECKING, Tuple, Dict
+from typing import TYPE_CHECKING, Tuple, Dict, Union
 
 if TYPE_CHECKING:
     from drukarnia_api.objects.article import Article
     from drukarnia_api.objects.tag import Tag
     from drukarnia_api.objects.author import Author
 
 
@@ -13,15 +13,15 @@
     async def find_author(self,
                           query: str,
                           create_authors: bool = True,
                           with_relations: bool = False,
                           offset: int = 0,
                           results_per_page: int = 20,
                           n_collect: int = None,
-                          *args, **kwargs) -> Tuple['Author'] or Tuple[Dict]:
+                          *args, **kwargs) -> Union[Tuple['Author'], Tuple[Dict]]:
         """
         Search for authors.
 
         Parameters:
         - query (str): The search query for authors.
         - create_authors (bool, optional): Whether to create author objects from the search results. Defaults to True.
         - with_relations (bool, optional): Whether to include author relationships in the search results.
@@ -48,15 +48,15 @@
 
     async def find_articles(self,
                             query: str,
                             create_articles: bool = True,
                             offset: int = 0,
                             results_per_page: int = 20,
                             n_collect: int = None,
-                            *args, **kwargs) -> Tuple['Article'] or Tuple[Dict]:
+                            *args, **kwargs) -> Union[Tuple['Article'], Tuple[Dict]]:
         """
         Search for articles.
 
         Parameters:
         - query (str): The search query for articles.
         - create_articles (bool, optional): Whether to create article objects from the search results. Defaults to True.
         - offset (int, optional): The starting index of the search results. Defaults to 0.
@@ -78,15 +78,15 @@
         return articles
 
     async def find_tags(self,
                         query: str,
                         create_tags: bool = True,
                         offset: int = 0,
                         results_per_page: int = 20,
-                        n_collect: int = None, **kwargs) -> Tuple['Tag'] or Tuple[Dict]:
+                        n_collect: int = None, **kwargs) -> Union[Tuple['Tag'], Tuple[Dict]]:
         """
         Search for tags.
 
         Parameters:
         - query (str): The search query for tags.
         - create_tags (bool, optional): Whether to create tag objects from the search results. Defaults to True.
         - offset (int, optional): The starting index of the search results. Defaults to 0.
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/objects/tag.py` & `drukarnia-api-1.1.2/drukarnia_api/objects/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 from aiohttp import ClientSession
 
 from drukarnia_api.objects.base_object import DrukarniaElement
 from drukarnia_api.shortcuts import data2articles, data2tags, data2authors
 
-from typing import TYPE_CHECKING, Tuple, Dict
+from typing import TYPE_CHECKING, Tuple, Dict, Union
 
 if TYPE_CHECKING:   # always False, used for type hints
     from drukarnia_api.objects.article import Article
     from drukarnia_api.objects.author import Author
 
 
 class Tag(DrukarniaElement):
@@ -27,15 +27,15 @@
 
         # Update the data with slug_name and tag_id
         self._update_data({'slug': slug_name, '_id': tag_id})
 
     @DrukarniaElement.requires_attributes(['slug'])
     async def get_articles(self, create_articles: bool = True,
                            offset: int = 0, results_per_page: int = 20, n_collect: int = None,
-                           **kwargs) -> Tuple['Article'] or Tuple[Dict]:
+                           **kwargs) -> Union[Tuple['Article'], Tuple[Dict]]:
         """
         Get articles associated with this tag.
 
         Args:
             create_articles (bool, optional): Whether to create Article objects from the retrieved data.
                                               Defaults to True.
             offset (int, optional): The offset of the result set. Defaults to 0.
@@ -53,15 +53,15 @@
                                                  **kwargs)
         if create_articles:
             articles = await data2articles(articles, self.session)
 
         return articles
 
     @DrukarniaElement.requires_attributes(['tag_id'])
-    async def related_tags(self, create_tags: bool = True) -> Tuple['Tag'] or Tuple[Dict]:
+    async def related_tags(self, create_tags: bool = True) -> Union[Tuple['Tag'], Tuple[Dict]]:
         """
         Get tags related to this tag.
 
         Args:
             create_tags (bool, optional): Whether to create Tag objects from the retrieved data. Defaults to True.
 
         Returns:
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api/shortcuts/class_generator.py` & `drukarnia-api-1.1.2/drukarnia_api/shortcuts/class_generator.py`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/drukarnia_api.egg-info/PKG-INFO` & `drukarnia-api-1.1.2/drukarnia_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drukarnia-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: wrapper for the Drukarnia API
 Home-page: https://github.com/androu-sys/drukarnia-api
 Author: Andrii Herts
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -31,15 +31,17 @@
 from drukarnia_api import Search
 
 
 async def get_author_article_titles():
     search = Search()
     
     async with search:
-        cupomanka, *_ = await search.find_author('cupomanka') 
+        search_res = await search.find_author('cupomanka')
+        # most probable
+        cupomanka = search_res[0]
 
         # Collect all data about the user
         await cupomanka.collect_data()
 
         # Get user articles
         articles = await cupomanka.articles
```

### Comparing `drukarnia-api-1.1.1/drukarnia_api.egg-info/SOURCES.txt` & `drukarnia-api-1.1.2/drukarnia_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drukarnia-api-1.1.1/setup.py` & `drukarnia-api-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Get requirements
 with open(path.join(HERE, 'requirements.txt')) as f:
     requirements = f.read().splitlines()
 
 # This call to setup() does all the work
 setup(
     name="drukarnia-api",
-    version="1.1.1",
+    version="1.1.2",
     description="wrapper for the Drukarnia API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/androu-sys/drukarnia-api",
     author="Andrii Herts",
     license="MIT",
     classifiers=[
```

