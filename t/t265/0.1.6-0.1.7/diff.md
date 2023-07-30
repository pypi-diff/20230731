# Comparing `tmp/t265-0.1.6.tar.gz` & `tmp/t265-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t265-0.1.6.tar", last modified: Sat Jul 29 06:58:48 2023, max compression
+gzip compressed data, was "t265-0.1.7.tar", last modified: Sun Jul 30 23:53:30 2023, max compression
```

## Comparing `t265-0.1.6.tar` & `t265-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 06:58:48.000561 t265-0.1.6/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       25 2023-07-18 00:54:55.000000 t265-0.1.6/MANIFEST.in
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 06:58:48.000561 t265-0.1.6/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-18 01:21:38.000000 t265-0.1.6/requirements.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       38 2023-07-29 06:58:48.000561 t265-0.1.6/setup.cfg
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     1008 2023-07-29 06:58:36.000000 t265-0.1.6/setup.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 06:58:48.000561 t265-0.1.6/t265/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)     5183 2023-07-29 06:57:49.000000 t265-0.1.6/t265/Tracking.py
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       31 2023-07-18 00:54:55.000000 t265-0.1.6/t265/__init__.py
-drwxrwxr-x   0 yusuke    (1000) yusuke    (1000)        0 2023-07-29 06:58:48.000561 t265-0.1.6/t265.egg-info/
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      549 2023-07-29 06:58:47.000000 t265-0.1.6/t265.egg-info/PKG-INFO
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)      210 2023-07-29 06:58:47.000000 t265-0.1.6/t265.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        1 2023-07-29 06:58:47.000000 t265-0.1.6/t265.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)       27 2023-07-29 06:58:47.000000 t265-0.1.6/t265.egg-info/requires.txt
--rw-rw-r--   0 yusuke    (1000) yusuke    (1000)        5 2023-07-29 06:58:47.000000 t265-0.1.6/t265.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-30 23:53:30.352349 t265-0.1.7/
+-rw-rw-rw-   0        0        0       26 2023-07-03 23:15:19.000000 t265-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      563 2023-07-30 23:53:30.352349 t265-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       29 2023-07-30 22:29:05.000000 t265-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-30 23:53:30.352349 t265-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-07-30 23:53:28.000000 t265-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-30 23:53:30.344349 t265-0.1.7/t265/
+-rw-rw-rw-   0        0        0    10093 2023-07-30 23:49:19.000000 t265-0.1.7/t265/Tracking.py
+-rw-rw-rw-   0        0        0       32 2023-07-05 01:41:09.000000 t265-0.1.7/t265/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-30 23:53:30.351349 t265-0.1.7/t265.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-07-30 23:53:30.000000 t265-0.1.7/t265.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-07-30 23:53:30.000000 t265-0.1.7/t265.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-30 23:53:30.000000 t265-0.1.7/t265.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-30 23:53:30.000000 t265-0.1.7/t265.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-30 23:53:30.000000 t265-0.1.7/t265.egg-info/top_level.txt
```

### Comparing `t265-0.1.6/PKG-INFO` & `t265-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: t265
-Version: 0.1.6
-Summary: t265 Tracking camera API wrapper
-Author: Yusuke Tanaka
-License: LGPLv3
-Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1
+Name: t265
+Version: 0.1.7
+Summary: t265 Tracking camera API wrapper
+Author: Yusuke Tanaka
+License: LGPLv3
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
```

### Comparing `t265-0.1.6/t265.egg-info/PKG-INFO` & `t265-0.1.7/t265.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
-Name: t265
-Version: 0.1.6
-Summary: t265 Tracking camera API wrapper
-Author: Yusuke Tanaka
-License: LGPLv3
-Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
-Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Robot Framework
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1
+Name: t265
+Version: 0.1.7
+Summary: t265 Tracking camera API wrapper
+Author: Yusuke Tanaka
+License: LGPLv3
+Project-URL: GitHub, https://github.com/Suke0811/Localization_T265
+Classifier: Development Status :: 4 - Beta
+Classifier: Framework :: Robot Framework
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Programming Language :: Python :: 3
```

