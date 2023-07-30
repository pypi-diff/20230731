# Comparing `tmp/powerpoint_generative_ai-0.1.1.tar.gz` & `tmp/powerpoint_generative_ai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpoint_generative_ai-0.1.1.tar", last modified: Sun Jul 30 22:24:12 2023, max compression
+gzip compressed data, was "powerpoint_generative_ai-0.1.2.tar", last modified: Sun Jul 30 22:33:45 2023, max compression
```

## Comparing `powerpoint_generative_ai-0.1.1.tar` & `powerpoint_generative_ai-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:24:12.745933 powerpoint_generative_ai-0.1.1/
--rw-r--r--   0 pat        (501) staff       (20)     1064 2023-07-26 15:51:12.000000 powerpoint_generative_ai-0.1.1/LICENSE
--rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:24:12.745978 powerpoint_generative_ai-0.1.1/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)     2724 2023-07-30 22:06:24.000000 powerpoint_generative_ai-0.1.1/README.md
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:24:12.745321 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/
--rw-r--r--   0 pat        (501) staff       (20)      139 2023-07-30 22:04:43.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/__init__.py
--rw-r--r--   0 pat        (501) staff       (20)     2010 2023-07-26 07:25:07.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/ppt_analyzer.py
--rw-r--r--   0 pat        (501) staff       (20)     3163 2023-07-26 07:05:17.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/ppt_generator.py
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:24:12.745838 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/
--rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:24:12.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)      395 2023-07-30 22:24:12.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 pat        (501) staff       (20)        1 2023-07-30 22:24:12.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 pat        (501) staff       (20)       53 2023-07-30 22:24:12.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/requires.txt
--rw-r--r--   0 pat        (501) staff       (20)       25 2023-07-30 22:24:12.000000 powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/top_level.txt
--rw-r--r--   0 pat        (501) staff       (20)       79 2023-07-30 22:24:12.746128 powerpoint_generative_ai-0.1.1/setup.cfg
--rw-r--r--   0 pat        (501) staff       (20)     1168 2023-07-30 22:23:43.000000 powerpoint_generative_ai-0.1.1/setup.py
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427919 powerpoint_generative_ai-0.1.2/
+-rw-r--r--   0 pat        (501) staff       (20)     1064 2023-07-26 15:51:12.000000 powerpoint_generative_ai-0.1.2/LICENSE
+-rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:33:45.427977 powerpoint_generative_ai-0.1.2/PKG-INFO
+-rw-r--r--   0 pat        (501) staff       (20)     2724 2023-07-30 22:06:24.000000 powerpoint_generative_ai-0.1.2/README.md
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427269 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/
+-rw-r--r--   0 pat        (501) staff       (20)      139 2023-07-30 22:04:43.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/__init__.py
+-rw-r--r--   0 pat        (501) staff       (20)     2060 2023-07-30 22:30:04.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_analyzer.py
+-rw-r--r--   0 pat        (501) staff       (20)     3288 2023-07-30 22:29:51.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_generator.py
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427801 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/
+-rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 pat        (501) staff       (20)      395 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 pat        (501) staff       (20)        1 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 pat        (501) staff       (20)       53 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 pat        (501) staff       (20)       25 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/top_level.txt
+-rw-r--r--   0 pat        (501) staff       (20)       79 2023-07-30 22:33:45.428154 powerpoint_generative_ai-0.1.2/setup.cfg
+-rw-r--r--   0 pat        (501) staff       (20)     1168 2023-07-30 22:33:30.000000 powerpoint_generative_ai-0.1.2/setup.py
```

### Comparing `powerpoint_generative_ai-0.1.1/LICENSE` & `powerpoint_generative_ai-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.1/PKG-INFO` & `powerpoint_generative_ai-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: powerpoint_generative_ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information
 Home-page: https://github.com/Width-ai/powerpoint-generative-ai
-Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: LLM,Semantic Search,PowerPoints
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `powerpoint_generative_ai-0.1.1/README.md` & `powerpoint_generative_ai-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/ppt_analyzer.py` & `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import openai
 import pinecone
 from typing import List, Callable
-from ppt.ppt_loader import PPTLoader
-from utils.pinecone_utils import index_data, search_pinecone_index
+from powerpoint_generative_ai.ppt.ppt_loader import PPTLoader
+from powerpoint_generative_ai.utils.pinecone_utils import index_data, search_pinecone_index
 
 class PowerPointAnalyzer:
     """Analyze PPT files."""
     def __init__(self, openai_key: str, pinecone_key: str, pinecone_index: str, pinecone_env: str, custom_embeddings_function: Callable[[List], List] = None):
         """
         Initialize with api_keys and other vars. Also takes in an optional custom
         embeddings function that can be used, function signature should be as follows:
```

### Comparing `powerpoint_generative_ai-0.1.1/powerpoint_generative_ai/ppt_generator.py` & `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_generator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import openai
-from domain.constants import MAX_CONTENT_LENGTH
-from domain.exceptions import InvalidModel
-from domain.prompts import (
+from powerpoint_generative_ai.domain.constants import MAX_CONTENT_LENGTH
+from powerpoint_generative_ai.domain.exceptions import InvalidModel
+from powerpoint_generative_ai.domain.prompts import (
     DECK_CREATION_SYSTEM_PROMPT,
     CHART_DATA_IDENTIFICATION,
     BEST_CHART_FOR_DATA_SYSTEM_PROMPT,
     TITLE_GEN_SYSTEM_PROMPT,
     FILENAME_SYSTEM_PROMPT
 )
-from ppt.ppt_creator import PowerPointCreator
-from utils.utils import format_simple_message_for_gpt, call_gpt_with_backoff
+from powerpoint_generative_ai.ppt.ppt_creator import PowerPointCreator
+from powerpoint_generative_ai.utils.utils import format_simple_message_for_gpt, call_gpt_with_backoff
 
 class PowerPointGenerator:
     def __init__(self, openai_key: str, model: str = "gpt-4"):
         openai.api_key = openai_key
         if model not in [model.id for model in openai.Model.list()['data']]:
             raise InvalidModel(
                 f"Model {model} not found in list of models from OpenAI, make sure the "
```

### Comparing `powerpoint_generative_ai-0.1.1/powerpoint_generative_ai.egg-info/PKG-INFO` & `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: powerpoint-generative-ai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information
 Home-page: https://github.com/Width-ai/powerpoint-generative-ai
-Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.1.tar.gz
+Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: LLM,Semantic Search,PowerPoints
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `powerpoint_generative_ai-0.1.1/setup.py` & `powerpoint_generative_ai-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'powerpoint_generative_ai',
   packages = ['powerpoint_generative_ai'],
-  version = '0.1.1',
+  version = '0.1.2',
   license='MIT',
   description = 'Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information',
   author = 'Patrick Hennis',
   author_email = 'patrick@width.ai',
   url = 'https://github.com/Width-ai/powerpoint-generative-ai',
-  download_url = 'https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.1.tar.gz',
+  download_url = 'https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz',
   keywords = ['LLM', 'Semantic Search', 'PowerPoints'],
   install_requires=[
         'langchain',
         'openai',
         'python-pptx',
         'backoff',
         'pinecone-client'
```

