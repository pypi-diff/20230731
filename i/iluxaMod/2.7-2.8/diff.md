# Comparing `tmp/iluxaMod-2.7.tar.gz` & `tmp/iluxaMod-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iluxaMod-2.7.tar", last modified: Mon Jul 31 16:28:41 2023, max compression
+gzip compressed data, was "iluxaMod-2.8.tar", last modified: Mon Jul 31 16:33:33 2023, max compression
```

## Comparing `iluxaMod-2.7.tar` & `iluxaMod-2.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.225865 iluxaMod-2.7/
--rw-rw-rw-   0        0        0      876 2023-07-31 16:28:41.224864 iluxaMod-2.7/PKG-INFO
--rw-rw-rw-   0        0        0     4466 2023-07-31 16:25:53.000000 iluxaMod-2.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.208636 iluxaMod-2.7/iluxaMod/
--rw-rw-rw-   0        0        0       24 2023-07-31 16:09:15.000000 iluxaMod-2.7/iluxaMod/__init__.py
--rw-rw-rw-   0        0        0    21458 2023-07-31 16:25:53.000000 iluxaMod-2.7/iluxaMod/tools.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.222866 iluxaMod-2.7/iluxaMod.egg-info/
--rw-rw-rw-   0        0        0      876 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 16:28:41.225865 iluxaMod-2.7/setup.cfg
--rw-rw-rw-   0        0        0     1578 2023-07-31 16:28:38.000000 iluxaMod-2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.590611 iluxaMod-2.8/
+-rw-rw-rw-   0        0        0     5387 2023-07-31 16:33:33.589591 iluxaMod-2.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4466 2023-07-31 16:25:53.000000 iluxaMod-2.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.581474 iluxaMod-2.8/iluxaMod/
+-rw-rw-rw-   0        0        0       24 2023-07-31 16:09:15.000000 iluxaMod-2.8/iluxaMod/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-07-31 16:25:53.000000 iluxaMod-2.8/iluxaMod/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:33:33.588590 iluxaMod-2.8/iluxaMod.egg-info/
+-rw-rw-rw-   0        0        0     5387 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 16:33:33.000000 iluxaMod-2.8/iluxaMod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:33:33.590611 iluxaMod-2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1765 2023-07-31 16:33:29.000000 iluxaMod-2.8/setup.py
```

### Comparing `iluxaMod-2.7/README.md` & `iluxaMod-2.8/README.md`

 * *Files identical despite different names*

### Comparing `iluxaMod-2.7/iluxaMod/tools.py` & `iluxaMod-2.8/iluxaMod/tools.py`

 * *Files identical despite different names*

### Comparing `iluxaMod-2.7/setup.py` & `iluxaMod-2.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from setuptools import setup, find_packages
 
+
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = str(f.read())
+
 setup(
     name='iluxaMod',
-    version='2.7',  # Версия вашего пакета
+    version='2.8',  # Версия вашего пакета
     packages=['iluxaMod'],  # Автоматически найдет все пакеты в корневой директории
     install_requires=[  # Зависимости вашего пакета
         'geopy',
         'psycopg2-binary',
         'pyTelegramBotAPI',
         'requests',
         'pyfirmata',
@@ -17,14 +21,16 @@
         'opencv-python',
         'selenium'
 
     ],
     author='Illya Lazarev',
     author_email='lazarevillya031@gmail.com',
     description='Module for simplified work with libraries: TG, PostgreSQL, locations and more...',
+    long_description_content_type="text/markdown",
+    long_description=long_description,
     url='https://sbdt.pro',
     classifiers=[  # Классификаторы, чтобы помочь пользователям понять ваш пакет
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Intended Audience :: End Users/Desktop',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
```

