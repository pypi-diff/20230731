# Comparing `tmp/VideoEmotionRecognition-0.2.1.tar.gz` & `tmp/VideoEmotionRecognition-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VideoEmotionRecognition-0.2.1.tar", last modified: Sat Jul  8 16:56:45 2023, max compression
+gzip compressed data, was "VideoEmotionRecognition-0.2.6.tar", last modified: Mon Jul 31 16:29:57 2023, max compression
```

## Comparing `VideoEmotionRecognition-0.2.1.tar` & `VideoEmotionRecognition-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/
--rw-r--r--   0 art       (1000) art       (1000)     1081 2023-06-26 12:27:40.000000 VideoEmotionRecognition-0.2.1/LICENSE
--rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)     1077 2023-06-25 22:04:56.000000 VideoEmotionRecognition-0.2.1/README.md
--rw-r--r--   0 art       (1000) art       (1000)      749 2023-07-08 16:56:21.000000 VideoEmotionRecognition-0.2.1/pyproject.toml
--rw-r--r--   0 art       (1000) art       (1000)       38 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/setup.cfg
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/
--rw-r--r--   0 art       (1000) art       (1000)       42 2023-07-08 13:23:30.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/__init__.py
--rw-r--r--   0 art       (1000) art       (1000)     7989 2023-07-08 16:53:34.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition/viemr.py
-drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-08 16:56:45.908448 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/
--rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/PKG-INFO
--rw-r--r--   0 art       (1000) art       (1000)      313 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/SOURCES.txt
--rw-r--r--   0 art       (1000) art       (1000)        1 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/dependency_links.txt
--rw-r--r--   0 art       (1000) art       (1000)       24 2023-07-08 16:56:45.000000 VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/top_level.txt
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/
+-rw-r--r--   0 art       (1000) art       (1000)     1081 2023-06-26 12:27:40.000000 VideoEmotionRecognition-0.2.6/LICENSE
+-rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)     1077 2023-06-25 22:04:56.000000 VideoEmotionRecognition-0.2.6/README.md
+-rw-r--r--   0 art       (1000) art       (1000)      749 2023-07-31 16:29:47.000000 VideoEmotionRecognition-0.2.6/pyproject.toml
+-rw-r--r--   0 art       (1000) art       (1000)       38 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/setup.cfg
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/src/
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition/
+-rw-r--r--   0 art       (1000) art       (1000)       42 2023-07-08 13:23:30.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition/__init__.py
+-rw-r--r--   0 art       (1000) art       (1000)    11411 2023-07-31 16:19:02.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition/viemr.py
+drwxr-xr-x   0 art       (1000) art       (1000)        0 2023-07-31 16:29:57.097240 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/
+-rw-r--r--   0 art       (1000) art       (1000)     1754 2023-07-31 16:29:57.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/PKG-INFO
+-rw-r--r--   0 art       (1000) art       (1000)      313 2023-07-31 16:29:57.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/SOURCES.txt
+-rw-r--r--   0 art       (1000) art       (1000)        1 2023-07-31 16:29:57.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/dependency_links.txt
+-rw-r--r--   0 art       (1000) art       (1000)       24 2023-07-31 16:29:57.000000 VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/top_level.txt
```

### Comparing `VideoEmotionRecognition-0.2.1/LICENSE` & `VideoEmotionRecognition-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `VideoEmotionRecognition-0.2.1/PKG-INFO` & `VideoEmotionRecognition-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoEmotionRecognition
-Version: 0.2.1
+Version: 0.2.6
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Deflyer/Multimodal-Emotion-Recognition-from-Videos
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `VideoEmotionRecognition-0.2.1/README.md` & `VideoEmotionRecognition-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `VideoEmotionRecognition-0.2.1/pyproject.toml` & `VideoEmotionRecognition-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "VideoEmotionRecognition"
-version = "0.2.1"
+version = "0.2.6"
 authors = [
   { name="Artur Lima", email="vligmart@gmail.com" },
 ]
 description = "This package receives an mp4 file classfying it according to its emotions and generating a heat map"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `VideoEmotionRecognition-0.2.1/src/VideoEmotionRecognition.egg-info/PKG-INFO` & `VideoEmotionRecognition-0.2.6/src/VideoEmotionRecognition.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VideoEmotionRecognition
-Version: 0.2.1
+Version: 0.2.6
 Summary: This package receives an mp4 file classfying it according to its emotions and generating a heat map
 Author-email: Artur Lima <vligmart@gmail.com>
 Project-URL: Homepage, https://github.com/Deflyer/Multimodal-Emotion-Recognition-from-Videos
 Project-URL: Example, https://colab.research.google.com/drive/1UqzA6bDgtZWGji652a0UjT7ZtDh3Xyi5?authuser=1#scrollTo=CKL-Mm9D18BB
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

