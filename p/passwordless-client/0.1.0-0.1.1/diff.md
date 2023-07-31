# Comparing `tmp/passwordless-client-0.1.0.tar.gz` & `tmp/passwordless-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passwordless-client-0.1.0.tar", last modified: Mon Jul 31 17:10:01 2023, max compression
+gzip compressed data, was "passwordless-client-0.1.1.tar", last modified: Mon Jul 31 17:47:15 2023, max compression
```

## Comparing `passwordless-client-0.1.0.tar` & `passwordless-client-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:10:01.302963 passwordless-client-0.1.0/
--rw-rw-rw-   0        0        0     1125 2023-07-31 17:10:01.302457 passwordless-client-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      459 2023-07-31 20:43:44.000000 passwordless-client-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 17:10:01.299917 passwordless-client-0.1.0/passwordless/
--rw-rw-rw-   0        0        0        0 2023-07-31 20:43:44.000000 passwordless-client-0.1.0/passwordless/__init__.py
--rw-rw-rw-   0        0        0     1863 2023-07-31 20:43:44.000000 passwordless-client-0.1.0/passwordless/client.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:10:01.301947 passwordless-client-0.1.0/passwordless_client.egg-info/
--rw-rw-rw-   0        0        0     1125 2023-07-31 17:10:01.000000 passwordless-client-0.1.0/passwordless_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-31 17:10:01.000000 passwordless-client-0.1.0/passwordless_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:10:01.000000 passwordless-client-0.1.0/passwordless_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 17:10:01.000000 passwordless-client-0.1.0/passwordless_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 17:10:01.000000 passwordless-client-0.1.0/passwordless_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 17:10:01.302963 passwordless-client-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      847 2023-07-31 17:08:50.000000 passwordless-client-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:47:15.720495 passwordless-client-0.1.1/
+-rw-rw-rw-   0        0        0      725 2023-07-31 17:47:15.719989 passwordless-client-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2023-07-31 21:26:14.000000 passwordless-client-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:47:15.716916 passwordless-client-0.1.1/passwordless/
+-rw-rw-rw-   0        0        0       38 2023-07-31 21:26:14.000000 passwordless-client-0.1.1/passwordless/__init__.py
+-rw-rw-rw-   0        0        0     3298 2023-07-31 21:26:14.000000 passwordless-client-0.1.1/passwordless/client.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:47:15.719483 passwordless-client-0.1.1/passwordless_client.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-07-31 17:47:15.000000 passwordless-client-0.1.1/passwordless_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-31 17:47:15.000000 passwordless-client-0.1.1/passwordless_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:47:15.000000 passwordless-client-0.1.1/passwordless_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 17:47:15.000000 passwordless-client-0.1.1/passwordless_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 17:47:15.000000 passwordless-client-0.1.1/passwordless_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 17:47:15.720495 passwordless-client-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-07-31 17:46:46.000000 passwordless-client-0.1.1/setup.py
```

### Comparing `passwordless-client-0.1.0/passwordless/client.py` & `passwordless-client-0.1.1/passwordless/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+from requests.exceptions import RequestException
 
 class PasswordlessClient:
     def __init__(self, api_secret):
         self.api_secret = api_secret
         self.headers = {
             "ApiSecret": api_secret,
             "Content-Type": "application/json"
@@ -12,38 +13,66 @@
         url = "https://v4.passwordless.dev/register/token"
         data = {
             "userId": user_id,
             "username": username,
             "displayname": displayname,
             **kwargs
         }
-        response = requests.post(url, json=data, headers=self.headers)
-        return self._handle_response(response)
+        try:
+            response = requests.post(url, json=data, headers=self.headers)
+            return self._handle_response(response)
+        except RequestException as e:
+            return f"An error occurred while registering the token: {str(e)}"
 
     def signin_verify(self, token):
         url = "https://v4.passwordless.dev/signin/verify"
         data = {"token": token}
-        response = requests.post(url, json=data, headers=self.headers)
-        return self._handle_response(response)
+        try:
+            response = requests.post(url, json=data, headers=self.headers)
+            return self._handle_response(response)
+        except RequestException as e:
+            return f"An error occurred while verifying the sign-in: {str(e)}"
 
     def alias(self, user_id, aliases, hashing=True):
         url = "https://v4.passwordless.dev/alias"
         data = {"userId": user_id, "aliases": aliases, "hashing": hashing}
-        response = requests.post(url, json=data, headers=self.headers)
-        return self._handle_response(response)
+        try:
+            response = requests.post(url, json=data, headers=self.headers)
+            return self._handle_response(response)
+        except RequestException as e:
+            return f"An error occurred while adding aliases: {str(e)}"
 
     def credentials_list(self, user_id):
         url = f"https://v4.passwordless.dev/credentials/list?userId={user_id}"
-        response = requests.get(url, headers=self.headers)
-        return self._handle_response(response)
+        try:
+            response = requests.get(url, headers=self.headers)
+            return self._handle_response(response)
+        except RequestException as e:
+            return f"An error occurred while listing credentials: {str(e)}"
 
     def credentials_delete(self, credential_id):
         url = "https://v4.passwordless.dev/credentials/delete"
         data = {"credentialId": credential_id}
-        response = requests.post(url, json=data, headers=self.headers)
-        return self._handle_response(response)
+        try:
+            response = requests.post(url, json=data, headers=self.headers)
+            return self._handle_response(response)
+        except RequestException as e:
+            return f"An error occurred while deleting the credential: {str(e)}"
 
     def _handle_response(self, response):
-        if response.status_code in [200, 201]:
-            return response.json()
-        else:
-            response.raise_for_status()
+        try:
+            if response.status_code == 200:
+                return response.json()
+            elif response.status_code == 201:
+                return "Everything is OK but empty."
+            elif response.status_code == 400:
+                return "Bad request. Please check your parameters."
+            elif response.status_code == 401:
+                return "You did not identify yourself. Please check your API secret."
+            elif response.status_code == 409:
+                return "Conflict (alias is already in use)."
+            elif response.status_code == 500:
+                return "Something went very wrong on the server side."
+            else:
+                response.raise_for_status()
+        except RequestException as e:
+            return f"An error occurred while processing the request: {str(e)}"
```

### Comparing `passwordless-client-0.1.0/setup.py` & `passwordless-client-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='passwordless-client',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
-    author='Matthew Fiallos',
+    author='Your Name',
     author_email='matthew.fiallos@randstadusa.com',
     description='A client library for Passwordless.dev API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/passwordless-client',
     classifiers=[
         'Development Status :: 3 - Alpha',
```

