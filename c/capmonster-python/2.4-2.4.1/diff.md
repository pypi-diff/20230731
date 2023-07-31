# Comparing `tmp/capmonster_python-2.4.tar.gz` & `tmp/capmonster_python-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capmonster_python-2.4.tar", last modified: Fri Mar 10 14:01:03 2023, max compression
+gzip compressed data, was "capmonster_python-2.4.1.tar", last modified: Mon Jul 31 09:07:51 2023, max compression
```

## Comparing `capmonster_python-2.4.tar` & `capmonster_python-2.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:01:03.464862 capmonster_python-2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-10 14:00:52.000000 capmonster_python-2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-10 14:01:03.464862 capmonster_python-2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-10 14:00:52.000000 capmonster_python-2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:01:03.464862 capmonster_python-2.4/capmonster_python/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/capmonster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/compleximage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/fun_captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/geetest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/hcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/recaptcha_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/recaptcha_v2_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/recaptcha_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/turnstile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-10 14:00:52.000000 capmonster_python-2.4/capmonster_python/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 14:01:03.464862 capmonster_python-2.4/capmonster_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-10 14:01:03.000000 capmonster_python-2.4/capmonster_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-10 14:01:03.000000 capmonster_python-2.4/capmonster_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 14:01:03.000000 capmonster_python-2.4/capmonster_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 14:01:03.000000 capmonster_python-2.4/capmonster_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-10 14:01:03.000000 capmonster_python-2.4/capmonster_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-10 14:01:03.464862 capmonster_python-2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-10 14:00:52.000000 capmonster_python-2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:07:51.934020 capmonster_python-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-31 09:07:51.934020 capmonster_python-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:07:51.934020 capmonster_python-2.4.1/capmonster_python/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/capmonster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/compleximage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/fun_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/geetest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/hcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/recaptcha_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/recaptcha_v2_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/recaptcha_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/turnstile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/capmonster_python/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 09:07:51.934020 capmonster_python-2.4.1/capmonster_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-31 09:07:51.000000 capmonster_python-2.4.1/capmonster_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-31 09:07:51.000000 capmonster_python-2.4.1/capmonster_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 09:07:51.000000 capmonster_python-2.4.1/capmonster_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 09:07:51.000000 capmonster_python-2.4.1/capmonster_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-31 09:07:51.000000 capmonster_python-2.4.1/capmonster_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 09:07:51.934020 capmonster_python-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-31 09:07:36.000000 capmonster_python-2.4.1/setup.py
```

### Comparing `capmonster_python-2.4/LICENSE` & `capmonster_python-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/PKG-INFO` & `capmonster_python-2.4.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonster_python
-Version: 2.4
+Version: 2.4.1
 Summary: capmonster.cloud library for Python
 Home-page: https://github.com/alperensert/capmonster_python
 Author: Alperen Sert
 Author-email: business@alperen.io
 License: MIT
 Project-URL: Documentation, https://alperensert.github.io/capmonster_python/
 Project-URL: Source, https://github.com/alperensert/capmonster_python/
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires: requests
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Capmonster.cloud for Python
 =
@@ -85,16 +87,28 @@
 ```
 
 #### GeeTest
 
 ```python
 from capmonster_python import GeeTestTask
 
-capmonster_python = GeeTestTask("API_KEY")
-task_id = capmonster_python.create_task("website_url", "gt", "challenge")
-result= capmonster_python.join_task_result(task_id)
+capmonster = GeeTestTask("API_KEY")
+task_id = capmonster.create_task("website_url", "gt", "challenge")
+result= capmonster.join_task_result(task_id)
 print(result.get("challenge"))
 print(result.get("seccode"))
 print(result.get("validate"))
 ```
 
+#### Report incorrect captchas
+
+```python
+from capmonster_python import RecaptchaV2Task
+
+capmonster = RecaptchaV2Task("API_KEY")
+task_id = capmonster.create_task("website_url", "website_key")
+result = capmonster.join_task_result(task_id)
+report_result = capmonster.report_incorrect_captcha("token", task_id)
+print(report_result)
+```
+
 For other examples and api documentation please visit [wiki](https://alperensert.github.io/capmonster_python)
```

### Comparing `capmonster_python-2.4/README.md` & `capmonster_python-2.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -60,16 +60,28 @@
 ```
 
 #### GeeTest
 
 ```python
 from capmonster_python import GeeTestTask
 
-capmonster_python = GeeTestTask("API_KEY")
-task_id = capmonster_python.create_task("website_url", "gt", "challenge")
-result= capmonster_python.join_task_result(task_id)
+capmonster = GeeTestTask("API_KEY")
+task_id = capmonster.create_task("website_url", "gt", "challenge")
+result= capmonster.join_task_result(task_id)
 print(result.get("challenge"))
 print(result.get("seccode"))
 print(result.get("validate"))
 ```
 
+#### Report incorrect captchas
+
+```python
+from capmonster_python import RecaptchaV2Task
+
+capmonster = RecaptchaV2Task("API_KEY")
+task_id = capmonster.create_task("website_url", "website_key")
+result = capmonster.join_task_result(task_id)
+report_result = capmonster.report_incorrect_captcha("token", task_id)
+print(report_result)
+```
+
 For other examples and api documentation please visit [wiki](https://alperensert.github.io/capmonster_python)
```

### Comparing `capmonster_python-2.4/capmonster_python/capmonster.py` & `capmonster_python-2.4.1/capmonster_python/capmonster.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 class Capmonster:
     __SOFT_ID = 30
     _HOST_URL = "https://api.capmonster.cloud"
     _CREATE_TASK_URL = "/createTask"
     _TASK_RESULT_URL = "/getTaskResult"
     _BALANCE_URL = "/getBalance"
+    _INCORRECT_IMAGE_CAPTCHA_URL = "/reportIncorrectImageCaptcha"
+    _INCORRECT_TOKEN_CAPTCHA_URL = "/reportIncorrectTokenCaptcha"
 
     def __init__(self, client_key):
         self._client_key = client_key
 
     def get_balance(self):
         data = {"clientKey": self._client_key}
         return self._make_request("getBalance", data).get("balance")
@@ -34,25 +36,50 @@
         for i in range(0, maximum_time + 1, 2):
             result = self.get_task_result(task_id)
             if result is not False and result is not None:
                 return result
             elif result is False:
                 i += 1
                 sleep(2)
-        raise CapmonsterException(61, "ERROR_MAXIMUM_TIME_EXCEED", "Maximum time is exceed.")
+        raise CapmonsterException(
+            61, "ERROR_MAXIMUM_TIME_EXCEED", "Maximum time is exceed.")
 
     async def join_task_result_async(self, task_id: int, maximum_time: int = 120):
         for i in range(0, maximum_time + 1, 2):
             result = self.get_task_result(task_id)
             if result is not False and result is not None:
                 return result
             elif result is False:
                 i += 1
                 await asyncio.sleep(2)
-        raise CapmonsterException(61, "ERROR_MAXIMUM_TIME_EXCEED", "Maximum time is exceed.")
+        raise CapmonsterException(
+            61, "ERROR_MAXIMUM_TIME_EXCEED", "Maximum time is exceed.")
+
+    def report_incorrect_captcha(self, captcha_type: str, task_id: int) -> bool:
+        if captcha_type is not "image" or "token":
+            raise CapmonsterException(
+                1, "ERROR_INCORRECT_CAPTCHA_TYPE", "Valid captcha_type parameters are only 'image' or 'token'.")
+        try:
+            self._report_incorrect_captcha(
+                captcha_type=captcha_type, task_id=task_id)
+            return True
+        except:
+            return False
+
+    @check_response()
+    def _report_incorrect_captcha(self, captcha_type: str, task_id: int):
+        data = {
+            "clientKey": self._client_key,
+            "taskId": task_id
+        }
+        if captcha_type is "image":
+            response = self._make_request("reportIncorrectImageCaptcha", data)
+        else:
+            response = self._make_request("reportIncorrectTokenCaptcha", data)
+        return response
 
     @staticmethod
     def _is_ready(response: dict):
         status = response.get("status")
         if status == "processing":
             return False
         elif status == "ready":
@@ -64,16 +91,21 @@
         if method == "getBalance":
             _method = self._BALANCE_URL
         elif method == "getTaskResult":
             _method = self._TASK_RESULT_URL
         elif method == "createTask":
             _method = self._CREATE_TASK_URL
             data["softId"] = self.__SOFT_ID
+        elif method == "reportIncorrectImageCaptcha":
+            _method = self._INCORRECT_IMAGE_CAPTCHA_URL
+        elif method == "reportIncorrectTokenCaptcha":
+            _method = self._INCORRECT_TOKEN_CAPTCHA_URL
         try:
-            response = requests.post("{}{}".format(self._HOST_URL, _method), json=data).json()
+            response = requests.post("{}{}".format(
+                self._HOST_URL, _method), json=data).json()
         except Exception as err:
             raise CapmonsterException(-1, type(err).__name__, str(err))
         return response
 
     @staticmethod
     def _add_cookies(cookies, data):
         if cookies is None:
@@ -84,15 +116,16 @@
                 if value == list(cookies.items())[-1][1]:
                     str_cookies += "{}={}".format(key, value)
                 else:
                     str_cookies += "{}={};".format(key, value)
         elif type(cookies) == list:
             for i in cookies:
                 if not len(cookies) % 2 == 0:
-                    raise AttributeError("List cookies length must be even numbers")
+                    raise AttributeError(
+                        "List cookies length must be even numbers")
                 if cookies.index(i) % 2 == 0:
                     str_cookies += "{}=".format(i)
                 elif cookies[cookies.index(i)] == cookies[-1]:
                     str_cookies += "{}".format(i)
                 elif cookies.index(i) % 2 == 1:
                     str_cookies += "{};".format(i)
         elif type(cookies) == str:
```

### Comparing `capmonster_python-2.4/capmonster_python/compleximage.py` & `capmonster_python-2.4.1/capmonster_python/compleximage.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/fun_captcha.py` & `capmonster_python-2.4.1/capmonster_python/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/geetest.py` & `capmonster_python-2.4.1/capmonster_python/geetest.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/hcaptcha.py` & `capmonster_python-2.4.1/capmonster_python/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/image_to_text.py` & `capmonster_python-2.4.1/capmonster_python/image_to_text.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/recaptcha_v2.py` & `capmonster_python-2.4.1/capmonster_python/recaptcha_v2.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/recaptcha_v2_enterprise.py` & `capmonster_python-2.4.1/capmonster_python/recaptcha_v2_enterprise.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/recaptcha_v3.py` & `capmonster_python-2.4.1/capmonster_python/recaptcha_v3.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/turnstile.py` & `capmonster_python-2.4.1/capmonster_python/turnstile.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python/utils.py` & `capmonster_python-2.4.1/capmonster_python/utils.py`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/capmonster_python.egg-info/PKG-INFO` & `capmonster_python-2.4.1/capmonster_python.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capmonster-python
-Version: 2.4
+Version: 2.4.1
 Summary: capmonster.cloud library for Python
 Home-page: https://github.com/alperensert/capmonster_python
 Author: Alperen Sert
 Author-email: business@alperen.io
 License: MIT
 Project-URL: Documentation, https://alperensert.github.io/capmonster_python/
 Project-URL: Source, https://github.com/alperensert/capmonster_python/
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires: requests
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Capmonster.cloud for Python
 =
@@ -85,16 +87,28 @@
 ```
 
 #### GeeTest
 
 ```python
 from capmonster_python import GeeTestTask
 
-capmonster_python = GeeTestTask("API_KEY")
-task_id = capmonster_python.create_task("website_url", "gt", "challenge")
-result= capmonster_python.join_task_result(task_id)
+capmonster = GeeTestTask("API_KEY")
+task_id = capmonster.create_task("website_url", "gt", "challenge")
+result= capmonster.join_task_result(task_id)
 print(result.get("challenge"))
 print(result.get("seccode"))
 print(result.get("validate"))
 ```
 
+#### Report incorrect captchas
+
+```python
+from capmonster_python import RecaptchaV2Task
+
+capmonster = RecaptchaV2Task("API_KEY")
+task_id = capmonster.create_task("website_url", "website_key")
+result = capmonster.join_task_result(task_id)
+report_result = capmonster.report_incorrect_captcha("token", task_id)
+print(report_result)
+```
+
 For other examples and api documentation please visit [wiki](https://alperensert.github.io/capmonster_python)
```

### Comparing `capmonster_python-2.4/capmonster_python.egg-info/SOURCES.txt` & `capmonster_python-2.4.1/capmonster_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capmonster_python-2.4/setup.py` & `capmonster_python-2.4.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="capmonster_python",
-    version="2.4",
+    version="2.4.1",
     packages=["capmonster_python"],
     url="https://github.com/alperensert/capmonster_python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Alperen Sert",
     author_email="business@alperen.io",
@@ -23,18 +23,20 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     use_scm_version=True,
     setup_requires=["setuptools_scm", "wheel"],
     install_requires=["requests", "six"],
     python_requires=">=3",
     project_urls={
         "Documentation": 'https://alperensert.github.io/capmonster_python/',
         "Source": 'https://github.com/alperensert/capmonster_python/',
         "Tracker": 'https://github.com/alperensert/capmonster_python/issues',
     },
-)
+)
```

