# Comparing `tmp/genetic-algo-0.1.0.tar.gz` & `tmp/genetic-algo-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.1.0.tar", last modified: Fri Jul  7 10:21:50 2023, max compression
+gzip compressed data, was "genetic-algo-1.0.0.tar", last modified: Mon Jul 31 16:07:42 2023, max compression
```

## Comparing `genetic-algo-0.1.0.tar` & `genetic-algo-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.543813 genetic-algo-0.1.0/
--rw-rw-rw-   0        0        0      115 2023-07-07 10:21:48.000000 genetic-algo-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2040 2023-07-07 10:21:50.542807 genetic-algo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-0.1.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.1.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.528807 genetic-algo-0.1.0/genetic_algo/
--rw-rw-rw-   0        0        0     9646 2023-07-07 10:19:44.000000 genetic-algo-0.1.0/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     6092 2023-07-07 10:20:42.000000 genetic-algo-0.1.0/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    15837 2023-07-07 10:18:26.000000 genetic-algo-0.1.0/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     4930 2023-07-07 10:21:09.000000 genetic-algo-0.1.0/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-07-07 10:21:50.541836 genetic-algo-0.1.0/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2040 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      382 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-07 10:21:50.000000 genetic-algo-0.1.0/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-07-07 10:21:48.000000 genetic-algo-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-0.1.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-0.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 10:21:50.543813 genetic-algo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-07-07 10:21:27.000000 genetic-algo-0.1.0/setup.py
--rw-rw-rw-   0        0        0     2842 2023-07-07 10:15:25.000000 genetic-algo-0.1.0/test.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:07:42.002089 genetic-algo-1.0.0/
+-rw-rw-rw-   0        0        0      115 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2040 2023-07-31 16:07:42.001081 genetic-algo-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1229 2023-07-01 09:05:38.000000 genetic-algo-1.0.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-1.0.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:07:41.984491 genetic-algo-1.0.0/genetic_algo/
+-rw-rw-rw-   0        0        0     9646 2023-07-07 10:19:44.000000 genetic-algo-1.0.0/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     6092 2023-07-07 10:20:42.000000 genetic-algo-1.0.0/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    15837 2023-07-31 16:07:22.000000 genetic-algo-1.0.0/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4930 2023-07-07 10:21:09.000000 genetic-algo-1.0.0/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:07:42.001081 genetic-algo-1.0.0/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2040 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      382 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-07-31 16:07:41.000000 genetic-algo-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       38 2023-06-18 08:47:03.000000 genetic-algo-1.0.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       29 2023-06-18 08:47:03.000000 genetic-algo-1.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:07:42.002089 genetic-algo-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-07-31 16:07:35.000000 genetic-algo-1.0.0/setup.py
+-rw-rw-rw-   0        0        0     2842 2023-07-07 10:15:25.000000 genetic-algo-1.0.0/test.py
```

### Comparing `genetic-algo-0.1.0/PKG-INFO` & `genetic-algo-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.1.0
+Version: 1.0.0
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.1.0/README.md` & `genetic-algo-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.1.0/build.py` & `genetic-algo-1.0.0/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.1.0/genetic_algo/attributes.py` & `genetic-algo-1.0.0/genetic_algo/attributes.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.1.0/genetic_algo/driver.py` & `genetic-algo-1.0.0/genetic_algo/driver.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.1.0/genetic_algo/environment.py` & `genetic-algo-1.0.0/genetic_algo/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,15 +403,15 @@
             callers = [
                 Caller(target=self.mate, args=(combination,))
                 for combination in parents_combinations
             ]
 
             return [
                 result.returns for result in
-                multi_threaded_call(callers=callers).callers.values()
+                multi_threaded_call(callers=callers).results.values()
             ]
         # end if
     # end mates
 
     def mutate(
             self,
             solution: Solution,
@@ -485,15 +485,15 @@
         else:
             return [
                 result.returns for result in multi_threaded_call(
                     callers=[
                         Caller(target=self.mutate, args=(solution,))
                         for solution in solutions
                     ]
-                ).callers.values()
+                ).results.values()
             ]
         # end if
     # end mutations
 
     def next(self, generation: Optional[Generation] = None) -> Generation:
         """
         Generates the next generation of solutions based on the given one.
```

### Comparing `genetic-algo-0.1.0/genetic_algo/solution.py` & `genetic-algo-1.0.0/genetic_algo/solution.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.1.0/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-1.0.0/genetic_algo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.1.0
+Version: 1.0.0
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.1.0/pyproject.toml` & `genetic-algo-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.1.0'
+version = '1.0.0'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.1.0/setup.py` & `genetic-algo-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.1.0',
+        version='1.0.0',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.1.0/test.py` & `genetic-algo-1.0.0/test.py`

 * *Files identical despite different names*

