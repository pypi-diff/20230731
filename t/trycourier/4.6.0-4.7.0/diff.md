# Comparing `tmp/trycourier-4.6.0.tar.gz` & `tmp/trycourier-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trycourier-4.6.0.tar", last modified: Mon Jul 24 18:18:14 2023, max compression
+gzip compressed data, was "trycourier-4.7.0.tar", last modified: Mon Jul 31 19:13:42 2023, max compression
```

## Comparing `trycourier-4.6.0.tar` & `trycourier-4.7.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.342455 trycourier-4.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-24 18:17:55.000000 trycourier-4.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-24 18:18:14.342455 trycourier-4.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-24 18:17:55.000000 trycourier-4.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:18:14.342455 trycourier-4.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-24 18:17:55.000000 trycourier-4.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.334454 trycourier-4.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-24 18:17:55.000000 trycourier-4.6.0/tests/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.338454 trycourier-4.6.0/trycourier/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/audiences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/audit_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/automations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-24 18:17:55.000000 trycourier-4.6.0/trycourier/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:18:14.338454 trycourier-4.6.0/trycourier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-24 18:18:14.000000 trycourier-4.6.0/trycourier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:42.501547 trycourier-4.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-31 19:13:29.000000 trycourier-4.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-31 19:13:42.501547 trycourier-4.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-31 19:13:29.000000 trycourier-4.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:13:42.501547 trycourier-4.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-31 19:13:29.000000 trycourier-4.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:42.501547 trycourier-4.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-31 19:13:29.000000 trycourier-4.7.0/tests/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:42.501547 trycourier-4.7.0/trycourier/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/audiences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/audit_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/automations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17609 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-31 19:13:29.000000 trycourier-4.7.0/trycourier/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:13:42.501547 trycourier-4.7.0/trycourier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15338 2023-07-31 19:13:42.000000 trycourier-4.7.0/trycourier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-31 19:13:42.000000 trycourier-4.7.0/trycourier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:13:42.000000 trycourier-4.7.0/trycourier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 19:13:42.000000 trycourier-4.7.0/trycourier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 19:13:42.000000 trycourier-4.7.0/trycourier.egg-info/top_level.txt
```

### Comparing `trycourier-4.6.0/LICENSE` & `trycourier-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/PKG-INFO` & `trycourier-4.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.6.0
+Version: 4.7.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trycourier-4.6.0/README.md` & `trycourier-4.7.0/README.md`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/setup.py` & `trycourier-4.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="trycourier",
-    version="4.6.0",
+    version="4.7.0",
     author="Courier",
     author_email="support@courier.com",
     description="A Python Package for communicating with the Courier REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/trycourier/courier-python",
     packages=setuptools.find_packages(),
```

### Comparing `trycourier-4.6.0/tests/test_accounts.py` & `trycourier-4.7.0/tests/test_accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,31 @@
 @responses.activate
 def test_success_get_accounts():
     responses.add(
         responses.GET,
         'https://api.courier.com/accounts',
         status=200,
         content_type='application/json',
-        body='{"items":[{"id":"ACME", "name":"ACME Inc", "properties":{}, "default_preferences":{}, "user_profile":{}}], "has_more": false}'
+        body='{"items":[{"id":"ACME", "name":"ACME Inc", "properties":{}, "default_preferences":{}, "user_profile":{}}], "has_more": false, "next_url": null, "url": "/accounts"}'
     )
 
     c = Courier(auth_token='123456789ABCDF')
     r = c.accounts.get_accounts()
 
     assert r == {
       "items": [{
         "id":"ACME",
         "name":"ACME Inc",
         "properties":{},
         "default_preferences":{},
         "user_profile":{}
       }],
-      "has_more": False
+      "has_more": False,
+      "next_url": None,
+      "url": "/accounts",
     }
 
 @responses.activate
 def test_success_put_account():
     responses.add(
         responses.PUT,
         'https://api.courier.com/accounts/account-1',
```

### Comparing `trycourier-4.6.0/tests/test_audiences.py` & `trycourier-4.7.0/tests/test_audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_audit_events.py` & `trycourier-4.7.0/tests/test_audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_automations.py` & `trycourier-4.7.0/tests/test_automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_bulk.py` & `trycourier-4.7.0/tests/test_bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_client.py` & `trycourier-4.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_lists.py` & `trycourier-4.7.0/tests/test_lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_messages.py` & `trycourier-4.7.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_notifications.py` & `trycourier-4.7.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_profiles.py` & `trycourier-4.7.0/tests/test_profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/tests/test_session.py` & `trycourier-4.7.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/accounts.py` & `trycourier-4.7.0/trycourier/accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,36 +29,36 @@
         resp = self.session.get(url)
 
         if resp.status_code >= 400:
             raise CourierAPIException(resp)
 
         return resp.json()
 
-    def get_accounts(self, limit=None, starting_after=None):
+    def get_accounts(self, limit=None, cursor=None):
         """
         Lists accounts
 
         Args:
             limit: The number of accounts to return (default 20, max 100)
-            starting_after: Value of next_page from previous response
+            cursor: Value of next_page from previous response
 
         Raises:
             CourierAPIException: Any error returned by the Courier API
 
         Returns:
             dict: Contains accounts items and paging info
         """
 
         params = {}
 
         if limit:
             params['limit'] = limit
 
-        if starting_after:
-            params['starting_after'] = starting_after
+        if cursor:
+            params['cursor'] = cursor
 
         resp = self.session.get(self.uri, params=params)
 
         if resp.status_code >= 400:
             raise CourierAPIException(resp)
 
         return resp.json()
```

### Comparing `trycourier-4.6.0/trycourier/audiences.py` & `trycourier-4.7.0/trycourier/audiences.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/audit_events.py` & `trycourier-4.7.0/trycourier/audit_events.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/automations.py` & `trycourier-4.7.0/trycourier/automations.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/bulk.py` & `trycourier-4.7.0/trycourier/bulk.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/client.py` & `trycourier-4.7.0/trycourier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .exceptions import CourierAPIException
 from .session import CourierAPISession
 from .lists import Lists
 from .messages import Messages
 from .notifications import Notifications
 from .profiles import Profiles
 
-__version__ = '4.6.0'
+__version__ = '4.7.0'
 
 
 class Courier(object):
 
     def __init__(self,
                  base_url=None,
                  auth_token=None,
```

### Comparing `trycourier-4.6.0/trycourier/lists.py` & `trycourier-4.7.0/trycourier/lists.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/messages.py` & `trycourier-4.7.0/trycourier/messages.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/notifications.py` & `trycourier-4.7.0/trycourier/notifications.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/profiles.py` & `trycourier-4.7.0/trycourier/profiles.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier/session.py` & `trycourier-4.7.0/trycourier/session.py`

 * *Files identical despite different names*

### Comparing `trycourier-4.6.0/trycourier.egg-info/PKG-INFO` & `trycourier-4.7.0/trycourier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trycourier
-Version: 4.6.0
+Version: 4.7.0
 Summary: A Python Package for communicating with the Courier REST API.
 Home-page: https://github.com/trycourier/courier-python
 Author: Courier
 Author-email: support@courier.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trycourier-4.6.0/trycourier.egg-info/SOURCES.txt` & `trycourier-4.7.0/trycourier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

