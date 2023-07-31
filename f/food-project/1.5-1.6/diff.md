# Comparing `tmp/food_project-1.5.tar.gz` & `tmp/food_project-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "food_project-1.5.tar", last modified: Mon Jul 31 10:54:46 2023, max compression
+gzip compressed data, was "food_project-1.6.tar", last modified: Mon Jul 31 11:05:00 2023, max compression
```

## Comparing `food_project-1.5.tar` & `food_project-1.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      693 2023-07-31 10:54:46.222680 food_project-1.5/PKG-INFO
--rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)       38 2023-07-31 10:54:46.222680 food_project-1.5/setup.cfg
--rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)     1769 2023-07-31 10:54:23.000000 food_project-1.5/setup.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.214680 food_project-1.5/src/
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.214680 food_project-1.5/src/food_project/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      785 2023-07-31 10:53:48.000000 food_project-1.5/src/food_project/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project/bread/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/bread/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project/bread/bulo4ka/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/bread/bulo4ka/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      199 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/bread/bulo4ka/bulo4ka_s_kunjutom.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project/extra/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/extra/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       15 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/extra/cheese.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       40 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/extra/sause.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project/extra/vegetables/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      286 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/extra/vegetables/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project/meat/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/meat/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       47 2023-07-31 08:18:41.000000 food_project-1.5/src/food_project/meat/kotleta.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:54:46.222680 food_project-1.5/src/food_project.egg-info/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      693 2023-07-31 10:54:46.000000 food_project-1.5/src/food_project.egg-info/PKG-INFO
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      633 2023-07-31 10:54:46.000000 food_project-1.5/src/food_project.egg-info/SOURCES.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 10:54:46.000000 food_project-1.5/src/food_project.egg-info/dependency_links.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       56 2023-07-31 10:54:46.000000 food_project-1.5/src/food_project.egg-info/entry_points.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 09:46:38.000000 food_project-1.5/src/food_project.egg-info/not-zip-safe
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       13 2023-07-31 10:54:46.000000 food_project-1.5/src/food_project.egg-info/top_level.txt
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      726 2023-07-31 11:05:00.477191 food_project-1.6/PKG-INFO
+-rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)       38 2023-07-31 11:05:00.477191 food_project-1.6/setup.cfg
+-rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)     1821 2023-07-31 11:04:58.000000 food_project-1.6/setup.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.469191 food_project-1.6/src/
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.469191 food_project-1.6/src/food_project/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      785 2023-07-31 10:53:48.000000 food_project-1.6/src/food_project/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project/bread/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/bread/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project/bread/bulo4ka/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/bread/bulo4ka/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      199 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/bread/bulo4ka/bulo4ka_s_kunjutom.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project/extra/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/extra/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       15 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/extra/cheese.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       40 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/extra/sause.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project/extra/vegetables/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      286 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/extra/vegetables/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project/meat/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/meat/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       47 2023-07-31 08:18:41.000000 food_project-1.6/src/food_project/meat/kotleta.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 11:05:00.477191 food_project-1.6/src/food_project.egg-info/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      726 2023-07-31 11:05:00.000000 food_project-1.6/src/food_project.egg-info/PKG-INFO
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      633 2023-07-31 11:05:00.000000 food_project-1.6/src/food_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 11:05:00.000000 food_project-1.6/src/food_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       56 2023-07-31 11:05:00.000000 food_project-1.6/src/food_project.egg-info/entry_points.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 09:46:38.000000 food_project-1.6/src/food_project.egg-info/not-zip-safe
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       13 2023-07-31 11:05:00.000000 food_project-1.6/src/food_project.egg-info/top_level.txt
```

### Comparing `food_project-1.5/PKG-INFO` & `food_project-1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: food_project
-Version: 1.5
+Version: 1.6
 Summary: An example package.
-Home-page: UNKNOWN
+Home-page: https://github.com/shuygena/food_project
 Author: Zukhra Khubieva & Vadim Petruhnenko \ shuygena
 Author-email: hubieva123@icloud.com
 License: UNKNOWN
 Description: Very tasty burger
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `food_project-1.5/setup.py` & `food_project-1.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,18 +21,19 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='food_project',
-    version='1.5',
+    version='1.6',
     description='An example package.',
     long_description='Very tasty burger',
     long_description_content_type='text/x-rst',
+    url='https://github.com/shuygena/food_project',
     author='Zukhra Khubieva & Vadim Petruhnenko \\ shuygena',
     author_email='hubieva123@icloud.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
```

### Comparing `food_project-1.5/src/food_project/__init__.py` & `food_project-1.6/src/food_project/__init__.py`

 * *Files identical despite different names*

### Comparing `food_project-1.5/src/food_project.egg-info/PKG-INFO` & `food_project-1.6/src/food_project.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: food-project
-Version: 1.5
+Version: 1.6
 Summary: An example package.
-Home-page: UNKNOWN
+Home-page: https://github.com/shuygena/food_project
 Author: Zukhra Khubieva & Vadim Petruhnenko \ shuygena
 Author-email: hubieva123@icloud.com
 License: UNKNOWN
 Description: Very tasty burger
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `food_project-1.5/src/food_project.egg-info/SOURCES.txt` & `food_project-1.6/src/food_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

