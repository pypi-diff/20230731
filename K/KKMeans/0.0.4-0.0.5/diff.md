# Comparing `tmp/KKMeans-0.0.4.tar.gz` & `tmp/KKMeans-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KKMeans-0.0.4.tar", last modified: Mon Jul 31 11:50:01 2023, max compression
+gzip compressed data, was "KKMeans-0.0.5.tar", last modified: Mon Jul 31 12:15:23 2023, max compression
```

## Comparing `KKMeans-0.0.4.tar` & `KKMeans-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.987842 KKMeans-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.963330 KKMeans-0.0.4/KKMeans.egg-info/
--rw-rw-rw-   0        0        0      634 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-31 11:50:01.000000 KKMeans-0.0.4/KKMeans.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      634 2023-07-31 11:50:01.987332 KKMeans-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.4/README.md
--rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.4/license.txt
--rw-rw-rw-   0        0        0      565 2023-07-31 11:49:38.000000 KKMeans-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-31 11:50:01.987842 KKMeans-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1684 2023-07-31 11:49:30.000000 KKMeans-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.946003 KKMeans-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-31 11:50:01.986307 KKMeans-0.0.4/src/KKMeans/
--rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.4/src/KKMeans/KKMeans.c
--rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.4/src/KKMeans/KKMeans.py
--rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/__init__.py
--rw-rw-rw-   0        0        0  1170842 2023-07-31 11:50:00.000000 KKMeans-0.0.4/src/KKMeans/elkan.c
--rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/elkan.pyx
--rw-rw-rw-   0        0        0  1182482 2023-07-31 11:50:01.000000 KKMeans-0.0.4/src/KKMeans/kernels.c
--rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/kernels.pyx
--rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.4/src/KKMeans/lloyd.c
--rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/lloyd.pyx
--rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.4/src/KKMeans/quality.c
--rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.4/src/KKMeans/quality.pyx
--rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.4/src/KKMeans/utils.c
--rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.4/src/KKMeans/utils.pyx
+drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.253541 KKMeans-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.231119 KKMeans-0.0.5/KKMeans.egg-info/
+-rw-rw-rw-   0        0        0      585 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-31 12:15:23.000000 KKMeans-0.0.5/KKMeans.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      585 2023-07-31 12:15:23.253034 KKMeans-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-07-30 20:10:21.000000 KKMeans-0.0.5/README.md
+-rw-rw-rw-   0        0        0     1086 2023-07-31 11:30:04.000000 KKMeans-0.0.5/license.txt
+-rw-rw-rw-   0        0        0      521 2023-07-31 12:14:25.000000 KKMeans-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:15:23.253541 KKMeans-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1663 2023-07-31 12:13:21.000000 KKMeans-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.212752 KKMeans-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 12:15:23.252014 KKMeans-0.0.5/src/KKMeans/
+-rw-rw-rw-   0        0        0   875796 2023-07-31 11:49:59.000000 KKMeans-0.0.5/src/KKMeans/KKMeans.c
+-rw-rw-rw-   0        0        0    27233 2023-07-31 11:36:19.000000 KKMeans-0.0.5/src/KKMeans/KKMeans.py
+-rw-rw-rw-   0        0        0       43 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/__init__.py
+-rw-rw-rw-   0        0        0  1170842 2023-07-31 12:15:21.000000 KKMeans-0.0.5/src/KKMeans/elkan.c
+-rw-rw-rw-   0        0        0     9984 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/elkan.pyx
+-rw-rw-rw-   0        0        0  1182482 2023-07-31 12:15:22.000000 KKMeans-0.0.5/src/KKMeans/kernels.c
+-rw-rw-rw-   0        0        0     6892 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/kernels.pyx
+-rw-rw-rw-   0        0        0  1022846 2023-07-29 08:23:01.000000 KKMeans-0.0.5/src/KKMeans/lloyd.c
+-rw-rw-rw-   0        0        0     3427 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/lloyd.pyx
+-rw-rw-rw-   0        0        0  1004899 2023-07-31 11:50:00.000000 KKMeans-0.0.5/src/KKMeans/quality.c
+-rw-rw-rw-   0        0        0     1966 2023-07-31 11:38:16.000000 KKMeans-0.0.5/src/KKMeans/quality.pyx
+-rw-rw-rw-   0        0        0  1091399 2023-07-29 08:23:02.000000 KKMeans-0.0.5/src/KKMeans/utils.c
+-rw-rw-rw-   0        0        0     5309 2023-07-29 08:20:16.000000 KKMeans-0.0.5/src/KKMeans/utils.pyx
```

### Comparing `KKMeans-0.0.4/KKMeans.egg-info/PKG-INFO` & `KKMeans-0.0.5/KKMeans.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.4
+Version: 0.0.5
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 This is the github repository for my bachelor thesis.<br>
```

### Comparing `KKMeans-0.0.4/KKMeans.egg-info/SOURCES.txt` & `KKMeans-0.0.5/KKMeans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/PKG-INFO` & `KKMeans-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: KKMeans
-Version: 0.0.4
+Version: 0.0.5
 Summary: https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy
 Author-email: Paul Theis <keymailt7@gmail.com>
-Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 This is the github repository for my bachelor thesis.<br>
```

### Comparing `KKMeans-0.0.4/license.txt` & `KKMeans-0.0.5/license.txt`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/pyproject.toml` & `KKMeans-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [build-system]
 requires = ["setuptools>=63", "wheel", "Cython"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KKMeans"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Paul Theis", email="keymailt7@gmail.com" },
 ]
 dependencies = ["numpy>=1.25"]
 description = "https://github.com/bauxn/kernel-kmeans. openMP is not enabled when installing via PiPy"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
-    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `KKMeans-0.0.4/setup.py` & `KKMeans-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,13 +32,12 @@
 package_data = {
     "KKMeans" : ["utils.pyx", "lloyd.pyx", "elkan.pyx", "kernels.pyx", "quality.pyx", "KKMeans.py"]
 }
 
 # variables set here (except ext_modules) and not in Pyproject.toml as setuptool-specifics is still in beta
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 setup(
-    name="KKMeans",
     ext_modules=cythonize(extensions, compiler_directives=compiler_directives),
     package_dir={"KKMeans":"src/KKMeans"}, 
     package_data=package_data, 
     include_package_data=True
 )
```

### Comparing `KKMeans-0.0.4/src/KKMeans/KKMeans.c` & `KKMeans-0.0.5/src/KKMeans/KKMeans.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/KKMeans.py` & `KKMeans-0.0.5/src/KKMeans/KKMeans.py`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/elkan.c` & `KKMeans-0.0.5/src/KKMeans/elkan.c`

 * *Files 0% similar despite different names*

```diff
@@ -18246,15 +18246,15 @@
                                 __Pyx_PyGILState_Release(__pyx_gilstate_save);
                                 #endif
                             }
                             __pyx_parallel_why = 4;
                             goto __pyx_L13;
                             __pyx_L13:;
                             #ifdef _OPENMP
-                            #pragma omp critical(__pyx_parallel_lastprivates1)
+                            #pragma omp critical(__pyx_parallel_lastprivates0)
                             #endif /* _OPENMP */
                             {
                                 __pyx_parallel_temp0 = __pyx_v_i;
                                 __pyx_parallel_temp1 = __pyx_v_j;
                                 __pyx_parallel_temp2 = __pyx_v_labels_i;
                                 __pyx_parallel_temp3 = __pyx_v_outer_sum;
                             }
```

### Comparing `KKMeans-0.0.4/src/KKMeans/elkan.pyx` & `KKMeans-0.0.5/src/KKMeans/elkan.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/kernels.c` & `KKMeans-0.0.5/src/KKMeans/kernels.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/kernels.pyx` & `KKMeans-0.0.5/src/KKMeans/kernels.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/lloyd.c` & `KKMeans-0.0.5/src/KKMeans/lloyd.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/lloyd.pyx` & `KKMeans-0.0.5/src/KKMeans/lloyd.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/quality.c` & `KKMeans-0.0.5/src/KKMeans/quality.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/quality.pyx` & `KKMeans-0.0.5/src/KKMeans/quality.pyx`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/utils.c` & `KKMeans-0.0.5/src/KKMeans/utils.c`

 * *Files identical despite different names*

### Comparing `KKMeans-0.0.4/src/KKMeans/utils.pyx` & `KKMeans-0.0.5/src/KKMeans/utils.pyx`

 * *Files identical despite different names*

