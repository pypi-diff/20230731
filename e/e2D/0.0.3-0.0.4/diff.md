# Comparing `tmp/e2D-0.0.3.tar.gz` & `tmp/e2D-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-0.0.3.tar", last modified: Mon Jul 31 16:08:20 2023, max compression
+gzip compressed data, was "e2D-0.0.4.tar", last modified: Mon Jul 31 16:16:23 2023, max compression
```

## Comparing `e2D-0.0.3.tar` & `e2D-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 16:08:20.130431 e2D-0.0.3/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3085 2023-07-31 16:08:20.131436 e2D-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2492 2023-07-31 14:47:36.000000 e2D-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-31 16:08:20.112620 e2D-0.0.3/e2D/
--rw-rw-rw-   0        0        0    49399 2023-07-31 14:52:29.000000 e2D-0.0.3/e2D/__init__.py
--rw-rw-rw-   0        0        0     3899 2023-07-31 14:51:50.000000 e2D-0.0.3/e2D/pg.py
-drwxrwxrwx   0        0        0        0 2023-07-31 16:08:20.129435 e2D-0.0.3/e2D.egg-info/
--rw-rw-rw-   0        0        0     3085 2023-07-31 16:08:20.000000 e2D-0.0.3/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-31 16:08:20.000000 e2D-0.0.3/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 16:08:20.000000 e2D-0.0.3/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-31 16:08:20.000000 e2D-0.0.3/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-31 16:08:20.000000 e2D-0.0.3/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      745 2023-07-31 16:08:20.133423 e2D-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 16:16:23.515781 e2D-0.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3085 2023-07-31 16:16:23.515781 e2D-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2492 2023-07-31 14:47:36.000000 e2D-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:16:23.500130 e2D-0.0.4/e2D/
+-rw-rw-rw-   0        0        0    49399 2023-07-31 14:52:29.000000 e2D-0.0.4/e2D/__init__.py
+-rw-rw-rw-   0        0        0     3899 2023-07-31 14:51:50.000000 e2D-0.0.4/e2D/pg.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:16:23.515781 e2D-0.0.4/e2D.egg-info/
+-rw-rw-rw-   0        0        0     3085 2023-07-31 16:16:23.000000 e2D-0.0.4/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-31 16:16:23.000000 e2D-0.0.4/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:16:23.000000 e2D-0.0.4/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-31 16:16:23.000000 e2D-0.0.4/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-31 16:16:23.000000 e2D-0.0.4/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      745 2023-07-31 16:16:23.531408 e2D-0.0.4/setup.cfg
```

### Comparing `e2D-0.0.3/LICENSE` & `e2D-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-0.0.3/PKG-INFO` & `e2D-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.0.3/README.md` & `e2D-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `e2D-0.0.3/e2D/__init__.py` & `e2D-0.0.4/e2D/__init__.py`

 * *Files identical despite different names*

### Comparing `e2D-0.0.3/e2D/pg.py` & `e2D-0.0.4/e2D/pg.py`

 * *Files identical despite different names*

### Comparing `e2D-0.0.3/e2D.egg-info/PKG-INFO` & `e2D-0.0.4/e2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-0.0.3/setup.cfg` & `e2D-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 302e 302e 330d 0a61 7574 686f 7220  = 0.0.3..author 
+00000020: 3d20 302e 302e 340d 0a61 7574 686f 7220  = 0.0.4..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

