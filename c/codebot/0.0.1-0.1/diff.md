# Comparing `tmp/codebot-0.0.1.tar.gz` & `tmp/codebot-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.1.tar", last modified: Mon Jul 31 03:18:36 2023, max compression
+gzip compressed data, was "codebot-0.1.tar", last modified: Mon Jul 31 01:38:17 2023, max compression
```

## Comparing `codebot-0.0.1.tar` & `codebot-0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.554797 codebot-0.0.1/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:18:36.554394 codebot-0.0.1/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.548959 codebot-0.0.1/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      297 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:18:36.554966 codebot-0.0.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      225 2023-07-31 03:18:18.000000 codebot-0.0.1/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.552021 codebot-0.0.1/src/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.1/src/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.1/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12714 2023-07-31 02:19:31.000000 codebot-0.0.1/src/app_cn.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.553813 codebot-0.0.1/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.1/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.1/src/functions/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.1/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.1/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:17.800235 codebot-0.1/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      179 2023-07-31 01:38:17.799933 codebot-0.1/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:17.796888 codebot-0.1/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      179 2023-07-31 01:38:17.000000 codebot-0.1/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      315 2023-07-31 01:38:17.000000 codebot-0.1/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 01:38:17.000000 codebot-0.1/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 01:38:17.000000 codebot-0.1/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 01:38:17.000000 codebot-0.1/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 01:38:17.800435 codebot-0.1/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      223 2023-07-31 01:35:39.000000 codebot-0.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:17.797823 codebot-0.1/src/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      206 2023-07-31 01:37:44.000000 codebot-0.1/src/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12528 2023-07-31 01:37:58.000000 codebot-0.1/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12618 2023-07-31 01:27:34.000000 codebot-0.1/src/app_cn.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:17.798485 codebot-0.1/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.1/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.1/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:17.799241 codebot-0.1/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:38:07.000000 codebot-0.1/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      744 2023-07-31 01:24:31.000000 codebot-0.1/src/language/gettext.py
```

### Comparing `codebot-0.0.1/src/app.py` & `codebot-0.1/src/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,26 +5,19 @@
 import os
 import chainlit as cl
 from functions.FunctionManager import FunctionManager
 import inspect
 import tiktoken
 import importlib
 import asyncio
-from get_text import get_text
+from .language.gettext import get_text
 
 
-# Path of the configuration file
-config_path = os.path.join(os.path.expanduser('~'), '.codebot', 'config.json')
-
-# Read the configuration file
-with open(config_path, 'r') as config_file:
-    config_env = json.load(config_file)
-
-openai.api_key = config_env['openai']['api_key']
-openai.api_base = config_env['openai']['api_base']
+openai.api_key = os.environ.get("OPENAI_API_KEY")
+openai.api_base = os.environ.get("OPENAI_API_BASE")
 
 plugin_dirs = [
     d for d in os.listdir('plugins')
     if os.path.isdir(os.path.join('plugins', d)) and d != '__pycache__'
 ]
 
 functions = []
@@ -42,15 +35,16 @@
     module = importlib.import_module(f'plugins.{dir}.functions')
     functions.extend([
         obj for name, obj in inspect.getmembers(module) if inspect.isfunction(obj)
     ])
 
 function_manager = FunctionManager(functions=functions)
 print("functions:", function_manager.generate_functions_array())
-env_max_tokens = config_env['openai']['max_tokens']
+
+env_max_tokens = os.environ.get("MAX_TOKENS", None)
 if env_max_tokens is not None:
     max_tokens = int(env_max_tokens)
 else:
     max_tokens = 5000
 is_stop = False
 
 
@@ -63,15 +57,15 @@
         else:
             break
     conversation.insert(0, system_con)
     return conversation
 
 
 def get_token_count(conversation):
-    encoding = tiktoken.encoding_for_model(config_env['openai']['model'])
+    encoding = tiktoken.encoding_for_model(os.environ.get("OPENAI_MODEL") or "gpt-4")
 
     num_tokens = 0
     for message in conversation:
         num_tokens += 4
         for key, value in message.items():
             num_tokens += len(encoding.encode(str(value)))
             if key == "name":
@@ -105,15 +99,15 @@
             user_plugin_api_info = cl.user_session.get('user_plugin_api_info')
             if user_plugin_api_info is not None:
                 for item in user_plugin_api_info:
                     for i in item['api_info']:
                         functions.append(i)
             print("functions:", functions)
             async for stream_resp in await openai.ChatCompletion.acreate(
-                    model=config_env['openai']['model'],
+                    model=os.environ.get("OPENAI_MODEL") or "gpt-4",
                     messages=send_message,
                     stream=True,
                     function_call="auto",
                     functions=functions,
                     temperature=0):  # type: ignore
                 new_delta = stream_resp.choices[0]["delta"]
                 if is_stop:
@@ -176,15 +170,15 @@
             description = function_response['description']
             del function_response['description']
             message_history.append({
                 "role": "function",
                 "name": function_name,
                 "content": json.dumps(function_response),
             })
-            language = config_env['openai']['language']
+            language = os.environ.get("LANGUAGE") or "chinese"
             message_history.append({
                 "role": "user",
                 "content": str(description) + "\n\n" + "Please answer me in " + language
             })
             print("🚀" * 20)
         else:
             message_history.append({
@@ -265,15 +259,15 @@
 function response is {"code_output": "show image: ./tmp/1690679381.220762.png", "status": "success"}
 you need to respond like ![image](./tmp/1690679381.220762.png)
 3.After encountering an error, please try to utilize existing functions as much as possible to attempt problem-solving instead of providing direct feedback.
 4.[IMPORTANT] LOOP UNTIL YOU SOLVE THE PROBLEM. DO NOT GIVE UP.Prohibited to repeatedly make the same mistake more than 3 times.
 5.[IMPORTANT] In the process of problem-solving, you have an absolute dominant role. Please try not to consult user opinions and proceed directly according to your own ideas.
 6.Try to avoid printing terminal data with more than 2000 characters. Before considering using operations like print, make sure to first check if the content to be printed is too large. If it is, please store it in a file for later use by subsequent programs.
     '''
-    language = config_env['openai']['language']
+    language = os.environ.get("LANGUAGE") or "chinese"
     cl.user_session.set(
         "message_history",
         [{
             "role":
             "system",
             "content": content + "\n\n" + "Please answer me in " + language
         }])
@@ -315,18 +309,17 @@
         with open(file_path, "wb") as f:
             f.write(content)
         message_history = cl.user_session.get("message_history")
         message_history.append({
             "role": "assistant",
             "content": f"upload file ./tmp/{save_path} success"
         })
-        language = config_env['openai']['language']
         await cl.Message(
             author="Chatbot",
-            content=f"{get_text(language, 'upload_notification')} ./tmp/{save_path}",
+            content=f"{get_text(os.environ.get('LANGUAGE') or 'chinese', 'upload_notification')} ./tmp/{save_path}",
         ).send()
         return
     
     await on_message(user_message)
 
 
 @cl.on_stop
```

### Comparing `codebot-0.0.1/src/app_cn.py` & `codebot-0.1/src/app_cn.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,26 +5,21 @@
 import os
 import chainlit as cl
 from functions.FunctionManager import FunctionManager
 import inspect
 import tiktoken
 import importlib
 import asyncio
-from get_text import get_text
+from functions.MakeRequest import make_request, make_request_chatgpt_plugin
+import globale_values as gv
+from language.gettext import get_text
 
 
-# Path of the configuration file
-config_path = os.path.join(os.path.expanduser('~'), '.codebot', 'config.json')
-
-# Read the configuration file
-with open(config_path, 'r') as config_file:
-    config_env = json.load(config_file)
-
-openai.api_key = config_env['openai']['api_key']
-openai.api_base = config_env['openai']['api_base']
+openai.api_key = os.environ.get("OPENAI_API_KEY")
+openai.api_base = os.environ.get("OPENAI_API_BASE")
 
 plugin_dirs = [
     d for d in os.listdir('plugins')
     if os.path.isdir(os.path.join('plugins', d)) and d != '__pycache__'
 ]
 
 functions = []
@@ -42,15 +37,16 @@
     module = importlib.import_module(f'plugins.{dir}.functions')
     functions.extend([
         obj for name, obj in inspect.getmembers(module) if inspect.isfunction(obj)
     ])
 
 function_manager = FunctionManager(functions=functions)
 print("functions:", function_manager.generate_functions_array())
-env_max_tokens = config_env['openai']['max_tokens']
+
+env_max_tokens = os.environ.get("MAX_TOKENS", None)
 if env_max_tokens is not None:
     max_tokens = int(env_max_tokens)
 else:
     max_tokens = 5000
 is_stop = False
 
 
@@ -63,15 +59,15 @@
         else:
             break
     conversation.insert(0, system_con)
     return conversation
 
 
 def get_token_count(conversation):
-    encoding = tiktoken.encoding_for_model(config_env['openai']['model'])
+    encoding = tiktoken.encoding_for_model(os.environ.get("OPENAI_MODEL") or "gpt-4")
 
     num_tokens = 0
     for message in conversation:
         num_tokens += 4
         for key, value in message.items():
             num_tokens += len(encoding.encode(str(value)))
             if key == "name":
@@ -105,15 +101,15 @@
             user_plugin_api_info = cl.user_session.get('user_plugin_api_info')
             if user_plugin_api_info is not None:
                 for item in user_plugin_api_info:
                     for i in item['api_info']:
                         functions.append(i)
             print("functions:", functions)
             for stream_resp in openai.ChatCompletion.create(
-                    model=config_env['openai']['model'],
+                    model=os.environ.get("OPENAI_MODEL") or "gpt-4",
                     messages=send_message,
                     stream=True,
                     function_call="auto",
                     functions=functions,
                     temperature=0):  # type: ignore
                 new_delta = stream_resp.choices[0]["delta"]
                 if is_stop:
@@ -176,15 +172,15 @@
             description = function_response['description']
             del function_response['description']
             message_history.append({
                 "role": "function",
                 "name": function_name,
                 "content": json.dumps(function_response),
             })
-            language = config_env['openai']['language']
+            language = os.environ.get("LANGUAGE") or "chinese"
             message_history.append({
                 "role": "user",
                 "content": str(description) + "\n\n" + "Please answer me in " + language
             })
             print("🚀" * 20)
         else:
             message_history.append({
@@ -265,15 +261,15 @@
 function response is {"code_output": "show image: ./tmp/1690679381.220762.png", "status": "success"}
 you need to respond like ![image](./tmp/1690679381.220762.png)
 3.After encountering an error, please try to utilize existing functions as much as possible to attempt problem-solving instead of providing direct feedback.
 4.[IMPORTANT] LOOP UNTIL YOU SOLVE THE PROBLEM. DO NOT GIVE UP.Prohibited to repeatedly make the same mistake more than 3 times.
 5.[IMPORTANT] In the process of problem-solving, you have an absolute dominant role. Please try not to consult user opinions and proceed directly according to your own ideas.
 6.Try to avoid printing terminal data with more than 2000 characters. Before considering using operations like print, make sure to first check if the content to be printed is too large. If it is, please store it in a file for later use by subsequent programs.
     '''
-    language = config_env['openai']['language']
+    language = os.environ.get("LANGUAGE") or "chinese"
     cl.user_session.set(
         "message_history",
         [{
             "role":
             "system",
             "content": content + "\n\n" + "Please answer me in " + language
         }])
@@ -315,18 +311,17 @@
         with open(file_path, "wb") as f:
             f.write(content)
         message_history = cl.user_session.get("message_history")
         message_history.append({
             "role": "assistant",
             "content": f"upload file ./tmp/{save_path} success"
         })
-        language = config_env['openai']['language']
         await cl.Message(
             author="Chatbot",
-            content=f"{get_text(language, 'upload_notification')} ./tmp/{save_path}",
+            content=f"{get_text(os.environ.get('LANGUAGE') or 'chinese', 'upload_notification')} ./tmp/{save_path}",
         ).send()
         return
     
     await on_message(user_message)
 
 
 @cl.on_stop
```

### Comparing `codebot-0.0.1/src/functions/FunctionManager.py` & `codebot-0.1/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.1/src/get_text.py` & `codebot-0.1/src/language/gettext.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # 获取对应的文件名
     file_name = language_map.get(language.lower())
 
     if file_name is None:
         raise ValueError(f"Unsupported language: {language}")
 
     # 创建文件路径
-    file_path = os.path.join(os.path.dirname(__file__), 'language' , f"{file_name}.json")
+    file_path = os.path.join(os.path.dirname(__file__), f"{file_name}.json")
 
     # 打开并读取 JSON 文件
     with open(file_path, 'r', encoding='utf-8') as file:
         translation = json.load(file)
 
     # 返回指定键的翻译文本
     return translation.get(key)
```

