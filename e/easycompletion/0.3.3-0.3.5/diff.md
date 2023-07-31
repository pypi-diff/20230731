# Comparing `tmp/easycompletion-0.3.3.tar.gz` & `tmp/easycompletion-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.3.3.tar", last modified: Mon Jul 31 07:15:45 2023, max compression
+gzip compressed data, was "easycompletion-0.3.5.tar", last modified: Mon Jul 31 21:30:55 2023, max compression
```

## Comparing `easycompletion-0.3.3.tar` & `easycompletion-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 07:15:34.000000 easycompletion-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 07:15:45.847635 easycompletion-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-31 07:15:34.000000 easycompletion-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 07:15:45.847635 easycompletion-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 07:15:34.000000 easycompletion-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 21:30:45.000000 easycompletion-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 21:30:55.776633 easycompletion-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-31 21:30:45.000000 easycompletion-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-31 21:30:45.000000 easycompletion-0.3.5/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:30:55.776633 easycompletion-0.3.5/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 21:30:55.000000 easycompletion-0.3.5/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 21:30:55.776633 easycompletion-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 21:30:45.000000 easycompletion-0.3.5/setup.py
```

### Comparing `easycompletion-0.3.3/LICENSE` & `easycompletion-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/PKG-INFO` & `easycompletion-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.3
+Version: 0.3.5
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.3/README.md` & `easycompletion-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/easycompletion/__init__.py` & `easycompletion-0.3.5/easycompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/easycompletion/constants.py` & `easycompletion-0.3.5/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/easycompletion/logger.py` & `easycompletion-0.3.5/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/easycompletion/model.py` & `easycompletion-0.3.5/easycompletion/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
     messages,
     system_message=None,
     model_failure_retries=5,
     model=None,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
     debug=DEBUG,
+    temperature=0.0
 ):
     """
     Function for sending chat messages and returning a chat response.
 
     Parameters:
         messages (str): Messages to send to the model. In the form {<role>: string, <content>: string} - roles are "user" and "assistant"
         system_message (str, optional): Message appended at the top sent by the system. Usually used to tell what the agent how to act.
@@ -253,15 +254,15 @@
 
     log(f"Prompt:\n{str(messages)}", type="prompt", log=debug)
 
     # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
         try:
-            response = openai.ChatCompletion.create(model=model, messages=messages)
+            response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
             break
         except Exception as e:
             log(f"OpenAI Error: {e}", type="error", log=debug)
             continue
         # wait 1 second
         time.sleep(1)
 
@@ -294,14 +295,15 @@
 def text_completion(
     text,
     model_failure_retries=5,
     model=None,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     api_key=None,
     debug=DEBUG,
+    temperature=0.0
 ):
     """
     Function for sending text and returning a text completion response.
 
     Parameters:
         text (str): Text to send to the model.
         model_failure_retries (int, optional): Number of retries if the request fails. Default is 5.
@@ -350,15 +352,15 @@
 
     log(f"Prompt:\n{text}", type="prompt", log=debug)
 
     # Try to make a request for a specified number of times
     response = None
     for i in range(model_failure_retries):
         try:
-            response = openai.ChatCompletion.create(model=model, messages=messages)
+            response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
             break
         except Exception as e:
             log(f"OpenAI Error: {e}", type="error", log=debug)
             continue
         # wait 1 second
         time.sleep(1)
 
@@ -396,14 +398,15 @@
     model_failure_retries=5,
     function_call=None,
     function_failure_retries=10,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     model=None,
     api_key=None,
     debug=DEBUG,
+    temperature=0.0
 ):
     """
     Send text and a list of functions to the model and return optional text and a function call.
     The function call is validated against the functions array.
     The input text is sent to the chat model and is treated as a user message.
 
     Args:
@@ -511,15 +514,15 @@
     if total_tokens > (16384 - chunk_length):
         log("Error: Message too long", type="error", log=debug)
         return {"error": "Message too long"}
 
     all_messages = []
 
     if system_message is not None:
-        messages.append({"role": "system", "content": system_message})
+        all_messages.append({"role": "system", "content": system_message})
 
     if messages is not None:
         all_messages += messages
 
     # Prepare the messages to be sent to the API
     all_messages.append({"role": "user", "content": text})
 
@@ -536,14 +539,15 @@
             try:
                 # If there are function(s) to call
                 response = openai.ChatCompletion.create(
                     model=model,
                     messages=all_messages,
                     functions=functions,
                     function_call=function_call,
+                    temperature=temperature
                 )
                 if not response.get("choices") or response["choices"][0] is None:
                     log("No choices in response", type="error", log=debug)
                     continue
                 break
             except Exception as e:
                 log(f"OpenAI Error: {e}", type="error", log=debug)
```

### Comparing `easycompletion-0.3.3/easycompletion/prompt.py` & `easycompletion-0.3.5/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.3/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.3.5/easycompletion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.3
+Version: 0.3.5
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.3.3/setup.py` & `easycompletion-0.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.3.3',
+    version='0.3.5',
     description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

