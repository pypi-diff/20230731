# Comparing `tmp/MAZAlib-0.0.8.tar.gz` & `tmp/MAZAlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAZAlib-0.0.8.tar", last modified: Sat Jul 29 14:13:20 2023, max compression
+gzip compressed data, was "MAZAlib-0.0.9.tar", last modified: Sat Jul 29 14:16:06 2023, max compression
```

## Comparing `MAZAlib-0.0.8.tar` & `MAZAlib-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.8/LICENSE.txt
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/MAZAlib.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 14:13:20.000000 MAZAlib-0.0.8/MAZAlib.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      246 2023-07-29 14:13:20.000000 MAZAlib-0.0.8/MAZAlib.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 14:13:20.000000 MAZAlib-0.0.8/MAZAlib.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       29 2023-07-29 14:13:20.000000 MAZAlib-0.0.8/MAZAlib.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1898 2023-07-29 13:42:12.000000 MAZAlib-0.0.8/README.md
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/maza_cwrapper/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:02:59.000000 MAZAlib-0.0.8/maza_cwrapper/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1206 2023-07-29 13:11:12.000000 MAZAlib-0.0.8/maza_cwrapper/pythoninterface.cpp
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/mydist/
--rwxrwxr-x   0 andrey    (1000) andrey    (1000)    15232 2023-07-29 14:07:23.000000 MAZAlib-0.0.8/mydist/libmydist.so
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 14:13:20.383650 MAZAlib-0.0.8/setup.cfg
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1195 2023-07-29 14:12:50.000000 MAZAlib-0.0.8/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    35148 2023-07-29 11:56:29.000000 MAZAlib-0.0.9/LICENSE.txt
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/MAZAlib.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 14:16:06.000000 MAZAlib-0.0.9/MAZAlib.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      276 2023-07-29 14:16:06.000000 MAZAlib-0.0.9/MAZAlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2023-07-29 14:16:06.000000 MAZAlib-0.0.9/MAZAlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       29 2023-07-29 14:16:06.000000 MAZAlib-0.0.9/MAZAlib.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2545 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1898 2023-07-29 13:42:12.000000 MAZAlib-0.0.9/README.md
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/maza_cwrapper/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:02:59.000000 MAZAlib-0.0.9/maza_cwrapper/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1206 2023-07-29 13:11:12.000000 MAZAlib-0.0.9/maza_cwrapper/pythoninterface.cpp
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/mydist/
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/mydist/build/
+-rwxrwxr-x   0 andrey    (1000) andrey    (1000)    15232 2023-07-29 14:07:16.000000 MAZAlib-0.0.9/mydist/build/libmydist.so
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/mydist/include/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      132 2023-07-29 12:48:08.000000 MAZAlib-0.0.9/mydist/include/mydist.h
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       79 2023-07-29 14:16:06.319825 MAZAlib-0.0.9/setup.cfg
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1215 2023-07-29 14:16:00.000000 MAZAlib-0.0.9/setup.py
```

### Comparing `MAZAlib-0.0.8/LICENSE.txt` & `MAZAlib-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.8/MAZAlib.egg-info/PKG-INFO` & `MAZAlib-0.0.9/MAZAlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: TODO
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MAZAlib-0.0.8/PKG-INFO` & `MAZAlib-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MAZAlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: TODO
 Home-page: UNKNOWN
 Author: Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina
 Author-email: mathieu.gravey@unil.ch
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `MAZAlib-0.0.8/README.md` & `MAZAlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.8/maza_cwrapper/pythoninterface.cpp` & `MAZAlib-0.0.9/maza_cwrapper/pythoninterface.cpp`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.8/mydist/libmydist.so` & `MAZAlib-0.0.9/mydist/build/libmydist.so`

 * *Files identical despite different names*

### Comparing `MAZAlib-0.0.8/setup.py` & `MAZAlib-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 libName="MAZAlib"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=libName,
-    version="0.0.8",
+    version="0.0.9",
     description='TODO',
     long_description=long_description,
     author='Mathieu Gravey, Roman V. Vasilyev, Timofey Sizonenko, Kirill M. Gerke, Marina V. Karsanina',
     author_email='mathieu.gravey@unil.ch',
     license='GPLv3',
     packages=setuptools.find_packages() + ["mydist"],
-    package_data={'mydist': ['*.so']},
+    package_data={'mydist': ['build/*.so', 'include/*.h']},
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Education',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Programming Language :: C++',
         'Programming Language :: Python :: 3 :: Only',
@@ -27,10 +27,10 @@
     ],
     ext_modules=[setuptools.Extension(libName, sources=['./maza_cwrapper/pythoninterface.cpp'],
 			language="c++", 
 			extra_compile_args=["-std=c++17",'-O3', '-w'],
 			extra_link_args=["-std=c++17"],
 			# include_dirs=['./mydist/include'],
 			libraries = ["mydist_lib"],
-			library_dirs = ["./mydist//"]
+			library_dirs = ["./mydist/"]
 			)]
 )
```

