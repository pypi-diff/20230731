# Comparing `tmp/vgis_utils-1.0.9.tar.gz` & `tmp/vgis_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_utils-1.0.9.tar", last modified: Tue Jul 11 10:45:28 2023, max compression
+gzip compressed data, was "dist\vgis_utils-1.1.0.tar", last modified: Mon Jul 31 06:49:33 2023, max compression
```

## Comparing `vgis_utils-1.0.9.tar` & `vgis_utils-1.1.0.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.177571 vgis_utils-1.0.9/
--rw-rw-rw-   0        0        0     1034 2023-07-11 10:45:28.176571 vgis_utils-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 10:45:28.177571 vgis_utils-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2200 2023-07-11 10:44:52.000000 vgis_utils-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:27.992243 vgis_utils-1.0.9/vgis_utils/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/__init__.py
--rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.0.9/vgis_utils/commonTools.py
--rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.0.9/vgis_utils/iteratorTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.028210 vgis_utils-1.0.9/vgis_utils/vgis_datetime/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_datetime/__init__.py
--rw-rw-rw-   0        0        0     8245 2023-07-06 07:08:32.000000 vgis_utils-1.0.9/vgis_utils/vgis_datetime/datetimeTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.050211 vgis_utils-1.0.9/vgis_utils/vgis_file/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_file/__init__.py
--rw-rw-rw-   0        0        0     8345 2023-07-10 02:56:16.000000 vgis_utils-1.0.9/vgis_utils/vgis_file/fileTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.072210 vgis_utils-1.0.9/vgis_utils/vgis_http/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_http/__init__.py
--rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.0.9/vgis_utils/vgis_http/httpTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.093238 vgis_utils-1.0.9/vgis_utils/vgis_image/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_image/__init__.py
--rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.0.9/vgis_utils/vgis_image/imageTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.110211 vgis_utils-1.0.9/vgis_utils/vgis_list/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_list/__init__.py
--rw-rw-rw-   0        0        0     2743 2023-07-11 10:42:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_list/listTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.113211 vgis_utils-1.0.9/vgis_utils/vgis_money/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_money/__init__.py
--rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.0.9/vgis_utils/vgis_money/moneyTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.135058 vgis_utils-1.0.9/vgis_utils/vgis_string/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.0.9/vgis_utils/vgis_string/__init__.py
--rw-rw-rw-   0        0        0     3353 2023-07-07 09:32:52.000000 vgis_utils-1.0.9/vgis_utils/vgis_string/stringTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.160573 vgis_utils-1.0.9/vgis_utils/vgis_video/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.0.9/vgis_utils/vgis_video/__init__.py
--rw-rw-rw-   0        0        0    10161 2023-06-27 08:48:22.000000 vgis_utils-1.0.9/vgis_utils/vgis_video/videoTools.py
-drwxrwxrwx   0        0        0        0 2023-07-11 10:45:28.025211 vgis_utils-1.0.9/vgis_utils.egg-info/
--rw-rw-rw-   0        0        0     1034 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      827 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-11 10:45:27.000000 vgis_utils-1.0.9/vgis_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.897397 vgis_utils-1.1.0/
+-rw-rw-rw-   0        0        0     1034 2023-07-31 06:49:33.896396 vgis_utils-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      120 2023-06-27 08:16:30.000000 vgis_utils-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:49:33.897397 vgis_utils-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2200 2023-07-31 06:49:13.000000 vgis_utils-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.675397 vgis_utils-1.1.0/vgis_utils/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.1.0/vgis_utils/__init__.py
+-rw-rw-rw-   0        0        0     1423 2023-06-27 07:36:52.000000 vgis_utils-1.1.0/vgis_utils/commonTools.py
+-rw-rw-rw-   0        0        0      985 2023-06-27 06:28:07.000000 vgis_utils-1.1.0/vgis_utils/iteratorTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.722397 vgis_utils-1.1.0/vgis_utils/vgis_datetime/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.1.0/vgis_utils/vgis_datetime/__init__.py
+-rw-rw-rw-   0        0        0     8245 2023-07-06 07:08:32.000000 vgis_utils-1.1.0/vgis_utils/vgis_datetime/datetimeTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.754396 vgis_utils-1.1.0/vgis_utils/vgis_file/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.1.0/vgis_utils/vgis_file/__init__.py
+-rw-rw-rw-   0        0        0     8345 2023-07-10 02:56:16.000000 vgis_utils-1.1.0/vgis_utils/vgis_file/fileTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.769396 vgis_utils-1.1.0/vgis_utils/vgis_http/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.1.0/vgis_utils/vgis_http/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-27 06:17:10.000000 vgis_utils-1.1.0/vgis_utils/vgis_http/httpTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.786397 vgis_utils-1.1.0/vgis_utils/vgis_image/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.1.0/vgis_utils/vgis_image/__init__.py
+-rw-rw-rw-   0        0        0     4672 2023-06-27 08:29:35.000000 vgis_utils-1.1.0/vgis_utils/vgis_image/imageTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.802397 vgis_utils-1.1.0/vgis_utils/vgis_list/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.1.0/vgis_utils/vgis_list/__init__.py
+-rw-rw-rw-   0        0        0     3273 2023-07-18 07:17:57.000000 vgis_utils-1.1.0/vgis_utils/vgis_list/listTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.823428 vgis_utils-1.1.0/vgis_utils/vgis_math/
+-rw-rw-rw-   0        0        0      202 2023-07-18 07:17:57.000000 vgis_utils-1.1.0/vgis_utils/vgis_math/__init__.py
+-rw-rw-rw-   0        0        0     3429 2023-07-18 07:17:57.000000 vgis_utils-1.1.0/vgis_utils/vgis_math/mathTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.839428 vgis_utils-1.1.0/vgis_utils/vgis_money/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.1.0/vgis_utils/vgis_money/__init__.py
+-rw-rw-rw-   0        0        0    13680 2023-07-06 02:10:11.000000 vgis_utils-1.1.0/vgis_utils/vgis_money/moneyTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.877396 vgis_utils-1.1.0/vgis_utils/vgis_string/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_utils-1.1.0/vgis_utils/vgis_string/__init__.py
+-rw-rw-rw-   0        0        0     6527 2023-07-31 06:48:37.000000 vgis_utils-1.1.0/vgis_utils/vgis_string/stringTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.881395 vgis_utils-1.1.0/vgis_utils/vgis_video/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_utils-1.1.0/vgis_utils/vgis_video/__init__.py
+-rw-rw-rw-   0        0        0    10184 2023-07-24 07:44:26.000000 vgis_utils-1.1.0/vgis_utils/vgis_video/videoTools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:49:33.718396 vgis_utils-1.1.0/vgis_utils.egg-info/
+-rw-rw-rw-   0        0        0     1034 2023-07-31 06:49:33.000000 vgis_utils-1.1.0/vgis_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-07-31 06:49:33.000000 vgis_utils-1.1.0/vgis_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:49:33.000000 vgis_utils-1.1.0/vgis_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-07-31 06:49:33.000000 vgis_utils-1.1.0/vgis_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 06:49:33.000000 vgis_utils-1.1.0/vgis_utils.egg-info/top_level.txt
```

### Comparing `vgis_utils-1.0.9/PKG-INFO` & `vgis_utils-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_utils
-Version: 1.0.9
+Version: 1.1.0
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.9/setup.py` & `vgis_utils-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_utils",  # Required 项目名称
-    version="1.0.9",  # Required 发布版本号
+    version="1.1.0",  # Required 发布版本号
     description="A libary for common operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisUtils",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_utils-1.0.9/vgis_utils/commonTools.py` & `vgis_utils-1.1.0/vgis_utils/commonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/iteratorTools.py` & `vgis_utils-1.1.0/vgis_utils/iteratorTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_datetime/datetimeTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_datetime/datetimeTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_file/fileTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_file/fileTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_http/httpTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_http/httpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_image/imageTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_image/imageTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_list/listTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_list/listTools.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 # -*- coding: utf-8 -*-
 # @Time    :  2023/6/27 14:20
 # @Author  : chenxw
 # @Email   : gisfanmachel@gmail.com
 # @File    : listTools.py
 # @Descr   : 
 # @Software: PyCharm
+from operator import itemgetter
+
+
 class ListHelper:
     def __int__(self):
         pass
 
 
 
     @staticmethod
@@ -89,8 +92,22 @@
     def get_number_str_by_list(num_list):
         number_str = ""
         for num in num_list:
             number_str = number_str + str(num) + ","
         number_str = number_str.rstrip(",")
         return number_str
 
+    @staticmethod
+    # 对dict里的字典内容进行排序
+    def sort_dict_by_filed(item_list, sort_field):
+        return sorted(item_list, key=itemgetter(sort_field))
+
+    @staticmethod
+    # 判断dict字典是否有搜索对象
+    def is_has_item_in_dict(search_item_value, item_list):
+        is_find = False
+        for item_name in item_list:
+            if item_name == search_item_value:
+                is_find = True
+                break
+        return is_find
```

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_money/moneyTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_money/moneyTools.py`

 * *Files identical despite different names*

### Comparing `vgis_utils-1.0.9/vgis_utils/vgis_video/videoTools.py` & `vgis_utils-1.1.0/vgis_utils/vgis_video/videoTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import cv2  ##加载OpenCV模块
 
 
 class VideoOperator:
     def __init__(self):
         pass
 
+    # 视频转图片
     def video2frames(self, pathIn='',
                      pathOut='',
                      only_output_video_info=False,
                      extract_time_points=None,
                      initial_extract_time=0,
                      end_extract_time=None,
                      extract_time_interval=-1,
```

### Comparing `vgis_utils-1.0.9/vgis_utils.egg-info/PKG-INFO` & `vgis_utils-1.1.0/vgis_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-utils
-Version: 1.0.9
+Version: 1.1.0
 Summary: A libary for common operator
 Home-page: https://github.com/gisfanmachel/vgisUtils
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Description: ## this  is  vgis common lib
```

### Comparing `vgis_utils-1.0.9/vgis_utils.egg-info/SOURCES.txt` & `vgis_utils-1.1.0/vgis_utils.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,13 +14,15 @@
 vgis_utils/vgis_file/fileTools.py
 vgis_utils/vgis_http/__init__.py
 vgis_utils/vgis_http/httpTools.py
 vgis_utils/vgis_image/__init__.py
 vgis_utils/vgis_image/imageTools.py
 vgis_utils/vgis_list/__init__.py
 vgis_utils/vgis_list/listTools.py
+vgis_utils/vgis_math/__init__.py
+vgis_utils/vgis_math/mathTools.py
 vgis_utils/vgis_money/__init__.py
 vgis_utils/vgis_money/moneyTools.py
 vgis_utils/vgis_string/__init__.py
 vgis_utils/vgis_string/stringTools.py
 vgis_utils/vgis_video/__init__.py
 vgis_utils/vgis_video/videoTools.py
```

