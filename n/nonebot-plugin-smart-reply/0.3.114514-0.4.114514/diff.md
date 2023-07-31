# Comparing `tmp/nonebot_plugin_smart_reply-0.3.114514.tar.gz` & `tmp/nonebot_plugin_smart_reply-0.4.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smart_reply-0.3.114514.tar", last modified: Mon Jul 31 16:45:22 2023, max compression
+gzip compressed data, was "nonebot_plugin_smart_reply-0.4.114514.tar", last modified: Mon Jul 31 16:53:01 2023, max compression
```

## Comparing `nonebot_plugin_smart_reply-0.3.114514.tar` & `nonebot_plugin_smart_reply-0.4.114514.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.964485 nonebot_plugin_smart_reply-0.3.114514/
--rw-rw-rw-   0        0        0      325 2023-07-31 16:45:22.963486 nonebot_plugin_smart_reply-0.3.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.885199 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/
--rw-rw-rw-   0        0        0     4014 2023-07-31 16:09:18.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-07-31 16:27:47.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/config.py
--rw-rw-rw-   0        0        0     5492 2023-07-31 16:08:30.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getnewbing.py
--rw-rw-rw-   0        0        0     7175 2023-07-31 16:30:17.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getopenai.py
--rw-rw-rw-   0        0        0     8080 2023-07-31 16:42:31.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/keywordhandle.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.873538 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.950485 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/
--rw-rw-rw-   0        0        0    32921 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
--rw-rw-rw-   0        0        0   122981 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
--rw-rw-rw-   0        0        0    67013 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
--rw-rw-rw-   0        0        0    42760 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
--rw-rw-rw-   0        0        0    36232 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
--rw-rw-rw-   0        0        0    11615 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
--rw-rw-rw-   0        0        0    68879 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
--rw-rw-rw-   0        0        0    15206 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
--rw-rw-rw-   0        0        0   101527 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
--rw-rw-rw-   0        0        0   105258 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
--rw-rw-rw-   0        0        0     6491 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
--rw-rw-rw-   0        0        0    15706 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
--rw-rw-rw-   0        0        0    96863 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
--rw-rw-rw-   0        0        0    14470 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
--rw-rw-rw-   0        0        0    74476 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.961487 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/
--rw-rw-rw-   0        0        0    81951 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/data.json
--rw-rw-rw-   0        0        0     2129 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/txtToImg.py
--rw-rw-rw-   0        0        0    10841 2023-07-31 16:26:15.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.907198 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1489 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 16:45:22.964485 nonebot_plugin_smart_reply-0.3.114514/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-07-31 16:45:00.000000 nonebot_plugin_smart_reply-0.3.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.461306 nonebot_plugin_smart_reply-0.4.114514/
+-rw-rw-rw-   0        0        0      325 2023-07-31 16:53:01.460305 nonebot_plugin_smart_reply-0.4.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.427307 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/
+-rw-rw-rw-   0        0        0     4014 2023-07-31 16:51:23.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-07-31 16:27:47.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/config.py
+-rw-rw-rw-   0        0        0     5492 2023-07-31 16:08:30.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/getnewbing.py
+-rw-rw-rw-   0        0        0     7175 2023-07-31 16:30:17.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/getopenai.py
+-rw-rw-rw-   0        0        0     8194 2023-07-31 16:51:55.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/keywordhandle.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.418307 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.457306 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/
+-rw-rw-rw-   0        0        0    32921 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
+-rw-rw-rw-   0        0        0   122981 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
+-rw-rw-rw-   0        0        0    67013 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
+-rw-rw-rw-   0        0        0    42760 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
+-rw-rw-rw-   0        0        0    36232 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
+-rw-rw-rw-   0        0        0    11615 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
+-rw-rw-rw-   0        0        0    68879 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
+-rw-rw-rw-   0        0        0    15206 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
+-rw-rw-rw-   0        0        0   101527 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
+-rw-rw-rw-   0        0        0   105258 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
+-rw-rw-rw-   0        0        0     6491 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
+-rw-rw-rw-   0        0        0    15706 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
+-rw-rw-rw-   0        0        0    96863 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
+-rw-rw-rw-   0        0        0    14470 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
+-rw-rw-rw-   0        0        0    74476 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.458306 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/json/
+-rw-rw-rw-   0        0        0    81951 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/json/data.json
+-rw-rw-rw-   0        0        0     2129 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/txtToImg.py
+-rw-rw-rw-   0        0        0    10841 2023-07-31 16:26:15.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:53:01.435306 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-07-31 16:53:01.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1489 2023-07-31 16:53:01.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:53:01.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-31 16:53:01.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-31 16:53:01.000000 nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:53:01.461306 nonebot_plugin_smart_reply-0.4.114514/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-07-31 16:52:45.000000 nonebot_plugin_smart_reply-0.4.114514/setup.py
```

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/__init__.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """,
         type="application",
         homepage="https://github.com/Special-Week/nonebot_plugin_smart_reply",
         supported_adapters={"~onebot.v11"},
         extra={
             "author": "Special-Week",
             "link": "https://github.com/Special-Week/nonebot_plugin_smart_reply",
-            "version": "0.02.114514",
+            "version": "0.04.114514",
             "priority": [1, 10, 11, 55, 999],
         },
     )
 
 
 # 戳一戳响应器 优先级1, 不会向下阻断, 条件: 戳一戳bot触发
 on_notice(rule=to_me(), block=False, handlers=[key_word_module.poke_handle])
```

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/config.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getnewbing.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/getnewbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getopenai.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/getopenai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/keywordhandle.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/keywordhandle.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
                 if self.have_url(resp["content"]):
                     if bool(utils.bing_cookies) and bool(utils.openai_api_key):
                         return f'这个问题{utils.bot_nickname}暂时不知道怎么回答你呢, 试试使用"openai"/"bing"命令头调用openai或new bing吧吧'
                     if bool(utils.openai_api_key):
                         return f'这个问题{utils.bot_nickname}暂时不知道怎么回答你呢, 试试使用"openai"命令头调用openai吧'
                     if bool(utils.bing_cookies):
                         return f'这个问题{utils.bot_nickname}暂时不知道怎么回答你呢, 试试使用"bing"命令头调用new bing吧'
+                    return f"这个问题{utils.bot_nickname}暂时不知道怎么回答你呢, 换个话题吧"
                 content: str = (resp["content"]).replace("{br}", "\n")
                 maybe_master = ["dn", "林欣", "贾彦娟", "周超辉", "鑫总", "张鑫", "1938877131"]
                 maybe_nickname = ["菲菲", "小燕"]
                 su = random.choice(list(utils.superuser))
                 for i in maybe_master:
                     content = content.replace(i, su)
                 for i in maybe_nickname:
```

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/data.json` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/resource/json/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/txtToImg.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/txtToImg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/utils.py` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt` & `nonebot_plugin_smart_reply-0.4.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.3.114514/setup.py` & `nonebot_plugin_smart_reply-0.4.114514/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_smart_reply",
-    version="0.03.114514",
+    version="0.04.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="nonebot2的融合了openai, newbing, 词库的智障回复插件",
     python_requires=">=3.9.0",
     packages=find_packages(),
     long_description="reply插件",
     url="https://github.com/Special-Week/nonebot_plugin_smart_reply",
```

