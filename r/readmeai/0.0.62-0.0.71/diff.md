# Comparing `tmp/readmeai-0.0.62.tar.gz` & `tmp/readmeai-0.0.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.62.tar", max compression
+gzip compressed data, was "readmeai-0.0.71.tar", max compression
```

## Comparing `readmeai-0.0.62.tar` & `readmeai-0.0.71.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.62/LICENSE
--rw-r--r--   0        0        0    17673 2023-07-31 00:23:39.657351 readmeai-0.0.62/README.md
--rw-r--r--   0        0        0     1986 2023-07-31 01:00:49.981617 readmeai-0.0.62/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.62/readmeai/__init__.py
--rw-r--r--   0        0        0     7698 2023-07-30 11:40:35.990264 readmeai-0.0.62/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-07-30 11:40:37.755686 readmeai-0.0.62/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 11:40:32.060627 readmeai-0.0.62/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.62/readmeai/logger.py
--rwxr-xr-x   0        0        0     3998 2023-07-30 11:40:23.385292 readmeai-0.0.62/readmeai/main.py
--rw-r--r--   0        0        0     7590 2023-07-30 20:20:43.267025 readmeai-0.0.62/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-07-30 11:40:26.019565 readmeai-0.0.62/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 11:40:28.294350 readmeai-0.0.62/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 11:40:29.234241 readmeai-0.0.62/readmeai/utils.py
--rw-r--r--   0        0        0    19205 1970-01-01 00:00:00.000000 readmeai-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.71/LICENSE
+-rw-r--r--   0        0        0    17673 2023-07-31 00:23:39.657351 readmeai-0.0.71/README.md
+-rw-r--r--   0        0        0     1946 2023-07-31 01:14:26.524565 readmeai-0.0.71/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.71/readmeai/__init__.py
+-rw-r--r--   0        0        0     7698 2023-07-30 11:40:35.990264 readmeai-0.0.71/readmeai/builder.py
+-rw-r--r--   0        0        0     6342 2023-07-30 11:40:37.755686 readmeai-0.0.71/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 11:40:32.060627 readmeai-0.0.71/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.71/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3998 2023-07-30 11:40:23.385292 readmeai-0.0.71/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-30 20:20:43.267025 readmeai-0.0.71/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-07-30 11:40:26.019565 readmeai-0.0.71/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 11:40:28.294350 readmeai-0.0.71/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 11:40:29.234241 readmeai-0.0.71/readmeai/utils.py
+-rw-r--r--   0        0        0    19205 1970-01-01 00:00:00.000000 readmeai-0.0.71/PKG-INFO
```

### Comparing `readmeai-0.0.62/LICENSE` & `readmeai-0.0.71/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/README.md` & `readmeai-0.0.71/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/pyproject.toml` & `readmeai-0.0.71/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.62"
+version = "0.0.71"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
@@ -29,15 +29,14 @@
   "openai-python",
   "chatgpt-python",
   "openai-chatbot",
   "gpt-35-turbo",
   "gpt-4-api",
   "llm-agent"
 ]
-packages = [{ include = "readmeai/*" }]
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `readmeai-0.0.62/readmeai/builder.py` & `readmeai-0.0.71/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/conf.py` & `readmeai-0.0.71/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/factory.py` & `readmeai-0.0.71/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/logger.py` & `readmeai-0.0.71/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/main.py` & `readmeai-0.0.71/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/model.py` & `readmeai-0.0.71/readmeai/model.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/parse.py` & `readmeai-0.0.71/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/preprocess.py` & `readmeai-0.0.71/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/readmeai/utils.py` & `readmeai-0.0.71/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.62/PKG-INFO` & `readmeai-0.0.71/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.62
+Version: 0.0.71
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

