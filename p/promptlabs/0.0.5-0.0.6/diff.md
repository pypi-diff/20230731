# Comparing `tmp/promptlabs-0.0.5.tar.gz` & `tmp/promptlabs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptlabs-0.0.5.tar", last modified: Sun Jul 30 08:45:32 2023, max compression
+gzip compressed data, was "promptlabs-0.0.6.tar", last modified: Mon Jul 31 02:52:59 2023, max compression
```

## Comparing `promptlabs-0.0.5.tar` & `promptlabs-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.5/LICENSE
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-30 08:45:32.663154 promptlabs-0.0.5/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.5/README.md
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       75 2023-07-30 08:44:44.000000 promptlabs-0.0.5/promptlabs/__init__.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/chain/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.5/promptlabs/chain/__init__.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1602 2023-07-28 05:55:16.000000 promptlabs-0.0.5/promptlabs/chain/base_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     6269 2023-07-28 06:22:47.000000 promptlabs-0.0.5/promptlabs/chain/function_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)    15272 2023-07-30 08:28:43.000000 promptlabs-0.0.5/promptlabs/chain/llm_chain.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2199 2023-07-27 05:36:18.000000 promptlabs-0.0.5/promptlabs/client.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     8106 2023-07-28 06:23:34.000000 promptlabs-0.0.5/promptlabs/pipeline.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs/scheme/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4403 2023-07-28 01:47:35.000000 promptlabs-0.0.5/promptlabs/scheme/llm.py
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.5/promptlabs/scheme/template.py
-drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-30 08:45:32.663154 promptlabs-0.0.5/promptlabs.egg-info/
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      264 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/PKG-INFO
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/SOURCES.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/dependency_links.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/requires.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-30 08:45:32.000000 promptlabs-0.0.5/promptlabs.egg-info/top_level.txt
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-30 08:45:32.663154 promptlabs-0.0.5/setup.cfg
--rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-30 08:44:45.000000 promptlabs-0.0.5/setup.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-31 02:52:59.333318 promptlabs-0.0.6/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.6/LICENSE
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-31 02:52:59.333318 promptlabs-0.0.6/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-24 04:54:11.000000 promptlabs-0.0.6/README.md
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-31 02:52:59.329319 promptlabs-0.0.6/promptlabs/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       75 2023-07-31 02:52:13.000000 promptlabs-0.0.6/promptlabs/__init__.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-31 02:52:59.333318 promptlabs-0.0.6/promptlabs/chain/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      184 2023-07-27 05:23:57.000000 promptlabs-0.0.6/promptlabs/chain/__init__.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     1602 2023-07-28 05:55:16.000000 promptlabs-0.0.6/promptlabs/chain/base_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4463 2023-07-30 08:46:45.000000 promptlabs-0.0.6/promptlabs/chain/function_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)    14698 2023-07-30 08:47:08.000000 promptlabs-0.0.6/promptlabs/chain/llm_chain.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     2205 2023-07-31 02:51:56.000000 promptlabs-0.0.6/promptlabs/client.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     8106 2023-07-28 06:23:34.000000 promptlabs-0.0.6/promptlabs/pipeline.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-31 02:52:59.333318 promptlabs-0.0.6/promptlabs/scheme/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)     4403 2023-07-28 01:47:35.000000 promptlabs-0.0.6/promptlabs/scheme/llm.py
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      711 2023-07-26 09:36:55.000000 promptlabs-0.0.6/promptlabs/scheme/template.py
+drwxrwxr-x   0 engineer_a  (1000) engineer_a  (1000)        0 2023-07-31 02:52:59.333318 promptlabs-0.0.6/promptlabs.egg-info/
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      328 2023-07-31 02:52:59.000000 promptlabs-0.0.6/promptlabs.egg-info/PKG-INFO
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      442 2023-07-31 02:52:59.000000 promptlabs-0.0.6/promptlabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)        1 2023-07-31 02:52:59.000000 promptlabs-0.0.6/promptlabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       25 2023-07-31 02:52:59.000000 promptlabs-0.0.6/promptlabs.egg-info/requires.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       11 2023-07-31 02:52:59.000000 promptlabs-0.0.6/promptlabs.egg-info/top_level.txt
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)       38 2023-07-31 02:52:59.333318 promptlabs-0.0.6/setup.cfg
+-rw-rw-r--   0 engineer_a  (1000) engineer_a  (1000)      546 2023-07-31 02:52:11.000000 promptlabs-0.0.6/setup.py
```

### Comparing `promptlabs-0.0.5/promptlabs/chain/base_chain.py` & `promptlabs-0.0.6/promptlabs/chain/base_chain.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.5/promptlabs/chain/llm_chain.py` & `promptlabs-0.0.6/promptlabs/chain/llm_chain.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,30 +56,14 @@
     @property
     def system_prompt(self) -> str:
         default_system_prompt = "You are a helpful assistant."
         if 'system_prompt' not in self.config:  
             return default_system_prompt
         else:
             return self.config["system_prompt"]
-    
-    
-    # def set_llm(self) -> BaseLLM:
-    #     if "llm_function" not in self.config:
-    #         if 'temperature' not in self.config:
-    #             temperature = 0.7
-    #         if 'max_tokens' not in self.config:
-    #             max_tokens = None
-    #         return ChatOpenAI(
-    #             model_name=self.model_name,
-    #             openai_api_key=self.config['openai_api_key'],
-    #             temperature=temperature,
-    #             max_tokens=max_tokens
-    #         )
-    #     else:
-    #         return self.config["llm_function"]
 
     def _call_llm(
         self,
         inputs: Dict[str, Any],
     ) -> Dict[str, Any]:
         max_retry = 3
         retry_count = 0
```

### Comparing `promptlabs-0.0.5/promptlabs/client.py` & `promptlabs-0.0.6/promptlabs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import promptlabs.chain as Chain
 from promptlabs.pipeline import Pipeline
 
 
 class Client:
     def __init__(self, api_key):
         self.api_key = api_key
-        self.endpoint_url = "https://pops.up.railway.app/api/package"
+        self.endpoint_url = "https://promptlabs.up.railway.app/api/package"
 
 
     def _fetch(self, url):
         try:
             response = requests.get(
                 self.endpoint_url + url,
                 headers={"Authorization": "Bearer " + self.api_key},
```

### Comparing `promptlabs-0.0.5/promptlabs/pipeline.py` & `promptlabs-0.0.6/promptlabs/pipeline.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.5/promptlabs/scheme/llm.py` & `promptlabs-0.0.6/promptlabs/scheme/llm.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.5/promptlabs/scheme/template.py` & `promptlabs-0.0.6/promptlabs/scheme/template.py`

 * *Files identical despite different names*

### Comparing `promptlabs-0.0.5/setup.py` & `promptlabs-0.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)
 """
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="promptlabs",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_namespace_packages(),
     description="promptlabs: A Python package for PromptOps (versioning, logging, experimenting, etc.)",
     auther="weavel",
     install_requires=['openai', 'pydantic', 'requests'],
     python_requires='>=3.7.1',
     keywords=['weavel', 'prompt', 'llm', 'promptops', 'promptlabs', 'prompt engineering']
 )
```

