# Comparing `tmp/midify-0.3.1.tar.gz` & `tmp/midify-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midify-0.3.1.tar", last modified: Mon Jul 31 10:46:19 2023, max compression
+gzip compressed data, was "midify-0.3.2.tar", last modified: Mon Jul 31 11:46:20 2023, max compression
```

## Comparing `midify-0.3.1.tar` & `midify-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:46:19.863864 midify-0.3.1/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1132 2023-07-31 10:46:19.863864 midify-0.3.1/PKG-INFO
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:46:19.863864 midify-0.3.1/midify/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      129 2023-07-31 06:09:04.831996 midify-0.3.1/midify/__init__.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      670 2023-07-31 10:25:05.750384 midify-0.3.1/midify/find_peaks.py
--rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)     4578 2023-07-31 10:01:16.683430 midify-0.3.1/midify/midify
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1124 2023-07-31 05:55:36.224896 midify-0.3.1/midify/notes.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      132 2023-07-31 09:58:33.782135 midify-0.3.1/midify/resample.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      651 2023-07-31 10:45:34.287525 midify-0.3.1/setup.py
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 11:46:20.103369 midify-0.3.2/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1685 2023-07-31 11:46:20.103369 midify-0.3.2/PKG-INFO
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 11:46:20.103369 midify-0.3.2/midify/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      163 2023-07-31 11:02:47.971322 midify-0.3.2/midify/__init__.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      670 2023-07-31 10:25:05.750384 midify-0.3.2/midify/find_peaks.py
+-rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)     3100 2023-07-31 11:14:35.184639 midify-0.3.2/midify/midify
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     2750 2023-07-31 11:30:08.367719 midify-0.3.2/midify/midify.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1124 2023-07-31 05:55:36.224896 midify-0.3.2/midify/notes.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      132 2023-07-31 09:58:33.782135 midify-0.3.2/midify/resample.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      670 2023-07-31 11:45:41.331062 midify-0.3.2/setup.py
```

### Comparing `midify-0.3.1/midify/find_peaks.py` & `midify-0.3.2/midify/find_peaks.py`

 * *Files identical despite different names*

### Comparing `midify-0.3.1/midify/notes.py` & `midify-0.3.2/midify/notes.py`

 * *Files identical despite different names*

### Comparing `midify-0.3.1/setup.py` & `midify-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python
 
+import pypandoc
 from distutils.core import setup
 
+long_description = pypandoc.convert_file('README.md', 'rst')
+
 setup(name='midify',
-    version='0.3.1',
+    version='0.3.2',
     packages=['midify'],
     description='Command line tool for converting Audio to MIDI.',
-    long_description=open('README.md').read(),
-    long_description_content_type='text/markdown',
+    long_description=long_description,
     author='Daniel Santana',
     author_email='danielsantanarocha@gmail.com',
     url='https://github.com/DanielSanRocha/midify',
     scripts=['midify/midify'],
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha'
```

