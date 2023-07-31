# Comparing `tmp/gungnir-0.2.1.tar.gz` & `tmp/gungnir-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gungnir-0.2.1.tar", last modified: Sat Jul 15 22:21:28 2023, max compression
+gzip compressed data, was "gungnir-0.2.2.tar", last modified: Mon Jul 31 20:21:34 2023, max compression
```

## Comparing `gungnir-0.2.1.tar` & `gungnir-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 22:21:02.000000 gungnir-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-15 22:21:28.000786 gungnir-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-15 22:21:02.000000 gungnir-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/dependencytrack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/gungnir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-15 22:21:02.000000 gungnir-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:21:28.000786 gungnir-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-15 22:21:02.000000 gungnir-0.2.1/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 20:21:06.000000 gungnir-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-31 20:21:34.709061 gungnir-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-31 20:21:06.000000 gungnir-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.705062 gungnir-0.2.2/gungnir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.705062 gungnir-0.2.2/gungnir/dependencytrack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-31 20:21:06.000000 gungnir-0.2.2/gungnir/dependencytrack/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/gungnir/gungnir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 20:21:34.000000 gungnir-0.2.2/gungnir/gungnir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-31 20:21:06.000000 gungnir-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 20:21:34.709061 gungnir-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:21:34.709061 gungnir-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-31 20:21:06.000000 gungnir-0.2.2/tests/test_project.py
```

### Comparing `gungnir-0.2.1/LICENSE` & `gungnir-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.1/PKG-INFO` & `gungnir-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.1
+Version: 0.2.2
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gungnir-0.2.1/README.md` & `gungnir-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.1/gungnir/dependencytrack/api.py` & `gungnir-0.2.2/gungnir/dependencytrack/api.py`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.1/gungnir/dependencytrack/project.py` & `gungnir-0.2.2/gungnir/dependencytrack/project.py`

 * *Files identical despite different names*

### Comparing `gungnir-0.2.1/gungnir/gungnir.egg-info/PKG-INFO` & `gungnir-0.2.2/gungnir/gungnir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.1
+Version: 0.2.2
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gungnir-0.2.1/pyproject.toml` & `gungnir-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [project]
 name = "gungnir"
-version = "0.2.1"
+version = "0.2.2"
 authors = [{ name = "GeekMasher" }]
 description = "Homelab Automation Bot to Guard your very own Asgard"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "certifi==2023.5.7",
+    "certifi==2023.7.22",
     "charset-normalizer==3.2.0",
     "docker==6.1.3",
     "idna==3.4",
     "packaging==23.1",
     "requests==2.31.0",
-    "urllib3==2.0.3",
+    "urllib3==2.0.4",
     "websocket-client==1.6.1",
 ]
 
 [tool.setuptools.packages.find]
 where = ["gungnir"]
 
 [project.urls]
```

