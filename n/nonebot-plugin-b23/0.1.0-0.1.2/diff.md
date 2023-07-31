# Comparing `tmp/nonebot-plugin-b23-0.1.0.tar.gz` & `tmp/nonebot-plugin-b23-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-b23-0.1.0.tar", last modified: Tue Jun 20 05:07:08 2023, max compression
+gzip compressed data, was "nonebot-plugin-b23-0.1.2.tar", last modified: Mon Jul 31 09:03:45 2023, max compression
```

## Comparing `nonebot-plugin-b23-0.1.0.tar` & `nonebot-plugin-b23-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 05:07:08.000000 nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-20 05:07:08.121469 nonebot-plugin-b23-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-20 05:06:52.000000 nonebot-plugin-b23-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:45.551333 nonebot-plugin-b23-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 09:03:34.000000 nonebot-plugin-b23-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-31 09:03:45.551333 nonebot-plugin-b23-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:45.551333 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-31 09:03:34.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-31 09:03:34.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:03:45.551333 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-31 09:03:45.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-31 09:03:45.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:03:45.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 09:03:45.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 09:03:45.000000 nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-31 09:03:34.000000 nonebot-plugin-b23-0.1.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-31 09:03:45.551333 nonebot-plugin-b23-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-31 09:03:34.000000 nonebot-plugin-b23-0.1.2/setup.py
```

### Comparing `nonebot-plugin-b23-0.1.0/LICENSE.txt` & `nonebot-plugin-b23-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-b23-0.1.0/PKG-INFO` & `nonebot-plugin-b23-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-b23
-Version: 0.1.0
+Version: 0.1.2
 Summary: nonebot2 plugin B站热搜
 Home-page: https://github.com/eya46/nonebot_plugin_b23
 Author: eya46
 Author-email: eya46@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -13,39 +13,45 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Bilibili热搜
 
 ## 默认命令
 
-* b站热搜
 * B站热搜
 * b23
 
+## 使用
+获取B站热搜(默认20条)
+> /b23
+
+获取10条B站热搜
+> /b23 10
+
+
 ## 作用
 
 获取B站热搜
 
 ## 安装
 
 * nonebot2 2.0.0rc版本👇
 
-> pip install nonebot-plugin-b23==0.0.8
+> pip install nonebot-plugin-b23==0.0.9
 
 * nonebot2 2.0.0正式版本👇
 
-> pip install nonebot-plugin-b23==0.1.0
+> pip install nonebot-plugin-b23==0.1.2
 
 ## 配置
 
-|       名称       |       默认值       |    描述    |
-|:--------------:|:---------------:|:--------:|
-|  b23_commands  | {'b23', 'B站热搜'} |   命令名    |
-|   b23_block    |      False      | 是否阻止向下传播 |
-|  b23_priority  |       99        |   优先级    |
-| b23_max_length |       21        |  最多热搜数量  |
+|         名称          |    默认值    |           描述            |
+|:-------------------:|:---------:|:-----------------------:|
+| b23_default_command |  'B站热搜'   |          默认命令           |
+|    b23_commands     | {'b23', } |           命令名           |
+|      b23_block      |   False   |        是否阻止向下传播         |
+|    b23_priority     |    99     |           优先级           |
+|   b23_max_length    |    20     | 热搜数量(1~100)<br />推荐别设太高 |
 
 ## [依赖](requirements.txt)
 
-* httpx~=0.23.0
-* nonebot2~=2.0.0
-* pydantic~=1.10.4
+* nonebot2[httpx]>=2.0.0
```

### Comparing `nonebot-plugin-b23-0.1.0/nonebot_plugin_b23/__init__.py` & `nonebot-plugin-b23-0.1.2/nonebot_plugin_b23/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 from httpx import AsyncClient
 from nonebot import on_command, get_driver
-from nonebot.params import RawCommand
+from nonebot.internal.adapter import Message
+from nonebot.params import RawCommand, CommandArg
 from nonebot.plugin import PluginMetadata
 
 from .config import Config
 
 config = Config.parse_obj(get_driver().config)
 
 __plugin_meta__ = PluginMetadata(
     name="B站热搜",
     description="获取B站热搜(移动端)",
     usage=(
         "发送指令获取B站热搜(移动端)\n"
-        f"指令:{','.join(config.b23_commands)}"
+        f"指令:{','.join(config.b23_commands | {config.b23_default_command, })}\n"
+        f"参数(可选):热搜数量\n"
+        f"例:/{config.b23_default_command} 10\n"
     ),
     type="application",
     homepage="https://github.com/eya46/nonebot_plugin_b23",
     config=Config,
     supported_adapters=None,
 )
 
 b23_command = on_command(
-    "b站热搜",
+    config.b23_default_command,
     aliases=config.b23_commands,
     block=config.b23_block,
     priority=config.b23_priority
 )
 
 
 @b23_command.handle()
-async def b23_handler(command: str = RawCommand()):
+async def b23_handler(command: str = RawCommand(), arg: Message = CommandArg()):
+    arg = arg.extract_plain_text()
+    if arg.isdigit():
+        try:
+            arg = int(arg)
+            if arg < 1 or arg > 100:
+                raise ValueError("热搜数量必须在1-100之间")
+            limit = arg
+        except Exception as e:
+            return await b23_command.send(f"参数错误[{arg}]:{e}")
+    else:
+        limit = config.b23_max_length
     try:
         async with AsyncClient() as client:
             res = await client.get(
-                "https://app.bilibili.com/x/v2/search/trending/ranking"
+                f"https://app.bilibili.com/x/v2/search/trending/ranking?limit={limit}"
             )
             msg = f"{command}:\n"
             b23_list = res.json().get("data", {}).get("list", [])
-            for i in range(min(len(b23_list), config.b23_max_length)):
-                msg += f"{i + 1}.{b23_list[i]['show_name']}\n"
+            for index, i in enumerate(b23_list):
+                msg += f"{index + 1}.{i['show_name']}\n"
             await b23_command.send(msg.strip())
     except Exception as e:
-        await b23_command.send(f"获取B站热搜失败,error:{e}")
+        await b23_command.send(f"获取<{command}>失败,error:\n{e}")
```

### Comparing `nonebot-plugin-b23-0.1.0/nonebot_plugin_b23.egg-info/PKG-INFO` & `nonebot-plugin-b23-0.1.2/nonebot_plugin_b23.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-b23
-Version: 0.1.0
+Version: 0.1.2
 Summary: nonebot2 plugin B站热搜
 Home-page: https://github.com/eya46/nonebot_plugin_b23
 Author: eya46
 Author-email: eya46@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -13,39 +13,45 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Bilibili热搜
 
 ## 默认命令
 
-* b站热搜
 * B站热搜
 * b23
 
+## 使用
+获取B站热搜(默认20条)
+> /b23
+
+获取10条B站热搜
+> /b23 10
+
+
 ## 作用
 
 获取B站热搜
 
 ## 安装
 
 * nonebot2 2.0.0rc版本👇
 
-> pip install nonebot-plugin-b23==0.0.8
+> pip install nonebot-plugin-b23==0.0.9
 
 * nonebot2 2.0.0正式版本👇
 
-> pip install nonebot-plugin-b23==0.1.0
+> pip install nonebot-plugin-b23==0.1.2
 
 ## 配置
 
-|       名称       |       默认值       |    描述    |
-|:--------------:|:---------------:|:--------:|
-|  b23_commands  | {'b23', 'B站热搜'} |   命令名    |
-|   b23_block    |      False      | 是否阻止向下传播 |
-|  b23_priority  |       99        |   优先级    |
-| b23_max_length |       21        |  最多热搜数量  |
+|         名称          |    默认值    |           描述            |
+|:-------------------:|:---------:|:-----------------------:|
+| b23_default_command |  'B站热搜'   |          默认命令           |
+|    b23_commands     | {'b23', } |           命令名           |
+|      b23_block      |   False   |        是否阻止向下传播         |
+|    b23_priority     |    99     |           优先级           |
+|   b23_max_length    |    20     | 热搜数量(1~100)<br />推荐别设太高 |
 
 ## [依赖](requirements.txt)
 
-* httpx~=0.23.0
-* nonebot2~=2.0.0
-* pydantic~=1.10.4
+* nonebot2[httpx]>=2.0.0
```

### Comparing `nonebot-plugin-b23-0.1.0/readme.md` & `nonebot-plugin-b23-0.1.2/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,42 @@
 # Bilibili热搜
 
 ## 默认命令
 
-* b站热搜
 * B站热搜
 * b23
 
+## 使用
+获取B站热搜(默认20条)
+> /b23
+
+获取10条B站热搜
+> /b23 10
+
+
 ## 作用
 
 获取B站热搜
 
 ## 安装
 
 * nonebot2 2.0.0rc版本👇
 
-> pip install nonebot-plugin-b23==0.0.8
+> pip install nonebot-plugin-b23==0.0.9
 
 * nonebot2 2.0.0正式版本👇
 
-> pip install nonebot-plugin-b23==0.1.0
+> pip install nonebot-plugin-b23==0.1.2
 
 ## 配置
 
-|       名称       |       默认值       |    描述    |
-|:--------------:|:---------------:|:--------:|
-|  b23_commands  | {'b23', 'B站热搜'} |   命令名    |
-|   b23_block    |      False      | 是否阻止向下传播 |
-|  b23_priority  |       99        |   优先级    |
-| b23_max_length |       21        |  最多热搜数量  |
+|         名称          |    默认值    |           描述            |
+|:-------------------:|:---------:|:-----------------------:|
+| b23_default_command |  'B站热搜'   |          默认命令           |
+|    b23_commands     | {'b23', } |           命令名           |
+|      b23_block      |   False   |        是否阻止向下传播         |
+|    b23_priority     |    99     |           优先级           |
+|   b23_max_length    |    20     | 热搜数量(1~100)<br />推荐别设太高 |
 
 ## [依赖](requirements.txt)
 
-* httpx~=0.23.0
-* nonebot2~=2.0.0
-* pydantic~=1.10.4
+* nonebot2[httpx]>=2.0.0
```

