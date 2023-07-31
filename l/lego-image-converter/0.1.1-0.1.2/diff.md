# Comparing `tmp/lego_image_converter-0.1.1.tar.gz` & `tmp/lego_image_converter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lego_image_converter-0.1.1.tar", last modified: Mon Jul 31 03:05:54 2023, max compression
+gzip compressed data, was "lego_image_converter-0.1.2.tar", last modified: Mon Jul 31 03:11:57 2023, max compression
```

## Comparing `lego_image_converter-0.1.1.tar` & `lego_image_converter-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.028165 lego_image_converter-0.1.1/
--rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.1.1/LICENSE
--rw-r--r--   0 zequnli    (501) staff       (20)     4573 2023-07-31 03:05:54.028232 lego_image_converter-0.1.1/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)     3905 2023-07-31 02:56:50.000000 lego_image_converter-0.1.1/README.md
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.027365 lego_image_converter-0.1.1/lego_image_converter/
--rw-r--r--   0 zequnli    (501) staff       (20)    10415 2023-07-31 03:04:16.000000 lego_image_converter-0.1.1/lego_image_converter/__init__.py
--rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.1.1/lego_image_converter/config.py
--rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.1.1/lego_image_converter/utility.py
-drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:05:54.028067 lego_image_converter-0.1.1/lego_image_converter.egg-info/
--rw-r--r--   0 zequnli    (501) staff       (20)     4573 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/PKG-INFO
--rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/SOURCES.txt
--rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/dependency_links.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/requires.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 03:05:54.000000 lego_image_converter-0.1.1/lego_image_converter.egg-info/top_level.txt
--rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 03:05:54.028439 lego_image_converter-0.1.1/setup.cfg
--rw-r--r--   0 zequnli    (501) staff       (20)      996 2023-07-31 03:04:16.000000 lego_image_converter-0.1.1/setup.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:11:57.804862 lego_image_converter-0.1.2/
+-rw-r--r--   0 zequnli    (501) staff       (20)     1063 2023-07-30 23:49:22.000000 lego_image_converter-0.1.2/LICENSE
+-rw-r--r--   0 zequnli    (501) staff       (20)     4567 2023-07-31 03:11:57.804975 lego_image_converter-0.1.2/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)     3905 2023-07-31 03:10:25.000000 lego_image_converter-0.1.2/README.md
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:11:57.803978 lego_image_converter-0.1.2/lego_image_converter/
+-rw-r--r--   0 zequnli    (501) staff       (20)    10415 2023-07-31 03:04:16.000000 lego_image_converter-0.1.2/lego_image_converter/__init__.py
+-rw-r--r--   0 zequnli    (501) staff       (20)      688 2023-07-30 23:45:16.000000 lego_image_converter-0.1.2/lego_image_converter/config.py
+-rw-r--r--   0 zequnli    (501) staff       (20)     1120 2023-07-30 13:48:25.000000 lego_image_converter-0.1.2/lego_image_converter/utility.py
+drwxr-xr-x   0 zequnli    (501) staff       (20)        0 2023-07-31 03:11:57.804719 lego_image_converter-0.1.2/lego_image_converter.egg-info/
+-rw-r--r--   0 zequnli    (501) staff       (20)     4567 2023-07-31 03:11:57.000000 lego_image_converter-0.1.2/lego_image_converter.egg-info/PKG-INFO
+-rw-r--r--   0 zequnli    (501) staff       (20)      351 2023-07-31 03:11:57.000000 lego_image_converter-0.1.2/lego_image_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)        1 2023-07-31 03:11:57.000000 lego_image_converter-0.1.2/lego_image_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       49 2023-07-31 03:11:57.000000 lego_image_converter-0.1.2/lego_image_converter.egg-info/requires.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       21 2023-07-31 03:11:57.000000 lego_image_converter-0.1.2/lego_image_converter.egg-info/top_level.txt
+-rw-r--r--   0 zequnli    (501) staff       (20)       79 2023-07-31 03:11:57.805210 lego_image_converter-0.1.2/setup.cfg
+-rw-r--r--   0 zequnli    (501) staff       (20)      990 2023-07-31 03:11:01.000000 lego_image_converter-0.1.2/setup.py
```

### Comparing `lego_image_converter-0.1.1/LICENSE` & `lego_image_converter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.1/PKG-INFO` & `lego_image_converter-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lego_image_converter
-Version: 0.1.1
-Summary: First minor update after formal release
+Version: 0.1.2
+Summary: minor update after formal release
 Home-page: https://github.com/zl3311/lego_image_converter
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.2.tar.gz
 Keywords: pypi,lego_image_converter,lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -48,15 +48,15 @@
 
 Don't get me wrong: I'm still a huge fan of Lego, 
 and I hope this package can save Lego players and likely programmers as well some time prototyping their ideas.
 
 ## How to use
 Please install the package using 
 
-`pip install lego_image_converter`
+`pip install lego-image-converter`
 
 You can check out some examples on [this Colab notebook](https://colab.research.google.com/drive/17k9ckWLznP_u6kH2rp3Ibujk6voFmn-X#scrollTo=nS3hGf1_kpy4). 
 
 **Disclaimer: I do not own any right of the pictures in examples, 
 and they are not intended for profit either. If you're the owner of the pictures
 and would like me to remove it, feel free to reach out, and I'm happy to remove it for you.**
```

### Comparing `lego_image_converter-0.1.1/README.md` & `lego_image_converter-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 Don't get me wrong: I'm still a huge fan of Lego, 
 and I hope this package can save Lego players and likely programmers as well some time prototyping their ideas.
 
 ## How to use
 Please install the package using 
 
-`pip install lego_image_converter`
+`pip install lego-image-converter`
 
 You can check out some examples on [this Colab notebook](https://colab.research.google.com/drive/17k9ckWLznP_u6kH2rp3Ibujk6voFmn-X#scrollTo=nS3hGf1_kpy4). 
 
 **Disclaimer: I do not own any right of the pictures in examples, 
 and they are not intended for profit either. If you're the owner of the pictures
 and would like me to remove it, feel free to reach out, and I'm happy to remove it for you.**
```

### Comparing `lego_image_converter-0.1.1/lego_image_converter/__init__.py` & `lego_image_converter-0.1.2/lego_image_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.1/lego_image_converter/config.py` & `lego_image_converter-0.1.2/lego_image_converter/config.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.1/lego_image_converter/utility.py` & `lego_image_converter-0.1.2/lego_image_converter/utility.py`

 * *Files identical despite different names*

### Comparing `lego_image_converter-0.1.1/lego_image_converter.egg-info/PKG-INFO` & `lego_image_converter-0.1.2/lego_image_converter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: lego-image-converter
-Version: 0.1.1
-Summary: First minor update after formal release
+Version: 0.1.2
+Summary: minor update after formal release
 Home-page: https://github.com/zl3311/lego_image_converter
 Author: Zequn Li
 Author-email: zequn1992@gmail.com
 License: MIT
-Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz
+Download-URL: https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.2.tar.gz
 Keywords: pypi,lego_image_converter,lego,image,8bit,art
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -48,15 +48,15 @@
 
 Don't get me wrong: I'm still a huge fan of Lego, 
 and I hope this package can save Lego players and likely programmers as well some time prototyping their ideas.
 
 ## How to use
 Please install the package using 
 
-`pip install lego_image_converter`
+`pip install lego-image-converter`
 
 You can check out some examples on [this Colab notebook](https://colab.research.google.com/drive/17k9ckWLznP_u6kH2rp3Ibujk6voFmn-X#scrollTo=nS3hGf1_kpy4). 
 
 **Disclaimer: I do not own any right of the pictures in examples, 
 and they are not intended for profit either. If you're the owner of the pictures
 and would like me to remove it, feel free to reach out, and I'm happy to remove it for you.**
```

### Comparing `lego_image_converter-0.1.1/setup.py` & `lego_image_converter-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='lego_image_converter',
     packages=['lego_image_converter'],
-    version='0.1.1',
+    version='0.1.2',
     license='MIT',
-    description='First minor update after formal release',
+    description='minor update after formal release',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Zequn Li',
     author_email='zequn1992@gmail.com',
     url='https://github.com/zl3311/lego_image_converter',
     install_requires=['requests', 'numpy', 'matplotlib', 'pillow', 'basic_colormath'],
     keywords=["pypi", "lego_image_converter", "lego", "image", "8bit", "art"],
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Documentation',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
 
-    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.1.tar.gz",
+    download_url="https://github.com/zl3311/lego_image_converter/archive/refs/tags/0.1.2.tar.gz",
 )
```

