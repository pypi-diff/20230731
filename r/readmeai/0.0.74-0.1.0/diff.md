# Comparing `tmp/readmeai-0.0.74.tar.gz` & `tmp/readmeai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.74.tar", max compression
+gzip compressed data, was "readmeai-0.1.0.tar", max compression
```

## Comparing `readmeai-0.0.74.tar` & `readmeai-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-07-31 02:06:11.454644 readmeai-0.0.74/LICENSE
--rw-r--r--   0        0        0    17673 2023-07-31 02:06:11.454644 readmeai-0.0.74/README.md
--rw-r--r--   0        0        0     1946 2023-07-31 02:06:11.494645 readmeai-0.0.74/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/__init__.py
--rw-r--r--   0        0        0     7698 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/logger.py
--rwxr-xr-x   0        0        0     3998 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-31 02:06:11.494645 readmeai-0.0.74/readmeai/utils.py
--rw-r--r--   0        0        0    19205 1970-01-01 00:00:00.000000 readmeai-0.0.74/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-31 03:27:10.723147 readmeai-0.1.0/LICENSE
+-rw-r--r--   0        0        0    17673 2023-07-31 03:27:10.723147 readmeai-0.1.0/README.md
+-rw-r--r--   0        0        0     1927 2023-07-31 03:27:10.763148 readmeai-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/__init__.py
+-rw-r--r--   0        0        0     7698 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/builder.py
+-rw-r--r--   0        0        0     6342 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3998 2023-07-31 03:27:10.763148 readmeai-0.1.0/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-31 03:27:10.767148 readmeai-0.1.0/readmeai/utils.py
+-rw-r--r--   0        0        0    19190 1970-01-01 00:00:00.000000 readmeai-0.1.0/PKG-INFO
```

### Comparing `readmeai-0.0.74/LICENSE` & `readmeai-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/README.md` & `readmeai-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/pyproject.toml` & `readmeai-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.74"
+version = "0.1.0"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
-  "markdown",
   "readme",
+  "python-cli",
   "readme-template",
-  "shieldsio",
   "readme-md",
   "awesome-readme",
   "readme-generator",
   "gpt-3",
   "openai-api",
   "automated-readme",
   "auto-readme",
   "gpt-4",
   "llms",
-  "awesome-chatgpt",
   "openai-python",
   "chatgpt-python",
-  "openai-chatbot",
   "gpt-35-turbo",
   "gpt-4-api",
-  "llm-agent"
+  "openai-cli",
+  "llm-prompting",
+  "llm-agent",
 ]
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
```

### Comparing `readmeai-0.0.74/readmeai/builder.py` & `readmeai-0.1.0/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/conf.py` & `readmeai-0.1.0/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/factory.py` & `readmeai-0.1.0/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/logger.py` & `readmeai-0.1.0/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/main.py` & `readmeai-0.1.0/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/model.py` & `readmeai-0.1.0/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/parse.py` & `readmeai-0.1.0/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/preprocess.py` & `readmeai-0.1.0/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/readmeai/utils.py` & `readmeai-0.1.0/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.74/PKG-INFO` & `readmeai-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.74
+Version: 0.1.0
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
-Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
+Keywords: readme,python-cli,readme-template,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,openai-python,chatgpt-python,gpt-35-turbo,gpt-4-api,openai-cli,llm-prompting,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

