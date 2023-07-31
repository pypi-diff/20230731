# Comparing `tmp/liangutil-0.0.3.tar.gz` & `tmp/liangutil-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liangutil-0.0.3.tar", last modified: Mon Jul 31 03:47:15 2023, max compression
+gzip compressed data, was "liangutil-0.0.4.tar", last modified: Mon Jul 31 04:00:08 2023, max compression
```

## Comparing `liangutil-0.0.3.tar` & `liangutil-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 03:47:15.150919 liangutil-0.0.3/
--rw-rw-rw-   0        0        0     4009 2023-07-31 03:47:15.149921 liangutil-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2381 2023-07-31 03:46:04.000000 liangutil-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 03:47:15.148925 liangutil-0.0.3/liangutil.egg-info/
--rw-rw-rw-   0        0        0     4009 2023-07-31 03:47:15.000000 liangutil-0.0.3/liangutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-07-31 03:47:15.000000 liangutil-0.0.3/liangutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 03:47:15.000000 liangutil-0.0.3/liangutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 03:47:15.000000 liangutil-0.0.3/liangutil.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 03:47:15.150919 liangutil-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1099 2023-07-31 03:47:02.000000 liangutil-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:00:08.216325 liangutil-0.0.4/
+-rw-rw-rw-   0        0        0     4009 2023-07-31 04:00:08.216325 liangutil-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2381 2023-07-31 03:46:04.000000 liangutil-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 04:00:08.215328 liangutil-0.0.4/liangutil.egg-info/
+-rw-rw-rw-   0        0        0     4009 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:00:08.000000 liangutil-0.0.4/liangutil.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:00:08.216325 liangutil-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2023-07-31 03:58:52.000000 liangutil-0.0.4/setup.py
```

### Comparing `liangutil-0.0.3/PKG-INFO` & `liangutil-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
```

### Comparing `liangutil-0.0.3/README.md` & `liangutil-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `liangutil-0.0.3/liangutil.egg-info/PKG-INFO` & `liangutil-0.0.4/liangutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liangutil
-Version: 0.0.3
+Version: 0.0.4
 Summary: Encapsulate some common tool methods
 Home-page: UNKNOWN
 Author: LiAng
 Author-email: l2545721422@163.com
 License: apache 3.0
 Description: # liangutil包
```

### Comparing `liangutil-0.0.3/setup.py` & `liangutil-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,24 +6,22 @@
         # 属于什么类型
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Programming Language :: Python :: 3.8",
         "Operating System :: Microsoft :: Windows :: Windows 11",
         "Natural Language :: Chinese (Simplified)"
     ],
     name='liangutil',
-    version='0.0.3',
+    version='0.0.4',
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
-    ext_package_data={
-        "bandwidth_report": ["*.md"]
-    },
+
     license="apache 3.0"
 )
```

