# Comparing `tmp/webcomix-3.6.6.tar.gz` & `tmp/webcomix-3.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcomix-3.6.6.tar", max compression
+gzip compressed data, was "webcomix-3.6.7.tar", max compression
```

## Comparing `webcomix-3.6.6.tar` & `webcomix-3.6.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1069 2023-03-04 20:44:36.672795 webcomix-3.6.6/LICENSE
--rw-r--r--   0        0        0     4434 2023-03-04 20:44:36.672795 webcomix-3.6.6/README.md
--rw-r--r--   0        0        0     1292 2023-03-04 20:44:36.672795 webcomix-3.6.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/__init__.py
--rw-r--r--   0        0        0     6860 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/cli.py
--rw-r--r--   0        0        0     7135 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/comic.py
--rw-r--r--   0        0        0     1191 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/docker.py
--rw-r--r--   0        0        0      216 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.672795 webcomix-3.6.6/webcomix/scrapy/__init__.py
--rw-r--r--   0        0        0     1493 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/crawler_worker.py
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/__init__.py
--rw-r--r--   0        0        0      154 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/comic_page.py
--rw-r--r--   0        0        0     2131 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/comic_pipeline.py
--rw-r--r--   0        0        0     2192 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/comic_spider.py
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/tests/__init__.py
--rw-r--r--   0        0        0     3785 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/tests/test_comic_pipeline.py
--rw-r--r--   0        0        0     3269 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/download/tests/test_comic_spider.py
--rw-r--r--   0        0        0      387 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/request_factory.py
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/tests/__init__.py
--rw-r--r--   0        0        0      701 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/tests/test_crawler_worker.py
--rw-r--r--   0        0        0      566 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/tests/test_request_factory.py
--rw-r--r--   0        0        0      113 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/util.py
--rw-r--r--   0        0        0        0 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/verification/__init__.py
--rw-r--r--   0        0        0     2477 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/verification/verification_spider.py
--rw-r--r--   0        0        0      157 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/scrapy/verification/web_page.py
--rw-r--r--   0        0        0     2575 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/search.py
--rw-r--r--   0        0        0     6596 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/supported_comics.py
--rw-r--r--   0        0        0        2 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/__init__.py
--rw-r--r--   0        0        0     1027 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/fixture.py
--rw-r--r--   0        0        0      169 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage/1.html
--rw-r--r--   0        0        0    25483 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage/1.jpeg
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage/2.jpeg
--rw-r--r--   0        0        0      197 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage_searchable/1.html
--rw-r--r--   0        0        0    25483 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg
--rw-r--r--   0        0        0      170 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/1.html
--rw-r--r--   0        0        0    25483 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/1.jpeg
--rw-r--r--   0        0        0      170 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/2.html
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/2.jpeg
--rw-r--r--   0        0        0      115 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/3.html
--rw-r--r--   0        0        0      189 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/1.html
--rw-r--r--   0        0        0    25483 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg
--rw-r--r--   0        0        0      190 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/2.html
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg
--rw-r--r--   0        0        0      115 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/3.html
--rw-r--r--   0        0        0      197 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/1.html
--rw-r--r--   0        0        0    25483 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg
--rw-r--r--   0        0        0      197 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/2.html
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg
--rw-r--r--   0        0        0      205 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/3.html
--rw-r--r--   0        0        0    31690 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg
--rw-r--r--   0        0        0      115 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/4.html
--rw-r--r--   0        0        0     9934 2023-03-04 20:44:36.676795 webcomix-3.6.6/webcomix/tests/test_cli.py
--rw-r--r--   0        0        0     8547 2023-03-04 20:44:36.680795 webcomix-3.6.6/webcomix/tests/test_comic.py
--rw-r--r--   0        0        0      562 2023-03-04 20:44:36.680795 webcomix-3.6.6/webcomix/tests/test_comic_availability.py
--rw-r--r--   0        0        0      934 2023-03-04 20:44:36.680795 webcomix-3.6.6/webcomix/tests/test_docker.py
--rw-r--r--   0        0        0     4068 2023-03-04 20:44:36.680795 webcomix-3.6.6/webcomix/tests/test_search.py
--rw-r--r--   0        0        0      440 2023-03-04 20:44:36.680795 webcomix-3.6.6/webcomix/util.py
--rw-r--r--   0        0        0     5867 1970-01-01 00:00:00.000000 webcomix-3.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 17:02:22.032640 webcomix-3.6.7/LICENSE
+-rw-r--r--   0        0        0     4434 2023-07-31 17:02:22.032640 webcomix-3.6.7/README.md
+-rw-r--r--   0        0        0     1323 2023-07-31 17:02:22.032640 webcomix-3.6.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.032640 webcomix-3.6.7/webcomix/__init__.py
+-rw-r--r--   0        0        0     6860 2023-07-31 17:02:22.032640 webcomix-3.6.7/webcomix/cli.py
+-rw-r--r--   0        0        0     7135 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/comic.py
+-rw-r--r--   0        0        0     1191 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/docker.py
+-rw-r--r--   0        0        0      216 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/__init__.py
+-rw-r--r--   0        0        0     1493 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/crawler_worker.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/comic_page.py
+-rw-r--r--   0        0        0     2131 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/comic_pipeline.py
+-rw-r--r--   0        0        0     2192 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/comic_spider.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/tests/__init__.py
+-rw-r--r--   0        0        0     3785 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/tests/test_comic_pipeline.py
+-rw-r--r--   0        0        0     3269 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/download/tests/test_comic_spider.py
+-rw-r--r--   0        0        0      387 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/request_factory.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/tests/__init__.py
+-rw-r--r--   0        0        0      701 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/tests/test_crawler_worker.py
+-rw-r--r--   0        0        0      566 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/tests/test_request_factory.py
+-rw-r--r--   0        0        0      113 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/util.py
+-rw-r--r--   0        0        0        0 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/verification/__init__.py
+-rw-r--r--   0        0        0     2477 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/verification/verification_spider.py
+-rw-r--r--   0        0        0      157 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/scrapy/verification/web_page.py
+-rw-r--r--   0        0        0     2575 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/search.py
+-rw-r--r--   0        0        0     6559 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/supported_comics.py
+-rw-r--r--   0        0        0        2 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/__init__.py
+-rw-r--r--   0        0        0     1027 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/fixture.py
+-rw-r--r--   0        0        0      169 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage/1.html
+-rw-r--r--   0        0        0    25483 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage/1.jpeg
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage/2.jpeg
+-rw-r--r--   0        0        0      197 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage_searchable/1.html
+-rw-r--r--   0        0        0    25483 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg
+-rw-r--r--   0        0        0      170 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/1.html
+-rw-r--r--   0        0        0    25483 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/1.jpeg
+-rw-r--r--   0        0        0      170 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/2.html
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/2.jpeg
+-rw-r--r--   0        0        0      115 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/3.html
+-rw-r--r--   0        0        0      189 2023-07-31 17:02:22.036641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/1.html
+-rw-r--r--   0        0        0    25483 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg
+-rw-r--r--   0        0        0      190 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/2.html
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg
+-rw-r--r--   0        0        0      115 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/3.html
+-rw-r--r--   0        0        0      197 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/1.html
+-rw-r--r--   0        0        0    25483 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg
+-rw-r--r--   0        0        0      197 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/2.html
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg
+-rw-r--r--   0        0        0      205 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/3.html
+-rw-r--r--   0        0        0    31690 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg
+-rw-r--r--   0        0        0      115 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/4.html
+-rw-r--r--   0        0        0     9934 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/test_cli.py
+-rw-r--r--   0        0        0     8547 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/test_comic.py
+-rw-r--r--   0        0        0      608 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/test_comic_availability.py
+-rw-r--r--   0        0        0      934 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/test_docker.py
+-rw-r--r--   0        0        0     4068 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/tests/test_search.py
+-rw-r--r--   0        0        0      440 2023-07-31 17:02:22.040641 webcomix-3.6.7/webcomix/util.py
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 webcomix-3.6.7/PKG-INFO
```

### Comparing `webcomix-3.6.6/LICENSE` & `webcomix-3.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/README.md` & `webcomix-3.6.7/README.md`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/pyproject.toml` & `webcomix-3.6.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webcomix"
-version = "3.6.6"
+version = "3.6.7"
 description = "Webcomic downloader"
 authors = ["Jean-Christophe Pelletier <pelletierj97@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/J-CPelletier/webcomix"
 homepage = "https://github.com/J-CPelletier/webcomix"
 license = "MIT"
 classifiers = [
@@ -21,21 +21,22 @@
     "Framework :: Scrapy",
 ]
 packages = [
     { include = "webcomix" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.1"
+python = "^3.7"
 click = "^7.1.1"
 tqdm = "^4.43.0"
 Scrapy = "^2.5.1"
-scrapy-splash = "^0.8.0"
+scrapy-splash = "^0.9.0"
 scrapy-fake-useragent = "^1.4.4"
 docker = "^5.0.3"
+pytest-rerunfailures = "^11.1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.6.1"
 coveralls = "^3.2.0"
 mypy = "^0.910"
```

### Comparing `webcomix-3.6.6/webcomix/cli.py` & `webcomix-3.6.7/webcomix/cli.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/comic.py` & `webcomix-3.6.7/webcomix/comic.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/docker.py` & `webcomix-3.6.7/webcomix/docker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/crawler_worker.py` & `webcomix-3.6.7/webcomix/scrapy/crawler_worker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/download/comic_pipeline.py` & `webcomix-3.6.7/webcomix/scrapy/download/comic_pipeline.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/download/comic_spider.py` & `webcomix-3.6.7/webcomix/scrapy/download/comic_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/download/tests/test_comic_pipeline.py` & `webcomix-3.6.7/webcomix/scrapy/download/tests/test_comic_pipeline.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/download/tests/test_comic_spider.py` & `webcomix-3.6.7/webcomix/scrapy/download/tests/test_comic_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/tests/test_crawler_worker.py` & `webcomix-3.6.7/webcomix/scrapy/tests/test_crawler_worker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/tests/test_request_factory.py` & `webcomix-3.6.7/webcomix/scrapy/tests/test_request_factory.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/scrapy/verification/verification_spider.py` & `webcomix-3.6.7/webcomix/scrapy/verification/verification_spider.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/search.py` & `webcomix-3.6.7/webcomix/search.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/supported_comics.py` & `webcomix-3.6.7/webcomix/supported_comics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         "start_url": "https://xkcd.com/1/",
         "comic_image_selector": "//div[@id='comic']//img/@src",
         "next_page_selector": "//a[@rel='next']/@href",
         "alt_text": "//div[@id='comic']//img/@title",
     },
     "Nedroid": {
         "name": "Nedroid",
-        "start_url": "http://nedroid.com/2005/09/2210-whee/",
-        "comic_image_selector": "//div[@id='comic']//img/@src",
-        "next_page_selector": "//a[contains(@class, 'comic-nav-next')]/@href",
+        "start_url": "https://nedroid.com/?1",
+        "comic_image_selector": "//img[@class='comic']/@src",
+        "next_page_selector": "//a[text()='NEXT>']/@href",
     },
     "JL8": {
         "name": "JL8",
         "start_url": "https://limbero.org/jl8/1",
         "comic_image_selector": "//img[@alt='Comic']/@src",
         "next_page_selector": "//a[text()='>']/@href",
     },
```

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/fixture.py` & `webcomix-3.6.7/webcomix/tests/fake_websites/fixture.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage/1.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage/2.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage_searchable/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/one_webpage_searchable/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/1.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages/2.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_alt_text/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/1.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/2.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg` & `webcomix-3.6.7/webcomix/tests/fake_websites/three_webpages_classes/3.jpeg`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/test_cli.py` & `webcomix-3.6.7/webcomix/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/test_comic.py` & `webcomix-3.6.7/webcomix/tests/test_comic.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/test_docker.py` & `webcomix-3.6.7/webcomix/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/webcomix/tests/test_search.py` & `webcomix-3.6.7/webcomix/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `webcomix-3.6.6/PKG-INFO` & `webcomix-3.6.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: webcomix
-Version: 3.6.6
+Version: 3.6.7
 Summary: Webcomic downloader
 Home-page: https://github.com/J-CPelletier/webcomix
 License: MIT
 Author: Jean-Christophe Pelletier
 Author-email: pelletierj97@gmail.com
-Requires-Python: >=3.6.1,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: Scrapy (>=2.5.1,<3.0.0)
 Requires-Dist: click (>=7.1.1,<8.0.0)
 Requires-Dist: docker (>=5.0.3,<6.0.0)
+Requires-Dist: pytest-rerunfailures (>=11.1.2,<12.0.0)
 Requires-Dist: scrapy-fake-useragent (>=1.4.4,<2.0.0)
-Requires-Dist: scrapy-splash (>=0.8.0,<0.9.0)
+Requires-Dist: scrapy-splash (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.43.0,<5.0.0)
 Project-URL: Repository, https://github.com/J-CPelletier/webcomix
 Description-Content-Type: text/markdown
 
 # webcomix
 
 [![Build Status](https://github.com/J-CPelletier/webcomix/workflows/Build/badge.svg?branch=master)](https://github.com/J-CPelletier/webcomix/actions)[![Coverage Status](https://coveralls.io/repos/github/J-CPelletier/webcomix/badge.svg?branch=master)](https://coveralls.io/github/J-CPelletier/webcomix?branch=master)[![PyPI version](https://badge.fury.io/py/webcomix.svg)](https://badge.fury.io/py/webcomix)
```

