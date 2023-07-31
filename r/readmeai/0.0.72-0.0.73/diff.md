# Comparing `tmp/readmeai-0.0.72.tar.gz` & `tmp/readmeai-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readmeai-0.0.72.tar", max compression
+gzip compressed data, was "readmeai-0.0.73.tar", max compression
```

## Comparing `readmeai-0.0.72.tar` & `readmeai-0.0.73.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.72/LICENSE
--rw-r--r--   0        0        0    17673 2023-07-31 00:23:39.657351 readmeai-0.0.72/README.md
--rw-r--r--   0        0        0     1946 2023-07-31 01:26:24.781932 readmeai-0.0.72/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.72/readmeai/__init__.py
--rw-r--r--   0        0        0     7698 2023-07-30 11:40:35.990264 readmeai-0.0.72/readmeai/builder.py
--rw-r--r--   0        0        0     6342 2023-07-30 11:40:37.755686 readmeai-0.0.72/readmeai/conf.py
--rw-r--r--   0        0        0     4893 2023-07-30 11:40:32.060627 readmeai-0.0.72/readmeai/factory.py
--rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.72/readmeai/logger.py
--rwxr-xr-x   0        0        0     3998 2023-07-30 11:40:23.385292 readmeai-0.0.72/readmeai/main.py
--rw-r--r--   0        0        0     7589 2023-07-31 01:26:30.275174 readmeai-0.0.72/readmeai/model.py
--rw-r--r--   0        0        0     7272 2023-07-30 11:40:26.019565 readmeai-0.0.72/readmeai/parse.py
--rw-r--r--   0        0        0     6536 2023-07-30 11:40:28.294350 readmeai-0.0.72/readmeai/preprocess.py
--rw-r--r--   0        0        0     3991 2023-07-30 11:40:29.234241 readmeai-0.0.72/readmeai/utils.py
--rw-r--r--   0        0        0    19205 1970-01-01 00:00:00.000000 readmeai-0.0.72/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readmeai-0.0.73/LICENSE
+-rw-r--r--   0        0        0    17673 2023-07-31 00:23:39.657351 readmeai-0.0.73/README.md
+-rw-r--r--   0        0        0     1946 2023-07-31 01:35:46.924291 readmeai-0.0.73/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-29 22:31:14.648662 readmeai-0.0.73/readmeai/__init__.py
+-rw-r--r--   0        0        0     7698 2023-07-30 11:40:35.990264 readmeai-0.0.73/readmeai/builder.py
+-rw-r--r--   0        0        0     6342 2023-07-30 11:40:37.755686 readmeai-0.0.73/readmeai/conf.py
+-rw-r--r--   0        0        0     4893 2023-07-30 11:40:32.060627 readmeai-0.0.73/readmeai/factory.py
+-rw-r--r--   0        0        0     1722 2023-07-29 22:31:14.649620 readmeai-0.0.73/readmeai/logger.py
+-rwxr-xr-x   0        0        0     3998 2023-07-30 11:40:23.385292 readmeai-0.0.73/readmeai/main.py
+-rw-r--r--   0        0        0     7590 2023-07-31 01:26:53.430459 readmeai-0.0.73/readmeai/model.py
+-rw-r--r--   0        0        0     7272 2023-07-30 11:40:26.019565 readmeai-0.0.73/readmeai/parse.py
+-rw-r--r--   0        0        0     6536 2023-07-30 11:40:28.294350 readmeai-0.0.73/readmeai/preprocess.py
+-rw-r--r--   0        0        0     3991 2023-07-30 11:40:29.234241 readmeai-0.0.73/readmeai/utils.py
+-rw-r--r--   0        0        0    19205 1970-01-01 00:00:00.000000 readmeai-0.0.73/PKG-INFO
```

### Comparing `readmeai-0.0.72/LICENSE` & `readmeai-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/README.md` & `readmeai-0.0.73/README.md`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/pyproject.toml` & `readmeai-0.0.73/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "readmeai"
-version = "0.0.72"
+version = "0.0.73"
 description = "🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <0x.eli.64s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/readme-ai"
 documentation = "https://github.com/eli64s/readme-ai/blob/main/README.md"
 keywords = [
```

### Comparing `readmeai-0.0.72/readmeai/builder.py` & `readmeai-0.0.73/readmeai/builder.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/conf.py` & `readmeai-0.0.73/readmeai/conf.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/factory.py` & `readmeai-0.0.73/readmeai/factory.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/logger.py` & `readmeai-0.0.73/readmeai/logger.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/main.py` & `readmeai-0.0.73/readmeai/main.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/model.py` & `readmeai-0.0.73/readmeai/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,21 @@
 import asyncio
 import time
 from typing import Dict, List, Tuple
 
 import httpx
 import openai
 from cachetools import TTLCache
-from tenacity import (RetryError, retry, retry_if_exception_type,
-                      stop_after_attempt, wait_exponential)
+from tenacity import (
+    RetryError,
+    retry,
+    retry_if_exception_type,
+    stop_after_attempt,
+    wait_exponential,
+)
 
 from . import conf, logger, utils
 
 
 class OpenAIHandler:
     """OpenAI API handler for generating text for the README.md file."""
```

### Comparing `readmeai-0.0.72/readmeai/parse.py` & `readmeai-0.0.73/readmeai/parse.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/preprocess.py` & `readmeai-0.0.73/readmeai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/readmeai/utils.py` & `readmeai-0.0.73/readmeai/utils.py`

 * *Files identical despite different names*

### Comparing `readmeai-0.0.72/PKG-INFO` & `readmeai-0.0.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readmeai
-Version: 0.0.72
+Version: 0.0.73
 Summary: 🚀 Generate awesome README.md files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/readme-ai
 License: MIT
 Keywords: markdown,readme,readme-template,shieldsio,readme-md,awesome-readme,readme-generator,gpt-3,openai-api,automated-readme,auto-readme,gpt-4,llms,awesome-chatgpt,openai-python,chatgpt-python,openai-chatbot,gpt-35-turbo,gpt-4-api,llm-agent
 Author: Eli
 Author-email: 0x.eli.64s@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
```

