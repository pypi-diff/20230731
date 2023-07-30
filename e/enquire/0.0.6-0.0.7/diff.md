# Comparing `tmp/enquire-0.0.6.tar.gz` & `tmp/enquire-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enquire-0.0.6.tar", last modified: Sun Jul 30 22:13:59 2023, max compression
+gzip compressed data, was "enquire-0.0.7.tar", last modified: Sun Jul 30 22:20:14 2023, max compression
```

## Comparing `enquire-0.0.6.tar` & `enquire-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-30 22:13:58.999915 enquire-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-30 22:13:47.000000 enquire-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire/question/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/style.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 22:13:47.000000 enquire-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:13:58.999915 enquire-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:13:47.000000 enquire-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-30 22:20:14.155850 enquire-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-30 22:20:02.000000 enquire-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire/question/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/question/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-30 22:20:02.000000 enquire-0.0.7/enquire/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:20:14.155850 enquire-0.0.7/enquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 22:20:14.000000 enquire-0.0.7/enquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 22:20:02.000000 enquire-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:20:14.155850 enquire-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:20:02.000000 enquire-0.0.7/setup.py
```

### Comparing `enquire-0.0.6/PKG-INFO` & `enquire-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: enquire
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyInquirer-inspired prompt library
 Author-email: Pavel Vorobyev <viert.ru@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/viert/enquire
 Keywords: click,PyInquirer,prompt-toolkit,cli,command-line,commandline,command-line-interface,python-inquiry,inquirer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## enquire
 
 ### Goal
 
-**Enquire** is a pet-project with no ambitions. However, a bit of a history my shed some light on the project goals.
+**Enquire** is a pet project with no ambitions. However, a bit of history might shed some light on the project goals.
 
-> _It was a cold April morning and the dew on the grass was frozen like tiny piece of glass._
+> _It was a cold April morning and the dew on the grass was frozen like a tiny piece of glass._
 > 
 > _Eric Cartman_
 
 I needed a modern cli prompt library to add some interactivity to my working projects.
 [PyInquirer](https://github.com/CITGuru/PyInquirer) turned out to be the most easy-to-use 
 and convenient among all the libs I could find.
```

### Comparing `enquire-0.0.6/README.md` & `enquire-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## enquire
 
 ### Goal
 
-**Enquire** is a pet-project with no ambitions. However, a bit of a history my shed some light on the project goals.
+**Enquire** is a pet project with no ambitions. However, a bit of history might shed some light on the project goals.
 
-> _It was a cold April morning and the dew on the grass was frozen like tiny piece of glass._
+> _It was a cold April morning and the dew on the grass was frozen like a tiny piece of glass._
 > 
 > _Eric Cartman_
 
 I needed a modern cli prompt library to add some interactivity to my working projects.
 [PyInquirer](https://github.com/CITGuru/PyInquirer) turned out to be the most easy-to-use 
 and convenient among all the libs I could find.
 
@@ -16,8 +16,8 @@
 the default value for `list` prompts. The GitHub version does not have that bug, however, it seems to be
 abandoned for quite some years.
 
 Since I only needed the basic, the radio button, and the checkbox types, these were implemented first.
 
 ---
 
-_This documentation is a work in progress, check out the examples folder to get some usage tips_
+_This documentation is a work in progress, check out the examples folder to get some usage tips_
```

### Comparing `enquire-0.0.6/enquire/prompt.py` & `enquire-0.0.7/enquire/prompt.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.6/enquire/question/base.py` & `enquire-0.0.7/enquire/question/base.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.6/enquire/question/checkbox.py` & `enquire-0.0.7/enquire/question/checkbox.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.6/enquire/question/radio.py` & `enquire-0.0.7/enquire/question/radio.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.6/enquire/question/text.py` & `enquire-0.0.7/enquire/question/text.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.6/enquire.egg-info/PKG-INFO` & `enquire-0.0.7/enquire.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: enquire
-Version: 0.0.6
+Version: 0.0.7
 Summary: PyInquirer-inspired prompt library
 Author-email: Pavel Vorobyev <viert.ru@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/viert/enquire
 Keywords: click,PyInquirer,prompt-toolkit,cli,command-line,commandline,command-line-interface,python-inquiry,inquirer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ## enquire
 
 ### Goal
 
-**Enquire** is a pet-project with no ambitions. However, a bit of a history my shed some light on the project goals.
+**Enquire** is a pet project with no ambitions. However, a bit of history might shed some light on the project goals.
 
-> _It was a cold April morning and the dew on the grass was frozen like tiny piece of glass._
+> _It was a cold April morning and the dew on the grass was frozen like a tiny piece of glass._
 > 
 > _Eric Cartman_
 
 I needed a modern cli prompt library to add some interactivity to my working projects.
 [PyInquirer](https://github.com/CITGuru/PyInquirer) turned out to be the most easy-to-use 
 and convenient among all the libs I could find.
```

### Comparing `enquire-0.0.6/pyproject.toml` & `enquire-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "enquire"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{name = "Pavel Vorobyev", email = "viert.ru@gmail.com"}]
 description = "PyInquirer-inspired prompt library"
 requires-python = ">=3.10"
 keywords = [
     "click",
     "PyInquirer",
     "prompt-toolkit",
```

