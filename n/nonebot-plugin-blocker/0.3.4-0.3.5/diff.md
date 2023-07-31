# Comparing `tmp/nonebot_plugin_blocker-0.3.4.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.4.tar", last modified: Mon Jul 31 14:32:38 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.5.tar", last modified: Mon Jul 31 17:03:29 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.4.tar` & `nonebot_plugin_blocker-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/LICENSE
--rw-r--r--   0        0        0     2969 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/README.md
--rw-r--r--   0        0        0      381 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3392 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     2785 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2422 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     2780 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6055 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-07-31 14:32:38.825409 nonebot_plugin_blocker-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     4579 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2935 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/README.md
+-rw-r--r--   0        0        0      381 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3313 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     2785 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2422 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     2780 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6055 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-07-31 17:03:29.896006 nonebot_plugin_blocker-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.5/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.4/LICENSE` & `nonebot_plugin_blocker-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/README.md` & `nonebot_plugin_blocker-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,12 +74,14 @@
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
 ### 如果你在WebUI设置了指令|回复那么指令|回复将会是你设置的文本
 
 ## TODO && 碎碎念
+ * 准备加上白名单模式
+
  * 非常感谢各位写过nonebot2插件的前辈（
- * 因为有些代码懒得自己手写拿来改改用了（（（
+
  * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
  * 什么时候用上PydanticV2啊我要用RootModel啊（
  * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -20,12 +20,12 @@
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
 ###
 å¦æä½ å¨WebUIè®¾ç½®äºæä»¤|åå¤é£ä¹æä»¤|åå¤å°ä¼æ¯ä½ è®¾ç½®çææ¬
-## TODO && ç¢ç¢å¿µ * éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
-å ä¸ºæäºä»£ç æå¾èªå·±æåæ¿æ¥æ¹æ¹ç¨äºï¼ï¼ï¼ *
+## TODO && ç¢ç¢å¿µ * åå¤å ä¸ç½ååæ¨¡å¼ *
+éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
 åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
 * ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
 ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,33 +28,28 @@
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
     
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
-    if (re.search("\[at:qq=\d+\]", event.get_plaintext()) and not event.is_tome()) or event.user_id == event.self_id:
+    if (re.search("[at:qq=\d+]", event.get_plaintext()) and not event.is_tome()) or event.user_id == event.self_id:
         return False # 如果是骰子自己发的或者当发现at了任何人但不是骰子的时候不执行
     try:
         reply_config: dict = get_reply_config().get(str(event.self_id))
+        state["this_reply"] = reply_config.get(state["blocker_state"])
         if re.match(reply_config.get("command_on")+"$", event.get_plaintext()):
             state["blocker_state"] = "reply_on"
         elif re.match(reply_config.get("command_off")+"$", event.get_plaintext()):
             state["blocker_state"] = "reply_off"
     except (AttributeError,KeyError,TypeError):
         if match := re.match("[.。]bot (on|off)\s?(|\[at:qq=\d+\])", event.get_plaintext()):
             state["blocker_state"] = "reply_"+match.group(1)
-    if "blocker_state" in state:
-        try:
-            state["this_reply"] = reply_config.get(state["blocker_state"])
-        except AttributeError:
             state["this_reply"] = reply_config_raw.get(state["blocker_state"])
-        return True
-    else:
-        return False
+    return True if "blocker_state" in state else False
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=1, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
     if blockerlist.check_blocker(event.group_id, str(event.self_id), matcher.plugin_name):
         logger.info("[Blocker]Your Message is Blocked By Blocker.")
```

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.4/pyproject.toml` & `nonebot_plugin_blocker-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.4"
+version = "0.3.5"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.4/PKG-INFO` & `nonebot_plugin_blocker-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.4
+Version: 0.3.5
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
@@ -96,12 +96,14 @@
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
 ### 如果你在WebUI设置了指令|回复那么指令|回复将会是你设置的文本
 
 ## TODO && 碎碎念
+ * 准备加上白名单模式
+
  * 非常感谢各位写过nonebot2插件的前辈（
- * 因为有些代码懒得自己手写拿来改改用了（（（
+
  * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
  * 什么时候用上PydanticV2啊我要用RootModel啊（
  * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.5 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -41,12 +41,12 @@
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
 ###
 å¦æä½ å¨WebUIè®¾ç½®äºæä»¤|åå¤é£ä¹æä»¤|åå¤å°ä¼æ¯ä½ è®¾ç½®çææ¬
-## TODO && ç¢ç¢å¿µ * éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
-å ä¸ºæäºä»£ç æå¾èªå·±æåæ¿æ¥æ¹æ¹ç¨äºï¼ï¼ï¼ *
+## TODO && ç¢ç¢å¿µ * åå¤å ä¸ç½ååæ¨¡å¼ *
+éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
 åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
 * ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
 ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

