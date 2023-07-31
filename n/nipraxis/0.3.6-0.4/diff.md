# Comparing `tmp/nipraxis-0.3.6.tar.gz` & `tmp/nipraxis-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nipraxis-0.3.6.tar", last modified: Wed Sep 28 03:20:43 2022, max compression
+gzip compressed data, was "nipraxis-0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nipraxis-0.3.6.tar` & `nipraxis-0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       61 2022-06-04 23:08:05.158960 nipraxis-0.3.6/.coveragerc
--rw-r--r--   0        0        0     1071 2022-06-04 23:06:07.191640 nipraxis-0.3.6/.github/workflows/testing.yml
--rw-r--r--   0        0        0       65 2022-06-04 23:01:14.082441 nipraxis-0.3.6/.gitignore
--rw-r--r--   0        0        0     1607 2022-03-17 17:46:42.127308 nipraxis-0.3.6/LICENSE
--rw-r--r--   0        0        0      278 2022-03-18 12:06:13.703840 nipraxis-0.3.6/README.md
--rw-r--r--   0        0        0      508 2022-09-28 01:52:50.628696 nipraxis-0.3.6/nipraxis/__init__.py
--rw-r--r--   0        0        0     3294 2022-09-28 02:05:32.696397 nipraxis-0.3.6/nipraxis/_fetcher.py
--rw-r--r--   0        0        0     1429 2022-03-18 20:24:20.743859 nipraxis-0.3.6/nipraxis/rotations.py
--rw-r--r--   0        0        0     1424 2022-03-18 20:26:01.959515 nipraxis-0.3.6/nipraxis/stimuli.py
--rw-r--r--   0        0        0        0 2022-03-17 17:45:36.192431 nipraxis-0.3.6/nipraxis/tests/__init__.py
--rw-r--r--   0        0        0     1049 2022-03-18 12:04:30.254428 nipraxis-0.3.6/nipraxis/tests/test_local_cache.py
--rw-r--r--   0        0        0     1087 2022-03-18 20:25:38.886290 nipraxis-0.3.6/nipraxis/tests/test_rotations.py
--rw-r--r--   0        0        0     1082 2022-03-18 20:26:01.960594 nipraxis-0.3.6/nipraxis/tests/test_stimuli.py
--rw-r--r--   0        0        0      520 2022-06-04 22:57:53.795946 nipraxis-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 nipraxis-0.3.6/setup.py
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 nipraxis-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-07-31 11:58:41.495402 nipraxis-0.4/.coveragerc
+-rw-r--r--   0        0        0     1071 2023-07-31 11:58:41.496299 nipraxis-0.4/.github/workflows/testing.yml
+-rw-r--r--   0        0        0       65 2023-07-31 11:58:41.497064 nipraxis-0.4/.gitignore
+-rw-r--r--   0        0        0     1607 2022-03-18 16:46:56.808775 nipraxis-0.4/LICENSE
+-rw-r--r--   0        0        0      278 2023-07-31 12:01:33.420932 nipraxis-0.4/README.md
+-rw-r--r--   0        0        0      506 2023-07-31 12:00:44.325251 nipraxis-0.4/nipraxis/__init__.py
+-rw-r--r--   0        0        0      249 2023-07-31 11:58:41.498013 nipraxis-0.4/nipraxis/_fetcher.py
+-rw-r--r--   0        0        0     1370 2023-07-31 11:58:41.498250 nipraxis-0.4/nipraxis/registry.yaml
+-rw-r--r--   0        0        0     1429 2022-04-04 15:15:30.625554 nipraxis-0.4/nipraxis/rotations.py
+-rw-r--r--   0        0        0     1424 2022-03-18 16:48:52.342462 nipraxis-0.4/nipraxis/stimuli.py
+-rw-r--r--   0        0        0        0 2022-03-18 16:46:56.809485 nipraxis-0.4/nipraxis/tests/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-31 11:58:41.498638 nipraxis-0.4/nipraxis/tests/test_local_cache.py
+-rw-r--r--   0        0        0     1087 2022-04-04 15:15:30.625886 nipraxis-0.4/nipraxis/tests/test_rotations.py
+-rw-r--r--   0        0        0     1082 2022-03-18 16:51:57.800992 nipraxis-0.4/nipraxis/tests/test_stimuli.py
+-rw-r--r--   0        0        0      524 2023-07-31 11:58:41.499076 nipraxis-0.4/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 nipraxis-0.4/PKG-INFO
```

### Comparing `nipraxis-0.3.6/.github/workflows/testing.yml` & `nipraxis-0.4/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/LICENSE` & `nipraxis-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/nipraxis/rotations.py` & `nipraxis-0.4/nipraxis/rotations.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/nipraxis/stimuli.py` & `nipraxis-0.4/nipraxis/stimuli.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/nipraxis/tests/test_rotations.py` & `nipraxis-0.4/nipraxis/tests/test_rotations.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/nipraxis/tests/test_stimuli.py` & `nipraxis-0.4/nipraxis/tests/test_stimuli.py`

 * *Files identical despite different names*

### Comparing `nipraxis-0.3.6/pyproject.toml` & `nipraxis-0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 name = "nipraxis"
 authors = [{name = "The Nipraxis team", email = "matthew.brett@gmail.com"}]
 classifiers = ["License :: OSI Approved :: BSD License",
                "Programming Language :: Python :: 3"]
 dynamic = ["version", "description"]
 readme = "README.md"
 license = {file = "LICENSE"}
-dependencies = ["pooch", "numpy"]
+dependencies = ["numpy", 'unscrewed']
 
 [project.optional-dependencies]
 test = ["pytest"]
 
 [project.urls]
 Home = "https://nipraxis.org"
```

### Comparing `nipraxis-0.3.6/PKG-INFO` & `nipraxis-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: nipraxis
-Version: 0.3.6
+Version: 0.4
 Summary: Nipraxis utilities
 Author-email: The Nipraxis team <matthew.brett@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: pooch
 Requires-Dist: numpy
+Requires-Dist: unscrewed
 Requires-Dist: pytest ; extra == "test"
 Project-URL: Home, https://nipraxis.org
 Provides-Extra: test
 
 # Nipraxis
 
 Tools for working with the [Nipraxis course](https://nipraxis.org)
```

