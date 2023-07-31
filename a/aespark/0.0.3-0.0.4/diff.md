# Comparing `tmp/aespark-0.0.3.tar.gz` & `tmp/aespark-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aespark-0.0.3.tar", last modified: Mon Jul 31 14:18:52 2023, max compression
+gzip compressed data, was "aespark-0.0.4.tar", last modified: Mon Jul 31 14:42:48 2023, max compression
```

## Comparing `aespark-0.0.3.tar` & `aespark-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:18:52.269404 aespark-0.0.3/
--rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      731 2023-07-31 14:18:52.269404 aespark-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 14:18:52.158794 aespark-0.0.3/aespark/
--rw-rw-rw-   0        0        0    16548 2023-07-31 14:18:02.000000 aespark-0.0.3/aespark/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:18:52.269404 aespark-0.0.3/aespark/static/
--rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.3/aespark/static/ip.txt
--rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.3/aespark/static/材料模板.docx
-drwxrwxrwx   0        0        0        0 2023-07-31 14:18:52.174416 aespark-0.0.3/aespark.egg-info/
--rw-rw-rw-   0        0        0      731 2023-07-31 14:18:51.000000 aespark-0.0.3/aespark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2023-07-31 14:18:52.000000 aespark-0.0.3/aespark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:18:51.000000 aespark-0.0.3/aespark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-31 14:18:51.000000 aespark-0.0.3/aespark.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       61 2023-07-31 14:18:51.000000 aespark-0.0.3/aespark.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 14:18:51.000000 aespark-0.0.3/aespark.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 14:18:52.269404 aespark-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1554 2023-07-31 14:18:29.000000 aespark-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.853349 aespark-0.0.4/
+-rw-rw-rw-   0        0        0       89 2023-07-31 13:45:05.000000 aespark-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      731 2023-07-31 14:42:48.853349 aespark-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2023-07-31 13:30:16.000000 aespark-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.743981 aespark-0.0.4/aespark/
+-rw-rw-rw-   0        0        0    16798 2023-07-31 14:41:52.000000 aespark-0.0.4/aespark/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.853349 aespark-0.0.4/aespark/static/
+-rw-rw-rw-   0        0        0 70035392 2023-07-31 09:33:52.000000 aespark-0.0.4/aespark/static/ip.txt
+-rw-rw-rw-   0        0        0    16706 2023-07-31 09:33:52.000000 aespark-0.0.4/aespark/static/材料模板.docx
+drwxrwxrwx   0        0        0        0 2023-07-31 14:42:48.759606 aespark-0.0.4/aespark.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       61 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 14:42:48.000000 aespark-0.0.4/aespark.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       63 2023-07-31 13:18:18.000000 aespark-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:42:48.853349 aespark-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-07-31 14:42:23.000000 aespark-0.0.4/setup.py
```

### Comparing `aespark-0.0.3/PKG-INFO` & `aespark-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `aespark-0.0.3/aespark/__init__.py` & `aespark-0.0.4/aespark/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,31 @@
 import pandas as pd
 import os
 import time
 import numpy as np
 import jieba
 import warnings
 import re
+import pkg_resources
 from tqdm import tqdm
 warnings.filterwarnings('ignore')
 
 
 class MyDocument(object):
     '''
     功能简介：
         读取模板文档创建空白文档供操作
     参数解释：
         url :   可选 word模板路径
     '''
 
-    def __init__(self, url: str = r'static\材料模板.docx', drop: bool = True):
+    def __init__(self, url: str = '', drop: bool = True):
+        if url == '':
+            dist = pkg_resources.get_distribution("aespark")
+            url = f'{dist.location}\aespark\static\材料模板.docx'
         self.doc = Document(url)
         if drop:
             self.all_clean()
 
     def add_text(self, string: str = '未指定插入内容', level: int = -1):
         '''
         功能简介：
@@ -428,15 +432,17 @@
 
     return times if times else np.nan
 
 
 class IP():
 
     def __init__(self):
-        self.df = pd.read_table(r'static\ip.txt', keep_default_na='')
+        dist = pkg_resources.get_distribution("aespark")
+        self.df = pd.read_table(
+            rf'{dist.location}\aespark\static\ip.txt', keep_default_na='')
 
     def Parse_ipv4(self, ipstr: str):
         '''
         功能简介：
             ip地址解析
         return：
             一个字典，包含省、市、区、运营商、地址、原始信息
```

### Comparing `aespark-0.0.3/aespark/static/ip.txt` & `aespark-0.0.4/aespark/static/ip.txt`

 * *Files identical despite different names*

### Comparing `aespark-0.0.3/aespark/static/材料模板.docx` & `aespark-0.0.4/aespark/static/材料模板.docx`

 * *Files identical despite different names*

### Comparing `aespark-0.0.3/aespark.egg-info/PKG-INFO` & `aespark-0.0.4/aespark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aespark
-Version: 0.0.3
+Version: 0.0.4
 Summary: Generate a QR code that can adapt to the cylinder
 Home-page: https://pypi.org/project/aespark/
 Author: wtianxin
 Author-email: 1007582510@qq.com
 License: MIT
 Keywords: aespark
 Classifier: Natural Language :: Chinese (Simplified)
```

### Comparing `aespark-0.0.3/setup.py` & `aespark-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-setuptools.setup(name='aespark', version='0.0.3',
+setuptools.setup(name='aespark', version='0.0.4',
                  description='Generate a QR code that can adapt to the cylinder',
                  long_description=open(
                      'README.md', 'r', encoding='utf-8').read(),
                  author='wtianxin',
                  author_email='1007582510@qq.com',
                  url='https://pypi.org/project/aespark/',
                  license='MIT',  # 与之前你选用的许可证类型有关系
```

