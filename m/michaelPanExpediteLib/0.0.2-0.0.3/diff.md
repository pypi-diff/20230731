# Comparing `tmp/michaelPanExpediteLib-0.0.2.tar.gz` & `tmp/michaelPanExpediteLib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "michaelPanExpediteLib-0.0.2.tar", last modified: Mon Jul 31 03:07:37 2023, max compression
+gzip compressed data, was "michaelPanExpediteLib-0.0.3.tar", last modified: Mon Jul 31 05:34:06 2023, max compression
```

## Comparing `michaelPanExpediteLib-0.0.2.tar` & `michaelPanExpediteLib-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/
--rw-rw-rw-   0        0        0    35162 2023-07-31 01:11:34.000000 michaelPanExpediteLib-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2000 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1605 2023-07-31 03:06:58.000000 michaelPanExpediteLib-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.528417 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/
--rw-rw-rw-   0        0        0       41 2023-07-31 01:15:17.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/__init__.py
--rw-rw-rw-   0        0        0     2384 2023-07-31 03:05:47.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/expedite_array_circulation.py
-drwxrwxrwx   0        0        0        0 2023-07-31 03:07:37.532407 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/
--rw-rw-rw-   0        0        0     2000 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-31 03:07:37.000000 michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 03:07:37.533404 michaelPanExpediteLib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      765 2023-07-31 03:07:35.000000 michaelPanExpediteLib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:34:06.043677 michaelPanExpediteLib-0.0.3/
+-rw-rw-rw-   0        0        0    35162 2023-07-31 01:11:34.000000 michaelPanExpediteLib-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2023 2023-07-31 05:34:06.043677 michaelPanExpediteLib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1628 2023-07-31 05:33:17.000000 michaelPanExpediteLib-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 05:34:06.035699 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib/
+-rw-rw-rw-   0        0        0       41 2023-07-31 01:15:17.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib/__init__.py
+-rw-rw-rw-   0        0        0     2384 2023-07-31 03:05:47.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib/expedite_array_circulation.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:34:06.041683 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/
+-rw-rw-rw-   0        0        0     2023 2023-07-31 05:34:05.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-07-31 05:34:05.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:34:05.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-31 05:34:05.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-31 05:34:05.000000 michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:34:06.043677 michaelPanExpediteLib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-07-31 05:33:45.000000 michaelPanExpediteLib-0.0.3/setup.py
```

### Comparing `michaelPanExpediteLib-0.0.2/LICENSE` & `michaelPanExpediteLib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `michaelPanExpediteLib-0.0.2/PKG-INFO` & `michaelPanExpediteLib-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: michaelPanExpediteLib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Expedite array circulation
 Author: chuntong pan
 Author-email: panzhang1314@gmail.com
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,16 +12,16 @@
 License-File: LICENSE
 
 # 加速数组循环库(Accelerated array loop library)
 
 ## 1. 简介(abstract)
 
 ```
-由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库和tqdm库，加速数组循环的同时显示循环进度，目的是避免重复编写加速代码。
-Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library and tqdm library to accelerate the array loop while showing the loop progress, the purpose is to avoid repeated writing of acceleration code.
+由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库，加速数组循环的同时完成求差、和、均值等功能，目的是避免重复编写加速代码。
+Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library to accelerate the array cycle while completing the difference, sum, mean and other functions, the purpose is to avoid repeated writing of acceleration code.
 ```
 
 ## 2. 使用说明(Use Method)
 
 > * **install the lib**: pip install michaelPanExpediteLib
 >
 > * ```python
```

### Comparing `michaelPanExpediteLib-0.0.2/README.md` & `michaelPanExpediteLib-0.0.3/michaelPanExpediteLib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: michaelPanExpediteLib
+Version: 0.0.3
+Summary: Expedite array circulation
+Author: chuntong pan
+Author-email: panzhang1314@gmail.com
+Platform: all
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 加速数组循环库(Accelerated array loop library)
 
 ## 1. 简介(abstract)
 
 ```
-由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库和tqdm库，加速数组循环的同时显示循环进度，目的是避免重复编写加速代码。
-Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library and tqdm library to accelerate the array loop while showing the loop progress, the purpose is to avoid repeated writing of acceleration code.
+由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库，加速数组循环的同时完成求差、和、均值等功能，目的是避免重复编写加速代码。
+Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library to accelerate the array cycle while completing the difference, sum, mean and other functions, the purpose is to avoid repeated writing of acceleration code.
 ```
 
 ## 2. 使用说明(Use Method)
 
 > * **install the lib**: pip install michaelPanExpediteLib
 >
 > * ```python
```

### Comparing `michaelPanExpediteLib-0.0.2/michaelPanExpediteLib/expedite_array_circulation.py` & `michaelPanExpediteLib-0.0.3/michaelPanExpediteLib/expedite_array_circulation.py`

 * *Files identical despite different names*

### Comparing `michaelPanExpediteLib-0.0.2/michaelPanExpediteLib.egg-info/PKG-INFO` & `michaelPanExpediteLib-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: michaelPanExpediteLib
-Version: 0.0.2
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
-由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库和tqdm库，加速数组循环的同时显示循环进度，目的是避免重复编写加速代码。
-Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library and tqdm library to accelerate the array loop while showing the loop progress, the purpose is to avoid repeated writing of acceleration code.
+由于python语言的自身特性，导致其在循环上的效率很低，因此得采取一定措施提升速度。本库依托于numba库，加速数组循环的同时完成求差、和、均值等功能，目的是避免重复编写加速代码。
+Due to the characteristics of the python language, its efficiency in the loop is very low, so some measures must be taken to improve the speed. This library relies on numba library to accelerate the array cycle while completing the difference, sum, mean and other functions, the purpose is to avoid repeated writing of acceleration code.
 ```
 
 ## 2. 使用说明(Use Method)
 
 > * **install the lib**: pip install michaelPanExpediteLib
 >
 > * ```python
```

### Comparing `michaelPanExpediteLib-0.0.2/setup.py` & `michaelPanExpediteLib-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="michaelPanExpediteLib",  # 库的名称
-    version="0.0.2",  # 库的版本号
+    version="0.0.3",  # 库的版本号
     author="chuntong pan",  # 库的作者
     author_email="panzhang1314@gmail.com",  # 作者邮箱
     description="Expedite array circulation",  # 库的简述
-    install_requires=['numba', 'tqdm'],  # 需要的依赖库
+    install_requires=['numba'],  # 需要的依赖库
     long_description=long_description,
     long_description_content_type="text/markdown",
     platforms=["all"],
     packages=setuptools.find_packages(),
     classifiers=["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License",
                  "Operating System :: OS Independent"],
 )
```

