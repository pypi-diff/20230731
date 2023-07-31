# Comparing `tmp/polyrepo-0.1.1.tar.gz` & `tmp/polyrepo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyrepo-0.1.1.tar", last modified: Mon Jul 31 02:10:29 2023, max compression
+gzip compressed data, was "polyrepo-0.1.2.tar", last modified: Mon Jul 31 02:20:16 2023, max compression
```

## Comparing `polyrepo-0.1.1.tar` & `polyrepo-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:10:29.591160 polyrepo-0.1.1/
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-31 02:09:40.000000 polyrepo-0.1.1/.version
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-31 02:10:29.591160 polyrepo-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-07-31 02:10:20.000000 polyrepo-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:10:29.587160 polyrepo-0.1.1/polyrepo/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:10:29.590160 polyrepo-0.1.1/polyrepo/command/
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/command/groups_command.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/command/sync_command.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-31 02:10:20.000000 polyrepo-0.1.1/polyrepo/handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:10:29.589160 polyrepo-0.1.1/polyrepo.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2045 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      479 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-31 02:10:29.000000 polyrepo-0.1.1/polyrepo.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-31 02:10:20.000000 polyrepo-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 02:10:29.591160 polyrepo-0.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:10:29.590160 polyrepo-0.1.1/test/
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-31 02:10:20.000000 polyrepo-0.1.1/test/test_command_groups.py
--rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-31 02:10:20.000000 polyrepo-0.1.1/test/test_command_sync.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-31 02:10:20.000000 polyrepo-0.1.1/test/test_gitlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:20:16.799484 polyrepo-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-31 02:19:25.000000 polyrepo-0.1.2/.version
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-31 02:20:16.799484 polyrepo-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-07-31 02:20:08.000000 polyrepo-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:20:16.796484 polyrepo-0.1.2/polyrepo/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:20:16.798484 polyrepo-0.1.2/polyrepo/command/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/command/groups_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/command/sync_command.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-31 02:20:08.000000 polyrepo-0.1.2/polyrepo/handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:20:16.797484 polyrepo-0.1.2/polyrepo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2045 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-31 02:20:16.000000 polyrepo-0.1.2/polyrepo.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-31 02:20:08.000000 polyrepo-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 02:20:16.799484 polyrepo-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 02:20:16.799484 polyrepo-0.1.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-31 02:20:08.000000 polyrepo-0.1.2/test/test_command_groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     1027 2023-07-31 02:20:08.000000 polyrepo-0.1.2/test/test_command_sync.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-07-31 02:20:08.000000 polyrepo-0.1.2/test/test_gitlab.py
```

### Comparing `polyrepo-0.1.1/PKG-INFO` & `polyrepo-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyrepo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Keep repos organized locally the same as on GitLab
 Author-email: Steampunk Wizard <polyrepo@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 PolyRepo
```

### Comparing `polyrepo-0.1.1/README.md` & `polyrepo-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/polyrepo/command/groups_command.py` & `polyrepo-0.1.2/polyrepo/command/groups_command.py`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/polyrepo/command/sync_command.py` & `polyrepo-0.1.2/polyrepo/command/sync_command.py`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/polyrepo/gitlab.py` & `polyrepo-0.1.2/polyrepo/gitlab.py`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/polyrepo.egg-info/PKG-INFO` & `polyrepo-0.1.2/polyrepo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyrepo
-Version: 0.1.1
+Version: 0.1.2
 Summary: Keep repos organized locally the same as on GitLab
 Author-email: Steampunk Wizard <polyrepo@steampunkwizard.ca>
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 PolyRepo
```

### Comparing `polyrepo-0.1.1/pyproject.toml` & `polyrepo-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     {name = "Steampunk Wizard", email = "polyrepo@steampunkwizard.ca"}
 ]
 description = "Keep repos organized locally the same as on GitLab"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 dependencies = [
-    "wizlib >= 0.8.2",
+    "wizlib >= 0.9.1",
     "requests >= 2.31.0",
     "PyYAML >= 6.0"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.package-dir]
 polyrepo = "polyrepo"
```

### Comparing `polyrepo-0.1.1/test/test_command_groups.py` & `polyrepo-0.1.2/test/test_command_groups.py`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/test/test_command_sync.py` & `polyrepo-0.1.2/test/test_command_sync.py`

 * *Files identical despite different names*

### Comparing `polyrepo-0.1.1/test/test_gitlab.py` & `polyrepo-0.1.2/test/test_gitlab.py`

 * *Files identical despite different names*

