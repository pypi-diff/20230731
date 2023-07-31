# Comparing `tmp/lollms-2.2.1.tar.gz` & `tmp/lollms-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.2.1.tar", last modified: Mon Jul 31 01:12:21 2023, max compression
+gzip compressed data, was "lollms-2.2.2.tar", last modified: Mon Jul 31 12:21:25 2023, max compression
```

## Comparing `lollms-2.2.1.tar` & `lollms-2.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.099380 lollms-2.2.1/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.1/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-07-31 01:12:21.098381 lollms-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.060347 lollms-2.2.1/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.1/lollms/__init__.py
--rw-rw-rw-   0        0        0     9349 2023-07-30 22:50:46.000000 lollms-2.2.1/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.078546 lollms-2.2.1/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.1/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.079546 lollms-2.2.1/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.080548 lollms-2.2.1/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.090672 lollms-2.2.1/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.091717 lollms-2.2.1/lollms/apps/server/
--rw-rw-rw-   0        0        0    34728 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.093720 lollms-2.2.1/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7681 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.094716 lollms-2.2.1/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.1/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.1/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.1/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.097380 lollms-2.2.1/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.1/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.1/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.1/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.1/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.1/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.1/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.1/lollms/paths.py
--rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.1/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.1/lollms/terminal.py
--rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.1/lollms/types.py
--rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.1/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-07-31 01:12:21.077547 lollms-2.2.1/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-31 01:12:20.000000 lollms-2.2.1/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 01:12:21.100379 lollms-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-07-30 23:44:34.000000 lollms-2.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.622616 lollms-2.2.2/
+-rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.2.2/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-07-31 12:21:25.621618 lollms-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.529858 lollms-2.2.2/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.2.2/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9349 2023-07-30 22:50:46.000000 lollms-2.2.2/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.548869 lollms-2.2.2/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.2.2/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.549869 lollms-2.2.2/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.2.2/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.550869 lollms-2.2.2/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.595387 lollms-2.2.2/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.603385 lollms-2.2.2/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.2.2/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.611385 lollms-2.2.2/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.2.2/lollms/apps/settings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.612387 lollms-2.2.2/lollms/assets/
+-rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.2.2/lollms/assets/logo.png
+-rw-rw-rw-   0        0        0    10963 2023-07-27 19:45:11.000000 lollms-2.2.2/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.2.2/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.620617 lollms-2.2.2/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.2.2/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.2.2/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.2.2/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.2.2/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.2.2/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.2.2/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.2.2/lollms/paths.py
+-rw-rw-rw-   0        0        0    50149 2023-07-30 23:55:31.000000 lollms-2.2.2/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.2.2/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2607 2023-07-30 23:55:13.000000 lollms-2.2.2/lollms/types.py
+-rw-rw-rw-   0        0        0    25307 2023-07-28 21:19:50.000000 lollms-2.2.2/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:21:25.547867 lollms-2.2.2/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-31 12:21:25.000000 lollms-2.2.2/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:21:25.622616 lollms-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-07-31 12:15:03.000000 lollms-2.2.2/setup.py
```

### Comparing `lollms-2.2.1/LICENSE` & `lollms-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/PKG-INFO` & `lollms-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.1
+Version: 2.2.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.1/README.md` & `lollms-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/app.py` & `lollms-2.2.2/lollms/app.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/console/__init__.py` & `lollms-2.2.2/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/playground/static/LICENSE` & `lollms-2.2.2/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/playground/static/README.md` & `lollms-2.2.2/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/playground/static/index.html` & `lollms-2.2.2/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/playground/static/logo.png` & `lollms-2.2.2/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.2.2/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/apps/server/__init__.py` & `lollms-2.2.2/lollms/apps/server/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from lollms.helpers import ASCIIColors
 from lollms.apps.console import MainMenu
 from lollms.paths import LollmsPaths
 from lollms.apps.console import MainMenu
 from lollms.app import LollmsApplication
 from lollms.utilities import TextVectorizer
 from typing import List, Tuple
+from typing import Callable
 import importlib
 from pathlib import Path
 import argparse
 import logging
 import yaml
 import copy
 import gc
```

### Comparing `lollms-2.2.1/lollms/apps/settings/__init__.py` & `lollms-2.2.2/lollms/apps/settings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import shutil
 from pathlib import Path
 import argparse
 from tqdm import tqdm
 from lollms.personality import PersonalityBuilder
 from lollms.apps.console import MainMenu
 from lollms.app import LollmsApplication
+from typing import Callable
 
 
 
 class Settings(LollmsApplication):
     def __init__(
                     self, 
                     configuration_path:str|Path=None,
```

### Comparing `lollms-2.2.1/lollms/assets/logo.png` & `lollms-2.2.2/lollms/assets/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/binding.py` & `lollms-2.2.2/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/config.py` & `lollms-2.2.2/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/configs/config.yaml` & `lollms-2.2.2/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/data.py` & `lollms-2.2.2/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/extension.py` & `lollms-2.2.2/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/helpers.py` & `lollms-2.2.2/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/langchain_integration.py` & `lollms-2.2.2/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/main_config.py` & `lollms-2.2.2/lollms/main_config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/paths.py` & `lollms-2.2.2/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/personality.py` & `lollms-2.2.2/lollms/personality.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/terminal.py` & `lollms-2.2.2/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/types.py` & `lollms-2.2.2/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms/utilities.py` & `lollms-2.2.2/lollms/utilities.py`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/lollms.egg-info/PKG-INFO` & `lollms-2.2.2/lollms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.2.1
+Version: 2.2.2
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.2.1/lollms.egg-info/SOURCES.txt` & `lollms-2.2.2/lollms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lollms-2.2.1/setup.py` & `lollms-2.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.2.1",
+    version="2.2.2",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

