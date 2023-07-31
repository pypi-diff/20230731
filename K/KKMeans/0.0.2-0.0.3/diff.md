# Comparing `tmp/KKMeans-0.0.2.tar.gz` & `tmp/KKMeans-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.2.tar", last modified: Sun Jul 30 22:43:03 2023, max compression
+gzip compressed data, was "KKMeans-0.0.3.tar", last modified: Mon Jul 31 11:18:17 2023, max compression
```

## Comparing `KKMeans-0.0.2.tar` & `KKMeans-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-30 22:43:03.093339 KKMeans-0.0.2/
-drwxrwxrwx   0        0        0        0 2023-07-30 22:43:03.069906 KKMeans-0.0.2/KKMeans.egg-info/
--rw-rw-rw-   0        0        0      547 2023-07-30 22:43:03.000000 KKMeans-0.0.2/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      570 2023-07-30 22:43:03.000000 KKMeans-0.0.2/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-30 22:43:03.000000 KKMeans-0.0.2/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-30 22:43:03.000000 KKMeans-0.0.2/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-07-30 22:43:03.092831 KKMeans-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.2/README.md
--rw-rw-rw-   0        0        0      473 2023-07-30 22:03:57.000000 KKMeans-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-30 22:43:03.093339 KKMeans-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1464 2023-07-30 21:24:52.000000 KKMeans-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-30 22:43:03.059183 KKMeans-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-30 22:43:03.091810 KKMeans-0.0.2/src/KKMeans/
--rw-rw-rw-   0        0        0   904324 2023-07-29 08:22:59.000000 KKMeans-0.0.2/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27766 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1170842 2023-07-30 22:43:01.000000 KKMeans-0.0.2/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-07-30 22:43:02.000000 KKMeans-0.0.2/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.2/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1020999 2023-07-29 08:23:01.000000 KKMeans-0.0.2/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     2757 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.2/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.2/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.817079 KKMeans-0.0.3/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.787474 KKMeans-0.0.3/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0      607 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 11:18:17.000000 KKMeans-0.0.3/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      607 2023-07-31 11:18:17.817079 KKMeans-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.3/README.md
+-rw-rw-rw-   0        0        0      565 2023-07-31 11:17:57.000000 KKMeans-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 11:18:17.818152 KKMeans-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1637 2023-07-31 11:16:17.000000 KKMeans-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.770835 KKMeans-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 11:18:17.816078 KKMeans-0.0.3/src/KKMeans/
+-rw-rw-rw-   0        0        0   904324 2023-07-29 08:22:59.000000 KKMeans-0.0.3/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27766 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1170842 2023-07-31 11:18:16.000000 KKMeans-0.0.3/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-07-31 11:18:16.000000 KKMeans-0.0.3/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.3/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1020999 2023-07-29 08:23:01.000000 KKMeans-0.0.3/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     2757 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.3/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.3/src/KKMeans/utils.pyx
```

### Comparing `KKMeans-0.0.2/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.3/KKMeans.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 README.md
 pyproject.toml
 setup.py
 KKMeans.egg-info/PKG-INFO
 KKMeans.egg-info/SOURCES.txt
 KKMeans.egg-info/dependency_links.txt
+KKMeans.egg-info/requires.txt
 KKMeans.egg-info/top_level.txt
 src/KKMeans/KKMeans.c
 src/KKMeans/elkan.c
 src/KKMeans/kernels.c
 src/KKMeans/lloyd.c
 src/KKMeans/quality.c
 src/KKMeans/utils.c
```

### Comparing `KKMeans-0.0.2/setup.py` & `KKMeans-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -28,9 +28,11 @@
 ]
 
 # This is used for building the distribution for pipy
 # https://stackoverflow.com/questions/73766918/creating-python-package-which-uses-cython-valueerror
 package_data = {
     "KKMeans" : ["utils.pyx", "lloyd.pyx", "elkan.pyx", "kernels.pyx", "quality.pyx", "KKMeans.py"]
 }
-        
+
+# variables set here (except ext_modules) and not in Pyproject.toml as setuptool-specifics is still in beta
+# https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 setup(ext_modules=cythonize(extensions, compiler_directives=compiler_directives),package_dir={"KKMeans":"src/KKMeans"}, package_data=package_data, include_package_data=True)
```

### Comparing `KKMeans-0.0.2/src/KKMeans/KKMeans.c` & `KKMeans-0.0.3/src/KKMeans/KKMeans.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/KKMeans.py` & `KKMeans-0.0.3/src/KKMeans/KKMeans.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/elkan.c` & `KKMeans-0.0.3/src/KKMeans/elkan.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/elkan.pyx` & `KKMeans-0.0.3/src/KKMeans/elkan.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/kernels.c` & `KKMeans-0.0.3/src/KKMeans/kernels.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/kernels.pyx` & `KKMeans-0.0.3/src/KKMeans/kernels.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/lloyd.c` & `KKMeans-0.0.3/src/KKMeans/lloyd.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.3/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/quality.c` & `KKMeans-0.0.3/src/KKMeans/quality.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/quality.pyx` & `KKMeans-0.0.3/src/KKMeans/quality.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/utils.c` & `KKMeans-0.0.3/src/KKMeans/utils.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.2/src/KKMeans/utils.pyx` & `KKMeans-0.0.3/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

