# Comparing `tmp/nonebot_plugin_blocker-0.3.5.tar.gz` & `tmp/nonebot_plugin_blocker-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.3.5.tar", last modified: Mon Jul 31 17:03:29 2023, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.3.6.tar", last modified: Mon Jul 31 17:08:27 2023, max compression
```

## Comparing `nonebot_plugin_blocker-0.3.5.tar` & `nonebot_plugin_blocker-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/LICENSE
--rw-r--r--   0        0        0     2935 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/README.md
--rw-r--r--   0        0        0      381 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3313 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     2785 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2422 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     2780 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6055 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2292 2023-07-31 17:03:05.035759 nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      640 2023-07-31 17:03:29.896006 nonebot_plugin_blocker-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/LICENSE
+-rw-r--r--   0        0        0     2935 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/README.md
+-rw-r--r--   0        0        0      381 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3313 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     2785 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2422 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     2780 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     6055 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2292 2023-07-31 17:08:00.149054 nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      640 2023-07-31 17:08:27.205239 nonebot_plugin_blocker-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     4545 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.3.6/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.3.5/LICENSE` & `nonebot_plugin_blocker-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/README.md` & `nonebot_plugin_blocker-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/__main__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     del blockerlist
     
 async def msg_checker_rule(event: GroupMessageEvent, state: T_State) -> bool:
     if (re.search("[at:qq=\d+]", event.get_plaintext()) and not event.is_tome()) or event.user_id == event.self_id:
         return False # 如果是骰子自己发的或者当发现at了任何人但不是骰子的时候不执行
     try:
         reply_config: dict = get_reply_config().get(str(event.self_id))
-        state["this_reply"] = reply_config.get(state["blocker_state"])
         if re.match(reply_config.get("command_on")+"$", event.get_plaintext()):
             state["blocker_state"] = "reply_on"
         elif re.match(reply_config.get("command_off")+"$", event.get_plaintext()):
             state["blocker_state"] = "reply_off"
+        state["this_reply"] = reply_config.get(state["blocker_state"])
     except (AttributeError,KeyError,TypeError):
         if match := re.match("[.。]bot (on|off)\s?(|\[at:qq=\d+\])", event.get_plaintext()):
             state["blocker_state"] = "reply_"+match.group(1)
             state["this_reply"] = reply_config_raw.get(state["blocker_state"])
     return True if "blocker_state" in state else False
     
 blocker = on_message(rule=msg_checker_rule, permission=GROUP_ADMIN | GROUP_OWNER | SUPERUSER, priority=1, block=True)
```

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/main.js` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/main.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.3.6/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.3.5/pyproject.toml` & `nonebot_plugin_blocker-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.3.5"
+version = "0.3.6"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.3.5/PKG-INFO` & `nonebot_plugin_blocker-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.3.5
+Version: 0.3.6
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.3.6 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

