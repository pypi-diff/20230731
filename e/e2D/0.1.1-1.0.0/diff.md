# Comparing `tmp/e2D-0.1.1.tar.gz` & `tmp/e2D-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-0.1.1.tar", last modified: Mon Jul 31 17:12:11 2023, max compression
+gzip compressed data, was "e2D-1.0.0.tar", last modified: Mon Jul 31 17:16:07 2023, max compression
```

## Comparing `e2D-0.1.1.tar` & `e2D-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.969078 e2D-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3081 2023-07-31 17:12:11.969078 e2D-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2488 2023-07-31 16:30:45.000000 e2D-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.949453 e2D-0.1.1/e2D/
--rw-rw-rw-   0        0        0    39663 2023-07-31 16:41:56.000000 e2D-0.1.1/e2D/__init__.py
--rw-rw-rw-   0        0        0    10427 2023-07-31 17:10:49.000000 e2D-0.1.1/e2D/envs.py
--rw-rw-rw-   0        0        0     3918 2023-07-31 17:10:43.000000 e2D-0.1.1/e2D/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-31 17:12:11.969078 e2D-0.1.1/e2D.egg-info/
--rw-rw-rw-   0        0        0     3081 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 17:12:11.000000 e2D-0.1.1/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-07-31 17:12:11.969078 e2D-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 17:16:07.436755 e2D-1.0.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3081 2023-07-31 17:16:07.436755 e2D-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2488 2023-07-31 16:30:45.000000 e2D-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 17:16:07.413511 e2D-1.0.0/e2D/
+-rw-rw-rw-   0        0        0    39663 2023-07-31 16:41:56.000000 e2D-1.0.0/e2D/__init__.py
+-rw-rw-rw-   0        0        0    10427 2023-07-31 17:10:49.000000 e2D-1.0.0/e2D/envs.py
+-rw-rw-rw-   0        0        0     3918 2023-07-31 17:10:43.000000 e2D-1.0.0/e2D/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-31 17:16:07.434204 e2D-1.0.0/e2D.egg-info/
+-rw-rw-rw-   0        0        0     3081 2023-07-31 17:16:07.000000 e2D-1.0.0/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-07-31 17:16:07.000000 e2D-1.0.0/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 17:16:07.000000 e2D-1.0.0/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-31 17:16:07.000000 e2D-1.0.0/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 17:16:07.000000 e2D-1.0.0/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-07-31 17:16:07.438222 e2D-1.0.0/setup.cfg
```

### Comparing `e2D-0.1.1/LICENSE` & `e2D-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-0.1.1/PKG-INFO` & `e2D-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.1.1
+Version: 1.0.0
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.1.1/README.md` & `e2D-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `e2D-0.1.1/e2D/__init__.py` & `e2D-1.0.0/e2D/__init__.py`

 * *Files identical despite different names*

### Comparing `e2D-0.1.1/e2D/envs.py` & `e2D-1.0.0/e2D/envs.py`

 * *Files identical despite different names*

### Comparing `e2D-0.1.1/e2D/utils.py` & `e2D-1.0.0/e2D/utils.py`

 * *Files identical despite different names*

### Comparing `e2D-0.1.1/e2D.egg-info/PKG-INFO` & `e2D-1.0.0/e2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.1.1
+Version: 1.0.0
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.1.1/setup.cfg` & `e2D-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 302e 312e 310d 0a61 7574 686f 7220  = 0.1.1..author 
+00000020: 3d20 312e 302e 300d 0a61 7574 686f 7220  = 1.0.0..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

