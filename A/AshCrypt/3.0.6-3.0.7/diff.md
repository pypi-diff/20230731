# Comparing `tmp/AshCrypt-3.0.6.tar.gz` & `tmp/AshCrypt-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AshCrypt-3.0.6.tar", last modified: Mon Jul 31 17:53:15 2023, max compression
+gzip compressed data, was "dist/AshCrypt-3.0.7.tar", last modified: Mon Jul 31 18:18:28 2023, max compression
```

## Comparing `AshCrypt-3.0.6.tar` & `AshCrypt-3.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/clicrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/filecrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/textcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/AshCrypt/unittests/unittest_crypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/AshCrypt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 17:53:15.000000 AshCrypt-3.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-31 17:52:57.000000 AshCrypt-3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/clicrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/filecrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39164 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/textcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/AshCrypt/unittests/unittest_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/AshCrypt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20172 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 18:18:28.000000 AshCrypt-3.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-07-31 18:18:13.000000 AshCrypt-3.0.7/setup.py
```

### Comparing `AshCrypt-3.0.6/AshCrypt/clicrypt.py` & `AshCrypt-3.0.7/AshCrypt/clicrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/crypt.py` & `AshCrypt-3.0.7/AshCrypt/crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/database.py` & `AshCrypt-3.0.7/AshCrypt/database.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/filecrypt.py` & `AshCrypt-3.0.7/AshCrypt/filecrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/gui.py` & `AshCrypt-3.0.7/AshCrypt/gui.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/textcrypt.py` & `AshCrypt-3.0.7/AshCrypt/textcrypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt/unittests/unittest_crypt.py` & `AshCrypt-3.0.7/AshCrypt/unittests/unittest_crypt.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-3.0.7/AshCrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.6/PKG-INFO` & `AshCrypt-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 3.0.6
+Version: 3.0.7
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 License: UNKNOWN
 Description: # Cryptography App & Library For AES-256
         ## Docs ##
```

### Comparing `AshCrypt-3.0.6/README.md` & `AshCrypt-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `AshCrypt-3.0.6/setup.py` & `AshCrypt-3.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('AshCrypt/README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='3.0.6',
+    version='3.0.7',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along"
                 " with a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

