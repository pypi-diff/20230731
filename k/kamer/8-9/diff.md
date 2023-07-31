# Comparing `tmp/kamer-8.tar.gz` & `tmp/kamer-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kamer-8.tar", last modified: Thu Oct 29 14:36:11 2015, max compression
+gzip compressed data, was "dist/kamer-9.tar", last modified: Sat Oct 31 12:54:45 2015, max compression
```

## Comparing `kamer-8.tar` & `kamer-9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-29 14:36:11.000000 kamer-8/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2942 2015-10-29 14:36:11.000000 kamer-8/PKG-INFO
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-29 14:36:11.000000 kamer-8/kamer/
--rw-rw-r--   0 bart      (1000) bart      (1000)      355 2015-10-27 20:41:47.000000 kamer-8/kamer/version.py
--rw-rw-r--   0 bart      (1000) bart      (1000)       65 2015-10-29 14:32:50.000000 kamer-8/kamer/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2179 2015-10-29 14:26:35.000000 kamer-8/README
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-29 14:36:11.000000 kamer-8/bin/
--rwxrwxr-x   0 bart      (1000) bart      (1000)      801 2015-10-25 09:15:50.000000 kamer-8/bin/kamer
--rw-rw-r--   0 bart      (1000) bart      (1000)       59 2015-10-29 14:36:11.000000 kamer-8/setup.cfg
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)     2942 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)      232 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        4 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2015-10-29 14:36:11.000000 kamer-8/kamer.egg-info/top_level.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-10-27 22:01:34.000000 kamer-8/kamer.egg-info/not-zip-safe
--rw-rw-r--   0 bart      (1000) bart      (1000)     3238 2015-10-29 14:32:44.000000 kamer-8/setup.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-31 12:54:45.000000 kamer-9/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2942 2015-10-31 12:54:45.000000 kamer-9/PKG-INFO
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-31 12:54:45.000000 kamer-9/kamer/
+-rw-rw-r--   0 bart      (1000) bart      (1000)      355 2015-10-27 20:41:47.000000 kamer-9/kamer/version.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)       65 2015-10-31 12:01:36.000000 kamer-9/kamer/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2179 2015-10-29 14:26:35.000000 kamer-9/README
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-31 12:54:45.000000 kamer-9/bin/
+-rwxrwxr-x   0 bart      (1000) bart      (1000)      801 2015-10-25 09:15:50.000000 kamer-9/bin/kamer
+-rw-rw-r--   0 bart      (1000) bart      (1000)       59 2015-10-31 12:54:45.000000 kamer-9/setup.cfg
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2942 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/dependency_links.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)      232 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/SOURCES.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        4 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/requires.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        6 2015-10-31 12:54:45.000000 kamer-9/kamer.egg-info/top_level.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2015-10-27 22:01:34.000000 kamer-9/kamer.egg-info/not-zip-safe
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3238 2015-10-31 12:54:39.000000 kamer-9/setup.py
```

### Comparing `kamer-8/PKG-INFO` & `kamer-9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kamer
-Version: 8
+Version: 9
 Summary:  KAMER - mishandeling gepleegd door toediening van voor het leven of de gezondheid schadelijk stoffen 
 Home-page: https://pikacode.com/bart/kamer
 Author: Bart Thate
 Author-email: bthate@dds.nl
 License: MIT
 Description:
```

### Comparing `kamer-8/README` & `kamer-9/README`

 * *Files identical despite different names*

### Comparing `kamer-8/bin/kamer` & `kamer-9/bin/kamer`

 * *Files identical despite different names*

### Comparing `kamer-8/kamer.egg-info/PKG-INFO` & `kamer-9/kamer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kamer
-Version: 8
+Version: 9
 Summary:  KAMER - mishandeling gepleegd door toediening van voor het leven of de gezondheid schadelijk stoffen 
 Home-page: https://pikacode.com/bart/kamer
 Author: Bart Thate
 Author-email: bthate@dds.nl
 License: MIT
 Description:
```

### Comparing `kamer-8/setup.py` & `kamer-9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 except Exception as ex: print(str(ex)) ; os._exit(1)
 
 from distutils import sysconfig
 site_packages_path = sysconfig.get_python_lib()
 
 setup(
     name='kamer',
-    version='8',
+    version='9',
     url='https://pikacode.com/bart/kamer',
     author='Bart Thate',
     author_email='bthate@dds.nl',
     description=""" KAMER - mishandeling gepleegd door toediening van voor het leven of de gezondheid schadelijk stoffen """,
     license='MIT',
     zip_safe=False,
     scripts=["bin/kamer",],
```

