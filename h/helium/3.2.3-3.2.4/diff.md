# Comparing `tmp/helium-3.2.3.tar.gz` & `tmp/helium-3.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helium-3.2.3.tar", last modified: Mon Jul 31 13:01:47 2023, max compression
+gzip compressed data, was "helium-3.2.4.tar", last modified: Mon Jul 31 13:06:04 2023, max compression
```

## Comparing `helium-3.2.3.tar` & `helium-3.2.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.208377 helium-3.2.3/
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2022-11-20 07:50:07.000000 helium-3.2.3/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)    30695 2022-11-20 07:50:07.000000 helium-3.2.3/NOTICE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:01:47.208377 helium-3.2.3/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-31 12:15:50.000000 helium-3.2.3/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium/
--rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-31 12:15:50.000000 helium-3.2.3/helium/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium/_impl/
--rw-r--r--   0 michael   (1000) michael   (1000)    44901 2023-07-31 12:15:50.000000 helium-3.2.3/helium/_impl/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-07-31 12:31:47.000000 helium-3.2.3/helium/_impl/chromedriver.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1140 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/match_type.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5411 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/selenium_wrappers.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium/_impl/util/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/dictionary.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6355 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/geom.py
--rw-r--r--   0 michael   (1000) michael   (1000)      979 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/html.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1210 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/inspect_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      570 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/lang.py
--rw-r--r--   0 michael   (1000) michael   (1000)      137 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/os_.py
--rw-r--r--   0 michael   (1000) michael   (1000)      584 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/path.py
--rw-r--r--   0 michael   (1000) michael   (1000)      374 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/system.py
--rw-r--r--   0 michael   (1000) michael   (1000)      466 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/util/xpath.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium/_impl/webdrivers/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium/_impl/webdrivers/linux/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/webdrivers/linux/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.200377 helium-3.2.3/helium/_impl/webdrivers/mac/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/webdrivers/mac/geckodriver
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.204377 helium-3.2.3/helium/_impl/webdrivers/windows/
--rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2022-11-20 07:50:07.000000 helium-3.2.3/helium/_impl/webdrivers/windows/geckodriver.exe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:01:47.196377 helium-3.2.3/helium.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:01:47.000000 helium-3.2.3/helium.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      759 2023-07-31 13:01:47.000000 helium-3.2.3/helium.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-31 13:01:47.000000 helium-3.2.3/helium.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-11-20 07:50:55.000000 helium-3.2.3/helium.egg-info/not-zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)      139 2023-07-31 13:01:47.000000 helium-3.2.3/helium.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-31 13:01:47.000000 helium-3.2.3/helium.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-31 13:01:47.208377 helium-3.2.3/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     1551 2023-07-31 12:57:21.000000 helium-3.2.3/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.310652 helium-3.2.4/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2022-11-20 07:50:07.000000 helium-3.2.4/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)    30695 2022-11-20 07:50:07.000000 helium-3.2.4/NOTICE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:06:04.310652 helium-3.2.4/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     6181 2023-07-31 12:15:50.000000 helium-3.2.4/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/
+-rw-r--r--   0 michael   (1000) michael   (1000)    36009 2023-07-31 12:15:50.000000 helium-3.2.4/helium/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/
+-rw-r--r--   0 michael   (1000) michael   (1000)    44901 2023-07-31 12:15:50.000000 helium-3.2.4/helium/_impl/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      278 2023-07-31 12:31:47.000000 helium-3.2.4/helium/_impl/chromedriver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1140 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/match_type.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5411 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/selenium_wrappers.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/dictionary.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6355 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/geom.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      979 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/html.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1210 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/inspect_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      570 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/lang.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      137 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/os_.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      584 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/path.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      374 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/system.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      466 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/util/xpath.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/webdrivers/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium/_impl/webdrivers/linux/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  7008696 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/linux/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.306651 helium-3.2.4/helium/_impl/webdrivers/mac/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  5259056 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/mac/geckodriver
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.310652 helium-3.2.4/helium/_impl/webdrivers/windows/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)  3566280 2022-11-20 07:50:07.000000 helium-3.2.4/helium/_impl/webdrivers/windows/geckodriver.exe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-31 13:06:04.302652 helium-3.2.4/helium.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1120 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      759 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2022-11-20 07:50:55.000000 helium-3.2.4/helium.egg-info/not-zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)       53 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-31 13:06:04.000000 helium-3.2.4/helium.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-31 13:06:04.310652 helium-3.2.4/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     1464 2023-07-31 13:05:24.000000 helium-3.2.4/setup.py
```

### Comparing `helium-3.2.3/LICENSE.txt` & `helium-3.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/NOTICE.txt` & `helium-3.2.4/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/PKG-INFO` & `helium-3.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helium
-Version: 3.2.3
+Version: 3.2.4
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 Keywords: helium selenium browser automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `helium-3.2.3/README.md` & `helium-3.2.4/README.md`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/__init__.py` & `helium-3.2.4/helium/__init__.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/__init__.py` & `helium-3.2.4/helium/_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/match_type.py` & `helium-3.2.4/helium/_impl/match_type.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/selenium_wrappers.py` & `helium-3.2.4/helium/_impl/selenium_wrappers.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/util/geom.py` & `helium-3.2.4/helium/_impl/util/geom.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/util/html.py` & `helium-3.2.4/helium/_impl/util/html.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/util/inspect_.py` & `helium-3.2.4/helium/_impl/util/inspect_.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/util/lang.py` & `helium-3.2.4/helium/_impl/util/lang.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/util/path.py` & `helium-3.2.4/helium/_impl/util/path.py`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/webdrivers/linux/geckodriver` & `helium-3.2.4/helium/_impl/webdrivers/linux/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/webdrivers/mac/geckodriver` & `helium-3.2.4/helium/_impl/webdrivers/mac/geckodriver`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium/_impl/webdrivers/windows/geckodriver.exe` & `helium-3.2.4/helium/_impl/webdrivers/windows/geckodriver.exe`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/helium.egg-info/PKG-INFO` & `helium-3.2.4/helium.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helium
-Version: 3.2.3
+Version: 3.2.4
 Summary: Lighter browser automation based on Selenium.
 Home-page: https://github.com/mherrmann/selenium-python-helium
 Author: Michael Herrmann
 Author-email: michael+removethisifyouarehuman@herrmann.io
 Keywords: helium selenium browser automation
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `helium-3.2.3/helium.egg-info/SOURCES.txt` & `helium-3.2.4/helium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helium-3.2.3/setup.py` & `helium-3.2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
 	name = 'helium',
 	# Also update docs/conf.py when you change this:
-	version = '3.2.3',
+	version = '3.2.4',
 	author = 'Michael Herrmann',
 	author_email = 'michael+removethisifyouarehuman@herrmann.io',
 	description = 'Lighter browser automation based on Selenium.',
 	keywords = 'helium selenium browser automation',
 	url = 'https://github.com/mherrmann/selenium-python-helium',
 	python_requires='>=3',
 	packages = find_packages(exclude=['tests', 'tests.*']),
 	install_requires = [
 		# Also update requirements/base.txt when you make changes here.
 		'selenium==3.141.0',
 		# Selenium 3 is incompatible with urllib3 >= 2:
 		'urllib3<2',
-		'webdriver-manager @ git+https://github.com/mherrmann/webdriver_manager@615a6f8589bbb902664d409de566da173b2260ae'
+		'webdriver-manager==4.0.0'
 	],
 	package_data = {
 		'helium._impl': ['webdrivers/**/*']
 	},
 	zip_safe = False,
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

