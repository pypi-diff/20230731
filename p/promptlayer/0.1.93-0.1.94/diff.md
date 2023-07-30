# Comparing `tmp/promptlayer-0.1.93.tar.gz` & `tmp/promptlayer-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/promptlayer-0.1.93.tar", last modified: Tue Jul 25 19:21:24 2023, max compression
+gzip compressed data, was "dist/promptlayer-0.1.94.tar", last modified: Sun Jul 30 21:58:29 2023, max compression
```

## Comparing `promptlayer-0.1.93.tar` & `promptlayer-0.1.94.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.634178 promptlayer-0.1.93/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.93/LICENSE
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-25 19:21:24.633874 promptlayer-0.1.93/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3855 2023-07-06 14:55:00.000000 promptlayer-0.1.93/README.md
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.624714 promptlayer-0.1.93/promptlayer/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-22 17:22:46.000000 promptlayer-0.1.93/promptlayer/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.627659 promptlayer-0.1.93/promptlayer/langchain/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.93/promptlayer/langchain/__init__.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.628813 promptlayer-0.1.93/promptlayer/langchain/llms/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.93/promptlayer/langchain/llms/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.93/promptlayer/langchain/llms/openai.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3085 2023-07-11 20:32:57.000000 promptlayer-0.1.93/promptlayer/promptlayer.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.630925 promptlayer-0.1.93/promptlayer/prompts/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.93/promptlayer/prompts/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2027 2023-07-25 19:19:57.000000 promptlayer-0.1.93/promptlayer/prompts/chat.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.93/promptlayer/prompts/prompts.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.632894 promptlayer-0.1.93/promptlayer/track/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.93/promptlayer/track/__init__.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.93/promptlayer/track/track.py
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13309 2023-07-11 20:32:57.000000 promptlayer-0.1.93/promptlayer/utils.py
-drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-25 19:21:24.627314 promptlayer-0.1.93/promptlayer.egg-info/
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-25 19:21:24.000000 promptlayer-0.1.93/promptlayer.egg-info/PKG-INFO
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-07-25 19:21:24.000000 promptlayer-0.1.93/promptlayer.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-07-25 19:21:24.000000 promptlayer-0.1.93/promptlayer.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-07-25 19:21:24.000000 promptlayer-0.1.93/promptlayer.egg-info/requires.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-07-25 19:21:24.000000 promptlayer-0.1.93/promptlayer.egg-info/top_level.txt
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-07-25 19:21:24.634288 promptlayer-0.1.93/setup.cfg
--rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-07-25 19:20:04.000000 promptlayer-0.1.93/setup.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.578253 promptlayer-0.1.94/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    11357 2023-01-26 22:51:29.000000 promptlayer-0.1.94/LICENSE
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-30 21:58:29.577986 promptlayer-0.1.94/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3855 2023-07-06 14:55:00.000000 promptlayer-0.1.94/README.md
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.567182 promptlayer-0.1.94/promptlayer/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      880 2023-06-22 17:22:46.000000 promptlayer-0.1.94/promptlayer/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.569985 promptlayer-0.1.94/promptlayer/langchain/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        0 2023-02-01 20:15:14.000000 promptlayer-0.1.94/promptlayer/langchain/__init__.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.571035 promptlayer-0.1.94/promptlayer/langchain/llms/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       26 2023-02-01 20:08:36.000000 promptlayer-0.1.94/promptlayer/langchain/llms/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2012 2023-02-15 16:07:17.000000 promptlayer-0.1.94/promptlayer/langchain/llms/openai.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     3085 2023-07-11 20:32:57.000000 promptlayer-0.1.94/promptlayer/promptlayer.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.574859 promptlayer-0.1.94/promptlayer/prompts/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      124 2023-02-16 22:50:19.000000 promptlayer-0.1.94/promptlayer/prompts/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     2069 2023-07-30 21:58:04.000000 promptlayer-0.1.94/promptlayer/prompts/chat.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1700 2023-06-06 13:57:37.000000 promptlayer-0.1.94/promptlayer/prompts/prompts.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.577086 promptlayer-0.1.94/promptlayer/track/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       59 2023-03-13 20:43:03.000000 promptlayer-0.1.94/promptlayer/track/__init__.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     1239 2023-05-12 18:10:56.000000 promptlayer-0.1.94/promptlayer/track/track.py
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)    13309 2023-07-11 20:32:57.000000 promptlayer-0.1.94/promptlayer/utils.py
+drwxr-xr-x   0 jonathanpedoeem   (501) staff       (20)        0 2023-07-30 21:58:29.569387 promptlayer-0.1.94/promptlayer.egg-info/
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)     5018 2023-07-30 21:58:29.000000 promptlayer-0.1.94/promptlayer.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      530 2023-07-30 21:58:29.000000 promptlayer-0.1.94/promptlayer.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)        1 2023-07-30 21:58:29.000000 promptlayer-0.1.94/promptlayer.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       19 2023-07-30 21:58:29.000000 promptlayer-0.1.94/promptlayer.egg-info/requires.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       12 2023-07-30 21:58:29.000000 promptlayer-0.1.94/promptlayer.egg-info/top_level.txt
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)       38 2023-07-30 21:58:29.578361 promptlayer-0.1.94/setup.cfg
+-rw-r--r--   0 jonathanpedoeem   (501) staff       (20)      837 2023-07-30 21:58:11.000000 promptlayer-0.1.94/setup.py
```

### Comparing `promptlayer-0.1.93/LICENSE` & `promptlayer-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/PKG-INFO` & `promptlayer-0.1.94/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.93
+Version: 0.1.94
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.93 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.94 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.93/README.md` & `promptlayer-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/__init__.py` & `promptlayer-0.1.94/promptlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/langchain/llms/openai.py` & `promptlayer-0.1.94/promptlayer/langchain/llms/openai.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/promptlayer.py` & `promptlayer-0.1.94/promptlayer/promptlayer.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/prompts/chat.py` & `promptlayer-0.1.94/promptlayer/prompts/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             elif role == ROLE_ASSISTANT:
                 message = prompts.AIMessagePromptTemplate(prompt=prompt, **message)
             elif role == ROLE_USER:
                 message = prompts.HumanMessagePromptTemplate(prompt=prompt, **message)
             messages.append(message)
         prompt_template = prompts.ChatPromptTemplate(
             messages=messages,
-            input_variables=prompt_dict_copy.pop("input_variables"),
-            output_parser=prompt_dict_copy.pop("output_parser"),
-            partial_variables=prompt_dict_copy.pop("partial_variables"),
+            input_variables=prompt_dict_copy.get("input_variables", []),
+            output_parser=prompt_dict_copy.get("output_parser", None),
+            partial_variables=prompt_dict_copy.get("partial_variables", {}),
         )
         return prompt_template
     except Exception as e:
-        print(e)
+        print("Unknown error occurred. ", e)
         return None
```

### Comparing `promptlayer-0.1.93/promptlayer/prompts/prompts.py` & `promptlayer-0.1.94/promptlayer/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/track/track.py` & `promptlayer-0.1.94/promptlayer/track/track.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer/utils.py` & `promptlayer-0.1.94/promptlayer/utils.py`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/promptlayer.egg-info/PKG-INFO` & `promptlayer-0.1.94/promptlayer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptlayer
-Version: 0.1.93
+Version: 0.1.94
 Summary: PromptLayer is a package to keep track of your GPT models training
 Home-page: https://www.promptlayer.com
 Author: Magniv
 Author-email: hello@magniv.io
 License: UNKNOWN
 Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: promptlayer Version: 0.1.93 Summary: PromptLayer is
+Metadata-Version: 2.1 Name: promptlayer Version: 0.1.94 Summary: PromptLayer is
 a package to keep track of your GPT models training Home-page: https://
 www.promptlayer.com Author: Magniv Author-email: hello@magniv.io License:
 UNKNOWN Project-URL: Documentation, https://magniv.notion.site/Prompt-Layer-
 Docs-db0e6f50cacf4564a6d09824ba17a629 Description:
 # ð° PromptLayer **The first platform built for prompt engineers** [Python]
                           [Docs] [Demo_with_Loom] ---
 [PromptLayer](https://promptlayer.com/) is the first platform that allows you
```

### Comparing `promptlayer-0.1.93/promptlayer.egg-info/SOURCES.txt` & `promptlayer-0.1.94/promptlayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `promptlayer-0.1.93/setup.py` & `promptlayer-0.1.94/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,12 +16,12 @@
     long_description_content_type="text/markdown",
     author="Magniv",
     author_email="hello@magniv.io",
     url="https://www.promptlayer.com",
     project_urls={
         "Documentation": "https://magniv.notion.site/Prompt-Layer-Docs-db0e6f50cacf4564a6d09824ba17a629",
     },
-    version="0.1.93",
+    version="0.1.94",
     py_modules=["promptlayer"],
     packages=find_packages(),
     install_requires=["requests", "langchain"],
 )
```

