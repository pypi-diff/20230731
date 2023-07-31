# Comparing `tmp/testApiGroup-1.0.0.5.tar.gz` & `tmp/testApiGroup-1.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testApiGroup-1.0.0.5.tar", last modified: Mon Jul 31 06:41:35 2023, max compression
+gzip compressed data, was "testApiGroup-1.0.0.6.tar", last modified: Mon Jul 31 06:44:06 2023, max compression
```

## Comparing `testApiGroup-1.0.0.5.tar` & `testApiGroup-1.0.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.440784 testApiGroup-1.0.0.5/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:41:35.439785 testApiGroup-1.0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-31 06:41:35.440784 testApiGroup-1.0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      281 2023-07-31 06:41:34.000000 testApiGroup-1.0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.322019 testApiGroup-1.0.0.5/testApiGroup/
--rw-rw-rw-   0        0        0     1120 2023-07-31 06:41:34.000000 testApiGroup-1.0.0.5/testApiGroup/testApiGroup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 06:41:35.437786 testApiGroup-1.0.0.5/testApiGroup.egg-info/
--rw-rw-rw-   0        0        0      129 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 06:41:35.000000 testApiGroup-1.0.0.5/testApiGroup.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.551614 testApiGroup-1.0.0.6/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:44:06.542533 testApiGroup-1.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:44:06.553616 testApiGroup-1.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      281 2023-07-31 06:44:05.000000 testApiGroup-1.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.476247 testApiGroup-1.0.0.6/testApiGroup/
+-rw-rw-rw-   0        0        0     1122 2023-07-31 06:44:05.000000 testApiGroup-1.0.0.6/testApiGroup/testApiGroup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:44:06.525302 testApiGroup-1.0.0.6/testApiGroup.egg-info/
+-rw-rw-rw-   0        0        0      129 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 06:44:06.000000 testApiGroup-1.0.0.6/testApiGroup.egg-info/top_level.txt
```

### Comparing `testApiGroup-1.0.0.5/testApiGroup/testApiGroup.py` & `testApiGroup-1.0.0.6/testApiGroup/testApiGroup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import requests
 import logging
 
 
 class testApiGroup:
     def __init__(self):
         self.headers = {'Content-Type': 'application/json'}
-        self.url = http://localhost:8080
+        self.url = 'http://localhost:8080'
         logging.basicConfig(
             level=logging.DEBUG,  # 设置日志级别为DEBUG
             format='%(asctime)s - %(levelname)s - %(message)s',
             datefmt='%Y-%m-%d %H:%M:%S'
         )
 
     def 用来测试的api(self, id):
```

