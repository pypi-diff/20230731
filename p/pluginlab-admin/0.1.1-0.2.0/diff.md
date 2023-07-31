# Comparing `tmp/pluginlab_admin-0.1.1.tar.gz` & `tmp/pluginlab_admin-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginlab_admin-0.1.1.tar", last modified: Tue Jul 25 15:12:46 2023, max compression
+gzip compressed data, was "pluginlab_admin-0.2.0.tar", last modified: Mon Jul 31 09:31:24 2023, max compression
```

## Comparing `pluginlab_admin-0.1.1.tar` & `pluginlab_admin-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.872781 pluginlab_admin-0.1.1/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.1.1/MANIFEST.in
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-25 15:12:46.872662 pluginlab_admin-0.1.1/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     5518 2023-07-25 14:55:56.000000 pluginlab_admin-0.1.1/README.md
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.871899 pluginlab_admin-0.1.1/pluginlab_admin/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       66 2023-07-23 15:50:42.000000 pluginlab_admin-0.1.1/pluginlab_admin/__init__.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      895 2023-07-25 15:12:21.000000 pluginlab_admin-0.1.1/pluginlab_admin/app.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-25 15:11:40.000000 pluginlab_admin-0.1.1/pluginlab_admin/auth.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1646 2023-07-24 20:49:47.000000 pluginlab_admin-0.1.1/pluginlab_admin/token_verifier.py
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.1.1/pluginlab_admin/webhook.py
-drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-25 15:12:46.872471 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/PKG-INFO
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      360 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/SOURCES.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/dependency_links.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/requires.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-25 15:12:46.000000 pluginlab_admin-0.1.1/pluginlab_admin.egg-info/top_level.txt
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-25 15:12:46.872838 pluginlab_admin-0.1.1/setup.cfg
--rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-25 15:12:27.000000 pluginlab_admin-0.1.1/setup.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-31 09:31:24.359516 pluginlab_admin-0.2.0/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       18 2023-07-23 16:14:55.000000 pluginlab_admin-0.2.0/MANIFEST.in
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-31 09:31:24.359398 pluginlab_admin-0.2.0/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     5524 2023-07-25 15:58:03.000000 pluginlab_admin-0.2.0/README.md
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-31 09:31:24.358564 pluginlab_admin-0.2.0/pluginlab_admin/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       99 2023-07-31 09:28:03.000000 pluginlab_admin-0.2.0/pluginlab_admin/__init__.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1246 2023-07-31 09:28:03.000000 pluginlab_admin-0.2.0/pluginlab_admin/app.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     6337 2023-07-30 20:06:55.000000 pluginlab_admin-0.2.0/pluginlab_admin/auth.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1570 2023-07-31 09:28:03.000000 pluginlab_admin-0.2.0/pluginlab_admin/event.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)     1646 2023-07-24 20:49:47.000000 pluginlab_admin-0.2.0/pluginlab_admin/token_verifier.py
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      894 2023-07-23 13:09:00.000000 pluginlab_admin-0.2.0/pluginlab_admin/webhook.py
+drwxr-xr-x   0 aurelienbrabant   (501) staff       (20)        0 2023-07-31 09:31:24.359217 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      140 2023-07-31 09:31:24.000000 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/PKG-INFO
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      385 2023-07-31 09:31:24.000000 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)        1 2023-07-31 09:31:24.000000 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       52 2023-07-31 09:31:24.000000 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/requires.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       16 2023-07-31 09:31:24.000000 pluginlab_admin-0.2.0/pluginlab_admin.egg-info/top_level.txt
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)       38 2023-07-31 09:31:24.359555 pluginlab_admin-0.2.0/setup.cfg
+-rw-r--r--   0 aurelienbrabant   (501) staff       (20)      267 2023-07-31 09:31:19.000000 pluginlab_admin-0.2.0/setup.py
```

### Comparing `pluginlab_admin-0.1.1/README.md` & `pluginlab_admin-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 from pluginlab_admin import WebhookHeaders, Webhook
 
 webhook_secret = os.getenv('WEBHOOK_SECRET')
 webhook = Webhook(webhook_secret)
 
 @app.route('/webhook', methods=['POST'])
 def api():
-    sig = request.headers.get(WebhookHeaders.Signature)
+    sig = request.headers.get(WebhookHeaders.Signature.value)
     raw_body = request.get_data(as_text=True)
 
     if not sig:
         return jsonify({'message': 'No signature was found.'})
 
     if not webhook.is_signature_valid(raw_body, sig):
         return jsonify({'message': 'Invalid signature.'})
```

### Comparing `pluginlab_admin-0.1.1/pluginlab_admin/app.py` & `pluginlab_admin-0.2.0/pluginlab_admin/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import requests
+
+from .event import AppEvent
 from .auth import AppAuth
 
 class App:
     def __init__(
             self,
             secret_key: str,
             plugin_id: str,
             auth_url = "https://auth.pluginlab.ai",
-            auth_cert_url = "https://auth.pluginlab.ai/admin/v1/cert"
+            auth_cert_url = "https://auth.pluginlab.ai/admin/v1/cert",
+            event_url = "https://event.pluginlab.ai"
         ):
         self.plugin_id = plugin_id
         self.secret_key = secret_key
         self.auth_url = auth_url
         self.auth_cert_url = auth_cert_url
+        self.event_url = event_url
 
         s = requests.Session()
         s.headers.update({
             'X-PluginLab-Admin-Secret': self.secret_key,
             'X-PluginLab-Plugin-Id': self.plugin_id
         })
         self.client = s
@@ -26,7 +30,17 @@
                 plugin_id=self.plugin_id,
                 secret_key=self.secret_key,
                 auth_url=self.auth_url,
                 auth_cert_url=self.auth_cert_url,
                 )
 
         return auth
+
+    def get_event(self) -> AppEvent:
+        event = AppEvent(
+                plugin_id=self.plugin_id,
+                secret_key=self.secret_key,
+                event_url=self.event_url,
+        )
+
+        return event
+
```

### Comparing `pluginlab_admin-0.1.1/pluginlab_admin/auth.py` & `pluginlab_admin-0.2.0/pluginlab_admin/auth.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.1.1/pluginlab_admin/token_verifier.py` & `pluginlab_admin-0.2.0/pluginlab_admin/token_verifier.py`

 * *Files identical despite different names*

### Comparing `pluginlab_admin-0.1.1/pluginlab_admin/webhook.py` & `pluginlab_admin-0.2.0/pluginlab_admin/webhook.py`

 * *Files identical despite different names*

