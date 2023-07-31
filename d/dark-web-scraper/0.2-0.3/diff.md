# Comparing `tmp/dark_web_scraper-0.2.tar.gz` & `tmp/dark_web_scraper-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dark_web_scraper-0.2.tar", last modified: Mon Jul 31 14:32:26 2023, max compression
+gzip compressed data, was "dark_web_scraper-0.3.tar", last modified: Mon Jul 31 14:36:28 2023, max compression
```

## Comparing `dark_web_scraper-0.2.tar` & `dark_web_scraper-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 14:32:26.476038 dark_web_scraper-0.2/
--rw-rw-rw-   0        0        0     1087 2023-07-30 16:23:56.000000 dark_web_scraper-0.2/LICENSE
--rw-rw-rw-   0        0        0      520 2023-07-31 14:32:26.473879 dark_web_scraper-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1599 2023-07-31 14:31:05.000000 dark_web_scraper-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 14:32:26.476038 dark_web_scraper-0.2/setup.cfg
--rw-rw-rw-   0        0        0      860 2023-07-31 14:31:57.000000 dark_web_scraper-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 14:32:26.406787 dark_web_scraper-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 14:32:26.470620 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-31 14:32:26.000000 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-07-31 14:32:26.000000 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 14:32:26.000000 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-31 14:32:26.000000 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 14:32:26.000000 dark_web_scraper-0.2/src/dark_web_scraper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2222 2023-07-30 18:04:28.000000 dark_web_scraper-0.2/src/dark_web_scraper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.859561 dark_web_scraper-0.3/
+-rw-rw-rw-   0        0        0     1087 2023-07-30 16:23:56.000000 dark_web_scraper-0.3/LICENSE
+-rw-rw-rw-   0        0        0     2112 2023-07-31 14:36:28.858410 dark_web_scraper-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1599 2023-07-31 14:31:05.000000 dark_web_scraper-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:36:28.860565 dark_web_scraper-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      900 2023-07-31 14:36:13.000000 dark_web_scraper-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.775247 dark_web_scraper-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 14:36:28.847463 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/
+-rw-rw-rw-   0        0        0     2112 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 14:36:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2222 2023-07-30 18:04:28.000000 dark_web_scraper-0.3/src/dark_web_scraper.py
```

### Comparing `dark_web_scraper-0.2/LICENSE` & `dark_web_scraper-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dark_web_scraper-0.2/README.md` & `dark_web_scraper-0.3/README.md`

 * *Files identical despite different names*

### Comparing `dark_web_scraper-0.2/setup.py` & `dark_web_scraper-0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='dark_web_scraper',
-    version='0.2',
+    version='0.3',
     description='A dark web link and image scraper',
     author= 'Pritam Sarbajna',
     url = 'https://github.com/PritamSarbajna/dark-web-scraper',
+    long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     keywords=['darkweb', 'web scraper', 'scraper'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
```

### Comparing `dark_web_scraper-0.2/src/dark_web_scraper.py` & `dark_web_scraper-0.3/src/dark_web_scraper.py`

 * *Files identical despite different names*

