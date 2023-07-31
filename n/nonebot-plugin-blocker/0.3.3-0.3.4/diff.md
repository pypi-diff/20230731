# Comparing `tmp/nonebot_plugin_blocker-0.3.3.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.3.tar", last modified: Fri Jul 28 18:33:41 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.4.tar", last modified: Mon Jul 31 14:32:38 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.3.tar` & `nonebot_plugin_blocker-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/LICENSE
--rw-r--r--   0        0        0     2538 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/README.md
--rw-r--r--   0        0        0      381 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3285 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     3994 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2383 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     2780 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6055 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-28 18:33:24.484757 nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-07-28 18:33:41.490188 nonebot_plugin_blocker-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/LICENSE
+-rw-r--r--   0        0        0     2969 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/README.md
+-rw-r--r--   0        0        0      381 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3392 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     2785 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2422 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     2780 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6055 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-07-31 14:32:21.573545 nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-07-31 14:32:38.825409 nonebot_plugin_blocker-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4579 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.3/LICENSE` & `nonebot_plugin_blocker-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.3/README.md` & `nonebot_plugin_blocker-0.3.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/MerCuJerry/nonebot-plugin-blocker.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
+<a href="https://pypi.python.org/pypi/nonebot-plugin-blocker" rel="nofollow">
+    <img alt="pypi download" src="https://img.shields.io/pypi/dm/nonebot-plugin-blocker" style="max-width: 100%;">
+</a>
 </div>
 
 ## 📖 介绍
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
 插件提供了一个简单的WebUI来让你配置Bot的开关指令以及对指令做出的回复。
@@ -36,46 +38,48 @@
 <summary>pip</summary>
 
     pip install nonebot-plugin-blocker
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot-plugin-blocker"]
+    plugins = ["nonebot_plugin_blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
-### 请注意，曾经使用过低版本本插件的请重新在WebUI里进行配置
+### 请注意，使用<0.3.1版本的更新之后请重新在WebUI里进行配置
+### >0.3.1,<0.3.3的请更新到0.3.3来自动更新配置项或者更新之后手动重新在WebUI里配置
 
 ### 常规配置项，位于.env文件里
 
 ```ini
 #WebUI的登录凭证，不设置即不进行验证
 BLOCKER_WEBUI_USERNAME=""
 BLOCKER_WEBUI_PASSWORD=""
 ```
 
 ### 其他配置项
 
-插件的回复配置文件位于 `data/blocker/reply_config.json` 里，不建议手动更改
+插件的回复配置文件位于 `data/blocker/config.json` 里，不建议手动更改
 
 `data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
-### 如果你在WebUI设置了指令那么指令将会是你设置的文本
+### 如果你在WebUI设置了指令|回复那么指令|回复将会是你设置的文本
 
 ## TODO && 碎碎念
-
+ * 非常感谢各位写过nonebot2插件的前辈（
+ * 因为有些代码懒得自己手写拿来改改用了（（（
  * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
  * 什么时候用上PydanticV2啊我要用RootModel啊（
  * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
-                                   [python]
+                           [python] [pypi_download]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
 ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
-è¯·æ³¨æï¼æ¾ç»ä½¿ç¨è¿ä½çæ¬æ¬æä»¶çè¯·éæ°å¨WebUIéè¿è¡éç½®
+["nonebot_plugin_blocker"]  ## âï¸ éç½® ###
+è¯·æ³¨æï¼ä½¿ç¨<0.3.1çæ¬çæ´æ°ä¹åè¯·éæ°å¨WebUIéè¿è¡éç½®
+###
+>0.3.1,<0.3.3çè¯·æ´æ°å°0.3.3æ¥èªå¨æ´æ°éç½®é¡¹æèæ´æ°ä¹åæå¨éæ°å¨WebUIééç½®
 ### å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini
 #WebUIçç»å½å­è¯ï¼ä¸è®¾ç½®å³ä¸è¿è¡éªè¯ BLOCKER_WEBUI_USERNAME=""
 BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
-æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
+æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/config.json`
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
-### å¦æä½ å¨WebUIè®¾ç½®äºæä»¤é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®çææ¬ ##
-TODO && ç¢ç¢å¿µ *
+###
+å¦æä½ å¨WebUIè®¾ç½®äºæä»¤|åå¤é£ä¹æä»¤|åå¤å°ä¼æ¯ä½ è®¾ç½®çææ¬
+## TODO && ç¢ç¢å¿µ * éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
+å ä¸ºæäºä»£ç æå¾èªå·±æåæ¿æ¥æ¹æ¹ç¨äºï¼ï¼ï¼ *
 åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
 * ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
 ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

### Comparing `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,71 +5,73 @@
 else:
     from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageSegment, GROUP_ADMIN, GROUP_OWNER
 
 from nonebot.permission import SUPERUSER
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.message import run_preprocessor
+from nonebot.exception import IgnoredException
 
 import re
-from .config import BlockerList, get_reply_config, upgrade_config, reply_config_raw
+from .config import BlockerList, get_reply_config, reply_config_raw
 from . import web
 
 blockerlist: BlockerList
     
 driver.server_app.mount("/blocker-webui", web.app, name="blocker-webui")
 
 @driver.on_startup
 async def load_blocker_on_start():
     global blockerlist
     blockerlist = BlockerList()
-    upgrade_config()
     logger.info("[Blocker]WebUI is now listening on "
                 f"http://{driver.config.host}:{driver.config.port}/blocker-webui/")
 
 @driver.on_shutdown
 async def save_blocker_on_shut():
     global blockerlist
     del blockerlist
     
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
-    if (event.get_plaintext().find('qq') != -1 and not event.is_tome()) or event.user_id == event.self_id:
-        return False
+    if (re.search("\[at:qq=\d+\]", event.get_plaintext()) and not event.is_tome()) or event.user_id == event.self_id:
+        return False # 如果是骰子自己发的或者当发现at了任何人但不是骰子的时候不执行
     try:
-        reply_config = get_reply_config().get(str(event.self_id))
-        if re.match(reply_config.get("command_on")+'$', event.get_plaintext()):
-            state['blocker_state'] = "reply_on"
-        elif re.match(reply_config.get("command_off")+'$', event.get_plaintext()):
-            state['blocker_state'] = "reply_off"
+        reply_config: dict = get_reply_config().get(str(event.self_id))
+        if re.match(reply_config.get("command_on")+"$", event.get_plaintext()):
+            state["blocker_state"] = "reply_on"
+        elif re.match(reply_config.get("command_off")+"$", event.get_plaintext()):
+            state["blocker_state"] = "reply_off"
     except (AttributeError,KeyError,TypeError):
-        if re.match('[.。]bot on\s?(|\[at:qq=\d+\])', event.get_plaintext()):
-            state['blocker_state'] = "reply_on"
-        elif re.match('[.。]bot off\s?(|\[at:qq=\d+\])', event.get_plaintext()):
-            state['blocker_state'] = "reply_off"
-    return True if 'blocker_state' in state else False
+        if match := re.match("[.。]bot (on|off)\s?(|\[at:qq=\d+\])", event.get_plaintext()):
+            state["blocker_state"] = "reply_"+match.group(1)
+    if "blocker_state" in state:
+        try:
+            state["this_reply"] = reply_config.get(state["blocker_state"])
+        except AttributeError:
+            state["this_reply"] = reply_config_raw.get(state["blocker_state"])
+        return True
+    else:
+        return False
     
-blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=2, block=True)
+blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=1, block=True)
 
 @run_preprocessor
 async def blocker_hook(matcher: Matcher, event: GroupMessageEvent):
-    if blockerlist.check_blocker(event.group_id, str(event.self_id)) and re.match('^nonebot_plugin_blocker$',matcher.plugin_name) is None:
-        logger.info('[Blocker]Your Message is Blocked By Blocker.')
-        matcher.handlers = None
+    if blockerlist.check_blocker(event.group_id, str(event.self_id), matcher.plugin_name):
+        logger.info("[Blocker]Your Message is Blocked By Blocker.")
+        raise IgnoredException("[Blocker]Matcher Blocked By Blocker")
         
 @blocker.handle()
 async def blocker_msg_handle(matcher: Matcher, event: GroupMessageEvent, state: T_State):
-    try:
-        reply_config = get_reply_config().get(str(event.self_id)).get(state['blocker_state'])
-    except AttributeError:
-        reply_config = reply_config_raw.get(state['blocker_state'])
-    msg_type = reply_config.get("type")
-    msg_data = reply_config.get("data")
-    if state['blocker_state'] == "reply_on":
+    assert state["this_reply"] and state["blocker_state"]
+    msg_type = state["this_reply"].get("type")
+    msg_data = state["this_reply"].get("data")
+    if state["blocker_state"] == "reply_on":
         blockerlist.del_blocker(event.group_id, str(event.self_id))
-        logger.info('[Blocker]Delete Blocker Successful.')
+        logger.info("[Blocker]Delete Blocker Successful.")
     else:
         blockerlist.add_blocker(event.group_id, str(event.self_id))
-        logger.info('[Blocker]Add Blocker Successful.')
+        logger.info("[Blocker]Add Blocker Successful.")
     if msg_type == "text":
         await matcher.finish(msg_data)
     else:
         await matcher.finish(MessageSegment(type=msg_type, data={"file":msg_data}))
```

### Comparing `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,42 +36,44 @@
     version=("nonebot-plugin-blocker")
 )
 
 app.mount("/static", StaticFiles(directory=STATIC_FILE_PATH, html=False), name="frontend")
 
 @app.get("/",response_class=HTMLResponse)
 async def show_webpage():
-    return HTMLResponse(content=MAIN_PAGE_PATH.read_text(encoding="UTF-8"), status_code=200)
+    return HTMLResponse(content=MAIN_PAGE_PATH.read_text(encoding="u8"), status_code=200)
 
 @app.post("/submit")
 async def __set_config__(form: ConfigModel):
-    save_dict = get_reply_config()
-    save_dict.update(form.dict().get("__root__"))
-    save_reply_config(ConfigModel.parse_obj(save_dict))
     try:
+        config = get_reply_config()
+        config.update(form.dict().get("__root__"))
+        save_reply_config(ConfigModel.parse_obj(config))
         return {"result":"success"}
     except:
         return {"result":"failed"}
         
 @app.get("/query_reply_list")
 async def __get_reply_list__():
     try:
-        return {"result":"success","data":list(get_reply_config().keys())}
+        config = get_reply_config()
+        return {"result":"success","data":list(config.keys())}
     except:
         return {"result":"failed"}
     
 @app.get("/query_reply")
 async def __get_reply_config__(uin: str):
     try:
-        return {"result":"success","data":get_reply_config().get(uin,"none")}
+        config = get_reply_config()
+        return {"result":"success","data":config.get(uin,"none")}
     except:
         return {"result":"failed"}
     
 @app.get("/delete")
 async def __delete_reply_config__(uin: str):
     try:
-        save_dict = get_reply_config()
-        save_dict.pop(uin)
-        save_reply_config(ConfigModel.parse_obj(save_dict))
+        config = get_reply_config()
+        config.pop(uin)
+        save_reply_config(ConfigModel.parse_obj(config))
         return {"result":"success"}
     except:
         return {"result":"failed"}
```

### Comparing `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.3/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.4/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.3/pyproject.toml` & `nonebot_plugin_blocker-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.3"
+version = "0.3.4"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.3/PKG-INFO` & `nonebot_plugin_blocker-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.3
+Version: 0.3.4
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
@@ -36,15 +36,17 @@
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/MerCuJerry/nonebot-plugin-blocker.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-blocker">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-blocker.svg" alt="pypi">
 </a>
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
-
+<a href="https://pypi.python.org/pypi/nonebot-plugin-blocker" rel="nofollow">
+    <img alt="pypi download" src="https://img.shields.io/pypi/dm/nonebot-plugin-blocker" style="max-width: 100%;">
+</a>
 </div>
 
 ## 📖 介绍
 
 这是一个 nonebot2 插件项目，用于分群配置机器人的开启关闭
 
 插件提供了一个简单的WebUI来让你配置Bot的开关指令以及对指令做出的回复。
@@ -58,46 +60,48 @@
 <summary>pip</summary>
 
     pip install nonebot-plugin-blocker
 </details>
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
 
-    plugins = ["nonebot-plugin-blocker"]
+    plugins = ["nonebot_plugin_blocker"]
 
 </details>
 
 ## ⚙️ 配置
 
-### 请注意，曾经使用过低版本本插件的请重新在WebUI里进行配置
+### 请注意，使用<0.3.1版本的更新之后请重新在WebUI里进行配置
+### >0.3.1,<0.3.3的请更新到0.3.3来自动更新配置项或者更新之后手动重新在WebUI里配置
 
 ### 常规配置项，位于.env文件里
 
 ```ini
 #WebUI的登录凭证，不设置即不进行验证
 BLOCKER_WEBUI_USERNAME=""
 BLOCKER_WEBUI_PASSWORD=""
 ```
 
 ### 其他配置项
 
-插件的回复配置文件位于 `data/blocker/reply_config.json` 里，不建议手动更改
+插件的回复配置文件位于 `data/blocker/config.json` 里，不建议手动更改
 
 `data/blocker/blocklist.json` 里是已经设置关闭Bot的群号，可以在关闭nonebot之后手动编辑
 
 ## 💬 指令
 
 指令只有管理员，群主以及Bot的SUPERUSER能够使用
 
 ### .bot on在该群开启bot
 
 ### .bot off在该群关闭bot
 
 ### 在上述指令后at特定bot将关闭使用了本插件的特定Bot，不会影响使用本插件的其他Bot
 
-### 如果你在WebUI设置了指令那么指令将会是你设置的文本
+### 如果你在WebUI设置了指令|回复那么指令|回复将会是你设置的文本
 
 ## TODO && 碎碎念
-
+ * 非常感谢各位写过nonebot2插件的前辈（
+ * 因为有些代码懒得自己手写拿来改改用了（（（
  * 准备接着改改配置项（现在就这样吧，如果nonebot有更新Pydantic的打算的话再进一步做）
  * 什么时候用上PydanticV2啊我要用RootModel啊（
  * 明明准备把代码改漂亮点的结果越写越丑，乐了
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.3 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.4 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -18,31 +18,35 @@
 DEALINGS IN THE SOFTWARE. Project-URL: Homepage, https://github.com/MerCuJerry/
 nonebot-plugin-blocker Requires-Python: <4.0,>=3.8 Requires-Dist: nonebot2
 [fastapi]>=2.0.0 Requires-Dist: nonebot-adapter-onebot>=2.1.0 Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
   # nonebot-plugin-blocker _â¨ NoneBot Plugin Blocker â¨_ [license] [pypi]
-                                   [python]
+                           [python] [pypi_download]
 ## ð ä»ç» è¿æ¯ä¸ä¸ª nonebot2
 æä»¶é¡¹ç®ï¼ç¨äºåç¾¤éç½®æºå¨äººçå¼å¯å³é­
 æä»¶æä¾äºä¸ä¸ªç®åçWebUIæ¥è®©ä½ éç½®Botçå¼å³æä»¤ä»¥åå¯¹æä»¤ååºçåå¤ã
 ## ð¿ å®è£  ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-blocker  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-["nonebot-plugin-blocker"]  ## âï¸ éç½® ###
-è¯·æ³¨æï¼æ¾ç»ä½¿ç¨è¿ä½çæ¬æ¬æä»¶çè¯·éæ°å¨WebUIéè¿è¡éç½®
+["nonebot_plugin_blocker"]  ## âï¸ éç½® ###
+è¯·æ³¨æï¼ä½¿ç¨<0.3.1çæ¬çæ´æ°ä¹åè¯·éæ°å¨WebUIéè¿è¡éç½®
+###
+>0.3.1,<0.3.3çè¯·æ´æ°å°0.3.3æ¥èªå¨æ´æ°éç½®é¡¹æèæ´æ°ä¹åæå¨éæ°å¨WebUIééç½®
 ### å¸¸è§éç½®é¡¹ï¼ä½äº.envæä»¶é ```ini
 #WebUIçç»å½å­è¯ï¼ä¸è®¾ç½®å³ä¸è¿è¡éªè¯ BLOCKER_WEBUI_USERNAME=""
 BLOCKER_WEBUI_PASSWORD="" ``` ### å¶ä»éç½®é¡¹
-æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/reply_config.json`
+æä»¶çåå¤éç½®æä»¶ä½äº `data/blocker/config.json`
 éï¼ä¸å»ºè®®æå¨æ´æ¹ `data/blocker/blocklist.json`
 éæ¯å·²ç»è®¾ç½®å³é­Botçç¾¤å·ï¼å¯ä»¥å¨å³é­nonebotä¹åæå¨ç¼è¾
 ## ð¬ æä»¤ æä»¤åªæç®¡çåï¼ç¾¤ä¸»ä»¥åBotçSUPERUSERè½å¤ä½¿ç¨
 ### .bot onå¨è¯¥ç¾¤å¼å¯bot ### .bot offå¨è¯¥ç¾¤å³é­bot ###
 å¨ä¸è¿°æä»¤åatç¹å®botå°å³é­ä½¿ç¨äºæ¬æä»¶çç¹å®Botï¼ä¸ä¼å½±åä½¿ç¨æ¬æä»¶çå¶ä»Bot
-### å¦æä½ å¨WebUIè®¾ç½®äºæä»¤é£ä¹æä»¤å°ä¼æ¯ä½ è®¾ç½®çææ¬ ##
-TODO && ç¢ç¢å¿µ *
+###
+å¦æä½ å¨WebUIè®¾ç½®äºæä»¤|åå¤é£ä¹æä»¤|åå¤å°ä¼æ¯ä½ è®¾ç½®çææ¬
+## TODO && ç¢ç¢å¿µ * éå¸¸æè°¢åä½åè¿nonebot2æä»¶çåè¾ï¼ *
+å ä¸ºæäºä»£ç æå¾èªå·±æåæ¿æ¥æ¹æ¹ç¨äºï¼ï¼ï¼ *
 åå¤æ¥çæ¹æ¹éç½®é¡¹ï¼ç°å¨å°±è¿æ ·å§ï¼å¦ænonebotææ´æ°Pydanticçæç®çè¯åè¿ä¸æ­¥åï¼
 * ä»ä¹æ¶åç¨ä¸PydanticV2åæè¦ç¨RootModelåï¼ *
 ææåå¤æä»£ç æ¹æ¼äº®ç¹çç»æè¶åè¶ä¸ï¼ä¹äº
```

