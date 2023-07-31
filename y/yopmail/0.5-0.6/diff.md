# Comparing `tmp/yopmail-0.5.tar.gz` & `tmp/yopmail-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-0.5.tar", last modified: Mon Apr 10 11:32:37 2023, max compression
+gzip compressed data, was "yopmail-0.6.tar", last modified: Mon Jul 31 15:46:10 2023, max compression
```

## Comparing `yopmail-0.5.tar` & `yopmail-0.6.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 11:32:37.736312 yopmail-0.5/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-04-10 11:32:37.736376 yopmail-0.5/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-04-10 10:41:06.000000 yopmail-0.5/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)      125 2023-04-10 11:32:37.736594 yopmail-0.5/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      701 2023-04-10 11:30:57.000000 yopmail-0.5/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-04-10 11:32:37.736212 yopmail-0.5/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      182 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       13 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        3 2023-04-10 11:32:37.000000 yopmail-0.5/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.713805 yopmail-0.6/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 15:46:10.713865 yopmail-0.6/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-0.6/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)      125 2023-07-31 15:46:10.714061 yopmail-0.6/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      767 2023-07-31 15:44:20.000000 yopmail-0.6/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.712571 yopmail-0.6/src/
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.713698 yopmail-0.6/src/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      202 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       13 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-0.5/PKG-INFO` & `yopmail-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 0.5
+Version: 0.6
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `yopmail-0.5/README.md` & `yopmail-0.6/README.md`

 * *Files identical despite different names*

### Comparing `yopmail-0.5/setup.py` & `yopmail-0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='0.5',
+    version='0.6',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
-    py_modules=["ym"],
+    package_dir = {"": "src"},
+    packages = find_packages(where="src"),
     python_requires='>=3.8',
     url='https://github.com/rklf/yopmail',
     keywords='yopmail get mails retrieve scrap emails',
     install_requires=[
           'bs4',
           'requests',
       ],
```

### Comparing `yopmail-0.5/yopmail.egg-info/PKG-INFO` & `yopmail-0.6/src/yopmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 0.5
+Version: 0.6
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

