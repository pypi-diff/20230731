# Comparing `tmp/locache-3.0.0.tar.gz` & `tmp/locache-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "locache-3.0.0.tar", last modified: Fri Apr 21 16:11:06 2023, max compression
+gzip compressed data, was "locache-3.0.1.tar", last modified: Mon Jul 31 09:10:36 2023, max compression
```

## Comparing `locache-3.0.0.tar` & `locache-3.0.1.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564981 locache-3.0.0/
--rw-r--r--   0 john       (504) staff       (20)     1069 2022-12-06 14:45:21.000000 locache-3.0.0/LICENCE.md
--rw-r--r--   0 john       (504) staff       (20)     3318 2023-04-21 16:11:06.564820 locache-3.0.0/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)     2830 2022-12-06 14:45:21.000000 locache-3.0.0/README.md
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.563607 locache-3.0.0/locache/
--rw-r--r--   0 john       (504) staff       (20)     4538 2023-04-21 16:09:53.000000 locache-3.0.0/locache/__init__.py
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564242 locache-3.0.0/locache.egg-info/
--rw-r--r--   0 john       (504) staff       (20)     3318 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/PKG-INFO
--rw-r--r--   0 john       (504) staff       (20)      231 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/SOURCES.txt
--rw-r--r--   0 john       (504) staff       (20)        1 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/dependency_links.txt
--rw-r--r--   0 john       (504) staff       (20)       51 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/requires.txt
--rw-r--r--   0 john       (504) staff       (20)        8 2023-04-21 16:11:06.000000 locache-3.0.0/locache.egg-info/top_level.txt
--rw-r--r--   0 john       (504) staff       (20)     1042 2023-04-21 16:09:56.000000 locache-3.0.0/pyproject.toml
--rw-r--r--   0 john       (504) staff       (20)       38 2023-04-21 16:11:06.565030 locache-3.0.0/setup.cfg
-drwxr-xr-x   0 john       (504) staff       (20)        0 2023-04-21 16:11:06.564378 locache-3.0.0/tests/
--rw-r--r--   0 john       (504) staff       (20)     2176 2023-04-21 15:08:42.000000 locache-3.0.0/tests/test_locache.py
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-07-31 09:10:36.513600 locache-3.0.1/
+-rw-r--r--   0 john       (504) staff       (20)     1069 2022-12-06 14:45:21.000000 locache-3.0.1/LICENCE.md
+-rw-r--r--   0 john       (504) staff       (20)     2771 2023-07-31 09:10:36.513463 locache-3.0.1/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)     2282 2023-07-31 09:09:01.000000 locache-3.0.1/README.md
+drwxr-xr-x   0 john       (504) staff       (20)        0 2023-07-31 09:10:36.513295 locache-3.0.1/locache.egg-info/
+-rw-r--r--   0 john       (504) staff       (20)     2771 2023-07-31 09:10:36.000000 locache-3.0.1/locache.egg-info/PKG-INFO
+-rw-r--r--   0 john       (504) staff       (20)      200 2023-07-31 09:10:36.000000 locache-3.0.1/locache.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (504) staff       (20)        1 2023-07-31 09:10:36.000000 locache-3.0.1/locache.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (504) staff       (20)       39 2023-07-31 09:10:36.000000 locache-3.0.1/locache.egg-info/requires.txt
+-rw-r--r--   0 john       (504) staff       (20)        8 2023-07-31 09:10:36.000000 locache-3.0.1/locache.egg-info/top_level.txt
+-rw-r--r--   0 john       (504) staff       (20)     4539 2023-07-31 09:10:14.000000 locache-3.0.1/locache.py
+-rw-r--r--   0 john       (504) staff       (20)     1015 2023-07-31 09:10:14.000000 locache-3.0.1/pyproject.toml
+-rw-r--r--   0 john       (504) staff       (20)       38 2023-07-31 09:10:36.513641 locache-3.0.1/setup.cfg
```

### Comparing `locache-3.0.0/LICENCE.md` & `locache-3.0.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `locache-3.0.0/pyproject.toml` & `locache-3.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "locache"
-version = "3.0.0"
+version = "3.0.1"
 description = "Cache expensive function calls to disk."
 readme = "README.md"
 authors = [{ name = "John Gardner", email = "gardner.john97@gmail.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["cache", "disk"]
 dependencies = ["astor"]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
-dev = ["pytest", "pytest-cov", "bumpver", "sphinx", "furo"]
+dev = ["pytest", "pytest-cov", "bumpver"]
 
 [project.urls]
 Homepage = "https://github.com/jla-gardner/locache"
 
 [tool.bumpver]
-current_version = "3.0.0"
+current_version = "3.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
-"locache/__init__.py" = ["{version}"]
+"locache.py" = ["{version}"]
```

