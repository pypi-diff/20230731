# Comparing `tmp/nonebot-plugin-sayoroll-0.4.3.tar.gz` & `tmp/nonebot-plugin-sayoroll-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sayoroll-0.4.3.tar", last modified: Mon Jul 31 16:41:05 2023, max compression
+gzip compressed data, was "nonebot-plugin-sayoroll-0.4.4.tar", last modified: Mon Jul 31 16:43:11 2023, max compression
```

## Comparing `nonebot-plugin-sayoroll-0.4.3.tar` & `nonebot-plugin-sayoroll-0.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:41:05.418036 nonebot-plugin-sayoroll-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-31 16:40:50.000000 nonebot-plugin-sayoroll-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-31 16:41:05.418036 nonebot-plugin-sayoroll-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-07-31 16:40:50.000000 nonebot-plugin-sayoroll-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:41:05.414036 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll/
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-31 16:40:50.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:41:05.418036 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-31 16:41:05.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-31 16:41:05.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 16:41:05.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-31 16:41:05.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-31 16:41:05.000000 nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 16:41:05.418036 nonebot-plugin-sayoroll-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-31 16:40:50.000000 nonebot-plugin-sayoroll-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:43:11.543796 nonebot-plugin-sayoroll-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-31 16:42:53.000000 nonebot-plugin-sayoroll-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-31 16:43:11.543796 nonebot-plugin-sayoroll-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3386 2023-07-31 16:42:53.000000 nonebot-plugin-sayoroll-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:43:11.539796 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll/
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-07-31 16:42:53.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 16:43:11.543796 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3858 2023-07-31 16:43:11.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-31 16:43:11.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 16:43:11.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-31 16:43:11.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-31 16:43:11.000000 nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 16:43:11.543796 nonebot-plugin-sayoroll-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-31 16:42:53.000000 nonebot-plugin-sayoroll-0.4.4/setup.py
```

### Comparing `nonebot-plugin-sayoroll-0.4.3/LICENSE` & `nonebot-plugin-sayoroll-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.4.3/PKG-INFO` & `nonebot-plugin-sayoroll-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.4.3
+Version: 0.4.4
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.4 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.4.3/README.md` & `nonebot-plugin-sayoroll-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll/__init__.py` & `nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from nonebot.adapters.onebot.v11.bot import Bot
 from nonebot.adapters.onebot.v11.event import MessageEvent
 from nonebot.adapters.onebot.v11.message import Message, MessageSegment
 
 __plugin_meta__ = PluginMetadata(
     name='sayoroll',
     type='application',
-    homepage='https://github.com/mas-alone/nonebot-plugin-sayoroll'
+    homepage='https://github.com/mas-alone/nonebot-plugin-sayoroll',
     description='随机数字或随机事件',
     usage='roll[数字] / 事件1 事件2 .../ xxx要不要xxx/ xxx还是xxx',
     config={},
     extra={}
 )
```

### Comparing `nonebot-plugin-sayoroll-0.4.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO` & `nonebot-plugin-sayoroll-0.4.4/nonebot_plugin_sayoroll.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.4.3
+Version: 0.4.4
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.4.4 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.4.3/setup.py` & `nonebot-plugin-sayoroll-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sayoroll",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.4.3",  # 程序版本
+    version="0.4.4",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="基于NoneBot的高仿以前小夜bot的roll功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

