# Comparing `tmp/news_toolkit_api-0.0.5.tar.gz` & `tmp/news_toolkit_api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_toolkit_api-0.0.5.tar", max compression
+gzip compressed data, was "news_toolkit_api-0.0.6.tar", max compression
```

## Comparing `news_toolkit_api-0.0.5.tar` & `news_toolkit_api-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.5/news_toolkit_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.5/news_toolkit_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/__init__.py
--rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/db.py
--rw-r--r--   0        0        0      279 2023-07-31 16:16:50.797792 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/__init__.py
--rw-r--r--   0        0        0      390 2023-07-31 16:13:29.772444 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/article.py
--rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/category.py
--rw-r--r--   0        0        0      433 2023-07-31 16:13:29.773420 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/subscription.py
--rw-r--r--   0        0        0     3316 2023-07-31 16:39:25.423120 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/routers.py
--rw-r--r--   0        0        0      462 2023-07-31 16:21:10.855920 news_toolkit_api-0.0.5/news_toolkit_api/main.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:36.810119 news_toolkit_api-0.0.5/news_toolkit_api/src/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/__init__.py
--rw-r--r--   0        0        0      849 2023-07-31 16:39:46.133229 news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/article.py
--rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.5/news_toolkit_api/src/client.py
--rw-r--r--   0        0        0      249 2023-07-31 16:13:33.504486 news_toolkit_api-0.0.5/news_toolkit_api/src/models/__init__.py
--rw-r--r--   0        0        0      822 2023-07-31 15:31:22.688825 news_toolkit_api-0.0.5/news_toolkit_api/src/models/article.py
--rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.5/news_toolkit_api/src/models/category.py
--rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.5/news_toolkit_api/src/models/subscription.py
--rw-r--r--   0        0        0      313 2023-07-31 16:13:33.506951 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/__init__.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/article_introduction_block.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/banner_ad_block.py
--rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/text_lead_paragraph_block.py
--rw-r--r--   0        0        0        0 2023-07-31 16:25:42.988744 news_toolkit_api-0.0.5/news_toolkit_api/src/repository/__init__.py
--rw-r--r--   0        0        0     2074 2023-07-31 16:48:51.216134 news_toolkit_api-0.0.5/news_toolkit_api/src/repository/article.py
--rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.5/news_toolkit_api/src/utils.py
--rw-r--r--   0        0        0      680 2023-07-31 16:48:51.212788 news_toolkit_api-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.6/news_toolkit_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.6/news_toolkit_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/db.py
+-rw-r--r--   0        0        0      459 2023-07-31 17:17:37.447241 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/__init__.py
+-rw-r--r--   0        0        0      413 2023-07-31 17:17:55.468722 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/article.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/category.py
+-rw-r--r--   0        0        0      711 2023-07-31 17:13:52.137907 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/related_articles.py
+-rw-r--r--   0        0        0      425 2023-07-31 16:56:03.922534 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/response/subscription.py
+-rw-r--r--   0        0        0     6546 2023-07-31 17:17:55.464654 news_toolkit_api-0.0.6/news_toolkit_api/api/v1/routers.py
+-rw-r--r--   0        0        0      455 2023-07-31 16:54:58.274972 news_toolkit_api-0.0.6/news_toolkit_api/app.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/__init__.py
+-rw-r--r--   0        0        0      833 2023-07-31 17:09:23.910533 news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/article.py
+-rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.6/news_toolkit_api/client.py
+-rw-r--r--   0        0        0      225 2023-07-31 16:56:03.918649 news_toolkit_api-0.0.6/news_toolkit_api/db/__init__.py
+-rw-r--r--   0        0        0      947 2023-07-31 17:06:06.542261 news_toolkit_api-0.0.6/news_toolkit_api/db/article.py
+-rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.6/news_toolkit_api/db/category.py
+-rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.6/news_toolkit_api/db/subscription.py
+-rw-r--r--   0        0        0      288 2023-07-31 17:09:23.927090 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/article_introduction_block.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/banner_ad_block.py
+-rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.6/news_toolkit_api/news_blocks/text_lead_paragraph_block.py
+-rw-r--r--   0        0        0       66 2023-07-31 16:54:58.270780 news_toolkit_api-0.0.6/news_toolkit_api/repository/__init__.py
+-rw-r--r--   0        0        0     2064 2023-07-31 17:09:23.908167 news_toolkit_api-0.0.6/news_toolkit_api/repository/article.py
+-rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.6/news_toolkit_api/utils.py
+-rw-r--r--   0        0        0      885 2023-07-31 17:20:15.089708 news_toolkit_api-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.6/PKG-INFO
```

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/article.py` & `news_toolkit_api-0.0.6/news_toolkit_api/background_tasks/article.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from google.cloud import ndb
 
-from news_toolkit_api.src.models.article import Article
-from news_toolkit_api.src.utils import sha3_256_hash
-from news_toolkit_api.src.repository.article import ArticleRepository
+from news_toolkit_api.db.article import Article
+from news_toolkit_api.repository.article import ArticleRepository
+from news_toolkit_api.utils import sha3_256_hash
 
 
 async def background_task_article(
     client: ndb.Client,
     article_repository: ArticleRepository,
     article_id: str,
     fetch_related_article: bool = True,
```

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/client.py` & `news_toolkit_api-0.0.6/news_toolkit_api/client.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/models/article.py` & `news_toolkit_api-0.0.6/news_toolkit_api/db/article.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from google.cloud import ndb
 
 
 class RelatedArticle(ndb.Model):
     article_id = ndb.StringProperty(required=True)
     title = ndb.StringProperty(required=True)
+    category = ndb.StringProperty(required=True)
     image_url = ndb.StringProperty(required=True)
+    auther = ndb.StringProperty()
+    published_at = ndb.DateTimeProperty()
 
 
 class Article(ndb.Model):
     article_id = ndb.StringProperty(required=True)
     title = ndb.StringProperty(required=True)
     content = ndb.TextProperty(repeated=True)
     url = ndb.StringProperty(required=True)
```

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/models/subscription.py` & `news_toolkit_api-0.0.6/news_toolkit_api/db/subscription.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/repository/article.py` & `news_toolkit_api-0.0.6/news_toolkit_api/repository/article.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from abc import ABCMeta, abstractmethod
-from news_toolkit_api.src.models import Article, RelatedArticle
-from news_toolkit_api.src.client import fetch_content
 from datetime import datetime
+
 from bs4 import BeautifulSoup
 
+from news_toolkit_api.client import fetch_content
+from news_toolkit_api.db import Article, RelatedArticle
+
 
 class ArticleRepository(metaclass=ABCMeta):
     def __init__(self) -> None:
         self.html_text: str | None = None
         self.soup: BeautifulSoup | None = None
 
     @abstractmethod
```

### Comparing `news_toolkit_api-0.0.5/news_toolkit_api/src/utils.py` & `news_toolkit_api-0.0.6/news_toolkit_api/utils.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.5/pyproject.toml` & `news_toolkit_api-0.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "news-toolkit-api"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 authors = ["wakita181009 <wakita181009@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "news_toolkit_api" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
@@ -18,14 +18,26 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.7.0"
 flake8 = "^6.1.0"
 flake8-pyproject = "^1.2.3"
 mypy = "^1.4.1"
 isort = "^5.12.0"
+types-beautifulsoup4 = "^4.12.0.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
+
+
+[tool.flake8]
+max-line-length = 120
+count = true
+ignore = ["E203", "F401"]
+
+[tool.mypy]
+[[tool.mypy.overrides]]
+module = "google.cloud.*"
+ignore_missing_imports = true
```

### Comparing `news_toolkit_api-0.0.5/PKG-INFO` & `news_toolkit_api-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-toolkit-api
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Author: wakita181009
 Author-email: wakita181009@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

