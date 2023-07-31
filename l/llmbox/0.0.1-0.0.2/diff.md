# Comparing `tmp/llmbox-0.0.1.tar.gz` & `tmp/llmbox-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmbox-0.0.1.tar", last modified: Wed Jul 26 05:54:27 2023, max compression
+gzip compressed data, was "llmbox-0.0.2.tar", last modified: Mon Jul 31 09:14:13 2023, max compression
```

## Comparing `llmbox-0.0.1.tar` & `llmbox-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-26 05:54:27.095861 llmbox-0.0.1/
--rw-r--r--   0 rohanrao   (501) staff       (20)    11357 2023-07-12 12:10:08.000000 llmbox-0.0.1/LICENSE
--rw-r--r--   0 rohanrao   (501) staff       (20)     2816 2023-07-26 05:54:27.095736 llmbox-0.0.1/PKG-INFO
--rw-r--r--   0 rohanrao   (501) staff       (20)     1961 2023-07-25 11:41:23.000000 llmbox-0.0.1/README.md
-drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-26 05:54:27.094243 llmbox-0.0.1/llmbox/
--rw-r--r--   0 rohanrao   (501) staff       (20)        0 2023-07-25 10:46:55.000000 llmbox-0.0.1/llmbox/__init__.py
-drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-26 05:54:27.095427 llmbox-0.0.1/llmbox/llms/
--rw-r--r--   0 rohanrao   (501) staff       (20)       40 2023-07-25 11:04:41.000000 llmbox-0.0.1/llmbox/llms/__init__.py
--rw-r--r--   0 rohanrao   (501) staff       (20)      249 2023-07-23 12:21:28.000000 llmbox-0.0.1/llmbox/llms/base.py
--rw-r--r--   0 rohanrao   (501) staff       (20)      571 2023-07-25 14:04:14.000000 llmbox-0.0.1/llmbox/llms/claude2.py
-drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-26 05:54:27.094814 llmbox-0.0.1/llmbox.egg-info/
--rw-r--r--   0 rohanrao   (501) staff       (20)     2816 2023-07-26 05:54:27.000000 llmbox-0.0.1/llmbox.egg-info/PKG-INFO
--rw-r--r--   0 rohanrao   (501) staff       (20)      261 2023-07-26 05:54:27.000000 llmbox-0.0.1/llmbox.egg-info/SOURCES.txt
--rw-r--r--   0 rohanrao   (501) staff       (20)        1 2023-07-26 05:54:27.000000 llmbox-0.0.1/llmbox.egg-info/dependency_links.txt
--rw-r--r--   0 rohanrao   (501) staff       (20)       10 2023-07-26 05:54:27.000000 llmbox-0.0.1/llmbox.egg-info/requires.txt
--rw-r--r--   0 rohanrao   (501) staff       (20)        7 2023-07-26 05:54:27.000000 llmbox-0.0.1/llmbox.egg-info/top_level.txt
--rw-r--r--   0 rohanrao   (501) staff       (20)       38 2023-07-26 05:54:27.095905 llmbox-0.0.1/setup.cfg
--rw-r--r--   0 rohanrao   (501) staff       (20)     1277 2023-07-25 12:24:50.000000 llmbox-0.0.1/setup.py
+drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-31 09:14:13.535211 llmbox-0.0.2/
+-rw-r--r--   0 rohanrao   (501) staff       (20)    11357 2023-07-12 12:10:08.000000 llmbox-0.0.2/LICENSE
+-rw-r--r--   0 rohanrao   (501) staff       (20)     2816 2023-07-31 09:14:13.535093 llmbox-0.0.2/PKG-INFO
+-rw-r--r--   0 rohanrao   (501) staff       (20)     1961 2023-07-25 11:41:23.000000 llmbox-0.0.2/README.md
+drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-31 09:14:13.532865 llmbox-0.0.2/llmbox/
+-rw-r--r--   0 rohanrao   (501) staff       (20)        0 2023-07-25 10:46:55.000000 llmbox-0.0.2/llmbox/__init__.py
+drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-31 09:14:13.533811 llmbox-0.0.2/llmbox/chat/
+-rw-r--r--   0 rohanrao   (501) staff       (20)       49 2023-07-31 08:59:13.000000 llmbox-0.0.2/llmbox/chat/__init__.py
+-rw-r--r--   0 rohanrao   (501) staff       (20)      497 2023-07-31 09:07:49.000000 llmbox-0.0.2/llmbox/chat/chat.py
+drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-31 09:14:13.534735 llmbox-0.0.2/llmbox/llms/
+-rw-r--r--   0 rohanrao   (501) staff       (20)       40 2023-07-25 11:04:41.000000 llmbox-0.0.2/llmbox/llms/__init__.py
+-rw-r--r--   0 rohanrao   (501) staff       (20)      249 2023-07-23 12:21:28.000000 llmbox-0.0.2/llmbox/llms/base.py
+-rw-r--r--   0 rohanrao   (501) staff       (20)      563 2023-07-28 09:29:21.000000 llmbox-0.0.2/llmbox/llms/claude2.py
+drwxr-xr-x   0 rohanrao   (501) staff       (20)        0 2023-07-31 09:14:13.533411 llmbox-0.0.2/llmbox.egg-info/
+-rw-r--r--   0 rohanrao   (501) staff       (20)     2816 2023-07-31 09:14:13.000000 llmbox-0.0.2/llmbox.egg-info/PKG-INFO
+-rw-r--r--   0 rohanrao   (501) staff       (20)      305 2023-07-31 09:14:13.000000 llmbox-0.0.2/llmbox.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanrao   (501) staff       (20)        1 2023-07-31 09:14:13.000000 llmbox-0.0.2/llmbox.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanrao   (501) staff       (20)       10 2023-07-31 09:14:13.000000 llmbox-0.0.2/llmbox.egg-info/requires.txt
+-rw-r--r--   0 rohanrao   (501) staff       (20)        7 2023-07-31 09:14:13.000000 llmbox-0.0.2/llmbox.egg-info/top_level.txt
+-rw-r--r--   0 rohanrao   (501) staff       (20)       38 2023-07-31 09:14:13.535249 llmbox-0.0.2/setup.cfg
+-rw-r--r--   0 rohanrao   (501) staff       (20)     1217 2023-07-28 09:30:03.000000 llmbox-0.0.2/setup.py
```

### Comparing `llmbox-0.0.1/LICENSE` & `llmbox-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llmbox-0.0.1/PKG-INFO` & `llmbox-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: LLMs at your service
 Home-page: https://github.com/victorycrest/llmbox
 Author: Victory Crest
 Author-email: victorycrest1602@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/victorycrest/llmbox
 Project-URL: Tracker, https://github.com/victorycrest/llmbox/issues
```

### Comparing `llmbox-0.0.1/README.md` & `llmbox-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `llmbox-0.0.1/llmbox/llms/claude2.py` & `llmbox-0.0.2/llmbox/llms/claude2.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 class Claude2(BaseLLM):
     def __init__(self, auth_token: str | None = None, api_key: str | None = None):
         super().__init__(author=LLMAuthor.ANTHROPIC)
         self._anthropic = Anthropic(auth_token=auth_token, api_key=api_key)
 
     def generate(self, prompt: str, max_tokens_to_sample: int = 1000):
         return self._anthropic.completions.create(
-            max_tokens_to_sample=max_tokens_to_sample,
+            prompt=prompt,
             model='claude-2',
-            prompt=prompt
-        ).completion.strip()
+            max_tokens_to_sample=max_tokens_to_sample
+        ).completion
```

### Comparing `llmbox-0.0.1/llmbox.egg-info/PKG-INFO` & `llmbox-0.0.2/llmbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmbox
-Version: 0.0.1
+Version: 0.0.2
 Summary: LLMs at your service
 Home-page: https://github.com/victorycrest/llmbox
 Author: Victory Crest
 Author-email: victorycrest1602@gmail.com
 License: Apache License, Version 2.0
 Project-URL: Source, https://github.com/victorycrest/llmbox
 Project-URL: Tracker, https://github.com/victorycrest/llmbox/issues
```

### Comparing `llmbox-0.0.1/setup.py` & `llmbox-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import setuptools
 
-with open('VERSION.txt', 'r') as f:
-    version = f.read()
-
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='llmbox',
-    version=version,
+    version='0.0.2',
     author='Victory Crest',
     author_email='victorycrest1602@gmail.com',
     description='LLMs at your service',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/victorycrest/llmbox',
     project_urls={
```

