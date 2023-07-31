# Comparing `tmp/midify-0.3.0.tar.gz` & `tmp/midify-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midify-0.3.0.tar", last modified: Mon Jul 31 10:05:56 2023, max compression
+gzip compressed data, was "midify-0.3.1.tar", last modified: Mon Jul 31 10:46:19 2023, max compression
```

## Comparing `midify-0.3.0.tar` & `midify-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:05:56.637665 midify-0.3.0/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      321 2023-07-31 10:05:56.637665 midify-0.3.0/PKG-INFO
-drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:05:56.637665 midify-0.3.0/midify/
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      129 2023-07-31 06:09:04.831996 midify-0.3.0/midify/__init__.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      670 2023-07-31 09:57:52.333806 midify-0.3.0/midify/find_peaks.py
--rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)     4578 2023-07-31 10:01:16.683430 midify-0.3.0/midify/midify
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1124 2023-07-31 05:55:36.224896 midify-0.3.0/midify/notes.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      132 2023-07-31 09:58:33.782135 midify-0.3.0/midify/resample.py
--rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      553 2023-07-31 07:44:46.824421 midify-0.3.0/setup.py
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:46:19.863864 midify-0.3.1/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1132 2023-07-31 10:46:19.863864 midify-0.3.1/PKG-INFO
+drwxrwxr-x   0 danielsan  (1000) danielsan  (1000)        0 2023-07-31 10:46:19.863864 midify-0.3.1/midify/
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      129 2023-07-31 06:09:04.831996 midify-0.3.1/midify/__init__.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      670 2023-07-31 10:25:05.750384 midify-0.3.1/midify/find_peaks.py
+-rwxrwxr-x   0 danielsan  (1000) danielsan  (1000)     4578 2023-07-31 10:01:16.683430 midify-0.3.1/midify/midify
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)     1124 2023-07-31 05:55:36.224896 midify-0.3.1/midify/notes.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      132 2023-07-31 09:58:33.782135 midify-0.3.1/midify/resample.py
+-rw-rw-r--   0 danielsan  (1000) danielsan  (1000)      651 2023-07-31 10:45:34.287525 midify-0.3.1/setup.py
```

### Comparing `midify-0.3.0/midify/find_peaks.py` & `midify-0.3.1/midify/find_peaks.py`

 * *Files identical despite different names*

### Comparing `midify-0.3.0/midify/midify` & `midify-0.3.1/midify/midify`

 * *Files identical despite different names*

### Comparing `midify-0.3.0/midify/notes.py` & `midify-0.3.1/midify/notes.py`

 * *Files identical despite different names*

### Comparing `midify-0.3.0/setup.py` & `midify-0.3.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(name='midify',
-    version='0.3.0',
+    version='0.3.1',
     packages=['midify'],
     description='Command line tool for converting Audio to MIDI.',
+    long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     author='Daniel Santana',
     author_email='danielsantanarocha@gmail.com',
     url='https://github.com/DanielSanRocha/midify',
     scripts=['midify/midify'],
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha'
```

