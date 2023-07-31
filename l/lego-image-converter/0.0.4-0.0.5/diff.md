# Comparing `tmp/lego_image_converter-0.0.4.tar.gz` & `tmp/lego_image_converter-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lego_image_converter-0.0.4.tar", last modified: Mon Jul 31 01:42:34 2023, max compression
+gzip compressed data, was "lego_image_converter-0.0.5.tar", last modified: Mon Jul 31 01:43:49 2023, max compression
```

## Comparing `lego_image_converter-0.0.4.tar` & `lego_image_converter-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:42:34.793678 lego_image_converter-0.0.4/
--rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.0.4/LICENSE
--rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:42:34.793744 lego_image_converter-0.0.4/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)     1858 2023-07-31 00:48:36.000000 lego_image_converter-0.0.4/README.md
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:42:34.792995 lego_image_converter-0.0.4/lego_image_converter/
--rw-r--r--   0 zequnli    (501) staff       (20)     8936 2023-07-31 01:41:38.000000 lego_image_converter-0.0.4/lego_image_converter/__init__.py
--rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.0.4/lego_image_converter/config.py
--rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.0.4/lego_image_converter/utility.py
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:42:34.793566 lego_image_converter-0.0.4/lego_image_converter.egg-info/
--rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:42:34.000000 lego_image_converter-0.0.4/lego_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 01:42:34.000000 lego_image_converter-0.0.4/lego_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 01:42:34.000000 lego_image_converter-0.0.4/lego_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 01:42:34.000000 lego_image_converter-0.0.4/lego_image_converter.egg-info/requires.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 01:42:34.000000 lego_image_converter-0.0.4/lego_image_converter.egg-info/top_level.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 01:42:34.793947 lego_image_converter-0.0.4/setup.cfg
--rw-r--r--   0 zequnli    (501) staff       (20)     1278 2023-07-31 01:41:38.000000 lego_image_converter-0.0.4/setup.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.906211 lego_image_converter-0.0.5/
+-rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.0.5/LICENSE
+-rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:43:49.906271 lego_image_converter-0.0.5/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)     1858 2023-07-31 00:48:36.000000 lego_image_converter-0.0.5/README.md
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.905498 lego_image_converter-0.0.5/lego_image_converter/
+-rw-r--r--   0 zequnli    (501) staff       (20)     8936 2023-07-31 01:41:38.000000 lego_image_converter-0.0.5/lego_image_converter/__init__.py
+-rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.0.5/lego_image_converter/config.py
+-rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.0.5/lego_image_converter/utility.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 01:43:49.906079 lego_image_converter-0.0.5/lego_image_converter.egg-info/
+-rw-r--r--   0 zequnli    (501) staff       (20)     2517 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/requires.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 01:43:49.000000 lego_image_converter-0.0.5/lego_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 01:43:49.906488 lego_image_converter-0.0.5/setup.cfg
+-rw-r--r--   0 zequnli    (501) staff       (20)     1278 2023-07-31 01:43:35.000000 lego_image_converter-0.0.5/setup.py
```

### Comparing `lego_image_converter-0.0.4/LICENSE` & `lego_image_converter-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.4/PKG-INFO` & `lego_image_converter-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lego_image_converter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Testing installation of Package 3
 Home-page: https://github.com/mike-huls/toolbox_public
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.5.tar.gz
 Keywords: pypi,lego_image_converter,Lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `lego_image_converter-0.0.4/README.md` & `lego_image_converter-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.4/lego_image_converter/__init__.py` & `lego_image_converter-0.0.5/lego_image_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.4/lego_image_converter/config.py` & `lego_image_converter-0.0.5/lego_image_converter/config.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.4/lego_image_converter/utility.py` & `lego_image_converter-0.0.5/lego_image_converter/utility.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.0.4/lego_image_converter.egg-info/PKG-INFO` & `lego_image_converter-0.0.5/lego_image_converter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lego-image-converter
-Version: 0.0.4
+Version: 0.0.5
 Summary: Testing installation of Package 3
 Home-page: https://github.com/mike-huls/toolbox_public
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.4.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.5.tar.gz
 Keywords: pypi,lego_image_converter,Lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `lego_image_converter-0.0.4/setup.py` & `lego_image_converter-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='lego_image_converter',  # should match the package folder
     packages=['lego_image_converter'],  # should match the package folder
-    version='0.0.4',  # important for updates
+    version='0.0.5',  # important for updates
     license='MIT',  # should match your chosen license
     description='Testing installation of Package 3',
     long_description=long_description,  # loads your README.md
     long_description_content_type="text/markdown",  # README.md is of type 'markdown'
     author='Zequn Li',
     author_email='zequn1992@gmail.com',
     url='https://github.com/mike-huls/toolbox_public',
@@ -19,9 +19,9 @@
     classifiers=[  # https://pypi.org/classifiers
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.4.tar.gz",
+    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.0.5.tar.gz",
 )
```

