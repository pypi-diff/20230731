# Comparing `tmp/MyNameBas-0.0.1.tar.gz` & `tmp/MyNameBas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyNameBas-0.0.1.tar", last modified: Mon Jul 31 13:59:12 2023, max compression
+gzip compressed data, was "MyNameBas-0.0.2.tar", last modified: Mon Jul 31 15:00:10 2023, max compression
```

## Comparing `MyNameBas-0.0.1.tar` & `MyNameBas-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 13:59:12.062715 MyNameBas-0.0.1/
--rw-rw-rw-   0        0        0     1071 2022-04-18 15:48:14.000000 MyNameBas-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1092 2022-04-18 15:48:14.000000 MyNameBas-0.0.1/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 13:59:12.052582 MyNameBas-0.0.1/MyNameBas/
--rw-rw-rw-   0        0        0       36 2023-07-31 12:03:52.000000 MyNameBas-0.0.1/MyNameBas/__init__.py
--rw-rw-rw-   0        0        0     1156 2023-07-31 11:48:32.000000 MyNameBas-0.0.1/MyNameBas/bas.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:59:12.062715 MyNameBas-0.0.1/MyNameBas.egg-info/
--rw-rw-rw-   0        0        0     2148 2023-07-31 13:59:12.000000 MyNameBas-0.0.1/MyNameBas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-07-31 13:59:12.000000 MyNameBas-0.0.1/MyNameBas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 13:59:12.000000 MyNameBas-0.0.1/MyNameBas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 13:59:12.000000 MyNameBas-0.0.1/MyNameBas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2148 2023-07-31 13:59:12.062715 MyNameBas-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1227 2023-07-31 13:38:32.000000 MyNameBas-0.0.1/README.rst
--rw-rw-rw-   0        0        0       86 2023-07-31 13:59:12.065228 MyNameBas-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1250 2023-07-31 13:57:54.000000 MyNameBas-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:00:10.509978 MyNameBas-0.0.2/
+-rw-rw-rw-   0        0        0     1081 2023-07-31 14:49:02.000000 MyNameBas-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1102 2023-07-31 14:49:02.000000 MyNameBas-0.0.2/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 15:00:10.501976 MyNameBas-0.0.2/MyNameBas/
+-rw-rw-rw-   0        0        0       36 2023-07-31 12:03:52.000000 MyNameBas-0.0.2/MyNameBas/__init__.py
+-rw-rw-rw-   0        0        0     1542 2023-07-31 14:52:14.000000 MyNameBas-0.0.2/MyNameBas/bas.py
+drwxrwxrwx   0        0        0        0 2023-07-31 15:00:10.509978 MyNameBas-0.0.2/MyNameBas.egg-info/
+-rw-rw-rw-   0        0        0     2168 2023-07-31 15:00:10.000000 MyNameBas-0.0.2/MyNameBas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-07-31 15:00:10.000000 MyNameBas-0.0.2/MyNameBas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 15:00:10.000000 MyNameBas-0.0.2/MyNameBas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 15:00:10.000000 MyNameBas-0.0.2/MyNameBas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2168 2023-07-31 15:00:10.509978 MyNameBas-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1227 2023-07-31 13:38:32.000000 MyNameBas-0.0.2/README.rst
+-rw-rw-rw-   0        0        0       86 2023-07-31 15:00:10.510978 MyNameBas-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1270 2023-07-31 14:49:02.000000 MyNameBas-0.0.2/setup.py
```

### Comparing `MyNameBas-0.0.1/LICENSE` & `MyNameBas-0.0.2/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Uncle Engineer
+Copyright (c) 2022 Chaikit Hirunrattanakorn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `MyNameBas-0.0.1/LICENSE.txt` & `MyNameBas-0.0.2/LICENSE.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Uncle Engineer
+Copyright (c) 2022 Chaikit Hirunrattanakorn
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `MyNameBas-0.0.1/MyNameBas/bas.py` & `MyNameBas-0.0.2/MyNameBas/bas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+import random
+
 class ClassOne:
     """
     ClassOne คือตัวทดสอบสำหรับ การเรียนรู้
     โดยใน class ให้ทดสอบโดย เขียน code
     เพื่อแนะนำตัวเอง
+
+    Example
+    # My.ShowName()
+    # My.ShowPage()
+    # My.About()
     """
 
     def __init__(self):
         self.name = 'บาส'
         self.page = 'https://folygon3d.com/'
 
     def ShowName(self):
@@ -19,15 +26,23 @@
         text = """
         ----------------------------------------
         สวัสดีจ้า ผมชื่อบาส ทำอาชีพ 3D จ้า
         สามารถติดตามผลงานของ page ผมได้เลยนะครับ
         ตอนนี้ผมพึ่งฝึกเรียนโปรแกรม Python อยู่ครับ
         ----------------------------------------"""
         print(text)
+
+    def dice(self):
+        list = ['1','2','3','4','5','6']
+        first = random.choice(list)
+        second = random.choice(list)
+        point = first + second
+        print(f'คุณสุ่มตัวเลขได้คะแนน {point} คะแนน')
  
 
 if __name__ == '__main__' :
     My = ClassOne()
     My.ShowName()
     My.ShowPage()
     My.About()
+    My.dice()
```

### Comparing `MyNameBas-0.0.1/MyNameBas.egg-info/PKG-INFO` & `MyNameBas-0.0.2/MyNameBas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MyNameBas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Who is Chaikit
-Home-page: https://github.com/chaikit
-Download-URL: https://github.com/chaikit
+Home-page: https://github.com/chaikit/MyNameBas
+Download-URL: https://github.com/chaikit/MyNameBas
 Author: Chaikit
 Author-email: foreground.3ds@gmail.com
 License: MIT
 Keywords: Name,Visual
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `MyNameBas-0.0.1/PKG-INFO` & `MyNameBas-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: MyNameBas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Who is Chaikit
-Home-page: https://github.com/chaikit
-Download-URL: https://github.com/chaikit
+Home-page: https://github.com/chaikit/MyNameBas
+Download-URL: https://github.com/chaikit/MyNameBas
 Author: Chaikit
 Author-email: foreground.3ds@gmail.com
 License: MIT
 Keywords: Name,Visual
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
```

### Comparing `MyNameBas-0.0.1/README.rst` & `MyNameBas-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `MyNameBas-0.0.1/setup.py` & `MyNameBas-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'MyNameBas',      
   packages = ['MyNameBas'], 
-  version = '0.0.1', 
+  version = '0.0.2', 
   license='MIT', 
   description = 'Who is Chaikit',
   long_description=DESCRIPTION,
   author = 'Chaikit',                 
   author_email = 'foreground.3ds@gmail.com',     
-  url = 'https://github.com/chaikit',  
-  download_url = 'https://github.com/chaikit',  
+  url = 'https://github.com/chaikit/MyNameBas',  
+  download_url = 'https://github.com/chaikit/MyNameBas',  
   keywords = ['Name', 'Visual'],
   classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Education',     
     'Topic :: Utilities',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',
```

