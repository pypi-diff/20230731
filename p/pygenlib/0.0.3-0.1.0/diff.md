# Comparing `tmp/pygenlib-0.0.3.tar.gz` & `tmp/pygenlib-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenlib-0.0.3.tar", last modified: Mon Jul 31 07:45:12 2023, max compression
+gzip compressed data, was "pygenlib-0.1.0.tar", last modified: Mon Jul 31 07:33:29 2023, max compression
```

## Comparing `pygenlib-0.0.3.tar` & `pygenlib-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 07:45:12.598526 pygenlib-0.0.3/
--rw-rw-rw-   0        0        0     1333 2023-07-31 07:45:12.596527 pygenlib-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-07-31 07:34:36.000000 pygenlib-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 07:45:12.583526 pygenlib-0.0.3/pygenlib.egg-info/
--rw-rw-rw-   0        0        0     1333 2023-07-31 07:45:12.000000 pygenlib-0.0.3/pygenlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-31 07:45:12.000000 pygenlib-0.0.3/pygenlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 07:45:12.000000 pygenlib-0.0.3/pygenlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-31 07:45:12.000000 pygenlib-0.0.3/pygenlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 07:45:12.000000 pygenlib-0.0.3/pygenlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-31 07:45:12.588526 pygenlib-0.0.3/pylibgen/
--rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.0.3/pylibgen/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-07-31 07:16:09.000000 pygenlib-0.0.3/pylibgen/create_library_template.py
-drwxrwxrwx   0        0        0        0 2023-07-31 07:45:12.593526 pygenlib-0.0.3/pylibgen/templates/
--rw-rw-rw-   0        0        0      528 2023-07-31 07:19:28.000000 pygenlib-0.0.3/pylibgen/templates/setup_template.py
--rw-rw-rw-   0        0        0     2827 2023-07-31 07:28:51.000000 pygenlib-0.0.3/pylibgen/templates/updater_template.py
--rw-rw-rw-   0        0        0       42 2023-07-31 07:45:12.598526 pygenlib-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-07-31 07:44:57.000000 pygenlib-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:29.327203 pygenlib-0.1.0/
+-rw-rw-rw-   0        0        0     1298 2023-07-31 07:33:29.323207 pygenlib-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      868 2023-07-31 07:31:37.000000 pygenlib-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:29.310207 pygenlib-0.1.0/pygenlib.egg-info/
+-rw-rw-rw-   0        0        0     1298 2023-07-31 07:33:28.000000 pygenlib-0.1.0/pygenlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-31 07:33:29.000000 pygenlib-0.1.0/pygenlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 07:33:28.000000 pygenlib-0.1.0/pygenlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 07:33:28.000000 pygenlib-0.1.0/pygenlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:29.315211 pygenlib-0.1.0/pylibgen/
+-rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.1.0/pylibgen/__init__.py
+-rw-rw-rw-   0        0        0     3014 2023-07-31 07:16:09.000000 pygenlib-0.1.0/pylibgen/create_library_template.py
+drwxrwxrwx   0        0        0        0 2023-07-31 07:33:29.321206 pygenlib-0.1.0/pylibgen/templates/
+-rw-rw-rw-   0        0        0      528 2023-07-31 07:19:28.000000 pygenlib-0.1.0/pylibgen/templates/setup_template.py
+-rw-rw-rw-   0        0        0     2827 2023-07-31 07:28:51.000000 pygenlib-0.1.0/pylibgen/templates/updater_template.py
+-rw-rw-rw-   0        0        0       42 2023-07-31 07:33:29.328205 pygenlib-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      684 2023-07-31 07:33:14.000000 pygenlib-0.1.0/setup.py
```

### Comparing `pygenlib-0.0.3/PKG-INFO` & `pygenlib-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.3
+Version: 0.1.0
 Summary: A Python library for generating other Python libraries
 Author: Harsh Avinash
 Author-email: harsh.avinash.official@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -41,9 +41,7 @@
 This will create the library in the specified target folder.
 
 After creating the template, you can customize the generated files to build your Python library as per your specific requirements.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-Made with 💖 by Harsh Avinash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygenlib-0.0.3/README.md` & `pygenlib-0.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -28,10 +28,8 @@
 
 This will create the library in the specified target folder.
 
 After creating the template, you can customize the generated files to build your Python library as per your specific requirements.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-Made with 💖 by Harsh Avinash
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygenlib-0.0.3/pygenlib.egg-info/PKG-INFO` & `pygenlib-0.1.0/pygenlib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.3
+Version: 0.1.0
 Summary: A Python library for generating other Python libraries
 Author: Harsh Avinash
 Author-email: harsh.avinash.official@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -41,9 +41,7 @@
 This will create the library in the specified target folder.
 
 After creating the template, you can customize the generated files to build your Python library as per your specific requirements.
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
-
-Made with 💖 by Harsh Avinash
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pygenlib-0.0.3/pylibgen/create_library_template.py` & `pygenlib-0.1.0/pylibgen/create_library_template.py`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.3/pylibgen/templates/setup_template.py` & `pygenlib-0.1.0/pylibgen/templates/setup_template.py`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.3/pylibgen/templates/updater_template.py` & `pygenlib-0.1.0/pylibgen/templates/updater_template.py`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.3/setup.py` & `pygenlib-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 from setuptools import setup
 
 # Read the long description from README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
-version = "0.0.3"
-
 setup(
     name='pygenlib',
-    version=version,
+    version='0.1.0',
     description='A Python library for generating other Python libraries',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Harsh Avinash',
     author_email='harsh.avinash.official@gmail.com',
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'Intended Audience :: Developers'
-    ],
-    entry_points={
-        'console_scripts': [
-            'pygenlib = pygenlib.create_library_template:main'
-        ]
-    },
+    ]
 )
```

