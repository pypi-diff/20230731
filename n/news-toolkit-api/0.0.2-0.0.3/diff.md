# Comparing `tmp/news_toolkit_api-0.0.2.tar.gz` & `tmp/news_toolkit_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "news_toolkit_api-0.0.2.tar", max compression
+gzip compressed data, was "news_toolkit_api-0.0.3.tar", max compression
```

## Comparing `news_toolkit_api-0.0.2.tar` & `news_toolkit_api-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,26 @@
--rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.2/news_toolkit_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.2/news_toolkit_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/__init__.py
--rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/db.py
--rw-r--r--   0        0        0      228 2023-07-31 16:02:53.769068 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/response/__init__.py
--rw-r--r--   0        0        0      390 2023-07-31 16:13:29.772444 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/response/article.py
--rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/response/category.py
--rw-r--r--   0        0        0      433 2023-07-31 16:13:29.773420 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/response/subscription.py
--rw-r--r--   0        0        0     2966 2023-07-31 16:13:33.494419 news_toolkit_api-0.0.2/news_toolkit_api/api/v1/routers.py
--rw-r--r--   0        0        0      305 2023-07-31 16:13:33.489689 news_toolkit_api-0.0.2/news_toolkit_api/main.py
--rw-r--r--   0        0        0        0 2023-07-31 14:37:36.810119 news_toolkit_api-0.0.2/news_toolkit_api/src/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.2/news_toolkit_api/src/background_tasks/__init__.py
--rw-r--r--   0        0        0      708 2023-07-31 16:13:29.771313 news_toolkit_api-0.0.2/news_toolkit_api/src/background_tasks/article.py
--rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.2/news_toolkit_api/src/client.py
--rw-r--r--   0        0        0        0 2023-07-31 15:38:01.859848 news_toolkit_api-0.0.2/news_toolkit_api/src/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 15:38:49.873783 news_toolkit_api-0.0.2/news_toolkit_api/src/config/global_settings.py
--rw-r--r--   0        0        0      249 2023-07-31 16:13:33.504486 news_toolkit_api-0.0.2/news_toolkit_api/src/models/__init__.py
--rw-r--r--   0        0        0      822 2023-07-31 15:31:22.688825 news_toolkit_api-0.0.2/news_toolkit_api/src/models/article.py
--rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.2/news_toolkit_api/src/models/category.py
--rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.2/news_toolkit_api/src/models/subscription.py
--rw-r--r--   0        0        0      313 2023-07-31 16:13:33.506951 news_toolkit_api-0.0.2/news_toolkit_api/src/news_blocks/__init__.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.2/news_toolkit_api/src/news_blocks/article_introduction_block.py
--rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.2/news_toolkit_api/src/news_blocks/banner_ad_block.py
--rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.2/news_toolkit_api/src/news_blocks/text_lead_paragraph_block.py
--rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.2/news_toolkit_api/src/utils.py
--rw-r--r--   0        0        0      653 2023-07-31 16:14:55.272786 news_toolkit_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-31 14:36:43.243763 news_toolkit_api-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-31 14:33:41.949127 news_toolkit_api-0.0.3/news_toolkit_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:42.991442 news_toolkit_api-0.0.3/news_toolkit_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:51.893138 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-31 14:48:20.474554 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/db.py
+-rw-r--r--   0        0        0      279 2023-07-31 16:16:50.797792 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/response/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-31 16:13:29.772444 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/response/article.py
+-rw-r--r--   0        0        0      112 2023-07-31 15:23:52.955109 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/response/category.py
+-rw-r--r--   0        0        0      433 2023-07-31 16:13:29.773420 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/response/subscription.py
+-rw-r--r--   0        0        0     2966 2023-07-31 16:13:33.494419 news_toolkit_api-0.0.3/news_toolkit_api/api/v1/routers.py
+-rw-r--r--   0        0        0      305 2023-07-31 16:13:33.489689 news_toolkit_api-0.0.3/news_toolkit_api/main.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:37:36.810119 news_toolkit_api-0.0.3/news_toolkit_api/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 15:25:16.529314 news_toolkit_api-0.0.3/news_toolkit_api/src/background_tasks/__init__.py
+-rw-r--r--   0        0        0      708 2023-07-31 16:13:29.771313 news_toolkit_api-0.0.3/news_toolkit_api/src/background_tasks/article.py
+-rw-r--r--   0        0        0      683 2023-07-31 15:28:51.877363 news_toolkit_api-0.0.3/news_toolkit_api/src/client.py
+-rw-r--r--   0        0        0      249 2023-07-31 16:13:33.504486 news_toolkit_api-0.0.3/news_toolkit_api/src/models/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-31 15:31:22.688825 news_toolkit_api-0.0.3/news_toolkit_api/src/models/article.py
+-rw-r--r--   0        0        0      103 2023-07-31 15:23:52.957324 news_toolkit_api-0.0.3/news_toolkit_api/src/models/category.py
+-rw-r--r--   0        0        0      557 2023-07-31 16:01:54.164641 news_toolkit_api-0.0.3/news_toolkit_api/src/models/subscription.py
+-rw-r--r--   0        0        0      313 2023-07-31 16:13:33.506951 news_toolkit_api-0.0.3/news_toolkit_api/src/news_blocks/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.695109 news_toolkit_api-0.0.3/news_toolkit_api/src/news_blocks/article_introduction_block.py
+-rw-r--r--   0        0        0      380 2023-07-31 15:15:00.691257 news_toolkit_api-0.0.3/news_toolkit_api/src/news_blocks/banner_ad_block.py
+-rw-r--r--   0        0        0      224 2023-07-31 15:15:00.693386 news_toolkit_api-0.0.3/news_toolkit_api/src/news_blocks/text_lead_paragraph_block.py
+-rw-r--r--   0        0        0      890 2023-07-31 16:01:54.161537 news_toolkit_api-0.0.3/news_toolkit_api/src/utils.py
+-rw-r--r--   0        0        0      653 2023-07-31 16:17:05.315283 news_toolkit_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 news_toolkit_api-0.0.3/PKG-INFO
```

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/api/v1/routers.py` & `news_toolkit_api-0.0.3/news_toolkit_api/api/v1/routers.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/src/background_tasks/article.py` & `news_toolkit_api-0.0.3/news_toolkit_api/src/background_tasks/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/src/client.py` & `news_toolkit_api-0.0.3/news_toolkit_api/src/client.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/src/models/article.py` & `news_toolkit_api-0.0.3/news_toolkit_api/src/models/article.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/src/models/subscription.py` & `news_toolkit_api-0.0.3/news_toolkit_api/src/models/subscription.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/news_toolkit_api/src/utils.py` & `news_toolkit_api-0.0.3/news_toolkit_api/src/utils.py`

 * *Files identical despite different names*

### Comparing `news_toolkit_api-0.0.2/pyproject.toml` & `news_toolkit_api-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "news-toolkit-api"
-version = "0.0.2"
+version = "0.0.3"
 description = ""
 authors = ["wakita181009 <wakita181009@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "news_toolkit_api" }]
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

### Comparing `news_toolkit_api-0.0.2/PKG-INFO` & `news_toolkit_api-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: news-toolkit-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: 
 Author: wakita181009
 Author-email: wakita181009@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
```

