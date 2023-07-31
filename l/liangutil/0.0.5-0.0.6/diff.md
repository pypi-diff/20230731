# Comparing `tmp/liangutil-0.0.5.tar.gz` & `tmp/liangutil-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.0.5.tar", last modified: Mon Jul 31 06:59:05 2023, max compression
+gzip compressed data, was "liangutil-0.0.6.tar", last modified: Mon Jul 31 07:54:58 2023, max compression
```

## Comparing `liangutil-0.0.5.tar` & `liangutil-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.537836 liangutil-0.0.5/
--rw-rw-rw-   0        0        0     4051 2023-07-31 06:59:05.537836 liangutil-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2381 2023-07-31 03:46:04.000000 liangutil-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.534375 liangutil-0.0.5/liangutil/
--rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.5/liangutil/__init__.py
--rw-rw-rw-   0        0        0     3191 2023-07-31 02:16:24.000000 liangutil-0.0.5/liangutil/lianglog.py
--rw-rw-rw-   0        0        0     3497 2023-07-31 02:51:24.000000 liangutil-0.0.5/liangutil/liangutils.py
--rw-rw-rw-   0        0        0     2262 2023-07-31 03:31:30.000000 liangutil-0.0.5/liangutil/minioutils.py
--rw-rw-rw-   0        0        0     2621 2023-07-31 02:14:57.000000 liangutil-0.0.5/liangutil/mysqlutils.py
--rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.5/liangutil/redisutils.py
--rw-rw-rw-   0        0        0    12009 2023-07-31 02:54:53.000000 liangutil-0.0.5/liangutil/requestutils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.536839 liangutil-0.0.5/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4051 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 06:59:05.537836 liangutil-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1095 2023-07-31 06:55:06.000000 liangutil-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:54:58.687431 liangutil-0.0.6/
+-rw-rw-rw-   0        0        0     4550 2023-07-31 07:54:58.686432 liangutil-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2816 2023-07-31 07:52:58.000000 liangutil-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:54:58.677273 liangutil-0.0.6/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.6/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3191 2023-07-31 02:16:24.000000 liangutil-0.0.6/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     3493 2023-07-31 07:12:21.000000 liangutil-0.0.6/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     2262 2023-07-31 03:31:30.000000 liangutil-0.0.6/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     2621 2023-07-31 02:14:57.000000 liangutil-0.0.6/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.6/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    12009 2023-07-31 02:54:53.000000 liangutil-0.0.6/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:54:58.686432 liangutil-0.0.6/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     4550 2023-07-31 07:54:58.000000 liangutil-0.0.6/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-31 07:54:58.000000 liangutil-0.0.6/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:54:58.000000 liangutil-0.0.6/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 07:54:58.000000 liangutil-0.0.6/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:54:58.687431 liangutil-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-07-31 07:54:54.000000 liangutil-0.0.6/setup.py
```

### Comparing `liangutil-0.0.5/PKG-INFO` & `liangutil-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.5
+Version: 0.0.6
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
         
         
-        
+        ![Python](https://img.shields.io/badge/python-3.x-blue.svg)   ![PyPI](https://img.shields.io/pypi/v/liangutil)   ![PyPI - Downloads](https://img.shields.io/pypi/dd/liangutil?link=https%3A%2F%2Fpypi.org%2Fproject%2Fliangutil%2F)   ![GitHub stars](https://img.shields.io/github/stars/Will-Liang/liangutil.svg)
         
         **说明：以Liang开头的类是单独写的类，以Utils结尾的都是基于第三方库封装的。函数详细说明请看代码注释。**
         
+        **安装**
+        
+        ```
+        pip install liangutil
+        ```
+        
+        
+        
         ## liangutils
         
         函数列表：
         
         - **is_filepath(path)**：判断路径是否为文件路径
         - **get_dirpath(path)**：根据文件路径获得其父级目录路径
         - **check_path(path)**：检查路径是否存在
@@ -33,45 +41,45 @@
         
         ### RequestUtils
         
         **基于Requests库的封装**
         
         函数列表：
         
-        - get_header(self, is_choice_agent=False)：获得请求头
-        - get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)：Get请求
+        - **get_header(self, is_choice_agent=False)**：获得请求头
+        - **get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)**：Get请求
         
         
         
         ## mysqlutils
         
         ### **MySQLUtils**
         
         **基于pymysql库的封装**
         
         函数列表：
         
-        - check_table_exist(self, table_name)：根据表名检查表是否存在
-        - insert_data(self, table_name, data: dict)：向数据表插入一条记录
-        - insert_datas(self, table_name, data_list: list)：向数据表中插入多条记录
+        - **check_table_exist(self, table_name)**：根据表名检查表是否存在
+        - **insert_data(self, table_name, data: dict)**：向数据表插入一条记录
+        - **insert_datas(self, table_name, data_list: list)**：向数据表中插入多条记录
         
         
         
         ## lianglog
         
         ### LiangLog
         
         依赖于 **MySQLUtils**
         
         函数列表：
         
-        - print_log(self, level, content)：打印日志到控制台
-        - record_log_to_file(self,level, content)：将日志输出到文件
-        - record_log_to_db(self, level, content)：将日志输出到mysql数据库中
-        - record_log(self, level, content)：记录日志总方法
+        - **print_log(self, level, content)**：打印日志到控制台
+        - **record_log_to_file(self,level, content)**：将日志输出到文件
+        - **record_log_to_db(self, level, content)**：将日志输出到mysql数据库中
+        - **record_log(self, level, content)**：记录日志总方法
         
         
         
         | 字段名   | 类型    | 长度 |
         | -------- | ------- | ---- |
         | datetime | varchar | 32   |
         | level    | varchar | 32   |
@@ -84,29 +92,29 @@
         
         ### RedisUtils
         
         **基于redis库的封装**
         
         函数列表：
         
-        - enqueue_message(self, message)：向redis插入条数据
+        - **enqueue_message(self, message)**：向redis插入条数据
         
         
         
         ## minioutils
         
         ### MinIOUtils
         
         **基于minio库的封装**，依赖于 **RedisUtils**
         
         函数列表
         
-        - get_configfile(self)：读取配置文件
-        - upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)：
-        - upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)：将文件上传至MinIO，并向Redis通知
+        - **get_configfile(self)**：读取配置文件
+        - **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
+        - **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
```

### Comparing `liangutil-0.0.5/README.md` & `liangutil-0.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 # liangutil包
 
 
 
-
+![Python](https://img.shields.io/badge/python-3.x-blue.svg)   ![PyPI](https://img.shields.io/pypi/v/liangutil)   ![PyPI - Downloads](https://img.shields.io/pypi/dd/liangutil?link=https%3A%2F%2Fpypi.org%2Fproject%2Fliangutil%2F)   ![GitHub stars](https://img.shields.io/github/stars/Will-Liang/liangutil.svg)
 
 **说明：以Liang开头的类是单独写的类，以Utils结尾的都是基于第三方库封装的。函数详细说明请看代码注释。**
 
+**安装**
+
+```
+pip install liangutil
+```
+
+
+
 ## liangutils
 
 函数列表：
 
 - **is_filepath(path)**：判断路径是否为文件路径
 - **get_dirpath(path)**：根据文件路径获得其父级目录路径
 - **check_path(path)**：检查路径是否存在
@@ -25,45 +33,45 @@
 
 ### RequestUtils
 
 **基于Requests库的封装**
 
 函数列表：
 
-- get_header(self, is_choice_agent=False)：获得请求头
-- get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)：Get请求
+- **get_header(self, is_choice_agent=False)**：获得请求头
+- **get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)**：Get请求
 
 
 
 ## mysqlutils
 
 ### **MySQLUtils**
 
 **基于pymysql库的封装**
 
 函数列表：
 
-- check_table_exist(self, table_name)：根据表名检查表是否存在
-- insert_data(self, table_name, data: dict)：向数据表插入一条记录
-- insert_datas(self, table_name, data_list: list)：向数据表中插入多条记录
+- **check_table_exist(self, table_name)**：根据表名检查表是否存在
+- **insert_data(self, table_name, data: dict)**：向数据表插入一条记录
+- **insert_datas(self, table_name, data_list: list)**：向数据表中插入多条记录
 
 
 
 ## lianglog
 
 ### LiangLog
 
 依赖于 **MySQLUtils**
 
 函数列表：
 
-- print_log(self, level, content)：打印日志到控制台
-- record_log_to_file(self,level, content)：将日志输出到文件
-- record_log_to_db(self, level, content)：将日志输出到mysql数据库中
-- record_log(self, level, content)：记录日志总方法
+- **print_log(self, level, content)**：打印日志到控制台
+- **record_log_to_file(self,level, content)**：将日志输出到文件
+- **record_log_to_db(self, level, content)**：将日志输出到mysql数据库中
+- **record_log(self, level, content)**：记录日志总方法
 
 
 
 | 字段名   | 类型    | 长度 |
 | -------- | ------- | ---- |
 | datetime | varchar | 32   |
 | level    | varchar | 32   |
@@ -76,29 +84,29 @@
 
 ### RedisUtils
 
 **基于redis库的封装**
 
 函数列表：
 
-- enqueue_message(self, message)：向redis插入条数据
+- **enqueue_message(self, message)**：向redis插入条数据
 
 
 
 ## minioutils
 
 ### MinIOUtils
 
 **基于minio库的封装**，依赖于 **RedisUtils**
 
 函数列表
 
-- get_configfile(self)：读取配置文件
-- upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)：
-- upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)：将文件上传至MinIO，并向Redis通知
+- **get_configfile(self)**：读取配置文件
+- **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
+- **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
```

### Comparing `liangutil-0.0.5/liangutil/lianglog.py` & `liangutil-0.0.6/liangutil/lianglog.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.5/liangutil/liangutils.py` & `liangutil-0.0.6/liangutil/liangutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,9 +81,7 @@
 # 获得现在的日期
 # now = datetime.datetime.now(pytz.timezone('Asia/Shanghai'))
 def get_nowdate(now):
     current_date = now.strftime('%Y-%m-%d')  # 2023-04-17
     return current_date
 
 
-
-
```

### Comparing `liangutil-0.0.5/liangutil/minioutils.py` & `liangutil-0.0.6/liangutil/minioutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.5/liangutil/mysqlutils.py` & `liangutil-0.0.6/liangutil/mysqlutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.5/liangutil/requestutils.py` & `liangutil-0.0.6/liangutil/requestutils.py`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.5/liangutil.egg-info/PKG-INFO` & `liangutil-0.0.6/liangutil.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.5
+Version: 0.0.6
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
         
         
-        
+        ![Python](https://img.shields.io/badge/python-3.x-blue.svg)   ![PyPI](https://img.shields.io/pypi/v/liangutil)   ![PyPI - Downloads](https://img.shields.io/pypi/dd/liangutil?link=https%3A%2F%2Fpypi.org%2Fproject%2Fliangutil%2F)   ![GitHub stars](https://img.shields.io/github/stars/Will-Liang/liangutil.svg)
         
         **说明：以Liang开头的类是单独写的类，以Utils结尾的都是基于第三方库封装的。函数详细说明请看代码注释。**
         
+        **安装**
+        
+        ```
+        pip install liangutil
+        ```
+        
+        
+        
         ## liangutils
         
         函数列表：
         
         - **is_filepath(path)**：判断路径是否为文件路径
         - **get_dirpath(path)**：根据文件路径获得其父级目录路径
         - **check_path(path)**：检查路径是否存在
@@ -33,45 +41,45 @@
         
         ### RequestUtils
         
         **基于Requests库的封装**
         
         函数列表：
         
-        - get_header(self, is_choice_agent=False)：获得请求头
-        - get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)：Get请求
+        - **get_header(self, is_choice_agent=False)**：获得请求头
+        - **get(self, url, header="", retry_count=3, is_response_json=False, time_sleep=1, proxy=None)**：Get请求
         
         
         
         ## mysqlutils
         
         ### **MySQLUtils**
         
         **基于pymysql库的封装**
         
         函数列表：
         
-        - check_table_exist(self, table_name)：根据表名检查表是否存在
-        - insert_data(self, table_name, data: dict)：向数据表插入一条记录
-        - insert_datas(self, table_name, data_list: list)：向数据表中插入多条记录
+        - **check_table_exist(self, table_name)**：根据表名检查表是否存在
+        - **insert_data(self, table_name, data: dict)**：向数据表插入一条记录
+        - **insert_datas(self, table_name, data_list: list)**：向数据表中插入多条记录
         
         
         
         ## lianglog
         
         ### LiangLog
         
         依赖于 **MySQLUtils**
         
         函数列表：
         
-        - print_log(self, level, content)：打印日志到控制台
-        - record_log_to_file(self,level, content)：将日志输出到文件
-        - record_log_to_db(self, level, content)：将日志输出到mysql数据库中
-        - record_log(self, level, content)：记录日志总方法
+        - **print_log(self, level, content)**：打印日志到控制台
+        - **record_log_to_file(self,level, content)**：将日志输出到文件
+        - **record_log_to_db(self, level, content)**：将日志输出到mysql数据库中
+        - **record_log(self, level, content)**：记录日志总方法
         
         
         
         | 字段名   | 类型    | 长度 |
         | -------- | ------- | ---- |
         | datetime | varchar | 32   |
         | level    | varchar | 32   |
@@ -84,29 +92,29 @@
         
         ### RedisUtils
         
         **基于redis库的封装**
         
         函数列表：
         
-        - enqueue_message(self, message)：向redis插入条数据
+        - **enqueue_message(self, message)**：向redis插入条数据
         
         
         
         ## minioutils
         
         ### MinIOUtils
         
         **基于minio库的封装**，依赖于 **RedisUtils**
         
         函数列表
         
-        - get_configfile(self)：读取配置文件
-        - upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)：
-        - upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)：将文件上传至MinIO，并向Redis通知
+        - **get_configfile(self)**：读取配置文件
+        - **upload_file_to_minio(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO
+        - **upload_file_to_minio_notify(self, bucket_name: str, file_path: str, current_path: str)**：将文件上传至MinIO，并向Redis通知
```

### Comparing `liangutil-0.0.5/setup.py` & `liangutil-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
 
-    version='0.0.5',
+    version='0.0.6',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
```

