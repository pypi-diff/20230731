# Comparing `tmp/michaelPanExpediteLib-0.0.1.tar.gz` & `tmp/michaelPanExpediteLib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michaelPanExpediteLib-0.0.1.tar", last modified: Mon Jul 31 03:00:31 2023, max compression
+gzip compressed data, was "michaelPanExpediteLib-0.0.2.tar", last modified: Mon Jul 31 03:07:37 2023, max compression
```

## Comparing `michaelPanExpediteLib-0.0.1.tar` & `michaelPanExpediteLib-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 03:00:31.800936 michaelPanExpediteLib-0.0.1/
--rw-rw-rw-   0        0        0    35162 2023-07-31 01:11:34.000000 michaelPanExpediteLib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1978 2023-07-31 03:00:31.799935 michaelPanExpediteLib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1583 2023-07-31 02:58:24.000000 michaelPanExpediteLib-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 03:00:31.792209 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib/
--rw-rw-rw-   0        0        0       41 2023-07-31 01:15:17.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib/__init__.py
--rw-rw-rw-   0        0        0     2364 2023-07-31 02:51:45.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib/expedite_array_circulation.py
-drwxrwxrwx   0        0        0        0 2023-07-31 03:00:31.798193 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/
--rw-rw-rw-   0        0        0     1978 2023-07-31 03:00:31.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-31 03:00:31.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 03:00:31.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 03:00:31.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-31 03:00:31.000000 michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 03:00:31.800936 michaelPanExpediteLib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-07-31 03:00:30.000000 michaelPanExpediteLib-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/
+-rw-rw-rw-   0        0        0    35162 2023-07-31 01:11:34.000000 michaelPanExpediteLib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2000 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1605 2023-07-31 03:06:58.000000 michaelPanExpediteLib-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.528417 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/
+-rw-rw-rw-   0        0        0       41 2023-07-31 01:15:17.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-07-31 03:05:47.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/expedite_array_circulation.py
+drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.532407 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/
+-rw-rw-rw-   0        0        0     2000 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      765 2023-07-31 03:07:35.000000 michaelPanExpediteLib-0.0.2/setup.py
```

### Comparing `michaelPanExpediteLib-0.0.1/LICENSE` & `michaelPanExpediteLib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `michaelPanExpediteLib-0.0.1/PKG-INFO` & `michaelPanExpediteLib-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: michaelPanExpediteLib
-Version: 0.0.1
-Summary: Expedite array circulation
-Author: chuntong pan
-Author-email: panzhang1314@gmail.com
-Platform: all
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 加速数组循环库(Accelerated array loop library)
 
 ## 1. 简介(abstract)
 
 ```
 由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库和tqdm库，加速数组循环的同时显示循环进度，目的是避免重复编写加速代码。
 Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library and tqdm library to accelerate the array loop while showing the loop progress, the purpose is to avoid repeated writing of acceleration code.
@@ -22,15 +9,15 @@
 
 ## 2. 使用说明(Use Method)
 
 > * **install the lib**: pip install michaelPanExpediteLib
 >
 > * ```python
 >   import numpy as np
->   from expedite_array_circulation import circulation_array
+>   from michaelPanExpediteLib.expedite_array_circulation import circulation_array
 >   
 >   
 >   arr1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 >   arr2 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 >   temp_array = np.ones((3, 3))
 >   temp_array_num = np.zeros((3, 3))
 >   x_dim = 3
```

### Comparing `michaelPanExpediteLib-0.0.1/michaelPanExpediteLib/expedite_array_circulation.py` & `michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/expedite_array_circulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,15 @@
     :param data_fill: fill-value of arrays 1 and 2
     :param method: 'add' or 'mean' or 'divide' or 'multiply' or 'minus'
     :param temp_array_num: Counting array
     :return: output array and counting array
 
     an example are as follows:
         import numpy as np
-
-        from expedite_array_circulation import circulation_array
+        from michaelPanExpediteLib.expedite_array_circulation import circulation_array
 
         arr1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 
         arr2 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 
         temp_array = np.ones((3, 3))
```

### Comparing `michaelPanExpediteLib-0.0.1/michaelPanExpediteLib.egg-info/PKG-INFO` & `michaelPanExpediteLib-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: michaelPanExpediteLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Expedite array circulation
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,15 +22,15 @@
 
 ## 2. 使用说明(Use Method)
 
 > * **install the lib**: pip install michaelPanExpediteLib
 >
 > * ```python
 >   import numpy as np
->   from expedite_array_circulation import circulation_array
+>   from michaelPanExpediteLib.expedite_array_circulation import circulation_array
 >   
 >   
 >   arr1 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 >   arr2 = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
 >   temp_array = np.ones((3, 3))
 >   temp_array_num = np.zeros((3, 3))
 >   x_dim = 3
```

### Comparing `michaelPanExpediteLib-0.0.1/setup.py` & `michaelPanExpediteLib-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="michaelPanExpediteLib",  # 库的名称
-    version="0.0.1",  # 库的版本号
+    version="0.0.2",  # 库的版本号
     author="chuntong pan",  # 库的作者
     author_email="panzhang1314@gmail.com",  # 作者邮箱
     description="Expedite array circulation",  # 库的简述
     install_requires=['numba', 'tqdm'],  # 需要的依赖库
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["all"],
```

