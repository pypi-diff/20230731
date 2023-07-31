# Comparing `tmp/yopmail-1.3.tar.gz` & `tmp/yopmail-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-1.3.tar", last modified: Mon Jul 31 16:43:45 2023, max compression
+gzip compressed data, was "yopmail-1.4.tar", last modified: Mon Jul 31 16:47:05 2023, max compression
```

## Comparing `yopmail-1.3.tar` & `yopmail-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:43:45.566497 yopmail-1.3/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:43:45.566379 yopmail-1.3/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.3/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.3/pyproject.toml
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:43:45.566542 yopmail-1.3/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:43:18.000000 yopmail-1.3/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:43:45.565582 yopmail-1.3/yopmail/
--rw-r--r--   0 rayhan     (503) staff       (20)       22 2023-07-31 16:42:55.000000 yopmail-1.3/yopmail/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.3/yopmail/yopmail.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:43:45.566212 yopmail-1.3/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:43:45.000000 yopmail-1.3/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      226 2023-07-31 16:43:45.000000 yopmail-1.3/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:43:45.000000 yopmail-1.3/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:43:45.000000 yopmail-1.3/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:43:45.000000 yopmail-1.3/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.802127 yopmail-1.4/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:47:05.802010 yopmail-1.4/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.4/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.4/pyproject.toml
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:47:05.802178 yopmail-1.4/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:46:50.000000 yopmail-1.4/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.801207 yopmail-1.4/yopmail/
+-rw-r--r--   0 rayhan     (503) staff       (20)       28 2023-07-31 16:46:29.000000 yopmail-1.4/yopmail/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.4/yopmail/yopmail.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:47:05.801839 yopmail-1.4/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      226 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:47:05.000000 yopmail-1.4/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-1.3/PKG-INFO` & `yopmail-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.3
+Version: 1.4
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `yopmail-1.3/README.md` & `yopmail-1.4/README.md`

 * *Files identical despite different names*

### Comparing `yopmail-1.3/setup.py` & `yopmail-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='1.3',
+    version='1.4',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
     packages = find_packages(),
```

### Comparing `yopmail-1.3/yopmail/yopmail.py` & `yopmail-1.4/yopmail/yopmail.py`

 * *Files identical despite different names*

### Comparing `yopmail-1.3/yopmail.egg-info/PKG-INFO` & `yopmail-1.4/yopmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.3
+Version: 1.4
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

