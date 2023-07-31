# Comparing `tmp/YahooRequests-0.1.5.5.tar.gz` & `tmp/YahooRequests-0.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YahooRequests-0.1.5.5.tar", last modified: Mon Jul 31 14:47:15 2023, max compression
+gzip compressed data, was "YahooRequests-0.1.5.6.tar", last modified: Mon Jul 31 15:04:25 2023, max compression
```

## Comparing `YahooRequests-0.1.5.5.tar` & `YahooRequests-0.1.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.5/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.5/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1728 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      827 2023-07-31 14:45:57.000000 YahooRequests-0.1.5.5/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.668552 YahooRequests-0.1.5.5/YahooRequests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 14:43:58.000000 YahooRequests-0.1.5.5/YahooRequests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 14:43:56.000000 YahooRequests-0.1.5.5/YahooRequests/yahoorequests.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/YahooRequests.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1728 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1221 2023-07-31 14:46:49.000000 YahooRequests-0.1.5.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.6/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.6/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1879 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      827 2023-07-31 14:45:57.000000 YahooRequests-0.1.5.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/YahooRequests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 14:43:58.000000 YahooRequests-0.1.5.6/YahooRequests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 14:43:56.000000 YahooRequests-0.1.5.6/YahooRequests/yahoorequests.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/YahooRequests.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1879 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 15:04:25.000000 YahooRequests-0.1.5.6/YahooRequests.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 15:04:25.324552 YahooRequests-0.1.5.6/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1378 2023-07-31 15:04:09.000000 YahooRequests-0.1.5.6/setup.py
```

### Comparing `YahooRequests-0.1.5.5/LICENSE` & `YahooRequests-0.1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.5/LICENSE.txt` & `YahooRequests-0.1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.5/PKG-INFO` & `YahooRequests-0.1.5.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.5
+Version: 0.1.5.6
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_six.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 # Yahoo Requests
 
 ## By Theodor Gajhede from the northeren part of Denmark
```

### Comparing `YahooRequests-0.1.5.5/README.md` & `YahooRequests-0.1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.5/YahooRequests/yahoorequests.py` & `YahooRequests-0.1.5.6/YahooRequests/yahoorequests.py`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.5/YahooRequests.egg-info/PKG-INFO` & `YahooRequests-0.1.5.6/YahooRequests.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.5
+Version: 0.1.5.6
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_six.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 # Yahoo Requests
 
 ## By Theodor Gajhede from the northeren part of Denmark
```

### Comparing `YahooRequests-0.1.5.5/setup.py` & `YahooRequests-0.1.5.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from setuptools import setup
 
 setup(
     name='YahooRequests',
     packages=['YahooRequests'],
-    version='0.1.5.5',
+    version='0.1.5.6',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     description='A simple Python library for getting stock prices and company names from Yahoo Finance.',
     author='Theodor Gajhede',
     author_email='theodorgajhede@gmail.com',
     url='https://github.com/TheodorGajhede/YahooRequests',
-    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz',
+    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_six.tar.gz',
     keywords=['Stocks', 'Ticker', 'Yahoo'],
     install_requires=[
           'requests'
           ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        
     ],
     entry_points={
         'console_scripts': [
             'yahoorequests=YahooRequests.yahoorequests:main',
         ],
     },
 )
```

