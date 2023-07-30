# Comparing `tmp/psycopg_infdate-1.0.2.tar.gz` & `tmp/psycopg_infdate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg_infdate-1.0.2.tar", last modified: Mon May 22 17:59:50 2023, max compression
+gzip compressed data, was "psycopg_infdate-1.0.3.tar", last modified: Sun Jul 30 22:37:29 2023, max compression
```

## Comparing `psycopg_infdate-1.0.2.tar` & `psycopg_infdate-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.142082 psycopg_infdate-1.0.2/
--rw-r--r--   0 pjb1008    (501) staff       (20)     7652 2023-04-29 22:38:10.000000 psycopg_infdate-1.0.2/LICENSE
--rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-05-22 17:59:50.141969 psycopg_infdate-1.0.2/PKG-INFO
--rw-r--r--   0 pjb1008    (501) staff       (20)     4262 2023-04-29 22:03:05.000000 psycopg_infdate-1.0.2/README.md
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.140870 psycopg_infdate-1.0.2/psycopg_infdate/
--rw-r--r--   0 pjb1008    (501) staff       (20)     8689 2023-05-22 17:54:06.000000 psycopg_infdate-1.0.2/psycopg_infdate/__init__.py
-drwxr-xr-x   0 pjb1008    (501) staff       (20)        0 2023-05-22 17:59:50.141827 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/
--rw-r--r--   0 pjb1008    (501) staff       (20)     4942 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/PKG-INFO
--rw-r--r--   0 pjb1008    (501) staff       (20)      254 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/SOURCES.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)        1 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/dependency_links.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)       11 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/requires.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)       16 2023-05-22 17:59:50.000000 psycopg_infdate-1.0.2/psycopg_infdate.egg-info/top_level.txt
--rw-r--r--   0 pjb1008    (501) staff       (20)      782 2023-05-22 17:59:25.000000 psycopg_infdate-1.0.2/pyproject.toml
--rw-r--r--   0 pjb1008    (501) staff       (20)       38 2023-05-22 17:59:50.142117 psycopg_infdate-1.0.2/setup.cfg
+drwxr-xr-x   0 pjb1008  (11369) pjb1008grp (111369)        0 2023-07-30 22:37:29.283953 psycopg_infdate-1.0.3/
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)     7652 2023-05-22 10:48:43.000000 psycopg_infdate-1.0.3/LICENSE
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)     4942 2023-07-30 22:37:29.283953 psycopg_infdate-1.0.3/PKG-INFO
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)     4262 2023-05-22 10:48:43.000000 psycopg_infdate-1.0.3/README.md
+drwxr-xr-x   0 pjb1008  (11369) pjb1008grp (111369)        0 2023-07-30 22:37:29.283953 psycopg_infdate-1.0.3/psycopg_infdate/
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)    13262 2023-07-30 22:33:31.000000 psycopg_infdate-1.0.3/psycopg_infdate/__init__.py
+drwxr-xr-x   0 pjb1008  (11369) pjb1008grp (111369)        0 2023-07-30 22:37:29.283953 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)     4942 2023-07-30 22:37:29.000000 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/PKG-INFO
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)      254 2023-07-30 22:37:29.000000 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/SOURCES.txt
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)        1 2023-07-30 22:37:29.000000 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/dependency_links.txt
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)       11 2023-07-30 22:37:29.000000 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/requires.txt
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)       16 2023-07-30 22:37:29.000000 psycopg_infdate-1.0.3/psycopg_infdate.egg-info/top_level.txt
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)      782 2023-07-30 22:33:31.000000 psycopg_infdate-1.0.3/pyproject.toml
+-rw-r--r--   0 pjb1008  (11369) pjb1008grp (111369)       38 2023-07-30 22:37:29.283953 psycopg_infdate-1.0.3/setup.cfg
```

### Comparing `psycopg_infdate-1.0.2/LICENSE` & `psycopg_infdate-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psycopg_infdate-1.0.2/PKG-INFO` & `psycopg_infdate-1.0.3/psycopg_infdate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: psycopg_infdate
-Version: 1.0.2
+Name: psycopg-infdate
+Version: 1.0.3
 Summary: Support postgresql 'infinity'::DATE in psycopg3
 Author-email: Peter Benie <pjb1008@cam.ac.uk>
 Project-URL: Homepage, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psycopg_infdate-1.0.2/README.md` & `psycopg_infdate-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `psycopg_infdate-1.0.2/psycopg_infdate.egg-info/PKG-INFO` & `psycopg_infdate-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: psycopg-infdate
-Version: 1.0.2
+Name: psycopg_infdate
+Version: 1.0.3
 Summary: Support postgresql 'infinity'::DATE in psycopg3
 Author-email: Peter Benie <pjb1008@cam.ac.uk>
 Project-URL: Homepage, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate
 Project-URL: Bug Tracker, https://gitlab.developers.cam.ac.uk/pjb1008/psycopg-infdate/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `psycopg_infdate-1.0.2/pyproject.toml` & `psycopg_infdate-1.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psycopg_infdate"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Peter Benie", email="pjb1008@cam.ac.uk" },
 ]
 description = "Support postgresql 'infinity'::DATE in psycopg3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

