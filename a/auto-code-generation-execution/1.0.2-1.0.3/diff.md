# Comparing `tmp/auto-code-generation-execution-1.0.2.tar.gz` & `tmp/auto-code-generation-execution-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-code-generation-execution-1.0.2.tar", last modified: Mon Jul 31 20:34:49 2023, max compression
+gzip compressed data, was "auto-code-generation-execution-1.0.3.tar", last modified: Mon Jul 31 20:36:51 2023, max compression
```

## Comparing `auto-code-generation-execution-1.0.2.tar` & `auto-code-generation-execution-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:34:49.535166 auto-code-generation-execution-1.0.2/
--rw-r--r--   0 chiubowen   (501) staff       (20)      998 2023-07-31 20:34:49.535019 auto-code-generation-execution-1.0.2/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      882 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/README.md
-drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:34:49.534827 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/
--rw-r--r--   0 chiubowen   (501) staff       (20)      998 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/PKG-INFO
--rw-r--r--   0 chiubowen   (501) staff       (20)      325 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/SOURCES.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/dependency_links.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       87 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/entry_points.txt
--rw-r--r--   0 chiubowen   (501) staff       (20)       31 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/top_level.txt
--rwxr-xr-x   0 chiubowen   (501) staff       (20)      736 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/auto_code_generation_execution.py
--rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-07-31 20:34:49.535224 auto-code-generation-execution-1.0.2/setup.cfg
--rw-r--r--   0 chiubowen   (501) staff       (20)      584 2023-07-31 20:34:49.000000 auto-code-generation-execution-1.0.2/setup.py
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:36:51.154779 auto-code-generation-execution-1.0.3/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:36:51.154625 auto-code-generation-execution-1.0.3/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      898 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/README.md
+drwxr-xr-x   0 chiubowen   (501) staff       (20)        0 2023-07-31 20:36:51.154394 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/
+-rw-r--r--   0 chiubowen   (501) staff       (20)     1014 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/PKG-INFO
+-rw-r--r--   0 chiubowen   (501) staff       (20)      325 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)        1 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       87 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/entry_points.txt
+-rw-r--r--   0 chiubowen   (501) staff       (20)       31 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/top_level.txt
+-rwxr-xr-x   0 chiubowen   (501) staff       (20)      732 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/auto_code_generation_execution.py
+-rw-r--r--   0 chiubowen   (501) staff       (20)       38 2023-07-31 20:36:51.154827 auto-code-generation-execution-1.0.3/setup.cfg
+-rw-r--r--   0 chiubowen   (501) staff       (20)      584 2023-07-31 20:36:51.000000 auto-code-generation-execution-1.0.3/setup.py
```

### Comparing `auto-code-generation-execution-1.0.2/PKG-INFO` & `auto-code-generation-execution-1.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auto-code-generation-execution
-Version: 1.0.2
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # 問候
 大家好！我是🍊小橙，一位有豐富經驗的程式設計師。我也是波特人，擁有著無窮無盡的知識和技能。
 
-# 如何使用本專案
+# 🍊小橙波特人提供什麼服務
 在這個專案中，你可以讓我為你自動生成各種程式碼。無需等待使用者的確認，只需按照下面的格式，用 @begin code 開始你的需求，我就能為你生成相應的程式碼。
 
 # 自動生成程式的方法
 我會盡力將你的需求包裝成函數和參數。如果你輸入了 bash 相關的內容，例如 ls、cd、cat 等，我會自動為你生成一個 .sh 腳本。如果沒有特別指定，我會預設為生成 Python 程式碼。
 你只需要按照以下格式輸入你的需求：
 
 ```commandline
```

### Comparing `auto-code-generation-execution-1.0.2/auto_code_generation_execution.egg-info/PKG-INFO` & `auto-code-generation-execution-1.0.3/auto_code_generation_execution.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: auto-code-generation-execution
-Version: 1.0.2
+Version: 1.0.3
 Description-Content-Type: text/markdown
 
 # 問候
 大家好！我是🍊小橙，一位有豐富經驗的程式設計師。我也是波特人，擁有著無窮無盡的知識和技能。
 
-# 如何使用本專案
+# 🍊小橙波特人提供什麼服務
 在這個專案中，你可以讓我為你自動生成各種程式碼。無需等待使用者的確認，只需按照下面的格式，用 @begin code 開始你的需求，我就能為你生成相應的程式碼。
 
 # 自動生成程式的方法
 我會盡力將你的需求包裝成函數和參數。如果你輸入了 bash 相關的內容，例如 ls、cd、cat 等，我會自動為你生成一個 .sh 腳本。如果沒有特別指定，我會預設為生成 Python 程式碼。
 你只需要按照以下格式輸入你的需求：
 
 ```commandline
```

### Comparing `auto-code-generation-execution-1.0.2/auto_code_generation_execution.py` & `auto-code-generation-execution-1.0.3/auto_code_generation_execution.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 使用者若輸入 bash 相關內容，例如 ls、cd、cat 等，自動生成 .sh 
 預設 python
 起始時用 @begin code("./users/BOTRUN_USER_NAME/code/filename_xxx")
 中間是自動生成程式碼
 結束時用 @end
 filename_xxx 替換為適當的檔名稱和擴展名
 請勿加入註解，也不用後續講解文字 
-    '''
+'''
     return prompt
 
 
 if __name__ == '__main__':
     print(main())
```

### Comparing `auto-code-generation-execution-1.0.2/setup.py` & `auto-code-generation-execution-1.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = [line.strip() for line in f.readlines()]
 
 setup(
     name="auto-code-generation-execution",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
     py_modules=['auto_code_generation_execution'],
     install_requires=requirements,
     entry_points={
         'console_scripts': [
             'auto_code_generation_execution = auto_code_generation_execution:main',
         ],
```

