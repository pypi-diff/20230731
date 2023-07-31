# Comparing `tmp/sentibank-0.0.1.tar.gz` & `tmp/sentibank-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentibank-0.0.1.tar", last modified: Mon Jul 31 16:57:21 2023, max compression
+gzip compressed data, was "sentibank-0.0.1.1.tar", last modified: Mon Jul 31 17:02:35 2023, max compression
```

## Comparing `sentibank-0.0.1.tar` & `sentibank-0.0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.821961 sentibank-0.0.1/
--rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      412 2023-07-31 16:57:21.821961 sentibank-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.691069 sentibank-0.0.1/sentibank/
--rw-rw-rw-   0        0        0       33 2023-07-31 16:55:28.000000 sentibank-0.0.1/sentibank/__init__.py
--rw-rw-rw-   0        0        0     2510 2023-07-31 16:55:43.000000 sentibank-0.0.1/sentibank/archive.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.728070 sentibank-0.0.1/sentibank/dict_arXiv/
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.741070 sentibank-0.0.1/sentibank/dict_arXiv/AFINN/
--rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
--rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.765774 sentibank-0.0.1/sentibank/dict_arXiv/Aigents/
--rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
--rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.805816 sentibank-0.0.1/sentibank/dict_arXiv/MASTER/
--rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
--rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.819960 sentibank-0.0.1/sentibank/dict_arXiv/VADER/
--rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1/sentibank/dict_arXiv/VADER/VADER_v2014.csv
--rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
--rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1/sentibank/dict_arXiv/emos.py
--rw-rw-rw-   0        0        0     8803 2023-07-31 16:56:44.000000 sentibank-0.0.1/sentibank/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:57:21.727070 sentibank-0.0.1/sentibank.egg-info/
--rw-rw-rw-   0        0        0      412 2023-07-31 16:57:21.000000 sentibank-0.0.1/sentibank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2023-07-31 16:57:21.000000 sentibank-0.0.1/sentibank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:57:21.000000 sentibank-0.0.1/sentibank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-07-31 16:57:21.000000 sentibank-0.0.1/sentibank.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-31 16:57:21.000000 sentibank-0.0.1/sentibank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-31 16:57:21.823961 sentibank-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      683 2023-07-31 16:56:53.000000 sentibank-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.352476 sentibank-0.0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-31 16:51:12.000000 sentibank-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-07-31 16:54:25.000000 sentibank-0.0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      416 2023-07-31 17:02:35.352476 sentibank-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2023-07-31 16:51:12.000000 sentibank-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.310598 sentibank-0.0.1.1/sentibank/
+-rw-rw-rw-   0        0        0        0 2023-07-31 17:01:20.000000 sentibank-0.0.1.1/sentibank/__init__.py
+-rw-rw-rw-   0        0        0     2510 2023-07-31 16:55:43.000000 sentibank-0.0.1.1/sentibank/archive.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.330475 sentibank-0.0.1.1/sentibank/dict_arXiv/
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.332475 sentibank-0.0.1.1/sentibank/dict_arXiv/AFINN/
+-rw-rw-rw-   0        0        0    42865 2023-07-25 14:30:20.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv
+-rw-rw-rw-   0        0        0    60808 2023-07-16 07:07:32.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.336476 sentibank-0.0.1.1/sentibank/dict_arXiv/Aigents/
+-rw-rw-rw-   0        0        0   291231 2023-07-25 14:32:19.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv
+-rw-rw-rw-   0        0        0   218491 2023-07-25 14:28:33.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.348475 sentibank-0.0.1.1/sentibank/dict_arXiv/MASTER/
+-rw-rw-rw-   0        0        0  8880507 2023-07-12 22:58:16.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv
+-rw-rw-rw-   0        0        0    69113 2023-07-13 22:11:21.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.351476 sentibank-0.0.1.1/sentibank/dict_arXiv/VADER/
+-rw-rw-rw-   0        0        0   449224 2023-07-14 01:06:34.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/VADER/VADER_v2014.csv
+-rw-rw-rw-   0        0        0   153216 2023-07-14 17:09:26.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle
+-rw-rw-rw-   0        0        0     3071 2023-07-25 14:11:12.000000 sentibank-0.0.1.1/sentibank/dict_arXiv/emos.py
+-rw-rw-rw-   0        0        0     8803 2023-07-31 16:56:44.000000 sentibank-0.0.1.1/sentibank/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:02:35.329476 sentibank-0.0.1.1/sentibank.egg-info/
+-rw-rw-rw-   0        0        0      416 2023-07-31 17:02:34.000000 sentibank-0.0.1.1/sentibank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2023-07-31 17:02:35.000000 sentibank-0.0.1.1/sentibank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:02:34.000000 sentibank-0.0.1.1/sentibank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-31 17:02:34.000000 sentibank-0.0.1.1/sentibank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 17:02:35.000000 sentibank-0.0.1.1/sentibank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-07-31 17:02:35.353475 sentibank-0.0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-07-31 17:01:51.000000 sentibank-0.0.1.1/setup.py
```

### Comparing `sentibank-0.0.1/LICENSE` & `sentibank-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/archive.py` & `sentibank-0.0.1.1/sentibank/archive.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv` & `sentibank-0.0.1.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle` & `sentibank-0.0.1.1/sentibank/dict_arXiv/AFINN/AFINN_v2015.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv` & `sentibank-0.0.1.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle` & `sentibank-0.0.1.1/sentibank/dict_arXiv/Aigents/Aigents+_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv` & `sentibank-0.0.1.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle` & `sentibank-0.0.1.1/sentibank/dict_arXiv/MASTER/MASTER_v2022.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/VADER/VADER_v2014.csv` & `sentibank-0.0.1.1/sentibank/dict_arXiv/VADER/VADER_v2014.csv`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle` & `sentibank-0.0.1.1/sentibank/dict_arXiv/VADER/VADER_v2014_mod.pickle`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/dict_arXiv/emos.py` & `sentibank-0.0.1.1/sentibank/dict_arXiv/emos.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank/utils.py` & `sentibank-0.0.1.1/sentibank/utils.py`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/sentibank.egg-info/SOURCES.txt` & `sentibank-0.0.1.1/sentibank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentibank-0.0.1/setup.py` & `sentibank-0.0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from distutils.core import setup
 
 setup(
   name = 'sentibank', 
   packages = ['sentibank'],   
-  version = '0.0.1',      
+  version = '0.0.1.1',      
   license='MIT',        
   description = 'TYPE YOUR DESCRIPTION HERE',   
   author = 'Nick S.H Oh',                   
   author_email = 'nick.sh.oh@socialscience.ai',      
   url = 'https://github.com/socius-org/sentibank',  
-  download_url = 'https://github.com/socius-org/sentibank/archive/refs/tags/0.0.1.tar.gz', 
+  download_url = 'https://github.com/socius-org/sentibank/archive/refs/tags/0.0.1.1.tar.gz', 
   keywords = ['AI', 'Social Science', 'Sentiment Analysis'],   # Keywords that define your package best
   install_requires=[
           'spacy',
           'spacymoji',
           'rich'
       ],
   include_package_data=True
```

