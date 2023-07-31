# Comparing `tmp/inpython-package-1.0.3.tar.gz` & `tmp/inpython-package-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inpython-package-1.0.3.tar", last modified: Fri Jul 14 14:28:03 2023, max compression
+gzip compressed data, was "inpython-package-1.0.4.tar", last modified: Mon Jul 31 06:52:59 2023, max compression
```

## Comparing `inpython-package-1.0.3.tar` & `inpython-package-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 14:28:03.561538 inpython-package-1.0.3/
--rw-rw-rw-   0        0        0     1092 2023-07-14 11:17:43.000000 inpython-package-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1079 2023-07-14 14:28:03.560527 inpython-package-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-07-14 14:26:49.000000 inpython-package-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-14 14:28:03.454570 inpython-package-1.0.3/inpython/
--rw-rw-rw-   0        0        0       47 2023-07-14 10:00:44.000000 inpython-package-1.0.3/inpython/__init__.py
--rw-rw-rw-   0        0        0       30 2023-07-14 10:01:04.000000 inpython-package-1.0.3/inpython/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:28:03.462538 inpython-package-1.0.3/inpython/ingraph/
--rw-rw-rw-   0        0        0      162 2023-07-14 14:27:31.000000 inpython-package-1.0.3/inpython/ingraph/__init__.py
--rw-rw-rw-   0        0        0     2442 2023-07-14 14:27:28.000000 inpython-package-1.0.3/inpython/ingraph/ingraph.py
-drwxrwxrwx   0        0        0        0 2023-07-14 14:28:03.556536 inpython-package-1.0.3/inpython_package.egg-info/
--rw-rw-rw-   0        0        0     1079 2023-07-14 14:28:03.000000 inpython-package-1.0.3/inpython_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      328 2023-07-14 14:28:03.000000 inpython-package-1.0.3/inpython_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 14:28:03.000000 inpython-package-1.0.3/inpython_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-14 14:28:03.000000 inpython-package-1.0.3/inpython_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-14 14:28:03.000000 inpython-package-1.0.3/inpython_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 14:28:03.562539 inpython-package-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      670 2023-07-14 14:27:23.000000 inpython-package-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:52:59.590288 inpython-package-1.0.4/
+-rw-rw-rw-   0        0        0     1092 2023-07-14 11:17:43.000000 inpython-package-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1078 2023-07-31 06:52:59.435278 inpython-package-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-07-14 14:26:49.000000 inpython-package-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:52:58.840677 inpython-package-1.0.4/inpython/
+-rw-rw-rw-   0        0        0       47 2023-07-14 10:00:44.000000 inpython-package-1.0.4/inpython/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-07-14 10:01:04.000000 inpython-package-1.0.4/inpython/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:52:59.246708 inpython-package-1.0.4/inpython/ingraph/
+-rw-rw-rw-   0        0        0      162 2023-07-14 14:27:31.000000 inpython-package-1.0.4/inpython/ingraph/__init__.py
+-rw-rw-rw-   0        0        0     6814 2023-07-31 06:52:04.000000 inpython-package-1.0.4/inpython/ingraph/ingraph.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:52:59.433285 inpython-package-1.0.4/inpython_package.egg-info/
+-rw-rw-rw-   0        0        0     1078 2023-07-31 06:52:56.000000 inpython-package-1.0.4/inpython_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2023-07-31 06:52:57.000000 inpython-package-1.0.4/inpython_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:52:56.000000 inpython-package-1.0.4/inpython_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-31 06:52:56.000000 inpython-package-1.0.4/inpython_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 06:52:57.000000 inpython-package-1.0.4/inpython_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:52:59.591295 inpython-package-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-07-31 06:51:59.000000 inpython-package-1.0.4/setup.py
```

### Comparing `inpython-package-1.0.3/LICENSE.txt` & `inpython-package-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inpython-package-1.0.3/PKG-INFO` & `inpython-package-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inpython-package
-Version: 1.0.3
+Version: 1.0.4
 Summary: # Infodata's IN-Tools U2Python Package
 Home-page: https://bitbucket.org/infodata-dev/inpython
 Author: infodata
-Author-email: info@infodata.lu
+Author-email: efv@infodata.lu
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # README #
```

### Comparing `inpython-package-1.0.3/README.md` & `inpython-package-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `inpython-package-1.0.3/inpython_package.egg-info/PKG-INFO` & `inpython-package-1.0.4/inpython_package.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: inpython-package
-Version: 1.0.3
+Version: 1.0.4
 Summary: # Infodata's IN-Tools U2Python Package
 Home-page: https://bitbucket.org/infodata-dev/inpython
 Author: infodata
-Author-email: info@infodata.lu
+Author-email: efv@infodata.lu
 License: MIT
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # README #
```

### Comparing `inpython-package-1.0.3/setup.py` & `inpython-package-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from setuptools import setup
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setup(
     name="inpython-package",
-    version="1.0.3",
+    version="1.0.4",
     author="infodata",
-    author_email="info@infodata.lu",
+    author_email="efv@infodata.lu",
     packages=find_packages(),
     description="# Infodata's IN-Tools U2Python Package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/infodata-dev/inpython",
     license='MIT',
     python_requires='>=3.4',
```

