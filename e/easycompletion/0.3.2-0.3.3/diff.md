# Comparing `tmp/easycompletion-0.3.2.tar.gz` & `tmp/easycompletion-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.3.2.tar", last modified: Fri Jul 28 16:32:01 2023, max compression
+gzip compressed data, was "easycompletion-0.3.3.tar", last modified: Mon Jul 31 07:15:45 2023, max compression
```

## Comparing `easycompletion-0.3.2.tar` & `easycompletion-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:32:01.182435 easycompletion-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 16:31:47.000000 easycompletion-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 16:32:01.182435 easycompletion-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-28 16:31:47.000000 easycompletion-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:32:01.182435 easycompletion-0.3.2/easycompletion/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 16:31:47.000000 easycompletion-0.3.2/easycompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 16:31:47.000000 easycompletion-0.3.2/easycompletion/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-28 16:31:47.000000 easycompletion-0.3.2/easycompletion/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-07-28 16:31:47.000000 easycompletion-0.3.2/easycompletion/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-28 16:31:47.000000 easycompletion-0.3.2/easycompletion/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:32:01.182435 easycompletion-0.3.2/easycompletion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-28 16:32:01.000000 easycompletion-0.3.2/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-28 16:32:01.000000 easycompletion-0.3.2/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:32:01.000000 easycompletion-0.3.2/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 16:32:01.000000 easycompletion-0.3.2/easycompletion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 16:32:01.000000 easycompletion-0.3.2/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 16:32:01.182435 easycompletion-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-28 16:31:47.000000 easycompletion-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 07:15:34.000000 easycompletion-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 07:15:45.847635 easycompletion-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-07-31 07:15:34.000000 easycompletion-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/easycompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20904 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-31 07:15:34.000000 easycompletion-0.3.3/easycompletion/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 07:15:45.847635 easycompletion-0.3.3/easycompletion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 07:15:45.000000 easycompletion-0.3.3/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 07:15:45.847635 easycompletion-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-31 07:15:34.000000 easycompletion-0.3.3/setup.py
```

### Comparing `easycompletion-0.3.2/LICENSE` & `easycompletion-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.2/PKG-INFO` & `easycompletion-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.2
+Version: 0.3.3
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -186,18 +186,20 @@
     "total_tokens": "number"
   },
   "error": "string|None",
   "finish_reason": "string"
 }
 ```
 
-### `function_completion(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
+### `function_completion(text, functions=None, system_message=None, messages=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the model and returns optional text and a function call. The function call is validated against the functions array.
 
+Optionally takes a system message and a list of messages to send to the model before the function call. If messages are provided, the "text" becomes the last user message in the list.
+
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
 }
 
 response = function_completion("Call the function.", function)
```

### Comparing `easycompletion-0.3.2/README.md` & `easycompletion-0.3.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -170,18 +170,20 @@
     "total_tokens": "number"
   },
   "error": "string|None",
   "finish_reason": "string"
 }
 ```
 
-### `function_completion(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
+### `function_completion(text, functions=None, system_message=None, messages=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the model and returns optional text and a function call. The function call is validated against the functions array.
 
+Optionally takes a system message and a list of messages to send to the model before the function call. If messages are provided, the "text" becomes the last user message in the list.
+
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
 }
 
 response = function_completion("Call the function.", function)
```

#### html2text {}

```diff
@@ -49,30 +49,32 @@
 model_failure_retries=5, model=None, chunk_length=DEFAULT_CHUNK_LENGTH,
 api_key=None)` Sends text to the model and returns a text response. ```python
 response = text_completion( "Hello, how are you?", model_failure_retries=3,
 model='gpt-3.5-turbo', chunk_length=1024, api_key='your_openai_api_key' ) ```
 The response object looks like this: ```json { "text": "string", "usage":
 { "prompt_tokens": "number", "completion_tokens": "number", "total_tokens":
 "number" }, "error": "string|None", "finish_reason": "string" } ``` ###
-`function_completion(text, functions=None, model_failure_retries=5,
-function_call=None, function_failure_retries=10,
+`function_completion(text, functions=None, system_message=None, messages=None,
+model_failure_retries=5, function_call=None, function_failure_retries=10,
 chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)` Sends text and a
 list of functions to the model and returns optional text and a function call.
-The function call is validated against the functions array. ```python function
-= { 'name': 'function1', 'parameters': {'param1': 'value1'} } response =
-function_completion("Call the function.", function) ``` The response object
-looks like this: ```json { "text": "string", "function_name": "string",
-"arguments": "dict", "usage": { "prompt_tokens": "number", "completion_tokens":
-"number", "total_tokens": "number" }, "finish_reason": "string", "error":
-"string|None" } ``` ### `trim_prompt(text, max_tokens=DEFAULT_CHUNK_LENGTH,
-model=DEFAULT_TEXT_MODEL, preserve_top=True)` Trim the given text to a maximum
-number of tokens. ```python trimmed_text = trim_prompt("This is a test.", 3,
-preserve_top=True) ``` ### `chunk_prompt(prompt,
-chunk_length=DEFAULT_CHUNK_LENGTH)` Split the given prompt into chunks where
-each chunk has a maximum number of tokens. ```python prompt_chunks =
+The function call is validated against the functions array. Optionally takes a
+system message and a list of messages to send to the model before the function
+call. If messages are provided, the "text" becomes the last user message in the
+list. ```python function = { 'name': 'function1', 'parameters': {'param1':
+'value1'} } response = function_completion("Call the function.", function) ```
+The response object looks like this: ```json { "text": "string",
+"function_name": "string", "arguments": "dict", "usage": { "prompt_tokens":
+"number", "completion_tokens": "number", "total_tokens": "number" },
+"finish_reason": "string", "error": "string|None" } ``` ### `trim_prompt(text,
+max_tokens=DEFAULT_CHUNK_LENGTH, model=DEFAULT_TEXT_MODEL, preserve_top=True)`
+Trim the given text to a maximum number of tokens. ```python trimmed_text =
+trim_prompt("This is a test.", 3, preserve_top=True) ``` ### `chunk_prompt
+(prompt, chunk_length=DEFAULT_CHUNK_LENGTH)` Split the given prompt into chunks
+where each chunk has a maximum number of tokens. ```python prompt_chunks =
 chunk_prompt("This is a test. I am writing a function.", 4) ``` ###
 `count_tokens(prompt, model=DEFAULT_TEXT_MODEL)` Count the number of tokens in
 a string. ```python num_tokens = count_tokens("This is a test.") ``` ###
 `get_tokens(prompt, model=DEFAULT_TEXT_MODEL)` Returns a list of tokens in a
 string. ```python tokens = get_tokens("This is a test.") ``` ###
 `compose_prompt(prompt_template, parameters)` Composes a prompt using a
 template and parameters. Parameter keys are enclosed in double curly brackets
```

### Comparing `easycompletion-0.3.2/easycompletion/__init__.py` & `easycompletion-0.3.3/easycompletion/__init__.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.2/easycompletion/constants.py` & `easycompletion-0.3.3/easycompletion/constants.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.2/easycompletion/logger.py` & `easycompletion-0.3.3/easycompletion/logger.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.2/easycompletion/model.py` & `easycompletion-0.3.3/easycompletion/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -386,14 +386,16 @@
         "finish_reason": finish_reason,
         "error": None,
     }
 
 
 def function_completion(
     text,
+    system_message=None,
+    messages=None,
     functions=None,
     model_failure_retries=5,
     function_call=None,
     function_failure_retries=10,
     chunk_length=DEFAULT_CHUNK_LENGTH,
     model=None,
     api_key=None,
@@ -506,16 +508,24 @@
         log("Warning: Message is long. Using 16k model", type="warning", log=debug)
 
     # Check if the total number of tokens exceeds the maximum allowable tokens for the model
     if total_tokens > (16384 - chunk_length):
         log("Error: Message too long", type="error", log=debug)
         return {"error": "Message too long"}
 
+    all_messages = []
+
+    if system_message is not None:
+        messages.append({"role": "system", "content": system_message})
+
+    if messages is not None:
+        all_messages += messages
+
     # Prepare the messages to be sent to the API
-    messages = [{"role": "user", "content": text}]
+    all_messages.append({"role": "user", "content": text})
 
     log(
         f"Prompt:\n{text}\n\nFunctions:\n{json.dumps(functions, indent=4)}",
         type="prompt",
         log=debug,
     )
 
@@ -523,15 +533,15 @@
     response = None
     for _ in range(function_failure_retries):
         for _ in range(model_failure_retries):
             try:
                 # If there are function(s) to call
                 response = openai.ChatCompletion.create(
                     model=model,
-                    messages=messages,
+                    messages=all_messages,
                     functions=functions,
                     function_call=function_call,
                 )
                 if not response.get("choices") or response["choices"][0] is None:
                     log("No choices in response", type="error", log=debug)
                     continue
                 break
```

### Comparing `easycompletion-0.3.2/easycompletion/prompt.py` & `easycompletion-0.3.3/easycompletion/prompt.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.3.2/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.3.3/easycompletion.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.3.2
+Version: 0.3.3
 Summary: Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -186,18 +186,20 @@
     "total_tokens": "number"
   },
   "error": "string|None",
   "finish_reason": "string"
 }
 ```
 
-### `function_completion(text, functions=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
+### `function_completion(text, functions=None, system_message=None, messages=None, model_failure_retries=5, function_call=None, function_failure_retries=10, chunk_length=DEFAULT_CHUNK_LENGTH, model=None, api_key=None)`
 
 Sends text and a list of functions to the model and returns optional text and a function call. The function call is validated against the functions array.
 
+Optionally takes a system message and a list of messages to send to the model before the function call. If messages are provided, the "text" becomes the last user message in the list.
+
 ```python
 function = {
     'name': 'function1',
     'parameters': {'param1': 'value1'}
 }
 
 response = function_completion("Call the function.", function)
```

### Comparing `easycompletion-0.3.2/setup.py` & `easycompletion-0.3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.3.2',
+    version='0.3.3',
     description="Easy text completion and function calling. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

