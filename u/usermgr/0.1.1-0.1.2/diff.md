# Comparing `tmp/usermgr-0.1.1.tar.gz` & `tmp/usermgr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usermgr-0.1.1.tar", max compression
+gzip compressed data, was "usermgr-0.1.2.tar", max compression
```

## Comparing `usermgr-0.1.1.tar` & `usermgr-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.1/LICENSE
--rw-r--r--   0        0        0      396 2023-06-24 11:29:36.602405 usermgr-0.1.1/README.md
--rw-r--r--   0        0        0      588 2023-07-04 23:20:06.629167 usermgr-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.1/usermgr/Factory.py
--rw-r--r--   0        0        0       22 2023-07-04 23:20:00.569171 usermgr-0.1.1/usermgr/__init__.py
--rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.1/usermgr/base.py
--rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.1/usermgr/providers/__init__.py
--rw-r--r--   0        0        0     3628 2023-07-04 23:18:10.049184 usermgr-0.1.1/usermgr/providers/cognito.py
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 usermgr-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.2/LICENSE
+-rw-r--r--   0        0        0      411 2023-07-31 06:02:25.989115 usermgr-0.1.2/README.md
+-rw-r--r--   0        0        0      588 2023-07-31 05:59:49.069134 usermgr-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.2/usermgr/Factory.py
+-rw-r--r--   0        0        0       22 2023-07-31 05:59:40.199134 usermgr-0.1.2/usermgr/__init__.py
+-rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.2/usermgr/base.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.2/usermgr/providers/__init__.py
+-rw-r--r--   0        0        0     3656 2023-07-31 05:54:04.809152 usermgr-0.1.2/usermgr/providers/cognito.py
+-rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 usermgr-0.1.2/PKG-INFO
```

### Comparing `usermgr-0.1.1/LICENSE` & `usermgr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.1/pyproject.toml` & `usermgr-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usermgr"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["tamuto <tamuto@infodb.jp>"]
 readme = "README.md"
 homepage = "https://github.com/tamuto/usermgr"
 repository = "https://github.com/tamuto/usermgr"
 
 packages = [
```

### Comparing `usermgr-0.1.1/usermgr/base.py` & `usermgr-0.1.2/usermgr/base.py`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.1/usermgr/providers/cognito.py` & `usermgr-0.1.2/usermgr/providers/cognito.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 def new_instance(**kwargs):
     return CognitoUserMgr(**kwargs)
 
 
 class CognitoUserMgr(UserManager):
 
-    def __init__(self, user_pool_id, client_id, client_secret, **kwargs):
-        self.idp = boto3.client('cognito-idp')
+    def __init__(self, region, user_pool_id, client_id, client_secret, **kwargs):
+        self.idp = boto3.client('cognito-idp', region_name=region)
         self.user_pool_id = user_pool_id
         self.client_id = client_id
         self.client_secret = client_secret
 
     def close(self):
         self.idp.close()
```

### Comparing `usermgr-0.1.1/PKG-INFO` & `usermgr-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usermgr
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/tamuto/usermgr
 Author: tamuto
 Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,15 @@
 
 ```
 AWS_ACCESS_KEY_ID=***
 AWS_SECRET_ACCESS_KEY=***
 or
 AWS_PROFILE=***
 
+AWS_REGION=***
 USER_POOL_ID=***
 CLIENT_ID=***
 CLIENT_SECRET=***
 ```
 
   * run unittest
```

