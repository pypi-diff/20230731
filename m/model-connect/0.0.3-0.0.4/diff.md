# Comparing `tmp/model-connect-0.0.3.tar.gz` & `tmp/model-connect-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model-connect-0.0.3.tar", last modified: Mon Jul 31 00:38:37 2023, max compression
+gzip compressed data, was "model-connect-0.0.4.tar", last modified: Mon Jul 31 02:59:24 2023, max compression
```

## Comparing `model-connect-0.0.3.tar` & `model-connect-0.0.4.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.607752 model-connect-0.0.3/
--rw-rw-rw-   0        0        0    11395 2023-07-31 00:38:37.607752 model-connect-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    11292 2023-07-31 00:38:26.000000 model-connect-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.556849 model-connect-0.0.3/model_connect/
--rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.3/model_connect/__init__.py
--rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.3/model_connect/connect.py
--rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.3/model_connect/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.581160 model-connect-0.0.3/model_connect/integrations/
--rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.3/model_connect/integrations/__init__.py
--rw-rw-rw-   0        0        0      807 2023-07-30 22:28:32.000000 model-connect-0.0.3/model_connect/integrations/base.py
--rw-rw-rw-   0        0        0      476 2023-07-30 21:04:25.000000 model-connect-0.0.3/model_connect/integrations/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.581160 model-connect-0.0.3/model_connect/integrations/fastapi/
--rw-rw-rw-   0        0        0      345 2023-07-30 18:45:18.000000 model-connect-0.0.3/model_connect/integrations/fastapi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.584709 model-connect-0.0.3/model_connect/integrations/fastapi/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/__init__.py
--rw-rw-rw-   0        0        0     1024 2023-07-30 18:52:41.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/model.py
--rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.3/model_connect/integrations/fastapi/options/model_field.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.590726 model-connect-0.0.3/model_connect/integrations/psycopg2/
--rw-rw-rw-   0        0        0      478 2023-07-30 19:40:57.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/__init__.py
--rw-rw-rw-   0        0        0      577 2023-07-28 02:51:40.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/commons.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/delete.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:34.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/insert.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.594084 model-connect-0.0.3/model_connect/integrations/psycopg2/options/
--rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/__init__.py
--rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/model.py
--rw-rw-rw-   0        0        0      633 2023-07-30 21:31:14.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/options/model_field.py
--rw-rw-rw-   0        0        0     6001 2023-07-30 23:55:10.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/select.py
--rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.3/model_connect/integrations/psycopg2/update.py
--rw-rw-rw-   0        0        0      533 2023-07-30 21:05:26.000000 model-connect-0.0.3/model_connect/integrations/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.596074 model-connect-0.0.3/model_connect/options/
--rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.3/model_connect/options/__init__.py
--rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.3/model_connect/options/connect.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.598073 model-connect-0.0.3/model_connect/options/global/
--rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.3/model_connect/options/global/__init__.py
--rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.3/model_connect/options/global/global.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.601074 model-connect-0.0.3/model_connect/options/model/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.3/model_connect/options/model/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-07-30 22:31:01.000000 model-connect-0.0.3/model_connect/options/model/model.py
--rw-rw-rw-   0        0        0     1508 2023-07-30 20:33:29.000000 model-connect-0.0.3/model_connect/options/model/query_params.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.602592 model-connect-0.0.3/model_connect/options/model_field/
--rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.3/model_connect/options/model_field/__init__.py
--rw-rw-rw-   0        0        0     3492 2023-07-30 22:35:02.000000 model-connect-0.0.3/model_connect/options/model_field/model_field.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.605611 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/
--rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/__init__.py
--rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/request.py
--rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/response.py
--rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.3/model_connect/registry.py
-drwxrwxrwx   0        0        0        0 2023-07-31 00:38:37.576593 model-connect-0.0.3/model_connect.egg-info/
--rw-rw-rw-   0        0        0    11395 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1667 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-31 00:38:37.000000 model-connect-0.0.3/model_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 00:38:37.607752 model-connect-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      598 2023-07-31 00:38:35.000000 model-connect-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.167861 model-connect-0.0.4/
+-rw-rw-rw-   0        0        0    10921 2023-07-31 02:59:24.167861 model-connect-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10818 2023-07-31 00:53:30.000000 model-connect-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.032334 model-connect-0.0.4/model_connect/
+-rw-rw-rw-   0        0        0       43 2023-07-30 16:19:42.000000 model-connect-0.0.4/model_connect/__init__.py
+-rw-rw-rw-   0        0        0      448 2023-07-30 19:34:46.000000 model-connect-0.0.4/model_connect/connect.py
+-rw-rw-rw-   0        0        0      452 2023-07-30 21:18:40.000000 model-connect-0.0.4/model_connect/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.075907 model-connect-0.0.4/model_connect/integrations/
+-rw-rw-rw-   0        0        0        0 2023-07-26 01:21:47.000000 model-connect-0.0.4/model_connect/integrations/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-07-31 00:56:43.000000 model-connect-0.0.4/model_connect/integrations/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.092996 model-connect-0.0.4/model_connect/integrations/fastapi/
+-rw-rw-rw-   0        0        0      401 2023-07-31 01:00:27.000000 model-connect-0.0.4/model_connect/integrations/fastapi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.107411 model-connect-0.0.4/model_connect/integrations/fastapi/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:41:37.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-07-31 00:49:20.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/model.py
+-rw-rw-rw-   0        0        0      137 2023-07-30 18:53:36.000000 model-connect-0.0.4/model_connect/integrations/fastapi/options/model_field.py
+-rw-rw-rw-   0        0        0      504 2023-07-31 00:52:20.000000 model-connect-0.0.4/model_connect/integrations/fastapi/router.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.112916 model-connect-0.0.4/model_connect/integrations/psycopg2/
+-rw-rw-rw-   0        0        0      846 2023-07-31 02:56:09.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.115915 model-connect-0.0.4/model_connect/integrations/psycopg2/common/
+-rw-rw-rw-   0        0        0        0 2023-07-31 01:29:50.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/__init__.py
+-rw-rw-rw-   0        0        0     3854 2023-07-31 02:03:39.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/processing.py
+-rw-rw-rw-   0        0        0      577 2023-07-31 01:34:36.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/common/streaming.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:37.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/delete.py
+-rw-rw-rw-   0        0        0     2811 2023-07-31 02:33:09.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/insert.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.125104 model-connect-0.0.4/model_connect/integrations/psycopg2/options/
+-rw-rw-rw-   0        0        0        0 2023-07-30 17:40:26.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/__init__.py
+-rw-rw-rw-   0        0        0      823 2023-07-30 22:17:23.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/model.py
+-rw-rw-rw-   0        0        0     1110 2023-07-31 02:27:12.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/options/model_field.py
+-rw-rw-rw-   0        0        0     2993 2023-07-31 02:33:07.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/select.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 03:23:16.000000 model-connect-0.0.4/model_connect/integrations/psycopg2/update.py
+-rw-rw-rw-   0        0        0      840 2023-07-31 01:16:35.000000 model-connect-0.0.4/model_connect/integrations/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.132690 model-connect-0.0.4/model_connect/options/
+-rw-rw-rw-   0        0        0      131 2023-07-30 18:37:32.000000 model-connect-0.0.4/model_connect/options/__init__.py
+-rw-rw-rw-   0        0        0      861 2023-07-30 21:15:19.000000 model-connect-0.0.4/model_connect/options/connect.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.145247 model-connect-0.0.4/model_connect/options/global/
+-rw-rw-rw-   0        0        0       32 2023-07-30 18:37:25.000000 model-connect-0.0.4/model_connect/options/global/__init__.py
+-rw-rw-rw-   0        0        0       31 2023-07-30 06:55:47.000000 model-connect-0.0.4/model_connect/options/global/global.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.149233 model-connect-0.0.4/model_connect/options/model/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:17.000000 model-connect-0.0.4/model_connect/options/model/__init__.py
+-rw-rw-rw-   0        0        0     2017 2023-07-31 02:56:34.000000 model-connect-0.0.4/model_connect/options/model/model.py
+-rw-rw-rw-   0        0        0     1508 2023-07-31 02:03:06.000000 model-connect-0.0.4/model_connect/options/model/query_params.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.151296 model-connect-0.0.4/model_connect/options/model_field/
+-rw-rw-rw-   0        0        0        0 2023-07-30 18:34:14.000000 model-connect-0.0.4/model_connect/options/model_field/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.166015 model-connect-0.0.4/model_connect/options/model_field/dtos/
+-rw-rw-rw-   0        0        0        0 2023-07-30 15:43:39.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/__init__.py
+-rw-rw-rw-   0        0        0     1631 2023-07-30 22:34:35.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/request.py
+-rw-rw-rw-   0        0        0     1544 2023-07-30 22:34:35.000000 model-connect-0.0.4/model_connect/options/model_field/dtos/response.py
+-rw-rw-rw-   0        0        0     3446 2023-07-31 02:03:39.000000 model-connect-0.0.4/model_connect/options/model_field/model_field.py
+-rw-rw-rw-   0        0        0      678 2023-07-30 22:50:35.000000 model-connect-0.0.4/model_connect/registry.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:59:24.058434 model-connect-0.0.4/model_connect.egg-info/
+-rw-rw-rw-   0        0        0    10921 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1723 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-31 02:59:23.000000 model-connect-0.0.4/model_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:59:24.167861 model-connect-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-07-31 02:59:11.000000 model-connect-0.0.4/setup.py
```

### Comparing `model-connect-0.0.3/PKG-INFO` & `model-connect-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-connect
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
@@ -110,132 +110,132 @@
 In fact, most complex applications will use these modules to handle unique business logic.
 But what this is demonstrating is that for a simple setup (where most of the code in these layers are boilerplate),
 you can remove these modules and just use the model as the scaffolding.
 
 ```python
 from fastapi import Depends
 from model_connect.integrations.fastapi import (
-    create_router,
-    create_response_dtos,
-    create_response_dto,
-    get_from_post_request_dto,
-    get_from_post_request_dtos,
-    get_from_put_request_dto,
-    get_from_patch_request_dto,
-    get_filter_options,
-    get_pagination_options,
-    get_sort_options
+  create_router,
+  create_response_dtos,
+  create_response_dto,
+  get_from_post_request_dto,
+  get_from_post_request_dtos,
+  get_from_put_request_dto,
+  get_from_patch_request_dto,
+  get_filter_options,
+  get_pagination_options,
+  get_sort_options
 )
 from model_connect.integrations.psycopg2 import (
-    stream_select,
-    stream_insert,
-    stream_update,
-    stream_partial_update,
-    stream_delete,
+  stream_select,
+  stream_insert,
+  stream_update,
+  stream_partial_update,
+  stream_delete,
 )
 
 from src.models import User
 from src.db import open_db_connection
 
 router = create_router(User)
 
 
 @router.get('')
 def get_users(
         filter_options: dict = Depends(get_filter_options(User)),
         pagination_options: dict = Depends(get_pagination_options(User)),
         sort_options: dict = Depends(get_sort_options(User))
 ):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_select(
-                User,
-                cursor,
-                filter_options=filter_options,
-                pagination_options=pagination_options,
-                sort_options=sort_options
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_select(
+        User,
+        cursor,
+        filter_options=filter_options,
+        pagination_options=pagination_options,
+        sort_options=sort_options
+      )
+    )
 
 
 @router.get('/{resource_id}')
 def get_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_select(
-                User,
-                cursor,
-                filter_options={'id': resource_id}
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_select(
+        User,
+        cursor,
+        filter_options={'id': resource_id}
+      )
+    )
 
 
 @router.post('')
 def post_user(user: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_insert(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_insert(
+        cursor,
+        user
+      )
+    )
 
 
 @router.post('/bulk')
 def post_users(users: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_insert(
-                cursor,
-                users,
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_insert(
+        cursor,
+        users,
+      )
+    )
 
 
 @router.put('/{resource_id}')
 def put_user(user: Depends(get_from_put_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.patch('/{resource_id}')
 def patch_user(user: Depends(get_from_patch_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_partial_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_partial_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.delete('/{resource_id}')
 def delete_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_delete(
-                cursor,
-                User,
-                filter_options={
-                    'id': resource_id
-                }
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_delete(
+        cursor,
+        User,
+        filter_options={
+          'id': resource_id
+        }
+      )
+    )
 ```
 
 Done!
 
 And just like that, you've created CRUD API that exposes several endpoints for your `User` resource.
 Normally, writing the DTOs, and the duplicate models (Pydantic, ORMs, etc.) would have taken hundreds of lines of code.
 But with ModelConnect, you're given functions that auto generate this functionality for you.
@@ -350,29 +350,27 @@
 
 connect(
     User,
     ConnectOptions(
         model=Model(
             override_integrations=(
                 Psycopg2Model(
-                    tablename='users'
-                    # <- overrides the default behaviour which is snake_case from dataclass name ('user')
+                    tablename='users' # <- overrides default snake case dataclass name ('user')
                 ),
             )
         ),
-        fields=ModelFields(
+        model_fields=ModelFields(
             id=ModelField(
-                is_identifier=True,
-                # <- metadata. downstream nodes (i.e. psycopg2) use this value to determine behaviour
-                validators=(),  # <- validators
-                dtos=(),  # <- dtos
-                # integrations=(...),  # <- no overrides so integrations will attempt to infer attributes from previous options
+                is_identifier=True, # <- downstream nodes (i.e. Psycopg2ModelField) read this during resolution
+                # validators=(),  # <- validators
+                # request_dtos=RequestDtos(),  # <- request dtos if we needed them
+                # integrations=(...),  # <- no overrides - ModelField will infer
             ),
             name=ModelField(),
-            # age=ModelField(), # <- not specified so ModelFields will attempt to infer attributes from dataclass
+            # age=ModelField(), # <- not specified - ModelFields will infer
         )
     )
 )
 ```
 
 In another case,
 you may not need to override the inferred behaviour from the dataclass.
```

### Comparing `model-connect-0.0.3/README.md` & `model-connect-0.0.4/model_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Metadata-Version: 2.1
+Name: model-connect
+Version: 0.0.4
+Description-Content-Type: text/markdown
+
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
 ModelConnect goals and how it achieves them:
 
@@ -105,132 +110,132 @@
 In fact, most complex applications will use these modules to handle unique business logic.
 But what this is demonstrating is that for a simple setup (where most of the code in these layers are boilerplate),
 you can remove these modules and just use the model as the scaffolding.
 
 ```python
 from fastapi import Depends
 from model_connect.integrations.fastapi import (
-    create_router,
-    create_response_dtos,
-    create_response_dto,
-    get_from_post_request_dto,
-    get_from_post_request_dtos,
-    get_from_put_request_dto,
-    get_from_patch_request_dto,
-    get_filter_options,
-    get_pagination_options,
-    get_sort_options
+  create_router,
+  create_response_dtos,
+  create_response_dto,
+  get_from_post_request_dto,
+  get_from_post_request_dtos,
+  get_from_put_request_dto,
+  get_from_patch_request_dto,
+  get_filter_options,
+  get_pagination_options,
+  get_sort_options
 )
 from model_connect.integrations.psycopg2 import (
-    stream_select,
-    stream_insert,
-    stream_update,
-    stream_partial_update,
-    stream_delete,
+  stream_select,
+  stream_insert,
+  stream_update,
+  stream_partial_update,
+  stream_delete,
 )
 
 from src.models import User
 from src.db import open_db_connection
 
 router = create_router(User)
 
 
 @router.get('')
 def get_users(
         filter_options: dict = Depends(get_filter_options(User)),
         pagination_options: dict = Depends(get_pagination_options(User)),
         sort_options: dict = Depends(get_sort_options(User))
 ):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_select(
-                User,
-                cursor,
-                filter_options=filter_options,
-                pagination_options=pagination_options,
-                sort_options=sort_options
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_select(
+        User,
+        cursor,
+        filter_options=filter_options,
+        pagination_options=pagination_options,
+        sort_options=sort_options
+      )
+    )
 
 
 @router.get('/{resource_id}')
 def get_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_select(
-                User,
-                cursor,
-                filter_options={'id': resource_id}
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_select(
+        User,
+        cursor,
+        filter_options={'id': resource_id}
+      )
+    )
 
 
 @router.post('')
 def post_user(user: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_insert(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_insert(
+        cursor,
+        user
+      )
+    )
 
 
 @router.post('/bulk')
 def post_users(users: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_insert(
-                cursor,
-                users,
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_insert(
+        cursor,
+        users,
+      )
+    )
 
 
 @router.put('/{resource_id}')
 def put_user(user: Depends(get_from_put_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.patch('/{resource_id}')
 def patch_user(user: Depends(get_from_patch_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_partial_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_partial_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.delete('/{resource_id}')
 def delete_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_delete(
-                cursor,
-                User,
-                filter_options={
-                    'id': resource_id
-                }
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_delete(
+        cursor,
+        User,
+        filter_options={
+          'id': resource_id
+        }
+      )
+    )
 ```
 
 Done!
 
 And just like that, you've created CRUD API that exposes several endpoints for your `User` resource.
 Normally, writing the DTOs, and the duplicate models (Pydantic, ORMs, etc.) would have taken hundreds of lines of code.
 But with ModelConnect, you're given functions that auto generate this functionality for you.
@@ -345,29 +350,27 @@
 
 connect(
     User,
     ConnectOptions(
         model=Model(
             override_integrations=(
                 Psycopg2Model(
-                    tablename='users'
-                    # <- overrides the default behaviour which is snake_case from dataclass name ('user')
+                    tablename='users' # <- overrides default snake case dataclass name ('user')
                 ),
             )
         ),
-        fields=ModelFields(
+        model_fields=ModelFields(
             id=ModelField(
-                is_identifier=True,
-                # <- metadata. downstream nodes (i.e. psycopg2) use this value to determine behaviour
-                validators=(),  # <- validators
-                dtos=(),  # <- dtos
-                # integrations=(...),  # <- no overrides so integrations will attempt to infer attributes from previous options
+                is_identifier=True, # <- downstream nodes (i.e. Psycopg2ModelField) read this during resolution
+                # validators=(),  # <- validators
+                # request_dtos=RequestDtos(),  # <- request dtos if we needed them
+                # integrations=(...),  # <- no overrides - ModelField will infer
             ),
             name=ModelField(),
-            # age=ModelField(), # <- not specified so ModelFields will attempt to infer attributes from dataclass
+            # age=ModelField(), # <- not specified - ModelFields will infer
         )
     )
 )
 ```
 
 In another case,
 you may not need to override the inferred behaviour from the dataclass.
```

### Comparing `model-connect-0.0.3/model_connect/integrations/base.py` & `model-connect-0.0.4/model_connect/integrations/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, TypeVar, Generic
+from typing import TYPE_CHECKING, TypeVar
 
 if TYPE_CHECKING:
     from model_connect.options import ConnectOptions, ModelField
 
 _T = TypeVar('_T')
 
 
-class BaseIntegration:
-    model_class: type['BaseIntegrationModel'] = None
-    model_field_class: type['BaseIntegrationModelField'] = None
-
-
 @dataclass
 class BaseIntegrationModel(ABC):
     @abstractmethod
     def resolve(self, options: 'ConnectOptions'):
         ...
```

### Comparing `model-connect-0.0.3/model_connect/integrations/psycopg2/commons.py` & `model-connect-0.0.4/model_connect/integrations/psycopg2/common/streaming.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Iterator, TypeVar, Generator
 
 from psycopg2.extras import DictCursor
 
 _T = TypeVar("_T")
 
 
-def stream_results_to_model_type(results: Iterator[dict], model_class: type[_T]) -> Generator[_T, None, None]:
-    for result in results:
-        yield model_class(**result)
-
-
 def stream_from_cursor(cursor: DictCursor, max_chunk_size: int = 1000) -> Generator[dict, None, None]:
     while True:
         results = cursor.fetchmany(max_chunk_size)
 
         if not results:
             break
 
         for result in results:
             yield result
+
+
+def stream_results_to_model_type(results: Iterator[dict], model_class: type[_T]) -> Generator[_T, None, None]:
+    for result in results:
+        yield model_class(**result)
```

### Comparing `model-connect-0.0.3/model_connect/integrations/psycopg2/options/model.py` & `model-connect-0.0.4/model_connect/integrations/psycopg2/options/model.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect/integrations/psycopg2/options/model_field.py` & `model-connect-0.0.4/model_connect/integrations/psycopg2/options/model_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,18 +5,36 @@
 from model_connect.options import ConnectOptions, ModelField
 
 
 @dataclass
 class Psycopg2ModelField(BaseIntegrationModelField):
     can_filter: bool = UNDEFINED
     can_sort: bool = UNDEFINED
+    column_name: str = UNDEFINED
+    include_in_insert: bool = UNDEFINED
+    include_in_select: bool = UNDEFINED
 
     def resolve(self, options: 'ConnectOptions', model_field: 'ModelField'):
         self.can_filter = coalesce(
             self.can_filter,
             True
         )
 
         self.can_sort = coalesce(
             self.can_sort,
             True
         )
+
+        self.column_name = coalesce(
+            self.column_name,
+            model_field.name
+        )
+
+        self.include_in_insert = coalesce(
+            self.include_in_insert,
+            not model_field.is_identifier
+        )
+
+        self.include_in_select = coalesce(
+            self.include_in_select,
+            True
+        )
```

### Comparing `model-connect-0.0.3/model_connect/options/connect.py` & `model-connect-0.0.4/model_connect/options/connect.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect/options/model/model.py` & `model-connect-0.0.4/model_connect/options/model/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,12 @@
         )
 
         self.query_params.resolve(connect_options)
 
         for integration in self.override_integrations:
             self._integrations[integration.__class__] = integration
 
-        for integration_class, _ in integrations_registry.iterate():
-            model_class = integration_class.model_class
-
+        for name, (model_class, model_field_class) in integrations_registry.iterate():
             if model_class not in self._integrations:
                 self._integrations[model_class] = model_class()
 
             self._integrations[model_class].resolve(connect_options)
```

### Comparing `model-connect-0.0.3/model_connect/options/model/query_params.py` & `model-connect-0.0.4/model_connect/options/model/query_params.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect/options/model_field/model_field.py` & `model-connect-0.0.4/model_connect/options/model_field/model_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import Field, fields, dataclass, field
 from typing import TYPE_CHECKING
 
 from model_connect.constants import UNDEFINED, coalesce
 from model_connect.integrations.base import BaseIntegrationModelField, ModelFieldIntegrations
 from model_connect.integrations import registry as integrations_registry
 from model_connect.options.model.query_params import QueryParams
-from model_connect.options.model_field.model_field_dtos.request import RequestDtos
-from model_connect.options.model_field.model_field_dtos.response import ResponseDtos
+from model_connect.options.model_field.dtos.request import RequestDtos
+from model_connect.options.model_field.dtos.response import ResponseDtos
 
 if TYPE_CHECKING:
     from model_connect.options import ConnectOptions
 
 
 class ModelFields(dict[str, 'ModelField']):
     def resolve(
@@ -27,14 +27,15 @@
             self[name].resolve(options, dataclass_field)
 
 
 @dataclass
 class ModelField:
     can_sort: bool = UNDEFINED
     can_filter: bool = UNDEFINED
+    is_identifier: bool = UNDEFINED
     request_dtos: RequestDtos = UNDEFINED
     response_dtos: ResponseDtos = UNDEFINED
     query_params: tuple[str, ...] = UNDEFINED
     override_integrations: tuple['BaseIntegrationModelField', ...] = UNDEFINED
 
     _connect_options: 'ConnectOptions' = field(
         init=False
@@ -86,40 +87,38 @@
         )
 
         self.can_filter = coalesce(
             self.can_filter,
             True
         )
 
+        self.is_identifier = coalesce(
+            self.is_identifier,
+            False
+        )
+
         self.request_dtos = coalesce(
             self.request_dtos,
             RequestDtos()
         )
 
         self.response_dtos = coalesce(
             self.response_dtos,
             ResponseDtos()
         )
 
-        self.query_params = coalesce(
-            self.query_params,
-            QueryParams()
-        )
-
         self.override_integrations = coalesce(
             self.override_integrations,
             ()
         )
 
         self.request_dtos.resolve(options, dataclass_field)
         self.response_dtos.resolve(options, dataclass_field)
 
         for integration in self.override_integrations:
             self._integrations[integration.__class__] = integration
 
-        for integration_class, _ in integrations_registry.iterate():
-            model_field_class = integration_class.model_field_class
-
+        for name, (model_class, model_field_class) in integrations_registry.iterate():
             if model_field_class not in self._integrations:
                 self._integrations[model_field_class] = model_field_class()
 
             self._integrations[model_field_class].resolve(options, self)
```

### Comparing `model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/request.py` & `model-connect-0.0.4/model_connect/options/model_field/dtos/request.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect/options/model_field/model_field_dtos/response.py` & `model-connect-0.0.4/model_connect/options/model_field/dtos/response.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect/registry.py` & `model-connect-0.0.4/model_connect/registry.py`

 * *Files identical despite different names*

### Comparing `model-connect-0.0.3/model_connect.egg-info/PKG-INFO` & `model-connect-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-Metadata-Version: 2.1
-Name: model-connect
-Version: 0.0.3
-Description-Content-Type: text/markdown
-
 # ModelConnect
 
 ModelConnect is a library that enables users to connect their dataclass models with other libraries
 without writing additional boilerplate code.
 
 ModelConnect goals and how it achieves them:
 
@@ -110,132 +105,132 @@
 In fact, most complex applications will use these modules to handle unique business logic.
 But what this is demonstrating is that for a simple setup (where most of the code in these layers are boilerplate),
 you can remove these modules and just use the model as the scaffolding.
 
 ```python
 from fastapi import Depends
 from model_connect.integrations.fastapi import (
-    create_router,
-    create_response_dtos,
-    create_response_dto,
-    get_from_post_request_dto,
-    get_from_post_request_dtos,
-    get_from_put_request_dto,
-    get_from_patch_request_dto,
-    get_filter_options,
-    get_pagination_options,
-    get_sort_options
+  create_router,
+  create_response_dtos,
+  create_response_dto,
+  get_from_post_request_dto,
+  get_from_post_request_dtos,
+  get_from_put_request_dto,
+  get_from_patch_request_dto,
+  get_filter_options,
+  get_pagination_options,
+  get_sort_options
 )
 from model_connect.integrations.psycopg2 import (
-    stream_select,
-    stream_insert,
-    stream_update,
-    stream_partial_update,
-    stream_delete,
+  stream_select,
+  stream_insert,
+  stream_update,
+  stream_partial_update,
+  stream_delete,
 )
 
 from src.models import User
 from src.db import open_db_connection
 
 router = create_router(User)
 
 
 @router.get('')
 def get_users(
         filter_options: dict = Depends(get_filter_options(User)),
         pagination_options: dict = Depends(get_pagination_options(User)),
         sort_options: dict = Depends(get_sort_options(User))
 ):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_select(
-                User,
-                cursor,
-                filter_options=filter_options,
-                pagination_options=pagination_options,
-                sort_options=sort_options
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_select(
+        User,
+        cursor,
+        filter_options=filter_options,
+        pagination_options=pagination_options,
+        sort_options=sort_options
+      )
+    )
 
 
 @router.get('/{resource_id}')
 def get_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_select(
-                User,
-                cursor,
-                filter_options={'id': resource_id}
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_select(
+        User,
+        cursor,
+        filter_options={'id': resource_id}
+      )
+    )
 
 
 @router.post('')
 def post_user(user: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_insert(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_insert(
+        cursor,
+        user
+      )
+    )
 
 
 @router.post('/bulk')
 def post_users(users: Depends(get_from_post_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dtos(
-            stream_insert(
-                cursor,
-                users,
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dtos(
+      stream_insert(
+        cursor,
+        users,
+      )
+    )
 
 
 @router.put('/{resource_id}')
 def put_user(user: Depends(get_from_put_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.patch('/{resource_id}')
 def patch_user(user: Depends(get_from_patch_request_dto(User))):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_partial_update(
-                cursor,
-                user
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_partial_update(
+        cursor,
+        user
+      )
+    )
 
 
 @router.delete('/{resource_id}')
 def delete_user(resource_id: int):
-    connection = open_db_connection()
-    with connection.cursor() as cursor:
-        return create_response_dto(
-            stream_delete(
-                cursor,
-                User,
-                filter_options={
-                    'id': resource_id
-                }
-            )
-        )
+  connection = open_db_connection()
+  with connection.cursor() as cursor:
+    return create_response_dto(
+      stream_delete(
+        cursor,
+        User,
+        filter_options={
+          'id': resource_id
+        }
+      )
+    )
 ```
 
 Done!
 
 And just like that, you've created CRUD API that exposes several endpoints for your `User` resource.
 Normally, writing the DTOs, and the duplicate models (Pydantic, ORMs, etc.) would have taken hundreds of lines of code.
 But with ModelConnect, you're given functions that auto generate this functionality for you.
@@ -350,29 +345,27 @@
 
 connect(
     User,
     ConnectOptions(
         model=Model(
             override_integrations=(
                 Psycopg2Model(
-                    tablename='users'
-                    # <- overrides the default behaviour which is snake_case from dataclass name ('user')
+                    tablename='users' # <- overrides default snake case dataclass name ('user')
                 ),
             )
         ),
-        fields=ModelFields(
+        model_fields=ModelFields(
             id=ModelField(
-                is_identifier=True,
-                # <- metadata. downstream nodes (i.e. psycopg2) use this value to determine behaviour
-                validators=(),  # <- validators
-                dtos=(),  # <- dtos
-                # integrations=(...),  # <- no overrides so integrations will attempt to infer attributes from previous options
+                is_identifier=True, # <- downstream nodes (i.e. Psycopg2ModelField) read this during resolution
+                # validators=(),  # <- validators
+                # request_dtos=RequestDtos(),  # <- request dtos if we needed them
+                # integrations=(...),  # <- no overrides - ModelField will infer
             ),
             name=ModelField(),
-            # age=ModelField(), # <- not specified so ModelFields will attempt to infer attributes from dataclass
+            # age=ModelField(), # <- not specified - ModelFields will infer
         )
     )
 )
 ```
 
 In another case,
 you may not need to override the inferred behaviour from the dataclass.
```

### Comparing `model-connect-0.0.3/model_connect.egg-info/SOURCES.txt` & `model-connect-0.0.4/model_connect.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,39 @@
 model_connect/__init__.py
 model_connect/connect.py
 model_connect/constants.py
 model_connect/registry.py
 model_connect.egg-info/PKG-INFO
 model_connect.egg-info/SOURCES.txt
 model_connect.egg-info/dependency_links.txt
-model_connect.egg-info/requires.txt
 model_connect.egg-info/top_level.txt
 model_connect/integrations/__init__.py
 model_connect/integrations/base.py
-model_connect/integrations/connect.py
 model_connect/integrations/registry.py
 model_connect/integrations/fastapi/__init__.py
+model_connect/integrations/fastapi/router.py
 model_connect/integrations/fastapi/options/__init__.py
 model_connect/integrations/fastapi/options/model.py
 model_connect/integrations/fastapi/options/model_field.py
 model_connect/integrations/psycopg2/__init__.py
-model_connect/integrations/psycopg2/commons.py
 model_connect/integrations/psycopg2/delete.py
 model_connect/integrations/psycopg2/insert.py
 model_connect/integrations/psycopg2/select.py
 model_connect/integrations/psycopg2/update.py
+model_connect/integrations/psycopg2/common/__init__.py
+model_connect/integrations/psycopg2/common/processing.py
+model_connect/integrations/psycopg2/common/streaming.py
 model_connect/integrations/psycopg2/options/__init__.py
 model_connect/integrations/psycopg2/options/model.py
 model_connect/integrations/psycopg2/options/model_field.py
 model_connect/options/__init__.py
 model_connect/options/connect.py
 model_connect/options/global/__init__.py
 model_connect/options/global/global.py
 model_connect/options/model/__init__.py
 model_connect/options/model/model.py
 model_connect/options/model/query_params.py
 model_connect/options/model_field/__init__.py
 model_connect/options/model_field/model_field.py
-model_connect/options/model_field/model_field_dtos/__init__.py
-model_connect/options/model_field/model_field_dtos/request.py
-model_connect/options/model_field/model_field_dtos/response.py
+model_connect/options/model_field/dtos/__init__.py
+model_connect/options/model_field/dtos/request.py
+model_connect/options/model_field/dtos/response.py
```

### Comparing `model-connect-0.0.3/setup.py` & `model-connect-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 from setuptools import setup, find_packages
 
 long_description = Path(__name__).parent / 'README.md'
 long_description = long_description.read_text()
 
 setup(
     name='model-connect',
-    version='0.0.3',
+    version='0.0.4',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(
         include=[
             'model_connect',
             'model_connect.*'
         ],
         exclude=[
             'tests',
             'tests.*'
         ]
     ),
     install_requires=[
-        'setuptools~=60.2.0',
     ]
 )
```

