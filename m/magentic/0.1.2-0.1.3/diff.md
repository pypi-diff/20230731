# Comparing `tmp/magentic-0.1.2.tar.gz` & `tmp/magentic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magentic-0.1.2.tar", max compression
+gzip compressed data, was "magentic-0.1.3.tar", max compression
```

## Comparing `magentic-0.1.2.tar` & `magentic-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.2/LICENSE
--rw-r--r--   0        0        0     5156 2023-07-21 07:11:25.073401 magentic-0.1.2/README.md
--rw-r--r--   0        0        0     1023 2023-07-21 07:35:56.486824 magentic-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      139 2023-07-15 07:11:09.503451 magentic-0.1.2/src/magentic/__init__.py
--rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.2/src/magentic/chat.py
--rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.2/src/magentic/chat_model/__init__.py
--rw-r--r--   0        0        0     1517 2023-07-16 21:00:12.901908 magentic-0.1.2/src/magentic/chat_model/base.py
--rw-r--r--   0        0        0     9536 2023-07-21 05:15:28.116776 magentic-0.1.2/src/magentic/chat_model/openai_chat_model.py
--rw-r--r--   0        0        0     1348 2023-07-21 05:14:05.054740 magentic-0.1.2/src/magentic/function_call.py
--rw-r--r--   0        0        0     1712 2023-07-15 07:11:09.513068 magentic-0.1.2/src/magentic/prompt_chain.py
--rw-r--r--   0        0        0     3271 2023-07-16 20:42:38.366497 magentic-0.1.2/src/magentic/prompt_function.py
--rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.2/src/magentic/py.typed
--rw-r--r--   0        0        0     1584 2023-07-17 05:50:31.713612 magentic-0.1.2/src/magentic/typing.py
--rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 magentic-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-18 04:31:45.568698 magentic-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5234 2023-07-31 05:46:57.808915 magentic-0.1.3/README.md
+-rw-r--r--   0        0        0     1024 2023-07-31 05:56:11.031586 magentic-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-07-22 08:49:34.718170 magentic-0.1.3/src/magentic/__init__.py
+-rw-r--r--   0        0        0     2100 2023-07-15 07:11:09.503748 magentic-0.1.3/src/magentic/chat.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:11:09.503836 magentic-0.1.3/src/magentic/chat_model/__init__.py
+-rw-r--r--   0        0        0     1517 2023-07-16 21:00:12.901908 magentic-0.1.3/src/magentic/chat_model/base.py
+-rw-r--r--   0        0        0    11940 2023-07-31 05:46:57.811033 magentic-0.1.3/src/magentic/chat_model/openai_chat_model.py
+-rw-r--r--   0        0        0     1348 2023-07-31 05:24:05.969931 magentic-0.1.3/src/magentic/function_call.py
+-rw-r--r--   0        0        0     1696 2023-07-31 05:46:57.811305 magentic-0.1.3/src/magentic/prompt_chain.py
+-rw-r--r--   0        0        0     5233 2023-07-31 05:46:57.811616 magentic-0.1.3/src/magentic/prompt_function.py
+-rw-r--r--   0        0        0       61 2023-07-15 07:11:09.514294 magentic-0.1.3/src/magentic/py.typed
+-rw-r--r--   0        0        0     1584 2023-07-17 05:50:31.713612 magentic-0.1.3/src/magentic/typing.py
+-rw-r--r--   0        0        0     5827 1970-01-01 00:00:00.000000 magentic-0.1.3/PKG-INFO
```

### Comparing `magentic-0.1.2/LICENSE` & `magentic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `magentic-0.1.2/README.md` & `magentic-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 # 'The current weather in Boston is 72°F and it is sunny and windy.'
 ```
 
 LLM-powered functions created using `@prompt` and `@prompt_chain` can be supplied as `functions` to other `@prompt`/`@prompt_chain` decorators, just like regular python functions. This enables increasingly complex LLM-powered functionality, while allowing individual components to be tested and improved in isolation.
 
 ### Additional Features
 
+- The `@prompt` decorator can also be used with `async` function definitions.
 - The docstring of the decorated function will be used as the prompt template if the `template` argument is not provided to `@prompt`/`@prompt_chain`.
 - The `Annotated` type annotation can be used to provide descriptions and other metadata for function parameters. See [the pydantic documentation on using `Field` to describe function arguments](https://docs.pydantic.dev/latest/usage/validation_decorator/#using-field-to-describe-function-arguments).
 - The `@prompt` and `@prompt_chain` decorators also accept a `model` argument. You can pass an instance of `OpenaiChatModel` (from `magentic.chat_model.openai_chat_model`) to use GPT4 or configure a different temperature.
 
 ## Type Checking
 
 Many type checkers will raise warnings or errors for functions with the `prompt` decorator due to the function having no body or return value. There are several ways to deal with these.
```

### Comparing `magentic-0.1.2/src/magentic/chat.py` & `magentic-0.1.3/src/magentic/chat.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.2/src/magentic/chat_model/base.py` & `magentic-0.1.3/src/magentic/chat_model/base.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.2/src/magentic/chat_model/openai_chat_model.py` & `magentic-0.1.3/src/magentic/chat_model/openai_chat_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -280,7 +280,63 @@
         if not includes_str_output_type:
             raise ValueError(
                 "String was returned by model but not expected. You may need to update"
                 " your prompt to encourage the model to return a specific type."
             )
 
         return AssistantMessage(response_message["content"])
+
+    # TODO: Deduplicate this and `complete`
+    async def acomplete(
+        self,
+        messages: Iterable[Message[Any]],
+        functions: Iterable[Callable[..., FuncR]] | None = None,
+        output_types: Iterable[type[R | str]] | None = None,
+    ) -> FunctionCallMessage[FuncR] | AssistantMessage[R]:
+        """Async version of `complete`."""
+        if output_types is None:
+            output_types = [str]
+
+        function_schemas = [FunctionCallFunctionSchema(f) for f in functions or []] + [
+            function_schema_for_type(type_)
+            for type_ in output_types
+            if not issubclass(type_, str)
+        ]
+
+        includes_str_output_type = any(issubclass(cls, str) for cls in output_types)
+
+        # `openai.ChatCompletion.acreate` doesn't accept `None`
+        # so only pass function args if there are functions
+        function_args: dict[str, Any] = {}
+        if function_schemas:
+            function_args["functions"] = [schema.dict() for schema in function_schemas]
+        if len(function_schemas) == 1 and not includes_str_output_type:
+            # Force the model to call the function
+            function_args["function_call"] = {"name": function_schemas[0].name}
+
+        response: dict[str, Any] = await openai.ChatCompletion.acreate(  # type: ignore[no-untyped-call]
+            model=self._model,
+            messages=[message_to_openai_message(m) for m in messages],
+            temperature=self._temperature,
+            **function_args,
+        )
+        response_message = response["choices"][0]["message"]
+
+        if response_message.get("function_call"):
+            function_schema_by_name = {
+                function_schema.name: function_schema
+                for function_schema in function_schemas
+            }
+            function_name = response_message["function_call"]["name"]
+            function_schema = function_schema_by_name[function_name]
+            message = function_schema.parse_args_to_message(
+                response_message["function_call"]["arguments"]
+            )
+            return message
+
+        if not includes_str_output_type:
+            raise ValueError(
+                "String was returned by model but not expected. You may need to update"
+                " your prompt to encourage the model to return a specific type."
+            )
+
+        return AssistantMessage(response_message["content"])
```

### Comparing `magentic-0.1.2/src/magentic/function_call.py` & `magentic-0.1.3/src/magentic/function_call.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.2/src/magentic/prompt_chain.py` & `magentic-0.1.3/src/magentic/prompt_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 from functools import update_wrapper
-from typing import Any, Callable, ParamSpec, TypeVar
+from typing import Any, Callable, ParamSpec, TypeVar, cast
 
 from magentic.chat import Chat
 from magentic.chat_model.base import FunctionCallMessage
 from magentic.chat_model.openai_chat_model import OpenaiChatModel
 from magentic.prompt_function import PromptFunction
 
 P = ParamSpec("P")
@@ -34,12 +34,12 @@
         )
 
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
             chat = Chat.from_prompt(prompt_function, *args, **kwargs).submit()
             while isinstance(chat.messages[-1], FunctionCallMessage):
                 function_result_message = chat.messages[-1].get_result()
                 chat = chat.add_message(function_result_message).submit()
-            return chat.messages[-1].content  # type: ignore[no-any-return]
+            return cast(R, chat.messages[-1].content)
 
         return update_wrapper(wrapper, func)
 
     return decorator
```

### Comparing `magentic-0.1.2/src/magentic/typing.py` & `magentic-0.1.3/src/magentic/typing.py`

 * *Files identical despite different names*

### Comparing `magentic-0.1.2/PKG-INFO` & `magentic-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magentic
-Version: 0.1.2
+Version: 0.1.3
 Summary: Seamlessly integrate LLMs as Python functions
 Home-page: https://github.com/jackmpcollins/magentic
 License: MIT
 Author: Jack Collins
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -129,14 +129,15 @@
 # 'The current weather in Boston is 72°F and it is sunny and windy.'
 ```
 
 LLM-powered functions created using `@prompt` and `@prompt_chain` can be supplied as `functions` to other `@prompt`/`@prompt_chain` decorators, just like regular python functions. This enables increasingly complex LLM-powered functionality, while allowing individual components to be tested and improved in isolation.
 
 ### Additional Features
 
+- The `@prompt` decorator can also be used with `async` function definitions.
 - The docstring of the decorated function will be used as the prompt template if the `template` argument is not provided to `@prompt`/`@prompt_chain`.
 - The `Annotated` type annotation can be used to provide descriptions and other metadata for function parameters. See [the pydantic documentation on using `Field` to describe function arguments](https://docs.pydantic.dev/latest/usage/validation_decorator/#using-field-to-describe-function-arguments).
 - The `@prompt` and `@prompt_chain` decorators also accept a `model` argument. You can pass an instance of `OpenaiChatModel` (from `magentic.chat_model.openai_chat_model`) to use GPT4 or configure a different temperature.
 
 ## Type Checking
 
 Many type checkers will raise warnings or errors for functions with the `prompt` decorator due to the function having no body or return value. There are several ways to deal with these.
```

