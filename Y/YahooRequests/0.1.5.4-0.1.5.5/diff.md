# Comparing `tmp/YahooRequests-0.1.5.4.tar.gz` & `tmp/YahooRequests-0.1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YahooRequests-0.1.5.4.tar", last modified: Mon Jul 31 13:53:43 2023, max compression
+gzip compressed data, was "YahooRequests-0.1.5.5.tar", last modified: Mon Jul 31 14:47:15 2023, max compression
```

## Comparing `YahooRequests-0.1.5.4.tar` & `YahooRequests-0.1.5.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:53:43.392552 YahooRequests-0.1.5.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.4/LICENSE.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1616 2023-07-31 13:53:43.392552 YahooRequests-0.1.5.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      716 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:53:43.388553 YahooRequests-0.1.5.4/YahooRequests/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.4/YahooRequests/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.4/YahooRequests/yahoorequests.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 13:53:43.392552 YahooRequests-0.1.5.4/YahooRequests.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1616 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       57 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 13:53:43.000000 YahooRequests-0.1.5.4/YahooRequests.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 13:53:43.392552 YahooRequests-0.1.5.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1239 2023-07-31 13:53:10.000000 YahooRequests-0.1.5.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1071 2023-07-31 09:06:36.000000 YahooRequests-0.1.5.5/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1728 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      827 2023-07-31 14:45:57.000000 YahooRequests-0.1.5.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.668552 YahooRequests-0.1.5.5/YahooRequests/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       70 2023-07-31 14:43:58.000000 YahooRequests-0.1.5.5/YahooRequests/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2116 2023-07-31 14:43:56.000000 YahooRequests-0.1.5.5/YahooRequests/yahoorequests.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/YahooRequests.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1728 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       67 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       14 2023-07-31 14:47:15.000000 YahooRequests-0.1.5.5/YahooRequests.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      470 2023-07-31 14:47:15.672552 YahooRequests-0.1.5.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1221 2023-07-31 14:46:49.000000 YahooRequests-0.1.5.5/setup.py
```

### Comparing `YahooRequests-0.1.5.4/LICENSE` & `YahooRequests-0.1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.4/LICENSE.txt` & `YahooRequests-0.1.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.4/PKG-INFO` & `YahooRequests-0.1.5.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.4
+Version: 0.1.5.5
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_two.tar.gz
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -38,7 +38,9 @@
 
     It is very simple you are only required to input a ticker  and it will return the live price
     the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
 
 ### YahooRequests.convert(ticker)
 
     The same goes for convert, the returned value will be the full company name
+
+If import YahooRequests gives an "import could not be resolved" error, try "pip install YahooRequests --user"
```

### Comparing `YahooRequests-0.1.5.4/README.md` & `YahooRequests-0.1.5.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 
     It is very simple you are only required to input a ticker  and it will return the live price
     the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
 
 ### YahooRequests.convert(ticker)
 
     The same goes for convert, the returned value will be the full company name
+
+If import YahooRequests gives an "import could not be resolved" error, try "pip install YahooRequests --user"
```

### Comparing `YahooRequests-0.1.5.4/YahooRequests/yahoorequests.py` & `YahooRequests-0.1.5.5/YahooRequests/yahoorequests.py`

 * *Files identical despite different names*

### Comparing `YahooRequests-0.1.5.4/YahooRequests.egg-info/PKG-INFO` & `YahooRequests-0.1.5.5/YahooRequests.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: YahooRequests
-Version: 0.1.5.4
+Version: 0.1.5.5
 Summary: A simple Python library for getting stock prices and company names from Yahoo Finance.
 Home-page: https://github.com/TheodorGajhede/YahooRequests
-Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_two.tar.gz
+Download-URL: https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz
 Author: Theodor Gajhede
 Author-email: theodorgajhede@gmail.com
 License: MIT
 Keywords: Stocks,Ticker,Yahoo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -38,7 +38,9 @@
 
     It is very simple you are only required to input a ticker  and it will return the live price
     the ticker will be unpacked using * so it can be a str, or a single byte list like ["googl"]
 
 ### YahooRequests.convert(ticker)
 
     The same goes for convert, the returned value will be the full company name
+
+If import YahooRequests gives an "import could not be resolved" error, try "pip install YahooRequests --user"
```

### Comparing `YahooRequests-0.1.5.4/setup.py` & `YahooRequests-0.1.5.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-from distutils.core import setup
+from setuptools import setup
+
 setup(
     name='YahooRequests',
     packages=['YahooRequests'],
-    version='0.1.5.4',
+    version='0.1.5.5',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     description='A simple Python library for getting stock prices and company names from Yahoo Finance.',
     author='Theodor Gajhede',
     author_email='theodorgajhede@gmail.com',
     url='https://github.com/TheodorGajhede/YahooRequests',
-    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_two.tar.gz',
+    download_url='https://github.com/TheodorGajhede/YahooRequests/archive/refs/tags/point_five.tar.gz',
     keywords=['Stocks', 'Ticker', 'Yahoo'],
     install_requires=[
           'requests'
           ],
     classifiers=[
         'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',      # Define that your audience are developers
+        'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',   # Again, pick a license
-        'Programming Language :: Python :: 3',      # Specify which pyhton versions that you want to support
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.8',
-            ],
+    ],
+    entry_points={
+        'console_scripts': [
+            'yahoorequests=YahooRequests.yahoorequests:main',
+        ],
+    },
 )
```

