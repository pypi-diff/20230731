# Comparing `tmp/directdb-0.0.2.tar.gz` & `tmp/directdb-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "directdb-0.0.2.tar", last modified: Mon Jul 31 13:53:43 2023, max compression
+gzip compressed data, was "directdb-1.0.0.tar", last modified: Mon Jul 31 14:03:11 2023, max compression
```

## Comparing `directdb-0.0.2.tar` & `directdb-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 13:53:43.602183 directdb-0.0.2/
--rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2448 2023-07-31 13:53:43.601187 directdb-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1731 2023-07-31 13:44:21.000000 directdb-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 13:53:43.594188 directdb-0.0.2/directdb/
--rw-rw-rw-   0        0        0       30 2023-07-31 13:36:43.000000 directdb-0.0.2/directdb/__init__.py
--rw-rw-rw-   0        0        0     1865 2023-07-31 06:56:02.000000 directdb-0.0.2/directdb/exceptions.py
--rw-rw-rw-   0        0        0     4598 2023-07-31 13:51:44.000000 directdb-0.0.2/directdb/main.py
-drwxrwxrwx   0        0        0        0 2023-07-31 13:53:43.600183 directdb-0.0.2/directdb.egg-info/
--rw-rw-rw-   0        0        0     2448 2023-07-31 13:53:43.000000 directdb-0.0.2/directdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-07-31 13:53:43.000000 directdb-0.0.2/directdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 13:53:43.000000 directdb-0.0.2/directdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 13:53:43.000000 directdb-0.0.2/directdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 13:53:43.000000 directdb-0.0.2/directdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 13:53:43.602183 directdb-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1117 2023-07-31 13:52:20.000000 directdb-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.434096 directdb-1.0.0/
+-rw-rw-rw-   0        0        0    35182 2023-07-31 07:28:41.000000 directdb-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     2515 2023-07-31 14:03:11.433100 directdb-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1796 2023-07-31 14:02:18.000000 directdb-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.427097 directdb-1.0.0/directdb/
+-rw-rw-rw-   0        0        0       30 2023-07-31 13:36:43.000000 directdb-1.0.0/directdb/__init__.py
+-rw-rw-rw-   0        0        0     1865 2023-07-31 06:56:02.000000 directdb-1.0.0/directdb/exceptions.py
+-rw-rw-rw-   0        0        0     4598 2023-07-31 13:51:44.000000 directdb-1.0.0/directdb/main.py
+drwxrwxrwx   0        0        0        0 2023-07-31 14:03:11.432099 directdb-1.0.0/directdb.egg-info/
+-rw-rw-rw-   0        0        0     2515 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 14:03:11.000000 directdb-1.0.0/directdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 14:03:11.434096 directdb-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2023-07-31 14:02:49.000000 directdb-1.0.0/setup.py
```

### Comparing `directdb-0.0.2/LICENSE` & `directdb-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `directdb-0.0.2/PKG-INFO` & `directdb-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 0.0.2
+Version: 1.0.0
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,17 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+## Github Repository
 
+https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
 
     
 ## License
```

### Comparing `directdb-0.0.2/README.md` & `directdb-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+## Github Repository
 
+https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
 
     
 ## License
```

### Comparing `directdb-0.0.2/directdb/exceptions.py` & `directdb-1.0.0/directdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `directdb-0.0.2/directdb/main.py` & `directdb-1.0.0/directdb/main.py`

 * *Files identical despite different names*

### Comparing `directdb-0.0.2/directdb.egg-info/PKG-INFO` & `directdb-1.0.0/directdb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directdb
-Version: 0.0.2
+Version: 1.0.0
 Summary: An async package that makes database handling extremely easy!
 Author: Cannonball Chris
 Author-email: cannonballchris8@gmail.com
 Keywords: db,bot,discord bot,database,postgresql,asyncpg,async,pgutils,nosql,sqlite
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,17 @@
 
 # directdb
 
 A simple library that makes handling SQL databases in python easy without the need to understand the syntax. The library would act like an interface between your code and the database server parsing the data to SQL format.
 
 If you enjoy using this project, consider giving it a star as it helps out a ton <3
 
+## Github Repository
 
+https://github.com/cannonballchris/directdb
 
 ## Installation
 
 To install the library, use `pip install directdb`
 
     
 ## License
```

### Comparing `directdb-0.0.2/setup.py` & `directdb-1.0.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import codecs
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '1.0.0'
 DESCRIPTION = 'An async package that makes database handling extremely easy!'
 
 # Setting up
 setup(
     name="directdb",
     version=VERSION,
     author="Cannonball Chris",
```

