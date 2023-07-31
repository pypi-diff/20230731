# Comparing `tmp/renus-1.1.5.tar.gz` & `tmp/renus-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.5.tar", last modified: Mon May 22 06:20:34 2023, max compression
+gzip compressed data, was "renus-1.1.6.tar", last modified: Mon Jul 31 07:19:29 2023, max compression
```

## Comparing `renus-1.1.5.tar` & `renus-1.1.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.572210 renus-1.1.5/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.5/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-05-22 06:20:34.570207 renus-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.194105 renus-1.1.5/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.5/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.5/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.279211 renus-1.1.5/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.460191 renus-1.1.5/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.5/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0     1092 2023-05-15 10:24:30.000000 renus-1.1.5/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.5/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.5/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.5/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.479193 renus-1.1.5/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.5/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.519241 renus-1.1.5/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.5/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.554239 renus-1.1.5/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-05-21 06:32:06.000000 renus-1.1.5/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.5/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.609627 renus-1.1.5/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     3760 2023-05-22 06:18:46.000000 renus-1.1.5/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     4148 2023-05-22 06:14:27.000000 renus-1.1.5/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.5/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.647300 renus-1.1.5/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.5/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.444233 renus-1.1.5/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.5/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/config.py
--rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.5/renus/core/cprint.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.5/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.5/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.5/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.5/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/middleware.py
--rw-rw-rw-   0        0        0    15322 2023-05-15 10:26:37.000000 renus-1.1.5/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.5/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.5/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.5/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.5/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.5/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.534207 renus-1.1.5/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.5/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.5/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.566206 renus-1.1.5/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.5/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.215105 renus-1.1.5/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-05-22 06:20:33.000000 renus-1.1.5/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 06:20:34.573167 renus-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-05-22 06:19:43.000000 renus-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.882069 renus-1.1.6/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-07-31 07:19:29.881067 renus-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.323069 renus-1.1.6/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.6/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.6/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.379068 renus-1.1.6/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.411086 renus-1.1.6/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1849 2023-07-31 07:12:37.000000 renus-1.1.6/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0      932 2023-07-31 07:19:07.000000 renus-1.1.6/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.6/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4262 2023-06-20 08:05:47.000000 renus-1.1.6/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.6/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.428084 renus-1.1.6/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.6/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.442083 renus-1.1.6/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.6/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.463089 renus-1.1.6/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-21 06:32:06.000000 renus-1.1.6/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.6/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.512090 renus-1.1.6/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     3760 2023-05-22 06:18:46.000000 renus-1.1.6/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     4148 2023-05-22 06:14:27.000000 renus-1.1.6/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.6/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.529089 renus-1.1.6/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.6/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.6/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.824083 renus-1.1.6/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.6/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/config.py
+-rw-rw-rw-   0        0        0     2271 2023-06-20 12:25:48.000000 renus-1.1.6/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.6/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.6/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.6/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.6/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    15511 2023-07-05 07:28:40.000000 renus-1.1.6/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.6/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.6/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.6/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.6/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1514 2023-06-27 07:00:06.000000 renus-1.1.6/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.860072 renus-1.1.6/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.6/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.6/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.6/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.880087 renus-1.1.6/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.6/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.6/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:19:29.339084 renus-1.1.6/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 07:19:29.000000 renus-1.1.6/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:19:29.882069 renus-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-07-31 07:15:20.000000 renus-1.1.6/setup.py
```

### Comparing `renus-1.1.5/LICENSE` & `renus-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/app.py` & `renus-1.1.6/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/app/controller.temp` & `renus-1.1.6/renus/commands/app/controller.temp`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from renus.core.request import Request
-from app.{name}.model import {name_camel}
+from app.{name}.model import {names_camel}
 from renus.core.response import JsonResponse
 from renus.core.validation.validate import Validate,vr
+from app.extension.renus.table.model import Table
 
 class {name_camel}Controller:
     def __init__(self,request:Request) -> None:
         self.request=request
 
     @property
     def __inputs(self):
@@ -13,15 +14,15 @@
 
     def index(self):
         """
         Get {name_camel} Records
         :method: get
         :return: JsonResponse of CRUD table
         """
-        m={name_camel}(self.request)
+        m=Table({names_camel}(self.request))
         m.fields = {
             '_id': {"type": "text-input", "formInput": False},
             'updated_at': {"type": "time-ago", "formInput": False},
             'created_at': {"type": "date-input", "formInput": False, "sortable": False, }
             }
         m.search_fields = []
         return JsonResponse(m.index())
@@ -29,30 +30,30 @@
     def store(self):
         """
         Add new {name_camel} Item
         :method: post
         :return: JsonResponse
         """
 
-        {name_camel}(self.request).create(self.__inputs)
+        {names_camel}(self.request).create(self.__inputs)
         return JsonResponse({'msg': 'stored'})
 
     def update(self, id):
         """
         Update {name_camel} where _id is id
         :method: put
         :param id: {name_camel} _id
         :return: JsonResponse
         """
 
-        {name_camel}(self.request).where({'_id': id}).update(self.__inputs)
+        {names_camel}(self.request).where({'_id': id}).update(self.__inputs)
         return JsonResponse({'msg': 'updated'})
 
     def delete(self, id):
         """
         Delete {name_camel} where _id is id
         :method: delete
         :param id: {name_camel} _id
         :return: JsonResponse
         """
-        {name_camel}(self.request).where({'_id': id}).delete()
+        {names_camel}(self.request).where({'_id': id}).delete()
         return JsonResponse({'msg': 'deleted'})
```

### Comparing `renus-1.1.5/renus/commands/app/model.temp` & `renus-1.1.6/renus/commands/app/model.temp`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import typing
 from datetime import datetime
 from bson import ObjectId
 from renus.core.model import ModelBase
 from app.extension.renus.activity.service import ActivityService
-from app.extension.renus.crud.model import CRUD
-from app.extension.renus.storage.model import Storage
 
-class _Base(dict):
+class {name_camel}:
     _id: ObjectId
     created_at: datetime
     updated_at: datetime
 
     def __init__(self, doc):
-        super().__init__(doc)
         for k, v in doc.items():
             setattr(self, k, v)
 
 
-class {name_camel}(ModelBase,CRUD):
+class {names_camel}(ModelBase):
     collection_name="{name_db}"
-    document_model=_Base
-    storage = Storage(None)
+    document_model={name_camel}
 
     def __init__(self,request) -> None:
         super().__init__()
         self.request=request
 
     def get(self,police: bool = True) -> typing.List[document_model]:
         return self._get(police)
```

### Comparing `renus-1.1.5/renus/commands/app/route.temp` & `renus-1.1.6/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/app/run.py` & `renus-1.1.6/renus/commands/app/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 route_temp = pkg_resources.resource_filename('renus', './commands/app/route.temp')
 
 def to_camel_case(snake_str):
     components = snake_str.split('_')
     return ''.join(x.title() for x in components)
 
 
-def add_temp(name,names, name_camel, name_db,folder:list):
+def add_temp(name,names, name_camel,names_camel, name_db,folder:list):
     pth = 'app/'
     pname = ''
     vname = ''
     if len(folder) > 0:
         pth += '/'.join(folder) + '/'
         pname = '.'.join(folder) + '.'
         vname = '/'+'/'.join(folder)+'/'
@@ -26,14 +26,15 @@
         all=all.replace('{name}',pname+name)
         all=all.replace('{name_camel}',name_camel)
         with open(pth+'controller.py','w') as controller:
             controller.write(all)
 
     with open(model_temp,'r') as file:
         all=file.read()
+        all=all.replace('{names_camel}',names_camel)
         all=all.replace('{name_camel}',name_camel)
         all=all.replace('{name_db}',name_db)
         with open(pth+'model.py','w') as controller:
             controller.write(all)
 
     with open(vue_temp,'r') as file:
         os.makedirs('./frontend/src/views/admin/'+vname.lstrip('/'), exist_ok=True)
@@ -107,14 +108,15 @@
     name = input('name (single lowercase):').lower()
     folder=name.split('.')
     name=folder[-1]
     folder=folder[:-1]
     name_camel = to_camel_case(name)
     names = to_plural(to_camel_case(name))
     names = names[0].lower() + names[1:]
+    names_camel = to_camel_case(names)
     name_db = name.replace('_', '-')
 
-    add_temp(name, names, name_camel, name_db,folder)
+    add_temp(name, names, name_camel,names_camel, name_db,folder)
     print('templates created.')
     add_routes(name, names, name_camel,folder)
     print('routes created.')
     print(f'{name} is done.')
```

### Comparing `renus-1.1.5/renus/commands/backup/run.py` & `renus-1.1.6/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/copy/run.py` & `renus-1.1.6/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/default/run.py` & `renus-1.1.6/renus/commands/default/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/help.py` & `renus-1.1.6/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/install/build.py` & `renus-1.1.6/renus/commands/install/build.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/install/run.py` & `renus-1.1.6/renus/commands/install/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/install/service.py` & `renus-1.1.6/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/commands/permission/run.py` & `renus-1.1.6/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/cache.py` & `renus-1.1.6/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/concurrency.py` & `renus-1.1.6/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/cprint.py` & `renus-1.1.6/renus/core/cprint.py`

 * *Files 10% similar despite different names*

```diff
@@ -101,12 +101,7 @@
     @staticmethod
     def bg_cyan(txt):
         return f'\033[46m{txt}\033[0m'
 
     @staticmethod
     def bg_grey(txt):
         return f'\033[47m{txt}\033[0m'
-
-
-if __name__ == "__main__":
-    c = Cprint()
-    c.print(c.bg_cyan('test ' + c.red('ok')))
```

### Comparing `renus-1.1.5/renus/core/crypt.py` & `renus-1.1.6/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/datastructures.py` & `renus-1.1.6/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/exception.py` & `renus-1.1.6/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/formparsers.py` & `renus-1.1.6/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/injection.py` & `renus-1.1.6/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/log.py` & `renus-1.1.6/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/model.py` & `renus-1.1.6/renus/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import typing
 from bson import ObjectId
 from pymongo import MongoClient
 from datetime import datetime
 from renus.core.config import Config
+from renus.core.cprint import Cprint
 
 
 class ModelBase:
     _client = MongoClient(Config('database').get('host', '127.0.0.1'),
                           Config('database').get('port', 27017),
                           username=Config('database').get('username', None),
                           password=Config('database').get('password', None))
@@ -61,18 +62,14 @@
         self._limit = None
         self._skip = None
         self._sort = None
         self._select = None
         self.visible_fields = []
         return self
 
-    def create_index(self, fields, unique=False):
-        return self.collection().create_index(fields,
-                                              unique=unique)
-
     def aggregate(self, pipeline: typing.Any, session: typing.Any = None):
         return self.__police(self.collection().aggregate(pipeline, session))
 
     def where(self, where: dict):
         if self._steps is not None:
             self._steps.append({
                 "$match": where
@@ -170,15 +167,18 @@
                     "from": collection,
                     "localField": local_field,
                     "foreignField": forigen_field,
                     "as": to
                 }
             })
             if single:
-                self._steps.append({'$unwind': f'${to}'})
+                self._steps.append({ '$addFields':{ f'{to}': {'$arrayElemAt': [ f"${to}", 0 ]} }})
+        else:
+            c=Cprint()
+            c.print(c.red('use steps mode for with_relation.'))
         return self
 
     def steps(self):
         self._steps = []
         return self
 
     def _get(self, police: bool = True) -> typing.List[document_model]:
@@ -246,30 +246,36 @@
         if self.add_time_fields:
             new["updated_at"] = datetime.utcnow()
         d = {"$set": new}
         if self.add_time_fields and "created_at" not in new:
             d["$setOnInsert"] = {'created_at': datetime.utcnow()}
         old = self.collection().find_one_and_update(where, d, upsert=upsert)
         self.boot_event('update', old, new)
-        new['_id'] = old['_id']
+        if old is None:
+            new={'_id':'upsert','doc':new}
+        else:
+            new['_id'] = old['_id']
         self._attach_file(new)
         return old if get_old else True
 
     def update_opt(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
         if '$setOnInsert' not in new:
             new['$setOnInsert'] = {}
         if self.add_time_fields:
             new['$set']["updated_at"] = datetime.utcnow()
             new['$setOnInsert']['created_at'] = datetime.utcnow()
         old = self.collection().find_one_and_update(where, new, upsert=upsert)
         self.boot_event('update', old, {k[1:]: v for k, v in new.items()})
-        new['_id'] = old['_id']
+        if old is None:
+            new={'_id':'upsert','doc':new}
+        else:
+            new['_id'] = old['_id']
         self._attach_file(new)
         return old if get_old else True
 
     def update_opt_many(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
```

### Comparing `renus-1.1.5/renus/core/request.py` & `renus-1.1.6/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/response.py` & `renus-1.1.6/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/routing.py` & `renus-1.1.6/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/schedule.py` & `renus-1.1.6/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/serialize.py` & `renus-1.1.6/renus/core/serialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
             r = o.isoformat()
             if o.microsecond:
                 r = r[:12]
             return r
 
         elif isinstance(o, (dict, list, tuple, str, int, float, bool, type(None))):
             return super().default(o)
+        elif hasattr(o, '__dict__'):
+            return dict(o)
         else:
             return str(o)
 
 
 def json_decoder(value):
     if isinstance(value, dict):
         for k, v in value.items():
```

### Comparing `renus-1.1.5/renus/core/status.py` & `renus-1.1.6/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/validation/rules.py` & `renus-1.1.6/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/validation/validate.py` & `renus-1.1.6/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/core/websockets.py` & `renus-1.1.6/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus/util/helper.py` & `renus-1.1.6/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.5/renus.egg-info/SOURCES.txt` & `renus-1.1.6/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

