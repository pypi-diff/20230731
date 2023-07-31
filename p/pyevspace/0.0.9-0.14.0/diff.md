# Comparing `tmp/pyevspace-0.0.9.tar.gz` & `tmp/pyevspace-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevspace-0.0.9.tar", last modified: Thu Nov 17 03:45:43 2022, max compression
+gzip compressed data, was "pyevspace-0.14.0.tar", last modified: Mon Jul 31 05:57:22 2023, max compression
```

## Comparing `pyevspace-0.0.9.tar` & `pyevspace-0.14.0.tar`

### file list

```diff
@@ -1,29 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.266339 pyevspace-0.0.9/
--rw-rw-rw-   0        0        0     1090 2022-05-02 23:40:08.000000 pyevspace-0.0.9/LICENSE.txt
--rw-rw-rw-   0        0        0       23 2022-08-30 02:23:39.000000 pyevspace-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4836 2022-11-17 03:45:43.264344 pyevspace-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3996 2022-07-24 05:57:45.000000 pyevspace-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.200514 pyevspace-0.0.9/pyevspace/
--rw-rw-rw-   0        0        0      157 2022-11-17 03:25:00.000000 pyevspace-0.0.9/pyevspace/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.237417 pyevspace-0.0.9/pyevspace/examples/
--rw-rw-rw-   0        0        0        0 2022-11-17 02:47:58.000000 pyevspace-0.0.9/pyevspace/examples/__init__.py
--rw-rw-rw-   0        0        0     4317 2022-11-17 01:56:58.000000 pyevspace-0.0.9/pyevspace/examples/arithmetic.py
--rw-rw-rw-   0        0        0     4961 2022-11-17 02:46:30.000000 pyevspace-0.0.9/pyevspace/examples/creating.py
--rw-rw-rw-   0        0        0     4790 2022-11-17 02:22:46.000000 pyevspace-0.0.9/pyevspace/examples/methods.py
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.239411 pyevspace-0.0.9/pyevspace/include/
--rw-rw-rw-   0        0        0     7471 2022-11-16 01:04:36.000000 pyevspace-0.0.9/pyevspace/include/evspacemodule.h
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.213480 pyevspace-0.0.9/pyevspace/src/
--rw-rw-rw-   0        0        0    39315 2022-11-17 03:30:00.000000 pyevspace-0.0.9/pyevspace/src/evspacemodule.c
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.261352 pyevspace-0.0.9/pyevspace/tests/
--rw-rw-rw-   0        0        0        0 2022-11-17 02:47:58.000000 pyevspace-0.0.9/pyevspace/tests/__init__.py
--rw-rw-rw-   0        0        0     6254 2022-11-16 21:17:45.000000 pyevspace-0.0.9/pyevspace/tests/matrix_test.py
--rw-rw-rw-   0        0        0     4474 2022-11-16 22:04:21.000000 pyevspace-0.0.9/pyevspace/tests/module_test.py
--rw-rw-rw-   0        0        0      728 2022-11-17 03:44:20.000000 pyevspace-0.0.9/pyevspace/tests/pyevspace_tests.py
--rw-rw-rw-   0        0        0     7377 2022-11-16 20:55:34.000000 pyevspace-0.0.9/pyevspace/tests/vector_test.py
-drwxrwxrwx   0        0        0        0 2022-11-17 03:45:43.211485 pyevspace-0.0.9/pyevspace.egg-info/
--rw-rw-rw-   0        0        0     4836 2022-11-17 03:45:42.000000 pyevspace-0.0.9/pyevspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2022-11-17 03:45:43.000000 pyevspace-0.0.9/pyevspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-17 03:45:42.000000 pyevspace-0.0.9/pyevspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2022-11-17 03:45:42.000000 pyevspace-0.0.9/pyevspace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-17 03:45:43.267337 pyevspace-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1325 2022-11-17 03:43:22.000000 pyevspace-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.650717 pyevspace-0.14.0/
+-rw-rw-rw-   0        0        0     1090 2023-07-31 05:39:21.000000 pyevspace-0.14.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       23 2023-01-13 04:56:37.000000 pyevspace-0.14.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3525 2023-07-31 05:57:22.649719 pyevspace-0.14.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2551 2023-07-31 05:39:21.000000 pyevspace-0.14.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:57:22.650717 pyevspace-0.14.0/setup.cfg
+-rw-rw-rw-   0        0        0     1578 2023-07-31 05:39:21.000000 pyevspace-0.14.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.617137 pyevspace-0.14.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.632765 pyevspace-0.14.0/src/pyevspace/
+-rw-rw-rw-   0        0        0      152 2023-07-31 05:39:21.000000 pyevspace-0.14.0/src/pyevspace/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.630772 pyevspace-0.14.0/src/pyevspace/src/
+-rw-rw-rw-   0        0        0    25597 2023-07-31 05:39:21.000000 pyevspace-0.14.0/src/pyevspace/src/evspacemodule.c
+drwxrwxrwx   0        0        0        0 2023-07-31 05:57:22.644732 pyevspace-0.14.0/src/pyevspace.egg-info/
+-rw-rw-rw-   0        0        0     3525 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-31 05:57:22.000000 pyevspace-0.14.0/src/pyevspace.egg-info/top_level.txt
```

### Comparing `pyevspace-0.0.9/LICENSE.txt` & `pyevspace-0.14.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Quinton Barnes
+Copyright (c) 2023 Quinton Barnes
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyevspace-0.0.9/setup.py` & `pyevspace-0.14.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-from setuptools import setup, Extension
+from setuptools import setup, Extension, find_packages
 
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
+import sys
+sys.path.insert(0, 'src')
+from pyevspace.__init__ import __version__, __doc__
+
+from pathlib import Path
+
+currentDirectory = Path(__file__).parent
+longDescription = (currentDirectory / "README.md").read_text()
 
 ext_modules = [Extension(
-    '_pyevspace',
-    include_dirs=['pyevspace/include'],
-    sources=['pyevspace/src/evspacemodule.c'],
+    'pyevspace.core',
+    include_dirs=['src/pyevspace/include'],
+    sources=['src/pyevspace/src/evspacemodule.c'],
 )]
 
 setup(name='pyevspace',
-      version='0.0.9',
+      version=__version__,
       author='Quinton Barnes',
       author_email='devqbizzle68@gmail.com',
-      description='A Euclidean vector space module.',
-      long_description=long_description,
+      description=__doc__,
+      long_description=longDescription,
       long_description_content_type='text/markdown',
       license='MIT',
       url='https://github.com/qbizzle68/pyevspace',
       classifiers=[
-          'Development Status :: 3 - Alpha',
+          'Development Status :: 4 - Beta',
           'Intended Audience :: Science/Research',
           'Intended Audience :: Developers',
           'License :: OSI Approved :: MIT License',
-          'Programming Language :: C',
-          'Programming Language :: Python :: 3',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
+          'Programming Language :: Python :: 3.11',
           'Programming Language :: Python :: Implementation :: CPython',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics',
           'Topic :: Software Development :: Libraries :: Python Modules',
       ],
-      packages=['pyevspace', 'pyevspace.examples', 'pyevspace.tests'],
+      packages=['pyevspace'],
+      package_dir={'': 'src'},
       ext_modules=ext_modules,
       )
```

