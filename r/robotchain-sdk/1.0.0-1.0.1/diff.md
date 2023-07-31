# Comparing `tmp/robotchain_sdk-1.0.0.tar.gz` & `tmp/robotchain_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotchain_sdk-1.0.0.tar", last modified: Sat Jul 29 02:19:01 2023, max compression
+gzip compressed data, was "robotchain_sdk-1.0.1.tar", last modified: Mon Jul 31 16:10:28 2023, max compression
```

## Comparing `robotchain_sdk-1.0.0.tar` & `robotchain_sdk-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 02:19:01.255572 robotchain_sdk-1.0.0/
--rw-rw-rw-   0        0        0     1566 2023-07-29 02:19:01.255572 robotchain_sdk-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-29 02:19:01.239950 robotchain_sdk-1.0.0/robotchain_sdk/
--rw-rw-rw-   0        0        0      731 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.0/robotchain_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 02:19:01.255572 robotchain_sdk-1.0.0/robotchain_sdk/ros/
--rw-rw-rw-   0        0        0     1080 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.0/robotchain_sdk/ros/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 02:19:01.255572 robotchain_sdk-1.0.0/robotchain_sdk/utils/
--rw-rw-rw-   0        0        0      233 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.0/robotchain_sdk/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-29 02:19:01.239950 robotchain_sdk-1.0.0/robotchain_sdk.egg-info/
--rw-rw-rw-   0        0        0     1566 2023-07-29 02:19:01.000000 robotchain_sdk-1.0.0/robotchain_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-29 02:19:01.000000 robotchain_sdk-1.0.0/robotchain_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 02:19:01.000000 robotchain_sdk-1.0.0/robotchain_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-29 02:19:01.000000 robotchain_sdk-1.0.0/robotchain_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 02:19:01.255572 robotchain_sdk-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-29 02:18:16.000000 robotchain_sdk-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.863266 robotchain_sdk-1.0.1/
+-rw-rw-rw-   0        0        0       45 2023-07-31 16:09:08.000000 robotchain_sdk-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1948 2023-07-31 16:10:28.862267 robotchain_sdk-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.840267 robotchain_sdk-1.0.1/robotchain_sdk/
+-rw-rw-rw-   0        0        0      731 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.853260 robotchain_sdk-1.0.1/robotchain_sdk/ros/
+-rw-rw-rw-   0        0        0     1080 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/ros/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.860260 robotchain_sdk-1.0.1/robotchain_sdk/utils/
+-rw-rw-rw-   0        0        0      233 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.861260 robotchain_sdk-1.0.1/robotchain_sdk/utils/loging/
+-rw-rw-rw-   0        0        0     2849 2023-07-25 08:53:36.000000 robotchain_sdk-1.0.1/robotchain_sdk/utils/loging/loging.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:10:28.844266 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1948 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-31 16:10:28.000000 robotchain_sdk-1.0.1/robotchain_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:10:28.863266 robotchain_sdk-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-07-31 16:09:16.000000 robotchain_sdk-1.0.1/setup.py
```

### Comparing `robotchain_sdk-1.0.0/PKG-INFO` & `robotchain_sdk-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain_sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,38 @@
 ## 📖 Initialization
 
 > 安装相关依赖
 > 
 > Install the required dependencies.
 
 ```shell
-pip3 install colorlog websocket-client==0.48.0 requests pyserial roslibpy empy colcon-common-extensions pymongo tornado
+pip3 install robotchain-sdk colorlog websocket-client==0.48.0 requests pyserial roslibpy empy colcon-common-extensions pymongo tornado
+```
+
+## 📖 Using templates
+
+```python
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import robotchain_sdk as framework
+
+def robot_start(sdk):
+    while True:
+        pass
+
+def robot_message(sdk, message):
+    pass
+
+def robot_exit(sdk):
+    pass
+
+if __name__ == '__main__':
+    framework_sdk = framework.Init()
+    robot_start(framework_sdk)
 ```
 
 ## 📖 Development
 
 > 安装相关依赖
 >
 > Install the required dependencies.
```

### Comparing `robotchain_sdk-1.0.0/robotchain_sdk/__init__.py` & `robotchain_sdk-1.0.1/robotchain_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.0/robotchain_sdk/ros/__init__.py` & `robotchain_sdk-1.0.1/robotchain_sdk/ros/__init__.py`

 * *Files identical despite different names*

### Comparing `robotchain_sdk-1.0.0/robotchain_sdk.egg-info/PKG-INFO` & `robotchain_sdk-1.0.1/robotchain_sdk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotchain-sdk
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python development framework for robotchain.
 Home-page: https://github.com/geekros/python_framework_sdk
 Author: MakerYang
 Author-email: admin@wileho.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -24,15 +24,38 @@
 ## 📖 Initialization
 
 > 安装相关依赖
 > 
 > Install the required dependencies.
 
 ```shell
-pip3 install colorlog websocket-client==0.48.0 requests pyserial roslibpy empy colcon-common-extensions pymongo tornado
+pip3 install robotchain-sdk colorlog websocket-client==0.48.0 requests pyserial roslibpy empy colcon-common-extensions pymongo tornado
+```
+
+## 📖 Using templates
+
+```python
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import robotchain_sdk as framework
+
+def robot_start(sdk):
+    while True:
+        pass
+
+def robot_message(sdk, message):
+    pass
+
+def robot_exit(sdk):
+    pass
+
+if __name__ == '__main__':
+    framework_sdk = framework.Init()
+    robot_start(framework_sdk)
 ```
 
 ## 📖 Development
 
 > 安装相关依赖
 >
 > Install the required dependencies.
```

### Comparing `robotchain_sdk-1.0.0/setup.py` & `robotchain_sdk-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="robotchain_sdk",
-    version="1.0.0",
+    version="1.0.1",
     author="MakerYang",
     author_email="admin@wileho.com",
     description="Python development framework for robotchain.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geekros/python_framework_sdk",
     packages=find_packages(),
```

