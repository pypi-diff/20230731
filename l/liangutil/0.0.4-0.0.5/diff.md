# Comparing `tmp/liangutil-0.0.4.tar.gz` & `tmp/liangutil-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.0.4.tar", last modified: Mon Jul 31 04:00:08 2023, max compression
+gzip compressed data, was "liangutil-0.0.5.tar", last modified: Mon Jul 31 06:59:05 2023, max compression
```

## Comparing `liangutil-0.0.4.tar` & `liangutil-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:00:08.216325 liangutil-0.0.4/
--rw-rw-rw-   0        0        0     4009 2023-07-31 04:00:08.216325 liangutil-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2381 2023-07-31 03:46:04.000000 liangutil-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 04:00:08.215328 liangutil-0.0.4/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4009 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 04:00:08.216325 liangutil-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1031 2023-07-31 03:58:52.000000 liangutil-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.537836 liangutil-0.0.5/
+-rw-rw-rw-   0        0        0     4051 2023-07-31 06:59:05.537836 liangutil-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2381 2023-07-31 03:46:04.000000 liangutil-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.534375 liangutil-0.0.5/liangutil/
+-rw-rw-rw-   0        0        0        0 2023-07-31 06:54:21.000000 liangutil-0.0.5/liangutil/__init__.py
+-rw-rw-rw-   0        0        0     3191 2023-07-31 02:16:24.000000 liangutil-0.0.5/liangutil/lianglog.py
+-rw-rw-rw-   0        0        0     3497 2023-07-31 02:51:24.000000 liangutil-0.0.5/liangutil/liangutils.py
+-rw-rw-rw-   0        0        0     2262 2023-07-31 03:31:30.000000 liangutil-0.0.5/liangutil/minioutils.py
+-rw-rw-rw-   0        0        0     2621 2023-07-31 02:14:57.000000 liangutil-0.0.5/liangutil/mysqlutils.py
+-rw-rw-rw-   0        0        0      447 2023-07-31 03:09:26.000000 liangutil-0.0.5/liangutil/redisutils.py
+-rw-rw-rw-   0        0        0    12009 2023-07-31 02:54:53.000000 liangutil-0.0.5/liangutil/requestutils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:59:05.536839 liangutil-0.0.5/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     4051 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      316 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 06:59:05.000000 liangutil-0.0.5/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:59:05.537836 liangutil-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1095 2023-07-31 06:55:06.000000 liangutil-0.0.5/setup.py
```

### Comparing `liangutil-0.0.4/PKG-INFO` & `liangutil-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.4
+Version: 0.0.5
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -111,14 +111,15 @@
         
         
         
         
         
         
         
+Keywords: python,utils,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Natural Language :: Chinese (Simplified)
 Requires: datetime
 Requires: os
```

### Comparing `liangutil-0.0.4/README.md` & `liangutil-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.4/liangutil.egg-info/PKG-INFO` & `liangutil-0.0.5/liangutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.4
+Version: 0.0.5
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
         
@@ -111,14 +111,15 @@
         
         
         
         
         
         
         
+Keywords: python,utils,windows,mac,linux
 Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: Natural Language :: Chinese (Simplified)
 Requires: datetime
 Requires: os
```

### Comparing `liangutil-0.0.4/setup.py` & `liangutil-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from setuptools import setup, find_packages
 with open('./README.md', encoding='utf-8') as f:
     long_description = f.read()
 setup(
+    name='liangutil',
     classifiers=[
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
-    name='liangutil',
-    version='0.0.4',
+
+    version='0.0.5',
     description='Encapsulate some common tool methods',
     author='LiAng',
     author_email='l2545721422@163.com',
     long_description=long_description,
     #README.md文本的格式，如果希望使用markdown语言就需要下面这句话
     long_description_content_type="text/markdown",
 
     requires=['datetime', 'os', 're', 'traceback', 'pytz', 'platform',
                  'random', 'time', 'requests', 'selenium', 'pymysql', 'redis',
                  'json', 'minio'],
     packages=find_packages(),
+    keywords=['python', 'utils', 'windows', 'mac', 'linux'],
 
     license="apache 3.0"
 )
```

