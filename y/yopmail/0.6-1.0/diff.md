# Comparing `tmp/yopmail-0.6.tar.gz` & `tmp/yopmail-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-0.6.tar", last modified: Mon Jul 31 15:46:10 2023, max compression
+gzip compressed data, was "yopmail-1.0.tar", last modified: Mon Jul 31 16:21:49 2023, max compression
```

## Comparing `yopmail-0.6.tar` & `yopmail-1.0.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.713805 yopmail-0.6/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 15:46:10.713865 yopmail-0.6/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-0.6/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)      125 2023-07-31 15:46:10.714061 yopmail-0.6/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      767 2023-07-31 15:44:20.000000 yopmail-0.6/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.712571 yopmail-0.6/src/
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 15:46:10.713698 yopmail-0.6/src/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      202 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       13 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 15:46:10.000000 yopmail-0.6/src/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.737014 yopmail-1.0/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:21:49.736850 yopmail-1.0/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.0/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.0/pyproject.toml
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:21:49.737057 yopmail-1.0/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      775 2023-07-31 16:21:20.000000 yopmail-1.0/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.734866 yopmail-1.0/src/
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.735555 yopmail-1.0/src/yopmail/
+-rw-r--r--   0 rayhan     (503) staff       (20)        0 2023-07-31 15:35:14.000000 yopmail-1.0/src/yopmail/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.0/src/yopmail/yopmail.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.736639 yopmail-1.0/src/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      254 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-0.6/PKG-INFO` & `yopmail-1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 0.6
+Version: 1.0
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `yopmail-0.6/README.md` & `yopmail-1.0/README.md`

 * *Files identical despite different names*

### Comparing `yopmail-0.6/setup.py` & `yopmail-1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='0.6',
+    version='1.0',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
-    package_dir = {"": "src"},
+    package_dir={"":"src"},
     packages = find_packages(where="src"),
     python_requires='>=3.8',
     url='https://github.com/rklf/yopmail',
     keywords='yopmail get mails retrieve scrap emails',
     install_requires=[
-          'bs4',
+          'beautifulsoup4',
           'requests',
       ],
 
 )
```

### Comparing `yopmail-0.6/src/yopmail.egg-info/PKG-INFO` & `yopmail-1.0/src/yopmail.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 0.6
+Version: 1.0
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

