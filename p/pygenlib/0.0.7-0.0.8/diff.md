# Comparing `tmp/pygenlib-0.0.7.tar.gz` & `tmp/pygenlib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygenlib-0.0.7.tar", last modified: Mon Jul 31 08:03:46 2023, max compression
+gzip compressed data, was "pygenlib-0.0.8.tar", last modified: Mon Jul 31 08:07:41 2023, max compression
```

## Comparing `pygenlib-0.0.7.tar` & `pygenlib-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 08:03:46.049305 pygenlib-0.0.7/
--rw-rw-rw-   0        0        0     1333 2023-07-31 08:03:46.048304 pygenlib-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      903 2023-07-31 07:34:36.000000 pygenlib-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 08:03:46.029307 pygenlib-0.0.7/pygenlib/
--rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.0.7/pygenlib/__init__.py
--rw-rw-rw-   0        0        0     3014 2023-07-31 07:16:09.000000 pygenlib-0.0.7/pygenlib/create_library_template.py
-drwxrwxrwx   0        0        0        0 2023-07-31 08:03:46.046304 pygenlib-0.0.7/pygenlib.egg-info/
--rw-rw-rw-   0        0        0     1333 2023-07-31 08:03:45.000000 pygenlib-0.0.7/pygenlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-07-31 08:03:45.000000 pygenlib-0.0.7/pygenlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 08:03:45.000000 pygenlib-0.0.7/pygenlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-31 08:03:45.000000 pygenlib-0.0.7/pygenlib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-07-31 08:03:45.000000 pygenlib-0.0.7/pygenlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 08:03:46.049305 pygenlib-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      885 2023-07-31 08:03:31.000000 pygenlib-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.293778 pygenlib-0.0.8/
+-rw-rw-rw-   0        0        0     1333 2023-07-31 08:07:41.291776 pygenlib-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      903 2023-07-31 07:34:36.000000 pygenlib-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.276778 pygenlib-0.0.8/pygenlib/
+-rw-rw-rw-   0        0        0       88 2023-07-31 07:03:08.000000 pygenlib-0.0.8/pygenlib/__init__.py
+-rw-rw-rw-   0        0        0     2999 2023-07-31 08:07:21.000000 pygenlib-0.0.8/pygenlib/create_library_template.py
+drwxrwxrwx   0        0        0        0 2023-07-31 08:07:41.289777 pygenlib-0.0.8/pygenlib.egg-info/
+-rw-rw-rw-   0        0        0     1333 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-07-31 08:07:41.000000 pygenlib-0.0.8/pygenlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 08:07:40.000000 pygenlib-0.0.8/pygenlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 08:07:41.293778 pygenlib-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      885 2023-07-31 08:07:26.000000 pygenlib-0.0.8/setup.py
```

### Comparing `pygenlib-0.0.7/PKG-INFO` & `pygenlib-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for generating other Python libraries
 Author: Harsh Avinash
 Author-email: harsh.avinash.official@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `pygenlib-0.0.7/README.md` & `pygenlib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pygenlib-0.0.7/pygenlib/create_library_template.py` & `pygenlib-0.0.8/pygenlib/create_library_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         updater_template = f.read()
     with open(os.path.join(library_path, 'updater.py'), 'w') as f:
         f.write(updater_template)
 
     print(f"Successfully created the '{library_name}' library template.")
 
 
-if __name__ == "__main__":
+def main():
     parser = argparse.ArgumentParser(
         description="Create a template for a Python library.")
     parser.add_argument("library_name", help="Name of the library to create.")
     parser.add_argument("--target", "-t", default=".",
                         help="Target folder to create the library (default: current directory).")
     args = parser.parse_args()
```

### Comparing `pygenlib-0.0.7/pygenlib.egg-info/PKG-INFO` & `pygenlib-0.0.8/pygenlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygenlib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python library for generating other Python libraries
 Author: Harsh Avinash
 Author-email: harsh.avinash.official@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
```

### Comparing `pygenlib-0.0.7/setup.py` & `pygenlib-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Read the long description from README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
-version = "0.0.7"
+version = "0.0.8"
 
 setup(
     name='pygenlib',
     version=version,
     description='A Python library for generating other Python libraries',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

