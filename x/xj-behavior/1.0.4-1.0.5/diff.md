# Comparing `tmp/xj_behavior-1.0.4.tar.gz` & `tmp/xj_behavior-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj_behavior-1.0.4.tar", last modified: Thu Jul 27 01:43:02 2023, max compression
+gzip compressed data, was "dist\xj_behavior-1.0.5.tar", last modified: Mon Jul 31 02:54:42 2023, max compression
```

## Comparing `xj_behavior-1.0.4.tar` & `xj_behavior-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/
--rw-rw-rw-   0        0        0     1092 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      529 2023-07-27 01:42:51.000000 xj_behavior-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior/
--rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.4/xj_behavior/__init__.py
--rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.4/xj_behavior/admin.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior/apis/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/apis/__init__.py
--rw-rw-rw-   0        0        0      682 2023-03-28 03:17:01.000000 xj_behavior-1.0.4/xj_behavior/apis/standing_book_apis.py
--rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.4/xj_behavior/apps.py
--rw-rw-rw-   0        0        0       32 2023-03-24 00:42:51.000000 xj_behavior-1.0.4/xj_behavior/models.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior/services/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/services/__init__.py
--rw-rw-rw-   0        0        0     3832 2023-07-27 01:42:09.000000 xj_behavior-1.0.4/xj_behavior/services/standing_book_services.py
--rw-rw-rw-   0        0        0      233 2023-03-24 02:10:22.000000 xj_behavior-1.0.4/xj_behavior/urls.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior/utils/
--rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/utils/__init__.py
--rw-rw-rw-   0        0        0     1076 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1399 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/utils/custom_response.py
--rw-rw-rw-   0        0        0     7806 2022-10-31 08:53:23.000000 xj_behavior-1.0.4/xj_behavior/utils/custom_tool.py
--rw-rw-rw-   0        0        0      958 2022-10-25 06:03:08.000000 xj_behavior-1.0.4/xj_behavior/utils/j_dict.py
--rw-rw-rw-   0        0        0     8365 2022-10-17 06:55:25.000000 xj_behavior-1.0.4/xj_behavior/utils/j_recur.py
--rw-rw-rw-   0        0        0      464 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/utils/join_list.py
--rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.4/xj_behavior/utils/model_handle.py
--rw-rw-rw-   0        0        0     2682 2022-08-27 10:02:03.000000 xj_behavior-1.0.4/xj_behavior/utils/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      708 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-27 01:43:02.000000 xj_behavior-1.0.4/xj_behavior.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/
+-rw-rw-rw-   0        0        0     1092 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-03-24 00:39:21.000000 xj_behavior-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      529 2023-07-31 02:54:25.000000 xj_behavior-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior/
+-rw-rw-rw-   0        0        0        0 2023-01-12 05:45:43.000000 xj_behavior-1.0.5/xj_behavior/__init__.py
+-rw-rw-rw-   0        0        0       22 2023-03-24 00:43:30.000000 xj_behavior-1.0.5/xj_behavior/admin.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.5/xj_behavior/apis/__init__.py
+-rw-rw-rw-   0        0        0      982 2023-07-28 02:53:16.000000 xj_behavior-1.0.5/xj_behavior/apis/standing_book_apis.py
+-rw-rw-rw-   0        0        0      207 2023-03-24 00:43:09.000000 xj_behavior-1.0.5/xj_behavior/apps.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior/services/
+-rw-rw-rw-   0        0        0        0 2022-08-27 10:02:03.000000 xj_behavior-1.0.5/xj_behavior/services/__init__.py
+-rw-rw-rw-   0        0        0    13225 2023-07-31 02:47:24.000000 xj_behavior-1.0.5/xj_behavior/services/standing_book_services.py
+-rw-rw-rw-   0        0        0      307 2023-07-28 02:26:27.000000 xj_behavior-1.0.5/xj_behavior/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-28 01:18:09.000000 xj_behavior-1.0.5/xj_behavior/utils/__init__.py
+-rw-rw-rw-   0        0        0     1076 2023-07-28 01:18:09.000000 xj_behavior-1.0.5/xj_behavior/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     4628 2023-07-11 05:41:09.000000 xj_behavior-1.0.5/xj_behavior/utils/custom_response.py
+-rw-rw-rw-   0        0        0    39226 2023-07-17 06:47:39.000000 xj_behavior-1.0.5/xj_behavior/utils/custom_tool.py
+-rw-rw-rw-   0        0        0      429 2022-11-29 06:32:59.000000 xj_behavior-1.0.5/xj_behavior/utils/j_dict.py
+-rw-rw-rw-   0        0        0     8365 2023-07-28 01:18:09.000000 xj_behavior-1.0.5/xj_behavior/utils/j_recur.py
+-rw-rw-rw-   0        0        0      464 2023-07-28 01:18:09.000000 xj_behavior-1.0.5/xj_behavior/utils/join_list.py
+-rw-rw-rw-   0        0        0     7050 2022-10-27 09:44:29.000000 xj_behavior-1.0.5/xj_behavior/utils/model_handle.py
+-rw-rw-rw-   0        0        0     6182 2023-06-05 06:33:17.000000 xj_behavior-1.0.5/xj_behavior/utils/service_manager.py
+-rw-rw-rw-   0        0        0     2682 2023-07-28 01:18:09.000000 xj_behavior-1.0.5/xj_behavior/utils/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior.egg-info/
+-rw-rw-rw-   0        0        0     1092 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 02:54:42.000000 xj_behavior-1.0.5/xj_behavior.egg-info/top_level.txt
```

### Comparing `xj_behavior-1.0.4/PKG-INFO` & `xj_behavior-1.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj_behavior
-Version: 1.0.4
+Version: 1.0.5
 Summary: 行为模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj-behavior
 
 #### 介绍
```

### Comparing `xj_behavior-1.0.4/README.md` & `xj_behavior-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.4/setup.py` & `xj_behavior-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj_behavior',  # 模块名称
-    version='1.0.4',  # 模块版本
+    version='1.0.5',  # 模块版本
     description='行为模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     license="apache 3.0",
     install_requires=[]
 )
```

### Comparing `xj_behavior-1.0.4/xj_behavior/apis/standing_book_apis.py` & `xj_behavior-1.0.5/xj_behavior/apis/standing_book_apis.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 """
 @project: djangoModel->standing_book_apis
 @author: 孙楷炎
 @Email: sky4834@163.com
 @synopsis:
 @created_time: 2023/3/24 9:47
 """
+import time
+
 from rest_framework.views import APIView
 
 from ..services.standing_book_services import StandingBookServices
 from ..utils.custom_response import util_response
 from ..utils.custom_tool import request_params_wrapper
 
 
 class StandingBookApis(APIView):
     @request_params_wrapper
     def get(self, *args, request_params, **kwargs):
         data, err = StandingBookServices.standing_book(request_params)
         if err:
             return util_response(err=1000, msg=err)
         return util_response(data=data)
+
+    @request_params_wrapper
+    def standing_book_v2(self, *args, request_params, **kwargs):
+        data, err = StandingBookServices.standing_book_v2(request_params)
+        if err:
+            return util_response(err=1000, msg=err)
+        return util_response(data=data)
+
```

### Comparing `xj_behavior-1.0.4/xj_behavior/utils/custom_authorization.py` & `xj_behavior-1.0.5/xj_behavior/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.4/xj_behavior/utils/j_recur.py` & `xj_behavior-1.0.5/xj_behavior/utils/j_recur.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.4/xj_behavior/utils/model_handle.py` & `xj_behavior-1.0.5/xj_behavior/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.4/xj_behavior/utils/validator.py` & `xj_behavior-1.0.5/xj_behavior/utils/validator.py`

 * *Files identical despite different names*

### Comparing `xj_behavior-1.0.4/xj_behavior.egg-info/PKG-INFO` & `xj_behavior-1.0.5/xj_behavior.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-behavior
-Version: 1.0.4
+Version: 1.0.5
 Summary: 行为模块
 License: apache 3.0
 Description-Content-Type: text/markdown
 
 # xj-behavior
 
 #### 介绍
```

### Comparing `xj_behavior-1.0.4/xj_behavior.egg-info/SOURCES.txt` & `xj_behavior-1.0.5/xj_behavior.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 README.md
 setup.py
 xj_behavior/__init__.py
 xj_behavior/admin.py
 xj_behavior/apps.py
-xj_behavior/models.py
 xj_behavior/urls.py
 xj_behavior.egg-info/PKG-INFO
 xj_behavior.egg-info/SOURCES.txt
 xj_behavior.egg-info/dependency_links.txt
 xj_behavior.egg-info/top_level.txt
 xj_behavior/apis/__init__.py
 xj_behavior/apis/standing_book_apis.py
@@ -17,8 +16,9 @@
 xj_behavior/utils/custom_authorization.py
 xj_behavior/utils/custom_response.py
 xj_behavior/utils/custom_tool.py
 xj_behavior/utils/j_dict.py
 xj_behavior/utils/j_recur.py
 xj_behavior/utils/join_list.py
 xj_behavior/utils/model_handle.py
+xj_behavior/utils/service_manager.py
 xj_behavior/utils/validator.py
```

