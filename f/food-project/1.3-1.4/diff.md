# Comparing `tmp/food_project-1.3.tar.gz` & `tmp/food_project-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "food_project-1.3.tar", last modified: Mon Jul 31 10:09:32 2023, max compression
+gzip compressed data, was "food_project-1.4.tar", last modified: Mon Jul 31 10:23:48 2023, max compression
```

## Comparing `food_project-1.3.tar` & `food_project-1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.048978 food_project-1.3/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      656 2023-07-31 10:09:32.048978 food_project-1.3/PKG-INFO
--rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)       38 2023-07-31 10:09:32.048978 food_project-1.3/setup.cfg
--rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)     1721 2023-07-31 10:09:13.000000 food_project-1.3/setup.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.036978 food_project-1.3/src/
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.036978 food_project-1.3/src/food_project/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      901 2023-07-31 09:51:27.000000 food_project-1.3/src/food_project/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.044978 food_project-1.3/src/food_project/bread/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/bread/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.044978 food_project-1.3/src/food_project/bread/bulo4ka/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/bread/bulo4ka/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      199 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/bread/bulo4ka/bulo4ka_s_kunjutom.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.044978 food_project-1.3/src/food_project/extra/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/extra/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       15 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/extra/cheese.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       40 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/extra/sause.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.048978 food_project-1.3/src/food_project/extra/vegetables/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      286 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/extra/vegetables/__init__.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.048978 food_project-1.3/src/food_project/meat/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/meat/__init__.py
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       47 2023-07-31 08:18:41.000000 food_project-1.3/src/food_project/meat/kotleta.py
-drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:09:32.044978 food_project-1.3/src/food_project.egg-info/
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      656 2023-07-31 10:09:31.000000 food_project-1.3/src/food_project.egg-info/PKG-INFO
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      633 2023-07-31 10:09:32.000000 food_project-1.3/src/food_project.egg-info/SOURCES.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 10:09:31.000000 food_project-1.3/src/food_project.egg-info/dependency_links.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       56 2023-07-31 10:09:31.000000 food_project-1.3/src/food_project.egg-info/entry_points.txt
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 09:46:38.000000 food_project-1.3/src/food_project.egg-info/not-zip-safe
--rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       13 2023-07-31 10:09:31.000000 food_project-1.3/src/food_project.egg-info/top_level.txt
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      693 2023-07-31 10:23:48.304672 food_project-1.4/PKG-INFO
+-rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)       38 2023-07-31 10:23:48.304672 food_project-1.4/setup.cfg
+-rwxrwxrwx   0 zukhra    (1000) zukhra    (1000)     1769 2023-07-31 10:23:36.000000 food_project-1.4/setup.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.296672 food_project-1.4/src/
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.296672 food_project-1.4/src/food_project/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      901 2023-07-31 09:51:27.000000 food_project-1.4/src/food_project/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project/bread/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/bread/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project/bread/bulo4ka/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/bread/bulo4ka/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      199 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/bread/bulo4ka/bulo4ka_s_kunjutom.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project/extra/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/extra/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       15 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/extra/cheese.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       40 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/extra/sause.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project/extra/vegetables/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      286 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/extra/vegetables/__init__.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project/meat/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/meat/__init__.py
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       47 2023-07-31 08:18:41.000000 food_project-1.4/src/food_project/meat/kotleta.py
+drwxrwxr-x   0 zukhra    (1000) zukhra    (1000)        0 2023-07-31 10:23:48.304672 food_project-1.4/src/food_project.egg-info/
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      693 2023-07-31 10:23:48.000000 food_project-1.4/src/food_project.egg-info/PKG-INFO
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)      633 2023-07-31 10:23:48.000000 food_project-1.4/src/food_project.egg-info/SOURCES.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 10:23:48.000000 food_project-1.4/src/food_project.egg-info/dependency_links.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       56 2023-07-31 10:23:48.000000 food_project-1.4/src/food_project.egg-info/entry_points.txt
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)        1 2023-07-31 09:46:38.000000 food_project-1.4/src/food_project.egg-info/not-zip-safe
+-rw-rw-r--   0 zukhra    (1000) zukhra    (1000)       13 2023-07-31 10:23:48.000000 food_project-1.4/src/food_project.egg-info/top_level.txt
```

### Comparing `food_project-1.3/PKG-INFO` & `food_project-1.4/src/food_project.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 1.1
-Name: food_project
-Version: 1.3
+Metadata-Version: 2.1
+Name: food-project
+Version: 1.4
 Summary: An example package.
 Home-page: UNKNOWN
 Author: Zukhra Khubieva & Vadim Petruhnenko \ shuygena
 Author-email: hubieva123@icloud.com
 License: UNKNOWN
 Description: Very tasty burger
 Platform: UNKNOWN
@@ -12,7 +12,8 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Description-Content-Type: text/x-rst
```

### Comparing `food_project-1.3/setup.py` & `food_project-1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='food_project',
-    version='1.3',
+    version='1.4',
     description='An example package.',
     long_description='Very tasty burger',
+    long_description_content_type='text/x-rst',
     author='Zukhra Khubieva & Vadim Petruhnenko \\ shuygena',
     author_email='hubieva123@icloud.com',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=False,
```

### Comparing `food_project-1.3/src/food_project/__init__.py` & `food_project-1.4/src/food_project/__init__.py`

 * *Files identical despite different names*

### Comparing `food_project-1.3/src/food_project.egg-info/SOURCES.txt` & `food_project-1.4/src/food_project.egg-info/SOURCES.txt`

 * *Files identical despite different names*

