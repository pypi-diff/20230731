# Comparing `tmp/python-hole-0.0.2.tar.gz` & `tmp/python-hole-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hole-0.0.2.tar", last modified: Mon Jul 31 13:18:55 2023, max compression
+gzip compressed data, was "python-hole-0.0.3.tar", last modified: Mon Jul 31 13:21:04 2023, max compression
```

## Comparing `python-hole-0.0.2.tar` & `python-hole-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.068118 python-hole-0.0.2/
--rw-rw-r--   0 julien    (1001) julien    (1001)     1070 2023-06-21 07:56:44.000000 python-hole-0.0.2/LICENSE
--rw-rw-r--   0 julien    (1001) julien    (1001)      225 2023-07-31 13:18:55.068118 python-hole-0.0.2/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)     6208 2023-07-31 12:49:54.000000 python-hole-0.0.2/README.md
--rw-rw-r--   0 julien    (1001) julien    (1001)      616 2023-07-31 12:10:55.000000 python-hole-0.0.2/pyproject.toml
--rw-rw-r--   0 julien    (1001) julien    (1001)       38 2023-07-31 13:18:55.068118 python-hole-0.0.2/setup.cfg
--rw-rw-r--   0 julien    (1001) julien    (1001)      315 2023-07-31 13:14:19.000000 python-hole-0.0.2/setup.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.064118 python-hole-0.0.2/src/
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.064118 python-hole-0.0.2/src/pyhole/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2543 2023-06-21 08:13:50.000000 python-hole-0.0.2/src/pyhole/AstWalker.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     9290 2023-07-26 08:26:03.000000 python-hole-0.0.2/src/pyhole/HoleAST.py
--rw-r--r--   0 julien    (1001) julien    (1001)     6172 2023-07-31 12:58:23.000000 python-hole-0.0.2/src/pyhole/Matcher.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     1456 2023-07-31 13:01:16.000000 python-hole-0.0.2/src/pyhole/PatternMatch.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      601 2023-06-21 11:52:40.000000 python-hole-0.0.2/src/pyhole/PyHoleErrorListener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      853 2023-06-21 11:52:56.000000 python-hole-0.0.2/src/pyhole/PyHoleParser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    40290 2023-06-21 12:19:25.000000 python-hole-0.0.2/src/pyhole/PyHoleVisitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-02-24 09:46:45.000000 python-hole-0.0.2/src/pyhole/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.068118 python-hole-0.0.2/src/pyhole/antlr/
--rw-rw-r--   0 julien    (1001) julien    (1001)    52568 2023-07-31 13:03:11.000000 python-hole-0.0.2/src/pyhole/antlr/Python3Lexer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    27385 2023-07-31 13:03:11.000000 python-hole-0.0.2/src/pyhole/antlr/Python3Listener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)   339487 2023-07-31 13:03:11.000000 python-hole-0.0.2/src/pyhole/antlr/Python3Parser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    16468 2023-07-31 13:03:11.000000 python-hole-0.0.2/src/pyhole/antlr/Python3Visitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-02-24 09:53:34.000000 python-hole-0.0.2/src/pyhole/antlr/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.068118 python-hole-0.0.2/src/pyhole/visualizer/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2744 2023-07-31 13:01:44.000000 python-hole-0.0.2/src/pyhole/visualizer/Visualizer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-04-26 13:22:46.000000 python-hole-0.0.2/src/pyhole/visualizer/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:18:55.068118 python-hole-0.0.2/src/python_hole.egg-info/
--rw-rw-r--   0 julien    (1001) julien    (1001)      225 2023-07-31 13:18:55.000000 python-hole-0.0.2/src/python_hole.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)      641 2023-07-31 13:18:55.000000 python-hole-0.0.2/src/python_hole.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        1 2023-07-31 13:18:55.000000 python-hole-0.0.2/src/python_hole.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        7 2023-07-31 13:18:55.000000 python-hole-0.0.2/src/python_hole.egg-info/top_level.txt
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     1070 2023-06-21 07:56:44.000000 python-hole-0.0.3/LICENSE
+-rw-rw-r--   0 julien    (1001) julien    (1001)      225 2023-07-31 13:21:04.522018 python-hole-0.0.3/PKG-INFO
+-rw-rw-r--   0 julien    (1001) julien    (1001)     6208 2023-07-31 12:49:54.000000 python-hole-0.0.3/README.md
+-rw-rw-r--   0 julien    (1001) julien    (1001)      616 2023-07-31 12:10:55.000000 python-hole-0.0.3/pyproject.toml
+-rw-rw-r--   0 julien    (1001) julien    (1001)       79 2023-07-31 13:21:04.522018 python-hole-0.0.3/setup.cfg
+-rw-rw-r--   0 julien    (1001) julien    (1001)      315 2023-07-31 13:21:03.000000 python-hole-0.0.3/setup.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/src/
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/src/pyhole/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     2543 2023-06-21 08:13:50.000000 python-hole-0.0.3/src/pyhole/AstWalker.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)     9290 2023-07-26 08:26:03.000000 python-hole-0.0.3/src/pyhole/HoleAST.py
+-rw-r--r--   0 julien    (1001) julien    (1001)     6172 2023-07-31 12:58:23.000000 python-hole-0.0.3/src/pyhole/Matcher.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)     1456 2023-07-31 13:01:16.000000 python-hole-0.0.3/src/pyhole/PatternMatch.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)      601 2023-06-21 11:52:40.000000 python-hole-0.0.3/src/pyhole/PyHoleErrorListener.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)      853 2023-06-21 11:52:56.000000 python-hole-0.0.3/src/pyhole/PyHoleParser.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    40290 2023-06-21 12:19:25.000000 python-hole-0.0.3/src/pyhole/PyHoleVisitor.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-02-24 09:46:45.000000 python-hole-0.0.3/src/pyhole/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/src/pyhole/antlr/
+-rw-rw-r--   0 julien    (1001) julien    (1001)    52568 2023-07-31 13:03:11.000000 python-hole-0.0.3/src/pyhole/antlr/Python3Lexer.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    27385 2023-07-31 13:03:11.000000 python-hole-0.0.3/src/pyhole/antlr/Python3Listener.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)   339487 2023-07-31 13:03:11.000000 python-hole-0.0.3/src/pyhole/antlr/Python3Parser.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)    16468 2023-07-31 13:03:11.000000 python-hole-0.0.3/src/pyhole/antlr/Python3Visitor.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-02-24 09:53:34.000000 python-hole-0.0.3/src/pyhole/antlr/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/src/pyhole/visualizer/
+-rw-rw-r--   0 julien    (1001) julien    (1001)     2744 2023-07-31 13:01:44.000000 python-hole-0.0.3/src/pyhole/visualizer/Visualizer.py
+-rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-04-26 13:22:46.000000 python-hole-0.0.3/src/pyhole/visualizer/__init__.py
+drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 13:21:04.522018 python-hole-0.0.3/src/python_hole.egg-info/
+-rw-rw-r--   0 julien    (1001) julien    (1001)      225 2023-07-31 13:21:04.000000 python-hole-0.0.3/src/python_hole.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1001) julien    (1001)      651 2023-07-31 13:21:04.000000 python-hole-0.0.3/src/python_hole.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1001) julien    (1001)        1 2023-07-31 13:21:04.000000 python-hole-0.0.3/src/python_hole.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1001) julien    (1001)        7 2023-07-31 13:21:04.000000 python-hole-0.0.3/src/python_hole.egg-info/top_level.txt
```

### Comparing `python-hole-0.0.2/LICENSE` & `python-hole-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/README.md` & `python-hole-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/pyproject.toml` & `python-hole-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/AstWalker.py` & `python-hole-0.0.3/src/pyhole/AstWalker.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/HoleAST.py` & `python-hole-0.0.3/src/pyhole/HoleAST.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/Matcher.py` & `python-hole-0.0.3/src/pyhole/Matcher.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/PatternMatch.py` & `python-hole-0.0.3/src/pyhole/PatternMatch.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/PyHoleErrorListener.py` & `python-hole-0.0.3/src/pyhole/PyHoleErrorListener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/PyHoleParser.py` & `python-hole-0.0.3/src/pyhole/PyHoleParser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/PyHoleVisitor.py` & `python-hole-0.0.3/src/pyhole/PyHoleVisitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/antlr/Python3Lexer.py` & `python-hole-0.0.3/src/pyhole/antlr/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/antlr/Python3Listener.py` & `python-hole-0.0.3/src/pyhole/antlr/Python3Listener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/antlr/Python3Parser.py` & `python-hole-0.0.3/src/pyhole/antlr/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/antlr/Python3Visitor.py` & `python-hole-0.0.3/src/pyhole/antlr/Python3Visitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/pyhole/visualizer/Visualizer.py` & `python-hole-0.0.3/src/pyhole/visualizer/Visualizer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.2/src/python_hole.egg-info/SOURCES.txt` & `python-hole-0.0.3/src/python_hole.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 setup.py
 src/pyhole/AstWalker.py
 src/pyhole/HoleAST.py
 src/pyhole/Matcher.py
 src/pyhole/PatternMatch.py
 src/pyhole/PyHoleErrorListener.py
 src/pyhole/PyHoleParser.py
```

