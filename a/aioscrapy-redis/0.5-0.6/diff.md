# Comparing `tmp/aioscrapy_redis-0.5.tar.gz` & `tmp/aioscrapy_redis-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioscrapy_redis-0.5.tar", last modified: Sat Jul 29 03:29:21 2023, max compression
+gzip compressed data, was "aioscrapy_redis-0.6.tar", last modified: Mon Jul 31 01:07:30 2023, max compression
```

## Comparing `aioscrapy_redis-0.5.tar` & `aioscrapy_redis-0.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.784538 aioscrapy_redis-0.5/
--rw-rw-rw-   0        0        0     1094 2023-07-29 03:29:21.783540 aioscrapy_redis-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      613 2021-02-19 10:07:03.000000 aioscrapy_redis-0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.705642 aioscrapy_redis-0.5/aioscrapy_redis/
--rw-rw-rw-   0        0        0       26 2023-07-29 03:24:34.000000 aioscrapy_redis-0.5/aioscrapy_redis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.733320 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/
--rw-rw-rw-   0        0        0      193 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/__init__.py
--rw-rw-rw-   0        0        0      192 2020-07-27 05:53:14.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/common.py
--rw-rw-rw-   0        0        0     1218 2021-01-05 09:44:53.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/connection.py
--rw-rw-rw-   0        0        0      727 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/defaults.py
--rw-rw-rw-   0        0        0     2820 2021-02-19 08:59:08.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/dupefilter.py
--rw-rw-rw-   0        0        0      263 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/picklecompat.py
--rw-rw-rw-   0        0        0     1201 2021-02-19 08:59:08.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/pipelines.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.742321 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/
--rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/__init__.py
--rw-rw-rw-   0        0        0      912 2020-08-04 09:23:58.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/decorators.py
--rw-rw-rw-   0        0        0     1396 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/exceptions.py
--rw-rw-rw-   0        0        0     4929 2023-07-29 03:24:34.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/misc.py
--rw-rw-rw-   0        0        0    11894 2021-01-05 09:44:53.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/python.py
--rw-rw-rw-   0        0        0     2474 2021-01-05 09:44:53.000000 aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/reqser.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.748320 aioscrapy_redis-0.5/aioscrapy_redis/core/
--rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.751321 aioscrapy_redis-0.5/aioscrapy_redis/core/downloader/
--rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/downloader/__init__.py
--rw-rw-rw-   0        0        0     5889 2021-02-19 09:08:54.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/downloader/downloader.py
--rw-rw-rw-   0        0        0     7870 2021-02-19 09:15:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/engine.py
--rw-rw-rw-   0        0        0     2130 2021-02-19 09:17:19.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/scheduler.py
--rw-rw-rw-   0        0        0     3387 2023-07-28 04:09:58.000000 aioscrapy_redis-0.5/aioscrapy_redis/core/spider.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.754316 aioscrapy_redis-0.5/aioscrapy_redis/downloadermiddlewares/
--rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/downloadermiddlewares/__init__.py
--rw-rw-rw-   0        0        0      310 2021-02-19 08:59:08.000000 aioscrapy_redis-0.5/aioscrapy_redis/downloadermiddlewares/middlewares.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.764320 aioscrapy_redis-0.5/aioscrapy_redis/https/
--rw-rw-rw-   0        0        0        0 2020-04-07 01:45:44.000000 aioscrapy_redis-0.5/aioscrapy_redis/https/__init__.py
--rw-rw-rw-   0        0        0     8210 2021-02-19 09:25:10.000000 aioscrapy_redis-0.5/aioscrapy_redis/https/form.py
--rw-rw-rw-   0        0        0      184 2021-01-05 09:35:42.000000 aioscrapy_redis-0.5/aioscrapy_redis/https/html.py
--rw-rw-rw-   0        0        0     3062 2021-02-19 09:23:49.000000 aioscrapy_redis-0.5/aioscrapy_redis/https/request.py
--rw-rw-rw-   0        0        0     3488 2021-02-19 09:21:56.000000 aioscrapy_redis-0.5/aioscrapy_redis/https/response.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.782527 aioscrapy_redis-0.5/aioscrapy_redis/utils/
--rw-rw-rw-   0        0        0       29 2023-07-28 02:06:49.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/__init__.py
--rw-rw-rw-   0        0        0     7983 2023-07-29 03:24:34.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/basesettings.py
--rw-rw-rw-   0        0        0     3996 2021-02-19 08:59:08.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/get_settings.py
--rw-rw-rw-   0        0        0   109627 2020-08-24 01:29:51.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/header_ua.py
--rw-rw-rw-   0        0        0      224 2020-04-13 08:22:49.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/http_proxy.py
--rw-rw-rw-   0        0        0     5539 2021-01-05 09:52:50.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/item.py
--rw-rw-rw-   0        0        0      755 2021-02-19 09:37:56.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/log.py
--rw-rw-rw-   0        0        0     2307 2021-02-19 09:38:29.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/logstats.py
--rw-rw-rw-   0        0        0     1223 2021-01-05 09:52:50.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/serialize.py
--rw-rw-rw-   0        0        0      104 2020-07-23 08:05:00.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/settings.py
--rw-rw-rw-   0        0        0     1688 2021-02-19 09:41:10.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/tools.py
--rw-rw-rw-   0        0        0      534 2020-08-04 08:56:10.000000 aioscrapy_redis-0.5/aioscrapy_redis/utils/trackref.py
-drwxrwxrwx   0        0        0        0 2023-07-29 03:29:21.720388 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/
--rw-rw-rw-   0        0        0     1094 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1767 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      126 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-29 03:29:21.000000 aioscrapy_redis-0.5/aioscrapy_redis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 03:29:21.784538 aioscrapy_redis-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1269 2023-07-29 03:27:44.000000 aioscrapy_redis-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.731878 aioscrapy_redis-0.6/
+-rw-rw-rw-   0        0        0     1383 2023-07-31 01:07:30.731878 aioscrapy_redis-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      613 2021-02-19 10:07:03.000000 aioscrapy_redis-0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.632170 aioscrapy_redis-0.6/aioscrapy_redis/
+-rw-rw-rw-   0        0        0       26 2023-07-29 03:24:34.000000 aioscrapy_redis-0.6/aioscrapy_redis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.659073 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/
+-rw-rw-rw-   0        0        0      193 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/__init__.py
+-rw-rw-rw-   0        0        0      192 2020-07-27 05:53:14.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/common.py
+-rw-rw-rw-   0        0        0     1218 2021-01-05 09:44:53.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/connection.py
+-rw-rw-rw-   0        0        0      727 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/defaults.py
+-rw-rw-rw-   0        0        0     2820 2021-02-19 08:59:08.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/dupefilter.py
+-rw-rw-rw-   0        0        0      263 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/picklecompat.py
+-rw-rw-rw-   0        0        0     1201 2021-02-19 08:59:08.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/pipelines.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.671042 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/
+-rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/__init__.py
+-rw-rw-rw-   0        0        0      912 2020-08-04 09:23:58.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/decorators.py
+-rw-rw-rw-   0        0        0     1396 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/exceptions.py
+-rw-rw-rw-   0        0        0     4929 2023-07-29 03:24:34.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/misc.py
+-rw-rw-rw-   0        0        0    11894 2021-01-05 09:44:53.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/python.py
+-rw-rw-rw-   0        0        0     2474 2021-01-05 09:44:53.000000 aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/reqser.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.678049 aioscrapy_redis-0.6/aioscrapy_redis/core/
+-rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.683009 aioscrapy_redis-0.6/aioscrapy_redis/core/downloader/
+-rw-rw-rw-   0        0        0       24 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/downloader/__init__.py
+-rw-rw-rw-   0        0        0     5889 2021-02-19 09:08:54.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/downloader/downloader.py
+-rw-rw-rw-   0        0        0     7870 2021-02-19 09:15:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/engine.py
+-rw-rw-rw-   0        0        0     2130 2021-02-19 09:17:19.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/scheduler.py
+-rw-rw-rw-   0        0        0     3387 2023-07-28 04:09:58.000000 aioscrapy_redis-0.6/aioscrapy_redis/core/spider.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.686998 aioscrapy_redis-0.6/aioscrapy_redis/downloadermiddlewares/
+-rw-rw-rw-   0        0        0       72 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/downloadermiddlewares/__init__.py
+-rw-rw-rw-   0        0        0      310 2021-02-19 08:59:08.000000 aioscrapy_redis-0.6/aioscrapy_redis/downloadermiddlewares/middlewares.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.698966 aioscrapy_redis-0.6/aioscrapy_redis/https/
+-rw-rw-rw-   0        0        0        0 2020-04-07 01:45:44.000000 aioscrapy_redis-0.6/aioscrapy_redis/https/__init__.py
+-rw-rw-rw-   0        0        0     8210 2021-02-19 09:25:10.000000 aioscrapy_redis-0.6/aioscrapy_redis/https/form.py
+-rw-rw-rw-   0        0        0      184 2021-01-05 09:35:42.000000 aioscrapy_redis-0.6/aioscrapy_redis/https/html.py
+-rw-rw-rw-   0        0        0     3062 2021-02-19 09:23:49.000000 aioscrapy_redis-0.6/aioscrapy_redis/https/request.py
+-rw-rw-rw-   0        0        0     3488 2021-02-19 09:21:56.000000 aioscrapy_redis-0.6/aioscrapy_redis/https/response.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.728887 aioscrapy_redis-0.6/aioscrapy_redis/utils/
+-rw-rw-rw-   0        0        0       29 2023-07-28 02:06:49.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/__init__.py
+-rw-rw-rw-   0        0        0     8057 2023-07-31 01:05:38.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/basesettings.py
+-rw-rw-rw-   0        0        0     3996 2021-02-19 08:59:08.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/get_settings.py
+-rw-rw-rw-   0        0        0   109627 2020-08-24 01:29:51.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/header_ua.py
+-rw-rw-rw-   0        0        0      224 2020-04-13 08:22:49.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/http_proxy.py
+-rw-rw-rw-   0        0        0     5539 2021-01-05 09:52:50.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/item.py
+-rw-rw-rw-   0        0        0      755 2021-02-19 09:37:56.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/log.py
+-rw-rw-rw-   0        0        0     2307 2021-02-19 09:38:29.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/logstats.py
+-rw-rw-rw-   0        0        0     1223 2021-01-05 09:52:50.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/serialize.py
+-rw-rw-rw-   0        0        0      104 2020-07-23 08:05:00.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/settings.py
+-rw-rw-rw-   0        0        0     1688 2021-02-19 09:41:10.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/tools.py
+-rw-rw-rw-   0        0        0      534 2020-08-04 08:56:10.000000 aioscrapy_redis-0.6/aioscrapy_redis/utils/trackref.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:07:30.645135 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/
+-rw-rw-rw-   0        0        0     1383 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1767 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      126 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-31 01:07:30.000000 aioscrapy_redis-0.6/aioscrapy_redis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 01:07:30.732876 aioscrapy_redis-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2023-07-31 01:03:30.000000 aioscrapy_redis-0.6/setup.py
```

### Comparing `aioscrapy_redis-0.5/README.md` & `aioscrapy_redis-0.6/README.md`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/connection.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/connection.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/defaults.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/defaults.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/dupefilter.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/dupefilter.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/pipelines.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/pipelines.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/decorators.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/exceptions.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/misc.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/python.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/python.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/aioscrapyredis/utils/reqser.py` & `aioscrapy_redis-0.6/aioscrapy_redis/aioscrapyredis/utils/reqser.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/core/downloader/downloader.py` & `aioscrapy_redis-0.6/aioscrapy_redis/core/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/core/engine.py` & `aioscrapy_redis-0.6/aioscrapy_redis/core/engine.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/core/scheduler.py` & `aioscrapy_redis-0.6/aioscrapy_redis/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/core/spider.py` & `aioscrapy_redis-0.6/aioscrapy_redis/core/spider.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/https/form.py` & `aioscrapy_redis-0.6/aioscrapy_redis/https/form.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/https/request.py` & `aioscrapy_redis-0.6/aioscrapy_redis/https/request.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/https/response.py` & `aioscrapy_redis-0.6/aioscrapy_redis/https/response.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/basesettings.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/basesettings.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,20 @@
 # Author:lw
 import copy
 
 import json
 import six
 from importlib import import_module
 from pprint import pformat
-from collections import MutableMapping
-import os, sys
+try:
+    from collections import MutableMapping
+except:
+    from collections.abc import MutableMapping
+import os
+import sys
 
 SETTINGS_PRIORITIES = {
     'default': 0,
     'command': 10,
     'project': 20,
     'spider': 30,
     'cmdline': 40,
```

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/get_settings.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/get_settings.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/header_ua.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/header_ua.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/item.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/item.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/log.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/log.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/logstats.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/logstats.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/serialize.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/tools.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis/utils/trackref.py` & `aioscrapy_redis-0.6/aioscrapy_redis/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/aioscrapy_redis.egg-info/SOURCES.txt` & `aioscrapy_redis-0.6/aioscrapy_redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioscrapy_redis-0.5/setup.py` & `aioscrapy_redis-0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 try:
     install_requires = [str(ir.req) for ir in parse_requirements("requirements.txt", session=False)]
 except:
     install_requires = [str(ir.requirement) for ir in parse_requirements("requirements.txt", session=False)]
 
 setup(
     name='aioscrapy_redis',
-    version=0.5,
+    version=0.6,
     description='A mini spider framework, Integrate aiohttp into scrapy',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(exclude=[]),
     author='道法自然_Tor',
     author_email='1540310556@qq.com',
     license='Apache License v2',
```

