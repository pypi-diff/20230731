# Comparing `tmp/lollms-2.2.0.tar.gz` & `tmp/lollms-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.0.tar", last modified: Sat Jul 29 00:02:05 2023, max compression
+gzip compressed data, was "lollms-2.2.1.tar", last modified: Mon Jul 31 01:12:21 2023, max compression
```

## Comparing `lollms-2.2.0.tar` & `lollms-2.2.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.087629 lollms-2.2.0/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.0/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-07-29 00:02:05.086628 lollms-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:04.994111 lollms-2.2.0/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.0/lollms/__init__.py
--rw-rw-rw-   0        0        0     9007 2023-07-23 16:01:43.000000 lollms-2.2.0/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.019631 lollms-2.2.0/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.0/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.020629 lollms-2.2.0/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.021630 lollms-2.2.0/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.072629 lollms-2.2.0/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.073630 lollms-2.2.0/lollms/apps/server/
--rw-rw-rw-   0        0        0    34728 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.075628 lollms-2.2.0/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7681 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.076630 lollms-2.2.0/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.0/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.0/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.0/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.084629 lollms-2.2.0/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.0/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.0/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.0/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.0/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.0/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.0/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.0/lollms/paths.py
--rw-rw-rw-   0        0        0    49264 2023-07-29 00:01:26.000000 lollms-2.2.0/lollms/personality.py
--rw-rw-rw-   0        0        0    21967 2023-07-19 17:04:35.000000 lollms-2.2.0/lollms/terminal.py
--rw-rw-rw-   0        0        0     2539 2023-07-29 00:00:49.000000 lollms-2.2.0/lollms/types.py
--rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.0/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-29 00:02:05.017630 lollms-2.2.0/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-29 00:02:04.000000 lollms-2.2.0/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 00:02:05.087629 lollms-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-07-29 00:01:36.000000 lollms-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.099380 lollms-2.2.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.1/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-31 01:12:21.098381 lollms-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.060347 lollms-2.2.1/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.1/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9349 2023-07-30 22:50:46.000000 lollms-2.2.1/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.078546 lollms-2.2.1/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.1/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.079546 lollms-2.2.1/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.080548 lollms-2.2.1/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.090672 lollms-2.2.1/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.091717 lollms-2.2.1/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34728 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.093720 lollms-2.2.1/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7681 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.094716 lollms-2.2.1/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.1/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.1/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.097380 lollms-2.2.1/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.1/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.1/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.1/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.1/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.1/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.1/lollms/paths.py
+-rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.1/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.1/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.1/lollms/types.py
+-rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.1/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.077547 lollms-2.2.1/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 01:12:21.100379 lollms-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-30 23:44:34.000000 lollms-2.2.1/setup.py
```

### Comparing `lollms-2.2.0/LICENSE` & `lollms-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/PKG-INFO` & `lollms-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.0/README.md` & `lollms-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/app.py` & `lollms-2.2.1/lollms/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,33 @@
 from lollms.config import InstallOption
 from lollms.helpers import trace_exception
 from lollms.terminal import MainMenu
 
 import subprocess
 
 class LollmsApplication:
-    def __init__(self, app_name:str, config:LOLLMSConfig, lollms_paths:LollmsPaths, load_binding=True, load_model=True, try_select_binding=False, try_select_model=False) -> None:
+    def __init__(
+                    self, 
+                    app_name:str, 
+                    config:LOLLMSConfig, 
+                    lollms_paths:LollmsPaths, 
+                    load_binding=True, 
+                    load_model=True, 
+                    try_select_binding=False, 
+                    try_select_model=False,
+                    callback=None
+                ) -> None:
         """
         Creates a LOLLMS Application
         """
         self.app_name               = app_name
         self.config                 = config
         self.lollms_paths           = lollms_paths
 
-        self.menu                   = MainMenu(self)
+        self.menu                   = MainMenu(self, callback)
         self.mounted_personalities  = []
         self.personality            = None
 
         self.binding=None
         self.model=None
 
         try:
@@ -101,17 +111,17 @@
             ASCIIColors.error(f"{self.config.get_model_path_infos()}")
             print("Please select a valid model or install a new one from a url")
             model = None
 
         return model
 
 
-    def mount_personality(self, id:int):
+    def mount_personality(self, id:int, callback=None):
         try:
-            personality = PersonalityBuilder(self.lollms_paths, self.config, self.model).build_personality(id)
+            personality = PersonalityBuilder(self.lollms_paths, self.config, self.model, callback=callback).build_personality(id)
             if personality.model is not None:
                 self.cond_tk = personality.model.tokenize(personality.personality_conditioning)
                 self.n_cond_tk = len(self.cond_tk)
                 ASCIIColors.success(f"Personality  {personality.name} mounted successfully")
             else:
                 ASCIIColors.success(f"Personality  {personality.name} mounted successfully but no model is selected")
 
@@ -123,19 +133,19 @@
             if id == self.config.active_personality_id:
                 self.config.active_personality_id=len(self.config.personalities)-1
             personality = None
         
         self.mounted_personalities.append(personality)
         return personality
     
-    def mount_personalities(self):
+    def mount_personalities(self, callback = None):
         self.mounted_personalities = []
         to_remove = []
         for i in range(len(self.config["personalities"])):
-            p = self.mount_personality(i)
+            p = self.mount_personality(i, callback = None)
             if p is None:
                 to_remove.append(i)
         to_remove.sort(reverse=True)
         for i in to_remove:
             self.unmount_personality(i)
 
         self.personality = self.mounted_personalities[self.config.active_personality_id]
@@ -160,17 +170,17 @@
             self.personality = self.mount_personalities[id]
             self.config.save_config()
             return True
         else:
             return False
 
 
-    def load_personality(self):
+    def load_personality(self, callback=None):
         try:
-            personality = PersonalityBuilder(self.lollms_paths, self.config, self.model).build_personality()
+            personality = PersonalityBuilder(self.lollms_paths, self.config, self.model, callback=callback).build_personality()
         except Exception as ex:
             ASCIIColors.error(f"Couldn't load personality. Please verify your configuration file at {self.configuration_path} or use the next menu to select a valid personality")
             ASCIIColors.error(f"Binding returned this exception : {ex}")
             ASCIIColors.error(f"{self.config.get_personality_path_infos()}")
             print("Please select a valid model or install a new one from a url")
             personality = None
         return personality
```

### Comparing `lollms-2.2.0/lollms/apps/console/__init__.py` & `lollms-2.2.1/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/playground/static/LICENSE` & `lollms-2.2.1/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/playground/static/README.md` & `lollms-2.2.1/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/playground/static/index.html` & `lollms-2.2.1/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/playground/static/logo.png` & `lollms-2.2.1/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.2.1/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/server/__init__.py` & `lollms-2.2.1/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/apps/settings/__init__.py` & `lollms-2.2.1/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/assets/logo.png` & `lollms-2.2.1/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/binding.py` & `lollms-2.2.1/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/config.py` & `lollms-2.2.1/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/configs/config.yaml` & `lollms-2.2.1/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/data.py` & `lollms-2.2.1/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/extension.py` & `lollms-2.2.1/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/helpers.py` & `lollms-2.2.1/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/langchain_integration.py` & `lollms-2.2.1/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/main_config.py` & `lollms-2.2.1/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/paths.py` & `lollms-2.2.1/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms/personality.py` & `lollms-2.2.1/lollms/personality.py`

 * *Files 2% similar despite different names*

```diff
@@ -991,15 +991,17 @@
             ASCIIColors.warning("Couldn't find Cuda build tools on your PC. Reverting to CPU.")
             result = subprocess.run(["pip", "install", "--upgrade", "torch", "torchvision", "torchaudio", "--no-cache-dir"])
             if result.returncode != 0:
                 ASCIIColors.error("Couldn't install pytorch !!")
             else:
                 ASCIIColors.error("Pytorch installed successfully!!")
 
-    def add_file(self, path):
+    def add_file(self, path, callback=None):
+        if callback is not None:
+            callback("File added successfully",MSG_TYPE.MSG_TYPE_INFO)
         self.files.append(path)
         return True
 
     def remove_file(self, path):
         self.files.remove(path)
 
     def load_config_file(self, path, default_config=None):
@@ -1277,26 +1279,39 @@
         """
         if not callback and self.callback:
             callback = self.callback
 
         if callback:
             callback(step_text, MSG_TYPE.MSG_TYPE_STEP_PROGRESS, {'progress':progress})
 
-    def new_message(self, step_text:str, message_type:MSG_TYPE, callback: Callable[[str, int, dict], bool]=None):
+    def new_message(self, message_text:str, message_type:MSG_TYPE, callback: Callable[[str, int, dict], bool]=None):
         """This sends step rogress to front end
 
         Args:
             step_text (dict): The step progress in %
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
         """
         if not callback and self.callback:
             callback = self.callback
 
         if callback:
-            callback(step_text, MSG_TYPE.MSG_TYPE_NEW_MESSAGE, {'type':message_type})
+            callback(message_text, MSG_TYPE.MSG_TYPE_NEW_MESSAGE, {'type':message_type})
+
+    def finished_message(self, message_text:str="", callback: Callable[[str, int, dict], bool]=None):
+        """This sends step rogress to front end
+
+        Args:
+            step_text (dict): The step progress in %
+            callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the progress to. Defaults to None.
+        """
+        if not callback and self.callback:
+            callback = self.callback
+
+        if callback:
+            callback(message_text, MSG_TYPE.MSG_TYPE_FINISHED_MESSAGE)
 
     #Helper method to convert outputs path to url
     def path2url(file):
         file = str(file).replace("\\","/")
         pth = file.split('/')
         idx = pth.index("outputs")
         pth = "/".join(pth[idx:])
@@ -1311,20 +1326,22 @@
 
 class PersonalityBuilder:
     def __init__(
                     self, 
                     lollms_paths:LollmsPaths, 
                     config:LOLLMSConfig, 
                     model:LLMBinding, 
-                    installation_option:InstallOption=InstallOption.INSTALL_IF_NECESSARY
+                    installation_option:InstallOption=InstallOption.INSTALL_IF_NECESSARY,
+                    callback=None
                 ):
         self.config = config
         self.lollms_paths = lollms_paths
         self.model = model
         self.installation_option = installation_option
+        self.callback = callback
 
 
     def build_personality(self, id:int=None):
         if id is None:
             id = self.config["active_personality_id"]
             if self.config["active_personality_id"]>=len(self.config["personalities"]):
                 ASCIIColors.warning("Personality ID was out of range. Resetting to 0.")
@@ -1335,22 +1352,24 @@
                 id = len(self.config["personalities"])-1
         if len(self.config["personalities"][id].split("/"))==3:
             self.personality = AIPersonality(
                                             self.lollms_paths.personalities_zoo_path / self.config["personalities"][id],
                                             self.lollms_paths,
                                             self.config,
                                             self.model, 
-                                            installation_option=self.installation_option
+                                            installation_option=self.installation_option,
+                                            callback=self.callback
                                         )
         else:
             self.personality = AIPersonality(
                                             self.config["personalities"][id],
                                             self.lollms_paths,
                                             self.config,
                                             self.model,
                                             is_relative_path=False,
-                                            installation_option=self.installation_option
+                                            installation_option=self.installation_option,
+                                            callback=self.callback
                                         )
         return self.personality
     
     def get_personality(self):
         return self.personality
```

### Comparing `lollms-2.2.0/lollms/terminal.py` & `lollms-2.2.1/lollms/terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,1067 +307,1074 @@
 00001320: 2061 6e73 7765 7220 7769 7468 2027 7965   answer with 'ye
 00001330: 7327 206f 7220 276e 6f27 2028 6f72 2027  s' or 'no' (or '
 00001340: 7927 2f27 6e27 292e 2229 0d0a 0d0a 636c  y'/'n').")....cl
 00001350: 6173 7320 4d61 696e 4d65 6e75 284d 656e  ass MainMenu(Men
 00001360: 7529 3a0d 0a20 2020 2064 6566 205f 5f69  u):..    def __i
 00001370: 6e69 745f 5f28 7365 6c66 2c20 6c6f 6c6c  nit__(self, loll
 00001380: 6d73 5f61 7070 3a27 4c6f 6c6c 6d73 4170  ms_app:'LollmsAp
-00001390: 706c 6963 6174 696f 6e27 293a 0d0a 2020  plication'):..  
-000013a0: 2020 2020 2020 7365 6c66 2e62 696e 6469        self.bindi
-000013b0: 6e67 5f69 6e66 7320 3d20 5b5d 0d0a 2020  ng_infs = []..  
-000013c0: 2020 2020 2020 7365 6c66 2e6c 6f6c 6c6d        self.lollm
-000013d0: 735f 6170 7020 3d20 6c6f 6c6c 6d73 5f61  s_app = lollms_a
-000013e0: 7070 0d0a 2020 2020 2020 2020 6d61 696e  pp..        main
-000013f0: 5f6d 656e 755f 6f70 7469 6f6e 7320 3d20  _menu_options = 
-00001400: 5b0d 0a20 2020 2020 2020 2020 2020 207b  [..            {
-00001410: 276e 616d 6527 3a20 274d 6169 6e20 7365  'name': 'Main se
-00001420: 7474 696e 6773 272c 2027 666e 273a 2073  ttings', 'fn': s
-00001430: 656c 662e 6d61 696e 5f73 6574 7469 6e67  elf.main_setting
-00001440: 732c 2027 6865 6c70 273a 2022 5368 6f77  s, 'help': "Show
-00001450: 206d 6169 6e20 7365 7474 696e 6773 2e22   main settings."
-00001460: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-00001470: 7b27 6e61 6d65 273a 2027 5365 6c65 6374  {'name': 'Select
-00001480: 2042 696e 6469 6e67 272c 2027 666e 273a   Binding', 'fn':
-00001490: 2073 656c 662e 7365 6c65 6374 5f62 696e   self.select_bin
-000014a0: 6469 6e67 2c20 2768 656c 7027 3a20 2243  ding, 'help': "C
-000014b0: 686f 6f73 6520 6120 6269 6e64 696e 672e  hoose a binding.
-000014c0: 227d 2c0d 0a20 2020 2020 2020 2020 2020  "},..           
-000014d0: 207b 276e 616d 6527 3a20 2753 656c 6563   {'name': 'Selec
-000014e0: 7420 4d6f 6465 6c27 2c20 2766 6e27 3a20  t Model', 'fn': 
-000014f0: 7365 6c66 2e73 656c 6563 745f 6d6f 6465  self.select_mode
-00001500: 6c2c 2027 6865 6c70 273a 2022 4368 6f6f  l, 'help': "Choo
-00001510: 7365 2061 206d 6f64 656c 2e22 7d2c 0d0a  se a model."},..
-00001520: 2020 2020 2020 2020 2020 2020 7b27 6e61              {'na
-00001530: 6d65 273a 2027 5669 6577 206d 6f75 6e74  me': 'View mount
-00001540: 6564 2050 6572 736f 6e61 6c69 7469 6573  ed Personalities
-00001550: 272c 2027 666e 273a 2073 656c 662e 7665  ', 'fn': self.ve
-00001560: 775f 6d6f 756e 7465 645f 7065 7273 6f6e  w_mounted_person
-00001570: 616c 6974 6965 732c 2027 6865 6c70 273a  alities, 'help':
-00001580: 2022 5669 6577 2061 6c6c 2063 7572 7265   "View all curre
-00001590: 6e74 6c79 206d 6f75 6e74 6564 2070 6572  ntly mounted per
-000015a0: 736f 6e61 6c69 7469 6573 2e22 7d2c 0d0a  sonalities."},..
-000015b0: 2020 2020 2020 2020 2020 2020 7b27 6e61              {'na
-000015c0: 6d65 273a 2027 4d6f 756e 7420 5065 7273  me': 'Mount Pers
-000015d0: 6f6e 616c 6974 7927 2c20 2766 6e27 3a20  onality', 'fn': 
-000015e0: 7365 6c66 2e6d 6f75 6e74 5f70 6572 736f  self.mount_perso
-000015f0: 6e61 6c69 7479 2c20 2768 656c 7027 3a20  nality, 'help': 
-00001600: 224d 6f75 6e74 2061 206e 6577 2070 6572  "Mount a new per
-00001610: 736f 6e61 6c69 7479 2e22 7d2c 0d0a 2020  sonality."},..  
-00001620: 2020 2020 2020 2020 2020 7b27 6e61 6d65            {'name
-00001630: 273a 2027 556e 6d6f 756e 7420 5065 7273  ': 'Unmount Pers
-00001640: 6f6e 616c 6974 7927 2c20 2766 6e27 3a20  onality', 'fn': 
-00001650: 7365 6c66 2e75 6e6d 6f75 6e74 5f70 6572  self.unmount_per
-00001660: 736f 6e61 6c69 7479 2c20 2768 656c 7027  sonality, 'help'
-00001670: 3a20 2255 6e6d 6f75 6e74 2061 2070 6572  : "Unmount a per
-00001680: 736f 6e61 6c69 7479 2e22 7d2c 0d0a 2020  sonality."},..  
-00001690: 2020 2020 2020 2020 2020 7b27 6e61 6d65            {'name
-000016a0: 273a 2027 5365 6c65 6374 2050 6572 736f  ': 'Select Perso
-000016b0: 6e61 6c69 7479 272c 2027 666e 273a 2073  nality', 'fn': s
-000016c0: 656c 662e 7365 6c65 6374 5f70 6572 736f  elf.select_perso
-000016d0: 6e61 6c69 7479 2c20 2768 656c 7027 3a20  nality, 'help': 
-000016e0: 2243 686f 6f73 6520 6120 7065 7273 6f6e  "Choose a person
-000016f0: 616c 6974 792e 227d 2c0d 0a20 2020 2020  ality."},..     
-00001700: 2020 2020 2020 207b 276e 616d 6527 3a20         {'name': 
-00001710: 2752 6569 6e73 7461 6c6c 2042 696e 6469  'Reinstall Bindi
-00001720: 6e67 272c 2027 666e 273a 2073 656c 662e  ng', 'fn': self.
-00001730: 7265 696e 7374 616c 6c5f 6269 6e64 696e  reinstall_bindin
-00001740: 672c 2027 6865 6c70 273a 2022 5265 696e  g, 'help': "Rein
-00001750: 7374 616c 6c20 7468 6520 7365 6c65 6374  stall the select
-00001760: 6564 2062 696e 6469 6e67 2e22 7d2c 0d0a  ed binding."},..
-00001770: 2020 2020 2020 2020 2020 2020 7b27 6e61              {'na
-00001780: 6d65 273a 2027 5265 696e 7374 616c 6c20  me': 'Reinstall 
-00001790: 6375 7272 656e 7420 5065 7273 6f6e 616c  current Personal
-000017a0: 6974 7927 2c20 2766 6e27 3a20 7365 6c66  ity', 'fn': self
-000017b0: 2e72 6569 6e73 7461 6c6c 5f70 6572 736f  .reinstall_perso
-000017c0: 6e61 6c69 7479 2c20 2768 656c 7027 3a20  nality, 'help': 
-000017d0: 2252 6569 6e73 7461 6c6c 2074 6865 2063  "Reinstall the c
-000017e0: 7572 7265 6e74 2073 656c 6563 7465 6420  urrent selected 
-000017f0: 7065 7273 6f6e 616c 6974 792e 227d 2c0d  personality."},.
-00001800: 0a20 2020 2020 2020 2020 2020 207b 276e  .            {'n
-00001810: 616d 6527 3a20 2752 6573 6574 2061 6c6c  ame': 'Reset all
-00001820: 2069 6e73 7461 6c6c 7327 2c20 2766 6e27   installs', 'fn'
-00001830: 3a20 7365 6c66 2e6c 6f6c 6c6d 735f 6170  : self.lollms_ap
-00001840: 702e 7265 7365 745f 616c 6c5f 696e 7374  p.reset_all_inst
-00001850: 616c 6c73 2c20 2768 656c 7027 3a20 2252  alls, 'help': "R
-00001860: 6573 6574 2061 6c6c 2069 6e73 7461 6c6c  eset all install
-00001870: 6564 2070 6572 736f 6e61 6c69 7469 6573  ed personalities
-00001880: 2e22 7d2c 0d0a 2020 2020 2020 2020 2020  ."},..          
-00001890: 2020 7b27 6e61 6d65 273a 2027 5265 7365    {'name': 'Rese
-000018a0: 7420 7061 7468 7327 2c20 2766 6e27 3a20  t paths', 'fn': 
-000018b0: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
-000018c0: 6c6f 6c6c 6d73 5f70 6174 6873 2e72 6573  lollms_paths.res
-000018d0: 6574 5061 7468 732c 2027 6865 6c70 273a  etPaths, 'help':
-000018e0: 2022 5265 7365 7420 616c 6c20 7061 7468   "Reset all path
-000018f0: 7320 746f 2064 6566 6175 6c74 2e22 7d2c  s to default."},
-00001900: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
-00001910: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00001920: 6e69 745f 5f28 224c 6f6c 6c6d 7320 4d61  nit__("Lollms Ma
-00001930: 696e 206d 656e 7522 2c20 6d61 696e 5f6d  in menu", main_m
-00001940: 656e 755f 6f70 7469 6f6e 7329 0d0a 0d0a  enu_options)....
-00001950: 2020 2020 6465 6620 6d61 696e 5f73 6574      def main_set
-00001960: 7469 6e67 7328 7365 6c66 293a 0d0a 2020  tings(self):..  
-00001970: 2020 2020 2020 7365 6c66 2e73 686f 7728        self.show(
-00001980: 5b0d 0a20 2020 2020 2020 2020 2020 207b  [..            {
-00001990: 276e 616d 6527 3a20 2753 6574 2075 7365  'name': 'Set use
-000019a0: 7220 6e61 6d65 272c 2027 666e 273a 2073  r name', 'fn': s
-000019b0: 656c 662e 7365 745f 7573 6572 5f6e 616d  elf.set_user_nam
-000019c0: 652c 2027 6865 6c70 273a 2022 5365 7473  e, 'help': "Sets
-000019d0: 2074 6865 2075 7365 7220 6e61 6d65 2e22   the user name."
-000019e0: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
-000019f0: 7b27 6e61 6d65 273a 2027 5365 7420 7573  {'name': 'Set us
-00001a00: 6520 7573 6572 206e 616d 6520 696e 2064  e user name in d
-00001a10: 6973 6375 7373 696f 6e27 2c20 2766 6e27  iscussion', 'fn'
-00001a20: 3a20 7365 6c66 2e73 6574 5f75 7365 5f75  : self.set_use_u
-00001a30: 7365 725f 6e61 6d65 5f69 6e5f 6469 7363  ser_name_in_disc
-00001a40: 7573 7369 6f6e 732c 2027 6865 6c70 273a  ussions, 'help':
-00001a50: 2022 5365 7473 2074 6865 2075 7365 7220   "Sets the user 
-00001a60: 6e61 6d65 2e22 7d2c 0d0a 2020 2020 2020  name."},..      
-00001a70: 2020 5d29 0d0a 0d0a 2020 2020 6465 6620    ])....    def 
-00001a80: 7365 745f 7573 6572 5f6e 616d 6528 7365  set_user_name(se
-00001a90: 6c66 293a 0d0a 2020 2020 2020 2020 7072  lf):..        pr
-00001aa0: 696e 7428 6622 4375 7272 656e 7420 7573  int(f"Current us
-00001ab0: 6572 206e 616d 6520 3a20 7b73 656c 662e  er name : {self.
-00001ac0: 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e 6669  lollms_app.confi
-00001ad0: 672e 7573 6572 5f6e 616d 657d 2229 0d0a  g.user_name}")..
-00001ae0: 2020 2020 2020 2020 7365 6c66 2e6c 6f6c          self.lol
-00001af0: 6c6d 735f 6170 702e 636f 6e66 6967 2e75  lms_app.config.u
-00001b00: 7365 725f 6e61 6d65 203d 2069 6e70 7574  ser_name = input
-00001b10: 2822 4e65 7720 7573 6572 206e 616d 653a  ("New user name:
-00001b20: 2229 0d0a 2020 2020 2020 2020 7365 6c66  ")..        self
-00001b30: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
-00001b40: 6967 2e73 6176 655f 636f 6e66 6967 2829  ig.save_config()
-00001b50: 0d0a 0d0a 2020 2020 6465 6620 7365 745f  ....    def set_
-00001b60: 7573 655f 7573 6572 5f6e 616d 655f 696e  use_user_name_in
-00001b70: 5f64 6973 6375 7373 696f 6e73 2873 656c  _discussions(sel
-00001b80: 6629 3a0d 0a20 2020 2020 2020 2041 5343  f):..        ASC
-00001b90: 4949 436f 6c6f 7273 2e69 6e66 6f28 6622  IIColors.info(f"
-00001ba0: 4375 7272 656e 7420 7374 6174 7573 3a20  Current status: 
-00001bb0: 7b73 656c 662e 6c6f 6c6c 6d73 5f61 7070  {self.lollms_app
-00001bc0: 2e63 6f6e 6669 672e 7573 655f 7573 6572  .config.use_user
-00001bd0: 5f6e 616d 655f 696e 5f64 6973 6375 7373  _name_in_discuss
-00001be0: 696f 6e73 7d22 290d 0a20 2020 2020 2020  ions}")..       
-00001bf0: 2073 656c 662e 6c6f 6c6c 6d73 5f61 7070   self.lollms_app
-00001c00: 2e63 6f6e 6669 672e 7573 655f 7573 6572  .config.use_user
-00001c10: 5f6e 616d 655f 696e 5f64 6973 6375 7373  _name_in_discuss
-00001c20: 696f 6e73 203d 2073 656c 662e 7965 735f  ions = self.yes_
-00001c30: 6e6f 5f71 7565 7374 696f 6e28 2755 7365  no_question('Use
-00001c40: 2075 7365 7220 6e61 6d65 2069 6e20 6469   user name in di
-00001c50: 6373 7573 7369 6f6e 2729 0d0a 2020 2020  csussion')..    
-00001c60: 2020 2020 7365 6c66 2e6c 6f6c 6c6d 735f      self.lollms_
-00001c70: 6170 702e 636f 6e66 6967 2e73 6176 655f  app.config.save_
-00001c80: 636f 6e66 6967 2829 0d0a 0d0a 2020 2020  config()....    
-00001c90: 6465 6620 7368 6f77 5f6c 6f67 6f28 7365  def show_logo(se
-00001ca0: 6c66 293a 0d0a 2020 2020 2020 2020 7072  lf):..        pr
-00001cb0: 696e 7428 6622 7b41 5343 4949 436f 6c6f  int(f"{ASCIIColo
-00001cc0: 7273 2e63 6f6c 6f72 5f62 7269 6768 745f  rs.color_bright_
-00001cd0: 7965 6c6c 6f77 7d22 290d 0a20 2020 2020  yellow}")..     
-00001ce0: 2020 2070 7269 6e74 2822 2020 2020 2020     print("      
-00001cf0: 5f5f 5f20 2020 2020 2020 5f5f 5f20 2020  ___       ___   
-00001d00: 2020 2020 2020 2020 5f5f 5f20 2020 2020          ___     
-00001d10: 2020 5f5f 5f20 2020 2020 2020 5f5f 5f20    ___       ___ 
-00001d20: 2020 2020 2020 2020 2020 5f5f 5f20 2020            ___   
-00001d30: 2020 2022 290d 0a20 2020 2020 2020 2070     ")..        p
-00001d40: 7269 6e74 2822 2020 2020 202f 5c5f 5f5c  rint("     /\__\
-00001d50: 2020 2020 202f 5c20 205c 2020 2020 2020       /\  \      
-00001d60: 2020 202f 5c5f 5f5c 2020 2020 202f 5c5f     /\__\     /\_
-00001d70: 5f5c 2020 2020 202f 5c5f 5f5c 2020 2020  _\     /\__\    
-00001d80: 2020 2020 202f 5c20 205c 2020 2020 2022       /\  \     "
-00001d90: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00001da0: 2822 2020 2020 2f3a 2f20 202f 2020 2020  ("    /:/  /    
-00001db0: 2f3a 3a5c 2020 5c20 2020 2020 2020 2f3a  /::\  \       /:
-00001dc0: 2f20 202f 2020 2020 2f3a 2f20 202f 2020  /  /    /:/  /  
-00001dd0: 2020 2f3a 3a7c 2020 7c20 2020 2020 2020    /::|  |       
-00001de0: 2f3a 3a5c 2020 5c20 2020 2022 290d 0a20  /::\  \    ").. 
-00001df0: 2020 2020 2020 2070 7269 6e74 2822 2020         print("  
-00001e00: 202f 3a2f 2020 2f20 2020 202f 3a2f 5c3a   /:/  /    /:/\:
-00001e10: 5c20 205c 2020 2020 202f 3a2f 2020 2f20  \  \     /:/  / 
-00001e20: 2020 202f 3a2f 2020 2f20 2020 202f 3a7c     /:/  /    /:|
-00001e30: 3a7c 2020 7c20 2020 2020 202f 3a2f 5c20  :|  |      /:/\ 
-00001e40: 5c20 205c 2020 2022 290d 0a20 2020 2020  \  \   ")..     
-00001e50: 2020 2070 7269 6e74 2822 2020 2f3a 2f20     print("  /:/ 
-00001e60: 202f 2020 2020 2f3a 2f20 205c 3a5c 2020   /    /:/  \:\  
-00001e70: 5c20 2020 2f3a 2f20 202f 2020 2020 2f3a  \   /:/  /    /:
-00001e80: 2f20 202f 2020 2020 2f3a 2f7c 3a7c 5f5f  /  /    /:/|:|__
-00001e90: 7c5f 5f20 2020 5f5c 3a5c 7e5c 205c 2020  |__   _\:\~\ \  
-00001ea0: 5c20 2022 290d 0a20 2020 2020 2020 2070  \  ")..        p
-00001eb0: 7269 6e74 2822 202f 3a2f 5f5f 2f20 2020  rint(" /:/__/   
-00001ec0: 202f 3a2f 5f5f 2f20 5c3a 5c5f 5f5c 202f   /:/__/ \:\__\ /
-00001ed0: 3a2f 5f5f 2f20 2020 202f 3a2f 5f5f 2f20  :/__/    /:/__/ 
-00001ee0: 2020 202f 3a2f 207c 3a3a 3a3a 5c5f 5f5c     /:/ |::::\__\
-00001ef0: 202f 5c20 5c3a 5c20 5c20 5c5f 5f5c 2022   /\ \:\ \ \__\ "
-00001f00: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00001f10: 2822 205c 3a5c 2020 5c20 2020 205c 3a5c  (" \:\  \    \:\
-00001f20: 2020 5c20 2f3a 2f20 202f 205c 3a5c 2020    \ /:/  / \:\  
-00001f30: 5c20 2020 205c 3a5c 2020 5c20 2020 205c  \    \:\  \    \
-00001f40: 2f5f 5f2f 7e7e 2f3a 2f20 202f 205c 3a5c  /__/~~/:/  / \:\
-00001f50: 205c 3a5c 205c 2f5f 5f2f 2022 290d 0a20   \:\ \/__/ ").. 
-00001f60: 2020 2020 2020 2070 7269 6e74 2822 2020         print("  
-00001f70: 5c3a 5c20 205c 2020 2020 5c3a 5c20 202f  \:\  \    \:\  /
-00001f80: 3a2f 2020 2f20 2020 5c3a 5c20 205c 2020  :/  /   \:\  \  
-00001f90: 2020 5c3a 5c20 205c 2020 2020 2020 2020    \:\  \        
-00001fa0: 202f 3a2f 2020 2f20 2020 5c3a 5c20 5c3a   /:/  /   \:\ \:
-00001fb0: 5c5f 5f5c 2020 2022 290d 0a20 2020 2020  \__\   ")..     
-00001fc0: 2020 2070 7269 6e74 2822 2020 205c 3a5c     print("   \:\
-00001fd0: 2020 5c20 2020 205c 3a5c 2f3a 2f20 202f    \    \:\/:/  /
-00001fe0: 2020 2020 205c 3a5c 2020 5c20 2020 205c       \:\  \    \
-00001ff0: 3a5c 2020 5c20 2020 2020 2020 2f3a 2f20  :\  \       /:/ 
-00002000: 202f 2020 2020 205c 3a5c 2f3a 2f20 202f   /     \:\/:/  /
-00002010: 2020 2022 290d 0a20 2020 2020 2020 2070     ")..        p
-00002020: 7269 6e74 2822 2020 2020 5c3a 5c5f 5f5c  rint("    \:\__\
-00002030: 2020 2020 5c3a 3a2f 2020 2f20 2020 2020      \::/  /     
-00002040: 2020 5c3a 5c5f 5f5c 2020 2020 5c3a 5c5f    \:\__\    \:\_
-00002050: 5f5c 2020 2020 202f 3a2f 2020 2f20 2020  _\     /:/  /   
-00002060: 2020 2020 5c3a 3a2f 2020 2f20 2020 2022      \::/  /    "
-00002070: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00002080: 2822 2020 2020 205c 2f5f 5f2f 2020 2020  ("     \/__/    
-00002090: 205c 2f5f 5f2f 2020 2020 2020 2020 205c   \/__/         \
-000020a0: 2f5f 5f2f 2020 2020 205c 2f5f 5f2f 2020  /__/     \/__/  
-000020b0: 2020 205c 2f5f 5f2f 2020 2020 2020 2020     \/__/        
-000020c0: 205c 2f5f 5f2f 2020 2020 2022 290d 0a0d   \/__/     ")...
-000020d0: 0a0d 0a0d 0a0d 0a20 2020 2020 2020 2070  .......        p
-000020e0: 7269 6e74 2866 227b 4153 4349 4943 6f6c  rint(f"{ASCIICol
-000020f0: 6f72 732e 636f 6c6f 725f 7265 7365 747d  ors.color_reset}
-00002100: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
-00002110: 7428 6622 7b41 5343 4949 436f 6c6f 7273  t(f"{ASCIIColors
-00002120: 2e63 6f6c 6f72 5f72 6564 7d56 6572 7369  .color_red}Versi
-00002130: 6f6e 3a20 7b41 5343 4949 436f 6c6f 7273  on: {ASCIIColors
-00002140: 2e63 6f6c 6f72 5f67 7265 656e 7d7b 706b  .color_green}{pk
-00002150: 675f 7265 736f 7572 6365 732e 6765 745f  g_resources.get_
-00002160: 6469 7374 7269 6275 7469 6f6e 2827 6c6f  distribution('lo
-00002170: 6c6c 6d73 2729 2e76 6572 7369 6f6e 7d22  llms').version}"
-00002180: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00002190: 2866 227b 4153 4349 4943 6f6c 6f72 732e  (f"{ASCIIColors.
-000021a0: 636f 6c6f 725f 7265 647d 4279 203a 207b  color_red}By : {
-000021b0: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
-000021c0: 725f 6772 6565 6e7d 5061 7269 734e 656f  r_green}ParisNeo
-000021d0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
-000021e0: 7428 6622 7b41 5343 4949 436f 6c6f 7273  t(f"{ASCIIColors
-000021f0: 2e63 6f6c 6f72 5f72 6573 6574 7d22 290d  .color_reset}").
-00002200: 0a0d 0a20 2020 2064 6566 2073 686f 775f  ...    def show_
-00002210: 636f 6d6d 616e 6473 5f6c 6973 7428 7365  commands_list(se
-00002220: 6c66 293a 0d0a 2020 2020 2020 2020 7072  lf):..        pr
-00002230: 696e 7428 290d 0a20 2020 2020 2020 2070  int()..        p
-00002240: 7269 6e74 2822 436f 6d6d 616e 6473 3a22  rint("Commands:"
-00002250: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
-00002260: 2866 2220 2020 7b41 5343 4949 436f 6c6f  (f"   {ASCIIColo
-00002270: 7273 2e63 6f6c 6f72 5f72 6564 7de2 949c  rs.color_red}...
-00002280: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
-00002290: 6f72 5f72 6573 6574 7d20 6d65 6e75 3a20  or_reset} menu: 
-000022a0: 7368 6f77 7320 6d61 696e 206d 656e 7522  shows main menu"
-000022b0: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
-000022c0: 2020 2070 7269 6e74 2866 2220 2020 7b41     print(f"   {A
-000022d0: 5343 4949 436f 6c6f 7273 2e63 6f6c 6f72  SCIIColors.color
-000022e0: 5f72 6564 7de2 949c 7b41 5343 4949 436f  _red}...{ASCIICo
-000022f0: 6c6f 7273 2e63 6f6c 6f72 5f72 6573 6574  lors.color_reset
-00002300: 7d20 6865 6c70 3a20 7368 6f77 7320 7468  } help: shows th
-00002310: 6973 2069 6e66 6f22 2920 2020 2020 2020  is info")       
-00002320: 200d 0a20 2020 2020 2020 2070 7269 6e74   ..        print
-00002330: 2866 2220 2020 7b41 5343 4949 436f 6c6f  (f"   {ASCIIColo
-00002340: 7273 2e63 6f6c 6f72 5f72 6564 7de2 949c  rs.color_red}...
-00002350: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
-00002360: 6f72 5f72 6573 6574 7d20 7265 7365 743a  or_reset} reset:
-00002370: 2072 6573 6574 7320 7468 6520 636f 6e74   resets the cont
-00002380: 6578 7422 290d 0a20 2020 2020 2020 2070  ext")..        p
-00002390: 7269 6e74 2866 2220 2020 7b41 5343 4949  rint(f"   {ASCII
-000023a0: 436f 6c6f 7273 2e63 6f6c 6f72 5f72 6564  Colors.color_red
-000023b0: 7de2 949c 7b41 5343 4949 436f 6c6f 7273  }...{ASCIIColors
-000023c0: 2e63 6f6c 6f72 5f72 6573 6574 7d20 3c65  .color_reset} <e
-000023d0: 6d70 7479 2070 726f 6d70 743e 3a20 666f  mpty prompt>: fo
-000023e0: 7263 6573 2074 6865 206d 6f64 656c 2074  rces the model t
-000023f0: 6f20 636f 6e74 696e 7565 2067 656e 6572  o continue gener
-00002400: 6174 696e 6722 290d 0a20 2020 2020 2020  ating")..       
-00002410: 2070 7269 6e74 2866 2220 2020 7b41 5343   print(f"   {ASC
-00002420: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f72  IIColors.color_r
-00002430: 6564 7de2 949c 7b41 5343 4949 436f 6c6f  ed}...{ASCIIColo
-00002440: 7273 2e63 6f6c 6f72 5f72 6573 6574 7d20  rs.color_reset} 
-00002450: 636f 6e74 6578 745f 696e 666f 733a 2063  context_infos: c
-00002460: 7572 7265 6e74 2063 6f6e 7465 7874 2073  urrent context s
-00002470: 697a 6520 616e 6420 7370 6163 6520 6c65  ize and space le
-00002480: 6674 2062 6566 6f72 6520 6372 6f70 7069  ft before croppi
-00002490: 6e67 2229 0d0a 2020 2020 2020 2020 7072  ng")..        pr
-000024a0: 696e 7428 6622 2020 207b 4153 4349 4943  int(f"   {ASCIIC
-000024b0: 6f6c 6f72 732e 636f 6c6f 725f 7265 647d  olors.color_red}
-000024c0: e294 9c7b 4153 4349 4943 6f6c 6f72 732e  ...{ASCIIColors.
-000024d0: 636f 6c6f 725f 7265 7365 747d 2073 7461  color_reset} sta
-000024e0: 7274 5f6c 6f67 3a20 7374 6172 7473 206c  rt_log: starts l
-000024f0: 6f67 6769 6e67 2074 6865 2064 6973 6375  ogging the discu
-00002500: 7373 696f 6e20 746f 2061 2074 6578 7420  ssion to a text 
-00002510: 6669 6c65 2229 0d0a 2020 2020 2020 2020  file")..        
-00002520: 7072 696e 7428 6622 2020 207b 4153 4349  print(f"   {ASCI
-00002530: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
-00002540: 647d e294 9c7b 4153 4349 4943 6f6c 6f72  d}...{ASCIIColor
-00002550: 732e 636f 6c6f 725f 7265 7365 747d 2073  s.color_reset} s
-00002560: 746f 705f 6c6f 673a 2073 746f 7073 206c  top_log: stops l
-00002570: 6f67 6769 6e67 2074 6865 2064 6973 6375  ogging the discu
-00002580: 7373 696f 6e20 746f 2061 2074 6578 7420  ssion to a text 
-00002590: 6669 6c65 2229 0d0a 2020 2020 2020 2020  file")..        
-000025a0: 7072 696e 7428 6622 2020 207b 4153 4349  print(f"   {ASCI
-000025b0: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
-000025c0: 647d e294 9c7b 4153 4349 4943 6f6c 6f72  d}...{ASCIIColor
-000025d0: 732e 636f 6c6f 725f 7265 7365 747d 2073  s.color_reset} s
-000025e0: 656e 645f 6669 6c65 3a20 7570 6c6f 6164  end_file: upload
-000025f0: 7320 6120 6669 6c65 2074 6f20 7468 6520  s a file to the 
-00002600: 4149 2229 0d0a 2020 2020 2020 2020 7072  AI")..        pr
-00002610: 696e 7428 6622 2020 207b 4153 4349 4943  int(f"   {ASCIIC
-00002620: 6f6c 6f72 732e 636f 6c6f 725f 7265 647d  olors.color_red}
-00002630: e294 947b 4153 4349 4943 6f6c 6f72 732e  ...{ASCIIColors.
-00002640: 636f 6c6f 725f 7265 7365 747d 2065 7869  color_reset} exi
-00002650: 743a 2065 7869 7374 7320 7468 6520 636f  t: exists the co
-00002660: 6e73 6f6c 6522 290d 0a20 2020 2020 2020  nsole")..       
-00002670: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
-00002680: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 7065  lf.lollms_app.pe
-00002690: 7273 6f6e 616c 6974 793a 0d0a 2020 2020  rsonality:..    
-000026a0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-000026b0: 6c6f 6c6c 6d73 5f61 7070 2e70 6572 736f  lollms_app.perso
-000026c0: 6e61 6c69 7479 2e68 656c 7020 213d 2222  nality.help !=""
-000026d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000026e0: 2020 2070 7269 6e74 2866 2250 6572 736f     print(f"Perso
-000026f0: 6e61 6c69 7479 2068 656c 703a 2229 0d0a  nality help:")..
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 7072 696e 7428 6622 7b73 656c 662e 6c6f  print(f"{self.lo
-00002720: 6c6c 6d73 5f61 7070 2e70 6572 736f 6e61  llms_app.persona
-00002730: 6c69 7479 2e68 656c 707d 2229 0d0a 2020  lity.help}")..  
-00002740: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00002750: 2020 2020 0d0a 0d0a 2020 2020 6465 6620      ....    def 
-00002760: 7368 6f77 5f6d 656e 7528 7365 6c66 2c20  show_menu(self, 
-00002770: 6f70 7469 6f6e 732c 2074 6974 6c65 3d22  options, title="
-00002780: 4d65 6e75 3a22 2c20 7365 6c65 6374 696f  Menu:", selectio
-00002790: 6e3a 696e 743d 4e6f 6e65 293a 0d0a 2020  n:int=None):..  
-000027a0: 2020 2020 2020 4153 4349 4943 6f6c 6f72        ASCIIColor
-000027b0: 732e 7965 6c6c 6f77 2874 6974 6c65 290d  s.yellow(title).
-000027c0: 0a20 2020 2020 2020 2066 6f72 2069 6e64  .        for ind
-000027d0: 6578 2c20 6f70 7469 6f6e 2069 6e20 656e  ex, option in en
-000027e0: 756d 6572 6174 6528 6f70 7469 6f6e 7329  umerate(options)
-000027f0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00002800: 6620 7365 6c65 6374 696f 6e20 6973 206e  f selection is n
-00002810: 6f74 204e 6f6e 6520 616e 6420 696e 6465  ot None and inde
-00002820: 783d 3d73 656c 6563 7469 6f6e 3a0d 0a20  x==selection:.. 
-00002830: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002840: 7269 6e74 2866 227b 4153 4349 4943 6f6c  rint(f"{ASCIICol
-00002850: 6f72 732e 636f 6c6f 725f 6772 6565 6e7d  ors.color_green}
-00002860: 7b69 6e64 6578 202b 2031 7d20 2d20 7b6f  {index + 1} - {o
-00002870: 7074 696f 6e7d 7b41 5343 4949 436f 6c6f  ption}{ASCIIColo
-00002880: 7273 2e63 6f6c 6f72 5f72 6573 6574 7d22  rs.color_reset}"
-00002890: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
-000028a0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-000028b0: 2020 2020 2020 7072 696e 7428 6622 7b41        print(f"{A
-000028c0: 5343 4949 436f 6c6f 7273 2e63 6f6c 6f72  SCIIColors.color
-000028d0: 5f67 7265 656e 7d7b 696e 6465 7820 2b20  _green}{index + 
-000028e0: 317d 202d 7b41 5343 4949 436f 6c6f 7273  1} -{ASCIIColors
-000028f0: 2e63 6f6c 6f72 5f72 6573 6574 7d20 7b6f  .color_reset} {o
-00002900: 7074 696f 6e7d 2229 0d0a 2020 2020 2020  ption}")..      
-00002910: 2020 6368 6f69 6365 203d 2069 6e70 7574    choice = input
-00002920: 2822 456e 7465 7220 796f 7572 2063 686f  ("Enter your cho
-00002930: 6963 653a 2022 290d 0a20 2020 2020 2020  ice: ")..       
-00002940: 2072 6574 7572 6e20 696e 7428 6368 6f69   return int(choi
-00002950: 6365 2920 6966 2063 686f 6963 652e 6973  ce) if choice.is
-00002960: 6469 6769 7428 2920 656c 7365 202d 310d  digit() else -1.
-00002970: 0a0d 0a20 2020 2064 6566 2073 656c 6563  ...    def selec
-00002980: 745f 6269 6e64 696e 6728 7365 6c66 293a  t_binding(self):
-00002990: 0d0a 2020 2020 2020 2020 6269 6e64 696e  ..        bindin
-000029a0: 6773 5f6c 6973 7420 3d20 5b5d 0d0a 2020  gs_list = []..  
-000029b0: 2020 2020 2020 7072 696e 7428 290d 0a20        print().. 
-000029c0: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
-000029d0: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
-000029e0: 725f 6772 6565 6e7d 4375 7272 656e 7420  r_green}Current 
-000029f0: 6269 6e64 696e 673a 207b 4153 4349 4943  binding: {ASCIIC
-00002a00: 6f6c 6f72 732e 636f 6c6f 725f 7265 7365  olors.color_rese
-00002a10: 747d 7b73 656c 662e 6c6f 6c6c 6d73 5f61  t}{self.lollms_a
-00002a20: 7070 2e63 6f6e 6669 675b 2762 696e 6469  pp.config['bindi
-00002a30: 6e67 5f6e 616d 6527 5d7d 2229 0d0a 2020  ng_name']}")..  
-00002a40: 2020 2020 2020 666f 7220 7020 696e 2073        for p in s
-00002a50: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e6c  elf.lollms_app.l
-00002a60: 6f6c 6c6d 735f 7061 7468 732e 6269 6e64  ollms_paths.bind
-00002a70: 696e 6773 5f7a 6f6f 5f70 6174 682e 6974  ings_zoo_path.it
-00002a80: 6572 6469 7228 293a 0d0a 2020 2020 2020  erdir():..      
-00002a90: 2020 2020 2020 6966 2070 2e69 735f 6469        if p.is_di
-00002aa0: 7228 2920 616e 6420 6e6f 7420 702e 7374  r() and not p.st
-00002ab0: 656d 2e73 7461 7274 7377 6974 6828 222e  em.startswith(".
-00002ac0: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-00002ad0: 2020 2020 2077 6974 6820 6f70 656e 2870       with open(p
-00002ae0: 2f22 6269 6e64 696e 675f 6361 7264 2e79  /"binding_card.y
-00002af0: 616d 6c22 2c20 2272 2229 2061 7320 663a  aml", "r") as f:
-00002b00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002b10: 2020 2020 2020 6361 7264 203d 2079 616d        card = yam
-00002b20: 6c2e 7361 6665 5f6c 6f61 6428 6629 0d0a  l.safe_load(f)..
-00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b40: 7769 7468 206f 7065 6e28 702f 226d 6f64  with open(p/"mod
-00002b50: 656c 732e 7961 6d6c 222c 2022 7222 2920  els.yaml", "r") 
-00002b60: 6173 2066 3a0d 0a20 2020 2020 2020 2020  as f:..         
-00002b70: 2020 2020 2020 2020 2020 206d 6f64 656c             model
-00002b80: 7320 3d20 7961 6d6c 2e73 6166 655f 6c6f  s = yaml.safe_lo
-00002b90: 6164 2866 290d 0a20 2020 2020 2020 2020  ad(f)..         
-00002ba0: 2020 2020 2020 2069 735f 696e 7374 616c         is_instal
-00002bb0: 6c65 6420 3d20 2873 656c 662e 6c6f 6c6c  led = (self.loll
-00002bc0: 6d73 5f61 7070 2e6c 6f6c 6c6d 735f 7061  ms_app.lollms_pa
-00002bd0: 7468 732e 7065 7273 6f6e 616c 5f63 6f6e  ths.personal_con
-00002be0: 6669 6775 7261 7469 6f6e 5f70 6174 682f  figuration_path/
-00002bf0: 6622 6269 6e64 696e 675f 7b70 2e6e 616d  f"binding_{p.nam
-00002c00: 657d 2e79 616d 6c22 292e 6578 6973 7473  e}.yaml").exists
-00002c10: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00002c20: 2020 2020 656e 7472 793d 6622 7b41 5343      entry=f"{ASC
-00002c30: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f67  IIColors.color_g
-00002c40: 7265 656e 2069 6620 6973 5f69 6e73 7461  reen if is_insta
-00002c50: 6c6c 6564 2065 6c73 6520 2727 7d7b 272a  lled else ''}{'*
-00002c60: 2720 6966 2073 656c 662e 6c6f 6c6c 6d73  ' if self.lollms
-00002c70: 5f61 7070 2e63 6f6e 6669 675b 2762 696e  _app.config['bin
-00002c80: 6469 6e67 5f6e 616d 6527 5d3d 3d63 6172  ding_name']==car
-00002c90: 645b 276e 616d 6527 5d20 656c 7365 2027  d['name'] else '
-00002ca0: 277d 207b 6361 7264 5b27 6e61 6d65 275d  '} {card['name']
-00002cb0: 7d20 2862 7920 7b63 6172 645b 2761 7574  } (by {card['aut
-00002cc0: 686f 7227 5d7d 2922 0d0a 2020 2020 2020  hor']})"..      
-00002cd0: 2020 2020 2020 2020 2020 6269 6e64 696e            bindin
-00002ce0: 6773 5f6c 6973 742e 6170 7065 6e64 2865  gs_list.append(e
-00002cf0: 6e74 7279 290d 0a20 2020 2020 2020 2020  ntry)..         
-00002d00: 2020 2020 2020 2065 6e74 7279 3d7b 0d0a         entry={..
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 226e 616d 6522 3a70 2e6e 616d      "name":p.nam
-00002d30: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00002d40: 2020 2020 2020 2020 2263 6172 6422 3a63          "card":c
-00002d50: 6172 642c 0d0a 2020 2020 2020 2020 2020  ard,..          
-00002d60: 2020 2020 2020 2020 2020 226d 6f64 656c            "model
-00002d70: 7322 3a6d 6f64 656c 732c 0d0a 2020 2020  s":models,..    
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2269 6e73 7461 6c6c 6564 223a 2069 735f  "installed": is_
-00002da0: 696e 7374 616c 6c65 640d 0a20 2020 2020  installed..     
-00002db0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002dd0: 6c66 2e62 696e 6469 6e67 5f69 6e66 732e  lf.binding_infs.
-00002de0: 6170 7065 6e64 2865 6e74 7279 290d 0a20  append(entry).. 
-00002df0: 2020 2020 2020 2062 696e 6469 6e67 735f         bindings_
-00002e00: 6c69 7374 202b 3d20 5b22 4261 636b 225d  list += ["Back"]
-00002e10: 0d0a 2020 2020 2020 2020 6368 6f69 6365  ..        choice
-00002e20: 203d 2073 656c 662e 7368 6f77 5f6d 656e   = self.show_men
-00002e30: 7528 6269 6e64 696e 6773 5f6c 6973 7429  u(bindings_list)
-00002e40: 0d0a 2020 2020 2020 2020 6966 2031 203c  ..        if 1 <
-00002e50: 3d20 6368 6f69 6365 203c 3d20 6c65 6e28  = choice <= len(
-00002e60: 6269 6e64 696e 6773 5f6c 6973 7429 2d31  bindings_list)-1
-00002e70: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00002e80: 7269 6e74 2866 2259 6f75 2073 656c 6563  rint(f"You selec
-00002e90: 7465 6420 6269 6e64 696e 673a 207b 4153  ted binding: {AS
-00002ea0: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
-00002eb0: 6772 6565 6e7d 7b73 656c 662e 6269 6e64  green}{self.bind
-00002ec0: 696e 675f 696e 6673 5b63 686f 6963 6520  ing_infs[choice 
-00002ed0: 2d20 315d 5b27 6e61 6d65 275d 7d7b 4153  - 1]['name']}{AS
-00002ee0: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
-00002ef0: 7265 7365 747d 2229 0d0a 2020 2020 2020  reset}")..      
-00002f00: 2020 2020 2020 7365 6c66 2e6c 6f6c 6c6d        self.lollm
-00002f10: 735f 6170 702e 636f 6e66 6967 5b27 6269  s_app.config['bi
-00002f20: 6e64 696e 675f 6e61 6d65 275d 3d73 656c  nding_name']=sel
-00002f30: 662e 6269 6e64 696e 675f 696e 6673 5b63  f.binding_infs[c
-00002f40: 686f 6963 6520 2d20 315d 5b27 6e61 6d65  hoice - 1]['name
-00002f50: 275d 0d0a 2020 2020 2020 2020 2020 2020  ']..            
-00002f60: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
-00002f70: 6269 6e64 696e 6720 3d20 7365 6c66 2e6c  binding = self.l
-00002f80: 6f6c 6c6d 735f 6170 702e 6c6f 6164 5f62  ollms_app.load_b
-00002f90: 696e 6469 6e67 2829 0d0a 2020 2020 2020  inding()..      
-00002fa0: 2020 2020 2020 7365 6c66 2e6c 6f6c 6c6d        self.lollm
-00002fb0: 735f 6170 702e 636f 6e66 6967 5b27 6d6f  s_app.config['mo
-00002fc0: 6465 6c5f 6e61 6d65 275d 3d4e 6f6e 650d  del_name']=None.
-00002fd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00002fe0: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
-00002ff0: 6669 672e 7361 7665 5f63 6f6e 6669 6728  fig.save_config(
-00003000: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00003010: 6368 6f69 6365 203c 3d20 6c65 6e28 6269  choice <= len(bi
-00003020: 6e64 696e 6773 5f6c 6973 7429 3a0d 0a20  ndings_list):.. 
-00003030: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00003040: 6e0d 0a20 2020 2020 2020 2065 6c73 653a  n..        else:
-00003050: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00003060: 696e 7428 2249 6e76 616c 6964 2063 686f  int("Invalid cho
-00003070: 6963 6521 2229 0d0a 0d0a 2020 2020 6465  ice!")....    de
-00003080: 6620 7365 6c65 6374 5f6d 6f64 656c 2873  f select_model(s
-00003090: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
-000030a0: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
-000030b0: 7072 696e 7428 6622 7b41 5343 4949 436f  print(f"{ASCIICo
-000030c0: 6c6f 7273 2e63 6f6c 6f72 5f67 7265 656e  lors.color_green
-000030d0: 7d43 7572 7265 6e74 2062 696e 6469 6e67  }Current binding
-000030e0: 3a20 7b41 5343 4949 436f 6c6f 7273 2e63  : {ASCIIColors.c
-000030f0: 6f6c 6f72 5f72 6573 6574 7d7b 7365 6c66  olor_reset}{self
-00003100: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
-00003110: 6967 5b27 6269 6e64 696e 675f 6e61 6d65  ig['binding_name
-00003120: 275d 7d22 290d 0a20 2020 2020 2020 2070  ']}")..        p
-00003130: 7269 6e74 2866 227b 4153 4349 4943 6f6c  rint(f"{ASCIICol
-00003140: 6f72 732e 636f 6c6f 725f 6772 6565 6e7d  ors.color_green}
-00003150: 4375 7272 656e 7420 6d6f 6465 6c3a 207b  Current model: {
-00003160: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
-00003170: 725f 7265 7365 747d 7b73 656c 662e 6c6f  r_reset}{self.lo
-00003180: 6c6c 6d73 5f61 7070 2e63 6f6e 6669 675b  llms_app.config[
-00003190: 276d 6f64 656c 5f6e 616d 6527 5d7d 2229  'model_name']}")
-000031a0: 0d0a 0d0a 2020 2020 2020 2020 6d6f 6465  ....        mode
-000031b0: 6c73 5f64 6972 3a50 6174 6820 3d20 2873  ls_dir:Path = (s
-000031c0: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e6c  elf.lollms_app.l
-000031d0: 6f6c 6c6d 735f 7061 7468 732e 7065 7273  ollms_paths.pers
-000031e0: 6f6e 616c 5f6d 6f64 656c 735f 7061 7468  onal_models_path
-000031f0: 2f73 656c 662e 6c6f 6c6c 6d73 5f61 7070  /self.lollms_app
-00003200: 2e63 6f6e 6669 675b 2762 696e 6469 6e67  .config['binding
-00003210: 5f6e 616d 6527 5d29 0d0a 2020 2020 2020  _name'])..      
-00003220: 2020 6d6f 6465 6c73 5f64 6972 2e6d 6b64    models_dir.mkd
-00003230: 6972 2870 6172 656e 7473 3d54 7275 652c  ir(parents=True,
-00003240: 2065 7869 7374 5f6f 6b3d 5472 7565 290d   exist_ok=True).
-00003250: 0a0d 0a20 2020 2020 2020 206d 6f64 656c  ...        model
-00003260: 735f 6c69 7374 203d 2073 656c 662e 6c6f  s_list = self.lo
-00003270: 6c6c 6d73 5f61 7070 2e62 696e 6469 6e67  llms_app.binding
-00003280: 2e6c 6973 745f 6d6f 6465 6c73 2873 656c  .list_models(sel
-00003290: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
-000032a0: 6669 6729 202b 205b 2249 6e73 7461 6c6c  fig) + ["Install
-000032b0: 206d 6f64 656c 222c 2022 4368 616e 6765   model", "Change
-000032c0: 2062 696e 6469 6e67 222c 2022 4261 636b   binding", "Back
-000032d0: 225d 0d0a 2020 2020 2020 2020 6368 6f69  "]..        choi
-000032e0: 6365 203d 2073 656c 662e 7368 6f77 5f6d  ce = self.show_m
-000032f0: 656e 7528 6d6f 6465 6c73 5f6c 6973 7429  enu(models_list)
-00003300: 0d0a 2020 2020 2020 2020 6966 2031 203c  ..        if 1 <
-00003310: 3d20 6368 6f69 6365 203c 3d20 6c65 6e28  = choice <= len(
-00003320: 6d6f 6465 6c73 5f6c 6973 7429 2d33 3a0d  models_list)-3:.
-00003330: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00003340: 6e74 2866 2259 6f75 2073 656c 6563 7465  nt(f"You selecte
-00003350: 6420 6d6f 6465 6c3a 207b 4153 4349 4943  d model: {ASCIIC
-00003360: 6f6c 6f72 732e 636f 6c6f 725f 6772 6565  olors.color_gree
-00003370: 6e7d 7b6d 6f64 656c 735f 6c69 7374 5b63  n}{models_list[c
-00003380: 686f 6963 6520 2d20 315d 7d7b 4153 4349  hoice - 1]}{ASCI
-00003390: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
-000033a0: 7365 747d 2229 0d0a 2020 2020 2020 2020  set}")..        
-000033b0: 2020 2020 7365 6c66 2e6c 6f6c 6c6d 735f      self.lollms_
-000033c0: 6170 702e 636f 6e66 6967 5b27 6d6f 6465  app.config['mode
-000033d0: 6c5f 6e61 6d65 275d 3d6d 6f64 656c 735f  l_name']=models_
-000033e0: 6c69 7374 5b63 686f 6963 6520 2d20 315d  list[choice - 1]
-000033f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00003400: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
-00003410: 6e66 6967 2e73 6176 655f 636f 6e66 6967  nfig.save_config
-00003420: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00003430: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
-00003440: 6c6f 6164 5f6d 6f64 656c 2829 0d0a 2020  load_model()..  
-00003450: 2020 2020 2020 656c 6966 2063 686f 6963        elif choic
-00003460: 6520 3c3d 206c 656e 286d 6f64 656c 735f  e <= len(models_
-00003470: 6c69 7374 292d 323a 0d0a 2020 2020 2020  list)-2:..      
-00003480: 2020 2020 2020 7365 6c66 2e69 6e73 7461        self.insta
-00003490: 6c6c 5f6d 6f64 656c 2829 0d0a 2020 2020  ll_model()..    
-000034a0: 2020 2020 656c 6966 2063 686f 6963 6520      elif choice 
-000034b0: 3c3d 206c 656e 286d 6f64 656c 735f 6c69  <= len(models_li
-000034c0: 7374 292d 313a 0d0a 2020 2020 2020 2020  st)-1:..        
-000034d0: 2020 2020 7365 6c66 2e73 656c 6563 745f      self.select_
-000034e0: 6269 6e64 696e 6728 290d 0a20 2020 2020  binding()..     
-000034f0: 2020 2020 2020 2073 656c 662e 7365 6c65         self.sele
-00003500: 6374 5f6d 6f64 656c 2829 0d0a 2020 2020  ct_model()..    
-00003510: 2020 2020 656c 6966 2063 686f 6963 6520      elif choice 
-00003520: 3c3d 206c 656e 286d 6f64 656c 735f 6c69  <= len(models_li
-00003530: 7374 293a 0d0a 2020 2020 2020 2020 2020  st):..          
-00003540: 2020 7265 7475 726e 0d0a 2020 2020 2020    return..      
-00003550: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-00003560: 2020 2020 2070 7269 6e74 2822 496e 7661       print("Inva
-00003570: 6c69 6420 6368 6f69 6365 2122 290d 0a0d  lid choice!")...
-00003580: 0a20 2020 2064 6566 2069 6e73 7461 6c6c  .    def install
-00003590: 5f6d 6f64 656c 2873 656c 6629 3a0d 0a0d  _model(self):...
-000035a0: 0a20 2020 2020 2020 206d 6f64 656c 735f  .        models_
-000035b0: 6c69 7374 203d 205b 2249 6e73 7461 6c6c  list = ["Install
-000035c0: 206d 6f64 656c 2066 726f 6d20 696e 7465   model from inte
-000035d0: 726e 6574 222c 2249 6e73 7461 6c6c 206d  rnet","Install m
-000035e0: 6f64 656c 2066 726f 6d20 6c6f 6361 6c20  odel from local 
-000035f0: 6669 6c65 222c 2242 6163 6b22 5d0d 0a20  file","Back"].. 
-00003600: 2020 2020 2020 2063 686f 6963 6520 3d20         choice = 
-00003610: 7365 6c66 2e73 686f 775f 6d65 6e75 286d  self.show_menu(m
-00003620: 6f64 656c 735f 6c69 7374 290d 0a20 2020  odels_list)..   
-00003630: 2020 2020 2069 6620 3120 3c3d 2063 686f       if 1 <= cho
-00003640: 6963 6520 3c3d 206c 656e 286d 6f64 656c  ice <= len(model
-00003650: 735f 6c69 7374 292d 323a 0d0a 2020 2020  s_list)-2:..    
-00003660: 2020 2020 2020 2020 7572 6c20 3d20 696e          url = in
-00003670: 7075 7428 2247 6976 6520 6120 5552 4c20  put("Give a URL 
-00003680: 746f 2074 6865 206d 6f64 656c 2074 6f20  to the model to 
-00003690: 6265 2064 6f77 6e6c 6f61 6465 6420 3a22  be downloaded :"
-000036a0: 290d 0a20 2020 2020 2020 2020 2020 2064  )..            d
-000036b0: 6566 2070 726f 6772 6573 735f 6361 6c6c  ef progress_call
-000036c0: 6261 636b 2862 6c6f 636b 732c 2062 6c6f  back(blocks, blo
-000036d0: 636b 5f73 697a 652c 2074 6f74 616c 5f73  ck_size, total_s
-000036e0: 697a 6529 3a0d 0a20 2020 2020 2020 2020  ize):..         
-000036f0: 2020 2020 2020 2074 7164 6d5f 6261 722e         tqdm_bar.
-00003700: 746f 7461 6c3d 746f 7461 6c5f 7369 7a65  total=total_size
-00003710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003720: 2020 7471 646d 5f62 6172 2e75 7064 6174    tqdm_bar.updat
-00003730: 6528 626c 6f63 6b5f 7369 7a65 290d 0a0d  e(block_size)...
-00003740: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
-00003750: 7361 6765 2065 7861 6d70 6c65 0d0a 2020  sage example..  
-00003760: 2020 2020 2020 2020 2020 7769 7468 2074            with t
-00003770: 7164 6d28 746f 7461 6c3d 3130 302c 2075  qdm(total=100, u
-00003780: 6e69 743d 2225 222c 2064 6573 633d 2244  nit="%", desc="D
-00003790: 6f77 6e6c 6f61 6420 5072 6f67 7265 7373  ownload Progress
-000037a0: 222c 206e 636f 6c73 3d38 3029 2061 7320  ", ncols=80) as 
-000037b0: 7471 646d 5f62 6172 3a0d 0a20 2020 2020  tqdm_bar:..     
-000037c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000037d0: 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e 6669  lollms_app.confi
-000037e0: 672e 646f 776e 6c6f 6164 5f6d 6f64 656c  g.download_model
-000037f0: 2875 726c 2c73 656c 662e 6c6f 6c6c 6d73  (url,self.lollms
-00003800: 5f61 7070 2e62 696e 6469 6e67 2c20 7072  _app.binding, pr
-00003810: 6f67 7265 7373 5f63 616c 6c62 6163 6b29  ogress_callback)
-00003820: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00003830: 6c66 2e73 656c 6563 745f 6d6f 6465 6c28  lf.select_model(
-00003840: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00003850: 6368 6f69 6365 203c 3d20 6c65 6e28 6d6f  choice <= len(mo
-00003860: 6465 6c73 5f6c 6973 7429 2d31 3a0d 0a20  dels_list)-1:.. 
-00003870: 2020 2020 2020 2020 2020 2070 6174 6820             path 
-00003880: 3d20 5061 7468 2869 6e70 7574 2822 4769  = Path(input("Gi
-00003890: 7665 2061 2070 6174 6820 746f 2074 6865  ve a path to the
-000038a0: 206d 6f64 656c 2074 6f20 6265 2075 7365   model to be use
-000038b0: 6420 6f6e 2079 6f75 7220 5043 3a22 2929  d on your PC:"))
-000038c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000038d0: 2070 6174 682e 6578 6973 7473 2829 3a0d   path.exists():.
-000038e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000038f0: 2073 656c 662e 6c6f 6c6c 6d73 5f61 7070   self.lollms_app
-00003900: 2e63 6f6e 6669 672e 7265 6665 7265 6e63  .config.referenc
-00003910: 655f 6d6f 6465 6c28 7061 7468 290d 0a20  e_model(path).. 
-00003920: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003930: 7365 6c65 6374 5f6d 6f64 656c 2829 0d0a  select_model()..
-00003940: 2020 2020 2020 2020 656c 6966 2063 686f          elif cho
-00003950: 6963 6520 3c3d 206c 656e 286d 6f64 656c  ice <= len(model
-00003960: 735f 6c69 7374 293a 0d0a 2020 2020 2020  s_list):..      
-00003970: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00003980: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
-00003990: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
-000039a0: 496e 7661 6c69 6420 6368 6f69 6365 2122  Invalid choice!"
-000039b0: 290d 0a0d 0a20 2020 2064 6566 206d 6f75  )....    def mou
-000039c0: 6e74 5f70 6572 736f 6e61 6c69 7479 2873  nt_personality(s
-000039d0: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
-000039e0: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
-000039f0: 4153 4349 4943 6f6c 6f72 732e 7265 6428  ASCIIColors.red(
-00003a00: 6622 4d6f 756e 7465 6420 7065 7273 6f6e  f"Mounted person
-00003a10: 616c 6974 6965 733a 2229 0d0a 2020 2020  alities:")..    
-00003a20: 2020 2020 666f 7220 692c 7065 7273 6f6e      for i,person
-00003a30: 616c 6974 7920 696e 2065 6e75 6d65 7261  ality in enumera
-00003a40: 7465 2873 656c 662e 6c6f 6c6c 6d73 5f61  te(self.lollms_a
-00003a50: 7070 2e63 6f6e 6669 675b 2770 6572 736f  pp.config['perso
-00003a60: 6e61 6c69 7469 6573 275d 293a 0d0a 2020  nalities']):..  
-00003a70: 2020 2020 2020 2020 2020 6966 2069 3d3d            if i==
-00003a80: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
-00003a90: 636f 6e66 6967 5b27 6163 7469 7665 5f70  config['active_p
-00003aa0: 6572 736f 6e61 6c69 7479 5f69 6427 5d3a  ersonality_id']:
-00003ab0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ac0: 2020 4153 4349 4943 6f6c 6f72 732e 6772    ASCIIColors.gr
-00003ad0: 6565 6e28 7065 7273 6f6e 616c 6974 7929  een(personality)
-00003ae0: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00003af0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003b00: 2020 2020 2041 5343 4949 436f 6c6f 7273       ASCIIColors
-00003b10: 2e79 656c 6c6f 7728 7065 7273 6f6e 616c  .yellow(personal
-00003b20: 6974 7929 0d0a 2020 2020 2020 2020 7065  ity)..        pe
-00003b30: 7273 6f6e 616c 6974 795f 6c61 6e67 7561  rsonality_langua
-00003b40: 6765 7320 3d20 5b70 2e73 7465 6d20 666f  ges = [p.stem fo
-00003b50: 7220 7020 696e 2073 656c 662e 6c6f 6c6c  r p in self.loll
-00003b60: 6d73 5f61 7070 2e6c 6f6c 6c6d 735f 7061  ms_app.lollms_pa
-00003b70: 7468 732e 7065 7273 6f6e 616c 6974 6965  ths.personalitie
-00003b80: 735f 7a6f 6f5f 7061 7468 2e69 7465 7264  s_zoo_path.iterd
-00003b90: 6972 2829 2069 6620 702e 6973 5f64 6972  ir() if p.is_dir
-00003ba0: 2829 2061 6e64 206e 6f74 2070 2e6e 616d  () and not p.nam
-00003bb0: 652e 7374 6172 7473 7769 7468 2822 2e22  e.startswith("."
-00003bc0: 295d 202b 205b 2242 6163 6b22 5d0d 0a20  )] + ["Back"].. 
-00003bd0: 2020 2020 2020 2070 7269 6e74 2822 5365         print("Se
-00003be0: 6c65 6374 206c 616e 6775 6167 6522 290d  lect language").
-00003bf0: 0a20 2020 2020 2020 2063 686f 6963 6520  .        choice 
-00003c00: 3d20 7365 6c66 2e73 686f 775f 6d65 6e75  = self.show_menu
-00003c10: 2870 6572 736f 6e61 6c69 7479 5f6c 616e  (personality_lan
-00003c20: 6775 6167 6573 290d 0a20 2020 2020 2020  guages)..       
-00003c30: 2069 6620 3120 3c3d 2063 686f 6963 6520   if 1 <= choice 
-00003c40: 3c3d 206c 656e 2870 6572 736f 6e61 6c69  <= len(personali
-00003c50: 7479 5f6c 616e 6775 6167 6573 292d 313a  ty_languages)-1:
-00003c60: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-00003c70: 6e67 7561 6765 203d 2070 6572 736f 6e61  nguage = persona
-00003c80: 6c69 7479 5f6c 616e 6775 6167 6573 5b63  lity_languages[c
-00003c90: 686f 6963 6520 2d20 315d 0d0a 2020 2020  hoice - 1]..    
-00003ca0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-00003cb0: 596f 7520 7365 6c65 6374 6564 206c 616e  You selected lan
-00003cc0: 6775 6167 653a 207b 4153 4349 4943 6f6c  guage: {ASCIICol
-00003cd0: 6f72 732e 636f 6c6f 725f 6772 6565 6e7d  ors.color_green}
-00003ce0: 7b6c 616e 6775 6167 657d 7b41 5343 4949  {language}{ASCII
-00003cf0: 436f 6c6f 7273 2e63 6f6c 6f72 5f72 6573  Colors.color_res
-00003d00: 6574 7d22 290d 0a20 2020 2020 2020 2020  et}")..         
-00003d10: 2020 2070 6572 736f 6e61 6c69 7479 5f63     personality_c
-00003d20: 6174 6567 6f72 6965 7320 3d20 5b70 2e73  ategories = [p.s
-00003d30: 7465 6d20 666f 7220 7020 696e 2028 7365  tem for p in (se
-00003d40: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 6c6f  lf.lollms_app.lo
-00003d50: 6c6c 6d73 5f70 6174 6873 2e70 6572 736f  llms_paths.perso
-00003d60: 6e61 6c69 7469 6573 5f7a 6f6f 5f70 6174  nalities_zoo_pat
-00003d70: 682f 6c61 6e67 7561 6765 292e 6974 6572  h/language).iter
-00003d80: 6469 7228 2920 6966 2070 2e69 735f 6469  dir() if p.is_di
-00003d90: 7228 2920 616e 6420 6e6f 7420 702e 6e61  r() and not p.na
-00003da0: 6d65 2e73 7461 7274 7377 6974 6828 222e  me.startswith(".
-00003db0: 2229 5d2b 5b22 4261 636b 225d 0d0a 2020  ")]+["Back"]..  
-00003dc0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00003dd0: 2253 656c 6563 7420 6361 7465 676f 7279  "Select category
-00003de0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00003df0: 6368 6f69 6365 203d 2073 656c 662e 7368  choice = self.sh
-00003e00: 6f77 5f6d 656e 7528 7065 7273 6f6e 616c  ow_menu(personal
-00003e10: 6974 795f 6361 7465 676f 7269 6573 290d  ity_categories).
-00003e20: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00003e30: 3120 3c3d 2063 686f 6963 6520 3c3d 206c  1 <= choice <= l
-00003e40: 656e 2870 6572 736f 6e61 6c69 7479 5f63  en(personality_c
-00003e50: 6174 6567 6f72 6965 7329 2d31 3a0d 0a20  ategories)-1:.. 
-00003e60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003e70: 6174 6567 6f72 7920 3d20 7065 7273 6f6e  ategory = person
-00003e80: 616c 6974 795f 6361 7465 676f 7269 6573  ality_categories
-00003e90: 5b63 686f 6963 6520 2d20 315d 0d0a 2020  [choice - 1]..  
-00003ea0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00003eb0: 696e 7428 6622 596f 7520 7365 6c65 6374  int(f"You select
-00003ec0: 6564 2063 6174 6567 6f72 793a 207b 4153  ed category: {AS
-00003ed0: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
-00003ee0: 6772 6565 6e7d 7b63 6174 6567 6f72 797d  green}{category}
-00003ef0: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
-00003f00: 6f72 5f72 6573 6574 7d22 290d 0a20 2020  or_reset}")..   
-00003f10: 2020 2020 2020 2020 2020 2020 2070 6572               per
-00003f20: 736f 6e61 6c69 7479 5f6e 616d 6573 203d  sonality_names =
-00003f30: 205b 702e 7374 656d 2066 6f72 2070 2069   [p.stem for p i
-00003f40: 6e20 2873 656c 662e 6c6f 6c6c 6d73 5f61  n (self.lollms_a
-00003f50: 7070 2e6c 6f6c 6c6d 735f 7061 7468 732e  pp.lollms_paths.
-00003f60: 7065 7273 6f6e 616c 6974 6965 735f 7a6f  personalities_zo
-00003f70: 6f5f 7061 7468 2f6c 616e 6775 6167 652f  o_path/language/
-00003f80: 6361 7465 676f 7279 292e 6974 6572 6469  category).iterdi
-00003f90: 7228 2920 6966 2070 2e69 735f 6469 7228  r() if p.is_dir(
-00003fa0: 2920 616e 6420 6e6f 7420 702e 6e61 6d65  ) and not p.name
-00003fb0: 2e73 7461 7274 7377 6974 6828 222e 2229  .startswith(".")
-00003fc0: 5d2b 5b22 4261 636b 225d 0d0a 2020 2020  ]+["Back"]..    
-00003fd0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00003fe0: 7428 2253 656c 6563 7420 7065 7273 6f6e  t("Select person
-00003ff0: 616c 6974 7922 290d 0a20 2020 2020 2020  ality")..       
-00004000: 2020 2020 2020 2020 2063 686f 6963 6520           choice 
-00004010: 3d20 7365 6c66 2e73 686f 775f 6d65 6e75  = self.show_menu
-00004020: 2870 6572 736f 6e61 6c69 7479 5f6e 616d  (personality_nam
-00004030: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
-00004040: 2020 2020 2069 6620 3120 3c3d 2063 686f       if 1 <= cho
-00004050: 6963 6520 3c3d 206c 656e 2870 6572 736f  ice <= len(perso
-00004060: 6e61 6c69 7479 5f6e 616d 6573 292d 313a  nality_names)-1:
-00004070: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00004080: 2020 2020 2020 6e61 6d65 203d 2070 6572        name = per
-00004090: 736f 6e61 6c69 7479 5f6e 616d 6573 5b63  sonality_names[c
-000040a0: 686f 6963 6520 2d20 315d 0d0a 2020 2020  hoice - 1]..    
-000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040c0: 7072 696e 7428 6622 596f 7520 7365 6c65  print(f"You sele
-000040d0: 6374 6564 2070 6572 736f 6e61 6c69 7479  cted personality
-000040e0: 3a20 7b41 5343 4949 436f 6c6f 7273 2e63  : {ASCIIColors.c
-000040f0: 6f6c 6f72 5f67 7265 656e 7d7b 6e61 6d65  olor_green}{name
-00004100: 7d7b 4153 4349 4943 6f6c 6f72 732e 636f  }{ASCIIColors.co
-00004110: 6c6f 725f 7265 7365 747d 2229 0d0a 2020  lor_reset}")..  
-00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004130: 2020 7365 6c66 2e6c 6f6c 6c6d 735f 6170    self.lollms_ap
-00004140: 702e 636f 6e66 6967 5b22 7065 7273 6f6e  p.config["person
-00004150: 616c 6974 6965 7322 5d2e 6170 7065 6e64  alities"].append
-00004160: 2866 227b 6c61 6e67 7561 6765 7d2f 7b63  (f"{language}/{c
-00004170: 6174 6567 6f72 797d 2f7b 6e61 6d65 7d22  ategory}/{name}"
-00004180: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004190: 2020 2020 2020 2073 656c 662e 6c6f 6c6c         self.loll
-000041a0: 6d73 5f61 7070 2e6d 6f75 6e74 5f70 6572  ms_app.mount_per
-000041b0: 736f 6e61 6c69 7479 286c 656e 2873 656c  sonality(len(sel
-000041c0: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
-000041d0: 6669 675b 2270 6572 736f 6e61 6c69 7469  fig["personaliti
-000041e0: 6573 225d 292d 3129 0d0a 2020 2020 2020  es"])-1)..      
-000041f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004200: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
-00004210: 6e66 6967 2e73 6176 655f 636f 6e66 6967  nfig.save_config
-00004220: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00004230: 2020 2020 2020 2020 7072 696e 7428 2250          print("P
-00004240: 6572 736f 6e61 6c69 7479 206d 6f75 6e74  ersonality mount
-00004250: 6564 2073 7563 6365 7373 6675 6c6c 7921  ed successfully!
-00004260: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00004270: 2020 2020 656c 6966 2031 203c 3d20 6368      elif 1 <= ch
-00004280: 6f69 6365 203c 3d20 6c65 6e28 7065 7273  oice <= len(pers
-00004290: 6f6e 616c 6974 795f 6e61 6d65 7329 3a0d  onality_names):.
-000042a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042b0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
-000042c0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000042d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000042e0: 2020 2020 2020 2020 7072 696e 7428 2249          print("I
-000042f0: 6e76 616c 6964 2063 686f 6963 6521 2229  nvalid choice!")
-00004300: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-00004310: 6966 2031 203c 3d20 6368 6f69 6365 203c  if 1 <= choice <
-00004320: 3d20 6c65 6e28 7065 7273 6f6e 616c 6974  = len(personalit
-00004330: 795f 6361 7465 676f 7269 6573 293a 0d0a  y_categories):..
-00004340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004350: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
-00004360: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00004370: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00004380: 2822 496e 7661 6c69 6420 6368 6f69 6365  ("Invalid choice
-00004390: 2122 290d 0a20 2020 2020 2020 2065 6c69  !")..        eli
-000043a0: 6620 3120 3c3d 2063 686f 6963 6520 3c3d  f 1 <= choice <=
-000043b0: 206c 656e 2870 6572 736f 6e61 6c69 7479   len(personality
-000043c0: 5f6c 616e 6775 6167 6573 293a 0d0a 2020  _languages):..  
-000043d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000043e0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-000043f0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004400: 6e74 2822 496e 7661 6c69 6420 6368 6f69  nt("Invalid choi
-00004410: 6365 2122 290d 0a0d 0a20 2020 2064 6566  ce!")....    def
-00004420: 2076 6577 5f6d 6f75 6e74 6564 5f70 6572   vew_mounted_per
-00004430: 736f 6e61 6c69 7469 6573 2873 656c 6629  sonalities(self)
-00004440: 3a0d 0a20 2020 2020 2020 2041 5343 4949  :..        ASCII
-00004450: 436f 6c6f 7273 2e69 6e66 6f28 2248 6572  Colors.info("Her
-00004460: 6520 6973 2074 6865 206c 6973 7420 6f66  e is the list of
-00004470: 206d 6f75 6e74 6564 2070 6572 736f 6e61   mounted persona
-00004480: 6c69 7469 6573 2229 0d0a 2020 2020 2020  lities")..      
-00004490: 2020 656e 7472 6965 7320 3d20 7365 6c66    entries = self
-000044a0: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
-000044b0: 6967 5b27 7065 7273 6f6e 616c 6974 6965  ig['personalitie
-000044c0: 7327 5d0d 0a20 2020 2020 2020 2066 6f72  s']..        for
-000044d0: 2069 642c 2065 6e74 7279 2069 6e20 656e   id, entry in en
-000044e0: 756d 6572 6174 6528 656e 7472 6965 7329  umerate(entries)
-000044f0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-00004500: 6620 6964 2021 3d20 7365 6c66 2e6c 6f6c  f id != self.lol
-00004510: 6c6d 735f 6170 702e 636f 6e66 6967 2e61  lms_app.config.a
-00004520: 6374 6976 655f 7065 7273 6f6e 616c 6974  ctive_personalit
-00004530: 795f 6964 3a0d 0a20 2020 2020 2020 2020  y_id:..         
-00004540: 2020 2020 2020 2041 5343 4949 436f 6c6f         ASCIIColo
-00004550: 7273 2e79 656c 6c6f 7728 6622 7b69 642b  rs.yellow(f"{id+
-00004560: 317d 202d 207b 656e 7472 797d 2229 0d0a  1} - {entry}")..
-00004570: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00004580: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00004590: 2020 2041 5343 4949 436f 6c6f 7273 2e67     ASCIIColors.g
-000045a0: 7265 656e 2866 227b 6964 2b31 7d20 2d20  reen(f"{id+1} - 
+00001390: 706c 6963 6174 696f 6e27 2c20 6361 6c6c  plication', call
+000013a0: 6261 636b 3d4e 6f6e 6529 3a0d 0a20 2020  back=None):..   
+000013b0: 2020 2020 2073 656c 662e 6269 6e64 696e       self.bindin
+000013c0: 675f 696e 6673 203d 205b 5d0d 0a20 2020  g_infs = []..   
+000013d0: 2020 2020 2073 656c 662e 6c6f 6c6c 6d73       self.lollms
+000013e0: 5f61 7070 203d 206c 6f6c 6c6d 735f 6170  _app = lollms_ap
+000013f0: 700d 0a20 2020 2020 2020 2073 656c 662e  p..        self.
+00001400: 6361 6c6c 6261 636b 203d 2063 616c 6c62  callback = callb
+00001410: 6163 6b0d 0a20 2020 2020 2020 206d 6169  ack..        mai
+00001420: 6e5f 6d65 6e75 5f6f 7074 696f 6e73 203d  n_menu_options =
+00001430: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00001440: 7b27 6e61 6d65 273a 2027 4d61 696e 2073  {'name': 'Main s
+00001450: 6574 7469 6e67 7327 2c20 2766 6e27 3a20  ettings', 'fn': 
+00001460: 7365 6c66 2e6d 6169 6e5f 7365 7474 696e  self.main_settin
+00001470: 6773 2c20 2768 656c 7027 3a20 2253 686f  gs, 'help': "Sho
+00001480: 7720 6d61 696e 2073 6574 7469 6e67 732e  w main settings.
+00001490: 227d 2c0d 0a20 2020 2020 2020 2020 2020  "},..           
+000014a0: 207b 276e 616d 6527 3a20 2753 656c 6563   {'name': 'Selec
+000014b0: 7420 4269 6e64 696e 6727 2c20 2766 6e27  t Binding', 'fn'
+000014c0: 3a20 7365 6c66 2e73 656c 6563 745f 6269  : self.select_bi
+000014d0: 6e64 696e 672c 2027 6865 6c70 273a 2022  nding, 'help': "
+000014e0: 4368 6f6f 7365 2061 2062 696e 6469 6e67  Choose a binding
+000014f0: 2e22 7d2c 0d0a 2020 2020 2020 2020 2020  ."},..          
+00001500: 2020 7b27 6e61 6d65 273a 2027 5365 6c65    {'name': 'Sele
+00001510: 6374 204d 6f64 656c 272c 2027 666e 273a  ct Model', 'fn':
+00001520: 2073 656c 662e 7365 6c65 6374 5f6d 6f64   self.select_mod
+00001530: 656c 2c20 2768 656c 7027 3a20 2243 686f  el, 'help': "Cho
+00001540: 6f73 6520 6120 6d6f 6465 6c2e 227d 2c0d  ose a model."},.
+00001550: 0a20 2020 2020 2020 2020 2020 207b 276e  .            {'n
+00001560: 616d 6527 3a20 2756 6965 7720 6d6f 756e  ame': 'View moun
+00001570: 7465 6420 5065 7273 6f6e 616c 6974 6965  ted Personalitie
+00001580: 7327 2c20 2766 6e27 3a20 7365 6c66 2e76  s', 'fn': self.v
+00001590: 6577 5f6d 6f75 6e74 6564 5f70 6572 736f  ew_mounted_perso
+000015a0: 6e61 6c69 7469 6573 2c20 2768 656c 7027  nalities, 'help'
+000015b0: 3a20 2256 6965 7720 616c 6c20 6375 7272  : "View all curr
+000015c0: 656e 746c 7920 6d6f 756e 7465 6420 7065  ently mounted pe
+000015d0: 7273 6f6e 616c 6974 6965 732e 227d 2c0d  rsonalities."},.
+000015e0: 0a20 2020 2020 2020 2020 2020 207b 276e  .            {'n
+000015f0: 616d 6527 3a20 274d 6f75 6e74 2050 6572  ame': 'Mount Per
+00001600: 736f 6e61 6c69 7479 272c 2027 666e 273a  sonality', 'fn':
+00001610: 2073 656c 662e 6d6f 756e 745f 7065 7273   self.mount_pers
+00001620: 6f6e 616c 6974 792c 2027 6865 6c70 273a  onality, 'help':
+00001630: 2022 4d6f 756e 7420 6120 6e65 7720 7065   "Mount a new pe
+00001640: 7273 6f6e 616c 6974 792e 227d 2c0d 0a20  rsonality."},.. 
+00001650: 2020 2020 2020 2020 2020 207b 276e 616d             {'nam
+00001660: 6527 3a20 2755 6e6d 6f75 6e74 2050 6572  e': 'Unmount Per
+00001670: 736f 6e61 6c69 7479 272c 2027 666e 273a  sonality', 'fn':
+00001680: 2073 656c 662e 756e 6d6f 756e 745f 7065   self.unmount_pe
+00001690: 7273 6f6e 616c 6974 792c 2027 6865 6c70  rsonality, 'help
+000016a0: 273a 2022 556e 6d6f 756e 7420 6120 7065  ': "Unmount a pe
+000016b0: 7273 6f6e 616c 6974 792e 227d 2c0d 0a20  rsonality."},.. 
+000016c0: 2020 2020 2020 2020 2020 207b 276e 616d             {'nam
+000016d0: 6527 3a20 2753 656c 6563 7420 5065 7273  e': 'Select Pers
+000016e0: 6f6e 616c 6974 7927 2c20 2766 6e27 3a20  onality', 'fn': 
+000016f0: 7365 6c66 2e73 656c 6563 745f 7065 7273  self.select_pers
+00001700: 6f6e 616c 6974 792c 2027 6865 6c70 273a  onality, 'help':
+00001710: 2022 4368 6f6f 7365 2061 2070 6572 736f   "Choose a perso
+00001720: 6e61 6c69 7479 2e22 7d2c 0d0a 2020 2020  nality."},..    
+00001730: 2020 2020 2020 2020 7b27 6e61 6d65 273a          {'name':
+00001740: 2027 5265 696e 7374 616c 6c20 4269 6e64   'Reinstall Bind
+00001750: 696e 6727 2c20 2766 6e27 3a20 7365 6c66  ing', 'fn': self
+00001760: 2e72 6569 6e73 7461 6c6c 5f62 696e 6469  .reinstall_bindi
+00001770: 6e67 2c20 2768 656c 7027 3a20 2252 6569  ng, 'help': "Rei
+00001780: 6e73 7461 6c6c 2074 6865 2073 656c 6563  nstall the selec
+00001790: 7465 6420 6269 6e64 696e 672e 227d 2c0d  ted binding."},.
+000017a0: 0a20 2020 2020 2020 2020 2020 207b 276e  .            {'n
+000017b0: 616d 6527 3a20 2752 6569 6e73 7461 6c6c  ame': 'Reinstall
+000017c0: 2063 7572 7265 6e74 2050 6572 736f 6e61   current Persona
+000017d0: 6c69 7479 272c 2027 666e 273a 2073 656c  lity', 'fn': sel
+000017e0: 662e 7265 696e 7374 616c 6c5f 7065 7273  f.reinstall_pers
+000017f0: 6f6e 616c 6974 792c 2027 6865 6c70 273a  onality, 'help':
+00001800: 2022 5265 696e 7374 616c 6c20 7468 6520   "Reinstall the 
+00001810: 6375 7272 656e 7420 7365 6c65 6374 6564  current selected
+00001820: 2070 6572 736f 6e61 6c69 7479 2e22 7d2c   personality."},
+00001830: 0d0a 2020 2020 2020 2020 2020 2020 7b27  ..            {'
+00001840: 6e61 6d65 273a 2027 5265 7365 7420 616c  name': 'Reset al
+00001850: 6c20 696e 7374 616c 6c73 272c 2027 666e  l installs', 'fn
+00001860: 273a 2073 656c 662e 6c6f 6c6c 6d73 5f61  ': self.lollms_a
+00001870: 7070 2e72 6573 6574 5f61 6c6c 5f69 6e73  pp.reset_all_ins
+00001880: 7461 6c6c 732c 2027 6865 6c70 273a 2022  talls, 'help': "
+00001890: 5265 7365 7420 616c 6c20 696e 7374 616c  Reset all instal
+000018a0: 6c65 6420 7065 7273 6f6e 616c 6974 6965  led personalitie
+000018b0: 732e 227d 2c0d 0a20 2020 2020 2020 2020  s."},..         
+000018c0: 2020 207b 276e 616d 6527 3a20 2752 6573     {'name': 'Res
+000018d0: 6574 2070 6174 6873 272c 2027 666e 273a  et paths', 'fn':
+000018e0: 2073 656c 662e 6c6f 6c6c 6d73 5f61 7070   self.lollms_app
+000018f0: 2e6c 6f6c 6c6d 735f 7061 7468 732e 7265  .lollms_paths.re
+00001900: 7365 7450 6174 6873 2c20 2768 656c 7027  setPaths, 'help'
+00001910: 3a20 2252 6573 6574 2061 6c6c 2070 6174  : "Reset all pat
+00001920: 6873 2074 6f20 6465 6661 756c 742e 227d  hs to default."}
+00001930: 2c0d 0a20 2020 2020 2020 205d 0d0a 2020  ,..        ]..  
+00001940: 2020 2020 2020 7375 7065 7228 292e 5f5f        super().__
+00001950: 696e 6974 5f5f 2822 4c6f 6c6c 6d73 204d  init__("Lollms M
+00001960: 6169 6e20 6d65 6e75 222c 206d 6169 6e5f  ain menu", main_
+00001970: 6d65 6e75 5f6f 7074 696f 6e73 290d 0a0d  menu_options)...
+00001980: 0a20 2020 2064 6566 206d 6169 6e5f 7365  .    def main_se
+00001990: 7474 696e 6773 2873 656c 6629 3a0d 0a20  ttings(self):.. 
+000019a0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
+000019b0: 285b 0d0a 2020 2020 2020 2020 2020 2020  ([..            
+000019c0: 7b27 6e61 6d65 273a 2027 5365 7420 7573  {'name': 'Set us
+000019d0: 6572 206e 616d 6527 2c20 2766 6e27 3a20  er name', 'fn': 
+000019e0: 7365 6c66 2e73 6574 5f75 7365 725f 6e61  self.set_user_na
+000019f0: 6d65 2c20 2768 656c 7027 3a20 2253 6574  me, 'help': "Set
+00001a00: 7320 7468 6520 7573 6572 206e 616d 652e  s the user name.
+00001a10: 227d 2c0d 0a20 2020 2020 2020 2020 2020  "},..           
+00001a20: 207b 276e 616d 6527 3a20 2753 6574 2075   {'name': 'Set u
+00001a30: 7365 2075 7365 7220 6e61 6d65 2069 6e20  se user name in 
+00001a40: 6469 7363 7573 7369 6f6e 272c 2027 666e  discussion', 'fn
+00001a50: 273a 2073 656c 662e 7365 745f 7573 655f  ': self.set_use_
+00001a60: 7573 6572 5f6e 616d 655f 696e 5f64 6973  user_name_in_dis
+00001a70: 6375 7373 696f 6e73 2c20 2768 656c 7027  cussions, 'help'
+00001a80: 3a20 2253 6574 7320 7468 6520 7573 6572  : "Sets the user
+00001a90: 206e 616d 652e 227d 2c0d 0a20 2020 2020   name."},..     
+00001aa0: 2020 205d 290d 0a0d 0a20 2020 2064 6566     ])....    def
+00001ab0: 2073 6574 5f75 7365 725f 6e61 6d65 2873   set_user_name(s
+00001ac0: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00001ad0: 7269 6e74 2866 2243 7572 7265 6e74 2075  rint(f"Current u
+00001ae0: 7365 7220 6e61 6d65 203a 207b 7365 6c66  ser name : {self
+00001af0: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
+00001b00: 6967 2e75 7365 725f 6e61 6d65 7d22 290d  ig.user_name}").
+00001b10: 0a20 2020 2020 2020 2073 656c 662e 6c6f  .        self.lo
+00001b20: 6c6c 6d73 5f61 7070 2e63 6f6e 6669 672e  llms_app.config.
+00001b30: 7573 6572 5f6e 616d 6520 3d20 696e 7075  user_name = inpu
+00001b40: 7428 224e 6577 2075 7365 7220 6e61 6d65  t("New user name
+00001b50: 3a22 290d 0a20 2020 2020 2020 2073 656c  :")..        sel
+00001b60: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
+00001b70: 6669 672e 7361 7665 5f63 6f6e 6669 6728  fig.save_config(
+00001b80: 290d 0a0d 0a20 2020 2064 6566 2073 6574  )....    def set
+00001b90: 5f75 7365 5f75 7365 725f 6e61 6d65 5f69  _use_user_name_i
+00001ba0: 6e5f 6469 7363 7573 7369 6f6e 7328 7365  n_discussions(se
+00001bb0: 6c66 293a 0d0a 2020 2020 2020 2020 4153  lf):..        AS
+00001bc0: 4349 4943 6f6c 6f72 732e 696e 666f 2866  CIIColors.info(f
+00001bd0: 2243 7572 7265 6e74 2073 7461 7475 733a  "Current status:
+00001be0: 207b 7365 6c66 2e6c 6f6c 6c6d 735f 6170   {self.lollms_ap
+00001bf0: 702e 636f 6e66 6967 2e75 7365 5f75 7365  p.config.use_use
+00001c00: 725f 6e61 6d65 5f69 6e5f 6469 7363 7573  r_name_in_discus
+00001c10: 7369 6f6e 737d 2229 0d0a 2020 2020 2020  sions}")..      
+00001c20: 2020 7365 6c66 2e6c 6f6c 6c6d 735f 6170    self.lollms_ap
+00001c30: 702e 636f 6e66 6967 2e75 7365 5f75 7365  p.config.use_use
+00001c40: 725f 6e61 6d65 5f69 6e5f 6469 7363 7573  r_name_in_discus
+00001c50: 7369 6f6e 7320 3d20 7365 6c66 2e79 6573  sions = self.yes
+00001c60: 5f6e 6f5f 7175 6573 7469 6f6e 2827 5573  _no_question('Us
+00001c70: 6520 7573 6572 206e 616d 6520 696e 2064  e user name in d
+00001c80: 6963 7375 7373 696f 6e27 290d 0a20 2020  icsussion')..   
+00001c90: 2020 2020 2073 656c 662e 6c6f 6c6c 6d73       self.lollms
+00001ca0: 5f61 7070 2e63 6f6e 6669 672e 7361 7665  _app.config.save
+00001cb0: 5f63 6f6e 6669 6728 290d 0a0d 0a20 2020  _config()....   
+00001cc0: 2064 6566 2073 686f 775f 6c6f 676f 2873   def show_logo(s
+00001cd0: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00001ce0: 7269 6e74 2866 227b 4153 4349 4943 6f6c  rint(f"{ASCIICol
+00001cf0: 6f72 732e 636f 6c6f 725f 6272 6967 6874  ors.color_bright
+00001d00: 5f79 656c 6c6f 777d 2229 0d0a 2020 2020  _yellow}")..    
+00001d10: 2020 2020 7072 696e 7428 2220 2020 2020      print("     
+00001d20: 205f 5f5f 2020 2020 2020 205f 5f5f 2020   ___       ___  
+00001d30: 2020 2020 2020 2020 205f 5f5f 2020 2020           ___    
+00001d40: 2020 205f 5f5f 2020 2020 2020 205f 5f5f     ___       ___
+00001d50: 2020 2020 2020 2020 2020 205f 5f5f 2020             ___  
+00001d60: 2020 2020 2229 0d0a 2020 2020 2020 2020      ")..        
+00001d70: 7072 696e 7428 2220 2020 2020 2f5c 5f5f  print("     /\__
+00001d80: 5c20 2020 2020 2f5c 2020 5c20 2020 2020  \     /\  \     
+00001d90: 2020 2020 2f5c 5f5f 5c20 2020 2020 2f5c      /\__\     /\
+00001da0: 5f5f 5c20 2020 2020 2f5c 5f5f 5c20 2020  __\     /\__\   
+00001db0: 2020 2020 2020 2f5c 2020 5c20 2020 2020        /\  \     
+00001dc0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+00001dd0: 7428 2220 2020 202f 3a2f 2020 2f20 2020  t("    /:/  /   
+00001de0: 202f 3a3a 5c20 205c 2020 2020 2020 202f   /::\  \       /
+00001df0: 3a2f 2020 2f20 2020 202f 3a2f 2020 2f20  :/  /    /:/  / 
+00001e00: 2020 202f 3a3a 7c20 207c 2020 2020 2020     /::|  |      
+00001e10: 202f 3a3a 5c20 205c 2020 2020 2229 0d0a   /::\  \    ")..
+00001e20: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00001e30: 2020 2f3a 2f20 202f 2020 2020 2f3a 2f5c    /:/  /    /:/\
+00001e40: 3a5c 2020 5c20 2020 2020 2f3a 2f20 202f  :\  \     /:/  /
+00001e50: 2020 2020 2f3a 2f20 202f 2020 2020 2f3a      /:/  /    /:
+00001e60: 7c3a 7c20 207c 2020 2020 2020 2f3a 2f5c  |:|  |      /:/\
+00001e70: 205c 2020 5c20 2020 2229 0d0a 2020 2020   \  \   ")..    
+00001e80: 2020 2020 7072 696e 7428 2220 202f 3a2f      print("  /:/
+00001e90: 2020 2f20 2020 202f 3a2f 2020 5c3a 5c20    /    /:/  \:\ 
+00001ea0: 205c 2020 202f 3a2f 2020 2f20 2020 202f   \   /:/  /    /
+00001eb0: 3a2f 2020 2f20 2020 202f 3a2f 7c3a 7c5f  :/  /    /:/|:|_
+00001ec0: 5f7c 5f5f 2020 205f 5c3a 5c7e 5c20 5c20  _|__   _\:\~\ \ 
+00001ed0: 205c 2020 2229 0d0a 2020 2020 2020 2020   \  ")..        
+00001ee0: 7072 696e 7428 2220 2f3a 2f5f 5f2f 2020  print(" /:/__/  
+00001ef0: 2020 2f3a 2f5f 5f2f 205c 3a5c 5f5f 5c20    /:/__/ \:\__\ 
+00001f00: 2f3a 2f5f 5f2f 2020 2020 2f3a 2f5f 5f2f  /:/__/    /:/__/
+00001f10: 2020 2020 2f3a 2f20 7c3a 3a3a 3a5c 5f5f      /:/ |::::\__
+00001f20: 5c20 2f5c 205c 3a5c 205c 205c 5f5f 5c20  \ /\ \:\ \ \__\ 
+00001f30: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+00001f40: 7428 2220 5c3a 5c20 205c 2020 2020 5c3a  t(" \:\  \    \:
+00001f50: 5c20 205c 202f 3a2f 2020 2f20 5c3a 5c20  \  \ /:/  / \:\ 
+00001f60: 205c 2020 2020 5c3a 5c20 205c 2020 2020   \    \:\  \    
+00001f70: 5c2f 5f5f 2f7e 7e2f 3a2f 2020 2f20 5c3a  \/__/~~/:/  / \:
+00001f80: 5c20 5c3a 5c20 5c2f 5f5f 2f20 2229 0d0a  \ \:\ \/__/ ")..
+00001f90: 2020 2020 2020 2020 7072 696e 7428 2220          print(" 
+00001fa0: 205c 3a5c 2020 5c20 2020 205c 3a5c 2020   \:\  \    \:\  
+00001fb0: 2f3a 2f20 202f 2020 205c 3a5c 2020 5c20  /:/  /   \:\  \ 
+00001fc0: 2020 205c 3a5c 2020 5c20 2020 2020 2020     \:\  \       
+00001fd0: 2020 2f3a 2f20 202f 2020 205c 3a5c 205c    /:/  /   \:\ \
+00001fe0: 3a5c 5f5f 5c20 2020 2229 0d0a 2020 2020  :\__\   ")..    
+00001ff0: 2020 2020 7072 696e 7428 2220 2020 5c3a      print("   \:
+00002000: 5c20 205c 2020 2020 5c3a 5c2f 3a2f 2020  \  \    \:\/:/  
+00002010: 2f20 2020 2020 5c3a 5c20 205c 2020 2020  /     \:\  \    
+00002020: 5c3a 5c20 205c 2020 2020 2020 202f 3a2f  \:\  \       /:/
+00002030: 2020 2f20 2020 2020 5c3a 5c2f 3a2f 2020    /     \:\/:/  
+00002040: 2f20 2020 2229 0d0a 2020 2020 2020 2020  /   ")..        
+00002050: 7072 696e 7428 2220 2020 205c 3a5c 5f5f  print("    \:\__
+00002060: 5c20 2020 205c 3a3a 2f20 202f 2020 2020  \    \::/  /    
+00002070: 2020 205c 3a5c 5f5f 5c20 2020 205c 3a5c     \:\__\    \:\
+00002080: 5f5f 5c20 2020 2020 2f3a 2f20 202f 2020  __\     /:/  /  
+00002090: 2020 2020 205c 3a3a 2f20 202f 2020 2020       \::/  /    
+000020a0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+000020b0: 7428 2220 2020 2020 5c2f 5f5f 2f20 2020  t("     \/__/   
+000020c0: 2020 5c2f 5f5f 2f20 2020 2020 2020 2020    \/__/         
+000020d0: 5c2f 5f5f 2f20 2020 2020 5c2f 5f5f 2f20  \/__/     \/__/ 
+000020e0: 2020 2020 5c2f 5f5f 2f20 2020 2020 2020      \/__/       
+000020f0: 2020 5c2f 5f5f 2f20 2020 2020 2229 0d0a    \/__/     ")..
+00002100: 0d0a 0d0a 0d0a 0d0a 2020 2020 2020 2020  ........        
+00002110: 7072 696e 7428 6622 7b41 5343 4949 436f  print(f"{ASCIICo
+00002120: 6c6f 7273 2e63 6f6c 6f72 5f72 6573 6574  lors.color_reset
+00002130: 7d22 290d 0a20 2020 2020 2020 2070 7269  }")..        pri
+00002140: 6e74 2866 227b 4153 4349 4943 6f6c 6f72  nt(f"{ASCIIColor
+00002150: 732e 636f 6c6f 725f 7265 647d 5665 7273  s.color_red}Vers
+00002160: 696f 6e3a 207b 4153 4349 4943 6f6c 6f72  ion: {ASCIIColor
+00002170: 732e 636f 6c6f 725f 6772 6565 6e7d 7b70  s.color_green}{p
+00002180: 6b67 5f72 6573 6f75 7263 6573 2e67 6574  kg_resources.get
+00002190: 5f64 6973 7472 6962 7574 696f 6e28 276c  _distribution('l
+000021a0: 6f6c 6c6d 7327 292e 7665 7273 696f 6e7d  ollms').version}
+000021b0: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+000021c0: 7428 6622 7b41 5343 4949 436f 6c6f 7273  t(f"{ASCIIColors
+000021d0: 2e63 6f6c 6f72 5f72 6564 7d42 7920 3a20  .color_red}By : 
+000021e0: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
+000021f0: 6f72 5f67 7265 656e 7d50 6172 6973 4e65  or_green}ParisNe
+00002200: 6f22 290d 0a20 2020 2020 2020 2070 7269  o")..        pri
+00002210: 6e74 2866 227b 4153 4349 4943 6f6c 6f72  nt(f"{ASCIIColor
+00002220: 732e 636f 6c6f 725f 7265 7365 747d 2229  s.color_reset}")
+00002230: 0d0a 0d0a 2020 2020 6465 6620 7368 6f77  ....    def show
+00002240: 5f63 6f6d 6d61 6e64 735f 6c69 7374 2873  _commands_list(s
+00002250: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00002260: 7269 6e74 2829 0d0a 2020 2020 2020 2020  rint()..        
+00002270: 7072 696e 7428 2243 6f6d 6d61 6e64 733a  print("Commands:
+00002280: 2229 0d0a 2020 2020 2020 2020 7072 696e  ")..        prin
+00002290: 7428 6622 2020 207b 4153 4349 4943 6f6c  t(f"   {ASCIICol
+000022a0: 6f72 732e 636f 6c6f 725f 7265 647d e294  ors.color_red}..
+000022b0: 9c7b 4153 4349 4943 6f6c 6f72 732e 636f  .{ASCIIColors.co
+000022c0: 6c6f 725f 7265 7365 747d 206d 656e 753a  lor_reset} menu:
+000022d0: 2073 686f 7773 206d 6169 6e20 6d65 6e75   shows main menu
+000022e0: 2229 2020 2020 2020 2020 0d0a 2020 2020  ")        ..    
+000022f0: 2020 2020 7072 696e 7428 6622 2020 207b      print(f"   {
+00002300: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
+00002310: 725f 7265 647d e294 9c7b 4153 4349 4943  r_red}...{ASCIIC
+00002320: 6f6c 6f72 732e 636f 6c6f 725f 7265 7365  olors.color_rese
+00002330: 747d 2068 656c 703a 2073 686f 7773 2074  t} help: shows t
+00002340: 6869 7320 696e 666f 2229 2020 2020 2020  his info")      
+00002350: 2020 0d0a 2020 2020 2020 2020 7072 696e    ..        prin
+00002360: 7428 6622 2020 207b 4153 4349 4943 6f6c  t(f"   {ASCIICol
+00002370: 6f72 732e 636f 6c6f 725f 7265 647d e294  ors.color_red}..
+00002380: 9c7b 4153 4349 4943 6f6c 6f72 732e 636f  .{ASCIIColors.co
+00002390: 6c6f 725f 7265 7365 747d 2072 6573 6574  lor_reset} reset
+000023a0: 3a20 7265 7365 7473 2074 6865 2063 6f6e  : resets the con
+000023b0: 7465 7874 2229 0d0a 2020 2020 2020 2020  text")..        
+000023c0: 7072 696e 7428 6622 2020 207b 4153 4349  print(f"   {ASCI
+000023d0: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
+000023e0: 647d e294 9c7b 4153 4349 4943 6f6c 6f72  d}...{ASCIIColor
+000023f0: 732e 636f 6c6f 725f 7265 7365 747d 203c  s.color_reset} <
+00002400: 656d 7074 7920 7072 6f6d 7074 3e3a 2066  empty prompt>: f
+00002410: 6f72 6365 7320 7468 6520 6d6f 6465 6c20  orces the model 
+00002420: 746f 2063 6f6e 7469 6e75 6520 6765 6e65  to continue gene
+00002430: 7261 7469 6e67 2229 0d0a 2020 2020 2020  rating")..      
+00002440: 2020 7072 696e 7428 6622 2020 207b 4153    print(f"   {AS
+00002450: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
+00002460: 7265 647d e294 9c7b 4153 4349 4943 6f6c  red}...{ASCIICol
+00002470: 6f72 732e 636f 6c6f 725f 7265 7365 747d  ors.color_reset}
+00002480: 2063 6f6e 7465 7874 5f69 6e66 6f73 3a20   context_infos: 
+00002490: 6375 7272 656e 7420 636f 6e74 6578 7420  current context 
+000024a0: 7369 7a65 2061 6e64 2073 7061 6365 206c  size and space l
+000024b0: 6566 7420 6265 666f 7265 2063 726f 7070  eft before cropp
+000024c0: 696e 6722 290d 0a20 2020 2020 2020 2070  ing")..        p
+000024d0: 7269 6e74 2866 2220 2020 7b41 5343 4949  rint(f"   {ASCII
+000024e0: 436f 6c6f 7273 2e63 6f6c 6f72 5f72 6564  Colors.color_red
+000024f0: 7de2 949c 7b41 5343 4949 436f 6c6f 7273  }...{ASCIIColors
+00002500: 2e63 6f6c 6f72 5f72 6573 6574 7d20 7374  .color_reset} st
+00002510: 6172 745f 6c6f 673a 2073 7461 7274 7320  art_log: starts 
+00002520: 6c6f 6767 696e 6720 7468 6520 6469 7363  logging the disc
+00002530: 7573 7369 6f6e 2074 6f20 6120 7465 7874  ussion to a text
+00002540: 2066 696c 6522 290d 0a20 2020 2020 2020   file")..       
+00002550: 2070 7269 6e74 2866 2220 2020 7b41 5343   print(f"   {ASC
+00002560: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f72  IIColors.color_r
+00002570: 6564 7de2 949c 7b41 5343 4949 436f 6c6f  ed}...{ASCIIColo
+00002580: 7273 2e63 6f6c 6f72 5f72 6573 6574 7d20  rs.color_reset} 
+00002590: 7374 6f70 5f6c 6f67 3a20 7374 6f70 7320  stop_log: stops 
+000025a0: 6c6f 6767 696e 6720 7468 6520 6469 7363  logging the disc
+000025b0: 7573 7369 6f6e 2074 6f20 6120 7465 7874  ussion to a text
+000025c0: 2066 696c 6522 290d 0a20 2020 2020 2020   file")..       
+000025d0: 2070 7269 6e74 2866 2220 2020 7b41 5343   print(f"   {ASC
+000025e0: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f72  IIColors.color_r
+000025f0: 6564 7de2 949c 7b41 5343 4949 436f 6c6f  ed}...{ASCIIColo
+00002600: 7273 2e63 6f6c 6f72 5f72 6573 6574 7d20  rs.color_reset} 
+00002610: 7365 6e64 5f66 696c 653a 2075 706c 6f61  send_file: uploa
+00002620: 6473 2061 2066 696c 6520 746f 2074 6865  ds a file to the
+00002630: 2041 4922 290d 0a20 2020 2020 2020 2070   AI")..        p
+00002640: 7269 6e74 2866 2220 2020 7b41 5343 4949  rint(f"   {ASCII
+00002650: 436f 6c6f 7273 2e63 6f6c 6f72 5f72 6564  Colors.color_red
+00002660: 7de2 9494 7b41 5343 4949 436f 6c6f 7273  }...{ASCIIColors
+00002670: 2e63 6f6c 6f72 5f72 6573 6574 7d20 6578  .color_reset} ex
+00002680: 6974 3a20 6578 6973 7473 2074 6865 2063  it: exists the c
+00002690: 6f6e 736f 6c65 2229 0d0a 2020 2020 2020  onsole")..      
+000026a0: 2020 0d0a 2020 2020 2020 2020 6966 2073    ..        if s
+000026b0: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e70  elf.lollms_app.p
+000026c0: 6572 736f 6e61 6c69 7479 3a0d 0a20 2020  ersonality:..   
+000026d0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000026e0: 2e6c 6f6c 6c6d 735f 6170 702e 7065 7273  .lollms_app.pers
+000026f0: 6f6e 616c 6974 792e 6865 6c70 2021 3d22  onality.help !="
+00002700: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+00002710: 2020 2020 7072 696e 7428 6622 5065 7273      print(f"Pers
+00002720: 6f6e 616c 6974 7920 6865 6c70 3a22 290d  onality help:").
+00002730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002740: 2070 7269 6e74 2866 227b 7365 6c66 2e6c   print(f"{self.l
+00002750: 6f6c 6c6d 735f 6170 702e 7065 7273 6f6e  ollms_app.person
+00002760: 616c 6974 792e 6865 6c70 7d22 290d 0a20  ality.help}").. 
+00002770: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00002780: 2020 2020 200d 0a0d 0a20 2020 2064 6566       ....    def
+00002790: 2073 686f 775f 6d65 6e75 2873 656c 662c   show_menu(self,
+000027a0: 206f 7074 696f 6e73 2c20 7469 746c 653d   options, title=
+000027b0: 224d 656e 753a 222c 2073 656c 6563 7469  "Menu:", selecti
+000027c0: 6f6e 3a69 6e74 3d4e 6f6e 6529 3a0d 0a20  on:int=None):.. 
+000027d0: 2020 2020 2020 2041 5343 4949 436f 6c6f         ASCIIColo
+000027e0: 7273 2e79 656c 6c6f 7728 7469 746c 6529  rs.yellow(title)
+000027f0: 0d0a 2020 2020 2020 2020 666f 7220 696e  ..        for in
+00002800: 6465 782c 206f 7074 696f 6e20 696e 2065  dex, option in e
+00002810: 6e75 6d65 7261 7465 286f 7074 696f 6e73  numerate(options
+00002820: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00002830: 6966 2073 656c 6563 7469 6f6e 2069 7320  if selection is 
+00002840: 6e6f 7420 4e6f 6e65 2061 6e64 2069 6e64  not None and ind
+00002850: 6578 3d3d 7365 6c65 6374 696f 6e3a 0d0a  ex==selection:..
+00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002870: 7072 696e 7428 6622 7b41 5343 4949 436f  print(f"{ASCIICo
+00002880: 6c6f 7273 2e63 6f6c 6f72 5f67 7265 656e  lors.color_green
+00002890: 7d7b 696e 6465 7820 2b20 317d 202d 207b  }{index + 1} - {
+000028a0: 6f70 7469 6f6e 7d7b 4153 4349 4943 6f6c  option}{ASCIICol
+000028b0: 6f72 732e 636f 6c6f 725f 7265 7365 747d  ors.color_reset}
+000028c0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000028d0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000028e0: 2020 2020 2020 2070 7269 6e74 2866 227b         print(f"{
+000028f0: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
+00002900: 725f 6772 6565 6e7d 7b69 6e64 6578 202b  r_green}{index +
+00002910: 2031 7d20 2d7b 4153 4349 4943 6f6c 6f72   1} -{ASCIIColor
+00002920: 732e 636f 6c6f 725f 7265 7365 747d 207b  s.color_reset} {
+00002930: 6f70 7469 6f6e 7d22 290d 0a20 2020 2020  option}")..     
+00002940: 2020 2063 686f 6963 6520 3d20 696e 7075     choice = inpu
+00002950: 7428 2245 6e74 6572 2079 6f75 7220 6368  t("Enter your ch
+00002960: 6f69 6365 3a20 2229 0d0a 2020 2020 2020  oice: ")..      
+00002970: 2020 7265 7475 726e 2069 6e74 2863 686f    return int(cho
+00002980: 6963 6529 2069 6620 6368 6f69 6365 2e69  ice) if choice.i
+00002990: 7364 6967 6974 2829 2065 6c73 6520 2d31  sdigit() else -1
+000029a0: 0d0a 0d0a 2020 2020 6465 6620 7365 6c65  ....    def sele
+000029b0: 6374 5f62 696e 6469 6e67 2873 656c 6629  ct_binding(self)
+000029c0: 3a0d 0a20 2020 2020 2020 2062 696e 6469  :..        bindi
+000029d0: 6e67 735f 6c69 7374 203d 205b 5d0d 0a20  ngs_list = [].. 
+000029e0: 2020 2020 2020 2070 7269 6e74 2829 0d0a         print()..
+000029f0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
+00002a00: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
+00002a10: 6f72 5f67 7265 656e 7d43 7572 7265 6e74  or_green}Current
+00002a20: 2062 696e 6469 6e67 3a20 7b41 5343 4949   binding: {ASCII
+00002a30: 436f 6c6f 7273 2e63 6f6c 6f72 5f72 6573  Colors.color_res
+00002a40: 6574 7d7b 7365 6c66 2e6c 6f6c 6c6d 735f  et}{self.lollms_
+00002a50: 6170 702e 636f 6e66 6967 5b27 6269 6e64  app.config['bind
+00002a60: 696e 675f 6e61 6d65 275d 7d22 290d 0a20  ing_name']}").. 
+00002a70: 2020 2020 2020 2066 6f72 2070 2069 6e20         for p in 
+00002a80: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
+00002a90: 6c6f 6c6c 6d73 5f70 6174 6873 2e62 696e  lollms_paths.bin
+00002aa0: 6469 6e67 735f 7a6f 6f5f 7061 7468 2e69  dings_zoo_path.i
+00002ab0: 7465 7264 6972 2829 3a0d 0a20 2020 2020  terdir():..     
+00002ac0: 2020 2020 2020 2069 6620 702e 6973 5f64         if p.is_d
+00002ad0: 6972 2829 2061 6e64 206e 6f74 2070 2e73  ir() and not p.s
+00002ae0: 7465 6d2e 7374 6172 7473 7769 7468 2822  tem.startswith("
+00002af0: 2e22 293a 0d0a 2020 2020 2020 2020 2020  ."):..          
+00002b00: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00002b10: 702f 2262 696e 6469 6e67 5f63 6172 642e  p/"binding_card.
+00002b20: 7961 6d6c 222c 2022 7222 2920 6173 2066  yaml", "r") as f
+00002b30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002b40: 2020 2020 2020 2063 6172 6420 3d20 7961         card = ya
+00002b50: 6d6c 2e73 6166 655f 6c6f 6164 2866 290d  ml.safe_load(f).
+00002b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b70: 2077 6974 6820 6f70 656e 2870 2f22 6d6f   with open(p/"mo
+00002b80: 6465 6c73 2e79 616d 6c22 2c20 2272 2229  dels.yaml", "r")
+00002b90: 2061 7320 663a 0d0a 2020 2020 2020 2020   as f:..        
+00002ba0: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00002bb0: 6c73 203d 2079 616d 6c2e 7361 6665 5f6c  ls = yaml.safe_l
+00002bc0: 6f61 6428 6629 0d0a 2020 2020 2020 2020  oad(f)..        
+00002bd0: 2020 2020 2020 2020 6973 5f69 6e73 7461          is_insta
+00002be0: 6c6c 6564 203d 2028 7365 6c66 2e6c 6f6c  lled = (self.lol
+00002bf0: 6c6d 735f 6170 702e 6c6f 6c6c 6d73 5f70  lms_app.lollms_p
+00002c00: 6174 6873 2e70 6572 736f 6e61 6c5f 636f  aths.personal_co
+00002c10: 6e66 6967 7572 6174 696f 6e5f 7061 7468  nfiguration_path
+00002c20: 2f66 2262 696e 6469 6e67 5f7b 702e 6e61  /f"binding_{p.na
+00002c30: 6d65 7d2e 7961 6d6c 2229 2e65 7869 7374  me}.yaml").exist
+00002c40: 7328 290d 0a20 2020 2020 2020 2020 2020  s()..           
+00002c50: 2020 2020 2065 6e74 7279 3d66 227b 4153       entry=f"{AS
+00002c60: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
+00002c70: 6772 6565 6e20 6966 2069 735f 696e 7374  green if is_inst
+00002c80: 616c 6c65 6420 656c 7365 2027 277d 7b27  alled else ''}{'
+00002c90: 2a27 2069 6620 7365 6c66 2e6c 6f6c 6c6d  *' if self.lollm
+00002ca0: 735f 6170 702e 636f 6e66 6967 5b27 6269  s_app.config['bi
+00002cb0: 6e64 696e 675f 6e61 6d65 275d 3d3d 6361  nding_name']==ca
+00002cc0: 7264 5b27 6e61 6d65 275d 2065 6c73 6520  rd['name'] else 
+00002cd0: 2727 7d20 7b63 6172 645b 276e 616d 6527  ''} {card['name'
+00002ce0: 5d7d 2028 6279 207b 6361 7264 5b27 6175  ]} (by {card['au
+00002cf0: 7468 6f72 275d 7d29 220d 0a20 2020 2020  thor']})"..     
+00002d00: 2020 2020 2020 2020 2020 2062 696e 6469             bindi
+00002d10: 6e67 735f 6c69 7374 2e61 7070 656e 6428  ngs_list.append(
+00002d20: 656e 7472 7929 0d0a 2020 2020 2020 2020  entry)..        
+00002d30: 2020 2020 2020 2020 656e 7472 793d 7b0d          entry={.
+00002d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002d50: 2020 2020 2022 6e61 6d65 223a 702e 6e61       "name":p.na
+00002d60: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
+00002d70: 2020 2020 2020 2020 2022 6361 7264 223a           "card":
+00002d80: 6361 7264 2c0d 0a20 2020 2020 2020 2020  card,..         
+00002d90: 2020 2020 2020 2020 2020 2022 6d6f 6465             "mode
+00002da0: 6c73 223a 6d6f 6465 6c73 2c0d 0a20 2020  ls":models,..   
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002dc0: 2022 696e 7374 616c 6c65 6422 3a20 6973   "installed": is
+00002dd0: 5f69 6e73 7461 6c6c 6564 0d0a 2020 2020  _installed..    
+00002de0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
+00002df0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002e00: 656c 662e 6269 6e64 696e 675f 696e 6673  elf.binding_infs
+00002e10: 2e61 7070 656e 6428 656e 7472 7929 0d0a  .append(entry)..
+00002e20: 2020 2020 2020 2020 6269 6e64 696e 6773          bindings
+00002e30: 5f6c 6973 7420 2b3d 205b 2242 6163 6b22  _list += ["Back"
+00002e40: 5d0d 0a20 2020 2020 2020 2063 686f 6963  ]..        choic
+00002e50: 6520 3d20 7365 6c66 2e73 686f 775f 6d65  e = self.show_me
+00002e60: 6e75 2862 696e 6469 6e67 735f 6c69 7374  nu(bindings_list
+00002e70: 290d 0a20 2020 2020 2020 2069 6620 3120  )..        if 1 
+00002e80: 3c3d 2063 686f 6963 6520 3c3d 206c 656e  <= choice <= len
+00002e90: 2862 696e 6469 6e67 735f 6c69 7374 292d  (bindings_list)-
+00002ea0: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
+00002eb0: 7072 696e 7428 6622 596f 7520 7365 6c65  print(f"You sele
+00002ec0: 6374 6564 2062 696e 6469 6e67 3a20 7b41  cted binding: {A
+00002ed0: 5343 4949 436f 6c6f 7273 2e63 6f6c 6f72  SCIIColors.color
+00002ee0: 5f67 7265 656e 7d7b 7365 6c66 2e62 696e  _green}{self.bin
+00002ef0: 6469 6e67 5f69 6e66 735b 6368 6f69 6365  ding_infs[choice
+00002f00: 202d 2031 5d5b 276e 616d 6527 5d7d 7b41   - 1]['name']}{A
+00002f10: 5343 4949 436f 6c6f 7273 2e63 6f6c 6f72  SCIIColors.color
+00002f20: 5f72 6573 6574 7d22 290d 0a20 2020 2020  _reset}")..     
+00002f30: 2020 2020 2020 2073 656c 662e 6c6f 6c6c         self.loll
+00002f40: 6d73 5f61 7070 2e63 6f6e 6669 675b 2762  ms_app.config['b
+00002f50: 696e 6469 6e67 5f6e 616d 6527 5d3d 7365  inding_name']=se
+00002f60: 6c66 2e62 696e 6469 6e67 5f69 6e66 735b  lf.binding_infs[
+00002f70: 6368 6f69 6365 202d 2031 5d5b 276e 616d  choice - 1]['nam
+00002f80: 6527 5d0d 0a20 2020 2020 2020 2020 2020  e']..           
+00002f90: 2073 656c 662e 6c6f 6c6c 6d73 5f61 7070   self.lollms_app
+00002fa0: 2e62 696e 6469 6e67 203d 2073 656c 662e  .binding = self.
+00002fb0: 6c6f 6c6c 6d73 5f61 7070 2e6c 6f61 645f  lollms_app.load_
+00002fc0: 6269 6e64 696e 6728 290d 0a20 2020 2020  binding()..     
+00002fd0: 2020 2020 2020 2073 656c 662e 6c6f 6c6c         self.loll
+00002fe0: 6d73 5f61 7070 2e63 6f6e 6669 675b 276d  ms_app.config['m
+00002ff0: 6f64 656c 5f6e 616d 6527 5d3d 4e6f 6e65  odel_name']=None
+00003000: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00003010: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
+00003020: 6e66 6967 2e73 6176 655f 636f 6e66 6967  nfig.save_config
+00003030: 2829 0d0a 2020 2020 2020 2020 656c 6966  ()..        elif
+00003040: 2063 686f 6963 6520 3c3d 206c 656e 2862   choice <= len(b
+00003050: 696e 6469 6e67 735f 6c69 7374 293a 0d0a  indings_list):..
+00003060: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003070: 726e 0d0a 2020 2020 2020 2020 656c 7365  rn..        else
+00003080: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
+00003090: 7269 6e74 2822 496e 7661 6c69 6420 6368  rint("Invalid ch
+000030a0: 6f69 6365 2122 290d 0a0d 0a20 2020 2064  oice!")....    d
+000030b0: 6566 2073 656c 6563 745f 6d6f 6465 6c28  ef select_model(
+000030c0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000030d0: 7072 696e 7428 290d 0a20 2020 2020 2020  print()..       
+000030e0: 2070 7269 6e74 2866 227b 4153 4349 4943   print(f"{ASCIIC
+000030f0: 6f6c 6f72 732e 636f 6c6f 725f 6772 6565  olors.color_gree
+00003100: 6e7d 4375 7272 656e 7420 6269 6e64 696e  n}Current bindin
+00003110: 673a 207b 4153 4349 4943 6f6c 6f72 732e  g: {ASCIIColors.
+00003120: 636f 6c6f 725f 7265 7365 747d 7b73 656c  color_reset}{sel
+00003130: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
+00003140: 6669 675b 2762 696e 6469 6e67 5f6e 616d  fig['binding_nam
+00003150: 6527 5d7d 2229 0d0a 2020 2020 2020 2020  e']}")..        
+00003160: 7072 696e 7428 6622 7b41 5343 4949 436f  print(f"{ASCIICo
+00003170: 6c6f 7273 2e63 6f6c 6f72 5f67 7265 656e  lors.color_green
+00003180: 7d43 7572 7265 6e74 206d 6f64 656c 3a20  }Current model: 
+00003190: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
+000031a0: 6f72 5f72 6573 6574 7d7b 7365 6c66 2e6c  or_reset}{self.l
+000031b0: 6f6c 6c6d 735f 6170 702e 636f 6e66 6967  ollms_app.config
+000031c0: 5b27 6d6f 6465 6c5f 6e61 6d65 275d 7d22  ['model_name']}"
+000031d0: 290d 0a0d 0a20 2020 2020 2020 206d 6f64  )....        mod
+000031e0: 656c 735f 6469 723a 5061 7468 203d 2028  els_dir:Path = (
+000031f0: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
+00003200: 6c6f 6c6c 6d73 5f70 6174 6873 2e70 6572  lollms_paths.per
+00003210: 736f 6e61 6c5f 6d6f 6465 6c73 5f70 6174  sonal_models_pat
+00003220: 682f 7365 6c66 2e6c 6f6c 6c6d 735f 6170  h/self.lollms_ap
+00003230: 702e 636f 6e66 6967 5b27 6269 6e64 696e  p.config['bindin
+00003240: 675f 6e61 6d65 275d 290d 0a20 2020 2020  g_name'])..     
+00003250: 2020 206d 6f64 656c 735f 6469 722e 6d6b     models_dir.mk
+00003260: 6469 7228 7061 7265 6e74 733d 5472 7565  dir(parents=True
+00003270: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
+00003280: 0d0a 0d0a 2020 2020 2020 2020 6d6f 6465  ....        mode
+00003290: 6c73 5f6c 6973 7420 3d20 7365 6c66 2e6c  ls_list = self.l
+000032a0: 6f6c 6c6d 735f 6170 702e 6269 6e64 696e  ollms_app.bindin
+000032b0: 672e 6c69 7374 5f6d 6f64 656c 7328 7365  g.list_models(se
+000032c0: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
+000032d0: 6e66 6967 2920 2b20 5b22 496e 7374 616c  nfig) + ["Instal
+000032e0: 6c20 6d6f 6465 6c22 2c20 2243 6861 6e67  l model", "Chang
+000032f0: 6520 6269 6e64 696e 6722 2c20 2242 6163  e binding", "Bac
+00003300: 6b22 5d0d 0a20 2020 2020 2020 2063 686f  k"]..        cho
+00003310: 6963 6520 3d20 7365 6c66 2e73 686f 775f  ice = self.show_
+00003320: 6d65 6e75 286d 6f64 656c 735f 6c69 7374  menu(models_list
+00003330: 290d 0a20 2020 2020 2020 2069 6620 3120  )..        if 1 
+00003340: 3c3d 2063 686f 6963 6520 3c3d 206c 656e  <= choice <= len
+00003350: 286d 6f64 656c 735f 6c69 7374 292d 333a  (models_list)-3:
+00003360: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00003370: 696e 7428 6622 596f 7520 7365 6c65 6374  int(f"You select
+00003380: 6564 206d 6f64 656c 3a20 7b41 5343 4949  ed model: {ASCII
+00003390: 436f 6c6f 7273 2e63 6f6c 6f72 5f67 7265  Colors.color_gre
+000033a0: 656e 7d7b 6d6f 6465 6c73 5f6c 6973 745b  en}{models_list[
+000033b0: 6368 6f69 6365 202d 2031 5d7d 7b41 5343  choice - 1]}{ASC
+000033c0: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f72  IIColors.color_r
+000033d0: 6573 6574 7d22 290d 0a20 2020 2020 2020  eset}")..       
+000033e0: 2020 2020 2073 656c 662e 6c6f 6c6c 6d73       self.lollms
+000033f0: 5f61 7070 2e63 6f6e 6669 675b 276d 6f64  _app.config['mod
+00003400: 656c 5f6e 616d 6527 5d3d 6d6f 6465 6c73  el_name']=models
+00003410: 5f6c 6973 745b 6368 6f69 6365 202d 2031  _list[choice - 1
+00003420: 5d0d 0a20 2020 2020 2020 2020 2020 2073  ]..            s
+00003430: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e63  elf.lollms_app.c
+00003440: 6f6e 6669 672e 7361 7665 5f63 6f6e 6669  onfig.save_confi
+00003450: 6728 290d 0a20 2020 2020 2020 2020 2020  g()..           
+00003460: 2073 656c 662e 6c6f 6c6c 6d73 5f61 7070   self.lollms_app
+00003470: 2e6c 6f61 645f 6d6f 6465 6c28 290d 0a20  .load_model().. 
+00003480: 2020 2020 2020 2065 6c69 6620 6368 6f69         elif choi
+00003490: 6365 203c 3d20 6c65 6e28 6d6f 6465 6c73  ce <= len(models
+000034a0: 5f6c 6973 7429 2d32 3a0d 0a20 2020 2020  _list)-2:..     
+000034b0: 2020 2020 2020 2073 656c 662e 696e 7374         self.inst
+000034c0: 616c 6c5f 6d6f 6465 6c28 290d 0a20 2020  all_model()..   
+000034d0: 2020 2020 2065 6c69 6620 6368 6f69 6365       elif choice
+000034e0: 203c 3d20 6c65 6e28 6d6f 6465 6c73 5f6c   <= len(models_l
+000034f0: 6973 7429 2d31 3a0d 0a20 2020 2020 2020  ist)-1:..       
+00003500: 2020 2020 2073 656c 662e 7365 6c65 6374       self.select
+00003510: 5f62 696e 6469 6e67 2829 0d0a 2020 2020  _binding()..    
+00003520: 2020 2020 2020 2020 7365 6c66 2e73 656c          self.sel
+00003530: 6563 745f 6d6f 6465 6c28 290d 0a20 2020  ect_model()..   
+00003540: 2020 2020 2065 6c69 6620 6368 6f69 6365       elif choice
+00003550: 203c 3d20 6c65 6e28 6d6f 6465 6c73 5f6c   <= len(models_l
+00003560: 6973 7429 3a0d 0a20 2020 2020 2020 2020  ist):..         
+00003570: 2020 2072 6574 7572 6e0d 0a20 2020 2020     return..     
+00003580: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00003590: 2020 2020 2020 7072 696e 7428 2249 6e76        print("Inv
+000035a0: 616c 6964 2063 686f 6963 6521 2229 0d0a  alid choice!")..
+000035b0: 0d0a 2020 2020 6465 6620 696e 7374 616c  ..    def instal
+000035c0: 6c5f 6d6f 6465 6c28 7365 6c66 293a 0d0a  l_model(self):..
+000035d0: 0d0a 2020 2020 2020 2020 6d6f 6465 6c73  ..        models
+000035e0: 5f6c 6973 7420 3d20 5b22 496e 7374 616c  _list = ["Instal
+000035f0: 6c20 6d6f 6465 6c20 6672 6f6d 2069 6e74  l model from int
+00003600: 6572 6e65 7422 2c22 496e 7374 616c 6c20  ernet","Install 
+00003610: 6d6f 6465 6c20 6672 6f6d 206c 6f63 616c  model from local
+00003620: 2066 696c 6522 2c22 4261 636b 225d 0d0a   file","Back"]..
+00003630: 2020 2020 2020 2020 6368 6f69 6365 203d          choice =
+00003640: 2073 656c 662e 7368 6f77 5f6d 656e 7528   self.show_menu(
+00003650: 6d6f 6465 6c73 5f6c 6973 7429 0d0a 2020  models_list)..  
+00003660: 2020 2020 2020 6966 2031 203c 3d20 6368        if 1 <= ch
+00003670: 6f69 6365 203c 3d20 6c65 6e28 6d6f 6465  oice <= len(mode
+00003680: 6c73 5f6c 6973 7429 2d32 3a0d 0a20 2020  ls_list)-2:..   
+00003690: 2020 2020 2020 2020 2075 726c 203d 2069           url = i
+000036a0: 6e70 7574 2822 4769 7665 2061 2055 524c  nput("Give a URL
+000036b0: 2074 6f20 7468 6520 6d6f 6465 6c20 746f   to the model to
+000036c0: 2062 6520 646f 776e 6c6f 6164 6564 203a   be downloaded :
+000036d0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000036e0: 6465 6620 7072 6f67 7265 7373 5f63 616c  def progress_cal
+000036f0: 6c62 6163 6b28 626c 6f63 6b73 2c20 626c  lback(blocks, bl
+00003700: 6f63 6b5f 7369 7a65 2c20 746f 7461 6c5f  ock_size, total_
+00003710: 7369 7a65 293a 0d0a 2020 2020 2020 2020  size):..        
+00003720: 2020 2020 2020 2020 7471 646d 5f62 6172          tqdm_bar
+00003730: 2e74 6f74 616c 3d74 6f74 616c 5f73 697a  .total=total_siz
+00003740: 650d 0a20 2020 2020 2020 2020 2020 2020  e..             
+00003750: 2020 2074 7164 6d5f 6261 722e 7570 6461     tqdm_bar.upda
+00003760: 7465 2862 6c6f 636b 5f73 697a 6529 0d0a  te(block_size)..
+00003770: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00003780: 5573 6167 6520 6578 616d 706c 650d 0a20  Usage example.. 
+00003790: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+000037a0: 7471 646d 2874 6f74 616c 3d31 3030 2c20  tqdm(total=100, 
+000037b0: 756e 6974 3d22 2522 2c20 6465 7363 3d22  unit="%", desc="
+000037c0: 446f 776e 6c6f 6164 2050 726f 6772 6573  Download Progres
+000037d0: 7322 2c20 6e63 6f6c 733d 3830 2920 6173  s", ncols=80) as
+000037e0: 2074 7164 6d5f 6261 723a 0d0a 2020 2020   tqdm_bar:..    
+000037f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003800: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
+00003810: 6967 2e64 6f77 6e6c 6f61 645f 6d6f 6465  ig.download_mode
+00003820: 6c28 7572 6c2c 7365 6c66 2e6c 6f6c 6c6d  l(url,self.lollm
+00003830: 735f 6170 702e 6269 6e64 696e 672c 2070  s_app.binding, p
+00003840: 726f 6772 6573 735f 6361 6c6c 6261 636b  rogress_callback
+00003850: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00003860: 656c 662e 7365 6c65 6374 5f6d 6f64 656c  elf.select_model
+00003870: 2829 0d0a 2020 2020 2020 2020 656c 6966  ()..        elif
+00003880: 2063 686f 6963 6520 3c3d 206c 656e 286d   choice <= len(m
+00003890: 6f64 656c 735f 6c69 7374 292d 313a 0d0a  odels_list)-1:..
+000038a0: 2020 2020 2020 2020 2020 2020 7061 7468              path
+000038b0: 203d 2050 6174 6828 696e 7075 7428 2247   = Path(input("G
+000038c0: 6976 6520 6120 7061 7468 2074 6f20 7468  ive a path to th
+000038d0: 6520 6d6f 6465 6c20 746f 2062 6520 7573  e model to be us
+000038e0: 6564 206f 6e20 796f 7572 2050 433a 2229  ed on your PC:")
+000038f0: 290d 0a20 2020 2020 2020 2020 2020 2069  )..            i
+00003900: 6620 7061 7468 2e65 7869 7374 7328 293a  f path.exists():
+00003910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003920: 2020 7365 6c66 2e6c 6f6c 6c6d 735f 6170    self.lollms_ap
+00003930: 702e 636f 6e66 6967 2e72 6566 6572 656e  p.config.referen
+00003940: 6365 5f6d 6f64 656c 2870 6174 6829 0d0a  ce_model(path)..
+00003950: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003960: 2e73 656c 6563 745f 6d6f 6465 6c28 290d  .select_model().
+00003970: 0a20 2020 2020 2020 2065 6c69 6620 6368  .        elif ch
+00003980: 6f69 6365 203c 3d20 6c65 6e28 6d6f 6465  oice <= len(mode
+00003990: 6c73 5f6c 6973 7429 3a0d 0a20 2020 2020  ls_list):..     
+000039a0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
+000039b0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000039c0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000039d0: 2249 6e76 616c 6964 2063 686f 6963 6521  "Invalid choice!
+000039e0: 2229 0d0a 0d0a 2020 2020 6465 6620 6d6f  ")....    def mo
+000039f0: 756e 745f 7065 7273 6f6e 616c 6974 7928  unt_personality(
+00003a00: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00003a10: 7072 696e 7428 290d 0a20 2020 2020 2020  print()..       
+00003a20: 2041 5343 4949 436f 6c6f 7273 2e72 6564   ASCIIColors.red
+00003a30: 2866 224d 6f75 6e74 6564 2070 6572 736f  (f"Mounted perso
+00003a40: 6e61 6c69 7469 6573 3a22 290d 0a20 2020  nalities:")..   
+00003a50: 2020 2020 2066 6f72 2069 2c70 6572 736f       for i,perso
+00003a60: 6e61 6c69 7479 2069 6e20 656e 756d 6572  nality in enumer
+00003a70: 6174 6528 7365 6c66 2e6c 6f6c 6c6d 735f  ate(self.lollms_
+00003a80: 6170 702e 636f 6e66 6967 5b27 7065 7273  app.config['pers
+00003a90: 6f6e 616c 6974 6965 7327 5d29 3a0d 0a20  onalities']):.. 
+00003aa0: 2020 2020 2020 2020 2020 2069 6620 693d             if i=
+00003ab0: 3d73 656c 662e 6c6f 6c6c 6d73 5f61 7070  =self.lollms_app
+00003ac0: 2e63 6f6e 6669 675b 2761 6374 6976 655f  .config['active_
+00003ad0: 7065 7273 6f6e 616c 6974 795f 6964 275d  personality_id']
+00003ae0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00003af0: 2020 2041 5343 4949 436f 6c6f 7273 2e67     ASCIIColors.g
+00003b00: 7265 656e 2870 6572 736f 6e61 6c69 7479  reen(personality
+00003b10: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00003b20: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00003b30: 2020 2020 2020 4153 4349 4943 6f6c 6f72        ASCIIColor
+00003b40: 732e 7965 6c6c 6f77 2870 6572 736f 6e61  s.yellow(persona
+00003b50: 6c69 7479 290d 0a20 2020 2020 2020 2070  lity)..        p
+00003b60: 6572 736f 6e61 6c69 7479 5f6c 616e 6775  ersonality_langu
+00003b70: 6167 6573 203d 205b 702e 7374 656d 2066  ages = [p.stem f
+00003b80: 6f72 2070 2069 6e20 7365 6c66 2e6c 6f6c  or p in self.lol
+00003b90: 6c6d 735f 6170 702e 6c6f 6c6c 6d73 5f70  lms_app.lollms_p
+00003ba0: 6174 6873 2e70 6572 736f 6e61 6c69 7469  aths.personaliti
+00003bb0: 6573 5f7a 6f6f 5f70 6174 682e 6974 6572  es_zoo_path.iter
+00003bc0: 6469 7228 2920 6966 2070 2e69 735f 6469  dir() if p.is_di
+00003bd0: 7228 2920 616e 6420 6e6f 7420 702e 6e61  r() and not p.na
+00003be0: 6d65 2e73 7461 7274 7377 6974 6828 222e  me.startswith(".
+00003bf0: 2229 5d20 2b20 5b22 4261 636b 225d 0d0a  ")] + ["Back"]..
+00003c00: 2020 2020 2020 2020 7072 696e 7428 2253          print("S
+00003c10: 656c 6563 7420 6c61 6e67 7561 6765 2229  elect language")
+00003c20: 0d0a 2020 2020 2020 2020 6368 6f69 6365  ..        choice
+00003c30: 203d 2073 656c 662e 7368 6f77 5f6d 656e   = self.show_men
+00003c40: 7528 7065 7273 6f6e 616c 6974 795f 6c61  u(personality_la
+00003c50: 6e67 7561 6765 7329 0d0a 2020 2020 2020  nguages)..      
+00003c60: 2020 6966 2031 203c 3d20 6368 6f69 6365    if 1 <= choice
+00003c70: 203c 3d20 6c65 6e28 7065 7273 6f6e 616c   <= len(personal
+00003c80: 6974 795f 6c61 6e67 7561 6765 7329 2d31  ity_languages)-1
+00003c90: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
+00003ca0: 616e 6775 6167 6520 3d20 7065 7273 6f6e  anguage = person
+00003cb0: 616c 6974 795f 6c61 6e67 7561 6765 735b  ality_languages[
+00003cc0: 6368 6f69 6365 202d 2031 5d0d 0a20 2020  choice - 1]..   
+00003cd0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00003ce0: 2259 6f75 2073 656c 6563 7465 6420 6c61  "You selected la
+00003cf0: 6e67 7561 6765 3a20 7b41 5343 4949 436f  nguage: {ASCIICo
+00003d00: 6c6f 7273 2e63 6f6c 6f72 5f67 7265 656e  lors.color_green
+00003d10: 7d7b 6c61 6e67 7561 6765 7d7b 4153 4349  }{language}{ASCI
+00003d20: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
+00003d30: 7365 747d 2229 0d0a 2020 2020 2020 2020  set}")..        
+00003d40: 2020 2020 7065 7273 6f6e 616c 6974 795f      personality_
+00003d50: 6361 7465 676f 7269 6573 203d 205b 702e  categories = [p.
+00003d60: 7374 656d 2066 6f72 2070 2069 6e20 2873  stem for p in (s
+00003d70: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e6c  elf.lollms_app.l
+00003d80: 6f6c 6c6d 735f 7061 7468 732e 7065 7273  ollms_paths.pers
+00003d90: 6f6e 616c 6974 6965 735f 7a6f 6f5f 7061  onalities_zoo_pa
+00003da0: 7468 2f6c 616e 6775 6167 6529 2e69 7465  th/language).ite
+00003db0: 7264 6972 2829 2069 6620 702e 6973 5f64  rdir() if p.is_d
+00003dc0: 6972 2829 2061 6e64 206e 6f74 2070 2e6e  ir() and not p.n
+00003dd0: 616d 652e 7374 6172 7473 7769 7468 2822  ame.startswith("
+00003de0: 2e22 295d 2b5b 2242 6163 6b22 5d0d 0a20  .")]+["Back"].. 
+00003df0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00003e00: 2822 5365 6c65 6374 2063 6174 6567 6f72  ("Select categor
+00003e10: 7922 290d 0a20 2020 2020 2020 2020 2020  y")..           
+00003e20: 2063 686f 6963 6520 3d20 7365 6c66 2e73   choice = self.s
+00003e30: 686f 775f 6d65 6e75 2870 6572 736f 6e61  how_menu(persona
+00003e40: 6c69 7479 5f63 6174 6567 6f72 6965 7329  lity_categories)
+00003e50: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00003e60: 2031 203c 3d20 6368 6f69 6365 203c 3d20   1 <= choice <= 
+00003e70: 6c65 6e28 7065 7273 6f6e 616c 6974 795f  len(personality_
+00003e80: 6361 7465 676f 7269 6573 292d 313a 0d0a  categories)-1:..
+00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ea0: 6361 7465 676f 7279 203d 2070 6572 736f  category = perso
+00003eb0: 6e61 6c69 7479 5f63 6174 6567 6f72 6965  nality_categorie
+00003ec0: 735b 6368 6f69 6365 202d 2031 5d0d 0a20  s[choice - 1].. 
+00003ed0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003ee0: 7269 6e74 2866 2259 6f75 2073 656c 6563  rint(f"You selec
+00003ef0: 7465 6420 6361 7465 676f 7279 3a20 7b41  ted category: {A
+00003f00: 5343 4949 436f 6c6f 7273 2e63 6f6c 6f72  SCIIColors.color
+00003f10: 5f67 7265 656e 7d7b 6361 7465 676f 7279  _green}{category
+00003f20: 7d7b 4153 4349 4943 6f6c 6f72 732e 636f  }{ASCIIColors.co
+00003f30: 6c6f 725f 7265 7365 747d 2229 0d0a 2020  lor_reset}")..  
+00003f40: 2020 2020 2020 2020 2020 2020 2020 7065                pe
+00003f50: 7273 6f6e 616c 6974 795f 6e61 6d65 7320  rsonality_names 
+00003f60: 3d20 5b70 2e73 7465 6d20 666f 7220 7020  = [p.stem for p 
+00003f70: 696e 2028 7365 6c66 2e6c 6f6c 6c6d 735f  in (self.lollms_
+00003f80: 6170 702e 6c6f 6c6c 6d73 5f70 6174 6873  app.lollms_paths
+00003f90: 2e70 6572 736f 6e61 6c69 7469 6573 5f7a  .personalities_z
+00003fa0: 6f6f 5f70 6174 682f 6c61 6e67 7561 6765  oo_path/language
+00003fb0: 2f63 6174 6567 6f72 7929 2e69 7465 7264  /category).iterd
+00003fc0: 6972 2829 2069 6620 702e 6973 5f64 6972  ir() if p.is_dir
+00003fd0: 2829 2061 6e64 206e 6f74 2070 2e6e 616d  () and not p.nam
+00003fe0: 652e 7374 6172 7473 7769 7468 2822 2e22  e.startswith("."
+00003ff0: 295d 2b5b 2242 6163 6b22 5d0d 0a20 2020  )]+["Back"]..   
+00004000: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00004010: 6e74 2822 5365 6c65 6374 2070 6572 736f  nt("Select perso
+00004020: 6e61 6c69 7479 2229 0d0a 2020 2020 2020  nality")..      
+00004030: 2020 2020 2020 2020 2020 6368 6f69 6365            choice
+00004040: 203d 2073 656c 662e 7368 6f77 5f6d 656e   = self.show_men
+00004050: 7528 7065 7273 6f6e 616c 6974 795f 6e61  u(personality_na
+00004060: 6d65 7329 0d0a 2020 2020 2020 2020 2020  mes)..          
+00004070: 2020 2020 2020 6966 2031 203c 3d20 6368        if 1 <= ch
+00004080: 6f69 6365 203c 3d20 6c65 6e28 7065 7273  oice <= len(pers
+00004090: 6f6e 616c 6974 795f 6e61 6d65 7329 2d31  onality_names)-1
+000040a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+000040b0: 2020 2020 2020 206e 616d 6520 3d20 7065         name = pe
+000040c0: 7273 6f6e 616c 6974 795f 6e61 6d65 735b  rsonality_names[
+000040d0: 6368 6f69 6365 202d 2031 5d0d 0a20 2020  choice - 1]..   
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2070 7269 6e74 2866 2259 6f75 2073 656c   print(f"You sel
+00004100: 6563 7465 6420 7065 7273 6f6e 616c 6974  ected personalit
+00004110: 793a 207b 4153 4349 4943 6f6c 6f72 732e  y: {ASCIIColors.
+00004120: 636f 6c6f 725f 6772 6565 6e7d 7b6e 616d  color_green}{nam
+00004130: 657d 7b41 5343 4949 436f 6c6f 7273 2e63  e}{ASCIIColors.c
+00004140: 6f6c 6f72 5f72 6573 6574 7d22 290d 0a20  olor_reset}").. 
+00004150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004160: 2020 2073 656c 662e 6c6f 6c6c 6d73 5f61     self.lollms_a
+00004170: 7070 2e63 6f6e 6669 675b 2270 6572 736f  pp.config["perso
+00004180: 6e61 6c69 7469 6573 225d 2e61 7070 656e  nalities"].appen
+00004190: 6428 6622 7b6c 616e 6775 6167 657d 2f7b  d(f"{language}/{
+000041a0: 6361 7465 676f 7279 7d2f 7b6e 616d 657d  category}/{name}
+000041b0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+000041c0: 2020 2020 2020 2020 7365 6c66 2e6c 6f6c          self.lol
+000041d0: 6c6d 735f 6170 702e 6d6f 756e 745f 7065  lms_app.mount_pe
+000041e0: 7273 6f6e 616c 6974 7928 6c65 6e28 7365  rsonality(len(se
+000041f0: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
+00004200: 6e66 6967 5b22 7065 7273 6f6e 616c 6974  nfig["personalit
+00004210: 6965 7322 5d29 2d31 2c20 6361 6c6c 6261  ies"])-1, callba
+00004220: 636b 203d 2073 656c 662e 6361 6c6c 6261  ck = self.callba
+00004230: 636b 290d 0a20 2020 2020 2020 2020 2020  ck)..           
+00004240: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00004250: 6c6c 6d73 5f61 7070 2e63 6f6e 6669 672e  llms_app.config.
+00004260: 7361 7665 5f63 6f6e 6669 6728 290d 0a20  save_config().. 
+00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004280: 2020 2070 7269 6e74 2822 5065 7273 6f6e     print("Person
+00004290: 616c 6974 7920 6d6f 756e 7465 6420 7375  ality mounted su
+000042a0: 6363 6573 7366 756c 6c79 2122 290d 0a20  ccessfully!").. 
+000042b0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000042c0: 6c69 6620 3120 3c3d 2063 686f 6963 6520  lif 1 <= choice 
+000042d0: 3c3d 206c 656e 2870 6572 736f 6e61 6c69  <= len(personali
+000042e0: 7479 5f6e 616d 6573 293a 0d0a 2020 2020  ty_names):..    
+000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004300: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
+00004310: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004330: 2020 2070 7269 6e74 2822 496e 7661 6c69     print("Invali
+00004340: 6420 6368 6f69 6365 2122 290d 0a20 2020  d choice!")..   
+00004350: 2020 2020 2020 2020 2065 6c69 6620 3120           elif 1 
+00004360: 3c3d 2063 686f 6963 6520 3c3d 206c 656e  <= choice <= len
+00004370: 2870 6572 736f 6e61 6c69 7479 5f63 6174  (personality_cat
+00004380: 6567 6f72 6965 7329 3a0d 0a20 2020 2020  egories):..     
+00004390: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000043a0: 6e0d 0a20 2020 2020 2020 2020 2020 2065  n..            e
+000043b0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+000043c0: 2020 2020 2020 7072 696e 7428 2249 6e76        print("Inv
+000043d0: 616c 6964 2063 686f 6963 6521 2229 0d0a  alid choice!")..
+000043e0: 2020 2020 2020 2020 656c 6966 2031 203c          elif 1 <
+000043f0: 3d20 6368 6f69 6365 203c 3d20 6c65 6e28  = choice <= len(
+00004400: 7065 7273 6f6e 616c 6974 795f 6c61 6e67  personality_lang
+00004410: 7561 6765 7329 3a0d 0a20 2020 2020 2020  uages):..       
+00004420: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00004430: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00004440: 2020 2020 2020 2020 7072 696e 7428 2249          print("I
+00004450: 6e76 616c 6964 2063 686f 6963 6521 2229  nvalid choice!")
+00004460: 0d0a 0d0a 2020 2020 6465 6620 7665 775f  ....    def vew_
+00004470: 6d6f 756e 7465 645f 7065 7273 6f6e 616c  mounted_personal
+00004480: 6974 6965 7328 7365 6c66 293a 0d0a 2020  ities(self):..  
+00004490: 2020 2020 2020 4153 4349 4943 6f6c 6f72        ASCIIColor
+000044a0: 732e 696e 666f 2822 4865 7265 2069 7320  s.info("Here is 
+000044b0: 7468 6520 6c69 7374 206f 6620 6d6f 756e  the list of moun
+000044c0: 7465 6420 7065 7273 6f6e 616c 6974 6965  ted personalitie
+000044d0: 7322 290d 0a20 2020 2020 2020 2065 6e74  s")..        ent
+000044e0: 7269 6573 203d 2073 656c 662e 6c6f 6c6c  ries = self.loll
+000044f0: 6d73 5f61 7070 2e63 6f6e 6669 675b 2770  ms_app.config['p
+00004500: 6572 736f 6e61 6c69 7469 6573 275d 0d0a  ersonalities']..
+00004510: 2020 2020 2020 2020 666f 7220 6964 2c20          for id, 
+00004520: 656e 7472 7920 696e 2065 6e75 6d65 7261  entry in enumera
+00004530: 7465 2865 6e74 7269 6573 293a 0d0a 2020  te(entries):..  
+00004540: 2020 2020 2020 2020 2020 6966 2069 6420            if id 
+00004550: 213d 2073 656c 662e 6c6f 6c6c 6d73 5f61  != self.lollms_a
+00004560: 7070 2e63 6f6e 6669 672e 6163 7469 7665  pp.config.active
+00004570: 5f70 6572 736f 6e61 6c69 7479 5f69 643a  _personality_id:
+00004580: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004590: 2020 4153 4349 4943 6f6c 6f72 732e 7965    ASCIIColors.ye
+000045a0: 6c6c 6f77 2866 227b 6964 2b31 7d20 2d20  llow(f"{id+1} - 
 000045b0: 7b65 6e74 7279 7d22 290d 0a20 2020 2020  {entry}")..     
-000045c0: 2020 2073 656c 662e 7368 6f77 5f6d 656e     self.show_men
-000045d0: 7528 5b22 4261 636b 225d 290d 0a0d 0a0d  u(["Back"]).....
-000045e0: 0a20 2020 2064 6566 2075 6e6d 6f75 6e74  .    def unmount
-000045f0: 5f70 6572 736f 6e61 6c69 7479 2873 656c  _personality(sel
-00004600: 6629 3a0d 0a20 2020 2020 2020 2041 5343  f):..        ASC
-00004610: 4949 436f 6c6f 7273 2e69 6e66 6f28 2253  IIColors.info("S
-00004620: 656c 6563 7420 7065 7273 6f6e 616c 6974  elect personalit
-00004630: 7920 746f 2075 6e6d 6f75 6e74 2229 0d0a  y to unmount")..
-00004640: 2020 2020 2020 2020 656e 7472 6965 7320          entries 
-00004650: 3d20 7365 6c66 2e6c 6f6c 6c6d 735f 6170  = self.lollms_ap
-00004660: 702e 636f 6e66 6967 5b27 7065 7273 6f6e  p.config['person
-00004670: 616c 6974 6965 7327 5d2b 5b22 4261 636b  alities']+["Back
-00004680: 225d 0d0a 2020 2020 2020 2020 7472 793a  "]..        try:
-00004690: 0d0a 2020 2020 2020 2020 2020 2020 6368  ..            ch
-000046a0: 6f69 6365 203d 2069 6e74 2873 656c 662e  oice = int(self.
-000046b0: 7368 6f77 5f6d 656e 7528 656e 7472 6965  show_menu(entrie
-000046c0: 732c 2073 656c 662e 6c6f 6c6c 6d73 5f61  s, self.lollms_a
-000046d0: 7070 2e63 6f6e 6669 675b 2761 6374 6976  pp.config['activ
-000046e0: 655f 7065 7273 6f6e 616c 6974 795f 6964  e_personality_id
-000046f0: 275d 2929 2d31 0d0a 2020 2020 2020 2020  ']))-1..        
-00004700: 2020 2020 6966 2063 686f 6963 653c 6c65      if choice<le
-00004710: 6e28 656e 7472 6965 7329 2d31 3a0d 0a20  n(entries)-1:.. 
-00004720: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00004730: 656c 662e 6c6f 6c6c 6d73 5f61 7070 2e75  elf.lollms_app.u
-00004740: 6e6d 6f75 6e74 5f70 6572 736f 6e61 6c69  nmount_personali
-00004750: 7479 2863 686f 6963 6529 0d0a 2020 2020  ty(choice)..    
-00004760: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00004770: 7469 6f6e 2061 7320 6578 3a0d 0a20 2020  tion as ex:..   
-00004780: 2020 2020 2020 2020 2041 5343 4949 436f           ASCIICo
-00004790: 6c6f 7273 2e65 7272 6f72 2866 2243 6f75  lors.error(f"Cou
-000047a0: 6c64 6e27 7420 7568 6e6d 6f75 6e74 2070  ldn't uhnmount p
-000047b0: 6572 736f 6e61 6c69 7479 2e5c 6e47 6f74  ersonality.\nGot
-000047c0: 2074 6869 7320 6578 6365 7074 696f 6e3a   this exception:
-000047d0: 7b65 787d 2229 0d0a 0d0a 2020 2020 6465  {ex}")....    de
-000047e0: 6620 7365 6c65 6374 5f70 6572 736f 6e61  f select_persona
-000047f0: 6c69 7479 2873 656c 6629 3a0d 0a20 2020  lity(self):..   
-00004800: 2020 2020 2041 5343 4949 436f 6c6f 7273       ASCIIColors
-00004810: 2e69 6e66 6f28 2253 656c 6563 7420 7065  .info("Select pe
-00004820: 7273 6f6e 616c 6974 7920 746f 2061 6374  rsonality to act
-00004830: 6976 6174 6522 290d 0a20 2020 2020 2020  ivate")..       
-00004840: 2065 6e74 7269 6573 203d 2073 656c 662e   entries = self.
-00004850: 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e 6669  lollms_app.confi
-00004860: 675b 2770 6572 736f 6e61 6c69 7469 6573  g['personalities
-00004870: 275d 2b5b 2242 6163 6b22 5d0d 0a20 2020  ']+["Back"]..   
-00004880: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00004890: 2020 2020 2020 2063 686f 6963 6520 3d20         choice = 
-000048a0: 696e 7428 7365 6c66 2e73 686f 775f 6d65  int(self.show_me
-000048b0: 6e75 2865 6e74 7269 6573 2c20 7365 6c66  nu(entries, self
-000048c0: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
-000048d0: 6967 5b27 6163 7469 7665 5f70 6572 736f  ig['active_perso
-000048e0: 6e61 6c69 7479 5f69 6427 5d29 292d 310d  nality_id']))-1.
-000048f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004900: 6368 6f69 6365 3c6c 656e 2865 6e74 7269  choice<len(entri
-00004910: 6573 292d 313a 0d0a 2020 2020 2020 2020  es)-1:..        
-00004920: 2020 2020 2020 2020 7365 6c66 2e6c 6f6c          self.lol
-00004930: 6c6d 735f 6170 702e 7365 6c65 6374 5f70  lms_app.select_p
-00004940: 6572 736f 6e61 6c69 7479 2863 686f 6963  ersonality(choic
-00004950: 6529 0d0a 2020 2020 2020 2020 6578 6365  e)..        exce
-00004960: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00004970: 6578 3a0d 0a20 2020 2020 2020 2020 2020  ex:..           
-00004980: 2041 5343 4949 436f 6c6f 7273 2e65 7272   ASCIIColors.err
-00004990: 6f72 2866 2243 6f75 6c64 6e27 7420 7365  or(f"Couldn't se
-000049a0: 7420 7065 7273 6f6e 616c 6974 792e 5c6e  t personality.\n
-000049b0: 476f 7420 7468 6973 2065 7863 6570 7469  Got this excepti
-000049c0: 6f6e 3a7b 6578 7d22 290d 0a0d 0a20 2020  on:{ex}")....   
-000049d0: 2064 6566 2072 6569 6e73 7461 6c6c 5f62   def reinstall_b
-000049e0: 696e 6469 6e67 2873 656c 6629 3a0d 0a20  inding(self):.. 
-000049f0: 2020 2020 2020 206c 6f6c 6c6d 735f 6170         lollms_ap
-00004a00: 7020 3d20 7365 6c66 2e6c 6f6c 6c6d 735f  p = self.lollms_
-00004a10: 6170 700d 0a20 2020 2020 2020 2062 696e  app..        bin
-00004a20: 6469 6e67 735f 6c69 7374 203d 205b 5d0d  dings_list = [].
-00004a30: 0a20 2020 2020 2020 2070 7269 6e74 2829  .        print()
-00004a40: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00004a50: 6622 7b41 5343 4949 436f 6c6f 7273 2e63  f"{ASCIIColors.c
-00004a60: 6f6c 6f72 5f67 7265 656e 7d43 7572 7265  olor_green}Curre
-00004a70: 6e74 2062 696e 6469 6e67 3a20 7b41 5343  nt binding: {ASC
-00004a80: 4949 436f 6c6f 7273 2e63 6f6c 6f72 5f72  IIColors.color_r
-00004a90: 6573 6574 7d7b 7365 6c66 2e6c 6f6c 6c6d  eset}{self.lollm
-00004aa0: 735f 6170 702e 636f 6e66 6967 5b27 6269  s_app.config['bi
-00004ab0: 6e64 696e 675f 6e61 6d65 275d 7d22 290d  nding_name']}").
-00004ac0: 0a20 2020 2020 2020 2066 6f72 2070 2069  .        for p i
-00004ad0: 6e20 7365 6c66 2e6c 6f6c 6c6d 735f 6170  n self.lollms_ap
-00004ae0: 702e 6c6f 6c6c 6d73 5f70 6174 6873 2e62  p.lollms_paths.b
-00004af0: 696e 6469 6e67 735f 7a6f 6f5f 7061 7468  indings_zoo_path
-00004b00: 2e69 7465 7264 6972 2829 3a0d 0a20 2020  .iterdir():..   
-00004b10: 2020 2020 2020 2020 2069 6620 702e 6973           if p.is
-00004b20: 5f64 6972 2829 2061 6e64 206e 6f74 2070  _dir() and not p
-00004b30: 2e73 7465 6d2e 7374 6172 7473 7769 7468  .stem.startswith
-00004b40: 2822 2e22 293a 0d0a 2020 2020 2020 2020  ("."):..        
-00004b50: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00004b60: 6e28 702f 2262 696e 6469 6e67 5f63 6172  n(p/"binding_car
-00004b70: 642e 7961 6d6c 222c 2022 7222 2920 6173  d.yaml", "r") as
-00004b80: 2066 3a0d 0a20 2020 2020 2020 2020 2020   f:..           
-00004b90: 2020 2020 2020 2020 2063 6172 6420 3d20           card = 
-00004ba0: 7961 6d6c 2e73 6166 655f 6c6f 6164 2866  yaml.safe_load(f
-00004bb0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004bc0: 2020 2077 6974 6820 6f70 656e 2870 2f22     with open(p/"
-00004bd0: 6d6f 6465 6c73 2e79 616d 6c22 2c20 2272  models.yaml", "r
-00004be0: 2229 2061 7320 663a 0d0a 2020 2020 2020  ") as f:..      
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
-00004c00: 6465 6c73 203d 2079 616d 6c2e 7361 6665  dels = yaml.safe
-00004c10: 5f6c 6f61 6428 6629 0d0a 2020 2020 2020  _load(f)..      
-00004c20: 2020 2020 2020 2020 2020 6973 5f69 6e73            is_ins
-00004c30: 7461 6c6c 6564 203d 2028 7365 6c66 2e6c  talled = (self.l
-00004c40: 6f6c 6c6d 735f 6170 702e 6c6f 6c6c 6d73  ollms_app.lollms
-00004c50: 5f70 6174 6873 2e70 6572 736f 6e61 6c5f  _paths.personal_
-00004c60: 636f 6e66 6967 7572 6174 696f 6e5f 7061  configuration_pa
-00004c70: 7468 2f66 2262 696e 6469 6e67 5f7b 702e  th/f"binding_{p.
-00004c80: 6e61 6d65 7d2e 7961 6d6c 2229 2e65 7869  name}.yaml").exi
-00004c90: 7374 7328 290d 0a20 2020 2020 2020 2020  sts()..         
-00004ca0: 2020 2020 2020 2065 6e74 7279 3d66 227b         entry=f"{
-00004cb0: 4153 4349 4943 6f6c 6f72 732e 636f 6c6f  ASCIIColors.colo
-00004cc0: 725f 6772 6565 6e20 6966 2069 735f 696e  r_green if is_in
-00004cd0: 7374 616c 6c65 6420 656c 7365 2027 277d  stalled else ''}
-00004ce0: 7b27 2a27 2069 6620 7365 6c66 2e6c 6f6c  {'*' if self.lol
-00004cf0: 6c6d 735f 6170 702e 636f 6e66 6967 5b27  lms_app.config['
-00004d00: 6269 6e64 696e 675f 6e61 6d65 275d 3d3d  binding_name']==
-00004d10: 6361 7264 5b27 6e61 6d65 275d 2065 6c73  card['name'] els
-00004d20: 6520 2727 7d20 7b63 6172 645b 276e 616d  e ''} {card['nam
-00004d30: 6527 5d7d 2028 6279 207b 6361 7264 5b27  e']} (by {card['
-00004d40: 6175 7468 6f72 275d 7d29 220d 0a20 2020  author']})"..   
-00004d50: 2020 2020 2020 2020 2020 2020 2062 696e               bin
-00004d60: 6469 6e67 735f 6c69 7374 2e61 7070 656e  dings_list.appen
-00004d70: 6428 656e 7472 7929 0d0a 2020 2020 2020  d(entry)..      
-00004d80: 2020 2020 2020 2020 2020 656e 7472 793d            entry=
-00004d90: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00004da0: 2020 2020 2020 2022 6e61 6d65 223a 702e         "name":p.
-00004db0: 6e61 6d65 2c0d 0a20 2020 2020 2020 2020  name,..         
-00004dc0: 2020 2020 2020 2020 2020 2022 6361 7264             "card
-00004dd0: 223a 6361 7264 2c0d 0a20 2020 2020 2020  ":card,..       
-00004de0: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-00004df0: 6465 6c73 223a 6d6f 6465 6c73 2c0d 0a20  dels":models,.. 
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2022 696e 7374 616c 6c65 6422 3a20     "installed": 
-00004e20: 6973 5f69 6e73 7461 6c6c 6564 0d0a 2020  is_installed..  
-00004e30: 2020 2020 2020 2020 2020 2020 2020 7d0d                }.
-00004e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e50: 2073 656c 662e 6269 6e64 696e 675f 696e   self.binding_in
-00004e60: 6673 2e61 7070 656e 6428 656e 7472 7929  fs.append(entry)
-00004e70: 0d0a 2020 2020 2020 2020 6269 6e64 696e  ..        bindin
-00004e80: 6773 5f6c 6973 7420 2b3d 205b 2242 6163  gs_list += ["Bac
-00004e90: 6b22 5d0d 0a20 2020 2020 2020 2063 686f  k"]..        cho
-00004ea0: 6963 6520 3d20 7365 6c66 2e73 686f 775f  ice = self.show_
-00004eb0: 6d65 6e75 2862 696e 6469 6e67 735f 6c69  menu(bindings_li
-00004ec0: 7374 290d 0a20 2020 2020 2020 2069 6620  st)..        if 
-00004ed0: 3120 3c3d 2063 686f 6963 6520 3c3d 206c  1 <= choice <= l
-00004ee0: 656e 2862 696e 6469 6e67 735f 6c69 7374  en(bindings_list
-00004ef0: 292d 313a 0d0a 2020 2020 2020 2020 2020  )-1:..          
-00004f00: 2020 7072 696e 7428 6622 596f 7520 7365    print(f"You se
-00004f10: 6c65 6374 6564 2062 696e 6469 6e67 3a20  lected binding: 
-00004f20: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
-00004f30: 6f72 5f67 7265 656e 7d7b 7365 6c66 2e62  or_green}{self.b
-00004f40: 696e 6469 6e67 5f69 6e66 735b 6368 6f69  inding_infs[choi
-00004f50: 6365 202d 2031 5d5b 276e 616d 6527 5d7d  ce - 1]['name']}
-00004f60: 7b41 5343 4949 436f 6c6f 7273 2e63 6f6c  {ASCIIColors.col
-00004f70: 6f72 5f72 6573 6574 7d22 290d 0a20 2020  or_reset}")..   
-00004f80: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00004f90: 6c6c 6d73 5f61 7070 2e63 6f6e 6669 675b  llms_app.config[
-00004fa0: 2762 696e 6469 6e67 5f6e 616d 6527 5d3d  'binding_name']=
-00004fb0: 7365 6c66 2e62 696e 6469 6e67 5f69 6e66  self.binding_inf
-00004fc0: 735b 6368 6f69 6365 202d 2031 5d5b 276e  s[choice - 1]['n
-00004fd0: 616d 6527 5d0d 0a0d 0a20 2020 2020 2020  ame']....       
-00004fe0: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00004ff0: 2020 2020 2020 2020 2020 206c 6f6c 6c6d             lollm
-00005000: 735f 6170 702e 6269 6e64 696e 6720 3d20  s_app.binding = 
-00005010: 4269 6e64 696e 6742 7569 6c64 6572 2829  BindingBuilder()
-00005020: 2e62 7569 6c64 5f62 696e 6469 6e67 286c  .build_binding(l
-00005030: 6f6c 6c6d 735f 6170 702e 636f 6e66 6967  ollms_app.config
-00005040: 2c20 6c6f 6c6c 6d73 5f61 7070 2e6c 6f6c  , lollms_app.lol
-00005050: 6c6d 735f 7061 7468 732c 496e 7374 616c  lms_paths,Instal
-00005060: 6c4f 7074 696f 6e2e 464f 5243 455f 494e  lOption.FORCE_IN
-00005070: 5354 414c 4c29 0d0a 2020 2020 2020 2020  STALL)..        
-00005080: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00005090: 7469 6f6e 2061 7320 6578 3a0d 0a20 2020  tion as ex:..   
-000050a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000050b0: 6e74 2865 7829 0d0a 2020 2020 2020 2020  nt(ex)..        
-000050c0: 2020 2020 2020 2020 7072 696e 7428 6622          print(f"
-000050d0: 436f 756c 646e 2774 2066 696e 6420 6269  Couldn't find bi
-000050e0: 6e64 696e 672e 2050 6c65 6173 6520 7665  nding. Please ve
-000050f0: 7269 6679 2079 6f75 7220 636f 6e66 6967  rify your config
-00005100: 7572 6174 696f 6e20 6669 6c65 2061 7420  uration file at 
-00005110: 7b6c 6f6c 6c6d 735f 6170 702e 636f 6e66  {lollms_app.conf
-00005120: 6967 2e66 696c 655f 7061 7468 7d20 6f72  ig.file_path} or
-00005130: 2075 7365 2074 6865 206e 6578 7420 6d65   use the next me
-00005140: 6e75 2074 6f20 7365 6c65 6374 2061 2076  nu to select a v
-00005150: 616c 6964 2062 696e 6469 6e67 2229 0d0a  alid binding")..
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 7365 6c66 2e73 656c 6563 745f 6269 6e64  self.select_bind
-00005180: 696e 6728 290d 0a0d 0a20 2020 2020 2020  ing()....       
-00005190: 2020 2020 2073 656c 662e 6c6f 6c6c 6d73       self.lollms
-000051a0: 5f61 7070 2e63 6f6e 6669 675b 276d 6f64  _app.config['mod
-000051b0: 656c 5f6e 616d 6527 5d3d 4e6f 6e65 0d0a  el_name']=None..
-000051c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000051d0: 2e6c 6f6c 6c6d 735f 6170 702e 636f 6e66  .lollms_app.conf
-000051e0: 6967 2e73 6176 655f 636f 6e66 6967 2829  ig.save_config()
-000051f0: 0d0a 2020 2020 2020 2020 656c 6966 2063  ..        elif c
-00005200: 686f 6963 6520 3c3d 206c 656e 2862 696e  hoice <= len(bin
-00005210: 6469 6e67 735f 6c69 7374 293a 0d0a 2020  dings_list):..  
-00005220: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00005230: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00005240: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00005250: 6e74 2822 496e 7661 6c69 6420 6368 6f69  nt("Invalid choi
-00005260: 6365 2122 2920 2020 2020 2020 200d 0a0d  ce!")        ...
-00005270: 0a0d 0a20 2020 200d 0a20 2020 2064 6566  ...    ..    def
-00005280: 2072 6569 6e73 7461 6c6c 5f70 6572 736f   reinstall_perso
-00005290: 6e61 6c69 7479 2873 656c 6629 3a0d 0a20  nality(self):.. 
-000052a0: 2020 2020 2020 206c 6f6c 6c6d 735f 6170         lollms_ap
-000052b0: 7020 3d20 7365 6c66 2e6c 6f6c 6c6d 735f  p = self.lollms_
-000052c0: 6170 700d 0a20 2020 2020 2020 2074 7279  app..        try
-000052d0: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-000052e0: 6f6c 6c6d 735f 6170 702e 7065 7273 6f6e  ollms_app.person
-000052f0: 616c 6974 7920 3d20 5065 7273 6f6e 616c  ality = Personal
-00005300: 6974 7942 7569 6c64 6572 286c 6f6c 6c6d  ityBuilder(lollm
-00005310: 735f 6170 702e 6c6f 6c6c 6d73 5f70 6174  s_app.lollms_pat
-00005320: 6873 2c20 6c6f 6c6c 6d73 5f61 7070 2e63  hs, lollms_app.c
-00005330: 6f6e 6669 672c 206c 6f6c 6c6d 735f 6170  onfig, lollms_ap
-00005340: 702e 6d6f 6465 6c2c 2069 6e73 7461 6c6c  p.model, install
-00005350: 6174 696f 6e5f 6f70 7469 6f6e 3d49 6e73  ation_option=Ins
-00005360: 7461 6c6c 4f70 7469 6f6e 2e46 4f52 4345  tallOption.FORCE
-00005370: 5f49 4e53 5441 4c4c 292e 6275 696c 645f  _INSTALL).build_
-00005380: 7065 7273 6f6e 616c 6974 7928 290d 0a20  personality().. 
-00005390: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000053a0: 6365 7074 696f 6e20 6173 2065 783a 0d0a  ception as ex:..
-000053b0: 2020 2020 2020 2020 2020 2020 4153 4349              ASCI
-000053c0: 4943 6f6c 6f72 732e 6572 726f 7228 6622  IColors.error(f"
-000053d0: 436f 756c 646e 2774 206c 6f61 6420 7065  Couldn't load pe
-000053e0: 7273 6f6e 616c 6974 792e 2050 6c65 6173  rsonality. Pleas
-000053f0: 6520 7665 7269 6679 2079 6f75 7220 636f  e verify your co
-00005400: 6e66 6967 7572 6174 696f 6e20 6669 6c65  nfiguration file
-00005410: 2061 7420 7b6c 6f6c 6c6d 735f 6170 702e   at {lollms_app.
-00005420: 636f 6e66 6967 7572 6174 696f 6e5f 7061  configuration_pa
-00005430: 7468 7d20 6f72 2075 7365 2074 6865 206e  th} or use the n
-00005440: 6578 7420 6d65 6e75 2074 6f20 7365 6c65  ext menu to sele
-00005450: 6374 2061 2076 616c 6964 2070 6572 736f  ct a valid perso
-00005460: 6e61 6c69 7479 2229 0d0a 2020 2020 2020  nality")..      
-00005470: 2020 2020 2020 4153 4349 4943 6f6c 6f72        ASCIIColor
-00005480: 732e 6572 726f 7228 6622 4269 6e64 696e  s.error(f"Bindin
-00005490: 6720 7265 7475 726e 6564 2074 6869 7320  g returned this 
-000054a0: 6578 6365 7074 696f 6e20 3a20 7b65 787d  exception : {ex}
-000054b0: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-000054c0: 7472 6163 655f 6578 6365 7074 696f 6e28  trace_exception(
-000054d0: 6578 290d 0a20 2020 2020 2020 2020 2020  ex)..           
-000054e0: 2041 5343 4949 436f 6c6f 7273 2e65 7272   ASCIIColors.err
-000054f0: 6f72 2866 227b 6c6f 6c6c 6d73 5f61 7070  or(f"{lollms_app
-00005500: 2e63 6f6e 6669 672e 6765 745f 7065 7273  .config.get_pers
-00005510: 6f6e 616c 6974 795f 7061 7468 5f69 6e66  onality_path_inf
-00005520: 6f73 2829 7d22 290d 0a20 2020 2020 2020  os()}")..       
-00005530: 2020 2020 2070 7269 6e74 2822 506c 6561       print("Plea
-00005540: 7365 2073 656c 6563 7420 6120 7661 6c69  se select a vali
-00005550: 6420 6d6f 6465 6c20 6f72 2069 6e73 7461  d model or insta
-00005560: 6c6c 2061 206e 6577 206f 6e65 2066 726f  ll a new one fro
-00005570: 6d20 6120 7572 6c22 290d 0a20 2020 2020  m a url")..     
-00005580: 2020 2020 2020 2073 656c 662e 7365 6c65         self.sele
-00005590: 6374 5f6d 6f64 656c 2829 0d0a 0d0a 2020  ct_model()....  
-000055a0: 2020 6465 6620 6d61 696e 5f6d 656e 7528    def main_menu(
-000055b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000055c0: 7365 6c66 2e73 686f 7728 290d 0a0d 0a    self.show()....
+000045c0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+000045d0: 2020 2020 2020 2020 2020 2020 2020 4153                AS
+000045e0: 4349 4943 6f6c 6f72 732e 6772 6565 6e28  CIIColors.green(
+000045f0: 6622 7b69 642b 317d 202d 207b 656e 7472  f"{id+1} - {entr
+00004600: 797d 2229 0d0a 2020 2020 2020 2020 7365  y}")..        se
+00004610: 6c66 2e73 686f 775f 6d65 6e75 285b 2242  lf.show_menu(["B
+00004620: 6163 6b22 5d29 0d0a 0d0a 0d0a 2020 2020  ack"])......    
+00004630: 6465 6620 756e 6d6f 756e 745f 7065 7273  def unmount_pers
+00004640: 6f6e 616c 6974 7928 7365 6c66 293a 0d0a  onality(self):..
+00004650: 2020 2020 2020 2020 4153 4349 4943 6f6c          ASCIICol
+00004660: 6f72 732e 696e 666f 2822 5365 6c65 6374  ors.info("Select
+00004670: 2070 6572 736f 6e61 6c69 7479 2074 6f20   personality to 
+00004680: 756e 6d6f 756e 7422 290d 0a20 2020 2020  unmount")..     
+00004690: 2020 2065 6e74 7269 6573 203d 2073 656c     entries = sel
+000046a0: 662e 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e  f.lollms_app.con
+000046b0: 6669 675b 2770 6572 736f 6e61 6c69 7469  fig['personaliti
+000046c0: 6573 275d 2b5b 2242 6163 6b22 5d0d 0a20  es']+["Back"].. 
+000046d0: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+000046e0: 2020 2020 2020 2020 2063 686f 6963 6520           choice 
+000046f0: 3d20 696e 7428 7365 6c66 2e73 686f 775f  = int(self.show_
+00004700: 6d65 6e75 2865 6e74 7269 6573 2c20 7365  menu(entries, se
+00004710: 6c66 2e6c 6f6c 6c6d 735f 6170 702e 636f  lf.lollms_app.co
+00004720: 6e66 6967 5b27 6163 7469 7665 5f70 6572  nfig['active_per
+00004730: 736f 6e61 6c69 7479 5f69 6427 5d29 292d  sonality_id']))-
+00004740: 310d 0a20 2020 2020 2020 2020 2020 2069  1..            i
+00004750: 6620 6368 6f69 6365 3c6c 656e 2865 6e74  f choice<len(ent
+00004760: 7269 6573 292d 313a 0d0a 2020 2020 2020  ries)-1:..      
+00004770: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+00004780: 6f6c 6c6d 735f 6170 702e 756e 6d6f 756e  ollms_app.unmoun
+00004790: 745f 7065 7273 6f6e 616c 6974 7928 6368  t_personality(ch
+000047a0: 6f69 6365 290d 0a20 2020 2020 2020 2065  oice)..        e
+000047b0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000047c0: 6173 2065 783a 0d0a 2020 2020 2020 2020  as ex:..        
+000047d0: 2020 2020 4153 4349 4943 6f6c 6f72 732e      ASCIIColors.
+000047e0: 6572 726f 7228 6622 436f 756c 646e 2774  error(f"Couldn't
+000047f0: 2075 686e 6d6f 756e 7420 7065 7273 6f6e   uhnmount person
+00004800: 616c 6974 792e 5c6e 476f 7420 7468 6973  ality.\nGot this
+00004810: 2065 7863 6570 7469 6f6e 3a7b 6578 7d22   exception:{ex}"
+00004820: 290d 0a0d 0a20 2020 2064 6566 2073 656c  )....    def sel
+00004830: 6563 745f 7065 7273 6f6e 616c 6974 7928  ect_personality(
+00004840: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00004850: 4153 4349 4943 6f6c 6f72 732e 696e 666f  ASCIIColors.info
+00004860: 2822 5365 6c65 6374 2070 6572 736f 6e61  ("Select persona
+00004870: 6c69 7479 2074 6f20 6163 7469 7661 7465  lity to activate
+00004880: 2229 0d0a 2020 2020 2020 2020 656e 7472  ")..        entr
+00004890: 6965 7320 3d20 7365 6c66 2e6c 6f6c 6c6d  ies = self.lollm
+000048a0: 735f 6170 702e 636f 6e66 6967 5b27 7065  s_app.config['pe
+000048b0: 7273 6f6e 616c 6974 6965 7327 5d2b 5b22  rsonalities']+["
+000048c0: 4261 636b 225d 0d0a 2020 2020 2020 2020  Back"]..        
+000048d0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+000048e0: 2020 6368 6f69 6365 203d 2069 6e74 2873    choice = int(s
+000048f0: 656c 662e 7368 6f77 5f6d 656e 7528 656e  elf.show_menu(en
+00004900: 7472 6965 732c 2073 656c 662e 6c6f 6c6c  tries, self.loll
+00004910: 6d73 5f61 7070 2e63 6f6e 6669 675b 2761  ms_app.config['a
+00004920: 6374 6976 655f 7065 7273 6f6e 616c 6974  ctive_personalit
+00004930: 795f 6964 275d 2929 2d31 0d0a 2020 2020  y_id']))-1..    
+00004940: 2020 2020 2020 2020 6966 2063 686f 6963          if choic
+00004950: 653c 6c65 6e28 656e 7472 6965 7329 2d31  e<len(entries)-1
+00004960: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004970: 2020 2073 656c 662e 6c6f 6c6c 6d73 5f61     self.lollms_a
+00004980: 7070 2e73 656c 6563 745f 7065 7273 6f6e  pp.select_person
+00004990: 616c 6974 7928 6368 6f69 6365 290d 0a20  ality(choice).. 
+000049a0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+000049b0: 6365 7074 696f 6e20 6173 2065 783a 0d0a  ception as ex:..
+000049c0: 2020 2020 2020 2020 2020 2020 4153 4349              ASCI
+000049d0: 4943 6f6c 6f72 732e 6572 726f 7228 6622  IColors.error(f"
+000049e0: 436f 756c 646e 2774 2073 6574 2070 6572  Couldn't set per
+000049f0: 736f 6e61 6c69 7479 2e5c 6e47 6f74 2074  sonality.\nGot t
+00004a00: 6869 7320 6578 6365 7074 696f 6e3a 7b65  his exception:{e
+00004a10: 787d 2229 0d0a 0d0a 2020 2020 6465 6620  x}")....    def 
+00004a20: 7265 696e 7374 616c 6c5f 6269 6e64 696e  reinstall_bindin
+00004a30: 6728 7365 6c66 293a 0d0a 2020 2020 2020  g(self):..      
+00004a40: 2020 6c6f 6c6c 6d73 5f61 7070 203d 2073    lollms_app = s
+00004a50: 656c 662e 6c6f 6c6c 6d73 5f61 7070 0d0a  elf.lollms_app..
+00004a60: 2020 2020 2020 2020 6269 6e64 696e 6773          bindings
+00004a70: 5f6c 6973 7420 3d20 5b5d 0d0a 2020 2020  _list = []..    
+00004a80: 2020 2020 7072 696e 7428 290d 0a20 2020      print()..   
+00004a90: 2020 2020 2070 7269 6e74 2866 227b 4153       print(f"{AS
+00004aa0: 4349 4943 6f6c 6f72 732e 636f 6c6f 725f  CIIColors.color_
+00004ab0: 6772 6565 6e7d 4375 7272 656e 7420 6269  green}Current bi
+00004ac0: 6e64 696e 673a 207b 4153 4349 4943 6f6c  nding: {ASCIICol
+00004ad0: 6f72 732e 636f 6c6f 725f 7265 7365 747d  ors.color_reset}
+00004ae0: 7b73 656c 662e 6c6f 6c6c 6d73 5f61 7070  {self.lollms_app
+00004af0: 2e63 6f6e 6669 675b 2762 696e 6469 6e67  .config['binding
+00004b00: 5f6e 616d 6527 5d7d 2229 0d0a 2020 2020  _name']}")..    
+00004b10: 2020 2020 666f 7220 7020 696e 2073 656c      for p in sel
+00004b20: 662e 6c6f 6c6c 6d73 5f61 7070 2e6c 6f6c  f.lollms_app.lol
+00004b30: 6c6d 735f 7061 7468 732e 6269 6e64 696e  lms_paths.bindin
+00004b40: 6773 5f7a 6f6f 5f70 6174 682e 6974 6572  gs_zoo_path.iter
+00004b50: 6469 7228 293a 0d0a 2020 2020 2020 2020  dir():..        
+00004b60: 2020 2020 6966 2070 2e69 735f 6469 7228      if p.is_dir(
+00004b70: 2920 616e 6420 6e6f 7420 702e 7374 656d  ) and not p.stem
+00004b80: 2e73 7461 7274 7377 6974 6828 222e 2229  .startswith(".")
+00004b90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00004ba0: 2020 2077 6974 6820 6f70 656e 2870 2f22     with open(p/"
+00004bb0: 6269 6e64 696e 675f 6361 7264 2e79 616d  binding_card.yam
+00004bc0: 6c22 2c20 2272 2229 2061 7320 663a 0d0a  l", "r") as f:..
+00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004be0: 2020 2020 6361 7264 203d 2079 616d 6c2e      card = yaml.
+00004bf0: 7361 6665 5f6c 6f61 6428 6629 0d0a 2020  safe_load(f)..  
+00004c00: 2020 2020 2020 2020 2020 2020 2020 7769                wi
+00004c10: 7468 206f 7065 6e28 702f 226d 6f64 656c  th open(p/"model
+00004c20: 732e 7961 6d6c 222c 2022 7222 2920 6173  s.yaml", "r") as
+00004c30: 2066 3a0d 0a20 2020 2020 2020 2020 2020   f:..           
+00004c40: 2020 2020 2020 2020 206d 6f64 656c 7320           models 
+00004c50: 3d20 7961 6d6c 2e73 6166 655f 6c6f 6164  = yaml.safe_load
+00004c60: 2866 290d 0a20 2020 2020 2020 2020 2020  (f)..           
+00004c70: 2020 2020 2069 735f 696e 7374 616c 6c65       is_installe
+00004c80: 6420 3d20 2873 656c 662e 6c6f 6c6c 6d73  d = (self.lollms
+00004c90: 5f61 7070 2e6c 6f6c 6c6d 735f 7061 7468  _app.lollms_path
+00004ca0: 732e 7065 7273 6f6e 616c 5f63 6f6e 6669  s.personal_confi
+00004cb0: 6775 7261 7469 6f6e 5f70 6174 682f 6622  guration_path/f"
+00004cc0: 6269 6e64 696e 675f 7b70 2e6e 616d 657d  binding_{p.name}
+00004cd0: 2e79 616d 6c22 292e 6578 6973 7473 2829  .yaml").exists()
+00004ce0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004cf0: 2020 656e 7472 793d 6622 7b41 5343 4949    entry=f"{ASCII
+00004d00: 436f 6c6f 7273 2e63 6f6c 6f72 5f67 7265  Colors.color_gre
+00004d10: 656e 2069 6620 6973 5f69 6e73 7461 6c6c  en if is_install
+00004d20: 6564 2065 6c73 6520 2727 7d7b 272a 2720  ed else ''}{'*' 
+00004d30: 6966 2073 656c 662e 6c6f 6c6c 6d73 5f61  if self.lollms_a
+00004d40: 7070 2e63 6f6e 6669 675b 2762 696e 6469  pp.config['bindi
+00004d50: 6e67 5f6e 616d 6527 5d3d 3d63 6172 645b  ng_name']==card[
+00004d60: 276e 616d 6527 5d20 656c 7365 2027 277d  'name'] else ''}
+00004d70: 207b 6361 7264 5b27 6e61 6d65 275d 7d20   {card['name']} 
+00004d80: 2862 7920 7b63 6172 645b 2761 7574 686f  (by {card['autho
+00004d90: 7227 5d7d 2922 0d0a 2020 2020 2020 2020  r']})"..        
+00004da0: 2020 2020 2020 2020 6269 6e64 696e 6773          bindings
+00004db0: 5f6c 6973 742e 6170 7065 6e64 2865 6e74  _list.append(ent
+00004dc0: 7279 290d 0a20 2020 2020 2020 2020 2020  ry)..           
+00004dd0: 2020 2020 2065 6e74 7279 3d7b 0d0a 2020       entry={..  
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004df0: 2020 226e 616d 6522 3a70 2e6e 616d 652c    "name":p.name,
+00004e00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004e10: 2020 2020 2020 2263 6172 6422 3a63 6172        "card":car
+00004e20: 642c 0d0a 2020 2020 2020 2020 2020 2020  d,..            
+00004e30: 2020 2020 2020 2020 226d 6f64 656c 7322          "models"
+00004e40: 3a6d 6f64 656c 732c 0d0a 2020 2020 2020  :models,..      
+00004e50: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00004e60: 6e73 7461 6c6c 6564 223a 2069 735f 696e  nstalled": is_in
+00004e70: 7374 616c 6c65 640d 0a20 2020 2020 2020  stalled..       
+00004e80: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
+00004e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004ea0: 2e62 696e 6469 6e67 5f69 6e66 732e 6170  .binding_infs.ap
+00004eb0: 7065 6e64 2865 6e74 7279 290d 0a20 2020  pend(entry)..   
+00004ec0: 2020 2020 2062 696e 6469 6e67 735f 6c69       bindings_li
+00004ed0: 7374 202b 3d20 5b22 4261 636b 225d 0d0a  st += ["Back"]..
+00004ee0: 2020 2020 2020 2020 6368 6f69 6365 203d          choice =
+00004ef0: 2073 656c 662e 7368 6f77 5f6d 656e 7528   self.show_menu(
+00004f00: 6269 6e64 696e 6773 5f6c 6973 7429 0d0a  bindings_list)..
+00004f10: 2020 2020 2020 2020 6966 2031 203c 3d20          if 1 <= 
+00004f20: 6368 6f69 6365 203c 3d20 6c65 6e28 6269  choice <= len(bi
+00004f30: 6e64 696e 6773 5f6c 6973 7429 2d31 3a0d  ndings_list)-1:.
+00004f40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004f50: 6e74 2866 2259 6f75 2073 656c 6563 7465  nt(f"You selecte
+00004f60: 6420 6269 6e64 696e 673a 207b 4153 4349  d binding: {ASCI
+00004f70: 4943 6f6c 6f72 732e 636f 6c6f 725f 6772  IColors.color_gr
+00004f80: 6565 6e7d 7b73 656c 662e 6269 6e64 696e  een}{self.bindin
+00004f90: 675f 696e 6673 5b63 686f 6963 6520 2d20  g_infs[choice - 
+00004fa0: 315d 5b27 6e61 6d65 275d 7d7b 4153 4349  1]['name']}{ASCI
+00004fb0: 4943 6f6c 6f72 732e 636f 6c6f 725f 7265  IColors.color_re
+00004fc0: 7365 747d 2229 0d0a 2020 2020 2020 2020  set}")..        
+00004fd0: 2020 2020 7365 6c66 2e6c 6f6c 6c6d 735f      self.lollms_
+00004fe0: 6170 702e 636f 6e66 6967 5b27 6269 6e64  app.config['bind
+00004ff0: 696e 675f 6e61 6d65 275d 3d73 656c 662e  ing_name']=self.
+00005000: 6269 6e64 696e 675f 696e 6673 5b63 686f  binding_infs[cho
+00005010: 6963 6520 2d20 315d 5b27 6e61 6d65 275d  ice - 1]['name']
+00005020: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00005030: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
+00005040: 2020 2020 2020 6c6f 6c6c 6d73 5f61 7070        lollms_app
+00005050: 2e62 696e 6469 6e67 203d 2042 696e 6469  .binding = Bindi
+00005060: 6e67 4275 696c 6465 7228 292e 6275 696c  ngBuilder().buil
+00005070: 645f 6269 6e64 696e 6728 6c6f 6c6c 6d73  d_binding(lollms
+00005080: 5f61 7070 2e63 6f6e 6669 672c 206c 6f6c  _app.config, lol
+00005090: 6c6d 735f 6170 702e 6c6f 6c6c 6d73 5f70  lms_app.lollms_p
+000050a0: 6174 6873 2c49 6e73 7461 6c6c 4f70 7469  aths,InstallOpti
+000050b0: 6f6e 2e46 4f52 4345 5f49 4e53 5441 4c4c  on.FORCE_INSTALL
+000050c0: 290d 0a20 2020 2020 2020 2020 2020 2065  )..            e
+000050d0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
+000050e0: 6173 2065 783a 0d0a 2020 2020 2020 2020  as ex:..        
+000050f0: 2020 2020 2020 2020 7072 696e 7428 6578          print(ex
+00005100: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00005110: 2020 2070 7269 6e74 2866 2243 6f75 6c64     print(f"Could
+00005120: 6e27 7420 6669 6e64 2062 696e 6469 6e67  n't find binding
+00005130: 2e20 506c 6561 7365 2076 6572 6966 7920  . Please verify 
+00005140: 796f 7572 2063 6f6e 6669 6775 7261 7469  your configurati
+00005150: 6f6e 2066 696c 6520 6174 207b 6c6f 6c6c  on file at {loll
+00005160: 6d73 5f61 7070 2e63 6f6e 6669 672e 6669  ms_app.config.fi
+00005170: 6c65 5f70 6174 687d 206f 7220 7573 6520  le_path} or use 
+00005180: 7468 6520 6e65 7874 206d 656e 7520 746f  the next menu to
+00005190: 2073 656c 6563 7420 6120 7661 6c69 6420   select a valid 
+000051a0: 6269 6e64 696e 6722 290d 0a20 2020 2020  binding")..     
+000051b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000051c0: 7365 6c65 6374 5f62 696e 6469 6e67 2829  select_binding()
+000051d0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000051e0: 7365 6c66 2e6c 6f6c 6c6d 735f 6170 702e  self.lollms_app.
+000051f0: 636f 6e66 6967 5b27 6d6f 6465 6c5f 6e61  config['model_na
+00005200: 6d65 275d 3d4e 6f6e 650d 0a20 2020 2020  me']=None..     
+00005210: 2020 2020 2020 2073 656c 662e 6c6f 6c6c         self.loll
+00005220: 6d73 5f61 7070 2e63 6f6e 6669 672e 7361  ms_app.config.sa
+00005230: 7665 5f63 6f6e 6669 6728 290d 0a20 2020  ve_config()..   
+00005240: 2020 2020 2065 6c69 6620 6368 6f69 6365       elif choice
+00005250: 203c 3d20 6c65 6e28 6269 6e64 696e 6773   <= len(bindings
+00005260: 5f6c 6973 7429 3a0d 0a20 2020 2020 2020  _list):..       
+00005270: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+00005280: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00005290: 2020 2020 2020 2020 7072 696e 7428 2249          print("I
+000052a0: 6e76 616c 6964 2063 686f 6963 6521 2229  nvalid choice!")
+000052b0: 2020 2020 2020 2020 0d0a 0d0a 0d0a 2020          ......  
+000052c0: 2020 0d0a 2020 2020 6465 6620 7265 696e    ..    def rein
+000052d0: 7374 616c 6c5f 7065 7273 6f6e 616c 6974  stall_personalit
+000052e0: 7928 7365 6c66 2c20 6361 6c6c 6261 636b  y(self, callback
+000052f0: 3d4e 6f6e 6529 3a0d 0a20 2020 2020 2020  =None):..       
+00005300: 206c 6f6c 6c6d 735f 6170 7020 3d20 7365   lollms_app = se
+00005310: 6c66 2e6c 6f6c 6c6d 735f 6170 700d 0a20  lf.lollms_app.. 
+00005320: 2020 2020 2020 2074 7279 3a0d 0a20 2020         try:..   
+00005330: 2020 2020 2020 2020 206c 6f6c 6c6d 735f           lollms_
+00005340: 6170 702e 7065 7273 6f6e 616c 6974 7920  app.personality 
+00005350: 3d20 5065 7273 6f6e 616c 6974 7942 7569  = PersonalityBui
+00005360: 6c64 6572 286c 6f6c 6c6d 735f 6170 702e  lder(lollms_app.
+00005370: 6c6f 6c6c 6d73 5f70 6174 6873 2c20 6c6f  lollms_paths, lo
+00005380: 6c6c 6d73 5f61 7070 2e63 6f6e 6669 672c  llms_app.config,
+00005390: 206c 6f6c 6c6d 735f 6170 702e 6d6f 6465   lollms_app.mode
+000053a0: 6c2c 2069 6e73 7461 6c6c 6174 696f 6e5f  l, installation_
+000053b0: 6f70 7469 6f6e 3d49 6e73 7461 6c6c 4f70  option=InstallOp
+000053c0: 7469 6f6e 2e46 4f52 4345 5f49 4e53 5441  tion.FORCE_INSTA
+000053d0: 4c4c 2c20 6361 6c6c 6261 636b 3d63 616c  LL, callback=cal
+000053e0: 6c62 6163 6b29 2e62 7569 6c64 5f70 6572  lback).build_per
+000053f0: 736f 6e61 6c69 7479 2829 0d0a 2020 2020  sonality()..    
+00005400: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00005410: 7469 6f6e 2061 7320 6578 3a0d 0a20 2020  tion as ex:..   
+00005420: 2020 2020 2020 2020 2041 5343 4949 436f           ASCIICo
+00005430: 6c6f 7273 2e65 7272 6f72 2866 2243 6f75  lors.error(f"Cou
+00005440: 6c64 6e27 7420 6c6f 6164 2070 6572 736f  ldn't load perso
+00005450: 6e61 6c69 7479 2e20 506c 6561 7365 2076  nality. Please v
+00005460: 6572 6966 7920 796f 7572 2063 6f6e 6669  erify your confi
+00005470: 6775 7261 7469 6f6e 2066 696c 6520 6174  guration file at
+00005480: 207b 6c6f 6c6c 6d73 5f61 7070 2e63 6f6e   {lollms_app.con
+00005490: 6669 6775 7261 7469 6f6e 5f70 6174 687d  figuration_path}
+000054a0: 206f 7220 7573 6520 7468 6520 6e65 7874   or use the next
+000054b0: 206d 656e 7520 746f 2073 656c 6563 7420   menu to select 
+000054c0: 6120 7661 6c69 6420 7065 7273 6f6e 616c  a valid personal
+000054d0: 6974 7922 290d 0a20 2020 2020 2020 2020  ity")..         
+000054e0: 2020 2041 5343 4949 436f 6c6f 7273 2e65     ASCIIColors.e
+000054f0: 7272 6f72 2866 2242 696e 6469 6e67 2072  rror(f"Binding r
+00005500: 6574 7572 6e65 6420 7468 6973 2065 7863  eturned this exc
+00005510: 6570 7469 6f6e 203a 207b 6578 7d22 290d  eption : {ex}").
+00005520: 0a20 2020 2020 2020 2020 2020 2074 7261  .            tra
+00005530: 6365 5f65 7863 6570 7469 6f6e 2865 7829  ce_exception(ex)
+00005540: 0d0a 2020 2020 2020 2020 2020 2020 4153  ..            AS
+00005550: 4349 4943 6f6c 6f72 732e 6572 726f 7228  CIIColors.error(
+00005560: 6622 7b6c 6f6c 6c6d 735f 6170 702e 636f  f"{lollms_app.co
+00005570: 6e66 6967 2e67 6574 5f70 6572 736f 6e61  nfig.get_persona
+00005580: 6c69 7479 5f70 6174 685f 696e 666f 7328  lity_path_infos(
+00005590: 297d 2229 0d0a 2020 2020 2020 2020 2020  )}")..          
+000055a0: 2020 7072 696e 7428 2250 6c65 6173 6520    print("Please 
+000055b0: 7365 6c65 6374 2061 2076 616c 6964 206d  select a valid m
+000055c0: 6f64 656c 206f 7220 696e 7374 616c 6c20  odel or install 
+000055d0: 6120 6e65 7720 6f6e 6520 6672 6f6d 2061  a new one from a
+000055e0: 2075 726c 2229 0d0a 2020 2020 2020 2020   url")..        
+000055f0: 2020 2020 7365 6c66 2e73 656c 6563 745f      self.select_
+00005600: 6d6f 6465 6c28 290d 0a0d 0a20 2020 2064  model()....    d
+00005610: 6566 206d 6169 6e5f 6d65 6e75 2873 656c  ef main_menu(sel
+00005620: 6629 3a0d 0a20 2020 2020 2020 2073 656c  f):..        sel
+00005630: 662e 7368 6f77 2829 0d0a 0d0a            f.show()....
```

### Comparing `lollms-2.2.0/lollms/types.py` & `lollms-2.2.1/lollms/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     MSG_TYPE_JSON_INFOS             = 11# A JSON output that is useful for summarizing the process of generation used by personalities like chain of thoughts and tree of thooughts
     MSG_TYPE_REF                    = 12# References (in form of  [text](path))
     MSG_TYPE_CODE                   = 13# A javascript code to execute
     MSG_TYPE_UI                     = 14# A vue.js component to show (we need to build some and parse the text to show it)
 
     #Commands
     MSG_TYPE_NEW_MESSAGE            = 15# A new message
+    MSG_TYPE_FINISHED_MESSAGE       = 17# End of current message
+
 
 class GenerationPresets:
     """
     Class containing various generation presets.
     """
 
     @staticmethod
```

### Comparing `lollms-2.2.0/lollms/utilities.py` & `lollms-2.2.1/lollms/utilities.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/lollms.egg-info/PKG-INFO` & `lollms-2.2.1/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.0
+Version: 2.2.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.0/lollms.egg-info/SOURCES.txt` & `lollms-2.2.1/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.0/setup.py` & `lollms-2.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.0",
+    version="2.2.1",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

