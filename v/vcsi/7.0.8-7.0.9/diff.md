# Comparing `tmp/vcsi-7.0.8.tar.gz` & `tmp/vcsi-7.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vcsi-7.0.8.tar", last modified: Fri Jan 11 10:33:57 2019, max compression
+gzip compressed data, was "dist/vcsi-7.0.9.tar", last modified: Wed Jan 16 14:36:34 2019, max compression
```

## Comparing `vcsi-7.0.8.tar` & `vcsi-7.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-11 10:33:57.000000 vcsi-7.0.8/
--rw-r--r--   0 user01    (1000) user01    (1000)      347 2019-01-11 10:33:57.000000 vcsi-7.0.8/PKG-INFO
--rw-r--r--   0 user01    (1000) user01    (1000)    13069 2018-07-31 07:15:54.000000 vcsi-7.0.8/README.md
--rw-r--r--   0 user01    (1000) user01    (1000)       38 2019-01-11 10:33:57.000000 vcsi-7.0.8/setup.cfg
--rw-r--r--   0 user01    (1000) user01    (1000)     2220 2019-01-08 17:20:55.000000 vcsi-7.0.8/setup.py
-drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi/
--rw-r--r--   0 user01    (1000) user01    (1000)        5 2019-01-11 10:29:43.000000 vcsi-7.0.8/vcsi/VERSION
--rw-r--r--   0 user01    (1000) user01    (1000)       54 2016-03-06 11:03:56.000000 vcsi-7.0.8/vcsi/__init__.py
--rwxr-xr-x   0 user01    (1000) user01    (1000)    54382 2019-01-11 10:29:18.000000 vcsi-7.0.8/vcsi/vcsi.py
-drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/
--rw-r--r--   0 user01    (1000) user01    (1000)      347 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/PKG-INFO
--rw-r--r--   0 user01    (1000) user01    (1000)      231 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/SOURCES.txt
--rw-r--r--   0 user01    (1000) user01    (1000)        1 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/dependency_links.txt
--rw-r--r--   0 user01    (1000) user01    (1000)       36 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/entry_points.txt
--rw-r--r--   0 user01    (1000) user01    (1000)       59 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/requires.txt
--rw-r--r--   0 user01    (1000) user01    (1000)        5 2019-01-11 10:33:57.000000 vcsi-7.0.8/vcsi.egg-info/top_level.txt
+drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-16 14:36:34.000000 vcsi-7.0.9/
+-rw-r--r--   0 user01    (1000) user01    (1000)      347 2019-01-16 14:36:34.000000 vcsi-7.0.9/PKG-INFO
+-rw-r--r--   0 user01    (1000) user01    (1000)    13069 2018-07-31 07:15:54.000000 vcsi-7.0.9/README.md
+-rw-r--r--   0 user01    (1000) user01    (1000)       38 2019-01-16 14:36:34.000000 vcsi-7.0.9/setup.cfg
+-rw-r--r--   0 user01    (1000) user01    (1000)     2233 2019-01-16 14:36:15.000000 vcsi-7.0.9/setup.py
+drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi/
+-rw-r--r--   0 user01    (1000) user01    (1000)        6 2019-01-16 14:36:32.000000 vcsi-7.0.9/vcsi/VERSION
+-rw-r--r--   0 user01    (1000) user01    (1000)       54 2016-03-06 11:03:56.000000 vcsi-7.0.9/vcsi/__init__.py
+-rwxr-xr-x   0 user01    (1000) user01    (1000)    54382 2019-01-11 10:29:18.000000 vcsi-7.0.9/vcsi/vcsi.py
+drwxr-xr-x   0 user01    (1000) user01    (1000)        0 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/
+-rw-r--r--   0 user01    (1000) user01    (1000)      347 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/PKG-INFO
+-rw-r--r--   0 user01    (1000) user01    (1000)      231 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/SOURCES.txt
+-rw-r--r--   0 user01    (1000) user01    (1000)        1 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/dependency_links.txt
+-rw-r--r--   0 user01    (1000) user01    (1000)       36 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/entry_points.txt
+-rw-r--r--   0 user01    (1000) user01    (1000)       69 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/requires.txt
+-rw-r--r--   0 user01    (1000) user01    (1000)        5 2019-01-16 14:36:34.000000 vcsi-7.0.9/vcsi.egg-info/top_level.txt
```

### Comparing `vcsi-7.0.8/README.md` & `vcsi-7.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vcsi-7.0.8/setup.py` & `vcsi-7.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "vcsi", "VERSION")) as f:
     VERSION = f.readline().strip()
 
-install_requires = ['numpy', 'pillow', 'jinja2']
+install_requires = ['numpy', 'pillow', 'jinja2', 'texttable']
 
 if sys.version_info < (3, 4):
     install_requires += ['enum34']
 
 setup(
     name='vcsi',
```

### Comparing `vcsi-7.0.8/vcsi/vcsi.py` & `vcsi-7.0.9/vcsi/vcsi.py`

 * *Files identical despite different names*

