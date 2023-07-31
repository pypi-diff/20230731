# Comparing `tmp/evenity-0.0.6.tar.gz` & `tmp/evenity-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evenity-0.0.6.tar", last modified: Sun Jul 30 18:03:45 2023, max compression
+gzip compressed data, was "evenity-0.0.7.tar", last modified: Mon Jul 31 21:13:31 2023, max compression
```

## Comparing `evenity-0.0.6.tar` & `evenity-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-30 18:03:45.987851 evenity-0.0.6/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.6/LICENSE
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1768 2023-07-30 18:03:45.987851 evenity-0.0.6/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1313 2023-07-30 17:32:58.000000 evenity-0.0.6/README.md
--rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-07-30 18:03:13.000000 evenity-0.0.6/pyproject.toml
--rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-30 18:03:45.987851 evenity-0.0.6/setup.cfg
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-30 18:03:45.984517 evenity-0.0.6/src/
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-30 18:03:45.984517 evenity-0.0.6/src/evenity/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-30 16:47:07.000000 evenity-0.0.6/src/evenity/observable.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      594 2023-07-29 11:49:18.000000 evenity-0.0.6/src/evenity/observer.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-30 18:03:45.987851 evenity-0.0.6/src/evenity/plugins/
--rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/plugins/__init__.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1327 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/plugins/ftp.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/plugins/kafka.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/plugins/shell.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)      617 2023-07-28 23:22:35.000000 evenity-0.0.6/src/evenity/plugins/telegram.py
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.0.6/src/evenity/plugins/websocket.py
-drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-30 18:03:45.984517 evenity-0.0.6/src/evenity.egg-info/
--rw-r--r--   0 localghost  (1000) localghost  (1000)     1768 2023-07-30 18:03:45.000000 evenity-0.0.6/src/evenity.egg-info/PKG-INFO
--rw-r--r--   0 localghost  (1000) localghost  (1000)      428 2023-07-30 18:03:45.000000 evenity-0.0.6/src/evenity.egg-info/SOURCES.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-30 18:03:45.000000 evenity-0.0.6/src/evenity.egg-info/dependency_links.txt
--rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-30 18:03:45.000000 evenity-0.0.6/src/evenity.egg-info/top_level.txt
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:13:31.126475 evenity-0.0.7/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 21:02:20.000000 evenity-0.0.7/LICENSE
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 21:13:31.126475 evenity-0.0.7/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7248 2023-07-31 21:11:07.000000 evenity-0.0.7/README.md
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      532 2023-07-31 21:11:07.000000 evenity-0.0.7/pyproject.toml
+-rw-r--r--   0 localghost  (1000) localghost  (1000)       38 2023-07-31 21:13:31.126475 evenity-0.0.7/setup.cfg
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:13:31.119808 evenity-0.0.7/src/
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:13:31.119808 evenity-0.0.7/src/evenity/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.7/src/evenity/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      404 2023-07-30 16:47:07.000000 evenity-0.0.7/src/evenity/observable.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      893 2023-07-31 21:11:07.000000 evenity-0.0.7/src/evenity/observer.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:13:31.123142 evenity-0.0.7/src/evenity/plugins/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        0 2023-07-28 23:22:35.000000 evenity-0.0.7/src/evenity/plugins/__init__.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1451 2023-07-31 21:11:07.000000 evenity-0.0.7/src/evenity/plugins/ftp.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      714 2023-07-28 23:22:35.000000 evenity-0.0.7/src/evenity/plugins/kafka.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      632 2023-07-28 23:22:35.000000 evenity-0.0.7/src/evenity/plugins/shell.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      742 2023-07-31 21:11:07.000000 evenity-0.0.7/src/evenity/plugins/telegram.py
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     1741 2023-07-30 17:27:26.000000 evenity-0.0.7/src/evenity/plugins/websocket.py
+drwxr-xr-x   0 localghost  (1000) localghost  (1000)        0 2023-07-31 21:13:31.119808 evenity-0.0.7/src/evenity.egg-info/
+-rw-r--r--   0 localghost  (1000) localghost  (1000)     7703 2023-07-31 21:13:31.000000 evenity-0.0.7/src/evenity.egg-info/PKG-INFO
+-rw-r--r--   0 localghost  (1000) localghost  (1000)      428 2023-07-31 21:13:31.000000 evenity-0.0.7/src/evenity.egg-info/SOURCES.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        1 2023-07-31 21:13:31.000000 evenity-0.0.7/src/evenity.egg-info/dependency_links.txt
+-rw-r--r--   0 localghost  (1000) localghost  (1000)        8 2023-07-31 21:13:31.000000 evenity-0.0.7/src/evenity.egg-info/top_level.txt
```

### Comparing `evenity-0.0.6/pyproject.toml` & `evenity-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools>=42"]
 
 [project]
 name = "evenity"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Mario Baldi", email="mariobaldi.py@gmail.com" },
 ]
 description = "Pluggable event hooks library"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

### Comparing `evenity-0.0.6/src/evenity/plugins/ftp.py` & `evenity-0.0.7/src/evenity/plugins/ftp.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,25 +8,26 @@
     """EventDispatcher class"""
     class CustomHandler(FTPHandler):
         """CustomHandler class"""
         def on_file_received(self, file):
             """On file received"""
             self.observable.on_file_received(file)
 
-    def __init__(self, user='admin', password='12345', port=21, path='./storage'): # pylint: disable=useless-super-delegation
+    def __init__(self, host='0.0.0.0', user='admin', password='12345', port=21, path='./storage', on_file_received_event='ftp'): # pylint: disable=useless-super-delegation
         super().__init__()
+        self.on_file_received_event = on_file_received_event
         authorizer = DummyAuthorizer()
         authorizer.add_user(user, password, path, perm="elradfmwMT")
         handler = self.CustomHandler
         handler.observable = self
         handler.authorizer = authorizer
         handler.passive_ports = range(60000, 65535)
         handler.permit_foreign_addresses = True
-        self.server = FTPServer(("0.0.0.0", port), handler)
+        self.server = FTPServer((host, port), handler)
 
     def consume(self):
         """Consume the observable"""
         self.server.serve_forever()
 
     def on_file_received(self, file):
         """On file received"""
-        self.notify_observers('ftp', file)
+        self.notify_observers(self.on_file_received_event, file)
```

### Comparing `evenity-0.0.6/src/evenity/plugins/kafka.py` & `evenity-0.0.7/src/evenity/plugins/kafka.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.6/src/evenity/plugins/shell.py` & `evenity-0.0.7/src/evenity/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `evenity-0.0.6/src/evenity/plugins/telegram.py` & `evenity-0.0.7/src/evenity/plugins/telegram.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import telepot
 from telepot.loop import MessageLoop
 from ..observable import Observable
 
 class AsyncTelegramaObservableConsumer(Observable):
     """EventDispatcher class"""
 
-    def __init__(self, token): # pylint: disable=useless-super-delegation
+    def __init__(self, token, on_message_received_event='telegram'): # pylint: disable=useless-super-delegation
         super().__init__()
+        self.on_message_received_event = on_message_received_event
         self.bot = telepot.Bot(token)
 
     def consume(self):
         """Consume the observable"""
         MessageLoop(self.bot, self.telegram_handler).run_as_thread()
 
     def telegram_handler(self, message):
         """Telegram handler"""
-        self.notify_observers('telegram', message)
+        self.notify_observers(self.on_message_received_event, message)
```

### Comparing `evenity-0.0.6/src/evenity/plugins/websocket.py` & `evenity-0.0.7/src/evenity/plugins/websocket.py`

 * *Files identical despite different names*

