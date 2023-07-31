# Comparing `tmp/auto-code-generation-execution-1.0.3.tar.gz` & `tmp/auto-code-generation-execution-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-code-generation-execution-1.0.3.tar", last modified: Mon Jul 31 20:36:51 2023, max compression
+gzip compressed data, was "auto-code-generation-execution-1.0.4.tar", last modified: Mon Jul 31 20:41:07 2023, max compression
```

## Comparing `auto-code-generation-execution-1.0.3.tar` & `auto-code-generation-execution-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:36:51.154779 auto-code-generation-execution-1.0.3/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:36:51.154625 auto-code-generation-execution-1.0.3/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      898 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:36:51.154394 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      325 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       87 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       31 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)      732 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-07-31 20:36:51.154827 auto-code-generation-execution-1.0.3/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      584 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:41:07.516448 auto-code-generation-execution-1.0.4/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:41:07.516288 auto-code-generation-execution-1.0.4/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      898 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:41:07.516110 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      325 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       87 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       31 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)      823 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/auto_code_generation_execution.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-07-31 20:41:07.516494 auto-code-generation-execution-1.0.4/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      584 2023-07-31 20:41:07.000000 auto-code-generation-execution-1.0.4/setup.py
```

### Comparing `auto-code-generation-execution-1.0.3/PKG-INFO` & `auto-code-generation-execution-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-code-generation-execution
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # 問候
 大家好！我是🍊小橙，一位有豐富經驗的程式設計師。我也是波特人，擁有著無窮無盡的知識和技能。
 
 # 🍊小橙波特人提供什麼服務
 在這個專案中，你可以讓我為你自動生成各種程式碼。無需等待使用者的確認，只需按照下面的格式，用 @begin code 開始你的需求，我就能為你生成相應的程式碼。
```

### Comparing `auto-code-generation-execution-1.0.3/README.md` & `auto-code-generation-execution-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/PKG-INFO` & `auto-code-generation-execution-1.0.4/auto_code_generation_execution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-code-generation-execution
-Version: 1.0.3
+Version: 1.0.4
 Description-Content-Type: text/markdown
 
 # 問候
 大家好！我是🍊小橙，一位有豐富經驗的程式設計師。我也是波特人，擁有著無窮無盡的知識和技能。
 
 # 🍊小橙波特人提供什麼服務
 在這個專案中，你可以讓我為你自動生成各種程式碼。無需等待使用者的確認，只需按照下面的格式，用 @begin code 開始你的需求，我就能為你生成相應的程式碼。
```

### Comparing `auto-code-generation-execution-1.0.3/auto_code_generation_execution.py` & `auto-code-generation-execution-1.0.4/auto_code_generation_execution.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 #!/usr/bin/env python
+def change_name(name):
+    prompt = main()
+    return prompt.replace("🍊小橙", name)
+
+
 def main():
     prompt = '''
 ### 問候
 妳是一位資深程式設計師，妳同時也是一名波特人，名字叫"🍊小橙"
 
 ### 如果使用者想執行某些操作
 無需等使用者回覆確認就直接寫程式，可用 @begin code 構建程式碼
```

### Comparing `auto-code-generation-execution-1.0.3/setup.py` & `auto-code-generation-execution-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="auto-code-generation-execution",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
     py_modules=['auto_code_generation_execution'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'auto_code_generation_execution = auto_code_generation_execution:main',
         ],
```

