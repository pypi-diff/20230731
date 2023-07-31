# Comparing `tmp/yopmail-1.0.tar.gz` & `tmp/yopmail-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yopmail-1.0.tar", last modified: Mon Jul 31 16:21:49 2023, max compression
+gzip compressed data, was "yopmail-1.1.tar", last modified: Mon Jul 31 16:30:22 2023, max compression
```

## Comparing `yopmail-1.0.tar` & `yopmail-1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.737014 yopmail-1.0/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:21:49.736850 yopmail-1.0/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.0/README.md
--rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.0/pyproject.toml
--rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:21:49.737057 yopmail-1.0/setup.cfg
--rw-r--r--   0 rayhan     (503) staff       (20)      775 2023-07-31 16:21:20.000000 yopmail-1.0/setup.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.734866 yopmail-1.0/src/
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.735555 yopmail-1.0/src/yopmail/
--rw-r--r--   0 rayhan     (503) staff       (20)        0 2023-07-31 15:35:14.000000 yopmail-1.0/src/yopmail/__init__.py
--rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.0/src/yopmail/yopmail.py
-drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:21:49.736639 yopmail-1.0/src/yopmail.egg-info/
--rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/PKG-INFO
--rw-r--r--   0 rayhan     (503) staff       (20)      254 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/SOURCES.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/dependency_links.txt
--rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/requires.txt
--rw-r--r--   0 rayhan     (503) staff       (20)        8 2023-07-31 16:21:49.000000 yopmail-1.0/src/yopmail.egg-info/top_level.txt
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.623103 yopmail-1.1/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:30:22.622943 yopmail-1.1/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)     1274 2023-07-31 15:31:54.000000 yopmail-1.1/README.md
+-rw-r--r--   0 rayhan     (503) staff       (20)       84 2023-07-31 16:18:35.000000 yopmail-1.1/pyproject.toml
+-rw-r--r--   0 rayhan     (503) staff       (20)       38 2023-07-31 16:30:22.623159 yopmail-1.1/setup.cfg
+-rw-r--r--   0 rayhan     (503) staff       (20)      736 2023-07-31 16:29:51.000000 yopmail-1.1/setup.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.621738 yopmail-1.1/src/
+-rw-r--r--   0 rayhan     (503) staff       (20)        0 2023-07-31 15:35:14.000000 yopmail-1.1/src/__init__.py
+-rw-r--r--   0 rayhan     (503) staff       (20)     5574 2023-07-31 15:31:54.000000 yopmail-1.1/src/yopmail.py
+drwxr-xr-x   0 rayhan     (503) staff       (20)        0 2023-07-31 16:30:22.622715 yopmail-1.1/yopmail.egg-info/
+-rw-r--r--   0 rayhan     (503) staff       (20)     1576 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/PKG-INFO
+-rw-r--r--   0 rayhan     (503) staff       (20)      218 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/SOURCES.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        1 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/dependency_links.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)       24 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/requires.txt
+-rw-r--r--   0 rayhan     (503) staff       (20)        4 2023-07-31 16:30:22.000000 yopmail-1.1/yopmail.egg-info/top_level.txt
```

### Comparing `yopmail-1.0/PKG-INFO` & `yopmail-1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.0
+Version: 1.1
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `yopmail-1.0/README.md` & `yopmail-1.1/README.md`

 * *Files identical despite different names*

### Comparing `yopmail-1.0/setup.py` & `yopmail-1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yopmail',
-    version='1.0',
+    version='1.1',
     description="A Python module to get mails from a Yopmail inbox, save them",
     long_description=long_description,
     long_description_content_type='text/markdown',
     readme = "README.md",
     license='MIT',
     author="rklf",
-    package_dir={"":"src"},
-    packages = find_packages(where="src"),
+    packages = find_packages(),
     python_requires='>=3.8',
     url='https://github.com/rklf/yopmail',
     keywords='yopmail get mails retrieve scrap emails',
     install_requires=[
           'beautifulsoup4',
           'requests',
       ],
```

### Comparing `yopmail-1.0/src/yopmail/yopmail.py` & `yopmail-1.1/src/yopmail.py`

 * *Files identical despite different names*

### Comparing `yopmail-1.0/src/yopmail.egg-info/PKG-INFO` & `yopmail-1.1/yopmail.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yopmail
-Version: 1.0
+Version: 1.1
 Summary: A Python module to get mails from a Yopmail inbox, save them
 Home-page: https://github.com/rklf/yopmail
 Author: rklf
 License: MIT
 Keywords: yopmail get mails retrieve scrap emails
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

