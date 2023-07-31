# Comparing `tmp/pyxk-0.6.5.tar.gz` & `tmp/pyxk-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxk-0.6.5.tar", last modified: Mon Jul 31 13:21:47 2023, max compression
+gzip compressed data, was "pyxk-0.6.6.tar", last modified: Mon Jul 31 13:28:01 2023, max compression
```

## Comparing `pyxk-0.6.5.tar` & `pyxk-0.6.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/
--rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.5/LICENSE
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:21:47.579178 pyxk-0.6.5/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.5/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/
--rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.5/pyxk/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/aclient/
--rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.5/pyxk/aclient/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    22508 2023-07-31 13:16:20.000000 pyxk-0.6.5/pyxk/aclient/client.py
--rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.5/pyxk/aclient/typedef.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk/aes/
--rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.5/pyxk/aes/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.5/pyxk/aes/cryptor.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/pyxk/m3u8/
--rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.5/pyxk/m3u8/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 12:53:28.000000 pyxk-0.6.5/pyxk/m3u8/_initial.py
--rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.5/pyxk/m3u8/downloader.py
--rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.5/pyxk/m3u8/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    10222 2023-07-31 13:12:02.000000 pyxk-0.6.5/pyxk/m3u8/m3u8parse.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.579178 pyxk-0.6.5/pyxk/requests/
--rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.5/pyxk/requests/__init__.py
--rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.5/pyxk/requests/api.py
--rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.5/pyxk/requests/entry_point.py
--rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.5/pyxk/requests/sessions.py
--rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.5/pyxk/utils.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:21:47.569178 pyxk-0.6.5/pyxk.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/requires.txt
--rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 13:21:47.000000 pyxk-0.6.5/pyxk.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 13:21:47.579178 pyxk-0.6.5/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 13:17:30.000000 pyxk-0.6.5/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/
+-rw-rw----   0 root         (0) everybody  (9997)     1079 2022-09-01 11:31:04.000000 pyxk-0.6.6/LICENSE
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:28:01.349178 pyxk-0.6.6/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1572 2023-07-31 13:21:29.000000 pyxk-0.6.6/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.339178 pyxk-0.6.6/pyxk/
+-rw-rw----   0 root         (0) everybody  (9997)       83 2023-07-31 13:15:26.000000 pyxk-0.6.6/pyxk/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/pyxk/aclient/
+-rw-rw----   0 root         (0) everybody  (9997)       49 2023-06-25 07:46:45.000000 pyxk-0.6.6/pyxk/aclient/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    22508 2023-07-31 13:16:20.000000 pyxk-0.6.6/pyxk/aclient/client.py
+-rw-rw----   0 root         (0) everybody  (9997)      595 2023-06-18 07:54:56.000000 pyxk-0.6.6/pyxk/aclient/typedef.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/pyxk/aes/
+-rw-rw----   0 root         (0) everybody  (9997)       61 2023-07-31 07:29:51.000000 pyxk-0.6.6/pyxk/aes/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     6318 2023-07-31 07:35:43.000000 pyxk-0.6.6/pyxk/aes/cryptor.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/pyxk/m3u8/
+-rw-rw----   0 root         (0) everybody  (9997)       67 2023-07-31 12:44:14.000000 pyxk-0.6.6/pyxk/m3u8/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     8840 2023-07-31 12:53:28.000000 pyxk-0.6.6/pyxk/m3u8/_initial.py
+-rw-rw----   0 root         (0) everybody  (9997)     4286 2023-07-31 13:09:27.000000 pyxk-0.6.6/pyxk/m3u8/downloader.py
+-rw-rw----   0 root         (0) everybody  (9997)     3296 2023-07-31 13:03:20.000000 pyxk-0.6.6/pyxk/m3u8/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    10222 2023-07-31 13:12:02.000000 pyxk-0.6.6/pyxk/m3u8/m3u8parse.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/pyxk/requests/
+-rw-rw----   0 root         (0) everybody  (9997)      248 2023-07-31 13:15:53.000000 pyxk-0.6.6/pyxk/requests/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)    20692 2023-07-11 16:32:20.000000 pyxk-0.6.6/pyxk/requests/api.py
+-rw-rw----   0 root         (0) everybody  (9997)     3770 2023-07-12 02:16:53.000000 pyxk-0.6.6/pyxk/requests/entry_point.py
+-rw-rw----   0 root         (0) everybody  (9997)    36177 2023-07-31 07:11:09.000000 pyxk-0.6.6/pyxk/requests/sessions.py
+-rw-rw----   0 root         (0) everybody  (9997)    20391 2023-07-31 13:15:42.000000 pyxk-0.6.6/pyxk/utils.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-07-31 13:28:01.349178 pyxk-0.6.6/pyxk.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1924 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      558 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       89 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       62 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)        5 2023-07-31 13:28:01.000000 pyxk-0.6.6/pyxk.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-07-31 13:28:01.349178 pyxk-0.6.6/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      898 2023-07-31 13:27:09.000000 pyxk-0.6.6/setup.py
```

### Comparing `pyxk-0.6.5/LICENSE` & `pyxk-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/PKG-INFO` & `pyxk-0.6.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.5
+Version: 0.6.6
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.5/README.md` & `pyxk-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/aclient/client.py` & `pyxk-0.6.6/pyxk/aclient/client.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/aclient/typedef.py` & `pyxk-0.6.6/pyxk/aclient/typedef.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/aes/cryptor.py` & `pyxk-0.6.6/pyxk/aes/cryptor.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/m3u8/_initial.py` & `pyxk-0.6.6/pyxk/m3u8/_initial.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/m3u8/downloader.py` & `pyxk-0.6.6/pyxk/m3u8/downloader.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/m3u8/entry_point.py` & `pyxk-0.6.6/pyxk/m3u8/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/m3u8/m3u8parse.py` & `pyxk-0.6.6/pyxk/m3u8/m3u8parse.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/requests/api.py` & `pyxk-0.6.6/pyxk/requests/api.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/requests/entry_point.py` & `pyxk-0.6.6/pyxk/requests/entry_point.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/requests/sessions.py` & `pyxk-0.6.6/pyxk/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk/utils.py` & `pyxk-0.6.6/pyxk/utils.py`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/pyxk.egg-info/PKG-INFO` & `pyxk-0.6.6/pyxk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxk
-Version: 0.6.5
+Version: 0.6.6
 Summary: pyxk
 Home-page: 
 Author: kai139
 Author-email: 925330867@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxk-0.6.5/pyxk.egg-info/SOURCES.txt` & `pyxk-0.6.6/pyxk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyxk-0.6.5/setup.py` & `pyxk-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 
 with open('README.md', 'r', encoding='utf-8') as read_file_obj:
     long_description = read_file_obj.read()
 
 setuptools.setup(
     name='pyxk',
-    version='0.6.5',
+    version='0.6.6',
     author='kai139',
     install_requires=[
         'requests', 'pycryptodome', 'rich', 'm3u8', 'aiohttp', 'aiofiles', 'click', 'parsel'
     ],
     entry_points={
         'console_scripts': [
-            'm3u8 = pyxk.m3u8.enter_point:main',
+            'm3u8 = pyxk.m3u8.entry_point:main',
             'req = pyxk.requests.entry_point:main'
         ],
     },
     author_email='925330867@qq.com',
     description='pyxk',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

