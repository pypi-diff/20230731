# Comparing `tmp/llm_code-0.4.2.tar.gz` & `tmp/llm_code-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_code-0.4.2.tar", max compression
+gzip compressed data, was "llm_code-0.5.0.tar", max compression
```

## Comparing `llm_code-0.4.2.tar` & `llm_code-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-19 17:43:32.824715 llm_code-0.4.2/LICENSE
--rw-r--r--   0        0        0     4709 2023-05-25 15:52:22.287781 llm_code-0.4.2/README.md
--rw-r--r--   0        0        0       75 2023-05-21 18:28:27.298792 llm_code-0.4.2/llm_code/__init__.py
--rw-r--r--   0        0        0     1938 2023-05-22 20:59:37.527156 llm_code-0.4.2/llm_code/db.py
--rw-r--r--   0        0        0     4405 2023-06-13 21:07:30.427337 llm_code-0.4.2/llm_code/llm_code.py
--rw-r--r--   0        0        0     3293 2023-05-19 22:57:07.356159 llm_code-0.4.2/llm_code/templates.py
--rw-r--r--   0        0        0      161 2023-05-19 18:26:22.445515 llm_code-0.4.2/prompts/coding/system.toml
--rw-r--r--   0        0        0      613 2023-05-19 18:23:27.578834 llm_code-0.4.2/prompts/coding/user/input.toml
--rw-r--r--   0        0        0      396 2023-05-19 18:19:43.905655 llm_code-0.4.2/prompts/coding/user/simple.toml
--rw-r--r--   0        0        0     1157 2023-06-13 21:09:49.832457 llm_code-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 llm_code-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-19 17:20:49.716226 llm_code-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4709 2023-07-05 17:35:54.839230 llm_code-0.5.0/README.md
+-rw-r--r--   0        0        0       75 2023-05-21 03:18:50.955110 llm_code-0.5.0/llm_code/__init__.py
+-rw-r--r--   0        0        0     1938 2023-05-23 04:05:15.623074 llm_code-0.5.0/llm_code/db.py
+-rw-r--r--   0        0        0     4842 2023-07-31 01:21:10.112067 llm_code-0.5.0/llm_code/llm_code.py
+-rw-r--r--   0        0        0     3294 2023-07-31 01:21:38.962158 llm_code-0.5.0/llm_code/templates.py
+-rw-r--r--   0        0        0      161 2023-05-21 02:14:00.117237 llm_code-0.5.0/prompts/coding/system.toml
+-rw-r--r--   0        0        0      632 2023-07-31 01:07:49.935181 llm_code-0.5.0/prompts/coding/user/input.toml
+-rw-r--r--   0        0        0      396 2023-05-21 02:14:00.117693 llm_code-0.5.0/prompts/coding/user/simple.toml
+-rw-r--r--   0        0        0     1157 2023-07-31 01:21:58.097370 llm_code-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 llm_code-0.5.0/PKG-INFO
```

### Comparing `llm_code-0.4.2/LICENSE` & `llm_code-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.2/README.md` & `llm_code-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.2/llm_code/db.py` & `llm_code-0.5.0/llm_code/db.py`

 * *Files identical despite different names*

### Comparing `llm_code-0.4.2/llm_code/llm_code.py` & `llm_code-0.5.0/llm_code/llm_code.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,16 +53,38 @@
 
     return Message(
         role="assistant",
         content=record.assistant_message,
     )
 
 
+def get_code(inputs) -> str:
+    print(inputs)
+    files = [f for input in inputs for f in Path.cwd().glob(input)]
+    file_name = [f.name for f in files]
+    file_texts = [f.read_text() for f in files]
+    file_blobs = [
+        f"FILENAME: {name}\n```{text}\n```"
+        for (name, text) in zip(file_name, file_texts)
+    ]
+    return "\n---\n".join(file_blobs)
+
+
+def get_max_tokens(message: str) -> int:
+    return len(message.split(" "))
+
+
 @click.command()
-@click.option("-i", "--inputs", default=None, help="Glob of input files.")
+@click.option(
+    "-i",
+    "--inputs",
+    default=None,
+    multiple=True,
+    help="Glob of input files. Use repeatedly for multiple files.",
+)
 @click.option("-nc", "--no-cache", is_flag=True, help="Don't use cache.")
 @click.option("-4", "--gpt-4", is_flag=True, help="Use GPT-4.")
 @click.option("--version", is_flag=True, help="Show version.")
 @click.argument("instructions", nargs=-1)
 def main(inputs, instructions, version, no_cache, gpt_4):
     """Coding assistant using OpenAI's chat models.
 
@@ -89,19 +111,17 @@
 
     library = load_templates(settings.config_dir) or load_templates(
         Path(__file__).parent.parent
     )
     if not library:
         raise click.UsageError("No templates found.")
 
-    inputs = Path.cwd().glob(inputs) if inputs else []
-    input = "\n\n".join([i.read_text() for i in inputs])
-
-    if input:
-        message = library["coding/input"].message(code=input, instructions=instructions)
+    if inputs:
+        code = get_code(inputs)
+        message = library["coding/input"].message(code=code, instructions=instructions)
     else:
         message = library["coding/simple"].message(instructions=instructions)
 
     messages = [library["coding/system"].message(), message]
 
     cached_response = get_cached_response(settings, messages)
     if no_cache or not cached_response:
```

### Comparing `llm_code-0.4.2/llm_code/templates.py` & `llm_code-0.5.0/llm_code/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class Message(BaseModel):
     role: str
     content: str
 
     def code(self) -> Optional[Code]:
-        match = re.search(r"```(.*?)?\n(.*?)```", self.content, re.DOTALL)
+        match = re.search(r"```(.*?)?\n(.*?)```$", self.content, re.DOTALL)
         if match:
             lang = match.group(1).strip()
             code = match.group(2).strip()
             return Code(lang=lang, code=code)
         else:
             return None
```

### Comparing `llm_code-0.4.2/prompts/coding/user/input.toml` & `llm_code-0.5.0/prompts/coding/user/input.toml`

 * *Files 22% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 For example:
 ---
 Instructions:
 Please write a function that prints "Hello World!" to the console.
 
 Context:
-```python
+FILENAME: hello_world.py
+```
 if __name__ == "__main__":
     hello_world()
 ```
 
 Response:
 ```python
 def hello_world():
```

### Comparing `llm_code-0.4.2/pyproject.toml` & `llm_code-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llm-code"
-version = "0.4.2"
+version = "0.5.0"
 description = "An OpenAI LLM based CLI coding assistant."
 authors = ["Rushabh Doshi <radoshi+pypi@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "llm_code" }]
 homepage = "https://github.com/radoshi/llm-code"
 repository = "https://github.com/radoshi/llm-code"
```

### Comparing `llm_code-0.4.2/PKG-INFO` & `llm_code-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-code
-Version: 0.4.2
+Version: 0.5.0
 Summary: An OpenAI LLM based CLI coding assistant.
 Home-page: https://github.com/radoshi/llm-code
 License: MIT
 Keywords: openai,llm,cli,coding,assistant
 Author: Rushabh Doshi
 Author-email: radoshi+pypi@gmail.com
 Requires-Python: >=3.11,<4.0
```

