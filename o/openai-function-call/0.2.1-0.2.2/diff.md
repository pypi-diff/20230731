# Comparing `tmp/openai_function_call-0.2.1.tar.gz` & `tmp/openai_function_call-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.2.1.tar", max compression
+gzip compressed data, was "openai_function_call-0.2.2.tar", max compression
```

## Comparing `openai_function_call-0.2.1.tar` & `openai_function_call-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-07-22 16:07:42.134784 openai_function_call-0.2.1/LICENSE
--rw-r--r--   0        0        0     8394 2023-07-22 16:07:42.134784 openai_function_call-0.2.1/README.md
--rw-r--r--   0        0        0      187 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/__init__.py
--rw-r--r--   0        0        0      151 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/__init__.py
--rw-r--r--   0        0        0     5799 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/completion.py
--rw-r--r--   0        0        0      505 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/__init__.py
--rw-r--r--   0        0        0     1669 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/base.py
--rw-r--r--   0        0        0     3260 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/messages.py
--rw-r--r--   0        0        0     1486 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/messages/user.py
--rw-r--r--   0        0        0     3698 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/dsl/multitask.py
--rw-r--r--   0        0        0     6330 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/openai_function_call/function_calls.py
--rw-r--r--   0        0        0      662 2023-07-22 16:07:42.146784 openai_function_call-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 openai_function_call-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-31 15:48:05.333210 openai_function_call-0.2.2/LICENSE
+-rw-r--r--   0        0        0     8394 2023-07-31 15:48:05.333210 openai_function_call-0.2.2/README.md
+-rw-r--r--   0        0        0      187 2023-07-31 15:48:05.337210 openai_function_call-0.2.2/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-31 15:48:05.337210 openai_function_call-0.2.2/openai_function_call/dsl/__init__.py
+-rw-r--r--   0        0        0     5799 2023-07-31 15:48:05.337210 openai_function_call-0.2.2/openai_function_call/dsl/completion.py
+-rw-r--r--   0        0        0      505 2023-07-31 15:48:05.337210 openai_function_call-0.2.2/openai_function_call/dsl/messages/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-31 15:48:05.337210 openai_function_call-0.2.2/openai_function_call/dsl/messages/base.py
+-rw-r--r--   0        0        0     3260 2023-07-31 15:48:05.341210 openai_function_call-0.2.2/openai_function_call/dsl/messages/messages.py
+-rw-r--r--   0        0        0     1486 2023-07-31 15:48:05.341210 openai_function_call-0.2.2/openai_function_call/dsl/messages/user.py
+-rw-r--r--   0        0        0     3713 2023-07-31 15:48:05.341210 openai_function_call-0.2.2/openai_function_call/dsl/multitask.py
+-rw-r--r--   0        0        0     6501 2023-07-31 15:48:05.341210 openai_function_call-0.2.2/openai_function_call/function_calls.py
+-rw-r--r--   0        0        0      662 2023-07-31 15:48:05.341210 openai_function_call-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     9127 1970-01-01 00:00:00.000000 openai_function_call-0.2.2/PKG-INFO
```

### Comparing `openai_function_call-0.2.1/LICENSE` & `openai_function_call-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/README.md` & `openai_function_call-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/openai_function_call/dsl/completion.py` & `openai_function_call-0.2.2/openai_function_call/dsl/completion.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/openai_function_call/dsl/messages/base.py` & `openai_function_call-0.2.2/openai_function_call/dsl/messages/base.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/openai_function_call/dsl/messages/messages.py` & `openai_function_call-0.2.2/openai_function_call/dsl/messages/messages.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/openai_function_call/dsl/messages/user.py` & `openai_function_call-0.2.2/openai_function_call/dsl/messages/user.py`

 * *Files identical despite different names*

### Comparing `openai_function_call-0.2.1/openai_function_call/dsl/multitask.py` & `openai_function_call-0.2.2/openai_function_call/dsl/multitask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pydantic import create_model, Field
-from typing import Optional, List, Type
+from pydantic import BaseModel, create_model, Field
+from typing import Optional, List, Type, Union
 from openai_function_call import OpenAISchema
 
 
 class MultiTaskBase:
     task_type = None  # type: ignore
 
     @classmethod
@@ -44,15 +44,15 @@
                 stack -= 1
                 if stack == 0:
                     return str[: i + 1], str[i + 2 :]
         return None, str
 
 
 def MultiTask(
-    subtask_class: Type[OpenAISchema],
+    subtask_class: Type[BaseModel],
     name: Optional[str] = None,
     description: Optional[str] = None,
 ):
     """
     Dynamically create a MultiTask OpenAISchema that can be used to segment multiple
     tasks given a base class. This creates class that can be used to create a toolkit
     for a specific task, names and descriptions are automatically generated. However
```

### Comparing `openai_function_call-0.2.1/openai_function_call/function_calls.py` & `openai_function_call-0.2.2/openai_function_call/function_calls.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         parameters = self.validate_func.model.model_json_schema()
         parameters["properties"] = {
             k: v
             for k, v in parameters["properties"].items()
             if k not in ("v__duplicate_kwargs", "args", "kwargs")
         }
         parameters["required"] = sorted(
-            parameters["properties"]
-        )  # bug workaround see lc
-        _remove_a_key(parameters, "title")
+            k for k, v in parameters["properties"].items() if not "default" in v
+        )
         _remove_a_key(parameters, "additionalProperties")
+        _remove_a_key(parameters, "title")
         self.openai_schema = {
             "name": self.func.__name__,
             "description": self.func.__doc__,
             "parameters": parameters,
         }
         self.model = self.validate_func.model
 
@@ -106,15 +106,15 @@
         if throw_error:
             assert "function_call" in message, "No function call detected"
             assert (
                 message["function_call"]["name"] == self.openai_schema["name"]
             ), "Function name does not match"
 
         function_call = message["function_call"]
-        arguments = json.loads(function_call["arguments"])
+        arguments = json.loads(function_call["arguments"], strict=False)
         return self.validate_func(**arguments)
 
 
 class OpenAISchema(BaseModel):
     @classmethod
     @property
     def openai_schema(cls):
@@ -127,22 +127,25 @@
         Returns:
             model_json_schema (dict): A dictionary in the format of OpenAI's schema as jsonschema
         """
         schema = cls.model_json_schema()
         parameters = {
             k: v for k, v in schema.items() if k not in ("title", "description")
         }
-        parameters["required"] = sorted(parameters["properties"])
-        _remove_a_key(parameters, "title")
+        parameters["required"] = sorted(
+            k for k, v in parameters["properties"].items() if not "default" in v
+        )
 
         if "description" not in schema:
             schema[
                 "description"
             ] = f"Correctly extracted `{cls.__name__}` with all the required parameters with correct types"
 
+        _remove_a_key(parameters, "additionalProperties")
+        _remove_a_key(parameters, "title")
         return {
             "name": schema["title"],
             "description": schema["description"],
             "parameters": parameters,
         }
 
     @classmethod
@@ -161,15 +164,15 @@
         if throw_error:
             assert "function_call" in message, "No function call detected"
             assert (
                 message["function_call"]["name"] == cls.openai_schema["name"]
             ), "Function name does not match"
 
         function_call = message["function_call"]
-        arguments = json.loads(function_call["arguments"])
+        arguments = json.loads(function_call["arguments"], strict=False)
         return cls(**arguments)
 
 
 def openai_schema(cls):
     if not issubclass(cls, BaseModel):
         raise TypeError("Class must be a subclass of pydantic.BaseModel")
```

### Comparing `openai_function_call-0.2.1/pyproject.toml` & `openai_function_call-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-function-call"
-version = "0.2.1"
+version = "0.2.2"
 description = "Helper functions that allow us to improve openai's function_call ergonomics"
 authors = ["Jason <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "openai_function_call"}]
 repository = "https://github.com/jxnl/openai_function_call"
```

### Comparing `openai_function_call-0.2.1/PKG-INFO` & `openai_function_call-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-function-call
-Version: 0.2.1
+Version: 0.2.2
 Summary: Helper functions that allow us to improve openai's function_call ergonomics
 Home-page: https://github.com/jxnl/openai_function_call
 License: MIT
 Author: Jason
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

