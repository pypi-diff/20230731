# Comparing `tmp/enquire-0.0.7.tar.gz` & `tmp/enquire-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enquire-0.0.7.tar", last modified: Sun Jul 30 22:20:14 2023, max compression
+gzip compressed data, was "enquire-0.0.8.tar", last modified: Mon Jul 31 08:35:46 2023, max compression
```

## Comparing `enquire-0.0.7.tar` & `enquire-0.0.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-30 22:20:14.155850 enquire-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-30 22:20:02.000000 enquire-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire/question/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 22:20:02.000000 enquire-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:20:14.155850 enquire-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:20:02.000000 enquire-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:35:46.370883 enquire-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 08:35:46.370883 enquire-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-31 08:35:19.000000 enquire-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:35:46.370883 enquire-0.0.8/enquire/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:35:46.370883 enquire-0.0.8/enquire/question/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/question/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/question/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/question/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/question/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/question/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-31 08:35:19.000000 enquire-0.0.8/enquire/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:35:46.370883 enquire-0.0.8/enquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-31 08:35:46.000000 enquire-0.0.8/enquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-31 08:35:46.000000 enquire-0.0.8/enquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:35:46.000000 enquire-0.0.8/enquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 08:35:46.000000 enquire-0.0.8/enquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 08:35:46.000000 enquire-0.0.8/enquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-31 08:35:19.000000 enquire-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:35:46.370883 enquire-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:35:19.000000 enquire-0.0.8/setup.py
```

### Comparing `enquire-0.0.7/PKG-INFO` & `enquire-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enquire
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyInquirer-inspired prompt library
 Author-email: Pavel Vorobyev <viert.ru@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/viert/enquire
 Keywords: click,PyInquirer,prompt-toolkit,cli,command-line,commandline,command-line-interface,python-inquiry,inquirer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `enquire-0.0.7/README.md` & `enquire-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire/prompt.py` & `enquire-0.0.8/enquire/prompt.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire/question/base.py` & `enquire-0.0.8/enquire/question/base.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire/question/checkbox.py` & `enquire-0.0.8/enquire/question/checkbox.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire/question/radio.py` & `enquire-0.0.8/enquire/question/radio.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire/question/text.py` & `enquire-0.0.8/enquire/question/text.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.7/enquire.egg-info/PKG-INFO` & `enquire-0.0.8/enquire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enquire
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyInquirer-inspired prompt library
 Author-email: Pavel Vorobyev <viert.ru@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/viert/enquire
 Keywords: click,PyInquirer,prompt-toolkit,cli,command-line,commandline,command-line-interface,python-inquiry,inquirer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

### Comparing `enquire-0.0.7/pyproject.toml` & `enquire-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "enquire"
-version = "0.0.7"
+version = "0.0.8"
 authors = [{name = "Pavel Vorobyev", email = "viert.ru@gmail.com"}]
 description = "PyInquirer-inspired prompt library"
 requires-python = ">=3.10"
 keywords = [
     "click",
     "PyInquirer",
     "prompt-toolkit",
@@ -20,13 +20,13 @@
     "inquirer"
 ]
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "python_toolkit",
+    "prompt_toolkit",
 ]
 readme = "README.md"
 
 [project.urls]
 repository = "https://github.com/viert/enquire"
```

