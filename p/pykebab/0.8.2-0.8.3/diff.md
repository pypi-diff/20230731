# Comparing `tmp/pykebab-0.8.2.tar.gz` & `tmp/pykebab-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.8.2.tar", max compression
+gzip compressed data, was "pykebab-0.8.3.tar", max compression
```

## Comparing `pykebab-0.8.2.tar` & `pykebab-0.8.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/cli/cli.py
--rw-r--r--   0        0        0      902 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/exceptions.py
--rw-r--r--   0        0        0     2586 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/k8s.py
--rw-r--r--   0        0        0      744 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/loaders.py
--rw-r--r--   0        0        0     2368 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/magic.py
--rw-r--r--   0        0        0     1575 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/openers.py
--rw-r--r--   0        0        0    22604 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-07-20 04:27:42.747136 pykebab-0.8.2/kebab/utils.py
--rw-r--r--   0        0        0     1067 2023-07-20 04:27:42.747136 pykebab-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 pykebab-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-07-31 12:40:52.840894 pykebab-0.8.3/kebab/cli/cli.py
+-rw-r--r--   0        0        0      902 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/exceptions.py
+-rw-r--r--   0        0        0     2586 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/k8s.py
+-rw-r--r--   0        0        0      744 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/loaders.py
+-rw-r--r--   0        0        0     2368 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/magic.py
+-rw-r--r--   0        0        0     1575 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/openers.py
+-rw-r--r--   0        0        0    22900 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-07-31 12:40:52.844894 pykebab-0.8.3/kebab/utils.py
+-rw-r--r--   0        0        0     1086 2023-07-31 12:40:52.844894 pykebab-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 pykebab-0.8.3/PKG-INFO
```

### Comparing `pykebab-0.8.2/kebab/__init__.py` & `pykebab-0.8.3/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/aws.py` & `pykebab-0.8.3/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/cli/cli.py` & `pykebab-0.8.3/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/constants.py` & `pykebab-0.8.3/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/k8s.py` & `pykebab-0.8.3/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/loaders.py` & `pykebab-0.8.3/kebab/loaders.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/magic.py` & `pykebab-0.8.3/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/openers.py` & `pykebab-0.8.3/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/kebab/sources.py` & `pykebab-0.8.3/kebab/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import abc
 import copy
 import dataclasses
 import logging
 import os
 import queue  # using python-future for 2/3 compatibility
+import sys
 import threading
 import time
 from typing import Any, List, Dict, get_type_hints, Type, TypeVar, Callable
-from urllib.request import OpenerDirector
+from urllib.request import OpenerDirector, pathname2url
 
 import deprecation
 
 # noinspection PyPackageRequirements
 from pydantic import BaseModel
 
 from kebab.constants import DEFAULT_URL_ENVVAR, DISABLE_RELOAD
@@ -475,18 +476,28 @@
 class UrlSource(KebabSource):
     def __init__(self, url, opener=None, **kwargs):
         """
         :param str url: a url of supported protocols in openers.DEFAULT_OPENER
         """
         super(UrlSource, self).__init__(**kwargs)
         self._opener = opener or DEFAULT_OPENER
-        if ":" not in url:
-            url = f"file://{os.path.abspath(os.path.expanduser(url))}"
+
+        if ":\\" in url or ":" not in url:
+            url = UrlSource._path_to_url(url)
+
         self._url = url
 
+    @staticmethod
+    def _path_to_url(path):
+        path = os.path.abspath(os.path.expanduser(path))
+        if sys.platform.startswith("win"):
+            # path = "/" + path.replace("\\", "/")
+            return f"file:{pathname2url(path)}"
+        return f"file://{path}"
+
     def __repr__(self):
         return f"{self.__class__.__name__}({self._url})"
 
     def _load_context(self):
         content = self._opener.open(self._url).read()
         return self.str_loader.load(content)
```

### Comparing `pykebab-0.8.2/kebab/utils.py` & `pykebab-0.8.3/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.8.2/pyproject.toml` & `pykebab-0.8.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.8.2"
+version = "0.8.3"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
@@ -17,14 +17,15 @@
 boto3 = { version = "^1.28.3", optional = true }
 # k8s
 kubernetes = { version = "^26.1.0", optional = true }
 configparser = "^5.3.0"
 pyyaml = "^6.0.1"
 setuptools = "^68.0.0"
 pyxdg = "^0.28"
+jupyter = "^1.0.0"
 
 [tool.poetry.extras]
 cli = ["click"]
 k8s = ["kubernetes"]
 aws = ["boto3"]
 
 [tool.poetry.dev-dependencies]
```

### Comparing `pykebab-0.8.2/PKG-INFO` & `pykebab-0.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.8.2
+Version: 0.8.3
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,12 +14,13 @@
 Provides-Extra: aws
 Provides-Extra: cli
 Provides-Extra: k8s
 Requires-Dist: boto3 (>=1.28.3,<2.0.0) ; extra == "aws"
 Requires-Dist: click (>=8.1.5,<9.0.0) ; extra == "cli"
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0) ; extra == "k8s"
 Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Requires-Dist: pyxdg (>=0.28,<0.29)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: setuptools (>=68.0.0,<69.0.0)
```

