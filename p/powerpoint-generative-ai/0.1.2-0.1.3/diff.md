# Comparing `tmp/powerpoint_generative_ai-0.1.2.tar.gz` & `tmp/powerpoint_generative_ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerpoint_generative_ai-0.1.2.tar", last modified: Sun Jul 30 22:33:45 2023, max compression
+gzip compressed data, was "powerpoint_generative_ai-0.1.3.tar", last modified: Sun Jul 30 22:44:38 2023, max compression
```

## Comparing `powerpoint_generative_ai-0.1.2.tar` & `powerpoint_generative_ai-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427919 powerpoint_generative_ai-0.1.2/
--rw-r--r--   0 pat        (501) staff       (20)     1064 2023-07-26 15:51:12.000000 powerpoint_generative_ai-0.1.2/LICENSE
--rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:33:45.427977 powerpoint_generative_ai-0.1.2/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)     2724 2023-07-30 22:06:24.000000 powerpoint_generative_ai-0.1.2/README.md
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427269 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/
--rw-r--r--   0 pat        (501) staff       (20)      139 2023-07-30 22:04:43.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/__init__.py
--rw-r--r--   0 pat        (501) staff       (20)     2060 2023-07-30 22:30:04.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_analyzer.py
--rw-r--r--   0 pat        (501) staff       (20)     3288 2023-07-30 22:29:51.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_generator.py
-drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:33:45.427801 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/
--rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 pat        (501) staff       (20)      395 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 pat        (501) staff       (20)        1 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 pat        (501) staff       (20)       53 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/requires.txt
--rw-r--r--   0 pat        (501) staff       (20)       25 2023-07-30 22:33:45.000000 powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/top_level.txt
--rw-r--r--   0 pat        (501) staff       (20)       79 2023-07-30 22:33:45.428154 powerpoint_generative_ai-0.1.2/setup.cfg
--rw-r--r--   0 pat        (501) staff       (20)     1168 2023-07-30 22:33:30.000000 powerpoint_generative_ai-0.1.2/setup.py
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:44:38.443482 powerpoint_generative_ai-0.1.3/
+-rw-r--r--   0 pat        (501) staff       (20)     1064 2023-07-26 15:51:12.000000 powerpoint_generative_ai-0.1.3/LICENSE
+-rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:44:38.443560 powerpoint_generative_ai-0.1.3/PKG-INFO
+-rw-r--r--   0 pat        (501) staff       (20)     2724 2023-07-30 22:06:24.000000 powerpoint_generative_ai-0.1.3/README.md
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:44:38.442656 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/
+-rw-r--r--   0 pat        (501) staff       (20)      139 2023-07-30 22:04:43.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/__init__.py
+-rw-r--r--   0 pat        (501) staff       (20)     2060 2023-07-30 22:36:39.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/ppt_analyzer.py
+-rw-r--r--   0 pat        (501) staff       (20)     3288 2023-07-30 22:29:51.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/ppt_generator.py
+drwxr-xr-x   0 pat        (501) staff       (20)        0 2023-07-30 22:44:38.443335 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/
+-rw-r--r--   0 pat        (501) staff       (20)      948 2023-07-30 22:44:38.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 pat        (501) staff       (20)      395 2023-07-30 22:44:38.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 pat        (501) staff       (20)        1 2023-07-30 22:44:38.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 pat        (501) staff       (20)       53 2023-07-30 22:44:38.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 pat        (501) staff       (20)       25 2023-07-30 22:44:38.000000 powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/top_level.txt
+-rw-r--r--   0 pat        (501) staff       (20)       79 2023-07-30 22:44:38.443753 powerpoint_generative_ai-0.1.3/setup.cfg
+-rw-r--r--   0 pat        (501) staff       (20)     1168 2023-07-30 22:44:23.000000 powerpoint_generative_ai-0.1.3/setup.py
```

### Comparing `powerpoint_generative_ai-0.1.2/LICENSE` & `powerpoint_generative_ai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.2/PKG-INFO` & `powerpoint_generative_ai-0.1.3/powerpoint_generative_ai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: powerpoint_generative_ai
-Version: 0.1.2
+Name: powerpoint-generative-ai
+Version: 0.1.3
 Summary: Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information
 Home-page: https://github.com/Width-ai/powerpoint-generative-ai
-Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.3.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: LLM,Semantic Search,PowerPoints
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `powerpoint_generative_ai-0.1.2/README.md` & `powerpoint_generative_ai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_analyzer.py` & `powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/ppt_analyzer.py`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai/ppt_generator.py` & `powerpoint_generative_ai-0.1.3/powerpoint_generative_ai/ppt_generator.py`

 * *Files identical despite different names*

### Comparing `powerpoint_generative_ai-0.1.2/powerpoint_generative_ai.egg-info/PKG-INFO` & `powerpoint_generative_ai-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: powerpoint-generative-ai
-Version: 0.1.2
+Name: powerpoint_generative_ai
+Version: 0.1.3
 Summary: Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information
 Home-page: https://github.com/Width-ai/powerpoint-generative-ai
-Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz
+Download-URL: https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.3.tar.gz
 Author: Patrick Hennis
 Author-email: patrick@width.ai
 License: MIT
 Keywords: LLM,Semantic Search,PowerPoints
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `powerpoint_generative_ai-0.1.2/setup.py` & `powerpoint_generative_ai-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from distutils.core import setup
 setup(
   name = 'powerpoint_generative_ai',
   packages = ['powerpoint_generative_ai'],
-  version = '0.1.2',
+  version = '0.1.3',
   license='MIT',
   description = 'Library written by Width.Ai. Streamlines the utilization of GPT models for automatic PowerPoint content generation. Also offers semantic searches on slide content, enabling you to quickly pinpoint relevant information',
   author = 'Patrick Hennis',
   author_email = 'patrick@width.ai',
   url = 'https://github.com/Width-ai/powerpoint-generative-ai',
-  download_url = 'https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.2.tar.gz',
+  download_url = 'https://github.com/Width-ai/powerpoint-generative-ai/archive/refs/tags/v0.1.3.tar.gz',
   keywords = ['LLM', 'Semantic Search', 'PowerPoints'],
   install_requires=[
         'langchain',
         'openai',
         'python-pptx',
         'backoff',
         'pinecone-client'
```

