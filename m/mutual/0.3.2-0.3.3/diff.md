# Comparing `tmp/mutual-0.3.2.tar.gz` & `tmp/mutual-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mutual-0.3.2.tar", last modified: Sun Jul 30 04:00:33 2023, max compression
+gzip compressed data, was "mutual-0.3.3.tar", last modified: Mon Jul 31 05:48:30 2023, max compression
```

## Comparing `mutual-0.3.2.tar` & `mutual-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.135270 mutual-0.3.2/
--rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.2/LICENSE.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-30 04:00:33.134937 mutual-0.3.2/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.2/README.md
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.133900 mutual-0.3.2/mutual/
--rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.2/mutual/APIKey.py
--rw-r--r--   0 alexbetita   (501) staff       (20)    13038 2023-07-30 03:57:23.000000 mutual-0.3.2/mutual/Bot.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4953 2023-07-29 02:49:25.000000 mutual-0.3.2/mutual/Chat.py
--rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.2/mutual/Dev.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.2/mutual/Judge.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.2/mutual/JudgeMessage.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.2/mutual/Material.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.2/mutual/Memory.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.2/mutual/Prompt.py
--rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-30 03:05:45.000000 mutual-0.3.2/mutual/__init__.py
-drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-30 04:00:33.134698 mutual-0.3.2/mutual.egg-info/
--rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/PKG-INFO
--rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/SOURCES.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/dependency_links.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/requires.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-30 04:00:33.000000 mutual-0.3.2/mutual.egg-info/top_level.txt
--rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-30 04:00:33.135333 mutual-0.3.2/setup.cfg
--rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-30 04:00:23.000000 mutual-0.3.2/setup.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.909247 mutual-0.3.3/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     1068 2023-07-14 00:38:03.000000 mutual-0.3.3/LICENSE.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-31 05:48:30.908999 mutual-0.3.3/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8420 2023-07-30 03:58:16.000000 mutual-0.3.3/README.md
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.907767 mutual-0.3.3/mutual/
+-rw-r--r--   0 alexbetita   (501) staff       (20)      977 2023-07-26 00:49:16.000000 mutual-0.3.3/mutual/APIKey.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)    13069 2023-07-31 05:46:52.000000 mutual-0.3.3/mutual/Bot.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4980 2023-07-31 05:47:35.000000 mutual-0.3.3/mutual/Chat.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)      532 2023-07-26 00:53:29.000000 mutual-0.3.3/mutual/Dev.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3308 2023-07-26 00:53:58.000000 mutual-0.3.3/mutual/Judge.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3290 2023-07-26 03:52:55.000000 mutual-0.3.3/mutual/JudgeMessage.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4103 2023-07-26 04:17:57.000000 mutual-0.3.3/mutual/Material.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     2995 2023-07-30 03:48:40.000000 mutual-0.3.3/mutual/Memory.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     3631 2023-07-26 00:55:56.000000 mutual-0.3.3/mutual/Prompt.py
+-rw-r--r--   0 alexbetita   (501) staff       (20)     4228 2023-07-31 05:05:14.000000 mutual-0.3.3/mutual/__init__.py
+drwxr-xr-x   0 alexbetita   (501) staff       (20)        0 2023-07-31 05:48:30.908772 mutual-0.3.3/mutual.egg-info/
+-rw-r--r--   0 alexbetita   (501) staff       (20)     8847 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/PKG-INFO
+-rw-r--r--   0 alexbetita   (501) staff       (20)      350 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/SOURCES.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        1 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/dependency_links.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        9 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/requires.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)        7 2023-07-31 05:48:30.000000 mutual-0.3.3/mutual.egg-info/top_level.txt
+-rw-r--r--   0 alexbetita   (501) staff       (20)       38 2023-07-31 05:48:30.909299 mutual-0.3.3/setup.cfg
+-rw-r--r--   0 alexbetita   (501) staff       (20)      727 2023-07-31 05:48:17.000000 mutual-0.3.3/setup.py
```

### Comparing `mutual-0.3.2/LICENSE.txt` & `mutual-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/PKG-INFO` & `mutual-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.3.2/README.md` & `mutual-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/APIKey.py` & `mutual-0.3.3/mutual/APIKey.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/Bot.py` & `mutual-0.3.3/mutual/Bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,14 +202,15 @@
         response = requests.post(url, data=json.dumps(data), headers=headers, stream=stream)
 
         if response.status_code < 300:
             # add the newly created bot to the bot class
             for line in response.iter_lines():
                 if line:  # filter out keep-alive new lines
                     yield line
+                    yield "\n"
             
             if flow or self.flow:
                 print("\n\n", end="", flush=True)
                 new_content = input("Please enter a new response or type exit to exit: ")
                 if new_content.strip().lower() == "exit":
                     return
                 for msg in self.chat(content=new_content, username=username, prompt=prompt,
```

### Comparing `mutual-0.3.2/mutual/Chat.py` & `mutual-0.3.3/mutual/Chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 def _create_stream(url=None, data=None, headers=None, error_logs = False):
     response = requests.post(url, data=json.dumps(data), headers=headers, stream=True)
 
     if response.status_code < 300:
         for line in response.iter_lines():
             if line:  # filter out keep-alive new lines
                 yield line
+                yield "\n"
     else:
         # raise Exception(f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail']}")
         default_stream_response['content'] = f"Request failed with status code {response.status_code}, with an Error Message: {json.loads(response.text)['detail'] or response.text}"
         return default_stream_response
     
 def _create_response(url=None, data=None, headers=None):
     response = requests.post(url, data=json.dumps(data), headers=headers)
```

### Comparing `mutual-0.3.2/mutual/Dev.py` & `mutual-0.3.3/mutual/Dev.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/Judge.py` & `mutual-0.3.3/mutual/Judge.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/JudgeMessage.py` & `mutual-0.3.3/mutual/JudgeMessage.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/Material.py` & `mutual-0.3.3/mutual/Material.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/Memory.py` & `mutual-0.3.3/mutual/Memory.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/Prompt.py` & `mutual-0.3.3/mutual/Prompt.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual/__init__.py` & `mutual-0.3.3/mutual/__init__.py`

 * *Files identical despite different names*

### Comparing `mutual-0.3.2/mutual.egg-info/PKG-INFO` & `mutual-0.3.3/mutual.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mutual
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Python client for the Mutual API.
 Home-page: https://github.com/Mutu-AI
 Author: Alex Betita
 Author-email: alexbetita25@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mutual-0.3.2/setup.py` & `mutual-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mutual',
-    version='0.3.2',  # beta
+    version='0.3.3',  # beta
     description='A Python client for the Mutual API.',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author='Alex Betita', # placeholder for now
     author_email='alexbetita25@gmail.com', # placeholder for now
     url='https://github.com/Mutu-AI',  # if you have a github repo for the package
     packages=find_packages(),
```

