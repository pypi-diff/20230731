# Comparing `tmp/lollms-2.2.2.tar.gz` & `tmp/lollms-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.2.tar", last modified: Mon Jul 31 12:21:25 2023, max compression
+gzip compressed data, was "lollms-2.2.3.tar", last modified: Mon Jul 31 20:04:57 2023, max compression
```

## Comparing `lollms-2.2.2.tar` & `lollms-2.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.622616 lollms-2.2.2/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.2/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-07-31 12:21:25.621618 lollms-2.2.2/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.529858 lollms-2.2.2/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.2/lollms/__init__.py
--rw-rw-rw-   0        0        0     9349 2023-07-30 22:50:46.000000 lollms-2.2.2/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.548869 lollms-2.2.2/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.2/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.549869 lollms-2.2.2/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.2/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.550869 lollms-2.2.2/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.595387 lollms-2.2.2/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.603385 lollms-2.2.2/lollms/apps/server/
--rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.2/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.611385 lollms-2.2.2/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.2/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.612387 lollms-2.2.2/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.2/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.2/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.2/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.620617 lollms-2.2.2/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.2/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.2/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.2/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.2/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.2/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.2/lollms/paths.py
--rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.2/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.2/lollms/terminal.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.2/lollms/types.py
--rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.2/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.547867 lollms-2.2.2/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 12:21:25.622616 lollms-2.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-07-31 12:15:03.000000 lollms-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.749146 lollms-2.2.3/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.3/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-31 20:04:57.749146 lollms-2.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.648646 lollms-2.2.3/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.3/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9442 2023-07-31 19:53:45.000000 lollms-2.2.3/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.674435 lollms-2.2.3/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.3/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.676436 lollms-2.2.3/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.3/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.678438 lollms-2.2.3/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.740678 lollms-2.2.3/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.741692 lollms-2.2.3/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.3/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.743702 lollms-2.2.3/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.3/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.744704 lollms-2.2.3/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.3/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.3/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.3/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.748147 lollms-2.2.3/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.3/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.3/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.3/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.3/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.3/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.3/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.3/lollms/paths.py
+-rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.3/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.3/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.3/lollms/types.py
+-rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.3/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-31 20:04:57.673437 lollms-2.2.3/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 20:04:57.000000 lollms-2.2.3/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 20:04:57.749146 lollms-2.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-31 19:57:11.000000 lollms-2.2.3/setup.py
```

### Comparing `lollms-2.2.2/LICENSE` & `lollms-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/PKG-INFO` & `lollms-2.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.2
+Version: 2.2.3
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.2/README.md` & `lollms-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/app.py` & `lollms-2.2.3/lollms/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,40 +50,41 @@
             trace_exception(ex)
 
         if self.config.binding_name is None:
             ASCIIColors.warning(f"No binding selected")
             if try_select_binding:
                 ASCIIColors.info("Please select a valid model or install a new one from a url")
                 self.menu.select_binding()
-        
+        else:
+            if load_binding:
+                try:
+                    self.binding            = self.load_binding()
+                except Exception as ex:
+                    ASCIIColors.error(f"Failed to load binding.\nReturned exception: {ex}")
+                    trace_exception(ex)
 
-        if load_binding:
-            try:
-                self.binding            = self.load_binding()
-            except Exception as ex:
-                ASCIIColors.error(f"Failed to load binding.\nReturned exception: {ex}")
-                trace_exception(ex)
-                self.binding            = None
+                if self.binding is not None:
+                    ASCIIColors.success(f"Binding {self.config.binding_name} loaded successfully.")
+                    if load_model:
+                        if self.config.model_name is None:
+                            ASCIIColors.warning(f"No model selected")
+                            if try_select_model:
+                                print("Please select a valid model")
+                                self.menu.select_model()
+                                
+                        if self.config.model_name is not None:
+                            try:
+                                self.model          = self.load_model()
+                            except Exception as ex:
+                                ASCIIColors.error(f"Failed to load model.\nReturned exception: {ex}")
+                                trace_exception(ex)
+                else:
+                    ASCIIColors.warning(f"Couldn't load binding {self.config.binding_name}.")
 
-            if self.binding is not None:
-                ASCIIColors.success(f"Binding {self.config.binding_name} loaded successfully.")
-                if load_model:
-                    if self.config.model_name is None:
-                        ASCIIColors.warning(f"No model selected")
-                        if try_select_model:
-                            print("Please select a valid model")
-                            self.menu.select_model()
-                    if self.config.model_name is not None:
-                        try:
-                            self.model          = self.load_model()
-                        except Exception as ex:
-                            ASCIIColors.error(f"Failed to load model.\nReturned exception: {ex}")
-                            trace_exception(ex)
-            else:
-                ASCIIColors.warning(f"Couldn't load binding {self.config.binding_name}.")
+            
         self.mount_personalities()
 
     def load_binding(self):
         try:
             binding = BindingBuilder().build_binding(self.config, self.lollms_paths)
             return binding    
         except Exception as ex:
```

### Comparing `lollms-2.2.2/lollms/apps/console/__init__.py` & `lollms-2.2.3/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/playground/static/LICENSE` & `lollms-2.2.3/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/playground/static/README.md` & `lollms-2.2.3/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/playground/static/index.html` & `lollms-2.2.3/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/playground/static/logo.png` & `lollms-2.2.3/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.2.3/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/server/__init__.py` & `lollms-2.2.3/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/apps/settings/__init__.py` & `lollms-2.2.3/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/assets/logo.png` & `lollms-2.2.3/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/binding.py` & `lollms-2.2.3/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/config.py` & `lollms-2.2.3/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/configs/config.yaml` & `lollms-2.2.3/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/data.py` & `lollms-2.2.3/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/extension.py` & `lollms-2.2.3/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/helpers.py` & `lollms-2.2.3/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/langchain_integration.py` & `lollms-2.2.3/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/main_config.py` & `lollms-2.2.3/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/paths.py` & `lollms-2.2.3/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/personality.py` & `lollms-2.2.3/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/terminal.py` & `lollms-2.2.3/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/types.py` & `lollms-2.2.3/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms/utilities.py` & `lollms-2.2.3/lollms/utilities.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/lollms.egg-info/PKG-INFO` & `lollms-2.2.3/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.2
+Version: 2.2.3
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.2/lollms.egg-info/SOURCES.txt` & `lollms-2.2.3/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.2/setup.py` & `lollms-2.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.2",
+    version="2.2.3",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

