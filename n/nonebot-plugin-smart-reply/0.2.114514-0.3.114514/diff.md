# Comparing `tmp/nonebot_plugin_smart_reply-0.2.114514.tar.gz` & `tmp/nonebot_plugin_smart_reply-0.3.114514.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_smart_reply-0.2.114514.tar", last modified: Tue Jul 11 19:39:34 2023, max compression
+gzip compressed data, was "nonebot_plugin_smart_reply-0.3.114514.tar", last modified: Mon Jul 31 16:45:22 2023, max compression
```

## Comparing `nonebot_plugin_smart_reply-0.2.114514.tar` & `nonebot_plugin_smart_reply-0.3.114514.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:34.062090 nonebot_plugin_smart_reply-0.2.114514/
--rw-rw-rw-   0        0        0      325 2023-07-11 19:39:34.062090 nonebot_plugin_smart_reply-0.2.114514/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:33.840951 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/
--rw-rw-rw-   0        0        0     4014 2023-07-11 18:39:41.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/__init__.py
--rw-rw-rw-   0        0        0     1370 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/config.py
--rw-rw-rw-   0        0        0     5635 2023-07-11 19:15:41.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/getnewbing.py
--rw-rw-rw-   0        0        0     7156 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/getopenai.py
--rw-rw-rw-   0        0        0     5963 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/keywordhandle.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:33.777289 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:34.052089 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/
--rw-rw-rw-   0        0        0    32921 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
--rw-rw-rw-   0        0        0   122981 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
--rw-rw-rw-   0        0        0    67013 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
--rw-rw-rw-   0        0        0    42760 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
--rw-rw-rw-   0        0        0    36232 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
--rw-rw-rw-   0        0        0    11615 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
--rw-rw-rw-   0        0        0    68879 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
--rw-rw-rw-   0        0        0    15206 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
--rw-rw-rw-   0        0        0   101527 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
--rw-rw-rw-   0        0        0   105258 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
--rw-rw-rw-   0        0        0     6491 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
--rw-rw-rw-   0        0        0    15706 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
--rw-rw-rw-   0        0        0    96863 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
--rw-rw-rw-   0        0        0    14470 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
--rw-rw-rw-   0        0        0    74476 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:34.057088 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/json/
--rw-rw-rw-   0        0        0    81951 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/json/data.json
--rw-rw-rw-   0        0        0     2129 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/txtToImg.py
--rw-rw-rw-   0        0        0    10797 2023-07-11 18:29:42.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:39:33.876361 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-11 19:39:33.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1489 2023-07-11 19:39:33.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:39:33.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-11 19:39:33.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-07-11 19:39:33.000000 nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 19:39:34.062090 nonebot_plugin_smart_reply-0.2.114514/setup.cfg
--rw-rw-rw-   0        0        0      743 2023-07-11 19:39:24.000000 nonebot_plugin_smart_reply-0.2.114514/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.964485 nonebot_plugin_smart_reply-0.3.114514/
+-rw-rw-rw-   0        0        0      325 2023-07-31 16:45:22.963486 nonebot_plugin_smart_reply-0.3.114514/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.885199 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/
+-rw-rw-rw-   0        0        0     4014 2023-07-31 16:09:18.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-07-31 16:27:47.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/config.py
+-rw-rw-rw-   0        0        0     5492 2023-07-31 16:08:30.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getnewbing.py
+-rw-rw-rw-   0        0        0     7175 2023-07-31 16:30:17.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getopenai.py
+-rw-rw-rw-   0        0        0     8080 2023-07-31 16:42:31.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/keywordhandle.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.873538 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.950485 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/
+-rw-rw-rw-   0        0        0    32921 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac
+-rw-rw-rw-   0        0        0   122981 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac
+-rw-rw-rw-   0        0        0    67013 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac
+-rw-rw-rw-   0        0        0    42760 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac
+-rw-rw-rw-   0        0        0    36232 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac
+-rw-rw-rw-   0        0        0    11615 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac
+-rw-rw-rw-   0        0        0    68879 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac
+-rw-rw-rw-   0        0        0    15206 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac
+-rw-rw-rw-   0        0        0   101527 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac
+-rw-rw-rw-   0        0        0   105258 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac
+-rw-rw-rw-   0        0        0     6491 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac
+-rw-rw-rw-   0        0        0    15706 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac
+-rw-rw-rw-   0        0        0    96863 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac
+-rw-rw-rw-   0        0        0    14470 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac
+-rw-rw-rw-   0        0        0    74476 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.961487 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/
+-rw-rw-rw-   0        0        0    81951 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/data.json
+-rw-rw-rw-   0        0        0     2129 2023-07-31 15:57:21.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/txtToImg.py
+-rw-rw-rw-   0        0        0    10841 2023-07-31 16:26:15.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:45:22.907198 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1489 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-07-31 16:45:22.000000 nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:45:22.964485 nonebot_plugin_smart_reply-0.3.114514/setup.cfg
+-rw-rw-rw-   0        0        0      743 2023-07-31 16:45:00.000000 nonebot_plugin_smart_reply-0.3.114514/setup.py
```

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/__init__.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/config.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     openai_api_key: Optional[Sequence[str]]
     openai_max_tokens: int = 1000
     openai_cd_time: int = 600
     openai_max_conversation: int = 10
     newbing_cd_time: int = 600
     newbing_style: str = "creative"
     bing_or_openai_proxy: str = ""
-    superusers: Optional[Sequence[str]] = []
+    superusers: Sequence[str] = []
 
     @validator("openai_api_key")
     def _check_openai_api_key(cls, v):
         if isinstance(v, str):
             logger.info("openai_api_key读取, 初始化成功, 共 1 个api_key")
             return [v]
         elif isinstance(v, Sequence) and v:
```

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/getnewbing.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getnewbing.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,87 +36,85 @@
         uid: str = event.get_user_id()  # 获取用户id
         if not self.reply_private and isinstance(event, PrivateMessageEvent):
             await matcher.finish()  # 配置私聊不启用后，私聊信息直接结束处理
         if msg.isspace() or not msg:  # 如果消息为空或者全为空格, 则结束处理
             await matcher.finish()
         if not self.cookie_allow:
             await matcher.finish("cookie未设置, 无法访问")
-        reply_msg: MessageSegment = MessageSegment.reply(
-            event.message_id
-        )  # 回复消息的MessageSegment
         if msg in utils.nonsense:
             await matcher.finish(
-                reply_msg + MessageSegment.text(await utils.rand_hello())
+                MessageSegment.text(await utils.rand_hello()), reply_message=True
             )
         if uid not in utils.bing_chat_dict:
             await utils.newbing_new_chat(event=event, matcher=matcher)
-            await matcher.send(reply_msg + MessageSegment.text("newbing新会话已创建"))
+            await matcher.send(MessageSegment.text("newbing新会话已创建"), reply_message=True)
         if utils.bing_chat_dict[uid]["isRunning"]:
-            await matcher.finish(reply_msg + MessageSegment.text("当前会话正在运行中, 请稍后再发起请求"))
+            await matcher.finish(
+                MessageSegment.text("当前会话正在运行中, 请稍后再发起请求"), reply_message=True
+            )
         utils.bing_chat_dict[uid]["isRunning"] = True
 
     async def bing_handle(
         self, matcher: Matcher, event: MessageEvent, args: Message = CommandArg()
     ) -> None:
         """newbing聊天的handle函数"""
         uid: str = event.get_user_id()  # 获取用户id
         msg: str = args.extract_plain_text()  # 获取消息
 
         await self.pretreatment(event=event, matcher=matcher, msg=msg)  # 预处理
 
         bot: Chatbot = utils.bing_chat_dict[uid]["chatbot"]  # 获取当前会话的Chatbot对象
         style: str = utils.bing_chat_dict[uid]["model"]  # 获取当前会话的对话样式
-        reply_msg: MessageSegment = MessageSegment.reply(
-            event.message_id
-        )  # 回复消息的MessageSegment
+
         try:  # 尝试获取bing的回复
             data: Dict[str, Any] = await bot.ask(
                 prompt=msg, conversation_style=self.style[style], simplify_response=True
             )
         except Exception as e:  # 如果出现异常, 则返回异常信息, 并且将当前会话状态设置为未运行
             utils.bing_chat_dict[uid]["isRunning"] = False
             await matcher.finish(
-                reply_msg
-                + MessageSegment.text(f'askError: {repr(e)}多次askError请尝试"重置bing"')
+                MessageSegment.text(f'askError: {repr(e)}多次askError请尝试"重置bing"'),
+                reply_message=True,
             )
 
         utils.bing_chat_dict[uid]["isRunning"] = False  # 将当前会话状态设置为未运行
         utils.bing_chat_dict[uid]["sessions_number"] += 1  # 会话数+1
         if "text" not in data:
             await matcher.finish(
-                reply_msg + MessageSegment.text("bing没有返回text, 请重试")
+                MessageSegment.text("bing没有返回text, 请重试"), reply_message=True
             )
         current_conversation: int = utils.bing_chat_dict[uid]["sessions_number"]
         max_conversation: int = data["messages_left"] + current_conversation
 
         rep_message: str = await utils.bing_string_handle(data["text"])
 
         try:  # 尝试发送回复
             await matcher.send(
-                reply_msg
-                + MessageSegment.text(
+                MessageSegment.text(
                     f"{rep_message}\n\n当前{current_conversation} 共 {max_conversation}"
-                )
+                ),
+                reply_message=True,
             )
             if max_conversation <= current_conversation:
-                await matcher.send(reply_msg + MessageSegment.text("达到对话上限, 正帮你重置会话"))
+                await matcher.send(
+                    MessageSegment.text("达到对话上限, 正帮你重置会话"), reply_message=True
+                )
                 try:
                     await utils.newbing_new_chat(event=event, matcher=matcher)
                 except Exception:
                     return
         except Exception as e:  # 如果发送失败, 则尝试把文字写在图片上发送
             try:
                 await matcher.send(
-                    reply_msg
-                    + MessageSegment.text(
-                        f"文本消息可能被风控了\n错误信息:{repr(e)}\n这里咱尝试把文字写在图片上发送了"
-                    )
-                    + MessageSegment.image(await utils.text_to_img(rep_message))
+                    MessageSegment.text(f"文本消息可能被风控了\n错误信息:{repr(e)}\n这里咱尝试把文字写在图片上发送了")
+                    + MessageSegment.image(await utils.text_to_img(rep_message)),
+                    reply_message=True,
                 )
             except Exception as eeee:  # 如果还是失败, 我也没辙了, 只能返回异常信息了
                 await matcher.send(
-                    reply_msg + MessageSegment.text(f"消息全被风控了, 这是捕获的异常: \n{repr(eeee)}")
+                    MessageSegment.text(f"消息全被风控了, 这是捕获的异常: \n{repr(eeee)}"),
+                    reply_message=True,
                 )
 
 
 # 实例化一个NewBing对象
 newbing = NewBing()
```

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/getopenai.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/getopenai.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,61 +44,63 @@
         msg: str = args.extract_plain_text()  # 获取消息
 
         if not self.apikey_allow:
             await matcher.finish("openai_api_key未设置, 无法访问")
 
         if msg.isspace() or not msg:
             return  # 如果消息为空, 则不处理
-        reply_msg: MessageSegment = MessageSegment.reply(
-            event.message_id
-        )  # 回复消息的MessageSegment
         if msg in utils.nonsense:
             # 如果消息为空或者是一些无意义的问候, 则返回一些问候语
             await matcher.finish(
-                reply_msg + MessageSegment.text(await utils.rand_hello())
+                MessageSegment.text(await utils.rand_hello()), reply_message=True
             )
         if uid not in utils.openai_chat_dict:  # 如果用户id不在会话字典中, 则新建一个会话
             await utils.openai_new_chat(event=event, matcher=matcher)
-            await matcher.send(reply_msg + MessageSegment.text("openai新会话已创建"))
+            await matcher.send(MessageSegment.text("openai新会话已创建"), reply_message=True)
         if utils.openai_chat_dict[uid]["isRunning"]:  # 如果当前会话正在运行, 则返回正在运行
-            await matcher.finish(reply_msg + MessageSegment.text("当前会话正在运行中, 请稍后再发起请求"))
+            await matcher.finish(
+                MessageSegment.text("当前会话正在运行中, 请稍后再发起请求"), reply_message=True
+            )
         if utils.openai_chat_dict[uid]["sessions_number"] >= self.max_sessions_number:
             # 如果会话数超过最大会话数, 则返回会话数已达上限
-            await matcher.send(reply_msg + MessageSegment.text("会话数已达上限, 正在帮您请重置会话"))
+            await matcher.send(
+                MessageSegment.text("会话数已达上限, 正在帮您请重置会话"), reply_message=True
+            )
             await self.reserve_openai(matcher=matcher, event=event)
             return
         utils.openai_chat_dict[uid]["isRunning"] = True  # 将当前会话状态设置为运行中
         bot: Chatbot = utils.openai_chat_dict[uid]["chatbot"]  # 获取当前会话的Chatbot对象
         try:
             loop = asyncio.get_event_loop()  # 调用ask会阻塞asyncio
             data: str = await loop.run_in_executor(None, bot.ask, msg)
             utils.openai_chat_dict[uid]["sessions_number"] += 1  # 会话数+1
         except Exception as e:  # 如果出现异常, 则返回异常信息, 并且将当前会话状态设置为未运行
             utils.openai_chat_dict[uid]["isRunning"] = False
             await matcher.finish(
-                reply_msg
-                + MessageSegment.text(f'askError: {repr(e)}多次askError请尝试发送"重置openai"')
+                MessageSegment.text(f'askError: {repr(e)}多次askError请尝试发送"重置openai"'),
+                reply_message=True,
             )
         utils.openai_chat_dict[uid]["isRunning"] = False  # 将当前会话状态设置为未运行
         sessions_number: int = utils.openai_chat_dict[uid][
             "sessions_number"
         ]  # 获取当前会话的会话数
         data += f'\n\n当前: {sessions_number} 共{self.max_sessions_number}  \n字数异常请发送"重置openai"'
         try:
-            await matcher.send(reply_msg + MessageSegment.text(data))
+            await matcher.send(MessageSegment.text(data), reply_message=True)
         except Exception as e:
             try:
                 await matcher.send(
-                    reply_msg
-                    + MessageSegment.text(f"文本消息被风控了,错误信息:{repr(e)}, 这里咱尝试把文字写在图片上发送了")
-                    + MessageSegment.image(await utils.text_to_img(data))
+                    MessageSegment.text(f"文本消息被风控了,错误信息:{repr(e)}, 这里咱尝试把文字写在图片上发送了")
+                    + MessageSegment.image(await utils.text_to_img(data)),
+                    reply_message=True,
                 )
             except Exception as eeee:
                 await matcher.send(
-                    reply_msg + MessageSegment.text(f"消息全被风控了, 这是捕获的异常: \n{repr(eeee)}")
+                    MessageSegment.text(f"消息全被风控了, 这是捕获的异常: \n{repr(eeee)}"),
+                    reply_message=True,
                 )
 
     async def get_usage(self, params: dict, apikey: str) -> str:
         headers: Dict[str, str] = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {apikey}",
         }
```

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/cnm傻逼吃屎滚.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊(振声!).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你寄吧谁啊我超.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你是不是有毛病.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/你正常一点.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/傻逼.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/南通啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/去死吧.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/变态啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/啊你好烦啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/我草泥马.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/操你妈.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/救命啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/草泥马(慢).aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/audio/非礼啊.aac`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/resource/json/data.json` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/resource/json/data.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/txtToImg.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/txtToImg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply/utils.py` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             "在吗",
             "在不在",
             "您好",
             "您好啊",
             "你好",
             "在",
         )
+        self.superuser = config.superusers
         self.module_path: Path = Path(__file__).parent
         self.keyword_path: Path = self.module_path / "resource/json/data.json"
         self.anime_thesaurus: Dict = json.load(
             open(self.keyword_path, "r", encoding="utf-8")
         )
         self.audio_path: Path = self.module_path / "resource/audio"
         self.audio_list: List[str] = os.listdir(self.audio_path)
```

### Comparing `nonebot_plugin_smart_reply-0.2.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt` & `nonebot_plugin_smart_reply-0.3.114514/nonebot_plugin_smart_reply.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_smart_reply-0.2.114514/setup.py` & `nonebot_plugin_smart_reply-0.3.114514/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="nonebot_plugin_smart_reply",
-    version="0.02.114514",
+    version="0.03.114514",
     author="Special-Week",
     author_email="HuaMing27499@gmail.com",
     description="nonebot2的融合了openai, newbing, 词库的智障回复插件",
     python_requires=">=3.9.0",
     packages=find_packages(),
     long_description="reply插件",
     url="https://github.com/Special-Week/nonebot_plugin_smart_reply",
```

