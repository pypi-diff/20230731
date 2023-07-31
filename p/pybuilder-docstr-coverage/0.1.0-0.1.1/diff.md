# Comparing `tmp/pybuilder-docstr-coverage-0.1.0.tar.gz` & `tmp/pybuilder-docstr-coverage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybuilder-docstr-coverage-0.1.0.tar", last modified: Thu Jul 27 13:48:52 2023, max compression
+gzip compressed data, was "pybuilder-docstr-coverage-0.1.1.tar", last modified: Mon Jul 31 11:09:49 2023, max compression
```

## Comparing `pybuilder-docstr-coverage-0.1.0.tar` & `pybuilder-docstr-coverage-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-27 13:48:52.005736 pybuilder-docstr-coverage-0.1.0/
--rw-rw-r--   0 chylek    (1000) chylek    (1000)      945 2023-07-27 13:48:52.005736 pybuilder-docstr-coverage-0.1.0/PKG-INFO
-drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-27 13:48:52.005736 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage/
--rw-rw-r--   0 chylek    (1000) chylek    (1000)     1226 2023-07-27 13:35:17.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage/__init__.py
-drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-27 13:48:52.005736 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/
--rw-rw-r--   0 chylek    (1000) chylek    (1000)      945 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/PKG-INFO
--rw-rw-r--   0 chylek    (1000) chylek    (1000)      344 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/SOURCES.txt
--rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/dependency_links.txt
--rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/namespace_packages.txt
--rw-rw-r--   0 chylek    (1000) chylek    (1000)       26 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/top_level.txt
--rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/zip-safe
--rw-rw-r--   0 chylek    (1000) chylek    (1000)       38 2023-07-27 13:48:52.005736 pybuilder-docstr-coverage-0.1.0/setup.cfg
--rwxr-xr-x   0 chylek    (1000) chylek    (1000)     2102 2023-07-27 13:48:51.000000 pybuilder-docstr-coverage-0.1.0/setup.py
+drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-31 11:09:49.655651 pybuilder-docstr-coverage-0.1.1/
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)      945 2023-07-31 11:09:49.655651 pybuilder-docstr-coverage-0.1.1/PKG-INFO
+drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-31 11:09:49.655651 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage/
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)     1232 2023-07-31 11:03:36.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage/__init__.py
+drwxrwxr-x   0 chylek    (1000) chylek    (1000)        0 2023-07-31 11:09:49.655651 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)      945 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/PKG-INFO
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)      344 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/SOURCES.txt
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/dependency_links.txt
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/namespace_packages.txt
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)       26 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/top_level.txt
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)        1 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/zip-safe
+-rw-rw-r--   0 chylek    (1000) chylek    (1000)       38 2023-07-31 11:09:49.655651 pybuilder-docstr-coverage-0.1.1/setup.cfg
+-rwxr-xr-x   0 chylek    (1000) chylek    (1000)     2102 2023-07-31 11:09:49.000000 pybuilder-docstr-coverage-0.1.1/setup.py
```

### Comparing `pybuilder-docstr-coverage-0.1.0/PKG-INFO` & `pybuilder-docstr-coverage-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-docstr-coverage
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyBuilder plugin that checks documentation coverage using docstr-coverage
 Home-page: https://github.com/chylek/pybuilder-docstr-coverage
 Author: Adam Chýlek
 Author-email: adam.chylek@amitia-ai.com
 Maintainer: 
 Maintainer-email: 
 License: MIT
```

### Comparing `pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage/__init__.py` & `pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
-from pybuilder.core import depends, init, task
+from pybuilder.core import dependents, init, task
 from pybuilder.errors import BuildFailedException
 
 
 @init
 def init_docstr_coverage_plugin(project):
     project.plugin_depends_on("docstr-coverage", "~=2.3.0")
 
 @task("docstr_coverage", "Checks coverage of docstrings")
-@depends("prepare")
+@dependents("analyze")
 def docstr_coverage(project, logger):
     # get location of source files
     src_dir = project.expand_path(project.get_property("dir_source_main_python"))
     docstr_args = [src_dir]
 
     # override default coverage threshold
     fail_under = project.get_property("docstr_coverage_fail_under", None)
```

### Comparing `pybuilder-docstr-coverage-0.1.0/pybuilder_docstr_coverage.egg-info/PKG-INFO` & `pybuilder-docstr-coverage-0.1.1/pybuilder_docstr_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybuilder-docstr-coverage
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyBuilder plugin that checks documentation coverage using docstr-coverage
 Home-page: https://github.com/chylek/pybuilder-docstr-coverage
 Author: Adam Chýlek
 Author-email: adam.chylek@amitia-ai.com
 Maintainer: 
 Maintainer-email: 
 License: MIT
```

### Comparing `pybuilder-docstr-coverage-0.1.0/setup.py` & `pybuilder-docstr-coverage-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.post_install_script()
 
 
 
 if __name__ == '__main__':
     setup(
         name = 'pybuilder-docstr-coverage',
-        version = '0.1.0',
+        version = '0.1.1',
         description = 'PyBuilder plugin that checks documentation coverage using docstr-coverage',
         long_description = 'Uses docstr-coverage to check documentation coverage of your project.\n\nYou can configure the docstr-coverage package using the following properties:\n\n- `docstr_coverage_fail_under`: The minimum coverage percentage that must be achieved. \n  If the coverage is below this value, the build will fail. This will take\n  precedence over the value set in the configuration file.\n- `docstr_coverage_config`: The path to the configuration file for docstr-coverage.\n  Default: .docstr.yaml\n',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'License :: OSI Approved :: MIT License',
             'Programming Language :: Python :: 3'
```

