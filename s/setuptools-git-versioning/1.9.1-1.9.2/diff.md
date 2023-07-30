# Comparing `tmp/setuptools-git-versioning-1.9.1.tar.gz` & `tmp/setuptools-git-versioning-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-git-versioning-1.9.1.tar", last modified: Mon Mar 21 14:45:47 2022, max compression
+gzip compressed data, was "setuptools-git-versioning-1.9.2.tar", last modified: Mon Mar 21 15:50:20 2022, max compression
```

## Comparing `setuptools-git-versioning-1.9.1.tar` & `setuptools-git-versioning-1.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 14:45:47.070646 setuptools-git-versioning-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 14:45:47.070646 setuptools-git-versioning-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-21 14:45:47.070646 setuptools-git-versioning-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 14:45:47.070646 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-21 14:45:46.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-03-21 14:45:30.000000 setuptools-git-versioning-1.9.1/setuptools_git_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3367 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-03-21 15:50:20.460611 setuptools-git-versioning-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 15:50:20.456611 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4627 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      503 2022-03-21 15:50:20.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-21 15:50:19.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-03-21 15:50:20.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-03-21 15:50:06.000000 setuptools-git-versioning-1.9.2/setuptools_git_versioning.py
```

### Comparing `setuptools-git-versioning-1.9.1/LICENSE` & `setuptools-git-versioning-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-git-versioning-1.9.1/PKG-INFO` & `setuptools-git-versioning-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-git-versioning
-Version: 1.9.1
+Version: 1.9.2
 Summary: Use git repo data for building a version number according PEP-440
 Home-page: https://setuptools-git-versioning.readthedocs.io
 Author: dolfinus
 Author-email: martinov.m.s.8@gmail.com
 License: MIT
 Project-URL: Documentation, https://setuptools-git-versioning.readthedocs.io
 Project-URL: Source, https://github.com/dolfinus/setuptools-git-versioning
```

### Comparing `setuptools-git-versioning-1.9.1/README.rst` & `setuptools-git-versioning-1.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `setuptools-git-versioning-1.9.1/setup.py` & `setuptools-git-versioning-1.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "CI/CD": "https://github.com/dolfinus/setuptools-git-versioning/actions",
         "Coverage": "https://app.codecov.io/gh/dolfinus/setuptools-git-versioning",
         "Tracker": "https://github.com/dolfinus/setuptools-git-versioning/issues",
     },
     python_requires=">=3.7",
     py_modules=["setuptools_git_versioning"],
     install_requires=requirements,
+    setup_requires=requirements,
     entry_points={
         "distutils.setup_keywords": [
             "version_config = setuptools_git_versioning:parse_config",
             "setuptools_git_versioning = setuptools_git_versioning:parse_config",
         ],
         "setuptools.finalize_distribution_options": [
             "setuptools_git_versioning = setuptools_git_versioning:infer_version",
```

### Comparing `setuptools-git-versioning-1.9.1/setuptools_git_versioning.egg-info/PKG-INFO` & `setuptools-git-versioning-1.9.2/setuptools_git_versioning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-git-versioning
-Version: 1.9.1
+Version: 1.9.2
 Summary: Use git repo data for building a version number according PEP-440
 Home-page: https://setuptools-git-versioning.readthedocs.io
 Author: dolfinus
 Author-email: martinov.m.s.8@gmail.com
 License: MIT
 Project-URL: Documentation, https://setuptools-git-versioning.readthedocs.io
 Project-URL: Source, https://github.com/dolfinus/setuptools-git-versioning
```

### Comparing `setuptools-git-versioning-1.9.1/setuptools_git_versioning.py` & `setuptools-git-versioning-1.9.2/setuptools_git_versioning.py`

 * *Files identical despite different names*

