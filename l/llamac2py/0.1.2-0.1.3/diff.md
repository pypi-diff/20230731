# Comparing `tmp/llamac2py-0.1.2.tar.gz` & `tmp/llamac2py-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamac2py-0.1.2.tar", last modified: Mon Jul 31 05:59:54 2023, max compression
+gzip compressed data, was "llamac2py-0.1.3.tar", last modified: Mon Jul 31 06:02:45 2023, max compression
```

## Comparing `llamac2py-0.1.2.tar` & `llamac2py-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 05:59:54.209163 llamac2py-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-07-30 17:40:42.000000 llamac2py-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      733 2023-07-31 05:59:54.209163 llamac2py-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1026 2023-07-31 04:11:20.000000 llamac2py-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 05:59:54.179947 llamac2py-0.1.2/llamac2py/
--rw-rw-rw-   0        0        0        0 2023-07-30 16:41:01.000000 llamac2py-0.1.2/llamac2py/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-30 18:50:11.000000 llamac2py-0.1.2/llamac2py/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-07-31 05:59:54.201041 llamac2py-0.1.2/llamac2py.egg-info/
--rw-rw-rw-   0        0        0      733 2023-07-31 05:59:53.000000 llamac2py-0.1.2/llamac2py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-07-31 05:59:54.000000 llamac2py-0.1.2/llamac2py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 05:59:53.000000 llamac2py-0.1.2/llamac2py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-31 05:59:27.000000 llamac2py-0.1.2/llamac2py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-31 05:59:53.000000 llamac2py-0.1.2/llamac2py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    22107 2023-07-30 17:40:42.000000 llamac2py-0.1.2/run.c
--rw-rw-rw-   0        0        0       42 2023-07-31 05:59:54.209163 llamac2py-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1386 2023-07-31 05:59:46.000000 llamac2py-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:02:45.746414 llamac2py-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-30 17:40:42.000000 llamac2py-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      733 2023-07-31 06:02:45.738414 llamac2py-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1026 2023-07-31 04:11:20.000000 llamac2py-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 06:02:45.714675 llamac2py-0.1.3/llamac2py/
+-rw-rw-rw-   0        0        0        0 2023-07-30 16:41:01.000000 llamac2py-0.1.3/llamac2py/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-30 18:50:11.000000 llamac2py-0.1.3/llamac2py/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-07-31 06:02:45.730397 llamac2py-0.1.3/llamac2py.egg-info/
+-rw-rw-rw-   0        0        0      733 2023-07-31 06:02:45.000000 llamac2py-0.1.3/llamac2py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-07-31 06:02:45.000000 llamac2py-0.1.3/llamac2py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 06:02:45.000000 llamac2py-0.1.3/llamac2py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-31 05:59:27.000000 llamac2py-0.1.3/llamac2py.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-31 06:02:45.000000 llamac2py-0.1.3/llamac2py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    22107 2023-07-30 17:40:42.000000 llamac2py-0.1.3/run.c
+-rw-rw-rw-   0        0        0       42 2023-07-31 06:02:45.746414 llamac2py-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1379 2023-07-31 06:02:41.000000 llamac2py-0.1.3/setup.py
```

### Comparing `llamac2py-0.1.2/LICENSE` & `llamac2py-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llamac2py-0.1.2/PKG-INFO` & `llamac2py-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: llamac2py
-Version: 0.1.2
+Version: 0.1.3
 Summary: llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.
 Author: Adarsh Shirawalmath
 License-File: LICENSE
 
 llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.
```

### Comparing `llamac2py-0.1.2/README.md` & `llamac2py-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llamac2py-0.1.2/llamac2py/wrapper.py` & `llamac2py-0.1.3/llamac2py/wrapper.py`

 * *Files identical despite different names*

### Comparing `llamac2py-0.1.2/llamac2py.egg-info/PKG-INFO` & `llamac2py-0.1.3/llamac2py.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 Metadata-Version: 2.1
 Name: llamac2py
-Version: 0.1.2
+Version: 0.1.3
 Summary: llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.
 Author: Adarsh Shirawalmath
 License-File: LICENSE
 
 llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.
```

### Comparing `llamac2py-0.1.2/run.c` & `llamac2py-0.1.3/run.c`

 * *Files identical despite different names*

### Comparing `llamac2py-0.1.2/setup.py` & `llamac2py-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 # Get the absolute path to the directory containing setup.py
 package_directory = os.path.abspath(os.path.dirname(__file__))
 
 # Define the C extension module
 c_extension = Extension(
     'llamac2py._c_module',  # The name of the C extension module
-    sources=[os.path.join(package_directory, 'llamac2py', 'run.c')],
+    sources=[os.path.join(package_directory, '..', 'run.c')],
 )
 
 
 # Setup the Python package
 setup(
     name='llamac2py',
     author='Adarsh Shirawalmath',
-    version='0.1.2',  # Update the version number accordingly
+    version='0.1.3',  # Update the version number accordingly
     description="llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.",
     long_description="llamac2py is a Python package that provides a wrapper for running inference using the Llama-2 Transformer model. The package includes a C executable (run.c) from Karpathy's llama2.c that performs the inference, and the wrapper module (wrapper.py) allows easy integration of the C code into Python scripts.",
     packages=['llamac2py'],
     ext_modules=[c_extension],  # Include the C extension module
     zip_safe=False,  # Set to False to ensure C extension is not placed in a zip archive
 )
```

