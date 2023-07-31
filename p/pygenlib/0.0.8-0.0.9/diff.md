# Comparing `tmp/pygenlib-0.0.8.tar.gz` & `tmp/pygenlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenlib-0.0.8.tar", last modified: Mon Jul 31 08:07:41 2023, max compression
+gzip compressed data, was "pygenlib-0.0.9.tar", last modified: Mon Jul 31 08:11:51 2023, max compression
```

## Comparing `pygenlib-0.0.8.tar` & `pygenlib-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.293778 pygenlib-0.0.8/
--rw-rw-rw-   0        0        0     1333 2023-07-31 08:07:41.291776 pygenlib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-07-31 07:34:36.000000 pygenlib-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.276778 pygenlib-0.0.8/pygenlib/
--rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.0.8/pygenlib/__init__.py
--rw-rw-rw-   0        0        0     2999 2023-07-31 08:07:21.000000 pygenlib-0.0.8/pygenlib/create_library_template.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.289777 pygenlib-0.0.8/pygenlib.egg-info/
--rw-rw-rw-   0        0        0     1333 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-31 08:07:41.000000 pygenlib-0.0.8/pygenlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 08:07:41.293778 pygenlib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-07-31 08:07:26.000000 pygenlib-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:11:51.243453 pygenlib-0.0.9/
+-rw-rw-rw-   0        0        0     1319 2023-07-31 08:11:51.242455 pygenlib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-07-31 07:34:36.000000 pygenlib-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 08:11:51.217451 pygenlib-0.0.9/pygenlib/
+-rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.0.9/pygenlib/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-07-31 08:07:21.000000 pygenlib-0.0.9/pygenlib/create_library_template.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:11:51.240455 pygenlib-0.0.9/pygenlib/templates/
+-rw-rw-rw-   0        0        0      314 2023-07-31 07:10:02.000000 pygenlib-0.0.9/pygenlib/templates/readme_template.md
+-rw-rw-rw-   0        0        0      528 2023-07-31 07:19:28.000000 pygenlib-0.0.9/pygenlib/templates/setup_template.py
+-rw-rw-rw-   0        0        0     2827 2023-07-31 07:28:51.000000 pygenlib-0.0.9/pygenlib/templates/updater_template.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:11:51.232457 pygenlib-0.0.9/pygenlib.egg-info/
+-rw-rw-rw-   0        0        0     1319 2023-07-31 08:11:50.000000 pygenlib-0.0.9/pygenlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-07-31 08:11:51.000000 pygenlib-0.0.9/pygenlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:11:50.000000 pygenlib-0.0.9/pygenlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-31 08:11:50.000000 pygenlib-0.0.9/pygenlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 08:11:50.000000 pygenlib-0.0.9/pygenlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 08:11:51.243453 pygenlib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-07-31 08:11:36.000000 pygenlib-0.0.9/setup.py
```

### Comparing `pygenlib-0.0.8/PKG-INFO` & `pygenlib-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for generating other Python libraries
-Author: Harsh Avinash
-Author-email: harsh.avinash.official@gmail.com
+Author: Your Name
+Author-email: your.email@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # PyGenLib
```

### Comparing `pygenlib-0.0.8/README.md` & `pygenlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.8/pygenlib/create_library_template.py` & `pygenlib-0.0.9/pygenlib/create_library_template.py`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.8/pygenlib.egg-info/PKG-INFO` & `pygenlib-0.0.9/pygenlib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python library for generating other Python libraries
-Author: Harsh Avinash
-Author-email: harsh.avinash.official@gmail.com
+Author: Your Name
+Author-email: your.email@example.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
 
 # PyGenLib
```

### Comparing `pygenlib-0.0.8/setup.py` & `pygenlib-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from setuptools import setup, find_packages
 
 # Read the long description from README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
-version = "0.0.8"
+version = "0.0.9"
 
 setup(
     name='pygenlib',
     version=version,
     description='A Python library for generating other Python libraries',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    author='Harsh Avinash',
-    author_email='harsh.avinash.official@gmail.com',
+    author='Your Name',
+    author_email='your.email@example.com',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers'
     ],
     packages=find_packages(),
+    package_data={
+        'pygenlib': ['templates/*'],
+    },
     entry_points={
         'console_scripts': [
             'pygenlib = pygenlib.create_library_template:main'
         ]
     },
 )
```

