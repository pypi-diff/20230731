# Comparing `tmp/news_toolkit_api-0.0.4.tar.gz` & `tmp/news_toolkit_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_toolkit_api-0.0.4.tar", max compression
+gzip compressed data, was "news_toolkit_api-0.0.5.tar", max compression
```

## Comparing `news_toolkit_api-0.0.4.tar` & `news_toolkit_api-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.4/news_toolkit_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.4/news_toolkit_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/__init__.py
--rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/db.py
--rw-r--r--   0        0        0      279 2023-07-31 16:16:50.797792 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/response/__init__.py
--rw-r--r--   0        0        0      390 2023-07-31 16:13:29.772444 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/response/article.py
--rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/response/category.py
--rw-r--r--   0        0        0      433 2023-07-31 16:13:29.773420 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/response/subscription.py
--rw-r--r--   0        0        0     3316 2023-07-31 16:39:25.423120 news_toolkit_api-0.0.4/news_toolkit_api/api/v1/routers.py
--rw-r--r--   0        0        0      462 2023-07-31 16:21:10.855920 news_toolkit_api-0.0.4/news_toolkit_api/main.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:36.810119 news_toolkit_api-0.0.4/news_toolkit_api/src/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.4/news_toolkit_api/src/background_tasks/__init__.py
--rw-r--r--   0        0        0      849 2023-07-31 16:39:46.133229 news_toolkit_api-0.0.4/news_toolkit_api/src/background_tasks/article.py
--rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.4/news_toolkit_api/src/client.py
--rw-r--r--   0        0        0      249 2023-07-31 16:13:33.504486 news_toolkit_api-0.0.4/news_toolkit_api/src/models/__init__.py
--rw-r--r--   0        0        0      822 2023-07-31 15:31:22.688825 news_toolkit_api-0.0.4/news_toolkit_api/src/models/article.py
--rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.4/news_toolkit_api/src/models/category.py
--rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.4/news_toolkit_api/src/models/subscription.py
--rw-r--r--   0        0        0      313 2023-07-31 16:13:33.506951 news_toolkit_api-0.0.4/news_toolkit_api/src/news_blocks/__init__.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.4/news_toolkit_api/src/news_blocks/article_introduction_block.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.4/news_toolkit_api/src/news_blocks/banner_ad_block.py
--rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.4/news_toolkit_api/src/news_blocks/text_lead_paragraph_block.py
--rw-r--r--   0        0        0        0 2023-07-31 16:25:42.988744 news_toolkit_api-0.0.4/news_toolkit_api/src/repository/__init__.py
--rw-r--r--   0        0        0     1908 2023-07-31 16:39:24.489478 news_toolkit_api-0.0.4/news_toolkit_api/src/repository/article.py
--rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.4/news_toolkit_api/src/utils.py
--rw-r--r--   0        0        0      680 2023-07-31 16:40:17.223413 news_toolkit_api-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.5/news_toolkit_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.5/news_toolkit_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/db.py
+-rw-r--r--   0        0        0      279 2023-07-31 16:16:50.797792 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-31 16:13:29.772444 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/article.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/category.py
+-rw-r--r--   0        0        0      433 2023-07-31 16:13:29.773420 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/response/subscription.py
+-rw-r--r--   0        0        0     3316 2023-07-31 16:39:25.423120 news_toolkit_api-0.0.5/news_toolkit_api/api/v1/routers.py
+-rw-r--r--   0        0        0      462 2023-07-31 16:21:10.855920 news_toolkit_api-0.0.5/news_toolkit_api/main.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:36.810119 news_toolkit_api-0.0.5/news_toolkit_api/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/__init__.py
+-rw-r--r--   0        0        0      849 2023-07-31 16:39:46.133229 news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/article.py
+-rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.5/news_toolkit_api/src/client.py
+-rw-r--r--   0        0        0      249 2023-07-31 16:13:33.504486 news_toolkit_api-0.0.5/news_toolkit_api/src/models/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-31 15:31:22.688825 news_toolkit_api-0.0.5/news_toolkit_api/src/models/article.py
+-rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.5/news_toolkit_api/src/models/category.py
+-rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.5/news_toolkit_api/src/models/subscription.py
+-rw-r--r--   0        0        0      313 2023-07-31 16:13:33.506951 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/article_introduction_block.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/banner_ad_block.py
+-rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.5/news_toolkit_api/src/news_blocks/text_lead_paragraph_block.py
+-rw-r--r--   0        0        0        0 2023-07-31 16:25:42.988744 news_toolkit_api-0.0.5/news_toolkit_api/src/repository/__init__.py
+-rw-r--r--   0        0        0     2074 2023-07-31 16:48:51.216134 news_toolkit_api-0.0.5/news_toolkit_api/src/repository/article.py
+-rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.5/news_toolkit_api/src/utils.py
+-rw-r--r--   0        0        0      680 2023-07-31 16:48:51.212788 news_toolkit_api-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      581 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.5/PKG-INFO
```

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/api/v1/routers.py` & `news_toolkit_api-0.0.5/news_toolkit_api/api/v1/routers.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/background_tasks/article.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/background_tasks/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/client.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/client.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/models/article.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/models/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/models/subscription.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/models/subscription.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/repository/article.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/repository/article.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,18 @@
         pass
 
     @abstractmethod
     def parse_content(self) -> list[str] | None:
         pass
 
     @abstractmethod
+    def parse_category(self) -> str | None:
+        pass
+
+    @abstractmethod
     def parse_image_url(self) -> str | None:
         pass
 
     @abstractmethod
     def parse_auther(self) -> str | None:
         pass
 
@@ -46,22 +50,24 @@
 
         self.soup = BeautifulSoup(self.html_text, features="html5lib")
         if not self.soup:
             return None
 
         title = self.parse_title()
         content = self.parse_content()
-        if not title or not content:
+        category = self.parse_category()
+        if not title or not content or not category:
             return None
 
         return Article(
             article_id=article_id,
             title=title,
             content=content,
             url=article_url,
+            category=category,
             image_url=self.parse_image_url(),
             auther=self.parse_auther(),
             published_at=self.parse_published_at(),
             related_articles=self.parse_related_articles(),
             is_premium=False,
             is_preview=False,
             created_at=datetime.utcnow(),
```

### Comparing `news_toolkit_api-0.0.4/news_toolkit_api/src/utils.py` & `news_toolkit_api-0.0.5/news_toolkit_api/src/utils.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.4/pyproject.toml` & `news_toolkit_api-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "news-toolkit-api"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["wakita181009 <wakita181009@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "news_toolkit_api" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `news_toolkit_api-0.0.4/PKG-INFO` & `news_toolkit_api-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-toolkit-api
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: wakita181009
 Author-email: wakita181009@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

