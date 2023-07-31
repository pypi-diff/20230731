# Comparing `tmp/Coquille-1.1.2.tar.gz` & `tmp/Coquille-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Coquille-1.1.2.tar", last modified: Sun Jul 16 09:11:15 2023, max compression
+gzip compressed data, was "Coquille-1.2.0.tar", last modified: Mon Jul 31 13:21:24 2023, max compression
```

## Comparing `Coquille-1.1.2.tar` & `Coquille-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.384041 Coquille-1.1.2/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.1.2/.gitignore
--rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.1.2/LICENSE
--rw-r--r--   0 qexat     (1000) qexat     (1001)     5241 2023-07-16 09:11:15.384041 Coquille-1.1.2/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)     3485 2023-07-16 09:10:18.000000 Coquille-1.1.2/README.md
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.377374 Coquille-1.1.2/examples/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.380708 Coquille-1.1.2/examples/coquille_context/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      437 2023-07-14 10:50:09.000000 Coquille-1.1.2/examples/coquille_context/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    60903 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/coquille_context/screenshot.png
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.380708 Coquille-1.1.2/examples/coquille_write/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      196 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/coquille_write/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    39301 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/coquille_write/screenshot.png
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.380708 Coquille-1.1.2/examples/write/
--rw-r--r--   0 qexat     (1000) qexat     (1001)      406 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/write/__main__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/write/output.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)    75317 2023-07-16 09:02:18.000000 Coquille-1.1.2/examples/write/screenshot.png
--rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-16 09:10:27.000000 Coquille-1.1.2/pyproject.toml
--rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-16 09:11:15.384041 Coquille-1.1.2/setup.cfg
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.377374 Coquille-1.1.2/src/
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.384041 Coquille-1.1.2/src/Coquille.egg-info/
--rw-r--r--   0 qexat     (1000) qexat     (1001)     5241 2023-07-16 09:11:15.000000 Coquille-1.1.2/src/Coquille.egg-info/PKG-INFO
--rw-r--r--   0 qexat     (1000) qexat     (1001)      649 2023-07-16 09:11:15.000000 Coquille-1.1.2/src/Coquille.egg-info/SOURCES.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-16 09:11:15.000000 Coquille-1.1.2/src/Coquille.egg-info/dependency_links.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-16 09:11:15.000000 Coquille-1.1.2/src/Coquille.egg-info/requires.txt
--rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-16 09:11:15.000000 Coquille-1.1.2/src/Coquille.egg-info/top_level.txt
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.384041 Coquille-1.1.2/src/coquille/
--rw-r--r--   0 qexat     (1000) qexat     (1001)       32 2023-07-14 10:50:09.000000 Coquille-1.1.2/src/coquille/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     7667 2023-07-16 09:02:18.000000 Coquille-1.1.2/src/coquille/coquille.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)    10596 2023-07-14 10:50:09.000000 Coquille-1.1.2/src/coquille/sequences.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)      392 2023-07-16 08:43:00.000000 Coquille-1.1.2/src/coquille/typeshed.py
-drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-16 09:11:15.384041 Coquille-1.1.2/tests/
--rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.1.2/tests/__init__.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     1081 2023-07-16 08:32:37.000000 Coquille-1.1.2/tests/coquille_test.py
--rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.1.2/tests/sequences_test.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.843366 Coquille-1.2.0/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1813 2023-07-14 10:50:09.000000 Coquille-1.2.0/.gitignore
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      551 2023-07-14 10:50:09.000000 Coquille-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1062 2023-07-14 10:50:09.000000 Coquille-1.2.0/LICENSE
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     5135 2023-07-31 13:21:24.843366 Coquille-1.2.0/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     3379 2023-07-31 13:18:41.000000 Coquille-1.2.0/README.md
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.833366 Coquille-1.2.0/examples/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.836699 Coquille-1.2.0/examples/coquille_context/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      327 2023-07-31 13:17:13.000000 Coquille-1.2.0/examples/coquille_context/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    60903 2023-07-16 09:02:18.000000 Coquille-1.2.0/examples/coquille_context/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.840032 Coquille-1.2.0/examples/coquille_write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      196 2023-07-16 09:02:18.000000 Coquille-1.2.0/examples/coquille_write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    39301 2023-07-16 09:02:18.000000 Coquille-1.2.0/examples/coquille_write/screenshot.png
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.840032 Coquille-1.2.0/examples/write/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      259 2023-07-31 13:17:43.000000 Coquille-1.2.0/examples/write/__main__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       45 2023-07-16 09:02:18.000000 Coquille-1.2.0/examples/write/output.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    75317 2023-07-16 09:02:18.000000 Coquille-1.2.0/examples/write/screenshot.png
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      698 2023-07-31 13:19:31.000000 Coquille-1.2.0/pyproject.toml
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       38 2023-07-31 13:21:24.843366 Coquille-1.2.0/setup.cfg
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.833366 Coquille-1.2.0/src/
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.840032 Coquille-1.2.0/src/Coquille.egg-info/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     5135 2023-07-31 13:21:24.000000 Coquille-1.2.0/src/Coquille.egg-info/PKG-INFO
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      648 2023-07-31 13:21:24.000000 Coquille-1.2.0/src/Coquille.egg-info/SOURCES.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        1 2023-07-31 13:21:24.000000 Coquille-1.2.0/src/Coquille.egg-info/dependency_links.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       35 2023-07-31 13:21:24.000000 Coquille-1.2.0/src/Coquille.egg-info/requires.txt
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        9 2023-07-31 13:21:24.000000 Coquille-1.2.0/src/Coquille.egg-info/top_level.txt
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.843366 Coquille-1.2.0/src/coquille/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)       31 2023-07-31 12:33:33.000000 Coquille-1.2.0/src/coquille/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     8135 2023-07-31 13:03:13.000000 Coquille-1.2.0/src/coquille/prelude.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)    10957 2023-07-31 13:16:57.000000 Coquille-1.2.0/src/coquille/sequences.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)      392 2023-07-16 08:43:00.000000 Coquille-1.2.0/src/coquille/typeshed.py
+drwxr-xr-x   0 qexat     (1000) qexat     (1001)        0 2023-07-31 13:21:24.843366 Coquille-1.2.0/tests/
+-rw-r--r--   0 qexat     (1000) qexat     (1001)        0 2023-07-14 10:50:09.000000 Coquille-1.2.0/tests/__init__.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     1191 2023-07-31 13:06:44.000000 Coquille-1.2.0/tests/coquille_test.py
+-rw-r--r--   0 qexat     (1000) qexat     (1001)     4219 2023-07-14 10:50:09.000000 Coquille-1.2.0/tests/sequences_test.py
```

### Comparing `Coquille-1.1.2/.gitignore` & `Coquille-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/.pre-commit-config.yaml` & `Coquille-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/LICENSE` & `Coquille-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/PKG-INFO` & `Coquille-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.1.2
+Version: 1.2.0
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,43 +54,42 @@
 
 Even though the examples are mostly showcasing [SGR escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) (because they are pretty visible), Coquille can do more! See the [documentation](#documentation).
 
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
-from coquille.sequences import bold, fg_magenta, italic
 
 print("Hello World!")
 
 # By default, the coquille wraps the standard output
-with Coquille.new(fg_magenta, italic) as coquille:
+with Coquille.new("fg_magenta", "italic") as coquille:
     print("Hello World, but in magenta and italic!")
-    coquille.apply(bold)
+    coquille.apply("bold")
     print("Now, with a touch of bold :D")
 
 print("Oh, we are back to normal now...")
+
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
 ### write()
 
 ```py
 from coquille import write
-from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", "fg_magenta", "italic")
 
 with open("examples/write/output.txt", "w") as my_file:
-    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+    write("A pretty Hello World in a file!", "fg_blue", "bold", file=my_file)
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
 
 Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
```

### Comparing `Coquille-1.1.2/README.md` & `Coquille-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,43 +17,42 @@
 
 Even though the examples are mostly showcasing [SGR escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) (because they are pretty visible), Coquille can do more! See the [documentation](#documentation).
 
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
-from coquille.sequences import bold, fg_magenta, italic
 
 print("Hello World!")
 
 # By default, the coquille wraps the standard output
-with Coquille.new(fg_magenta, italic) as coquille:
+with Coquille.new("fg_magenta", "italic") as coquille:
     print("Hello World, but in magenta and italic!")
-    coquille.apply(bold)
+    coquille.apply("bold")
     print("Now, with a touch of bold :D")
 
 print("Oh, we are back to normal now...")
+
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
 ### write()
 
 ```py
 from coquille import write
-from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", "fg_magenta", "italic")
 
 with open("examples/write/output.txt", "w") as my_file:
-    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+    write("A pretty Hello World in a file!", "fg_blue", "bold", file=my_file)
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
 
 Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
```

### Comparing `Coquille-1.1.2/examples/coquille_context/screenshot.png` & `Coquille-1.2.0/examples/coquille_context/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/examples/coquille_write/screenshot.png` & `Coquille-1.2.0/examples/coquille_write/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/examples/write/screenshot.png` & `Coquille-1.2.0/examples/write/screenshot.png`

 * *Files identical despite different names*

### Comparing `Coquille-1.1.2/pyproject.toml` & `Coquille-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Coquille"
-version = "1.1.2"
+version = "1.2.0"
 authors = [{ name = "Qexat" }]
 description = "Coquille is a library that wraps terminal escape sequences as convenient functions."
 readme = "README.md"
 requires-python = ">=3.9"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `Coquille-1.1.2/src/Coquille.egg-info/PKG-INFO` & `Coquille-1.2.0/src/Coquille.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Coquille
-Version: 1.1.2
+Version: 1.2.0
 Summary: Coquille is a library that wraps terminal escape sequences as convenient functions.
 Author: Qexat
 License: MIT License
         
         Copyright (c) 2023 Qexat
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,43 +54,42 @@
 
 Even though the examples are mostly showcasing [SGR escape sequences](https://en.wikipedia.org/wiki/ANSI_escape_code#SGR_(Select_Graphic_Rendition)_parameters) (because they are pretty visible), Coquille can do more! See the [documentation](#documentation).
 
 ### Coquille context manager
 
 ```py
 from coquille import Coquille
-from coquille.sequences import bold, fg_magenta, italic
 
 print("Hello World!")
 
 # By default, the coquille wraps the standard output
-with Coquille.new(fg_magenta, italic) as coquille:
+with Coquille.new("fg_magenta", "italic") as coquille:
     print("Hello World, but in magenta and italic!")
-    coquille.apply(bold)
+    coquille.apply("bold")
     print("Now, with a touch of bold :D")
 
 print("Oh, we are back to normal now...")
+
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/coquille_context/screenshot.png)
 
 Source code: [examples/coquille_context/](https://github.com/qexat/Coquille/blob/main/examples/coquille_context/__main__.py)
 
 ### write()
 
 ```py
 from coquille import write
-from coquille.sequences import bold, fg_blue, fg_magenta, italic
 
 print("Hello World!")
 
-write("Hello World, but in magenta and italic!", fg_magenta, italic)
+write("Hello World, but in magenta and italic!", "fg_magenta", "italic")
 
 with open("examples/write/output.txt", "w") as my_file:
-    write("A pretty Hello World in a file!", fg_blue, bold, file=my_file)
+    write("A pretty Hello World in a file!", "fg_blue", "bold", file=my_file)
 
 ```
 
 ![screenshot.png](https://raw.githubusercontent.com/qexat/Coquille/main/examples/write/screenshot.png)
 
 Source code: [examples/write/](https://github.com/qexat/Coquille/blob/main/examples/write/__main__.py)
```

### Comparing `Coquille-1.1.2/src/Coquille.egg-info/SOURCES.txt` & `Coquille-1.2.0/src/Coquille.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 examples/write/screenshot.png
 src/Coquille.egg-info/PKG-INFO
 src/Coquille.egg-info/SOURCES.txt
 src/Coquille.egg-info/dependency_links.txt
 src/Coquille.egg-info/requires.txt
 src/Coquille.egg-info/top_level.txt
 src/coquille/__init__.py
-src/coquille/coquille.py
+src/coquille/prelude.py
 src/coquille/sequences.py
 src/coquille/typeshed.py
 tests/__init__.py
 tests/coquille_test.py
 tests/sequences_test.py
```

### Comparing `Coquille-1.1.2/src/coquille/coquille.py` & `Coquille-1.2.0/src/coquille/prelude.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,64 +6,78 @@
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import overload
 from typing import Protocol
 from typing import TYPE_CHECKING
 
 from coquille.sequences import EscapeSequence
+from coquille.sequences import EscapeSequenceName
+from coquille.sequences import get_sequence_from_name
 from coquille.sequences import soft_reset
 
-__all__ = ["apply", "Coquille", "EscapeSequence", "prepare", "write"]
+__all__ = [
+    "apply",
+    "Coquille",
+    "EscapeSequence",
+    "EscapeSequenceName",
+    "prepare",
+    "write",
+]
+
 
 # ... don't say anything.
 if TYPE_CHECKING:  # pragma: no cover
     if sys.version_info >= (3, 10):
         from typing import ParamSpec
 
         P = ParamSpec("P")
 
     from coquille.typeshed import Self
     from coquille.typeshed import SupportsWrite
 
 
 @overload
-def prepare(sequence: EscapeSequence) -> EscapeSequence:  # pragma: no cover
+def prepare(
+    sequence: EscapeSequence | EscapeSequenceName,
+) -> EscapeSequence:  # pragma: no cover
     pass
 
 
 @overload
 def prepare(
     sequence: Callable[P, EscapeSequence],
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> EscapeSequence:  # pragma: no cover
     pass
 
 
 def prepare(
-    sequence: EscapeSequence | Callable[P, EscapeSequence],
+    sequence: EscapeSequence | EscapeSequenceName | Callable[P, EscapeSequence],
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> EscapeSequence:
     """
     Prepare an escape sequence.
 
     If `sequence` is already one, it is returned ; else, it passes
     the arguments to the escape sequence factory to construct one.
     """
 
-    if isinstance(sequence, str):
+    if isinstance(sequence, EscapeSequence):
         return sequence
+    elif isinstance(sequence, str):
+        return get_sequence_from_name(sequence)
 
     return sequence(*args, **kwargs)
 
 
 @overload
 def apply(
-    sequence: EscapeSequence,
+    sequence: EscapeSequence | EscapeSequenceName,
     file: SupportsWrite[str] | None = None,
 ) -> None:  # pragma: no cover
     pass
 
 
 @overload
 def apply(
@@ -72,15 +86,15 @@
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> None:  # pragma: no cover
     pass
 
 
 def apply(
-    sequence: EscapeSequence | Callable[P, EscapeSequence],
+    sequence: EscapeSequence | EscapeSequenceName | Callable[P, EscapeSequence],
     file: SupportsWrite[str] | None = None,
     *args: P.args,
     **kwargs: P.kwargs,
 ) -> None:
     """
     Apply an escape sequence to a stream (by default, stdout).
     """
@@ -105,15 +119,15 @@
 
 
 @dataclass(slots=True)
 class _ContextCoquille:
     sequences: list[EscapeSequence]
     file: SupportsWrite[str] | None
 
-    def apply(self, sequence: EscapeSequence) -> None:
+    def apply(self, sequence: EscapeSequence | EscapeSequenceName) -> None:
         """
         Apply an escape sequence in the context manager of a Coquille
         in live.
 
         It is not added to the base `coquille.sequences`, but will still
         be reset at the end of the block.
         """
@@ -151,30 +165,33 @@
 @dataclass(slots=True)
 class Coquille:
     sequences: list[EscapeSequence]
     file: SupportsWrite[str] | None
 
     @overload
     @classmethod
-    def new(cls: type[Self], *sequences: EscapeSequence) -> Self:  # pragma: no cover
+    def new(
+        cls: type[Self],
+        *sequences: EscapeSequence | EscapeSequenceName,
+    ) -> Self:  # pragma: no cover
         pass
 
     @overload
     @classmethod
     def new(
         cls: type[Self],
-        *sequences: EscapeSequence,
+        *sequences: EscapeSequence | EscapeSequenceName,
         file: SupportsWrite[str],
     ) -> Self:  # pragma: no cover
         pass
 
     @classmethod
     def new(
         cls: type[Self],
-        *sequences: EscapeSequence,
+        *sequences: EscapeSequence | EscapeSequenceName,
         file: SupportsWrite[str] | None = None,
     ) -> Self:
         """
         Convenient constructor for a Coquille.
         """
 
         return cls(list(sequences), file)
@@ -260,15 +277,15 @@
         """
 
         apply(soft_reset, self.file)
 
 
 def write(
     text: str,
-    *sequences: EscapeSequence,
+    *sequences: EscapeSequence | EscapeSequenceName,
     end: str | None = "\n",
     file: SupportsWrite[str] | None = None,
 ) -> None:
     """
     A function relatively similar to built-in `print`, but with
     support of escape sequences that are prepended to the printed
     text.
```

### Comparing `Coquille-1.1.2/src/coquille/sequences.py` & `Coquille-1.2.0/src/coquille/sequences.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 ## Bracket notation
 
 - [U] = the abbreviation was made up for convenience.
 - [RS] = rarely (never, basically) supported.
 """
 from typing import Literal
-from typing import NewType
 
 
 # Constants
 
 CHAR_ESC = "\u001b"
 
 CURSOR_VISIBILITY = 25
@@ -35,18 +34,22 @@
 FOREGROUND_CODE = 30
 BACKGROUND_CODE = 40
 UNDERLINE_CODE = 50
 RESET = 9
 
 
 # Helper types
-EscapeSequence = NewType("EscapeSequence", str)
+EscapeSequenceName = str
 AltFontNumber = Literal[1, 2, 3, 4, 5, 6, 7, 8, 9]
 
 
+class EscapeSequence(str):
+    pass
+
+
 def escape_sequence(
     code: str,
     subcode: str | None = None,
     *args: int,
 ) -> EscapeSequence:
     r"""
     Generate an escape sequence string.
@@ -457,7 +460,22 @@
 # *- Extensions -* #
 
 soft_reset = ESC("[!", "p")
 
 
 # aliases
 DECSTR = soft_reset
+
+
+def get_sequence_from_name(name: str) -> EscapeSequence:
+    module_items = dict(globals())
+    sequence_error = ValueError(f"{name!r} is not a valid escape sequence name")
+
+    if name not in module_items:
+        raise sequence_error
+
+    sequence = module_items[name]
+
+    if not isinstance(sequence, EscapeSequence):
+        raise sequence_error
+
+    return sequence
```

### Comparing `Coquille-1.1.2/tests/coquille_test.py` & `Coquille-1.2.0/tests/coquille_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,38 @@
+import pytest
 from io import StringIO
 
-import pytest
-from coquille.coquille import *
+from coquille.prelude import *
 from coquille.sequences import DEC_save_cursor
 from coquille.sequences import erase_in_display
+from coquille.sequences import fg_black
 from coquille.sequences import select_graphical_rendition
 from coquille.sequences import start_of_string
 
 
 @pytest.mark.parametrize(
     ["args", "output"],
     [
         ((DEC_save_cursor,), DEC_save_cursor),
+        (("fg_black",), fg_black),
         ((start_of_string,), "\u001bX"),
         ((erase_in_display, 2), "\u001b[2J"),
         ((select_graphical_rendition, 38, 5, 16), "\x1b[38;5;16m"),
     ],
 )
 def test_prepare(args, output):
     assert prepare(*args) == output
 
 
 @pytest.mark.parametrize(
     ["sequence", "args", "output"],
     [
         (DEC_save_cursor, (), DEC_save_cursor),
         (start_of_string, (), "\u001bX"),
+        ("fg_black", (), fg_black),
         (erase_in_display, (2,), "\u001b[2J"),
         (select_graphical_rendition, (38, 5, 16), "\x1b[38;5;16m"),
     ],
 )
 def test_apply(sequence, args, output):
     file = StringIO()
     apply(sequence, file, *args)
```

### Comparing `Coquille-1.1.2/tests/sequences_test.py` & `Coquille-1.2.0/tests/sequences_test.py`

 * *Files identical despite different names*

