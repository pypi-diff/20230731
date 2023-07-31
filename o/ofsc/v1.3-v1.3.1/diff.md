# Comparing `tmp/ofsc-v1.3.tar.gz` & `tmp/ofsc-v1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ofsc-v1.3.tar", last modified: Wed Oct 23 15:50:33 2019, max compression
+gzip compressed data, was "dist/ofsc-v1.3.1.tar", last modified: Wed Oct 23 16:47:59 2019, max compression
```

## Comparing `ofsc-v1.3.tar` & `ofsc-v1.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 borja      (501) staff       (20)        0 2019-10-23 15:50:33.000000 ofsc-v1.3/
--rw-r--r--   0 borja      (501) staff       (20)      817 2019-10-23 15:50:33.000000 ofsc-v1.3/PKG-INFO
-drwxr-xr-x   0 borja      (501) staff       (20)        0 2019-10-23 15:50:33.000000 ofsc-v1.3/ofsc/
--rw-r--r--   0 borja      (501) staff       (20)        0 2019-10-23 15:50:26.000000 ofsc-v1.3/ofsc/__init__.py
--rw-r--r--   0 borja      (501) staff       (20)     2224 2019-10-22 22:27:33.000000 ofsc-v1.3/ofsc/core.py
--rw-r--r--   0 borja      (501) staff       (20)       62 2019-10-23 15:47:11.000000 ofsc-v1.3/setup.cfg
--rw-r--r--   0 borja      (501) staff       (20)     1707 2019-10-23 15:49:40.000000 ofsc-v1.3/setup.py
+drwxr-xr-x   0 borja      (501) staff       (20)        0 2019-10-23 16:47:59.000000 ofsc-v1.3.1/
+-rw-r--r--   0 borja      (501) staff       (20)      821 2019-10-23 16:47:59.000000 ofsc-v1.3.1/PKG-INFO
+drwxr-xr-x   0 borja      (501) staff       (20)        0 2019-10-23 16:47:59.000000 ofsc-v1.3.1/ofsc/
+-rw-r--r--   0 borja      (501) staff       (20)        0 2019-10-23 15:50:26.000000 ofsc-v1.3.1/ofsc/__init__.py
+-rw-r--r--   0 borja      (501) staff       (20)     2224 2019-10-22 22:27:33.000000 ofsc-v1.3.1/ofsc/core.py
+-rw-r--r--   0 borja      (501) staff       (20)     1691 2019-10-23 16:47:48.000000 ofsc-v1.3.1/setup.py
+-rw-r--r--   0 borja      (501) staff       (20)       62 2019-10-23 15:47:11.000000 ofsc-v1.3.1/setup.cfg
```

### Comparing `ofsc-v1.3/PKG-INFO` & `ofsc-v1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: ofsc
-Version: v1.3
+Version: v1.3.1
 Summary: Python Wrapper for Oracle Field Service Cloud API
 Home-page: https://github.com/btoron/pyOFSC
 Author: Borja Toron
 Author-email: borja.toron@gmail.com
 License: MIT
-Download-URL: https://github.com/btoron/pyOFSC/archive/v1.3.tar.gz
+Download-URL: https://github.com/btoron/pyOFSC/archive/v1.3.1.tar.gz
 Description: UNKNOWN
 Keywords: OFSC,Python,ORACLE FIELD SERVICE CLOUD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ofsc-v1.3/ofsc/core.py` & `ofsc-v1.3.1/ofsc/core.py`

 * *Files identical despite different names*

### Comparing `ofsc-v1.3/setup.py` & `ofsc-v1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'ofsc',         # How you named your package folder (MyLib)
   packages = ['ofsc'],   # Chose the same as "name"
-  version = 'v1.3',      # Start with a small number and increase it with every change you make
+  version = 'v1.3.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Python Wrapper for Oracle Field Service Cloud API',   # Give a short description about your library
   author = 'Borja Toron',                   # Type in your name
   author_email = 'borja.toron@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/btoron/pyOFSC',   # Provide either the link to your github or to your website
-  download_url = 'https://github.com/btoron/pyOFSC/archive/v1.3.tar.gz',    # I explain this later on
+  download_url = 'https://github.com/btoron/pyOFSC/archive/v1.3.1.tar.gz',    # I explain this later on
   keywords = ['OFSC', 'Python', 'ORACLE FIELD SERVICE CLOUD'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests',
-          'base64',
       ],
   classifiers=[
     'Development Status :: 4 - Beta',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

