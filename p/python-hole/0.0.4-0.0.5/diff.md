# Comparing `tmp/python-hole-0.0.4.tar.gz` & `tmp/python-hole-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hole-0.0.4.tar", last modified: Mon Jul 31 14:07:24 2023, max compression
+gzip compressed data, was "python-hole-0.0.5.tar", last modified: Mon Jul 31 14:16:10 2023, max compression
```

## Comparing `python-hole-0.0.4.tar` & `python-hole-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/
--rw-rw-r--   0 julien    (1001) julien    (1001)     1070 2023-06-21 07:56:44.000000 python-hole-0.0.4/LICENSE
--rw-rw-r--   0 julien    (1001) julien    (1001)      282 2023-07-31 14:07:24.616885 python-hole-0.0.4/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)     6208 2023-07-31 13:40:17.000000 python-hole-0.0.4/README.md
--rw-rw-r--   0 julien    (1001) julien    (1001)      742 2023-07-31 14:06:34.000000 python-hole-0.0.4/pyproject.toml
--rw-rw-r--   0 julien    (1001) julien    (1001)       79 2023-07-31 14:07:24.616885 python-hole-0.0.4/setup.cfg
--rw-rw-r--   0 julien    (1001) julien    (1001)      379 2023-07-31 14:06:19.000000 python-hole-0.0.4/setup.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/src/
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/src/pyhole/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2543 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/AstWalker.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     9290 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/HoleAST.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     6172 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/Matcher.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     1456 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/PatternMatch.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      601 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/PyHoleErrorListener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      853 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/PyHoleParser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    40290 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/PyHoleVisitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/src/pyhole/antlr/
--rw-rw-r--   0 julien    (1001) julien    (1001)    52568 2023-07-31 13:45:56.000000 python-hole-0.0.4/src/pyhole/antlr/Python3Lexer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    27385 2023-07-31 13:45:56.000000 python-hole-0.0.4/src/pyhole/antlr/Python3Listener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)   339487 2023-07-31 13:45:56.000000 python-hole-0.0.4/src/pyhole/antlr/Python3Parser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    16468 2023-07-31 13:45:56.000000 python-hole-0.0.4/src/pyhole/antlr/Python3Visitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/antlr/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/src/pyhole/visualizer/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2744 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/visualizer/Visualizer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.4/src/pyhole/visualizer/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:07:24.616885 python-hole-0.0.4/src/python_hole.egg-info/
--rw-rw-r--   0 julien    (1001) julien    (1001)      282 2023-07-31 14:07:24.000000 python-hole-0.0.4/src/python_hole.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)      651 2023-07-31 14:07:24.000000 python-hole-0.0.4/src/python_hole.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        1 2023-07-31 14:07:24.000000 python-hole-0.0.4/src/python_hole.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        7 2023-07-31 14:07:24.000000 python-hole-0.0.4/src/python_hole.egg-info/top_level.txt
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     1070 2023-06-21 07:56:44.000000 python-hole-0.0.5/LICENSE
+-rw-rw-r--   0 julien    (1001) julien    (1001)     6523 2023-07-31 14:16:10.372984 python-hole-0.0.5/PKG-INFO
+-rw-rw-r--   0 julien    (1001) julien    (1001)     6208 2023-07-31 13:40:17.000000 python-hole-0.0.5/README.md
+-rw-rw-r--   0 julien    (1001) julien    (1001)       79 2023-07-31 14:16:10.372984 python-hole-0.0.5/setup.cfg
+-rw-rw-r--   0 julien    (1001) julien    (1001)      757 2023-07-31 14:16:08.000000 python-hole-0.0.5/setup.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     2543 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/AstWalker.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)     9290 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/HoleAST.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)     6172 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/Matcher.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)     1456 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PatternMatch.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)      601 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleErrorListener.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)      853 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleParser.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    40290 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleVisitor.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/antlr/
+-rw-rw-r--   0 julien    (1001) julien    (1001)    52568 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Lexer.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    27385 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Listener.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)   339487 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Parser.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    16468 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Visitor.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/antlr/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/visualizer/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     2744 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/visualizer/Visualizer.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/visualizer/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/python_hole.egg-info/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     6523 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1001) julien    (1001)      674 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1001) julien    (1001)        1 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1001) julien    (1001)       59 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1001) julien    (1001)        7 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/top_level.txt
```

### Comparing `python-hole-0.0.4/LICENSE` & `python-hole-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/README.md` & `python-hole-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/AstWalker.py` & `python-hole-0.0.5/src/pyhole/AstWalker.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/HoleAST.py` & `python-hole-0.0.5/src/pyhole/HoleAST.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/Matcher.py` & `python-hole-0.0.5/src/pyhole/Matcher.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/PatternMatch.py` & `python-hole-0.0.5/src/pyhole/PatternMatch.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/PyHoleErrorListener.py` & `python-hole-0.0.5/src/pyhole/PyHoleErrorListener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/PyHoleParser.py` & `python-hole-0.0.5/src/pyhole/PyHoleParser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/PyHoleVisitor.py` & `python-hole-0.0.5/src/pyhole/PyHoleVisitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/antlr/Python3Lexer.py` & `python-hole-0.0.5/src/pyhole/antlr/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/antlr/Python3Listener.py` & `python-hole-0.0.5/src/pyhole/antlr/Python3Listener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/antlr/Python3Parser.py` & `python-hole-0.0.5/src/pyhole/antlr/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/antlr/Python3Visitor.py` & `python-hole-0.0.5/src/pyhole/antlr/Python3Visitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/pyhole/visualizer/Visualizer.py` & `python-hole-0.0.5/src/pyhole/visualizer/Visualizer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.4/src/python_hole.egg-info/SOURCES.txt` & `python-hole-0.0.5/src/python_hole.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 src/pyhole/AstWalker.py
 src/pyhole/HoleAST.py
 src/pyhole/Matcher.py
 src/pyhole/PatternMatch.py
 src/pyhole/PyHoleErrorListener.py
@@ -17,8 +16,9 @@
 src/pyhole/antlr/Python3Visitor.py
 src/pyhole/antlr/__init__.py
 src/pyhole/visualizer/Visualizer.py
 src/pyhole/visualizer/__init__.py
 src/python_hole.egg-info/PKG-INFO
 src/python_hole.egg-info/SOURCES.txt
 src/python_hole.egg-info/dependency_links.txt
+src/python_hole.egg-info/requires.txt
 src/python_hole.egg-info/top_level.txt
```

