# Comparing `tmp/news_toolkit_api-0.0.6.tar.gz` & `tmp/news_toolkit_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_toolkit_api-0.0.6.tar", max compression
+gzip compressed data, was "news_toolkit_api-0.0.7.tar", max compression
```

## Comparing `news_toolkit_api-0.0.6.tar` & `news_toolkit_api-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,34 @@
--rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.6/news_toolkit_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.6/news_toolkit_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/__init__.py
--rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/db.py
--rw-r--r--   0        0        0      459 2023-07-31 17:17:37.447241 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/__init__.py
--rw-r--r--   0        0        0      413 2023-07-31 17:17:55.468722 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/article.py
--rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/category.py
--rw-r--r--   0        0        0      711 2023-07-31 17:13:52.137907 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/related_articles.py
--rw-r--r--   0        0        0      425 2023-07-31 16:56:03.922534 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/subscription.py
--rw-r--r--   0        0        0     6546 2023-07-31 17:17:55.464654 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/routers.py
--rw-r--r--   0        0        0      455 2023-07-31 16:54:58.274972 news_toolkit_api-0.0.6/news_toolkit_api/app.py
--rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/__init__.py
--rw-r--r--   0        0        0      833 2023-07-31 17:09:23.910533 news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/article.py
--rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.6/news_toolkit_api/client.py
--rw-r--r--   0        0        0      225 2023-07-31 16:56:03.918649 news_toolkit_api-0.0.6/news_toolkit_api/db/__init__.py
--rw-r--r--   0        0        0      947 2023-07-31 17:06:06.542261 news_toolkit_api-0.0.6/news_toolkit_api/db/article.py
--rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.6/news_toolkit_api/db/category.py
--rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.6/news_toolkit_api/db/subscription.py
--rw-r--r--   0        0        0      288 2023-07-31 17:09:23.927090 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/__init__.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/article_introduction_block.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/banner_ad_block.py
--rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/text_lead_paragraph_block.py
--rw-r--r--   0        0        0       66 2023-07-31 16:54:58.270780 news_toolkit_api-0.0.6/news_toolkit_api/repository/__init__.py
--rw-r--r--   0        0        0     2064 2023-07-31 17:09:23.908167 news_toolkit_api-0.0.6/news_toolkit_api/repository/article.py
--rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.6/news_toolkit_api/utils.py
--rw-r--r--   0        0        0      885 2023-07-31 17:20:15.089708 news_toolkit_api-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.7/news_toolkit_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.7/news_toolkit_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/db.py
+-rw-r--r--   0        0        0      503 2023-07-31 18:04:25.893255 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-31 17:17:55.468722 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/article.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/category.py
+-rw-r--r--   0        0        0      562 2023-07-31 18:12:42.744676 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/feed.py
+-rw-r--r--   0        0        0      524 2023-07-31 17:56:44.386755 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/related_articles.py
+-rw-r--r--   0        0        0      425 2023-07-31 16:56:03.922534 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/response/subscription.py
+-rw-r--r--   0        0        0     8096 2023-07-31 18:23:16.572703 news_toolkit_api-0.0.7/news_toolkit_api/api/v1/routers.py
+-rw-r--r--   0        0        0      479 2023-07-31 17:34:29.932031 news_toolkit_api-0.0.7/news_toolkit_api/app.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.7/news_toolkit_api/background_tasks/__init__.py
+-rw-r--r--   0        0        0      833 2023-07-31 17:09:23.910533 news_toolkit_api-0.0.7/news_toolkit_api/background_tasks/article.py
+-rw-r--r--   0        0        0     1069 2023-07-31 18:23:16.529179 news_toolkit_api-0.0.7/news_toolkit_api/background_tasks/feed.py
+-rw-r--r--   0        0        0      722 2023-07-31 17:30:01.061321 news_toolkit_api-0.0.7/news_toolkit_api/client.py
+-rw-r--r--   0        0        0      267 2023-07-31 17:56:44.375693 news_toolkit_api-0.0.7/news_toolkit_api/db/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-31 17:06:06.542261 news_toolkit_api-0.0.7/news_toolkit_api/db/article.py
+-rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.7/news_toolkit_api/db/category.py
+-rw-r--r--   0        0        0      429 2023-07-31 17:52:45.739386 news_toolkit_api-0.0.7/news_toolkit_api/db/feed.py
+-rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.7/news_toolkit_api/db/subscription.py
+-rw-r--r--   0        0        0      516 2023-07-31 17:56:44.390573 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/article_introduction_block.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/banner_ad_block.py
+-rw-r--r--   0        0        0      115 2023-07-31 17:52:45.740226 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/block_type.py
+-rw-r--r--   0        0        0      217 2023-07-31 17:52:45.741799 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/navigate_to_article.py
+-rw-r--r--   0        0        0      216 2023-07-31 17:56:41.480758 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/section_header_block.py
+-rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.7/news_toolkit_api/news_blocks/text_lead_paragraph_block.py
+-rw-r--r--   0        0        0       66 2023-07-31 16:54:58.270780 news_toolkit_api-0.0.7/news_toolkit_api/repository/__init__.py
+-rw-r--r--   0        0        0     2812 2023-07-31 18:20:11.188625 news_toolkit_api-0.0.7/news_toolkit_api/repository/article.py
+-rw-r--r--   0        0        0      949 2023-07-31 17:30:43.852193 news_toolkit_api-0.0.7/news_toolkit_api/utils.py
+-rw-r--r--   0        0        0      845 2023-07-31 18:24:40.543916 news_toolkit_api-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.7/PKG-INFO
```

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/api/v1/routers.py` & `news_toolkit_api-0.0.7/news_toolkit_api/api/v1/routers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 from fastapi import APIRouter, BackgroundTasks, Depends
 from fastapi_injector import Injected
 from google.cloud import ndb
 
 from news_toolkit_api.api.v1.db import get_client
 from news_toolkit_api.api.v1.response import (
     ArticleResponse,
-    BlockType,
     CategoriesResponse,
     ContentType,
-    NavigateToArticleAction,
+    FeedResponse,
+    FeedsResponse,
+    FeedType,
     RelatedArticleResponse,
     RelatedArticlesResponse,
     SubscriptionCost,
     SubscriptionResponse,
     SubscriptionsResponse,
 )
 from news_toolkit_api.background_tasks.article import background_task_article
-from news_toolkit_api.db import Article, Category, Subscription
+from news_toolkit_api.background_tasks.feed import background_task_feed
+from news_toolkit_api.db import Article, Category, Feed, Subscription
 from news_toolkit_api.news_blocks import (
     ArticleIntroductionBlock,
     BannerAdContent,
     BannerAdSize,
+    BlockType,
+    NavigateToArticleAction,
+    SectionHeaderBlock,
     TextLeadParagraphBlock,
 )
 from news_toolkit_api.repository import ArticleRepository
 from news_toolkit_api.utils import needs_update, sha3_256_hash
 
 router = APIRouter(prefix="/api/v1")
 
@@ -117,14 +122,55 @@
         )
     return RelatedArticlesResponse(
         related_articles=related_articles,
         total_count=len(article.related_articles),
     )
 
 
+@router.get("/feed")
+async def get_feed(
+    category: str,
+    background_tasks: BackgroundTasks,
+    limit: int = 20,
+    offset: int = 0,
+    client: ndb.Client = Depends(get_client),
+    article_repository: ArticleRepository = Injected(ArticleRepository),
+):
+    with client.context():
+        if not ndb.Key(Category, sha3_256_hash(category)).get():
+            return FeedsResponse(feed=[], total_count=0)
+
+    feeds: FeedType = []
+    if offset == 0:
+        feeds.append(SectionHeaderBlock(title="新着記事"))
+    with client.context():
+        query = Feed.query().order("published_at")
+        # Aggregate total count
+        total_count = query.count()
+        for feed in query.fetch(limit=limit, offset=offset):
+            feeds.append(
+                FeedResponse(
+                    id=feed.key.id(),
+                    title=feed.title,
+                    category=feed.category,
+                    image_url=feed.image_url,
+                    author=feed.auther,
+                    published_at=feed.published_at,
+                    is_premium=False,
+                    type=BlockType.post_large,
+                    action=NavigateToArticleAction(feed.article_id),
+                )
+            )
+
+    background_tasks.add_task(
+        background_task_feed, client, article_repository, category
+    )
+    return FeedsResponse(feed=feeds, total_count=total_count)
+
+
 @router.get("/subscriptions")
 async def get_subscriptions(client: ndb.Client = Depends(get_client)):
     with client.context():
         subscriptions = []
         for subscription in Subscription.query():
             subscriptions.append(
                 SubscriptionResponse(
```

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/article.py` & `news_toolkit_api-0.0.7/news_toolkit_api/background_tasks/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/client.py` & `news_toolkit_api-0.0.7/news_toolkit_api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
 import logging
 import os
 
 import aiohttp
 from aiohttp import ClientTimeout
 
-REQUEST_TIMEOUT = int(os.getenv("REQUEST_TIMEOUT", 60))
+NEWS_TOOLKIT_REQUEST_TIMEOUT = int(os.getenv("NEWS_TOOLKIT_REQUEST_TIMEOUT", 60))
 
 
 async def fetch_content(url: str) -> str | None:
     try:
         async with aiohttp.ClientSession(
-            timeout=ClientTimeout(REQUEST_TIMEOUT)
+            timeout=ClientTimeout(NEWS_TOOLKIT_REQUEST_TIMEOUT)
         ) as session:
             async with session.get(url) as res:
                 res.raise_for_status()
                 return await res.text()
     except aiohttp.ClientError as e:
         logging.error(f"Error fetching the url {url}: {e}")
         return None
```

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/db/article.py` & `news_toolkit_api-0.0.7/news_toolkit_api/db/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/db/subscription.py` & `news_toolkit_api-0.0.7/news_toolkit_api/db/subscription.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/repository/article.py` & `news_toolkit_api-0.0.7/news_toolkit_api/repository/article.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,76 +1,96 @@
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 
 from bs4 import BeautifulSoup
 
 from news_toolkit_api.client import fetch_content
-from news_toolkit_api.db import Article, RelatedArticle
+from news_toolkit_api.db import Article, Feed, RelatedArticle
 
 
 class ArticleRepository(metaclass=ABCMeta):
     def __init__(self) -> None:
         self.html_text: str | None = None
         self.soup: BeautifulSoup | None = None
 
     @abstractmethod
-    def build_url(self, article_id: str) -> str:
+    def build_article_url(self, article_id: str) -> str:
         pass
 
     @abstractmethod
-    def parse_title(self) -> str | None:
+    def build_feed_url(self, category: str) -> str:
         pass
 
     @abstractmethod
-    def parse_content(self) -> list[str] | None:
+    def parse_title(self, soup: BeautifulSoup) -> str | None:
         pass
 
     @abstractmethod
-    def parse_category(self) -> str | None:
+    def parse_content(self, soup: BeautifulSoup) -> list[str] | None:
         pass
 
     @abstractmethod
-    def parse_image_url(self) -> str | None:
+    def parse_category(self, soup: BeautifulSoup) -> str | None:
         pass
 
     @abstractmethod
-    def parse_auther(self) -> str | None:
+    def parse_image_url(self, soup: BeautifulSoup) -> str | None:
         pass
 
     @abstractmethod
-    def parse_published_at(self) -> datetime | None:
+    def parse_auther(self, soup: BeautifulSoup) -> str | None:
         pass
 
     @abstractmethod
-    def parse_related_articles(self) -> list[RelatedArticle]:
+    def parse_published_at(self, soup: BeautifulSoup) -> datetime | None:
+        pass
+
+    @abstractmethod
+    def parse_related_articles(self, soup: BeautifulSoup) -> list[RelatedArticle]:
+        pass
+
+    @abstractmethod
+    def parse_feed(self, soup: BeautifulSoup, category: str) -> list[Feed] | None:
         pass
 
     async def fetch_content(self, article_id: str) -> Article | None:
-        article_url = self.build_url(article_id)
-        self.html_text = await fetch_content(article_url)
-        if not self.html_text:
+        article_url = self.build_article_url(article_id)
+        html_text = await fetch_content(article_url)
+        if not html_text:
             return None
 
-        self.soup = BeautifulSoup(self.html_text, features="html5lib")
-        if not self.soup:
+        soup = BeautifulSoup(html_text, features="html5lib")
+        if not soup:
             return None
 
-        title = self.parse_title()
-        content = self.parse_content()
-        category = self.parse_category()
+        title = self.parse_title(soup)
+        content = self.parse_content(soup)
+        category = self.parse_category(soup)
         if not title or not content or not category:
             return None
 
         return Article(
             article_id=article_id,
             title=title,
             content=content,
             url=article_url,
             category=category,
-            image_url=self.parse_image_url(),
-            auther=self.parse_auther(),
-            published_at=self.parse_published_at(),
-            related_articles=self.parse_related_articles(),
+            image_url=self.parse_image_url(soup),
+            auther=self.parse_auther(soup),
+            published_at=self.parse_published_at(soup),
+            related_articles=self.parse_related_articles(soup),
             is_premium=False,
             is_preview=False,
             created_at=datetime.utcnow(),
         )
+
+    async def fetch_feed(self, category: str) -> list[Feed] | None:
+        feed_url = self.build_feed_url(category)
+        html_text = await fetch_content(feed_url)
+        if not html_text:
+            return None
+
+        soup = BeautifulSoup(html_text, features="html5lib")
+        if not soup:
+            return None
+
+        return self.parse_feed(soup, category)
```

### Comparing `news_toolkit_api-0.0.6/news_toolkit_api/utils.py` & `news_toolkit_api-0.0.7/news_toolkit_api/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import hashlib
 import os
 from datetime import datetime, timedelta
 
-UPDATE_INTERVAL_MINUTES = int(os.getenv("UPDATE_INTERVAL_MINUTES", 60))
+NEWS_TOOLKIT_UPDATE_INTERVAL_MINUTES = int(
+    os.getenv("NEWS_TOOLKIT_UPDATE_INTERVAL_MINUTES", 60)
+)
 
 
 def sha3_256_hash(data: str) -> str:
     """
     Computes the SHA-3 256-bit hash of the given string.
 
     :param data: The string to be hashed.
@@ -21,9 +23,11 @@
     """
     Check if the provided datetime is older than the allowed interval.
 
     :param last_updated_time: The datetime to check against.
     :return: True if an update is required, False otherwise.
     """
     current_time = datetime.utcnow()
-    deadline_time = current_time - timedelta(minutes=UPDATE_INTERVAL_MINUTES)
+    deadline_time = current_time - timedelta(
+        minutes=NEWS_TOOLKIT_UPDATE_INTERVAL_MINUTES
+    )
     return last_updated_time < deadline_time
```

### Comparing `news_toolkit_api-0.0.6/pyproject.toml` & `news_toolkit_api-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "news-toolkit-api"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["wakita181009 <wakita181009@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "news_toolkit_api" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 fastapi = "^0.100.1"
 fastapi-injector = "^0.5.1"
-google-cloud-ndb = "^2.2.0"
-uvicorn = { extras = ["standard"], version = "^0.23.2" }
 aiohttp = "^3.8.5"
+google-cloud-ndb = "^2.2.0"
 beautifulsoup4 = "^4.12.2"
-
+html5lib = "^1.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 flake8 = "^6.1.0"
 flake8-pyproject = "^1.2.3"
 mypy = "^1.4.1"
 isort = "^5.12.0"
```

### Comparing `news_toolkit_api-0.0.6/PKG-INFO` & `news_toolkit_api-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: news-toolkit-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: wakita181009
 Author-email: wakita181009@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: fastapi (>=0.100.1,<0.101.0)
 Requires-Dist: fastapi-injector (>=0.5.1,<0.6.0)
 Requires-Dist: google-cloud-ndb (>=2.2.0,<3.0.0)
-Requires-Dist: uvicorn[standard] (>=0.23.2,<0.24.0)
+Requires-Dist: html5lib (>=1.1,<2.0)
 Description-Content-Type: text/markdown
```

