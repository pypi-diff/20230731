# Comparing `tmp/dicergirl-3.0.6.tar.gz` & `tmp/dicergirl-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicergirl-3.0.6.tar", last modified: Sun Jul 30 07:01:15 2023, max compression
+gzip compressed data, was "dicergirl-3.0.7.tar", last modified: Mon Jul 31 07:36:24 2023, max compression
```

## Comparing `dicergirl-3.0.6.tar` & `dicergirl-3.0.7.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.314479 dicergirl-3.0.6/
--rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.6/LICENSE
--rw-rw-rw-   0        0        0     9351 2023-07-30 07:01:15.314479 dicergirl-3.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.283583 dicergirl-3.0.6/dicergirl/
--rw-rw-rw-   0        0        0    18998 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.301333 dicergirl-3.0.6/dicergirl/coc/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/coc/__init__.py
--rw-rw-rw-   0        0        0     4362 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/coc/coccards.py
--rw-rw-rw-   0        0        0     9147 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/coc/cocutils.py
--rw-rw-rw-   0        0        0     6020 2023-07-29 10:23:31.000000 dicergirl-3.0.6/dicergirl/coc/investigator.py
--rw-rw-rw-   0        0        0    16467 2023-07-30 06:57:07.000000 dicergirl-3.0.6/dicergirl/main.py
--rw-rw-rw-   0        0        0     3430 2023-07-30 07:00:21.000000 dicergirl-3.0.6/dicergirl/run.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.306275 dicergirl-3.0.6/dicergirl/scp/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/scp/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/agent.py
--rw-rw-rw-   0        0        0     2832 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/scpcards.py
--rw-rw-rw-   0        0        0     5191 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/scp/scputils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.313479 dicergirl-3.0.6/dicergirl/utils/
--rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/chat.py
--rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.6/dicergirl/utils/decorators.py
--rw-rw-rw-   0        0        0     7129 2023-07-30 06:42:58.000000 dicergirl-3.0.6/dicergirl/utils/dicer.py
--rw-rw-rw-   0        0        0    16252 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/handlers.py
--rw-rw-rw-   0        0        0    23148 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/messages.py
--rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.6/dicergirl/utils/settings.py
--rw-rw-rw-   0        0        0     5220 2023-07-30 07:01:05.000000 dicergirl-3.0.6/dicergirl/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-30 07:01:15.298876 dicergirl-3.0.6/dicergirl.egg-info/
--rw-rw-rw-   0        0        0     9351 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-30 07:01:15.000000 dicergirl-3.0.6/dicergirl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-30 07:01:15.315480 dicergirl-3.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1093 2023-07-30 05:42:11.000000 dicergirl-3.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.269765 dicergirl-3.0.7/
+-rw-rw-rw-   0        0        0    11558 2023-07-29 07:34:15.000000 dicergirl-3.0.7/LICENSE
+-rw-rw-rw-   0        0        0     9363 2023-07-31 07:36:24.269765 dicergirl-3.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8766 2023-07-30 06:15:15.000000 dicergirl-3.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.232723 dicergirl-3.0.7/dicergirl/
+-rw-rw-rw-   0        0        0    18920 2023-07-31 05:49:32.000000 dicergirl-3.0.7/dicergirl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/coc/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:17:05.000000 dicergirl-3.0.7/dicergirl/coc/__init__.py
+-rw-rw-rw-   0        0        0     4362 2023-07-31 05:29:50.000000 dicergirl-3.0.7/dicergirl/coc/coccards.py
+-rw-rw-rw-   0        0        0     9147 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/coc/cocutils.py
+-rw-rw-rw-   0        0        0     6020 2023-07-30 16:30:57.000000 dicergirl-3.0.7/dicergirl/coc/investigator.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/dnd/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:32.000000 dicergirl-3.0.7/dicergirl/dnd/__init__.py
+-rw-rw-rw-   0        0        0     2988 2023-07-30 16:18:46.000000 dicergirl-3.0.7/dicergirl/dnd/adventurer.py
+-rw-rw-rw-   0        0        0     2831 2023-07-30 14:43:40.000000 dicergirl-3.0.7/dicergirl/dnd/dndcards.py
+-rw-rw-rw-   0        0        0     4580 2023-07-30 14:39:09.000000 dicergirl-3.0.7/dicergirl/dnd/dndutils.py
+-rw-rw-rw-   0        0        0    17306 2023-07-31 07:23:30.000000 dicergirl-3.0.7/dicergirl/main.py
+-rw-rw-rw-   0        0        0     3439 2023-07-30 16:39:51.000000 dicergirl-3.0.7/dicergirl/run.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl/scp/
+-rw-rw-rw-   0        0        0       19 2023-07-31 06:30:31.000000 dicergirl-3.0.7/dicergirl/scp/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-07-30 16:20:07.000000 dicergirl-3.0.7/dicergirl/scp/agent.py
+-rw-rw-rw-   0        0        0     2824 2023-07-31 06:08:08.000000 dicergirl-3.0.7/dicergirl/scp/scpcards.py
+-rw-rw-rw-   0        0        0     5191 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/scp/scputils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.269238 dicergirl-3.0.7/dicergirl/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/chat.py
+-rw-rw-rw-   0        0        0     1934 2023-07-29 07:34:15.000000 dicergirl-3.0.7/dicergirl/utils/decorators.py
+-rw-rw-rw-   0        0        0     7129 2023-07-30 06:42:58.000000 dicergirl-3.0.7/dicergirl/utils/dicer.py
+-rw-rw-rw-   0        0        0    22450 2023-07-31 07:16:02.000000 dicergirl-3.0.7/dicergirl/utils/handlers.py
+-rw-rw-rw-   0        0        0    23207 2023-07-31 07:18:19.000000 dicergirl-3.0.7/dicergirl/utils/messages.py
+-rw-rw-rw-   0        0        0     1275 2023-07-30 05:42:11.000000 dicergirl-3.0.7/dicergirl/utils/settings.py
+-rw-rw-rw-   0        0        0     5839 2023-07-31 06:36:24.000000 dicergirl-3.0.7/dicergirl/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:36:24.250400 dicergirl-3.0.7/dicergirl.egg-info/
+-rw-rw-rw-   0        0        0     9363 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 07:36:24.000000 dicergirl-3.0.7/dicergirl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:36:24.269765 dicergirl-3.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-07-31 07:36:19.000000 dicergirl-3.0.7/setup.py
```

### Comparing `dicergirl-3.0.6/LICENSE` & `dicergirl-3.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/PKG-INFO` & `dicergirl-3.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.6
+Version: 3.0.7
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DicerGirl
```

### Comparing `dicergirl-3.0.6/README.md` & `dicergirl-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/__init__.py` & `dicergirl-3.0.7/dicergirl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,19 @@
 current_dir = Path(__file__).resolve().parent
 mode = "scp"
 
 try:
     driver = nonebot.get_driver()
     set_package("nonebot2")
 except ValueError:
-    utilless = True
-else:
-    utilless = False
+    set_package("qqguild")
 
 package = get_package()
 
-if package == "nonebot2" and not utilless:
+if package == "nonebot2":
     from .coc.investigator import Investigator
     from .scp.agent import Agent
     from .coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
     from .coc.coccards import cards, cache_cards, sa_handler
     from .scp.scpcards import scp_cards, scp_cache_cards
     from .scp.scputils import sra, scp_dam, at as sat
     from .utils.messages import help_message
@@ -479,12 +477,10 @@
     @versioncommand.handle()
     async def versionhandler(matcher: Matcher, event: GroupMessageEvent):
         args = format_str(event.get_message(), begin=(".version", ".v"))
         await matcher.send(f"欧若可骰娘 版本 {version}, 未知访客版权所有.\nCopyright © 2011-2023 Unknown Visitor. All Rights Reserved.")
         return
 elif package == "qqguild":
     pass
-elif package == "nonebot2":
-    pass
 else:
     logger.critical(f"未知的包模式: {package}!")
     sys.exit()
```

### Comparing `dicergirl-3.0.6/dicergirl/coc/coccards.py` & `dicergirl-3.0.7/dicergirl/coc/coccards.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/coc/cocutils.py` & `dicergirl-3.0.7/dicergirl/coc/cocutils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/coc/investigator.py` & `dicergirl-3.0.7/dicergirl/coc/investigator.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,16 +146,16 @@
 
     def __repr__(self):
         data = "姓名: %s\n" % self.name
         data += "性别: %s 年龄: %d\n" % (self.sex, self.age)
         data += "力量: %d 体质: %d 体型: %d\n" % (self.str, self.con, self.siz)
         data += "敏捷: %d 外貌: %d 智力: %d\n" % (self.dex, self.app, self.int)
         data += "意志: %d 教育: %d 幸运: %d\n" % (self.pow, self.edu, self.luc)
-        data += "DB: %d 移动速度: %d SAN: %d\n" % (self.db(), self.mov(), self.san)
-        data += "生命值: %s/%s" % (self.hp, self.lp_max())
+        data += "DB: %s 移动速度: %d SAN: %d\n" % (self.db(), self.mov(), self.san)
+        data += "生命值: %d/%d" % (self.hp, self.lp_max())
         return data
 
     def skills_output(self) -> str:
         if not self.skills:
             return "%s 当前无任何技能数据。" % self.name
         r = "%s技能数据: " % self.name
         for k, v in self.skills.items():
```

### Comparing `dicergirl-3.0.6/dicergirl/main.py` & `dicergirl-3.0.7/dicergirl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,30 @@
 from botpy.api import BotAPI
 from botpy.logging import get_logger
 from pathlib import Path
 
 from utils.settings import set_package, get_package
 set_package("qqguild")
 
-from coc.investigator import Investigator
-from scp.agent import Agent
-from coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
-from coc.coccards import cards, cache_cards, sa_handler
-from scp.scpcards import scp_cards, scp_cache_cards
-from scp.scputils import sra, scp_dam, at as sat
-from utils.decorators import Commands
-from utils.messages import help_message, version
-from utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config
-from utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, set_handler, show_handler, del_handler
-from utils.chat import chat
+from dicergirl.coc.investigator import Investigator
+from dicergirl.coc.coccards import cards, cache_cards, sa_handler
+from dicergirl.coc.cocutils import sc, st, at, dam, en, rd0, ra, ti, li, rb, rp
+
+from dicergirl.scp.agent import Agent
+from dicergirl.scp.scpcards import scp_cards, scp_cache_cards
+from dicergirl.scp.scputils import sra, scp_dam, at as sat
+
+from dicergirl.dnd.adventurer import Adventurer
+from dicergirl.dnd.dndcards import dnd_cards, dnd_cache_cards
+
+from dicergirl.utils.decorators import Commands
+from dicergirl.utils.messages import help_message, version
+from dicergirl.utils.utils import logger, init, is_super_user, add_super_user, rm_super_user, su_uuid, format_msg, format_str, get_handlers, get_config, modes
+from dicergirl.utils.handlers import scp_set_handler, scp_show_handler, scp_del_handler, coc_set_handler, coc_show_handler, coc_del_handler, dnd_set_handler, dnd_show_handler, dnd_del_handler
+from dicergirl.utils.chat import chat
 
 import botpy
 import logging
 import sys
 
 DEBUG = False
 current_dir = Path(__file__).resolve().parent
@@ -147,69 +152,113 @@
     await message.reply(content=inv.age_change(args))
 
     if 15 <= args and args < 90:
         cache_cards.update(message, inv.__dict__, save=False)
         await message.reply(content=str(inv.output()))
     return True
 
+@Commands(name=(".scp"))
+async def scp_handler(api: BotAPI, message: Message, params=None):
+    args = format_msg(message, begin=".scp")
+    if len(args) > 1:
+        logger.info("指令错误, 驳回.")
+        await message.reply(content="[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
+        return True
+
+    try:
+        if len(args) == 0:
+            raise ValueError
+        args = int(args[0])
+    except ValueError:
+        await message.reply(content=f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
+        args = 20
+
+    agt = Agent()
+    agt.age_check(args)
+    agt.init()
+    
+    if 15 <= args and args < 90:
+        scp_cache_cards.update(message, agt.__dict__, save=False)
+        await message.reply(content=str(agt.output()))
+    return True
+
+@Commands(name=(".dnd"))
+async def dnd_handler(api: BotAPI, message: Message, params=None):
+    args = format_msg(message, begin=".dnd")
+    if len(args) > 1:
+        logger.info("指令错误, 驳回.")
+        await message.reply(content="[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
+        return True
+
+    try:
+        if len(args) == 0:
+            raise ValueError
+        args = int(args[0])
+    except ValueError:
+        await message.reply(content=f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
+        args = 20
+
+    adv = Adventurer()
+    adv.age_check(args)
+    adv.init()
+    
+    if adv.int <= 8:
+        await message.reply(content="[Orcale] 很遗憾, 检定新的冒险者智力不足, 弱智是不允许成为冒险者的, 请重新进行车卡检定.")
+        return True
+
+    if 15 <= args and args < 90:
+        scp_cache_cards.update(message, adv.__dict__, save=False)
+        await message.reply(content=str(adv.output()))
+    return True
+
 @Commands(name=(".show"))
 async def showhandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=(".show", ".display"))
     if not args:
-        if mode == "scp":
-            sh = scp_show_handler(message, args)
-        elif mode == "coc":
-            sh = show_handler(message, args)
+        if mode in modes:
+            try:
+                sh = eval(f"{mode}_show_handler(message, args)")
+            except:
+                sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
         else:
             await message.reply(content="未知的跑团模式.")
             return True
 
         for msg in sh:
             await message.reply(content=str(msg))
         return True
 
-    if args[0] in ["s", "scp"]:
-        args.remove(args[0])
-        sh = scp_show_handler(message, args)
-    elif args[0] in ["c", "coc"]:
+    if args[0] in modes:
         args.remove(args[0])
-        sh = show_handler(message, args)
+        sh = eval(f"{args[0]}_show_handler(message, args)")
     else:
-        if mode == "scp":
-            sh = scp_show_handler(message, args)
-        elif mode == "coc":
-            sh = show_handler(message, args)
-        else:
-            await message.reply(content="未知的跑团模式.")
-            return True
+        try:
+            sh = eval(f"{mode}_show_handler(message, args)")
+        except:
+            sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
 
     for msg in sh:
         await message.reply(content=str(msg))
     return True
 
 @Commands(name=(".set"))
 async def sethandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=".set")
     if not args:
         args.append(mode)
 
-    if args[0] in ["s", "scp"]:
-        args.remove(args[0])
-        sh = scp_set_handler(message, args)
-    elif args[0] in ["c", "coc"]:
-        args.remove(args[0])
-        sh = set_handler(message, args)
+    if args[0] in modes:
+        try:
+            now = args[0]
+            args.remove(args[0])
+            sh = eval(f"{now}_set_handler(message, args)")
+        except:
+            sh = [f"[Oracle] 错误: 执行指令失败, 疑似该模式不存在该指令."]
     else:
-        if mode == "scp":
-            sh = scp_set_handler(message, args)
-        elif mode == "coc":
-            sh = set_handler(message, args)
-        else:
-            await message.reply(content="未知的跑团模式.")
-            return True
+        sh = [f"[Oracle] 错误: 未知的跑团模式."]
 
     await message.reply(content=sh)
     return True
 
 @Commands(name=(".help", ".h"))
 async def rdhelphandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=(".help", ".h"))
@@ -221,28 +270,24 @@
     return True
 
 @Commands(name=(".mode", ".m"))
 async def modehandler(api: BotAPI, message: Message, params=None):
     global mode
     args = format_msg(message, begin=(".mode", ".m"))
     if args:
-        if args[0] == "coc":
-            mode = "coc"
-            await message.reply(content="[Oracle] 已切换到COC跑团模式.")
-            return True
-        elif args[0] == "scp":
-            mode = "scp"
-            await message.reply(content="[Oracle] 已切换到SCP跑团模式.")
+        if args[0].lower() in modes:
+            mode = args[0].lower()
+            await message.reply(content=f"[Oracle] 已切换到 {mode.upper()} 跑团模式.")
             return True
         else:
             await message.reply(content="[Oracle] 未知的跑团模式, 忽略.")
             await message.reply(content=help_message("mode"))
             return True
     else:
-        await message.reply(content=f"[Oracle] 当前的跑团模式为 {mode}.")
+        await message.reply(content=f"[Oracle] 当前的跑团模式为 {mode.upper()}.")
     return True
 
 @Commands(name=(".st"))
 async def stcommandhandler(api: BotAPI, message: Message, params=None):
     try:
         await message.reply(content=st())
     except:
@@ -281,18 +326,21 @@
     await message.reply(content=en(args, message))
     return True
 
 
 @Commands(name=(".ra"))
 async def rahandler(api: BotAPI, message: Message, params=None):
     args = format_msg(message, begin=".ra")
-    await message.reply(content=ra(args, message))
+    if mode in ["coc", "scp", "dnd"]:
+        if mode == "scp":
+            await message.reply(content=sra(args, message))
+        elif mode == "coc":
+            await message.reply(content=ra(args, message))
     return True
 
-
 @Commands(name=(".rh"))
 async def rhhandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=".rh")
     await message.reply(content="[Oracle] 暗骰: 命运的齿轮在转动.")
     await api.post_dms(guild_id=message.guild_id, msg_id=message.id, content=rd0(args))
 
 @Commands(name=(".rha"))
@@ -353,51 +401,17 @@
 async def sahandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=".sa")
     await message.reply(content=sa_handler(message, args))
 
 @Commands(name=(".del", ".delete"))
 async def delhandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=(".del", ".delete"))
-    if mode == "coc":
-        for msg in del_handler(message, args):
+    if mode in modes:
+        for msg in eval(f"{mode}_del_handler(message, args)"):
             await message.reply(content=msg)
-    elif mode == "scp":
-        for msg in scp_del_handler(message, args):
-            await message.reply(content=msg)
-    return True
-
-@Commands(name=(".scp"))
-async def scp_handler(api: BotAPI, message: Message, params=None):
-    args = format_msg(message, begin=".scp")
-    if len(args) > 1:
-        logger.info("指令错误, 驳回.")
-        await message.reply(content="[Oracle] 错误: 参数超出预计(1需要 但 %d传入), 指令驳回." % len(args))
-        return True
-
-    try:
-        if len(args) == 0:
-            raise ValueError
-        args = int(args[0])
-    except ValueError:
-        await message.reply(content=f'警告: 参数 {args} 不合法, 使用默认值 20 替代.')
-        args = 20
-
-    agt = Agent()
-    agt.age_check(args)
-    agt.init()
-    
-    if 15 <= args and args < 90:
-        scp_cache_cards.update(message, agt.__dict__, save=False)
-        await message.reply(content=str(agt.output()))
-    return True
-
-@Commands(name=(".sra"))
-async def scp_rahandler(api: BotAPI, message: Message, params=None):
-    args = format_msg(message, begin=".sra")
-    await message.reply(content=sra(args, message))
     return True
 
 @Commands(name=(".chat"))
 async def chathandler(api: BotAPI, message: Message, params=None):
     args = format_str(message, begin=".chat")
     if not args:
         await message.reply(content="[Oracle] 空消息是不被允许的.")
```

### Comparing `dicergirl-3.0.6/dicergirl/run.py` & `dicergirl-3.0.7/dicergirl/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from watchdog.events import FileSystemEventHandler
 from multiprocessing import Process, freeze_support
 try:
     from .utils.settings import package
     from .utils.utils import version
 except ImportError:
     from dicergirl.utils.settings import package
-    from .utils.utils import version
+    from dicergirl.utils.utils import version
 
 import sys
 import runpy
 import time
 import os
 
 current_dir = Path(__file__).resolve().parent
```

### Comparing `dicergirl-3.0.6/dicergirl/scp/agent.py` & `dicergirl-3.0.7/dicergirl/scp/agent.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/scp/scpcards.py` & `dicergirl-3.0.7/dicergirl/scp/scpcards.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import json
 
 class Cards():
     def __init__(self):
         self.data = {}
 
     def save(self):
-        _log.info("[cards] 保存SCP人物卡数据.")
+        _log.info("保存 SCP 人物卡数据.")
         with open(_scp_cachepath, "w", encoding="utf-8") as f:
             json.dump(self.data, f, ensure_ascii=False)
 
     def load(self):
         with open(_scp_cachepath, "r", encoding="utf-8") as f:
             data = f.read()
             if not data:
@@ -72,8 +72,8 @@
     "灵巧": ["dex", "灵巧"],
     "健康": ["hth", "健康"],
     "命运": ["fte", "命运"],
     "魅力": ["chr", "魅力"],
     "情报": ["int", "情报"],
     "意志": ["wil", "意志", "精神"],
     "生命": ["hp", "生命"]
-}
+}
```

### Comparing `dicergirl-3.0.6/dicergirl/scp/scputils.py` & `dicergirl-3.0.7/dicergirl/scp/scputils.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/utils/chat.py` & `dicergirl-3.0.7/dicergirl/utils/chat.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/utils/decorators.py` & `dicergirl-3.0.7/dicergirl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/utils/dicer.py` & `dicergirl-3.0.7/dicergirl/utils/dicer.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/utils/handlers.py` & `dicergirl-3.0.7/dicergirl/utils/handlers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,38 @@
+from loguru import logger
 try:
     from ..utils.utils import _coc_cachepath, _scp_cachepath, logger as _log, get_group_id
     from ..utils.dicer import Dice, expr
     from ..utils.messages import help_messages
     from ..coc.investigator import Investigator
     from ..coc.coccards import cache_cards, cards, attrs_dict
     from ..scp.agent import Agent
     from ..scp.scpcards import scp_cache_cards, scp_cards, scp_attrs_dict
+    from ..dnd.adventurer import Adventurer
+    from ..dnd.dndcards import dnd_cache_cards, dnd_cards, dnd_attrs_dict
 except ImportError:
     from dicergirl.utils.utils import _coc_cachepath, _scp_cachepath, logger as _log, get_group_id
     from dicergirl.utils.dicer import Dice, expr
     from dicergirl.utils.messages import help_messages
     from dicergirl.coc.investigator import Investigator
     from dicergirl.coc.coccards import cache_cards, cards, attrs_dict
     from dicergirl.scp.agent import Agent
     from dicergirl.scp.scpcards import scp_cache_cards, scp_cards, scp_attrs_dict
+    from dicergirl.dnd.adventurer import Adventurer
+    from dicergirl.dnd.dndcards import dnd_cache_cards, dnd_cards, dnd_attrs_dict
 
-def set_handler(message, args):
+def coc_set_handler(message, args):
     if not args:
         if cache_cards.get(message):
             card_data = cache_cards.get(message)
             cards.update(message, inv_dict=card_data)
             inv = Investigator().load(card_data)
             return "[Oracle] 成功从缓存保存人物卡属性: \n" + inv.output()
         else:
-            return "[Oracle] 未找到缓存数据, 请先使用coc指令进行车卡生成角色卡."
+            return "[Oracle] 未找到缓存数据, 请先使用`.coc`指令进行车卡生成角色卡."
     else:
         if cards.get(message):
             card_data = cards.get(message)
             inv = Investigator().load(card_data)
         else:
             return "[Oracle] 未找到已保存数据, 请先使用空白set指令保存角色数据."
         if len(args) % 2 != 0:
@@ -94,16 +99,15 @@
             rep = "[Oracle]\n"
             for r in reply:
                 rep += r + "\n"
             return rep.rstrip("\n")
         else:
             return "[Oracle] 参数错误, 可能是由于传输的数据数量错误, 此外, 这看起来不像是来源于我的错误."
 
-
-def show_handler(message, args):
+def coc_show_handler(message, args):
     r = []
     if not args:
         if cards.get(message):
             card_data = cards.get(message)
             inv = Investigator().load(card_data)
             data = "[Oracle] 使用中人物卡: \n" 
             data += inv.output() + "\n"
@@ -127,15 +131,15 @@
             r.append(d)
     else:
         r.append("[Oracle] 参数异常.")
     if not r:
         r.append("[Oracle] 未查询到保存或暂存信息.")
     return r
 
-def del_handler(message, args: str):
+def coc_del_handler(message, args: str):
     r = []
     args = args.split(" ")
     if args:
         args = list(filter(None, args))
     else:
         args = None
     for arg in args:
@@ -306,40 +310,153 @@
         else:
             if scp_cards.delete_skill(message, arg):
                 r.append(f"已删除技能 {arg}.")
     if not r:
         r.append(help_messages.del_)
     return r
 
-def sa_handler(message, args: str):
+def dnd_set_handler(message, args):
+    if not args:
+        if dnd_cache_cards.get(message):
+            card_data = dnd_cache_cards.get(message)
+            dnd_cards.update(message, inv_dict=card_data)
+            inv = Agent().load(card_data)
+            return "[Oracle] 成功从缓存保存人物卡属性: \n" + inv.output()
+        else:
+            return "[Oracle] 未找到缓存数据, 请先使用`.dnd`指令进行车卡生成角色卡."
+    else:
+        if dnd_cards.get(message):
+            card_data = dnd_cards.get(message)
+            inv = Agent().load(card_data)
+        else:
+            return "[Oracle] 未找到已保存数据, 请先使用空白`.set`指令保存角色数据."
+        if len(args) % 2 != 0:
+            return "[Oracle] 参数错误, 这是由于传输的数据数量错误, 我只接受为偶数的参数数量, 因为我无法连接到OpenAI, 这使得我无法使用 GPT-4 作为神经网络引擎, 我使用 TensorFlow 作为替代.\n此外, 这看起来不像是来源于我的错误."
+        elif len(args) == 2:
+            for attr, alias in scp_attrs_dict.items():
+                if args[0] in alias:
+                    if attr in ["名字", "性别"]:
+                        if attr == "性别" and not args[1] in ["男", "女"]:
+                            return "[Oracle] 欧若可拒绝将基金会特工性别将设置为 {sex}, 这是对物种的侮辱.".format(sex=args[1])
+                        inv.__dict__[alias[0]] = args[1]
+                    else:
+                        try:
+                            inv.__dict__[alias[0]] = int(args[1])
+                        except ValueError:
+                            return "[Oracle] 请输入正整数属性数据"
+                    dnd_cards.update(message, inv.__dict__)
+                    return "[Oracle] 设置基金会特工 %s 为: %s" % (attr, args[1])
+            try:
+                inv.skills[args[0]] = int(args[1])
+                dnd_cards.update(message, inv.__dict__)
+                return "[Oracle] 设置基金会特工 %s 技能为: %s." % (args[0], args[1])
+            except ValueError:
+                return "[Oracle] 请输入正整数技能数据."
+        elif len(args) > 2:
+            reply = []
+            li = []
+            sub_li = []
+            for arg in args:
+                index = args.index(arg)
+                if index % 2 == 0:
+                    sub_li.append(arg)
+                elif index % 2 == 1:
+                    sub_li.append(arg)
+                    li.append(sub_li)
+                    sub_li = []
+                else:
+                    return "[Oracle] 参数错误, 可能是 Python 解释器的错误, 请检查该服务的 Python 版本, 我无法解析到我当前承载的服务器状态, 因为开发者并未给我提供 API 接口.\n此外, 这看起来不像是来源于我的错误."
+            for sub_li in li:
+                has_set = False
+                for attr, alias in scp_attrs_dict.items():
+                    if sub_li[0] in alias:
+                        if attr in ["名字", "性别"]:
+                            if attr == "性别" and not sub_li[1] in ["男", "女"]:
+                                return "[Oracle] 欧若可拒绝将基金会特工性别将设置为 {sex}, 这是对物种的侮辱.".format(sex=sub_li[1])
+                            inv.__dict__[alias[0]] = sub_li[1]
+                        else:
+                            try:
+                                inv.__dict__[alias[0]] = int(sub_li[1])
+                            except ValueError:
+                                reply.append("基础数据 %s 要求正整数数据, 但你传入了 %s." % (sub_li[0], sub_li[1]))
+                                continue
+                        dnd_cards.update(message, inv.__dict__)
+                        reply.append("设置基金会特工基础数据 %s 为: %s" % (attr, sub_li[1]))
+                        has_set = True
+                if has_set:
+                    continue
+                try:
+                    inv.skills[sub_li[0]] = int(sub_li[1])
+                    dnd_cards.update(message, inv.__dict__)
+                    reply.append("设置基金会特工 %s 技能为: %s." % (sub_li[0], sub_li[1]))
+                except ValueError:
+                    reply.append("技能 %s 要求正整数数据, 但你传入了 %s." % (sub_li[0], sub_li[1]))
+            rep = "[Oracle]\n"
+            for r in reply:
+                rep += r + "\n"
+            return rep.rstrip("\n")
+        else:
+            return "[Oracle] 参数错误, 可能是由于传输的数据数量错误, 此外, 这看起来不像是来源于我的错误."
+
+def dnd_show_handler(message, args):
+    r = []
+    if not args:
+        if dnd_cards.get(message):
+            card_data = dnd_cards.get(message)
+            inv = Agent().load(card_data)
+            data = "[Oracle] 使用中人物卡: \n" 
+            data += inv.output() + "\n"
+            data += inv.skills_output()
+            r.append(data)
+        if dnd_cache_cards.get(message):
+            card_data = dnd_cache_cards.get(message)
+            inv = Agent().load(card_data)
+            r.append("[Oracle] 已暂存人物卡: \n" + inv.output())
+    elif args[0] in ["skill", "s", "skills"]:
+        if dnd_cards.get(message):
+            card_data = dnd_cards.get(message)
+            inv = Agent().load(card_data)
+            r.append(inv.skills_output())
+    elif args[0] == "all":
+        cd = dnd_cards.data[get_group_id(message)]
+        for data in cd:
+            inv = Agent().load(cd[data])
+            d = inv.output() + "\n"
+            d += inv.skills_output()
+            r.append(d)
+    else:
+        r.append("[Oracle] 参数异常.")
+    if not r:
+        r.append("[Oracle] 未查询到保存或暂存信息.")
+    return r
+
+def dnd_del_handler(message, args: str):
+    r = []
     args = args.split(" ")
-    args = list(filter(None, args))
     if args:
-        args = args[0]
+        args = list(filter(None, args))
     else:
         args = None
-    if not args:
-        return help_messages.sa
-    elif not scp_cards.get(message):
-        return "[Oracle] 请先使用`.set`指令保存人物卡后再使用快速检定功能."
-    for attr, alias in attrs_dict.items():
-        if args in alias:
-            arg = alias[0]
-            break
-        else:
-            arg = None
-    if not arg:
-        return f"[Oracle] 错误: 目标参数不在 {attrs_dict} 之内."
-    card_data = scp_cards.get(message)
-    dices = Dice()
-    try:
-        data = card_data[arg]
-        if arg != "名字":
-            val = int(data)
-        else:
-            val = None
-    except KeyError:
-        return f"[Oracle] 致命错误: 存储的数据 {data} 转化为数字的时候出现错误."
-    if not isinstance(val, int):
-        return f"[Oracle] 错误: 参数 {arg} 不可以进行快速检定, 即便它在合法指令中, 因为它没有数值.\n\
-            如果你确信这是一个错误, 请尝试重新车卡或联系管理员."
-    return expr(dices, val)
+    for arg in args:
+        if not arg:
+            pass
+        elif arg == "c":
+            if dnd_cache_cards.get(message):
+                if dnd_cache_cards.delete(message, save=False):
+                    r.append("[Oracle] 已清空暂存人物卡数据.")
+                else:
+                    r.append("[Oracle] 错误: 未知错误.")
+            r.append("[Oracle] 暂无缓存人物卡数据.")
+        elif arg == "card":
+            if dnd_cards.get(message):
+                if dnd_cards.delete(message):
+                    r.append("[Oracle] 已删除使用中的人物卡！")
+                else:
+                    r.append("[Oracle] 错误: 未知错误.")
+            else:
+                r.append("[Oracle] 暂无使用中的人物卡.")
+        else:
+            if dnd_cards.delete_skill(message, arg):
+                r.append(f"已删除技能 {arg}.")
+    if not r:
+        r.append(help_messages.del_)
+    return r
```

### Comparing `dicergirl-3.0.6/dicergirl/utils/messages.py` & `dicergirl-3.0.7/dicergirl/utils/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,23 +2,24 @@
     from .utils import version
 except ImportError:
     from dicergirl.utils.utils import version
 
 class Help_Messages():
     def __init__(self):
         self.main = f"""欧若可骰娘 Version {version}
-此骰娘基于腾讯QQ机器人(botpy)搭建, \
+此骰娘基于腾讯 QQ频道(qq-botpy)及 Nonebot2 搭建, \
 由欧若可(Oracle)提供部分算法支持.
 最终版本由未知访客团队(Unknow Visitor, 原左旋联盟)完成.
 感谢 灵冬-老孙 提供相关技术支持.
 
 .help 帮助信息
 .su   进行超级管理员鉴权
 .coc  进行车卡, 完成 COC 角色作成
 .scp  进行车卡, 完成 SCP 角色作成
+.dnd  进行车卡, 完成 DND 角色作成
 .mode 切换当前跑团模式
 .r    投掷指令 例如:
             .r 10 100 (10D100)
             .r 10d100 (10D100)
         d   制定骰子面数
         a   检定
             .ra [str: 数据名] 例如:
```

### Comparing `dicergirl-3.0.6/dicergirl/utils/settings.py` & `dicergirl-3.0.7/dicergirl/utils/settings.py`

 * *Files identical despite different names*

### Comparing `dicergirl-3.0.6/dicergirl/utils/utils.py` & `dicergirl-3.0.7/dicergirl/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from pathlib import Path
 from loguru import logger
 from typing import Union
 
 import json
-import os
+import sys
 import uuid
 import re
 import inspect
 
 try:
     from dicergirl.utils.decorators import translate_punctuation
-    from dicergirl.utils.settings import package, setconfig, getconfig
+    from dicergirl.utils.settings import get_package, setconfig, getconfig
+    from dicergirl import coc, scp, dnd
 except ImportError:
     from .decorators import translate_punctuation
-    from .settings import package, setconfig, getconfig
+    from .settings import get_package, setconfig, getconfig
+    from . import coc, scp, dnd
+
+package = get_package()
 
 if package == "nonebot2":
     class Message:
         pass
     try:
         from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent
     except ModuleNotFoundError:
@@ -34,41 +38,47 @@
     try:
         from botpy.message import Message
     except ModuleNotFoundError:
         logger.warning("未找到依赖`qq-botpy`, 请检查你的配置.")
         class Message:
             pass
 
+version = "3.0.7"
 current_dir = Path(__file__).resolve().parent
 dicer_girl_dir = Path.home() / ".dicergirl"
 data_dir = dicer_girl_dir / "data"
 _coc_cachepath = data_dir / "coc_cards.json"
 _scp_cachepath = data_dir / "scp_cards.json"
+_dnd_cachepath = data_dir / "dnd_cards.json"
 _super_user = data_dir / "super_user.json"
 _log = logger
 su_uuid = (str(uuid.uuid1()) + str(uuid.uuid4())).replace("-", "")
-version = "3.0.6"
+modes = {module.split(".")[-1]: sys.modules[module] for module in sys.modules if hasattr(sys.modules[module], "__type__")}
 
 def init():
     if not dicer_girl_dir.exists():
         _log.info("Dicer Girl 文件夹未建立, 建立它.")
         dicer_girl_dir.mkdir()
     if not data_dir.exists():
         _log.info("Dicer Girl 数据文件夹未建立, 建立它.")
         data_dir.mkdir()
-    if not os.path.exists(_coc_cachepath):
-        _log.info("[cocdicer] COC存储文件未建立, 建立它.")
+    if not _coc_cachepath.exists():
+        _log.info("COC 存储文件未建立, 建立它.")
         with open(_coc_cachepath, "w", encoding="utf-8") as f:
             f.write("{}")
-    if not os.path.exists(_scp_cachepath):
-        _log.info("[cocdicer] SCP存储文件未建立, 建立它.")
+    if not _scp_cachepath.exists():
+        _log.info("SCP 存储文件未建立, 建立它.")
         with open(_scp_cachepath, "w", encoding="utf-8") as f:
             f.write("{}")
-    if not os.path.exists(_super_user):
-        _log.info("[cocdicer] 超级用户存储文件未建立, 建立它.")
+    if not _dnd_cachepath.exists():
+        _log.info("DND 存储文件未建立, 建立它.")
+        with open(_dnd_cachepath, "w", encoding="utf-8") as f:
+            f.write("{}")
+    if not _super_user.exists():
+        _log.info("超级用户存储文件未建立, 建立它.")
         with open(_super_user, "w", encoding="utf-8") as f:
             f.write("{}")
 
 def set_config(appid, token):
     return setconfig(appid, token, path=dicer_girl_dir, filename="config.yaml")
 
 def get_config() -> dict:
@@ -110,26 +120,31 @@
             if annotations.get('message') is Message:
                 commands_functions.append(obj)
 
     return commands_functions
 
 def get_group_id(event):
     try:
-        if package == "nonebot2":
+        if package == "qqguild":
+            return str(event.channel_id)
+        elif package == "nonebot2":
             return str(event.group_id)
-        elif package == "qqguild":
-            return 
-    except KeyError:
+    except:
+        logger.warning(f"超出预计的 package: {package}, 将 Group ID 设置为 0.")
         return "0"
 
-def get_user_id(event: Union[Message, MessageEvent, GroupMessageEvent]):
-    if isinstance(event, Message):
-        return eval(str(event.author))["id"]
-    else:
-        return str(event.get_user_id())
+def get_user_id(event):
+    try:
+        if package == "qqguild":
+            return eval(str(event.author))["id"]
+        elif package:
+            return str(event.get_user_id())
+    except:
+        logger.warning(f"超出预计的 package: {package}, 将 User ID 设置为 0.")
+        return "0"
 
 def add_super_user(message):
     with open(_super_user, "w+") as _su:
         sr = _su.read()
         if not sr:
             sudos = {}
         else:
```

### Comparing `dicergirl-3.0.6/dicergirl.egg-info/PKG-INFO` & `dicergirl-3.0.7/dicergirl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: dicergirl
-Version: 3.0.6
+Version: 3.0.7
 Summary: 跑团骰娘机器人欧若可, 支持 QQ频道 及 Nonebot2 部署.
 Home-page: https://gitee.com/unvisitor/dicer
 Author: Night Resurgent <fu050409@163.com>
 Author-email: fu050409@163.com
 License: Apache-2.0
 Project-URL: Bug Tracker, https://gitee.com/unvisitor/dicer/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DicerGirl
```

### Comparing `dicergirl-3.0.6/dicergirl.egg-info/SOURCES.txt` & `dicergirl-3.0.7/dicergirl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 dicergirl.egg-info/dependency_links.txt
 dicergirl.egg-info/requires.txt
 dicergirl.egg-info/top_level.txt
 dicergirl/coc/__init__.py
 dicergirl/coc/coccards.py
 dicergirl/coc/cocutils.py
 dicergirl/coc/investigator.py
+dicergirl/dnd/__init__.py
+dicergirl/dnd/adventurer.py
+dicergirl/dnd/dndcards.py
+dicergirl/dnd/dndutils.py
 dicergirl/scp/__init__.py
 dicergirl/scp/agent.py
 dicergirl/scp/scpcards.py
 dicergirl/scp/scputils.py
 dicergirl/utils/__init__.py
 dicergirl/utils/chat.py
 dicergirl/utils/decorators.py
```

### Comparing `dicergirl-3.0.6/setup.py` & `dicergirl-3.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     long_description_content_type = "text/markdown",
     url = "https://gitee.com/unvisitor/dicer",
     project_urls = {
         "Bug Tracker": "https://gitee.com/unvisitor/dicer/issues",
     },
     classifiers = [
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license = "Apache-2.0",
     packages = setuptools.find_packages(),
     install_requires = [
         'nb-cli',
         'nonebot2',
```

