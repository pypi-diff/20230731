# Comparing `tmp/yopmail-1.1.tar.gz` & `tmp/yopmail-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-1.1.tar", last modified: Mon Jul 31 16:30:22 2023, max compression
+gzip compressed data, was "yopmail-1.2.tar", last modified: Mon Jul 31 16:36:43 2023, max compression
```

## Comparing `yopmail-1.1.tar` & `yopmail-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.623103 yopmail-1.1/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:30:22.622943 yopmail-1.1/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.1/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.1/pyproject.toml
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:30:22.623159 yopmail-1.1/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:29:51.000000 yopmail-1.1/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.621738 yopmail-1.1/src/
--rw-r--r--   0 rayhan     (503) staff       (20)        0 2023-07-31 15:35:14.000000 yopmail-1.1/src/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.1/src/yopmail.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.622715 yopmail-1.1/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      218 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        4 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:36:43.673353 yopmail-1.2/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:36:43.673189 yopmail-1.2/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.2/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.2/pyproject.toml
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:36:43.673388 yopmail-1.2/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:36:29.000000 yopmail-1.2/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:36:43.672157 yopmail-1.2/yopmail/
+-rw-r--r--   0 rayhan     (503) staff       (20)        0 2023-07-31 15:35:14.000000 yopmail-1.2/yopmail/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.2/yopmail/yopmail.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:36:43.672991 yopmail-1.2/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:36:43.000000 yopmail-1.2/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      226 2023-07-31 16:36:43.000000 yopmail-1.2/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:36:43.000000 yopmail-1.2/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:36:43.000000 yopmail-1.2/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:36:43.000000 yopmail-1.2/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-1.1/PKG-INFO` & `yopmail-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.1
+Version: 1.2
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `yopmail-1.1/README.md` & `yopmail-1.2/README.md`

 * *Files identical despite different names*

### Comparing `yopmail-1.1/setup.py` & `yopmail-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='1.1',
+    version='1.2',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
     packages = find_packages(),
```

### Comparing `yopmail-1.1/src/yopmail.py` & `yopmail-1.2/yopmail/yopmail.py`

 * *Files identical despite different names*

### Comparing `yopmail-1.1/yopmail.egg-info/PKG-INFO` & `yopmail-1.2/yopmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.1
+Version: 1.2
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

