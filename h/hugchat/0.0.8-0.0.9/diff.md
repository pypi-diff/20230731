# Comparing `tmp/hugchat-0.0.8.tar.gz` & `tmp/hugchat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.8.tar", last modified: Sat Jul  1 09:48:20 2023, max compression
+gzip compressed data, was "hugchat-0.0.9.tar", last modified: Mon Jul 31 19:05:00 2023, max compression
```

## Comparing `hugchat-0.0.8.tar` & `hugchat-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-01 09:48:20.741405 hugchat-0.0.8/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-07-01 09:43:40.000000 hugchat-0.0.8/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4417 2023-07-01 09:48:20.741405 hugchat-0.0.8/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3399 2023-07-01 09:43:40.000000 hugchat-0.0.8/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-01 09:48:20.741405 hugchat-0.0.8/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1434 2023-07-01 09:48:18.000000 hugchat-0.0.8/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-01 09:48:20.733405 hugchat-0.0.8/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-01 09:48:20.737405 hugchat-0.0.8/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-01 09:44:03.000000 hugchat-0.0.8/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3895 2023-07-01 09:43:40.000000 hugchat-0.0.8/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2023-07-01 09:43:40.000000 hugchat-0.0.8/src/hugchat/exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10711 2023-07-01 09:43:40.000000 hugchat-0.0.8/src/hugchat/hugchat.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7367 2023-07-01 09:43:40.000000 hugchat-0.0.8/src/hugchat/login.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-01 09:48:20.741405 hugchat-0.0.8/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4417 2023-07-01 09:48:20.000000 hugchat-0.0.8/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      313 2023-07-01 09:48:20.000000 hugchat-0.0.8/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-01 09:48:20.000000 hugchat-0.0.8/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-07-01 09:48:20.000000 hugchat-0.0.8/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-07-01 09:48:20.000000 hugchat-0.0.8/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 19:05:00.676207 hugchat-0.0.9/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-07-31 17:16:09.000000 hugchat-0.0.9/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4459 2023-07-31 19:05:00.676207 hugchat-0.0.9/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3441 2023-07-31 17:16:09.000000 hugchat-0.0.9/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-31 19:05:00.676207 hugchat-0.0.9/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1434 2023-07-31 19:04:41.000000 hugchat-0.0.9/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 19:05:00.668207 hugchat-0.0.9/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 19:05:00.672207 hugchat-0.0.9/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-07-31 17:16:29.000000 hugchat-0.0.9/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3895 2023-07-31 17:16:09.000000 hugchat-0.0.9/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      876 2023-07-31 17:16:09.000000 hugchat-0.0.9/src/hugchat/exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13825 2023-07-31 19:03:21.000000 hugchat-0.0.9/src/hugchat/hugchat.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7367 2023-07-31 17:16:09.000000 hugchat-0.0.9/src/hugchat/login.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 19:05:00.676207 hugchat-0.0.9/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4459 2023-07-31 19:05:00.000000 hugchat-0.0.9/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      351 2023-07-31 19:05:00.000000 hugchat-0.0.9/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 19:05:00.000000 hugchat-0.0.9/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       27 2023-07-31 19:05:00.000000 hugchat-0.0.9/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       20 2023-07-31 19:05:00.000000 hugchat-0.0.9/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 19:05:00.676207 hugchat-0.0.9/src/usercookies/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      192 2023-07-31 17:55:15.000000 hugchat-0.0.9/src/usercookies/905617992@qq.com.json
```

### Comparing `hugchat-0.0.8/LICENSE` & `hugchat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.8/PKG-INFO` & `hugchat-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,19 +51,19 @@
 
 ```python
 from hugchat.login import Login
 
 # login
 sign = Login(email, passwd)
 cookies = sign.login()
-sign.saveCookies()
+sign.saveCookiesToDir(cookie_path_dir)
 
 # load cookies from usercookies/<email>.json
 sign = login(email, None)
-cookies = sign.loadCookies() # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
+cookies = sign.loadCookiesFromDir(cookie_path_dir) # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
 ```
 
 ## Usage
 
 ### Basic mode
 
 ```bash
```

### Comparing `hugchat-0.0.8/README.md` & `hugchat-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 
 ```python
 from hugchat.login import Login
 
 # login
 sign = Login(email, passwd)
 cookies = sign.login()
-sign.saveCookies()
+sign.saveCookiesToDir(cookie_path_dir)
 
 # load cookies from usercookies/<email>.json
 sign = login(email, None)
-cookies = sign.loadCookies() # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
+cookies = sign.loadCookiesFromDir(cookie_path_dir) # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
 ```
 
 ## Usage
 
 ### Basic mode
 
 ```bash
```

### Comparing `hugchat-0.0.8/setup.py` & `hugchat-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.8",
+    version="0.0.9",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.8/src/hugchat/cli.py` & `hugchat-0.0.9/src/hugchat/cli.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.8/src/hugchat/exceptions.py` & `hugchat-0.0.9/src/hugchat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.8/src/hugchat/login.py` & `hugchat-0.0.9/src/hugchat/login.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.8/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.9/src/hugchat.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -51,19 +51,19 @@
 
 ```python
 from hugchat.login import Login
 
 # login
 sign = Login(email, passwd)
 cookies = sign.login()
-sign.saveCookies()
+sign.saveCookiesToDir(cookie_path_dir)
 
 # load cookies from usercookies/<email>.json
 sign = login(email, None)
-cookies = sign.loadCookies() # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
+cookies = sign.loadCookiesFromDir(cookie_path_dir) # This will detect if the JSON file exists, return cookies if it does and raise an Exception if it's not.
 ```
 
 ## Usage
 
 ### Basic mode
 
 ```bash
```

