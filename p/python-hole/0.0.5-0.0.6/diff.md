# Comparing `tmp/python-hole-0.0.5.tar.gz` & `tmp/python-hole-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-hole-0.0.5.tar", last modified: Mon Jul 31 14:16:10 2023, max compression
+gzip compressed data, was "python-hole-0.0.6.tar", last modified: Mon Jul 31 14:37:51 2023, max compression
```

## Comparing `python-hole-0.0.5.tar` & `python-hole-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/
--rw-rw-r--   0 julien    (1001) julien    (1001)     1070 2023-06-21 07:56:44.000000 python-hole-0.0.5/LICENSE
--rw-rw-r--   0 julien    (1001) julien    (1001)     6523 2023-07-31 14:16:10.372984 python-hole-0.0.5/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)     6208 2023-07-31 13:40:17.000000 python-hole-0.0.5/README.md
--rw-rw-r--   0 julien    (1001) julien    (1001)       79 2023-07-31 14:16:10.372984 python-hole-0.0.5/setup.cfg
--rw-rw-r--   0 julien    (1001) julien    (1001)      757 2023-07-31 14:16:08.000000 python-hole-0.0.5/setup.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2543 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/AstWalker.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     9290 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/HoleAST.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     6172 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/Matcher.py
--rw-rw-r--   0 julien    (1001) julien    (1001)     1456 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PatternMatch.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      601 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleErrorListener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)      853 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleParser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    40290 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/PyHoleVisitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/antlr/
--rw-rw-r--   0 julien    (1001) julien    (1001)    52568 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Lexer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    27385 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Listener.py
--rw-rw-r--   0 julien    (1001) julien    (1001)   339487 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Parser.py
--rw-rw-r--   0 julien    (1001) julien    (1001)    16468 2023-07-31 13:45:56.000000 python-hole-0.0.5/src/pyhole/antlr/Python3Visitor.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/antlr/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/pyhole/visualizer/
--rw-rw-r--   0 julien    (1001) julien    (1001)     2744 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/visualizer/Visualizer.py
--rw-rw-r--   0 julien    (1001) julien    (1001)        0 2023-07-31 13:40:17.000000 python-hole-0.0.5/src/pyhole/visualizer/__init__.py
-drwxrwxr-x   0 julien    (1001) julien    (1001)        0 2023-07-31 14:16:10.372984 python-hole-0.0.5/src/python_hole.egg-info/
--rw-rw-r--   0 julien    (1001) julien    (1001)     6523 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1001) julien    (1001)      674 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        1 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)       59 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/requires.txt
--rw-rw-r--   0 julien    (1001) julien    (1001)        7 2023-07-31 14:16:10.000000 python-hole-0.0.5/src/python_hole.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 14:37:45.000000 python-hole-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-31 14:37:51.764876 python-hole-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-31 14:37:45.000000 python-hole-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:37:51.764876 python-hole-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-31 14:37:45.000000 python-hole-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.756876 python-hole-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.760877 python-hole-0.0.6/src/pyhole/
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/AstWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/HoleAST.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/Matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PatternMatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleErrorListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40290 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/PyHoleVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/pyhole/antlr/
+-rw-r--r--   0 runner    (1001) docker     (123)    52568 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27385 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   339487 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/Python3Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/antlr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/pyhole/visualizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/visualizer/Visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:45.000000 python-hole-0.0.6/src/pyhole/visualizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:37:51.764876 python-hole-0.0.6/src/python_hole.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-31 14:37:51.000000 python-hole-0.0.6/src/python_hole.egg-info/top_level.txt
```

### Comparing `python-hole-0.0.5/LICENSE` & `python-hole-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/PKG-INFO` & `python-hole-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: python-hole
-Version: 0.0.5
-Summary: Python package to build code patterns
-Home-page: https://github.com/JulienLie/python-hole
-Author: Julien Lienard
-Author-email: julien.lienard@uclouvain.be
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Hole
 
 ![Tests Status](https://github.com/JulienLie/python-hole/actions/workflows/python-app.yml/badge.svg?event=push)
 
 Python Hole (or PyHole) is a python library to create patterns file for Python code.
 
 ## Syntax
@@ -158,9 +146,8 @@
 pattern = "pattern_file.py"
 val, match = match_files(pattern, code, strict_match=False, match_details=True)
 
 output_file = "example.html"
 html = Visualizer.match_to_hml(match, code, pattern)
 html.write(output_file)
 ```
-![Visualisation of a match](match.png)
-
+![Visualisation of a match](match.png)
```

### Comparing `python-hole-0.0.5/README.md` & `python-hole-0.0.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,153 +1,163 @@
-# Python Hole
-
-![Tests Status](https://github.com/JulienLie/python-hole/actions/workflows/python-app.yml/badge.svg?event=push)
-
-Python Hole (or PyHole) is a python library to create patterns file for Python code.
-
-## Syntax
-
-We extended the python syntax to create patterns file. Our new syntax include the following elements:
-
-| Wildcard          | Description                                       |
-|-------------------|---------------------------------------------------|
-| ?                 | Match 1 element                                   |
-| ?*                | Match 0 or more elements                          |
-| ?{name}           | Match 1 element and bind it to {``name``}         |
-| ?:                | Match 1 element with a body                       |
-| ?*:               | Match the body of the wildcard in any indentation |
-| ?![<br/>...<br/>] | Use strict match for the body of this wildcard    |
-
-## Usage
-
-```python
-
-import Matcher
-
-code = "code_file.py"
-pattern = "pattern_file.py"
-match = Matcher.match_files(pattern, code, strict_match=False, match_details=False)
-if match:
-    print("We found a match")
-else:
-    print("No match")
-```
-The `match_files` function takes 4 arguments:
-1. `pattern_file: string` The path to the file describing the pattern
-2. `code_file: string` The path to the python code file
-3. `strict_match: boolean` When strict_match is set to True, a strict match is performed. 
-A strict match requires an exact match between the code file and the pattern file, including code structure and syntax. 
-If strict_match is set to False, a "soft" match is performed, which allows for flexibility in code sections using wildcards.
-4. `match_details: boolean` If match_details is set to True, the function returns a tuple (result, details), 
-where result is a boolean value indicating whether the code matches the pattern. 
-If result is True, details contains the match details. If result is False, details contains the error that prevented the match.
-
-
-## Examples
-### Python code:
-```python
-def multiplications(n):
-    """
-    pre:  n is a positive integer
-    post: Return the number of distinct decompositions a,b 
-          such that n == a*b == b*a
-    """
-    b=n
-    a=1
-    c=0
-    while a*b==n:
-        c=a*(b/a)
-        a+=1
-    return c
-```
-### Pattern file:
-#### Soft match
-```python
-def multiplications(n):
-    ?var1 = ?       # We want to have a initial variable
-    ?*:
-        ?var1 = ?   # This variable has to be updated somewhere
-    return ?var1    # And we want to return it
-```
-#### Strict match
-```python
-def multiplications(n):
-    ?*
-    ?var1 = ?       # We want to have a initial variable
-    ?*
-    ?*:
-        ?*
-        ?var1 = ?   # This variable has to be updated somewhere
-        ?*
-    return ?var1    # And we want to return it
-```
-
-Those two piece of codes describes the same patterns. The soft match hide the multiple wildcards `?*` in the strict match.
-
-
-## Strict match / Soft match
-### Main difference
-In a soft match, there is flexibility in code structure and the possibility of including extra code, 
-as long as the main matching criteria are met. In contrast, in a strict match, precise adherence to the defined 
-code structure and syntax is necessary, and there is limited to no allowance for variations or 
-additional code outside of the specified structure.
-
-### The wildcard `?:[]`
-The wildcard `?![]` is a notation that allows for a combination of strict and soft matching in certain parts of a code pattern. It is useful when you want to perform a soft match but have a strict match requirement within a specific section of code.
-
-Let's consider an example to illustrate this. Suppose we have the following pattern:
-
-```python
-def foo(bar):
-    ?var = 0
-    for ? in range(?*):
-        ?![
-        if ?:
-           ?var += 1 
-        ]
-```
-In this pattern, the wildcard ? represents a placeholder for any valid Python identifier. The ?var = 0 statement assigns the value 0 to a variable, which we'll refer to as x. The for ? in range(?*) loop iterates over a range of values, which we'll refer to as y. Finally, ?![ ... ] represents a strict match requirement that enforces certain code within the if statement.
-
-Now, let's say we have the following code snippet:
-
-```python
-def foo(bar):
-    x = 0
-    y = len(bar)
-    for i in range(y):
-        z = bar[i]
-        if z:
-            x += 1
-    return x
-```
-We want to match this code snippet with the given pattern. Let's go through each line and see how the wildcard ?![] allows for matching.
-
-- In the pattern, `?var = 0` matches the code `x = 0` because the wildcard `?var` represents the variable named `x`.
-- The loop statement `for ? in range(?*)` in the pattern matches the code `for i in range(y)`. 
-- Here, `?` corresponds to the loop variable `i`, and `?*` corresponds to the length of the bar list, which is stored in `y`.
-- The strict match requirement `?![ ... ]` checks the code within the if statement. 
-- In the pattern, `?` represents the condition `z`, and `?var += 1` corresponds to `x += 1` within the if block.
-
-As a result, the code snippet matches the pattern because all the placeholders and the strict match requirements are satisfied. 
-However, if we have additional code within the if block, such as a print statement like `print("true")`, 
-the pattern won't match because the strict match requirement `?![ ... ]` doesn't accommodate that extra code.
-
-In summary, the wildcard `?![]` allows for a combination of soft and strict matching. 
-It provides flexibility by allowing soft matches for variables and loop structures while enforcing strict matches for 
-specific code sections. This helps in creating adaptable code patterns that can match similar code snippets with some variations.
-
-## Visualization
-You can visualize the pattern match using the `match_details` argument and the visualiser.
-
-```python
-from src.pyhole import Visualizer
-import Matcher
-
-code = "code_file.py"
-pattern = "pattern_file.py"
-val, match = match_files(pattern, code, strict_match=False, match_details=True)
-
-output_file = "example.html"
-html = Visualizer.match_to_hml(match, code, pattern)
-html.write(output_file)
-```
-![Visualisation of a match](match.png)
+Metadata-Version: 2.1
+Name: python-hole
+Version: 0.0.6
+Summary: Python package to build code patterns
+Home-page: https://github.com/JulienLie/python-hole
+Author: Julien Lienard
+Author-email: julien.lienard@uclouvain.be
+License: MIT
+Description: # Python Hole
+        
+        ![Tests Status](https://github.com/JulienLie/python-hole/actions/workflows/python-app.yml/badge.svg?event=push)
+        
+        Python Hole (or PyHole) is a python library to create patterns file for Python code.
+        
+        ## Syntax
+        
+        We extended the python syntax to create patterns file. Our new syntax include the following elements:
+        
+        | Wildcard          | Description                                       |
+        |-------------------|---------------------------------------------------|
+        | ?                 | Match 1 element                                   |
+        | ?*                | Match 0 or more elements                          |
+        | ?{name}           | Match 1 element and bind it to {``name``}         |
+        | ?:                | Match 1 element with a body                       |
+        | ?*:               | Match the body of the wildcard in any indentation |
+        | ?![<br/>...<br/>] | Use strict match for the body of this wildcard    |
+        
+        ## Usage
+        
+        ```python
+        
+        import Matcher
+        
+        code = "code_file.py"
+        pattern = "pattern_file.py"
+        match = Matcher.match_files(pattern, code, strict_match=False, match_details=False)
+        if match:
+            print("We found a match")
+        else:
+            print("No match")
+        ```
+        The `match_files` function takes 4 arguments:
+        1. `pattern_file: string` The path to the file describing the pattern
+        2. `code_file: string` The path to the python code file
+        3. `strict_match: boolean` When strict_match is set to True, a strict match is performed. 
+        A strict match requires an exact match between the code file and the pattern file, including code structure and syntax. 
+        If strict_match is set to False, a "soft" match is performed, which allows for flexibility in code sections using wildcards.
+        4. `match_details: boolean` If match_details is set to True, the function returns a tuple (result, details), 
+        where result is a boolean value indicating whether the code matches the pattern. 
+        If result is True, details contains the match details. If result is False, details contains the error that prevented the match.
+        
+        
+        ## Examples
+        ### Python code:
+        ```python
+        def multiplications(n):
+            """
+            pre:  n is a positive integer
+            post: Return the number of distinct decompositions a,b 
+                  such that n == a*b == b*a
+            """
+            b=n
+            a=1
+            c=0
+            while a*b==n:
+                c=a*(b/a)
+                a+=1
+            return c
+        ```
+        ### Pattern file:
+        #### Soft match
+        ```python
+        def multiplications(n):
+            ?var1 = ?       # We want to have a initial variable
+            ?*:
+                ?var1 = ?   # This variable has to be updated somewhere
+            return ?var1    # And we want to return it
+        ```
+        #### Strict match
+        ```python
+        def multiplications(n):
+            ?*
+            ?var1 = ?       # We want to have a initial variable
+            ?*
+            ?*:
+                ?*
+                ?var1 = ?   # This variable has to be updated somewhere
+                ?*
+            return ?var1    # And we want to return it
+        ```
+        
+        Those two piece of codes describes the same patterns. The soft match hide the multiple wildcards `?*` in the strict match.
+        
+        
+        ## Strict match / Soft match
+        ### Main difference
+        In a soft match, there is flexibility in code structure and the possibility of including extra code, 
+        as long as the main matching criteria are met. In contrast, in a strict match, precise adherence to the defined 
+        code structure and syntax is necessary, and there is limited to no allowance for variations or 
+        additional code outside of the specified structure.
+        
+        ### The wildcard `?:[]`
+        The wildcard `?![]` is a notation that allows for a combination of strict and soft matching in certain parts of a code pattern. It is useful when you want to perform a soft match but have a strict match requirement within a specific section of code.
+        
+        Let's consider an example to illustrate this. Suppose we have the following pattern:
+        
+        ```python
+        def foo(bar):
+            ?var = 0
+            for ? in range(?*):
+                ?![
+                if ?:
+                   ?var += 1 
+                ]
+        ```
+        In this pattern, the wildcard ? represents a placeholder for any valid Python identifier. The ?var = 0 statement assigns the value 0 to a variable, which we'll refer to as x. The for ? in range(?*) loop iterates over a range of values, which we'll refer to as y. Finally, ?![ ... ] represents a strict match requirement that enforces certain code within the if statement.
+        
+        Now, let's say we have the following code snippet:
+        
+        ```python
+        def foo(bar):
+            x = 0
+            y = len(bar)
+            for i in range(y):
+                z = bar[i]
+                if z:
+                    x += 1
+            return x
+        ```
+        We want to match this code snippet with the given pattern. Let's go through each line and see how the wildcard ?![] allows for matching.
+        
+        - In the pattern, `?var = 0` matches the code `x = 0` because the wildcard `?var` represents the variable named `x`.
+        - The loop statement `for ? in range(?*)` in the pattern matches the code `for i in range(y)`. 
+        - Here, `?` corresponds to the loop variable `i`, and `?*` corresponds to the length of the bar list, which is stored in `y`.
+        - The strict match requirement `?![ ... ]` checks the code within the if statement. 
+        - In the pattern, `?` represents the condition `z`, and `?var += 1` corresponds to `x += 1` within the if block.
+        
+        As a result, the code snippet matches the pattern because all the placeholders and the strict match requirements are satisfied. 
+        However, if we have additional code within the if block, such as a print statement like `print("true")`, 
+        the pattern won't match because the strict match requirement `?![ ... ]` doesn't accommodate that extra code.
+        
+        In summary, the wildcard `?![]` allows for a combination of soft and strict matching. 
+        It provides flexibility by allowing soft matches for variables and loop structures while enforcing strict matches for 
+        specific code sections. This helps in creating adaptable code patterns that can match similar code snippets with some variations.
+        
+        ## Visualization
+        You can visualize the pattern match using the `match_details` argument and the visualiser.
+        
+        ```python
+        from src.pyhole import Visualizer
+        import Matcher
+        
+        code = "code_file.py"
+        pattern = "pattern_file.py"
+        val, match = match_files(pattern, code, strict_match=False, match_details=True)
+        
+        output_file = "example.html"
+        html = Visualizer.match_to_hml(match, code, pattern)
+        html.write(output_file)
+        ```
+        ![Visualisation of a match](match.png)
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `python-hole-0.0.5/setup.py` & `python-hole-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from setuptools import setup
-
 # read the contents of your README file
 from pathlib import Path
+
+from setuptools import setup
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='python-hole',
-    version='0.0.5',
+    version='0.0.6',
     packages=['pyhole', 'pyhole.antlr', 'pyhole.visualizer'],
     package_dir={'': 'src'},
     url='https://github.com/JulienLie/python-hole',
     license='MIT',
     author='Julien Lienard',
     author_email='julien.lienard@uclouvain.be',
     description="Python package to build code patterns",
```

### Comparing `python-hole-0.0.5/src/pyhole/AstWalker.py` & `python-hole-0.0.6/src/pyhole/AstWalker.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/HoleAST.py` & `python-hole-0.0.6/src/pyhole/HoleAST.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/Matcher.py` & `python-hole-0.0.6/src/pyhole/Matcher.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/PatternMatch.py` & `python-hole-0.0.6/src/pyhole/PatternMatch.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/PyHoleErrorListener.py` & `python-hole-0.0.6/src/pyhole/PyHoleErrorListener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/PyHoleParser.py` & `python-hole-0.0.6/src/pyhole/PyHoleParser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/PyHoleVisitor.py` & `python-hole-0.0.6/src/pyhole/PyHoleVisitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/antlr/Python3Lexer.py` & `python-hole-0.0.6/src/pyhole/antlr/Python3Lexer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/antlr/Python3Listener.py` & `python-hole-0.0.6/src/pyhole/antlr/Python3Listener.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/antlr/Python3Parser.py` & `python-hole-0.0.6/src/pyhole/antlr/Python3Parser.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/antlr/Python3Visitor.py` & `python-hole-0.0.6/src/pyhole/antlr/Python3Visitor.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/pyhole/visualizer/Visualizer.py` & `python-hole-0.0.6/src/pyhole/visualizer/Visualizer.py`

 * *Files identical despite different names*

### Comparing `python-hole-0.0.5/src/python_hole.egg-info/PKG-INFO` & `python-hole-0.0.6/src/python_hole.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,163 @@
 Metadata-Version: 2.1
 Name: python-hole
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python package to build code patterns
 Home-page: https://github.com/JulienLie/python-hole
 Author: Julien Lienard
 Author-email: julien.lienard@uclouvain.be
 License: MIT
+Description: # Python Hole
+        
+        ![Tests Status](https://github.com/JulienLie/python-hole/actions/workflows/python-app.yml/badge.svg?event=push)
+        
+        Python Hole (or PyHole) is a python library to create patterns file for Python code.
+        
+        ## Syntax
+        
+        We extended the python syntax to create patterns file. Our new syntax include the following elements:
+        
+        | Wildcard          | Description                                       |
+        |-------------------|---------------------------------------------------|
+        | ?                 | Match 1 element                                   |
+        | ?*                | Match 0 or more elements                          |
+        | ?{name}           | Match 1 element and bind it to {``name``}         |
+        | ?:                | Match 1 element with a body                       |
+        | ?*:               | Match the body of the wildcard in any indentation |
+        | ?![<br/>...<br/>] | Use strict match for the body of this wildcard    |
+        
+        ## Usage
+        
+        ```python
+        
+        import Matcher
+        
+        code = "code_file.py"
+        pattern = "pattern_file.py"
+        match = Matcher.match_files(pattern, code, strict_match=False, match_details=False)
+        if match:
+            print("We found a match")
+        else:
+            print("No match")
+        ```
+        The `match_files` function takes 4 arguments:
+        1. `pattern_file: string` The path to the file describing the pattern
+        2. `code_file: string` The path to the python code file
+        3. `strict_match: boolean` When strict_match is set to True, a strict match is performed. 
+        A strict match requires an exact match between the code file and the pattern file, including code structure and syntax. 
+        If strict_match is set to False, a "soft" match is performed, which allows for flexibility in code sections using wildcards.
+        4. `match_details: boolean` If match_details is set to True, the function returns a tuple (result, details), 
+        where result is a boolean value indicating whether the code matches the pattern. 
+        If result is True, details contains the match details. If result is False, details contains the error that prevented the match.
+        
+        
+        ## Examples
+        ### Python code:
+        ```python
+        def multiplications(n):
+            """
+            pre:  n is a positive integer
+            post: Return the number of distinct decompositions a,b 
+                  such that n == a*b == b*a
+            """
+            b=n
+            a=1
+            c=0
+            while a*b==n:
+                c=a*(b/a)
+                a+=1
+            return c
+        ```
+        ### Pattern file:
+        #### Soft match
+        ```python
+        def multiplications(n):
+            ?var1 = ?       # We want to have a initial variable
+            ?*:
+                ?var1 = ?   # This variable has to be updated somewhere
+            return ?var1    # And we want to return it
+        ```
+        #### Strict match
+        ```python
+        def multiplications(n):
+            ?*
+            ?var1 = ?       # We want to have a initial variable
+            ?*
+            ?*:
+                ?*
+                ?var1 = ?   # This variable has to be updated somewhere
+                ?*
+            return ?var1    # And we want to return it
+        ```
+        
+        Those two piece of codes describes the same patterns. The soft match hide the multiple wildcards `?*` in the strict match.
+        
+        
+        ## Strict match / Soft match
+        ### Main difference
+        In a soft match, there is flexibility in code structure and the possibility of including extra code, 
+        as long as the main matching criteria are met. In contrast, in a strict match, precise adherence to the defined 
+        code structure and syntax is necessary, and there is limited to no allowance for variations or 
+        additional code outside of the specified structure.
+        
+        ### The wildcard `?:[]`
+        The wildcard `?![]` is a notation that allows for a combination of strict and soft matching in certain parts of a code pattern. It is useful when you want to perform a soft match but have a strict match requirement within a specific section of code.
+        
+        Let's consider an example to illustrate this. Suppose we have the following pattern:
+        
+        ```python
+        def foo(bar):
+            ?var = 0
+            for ? in range(?*):
+                ?![
+                if ?:
+                   ?var += 1 
+                ]
+        ```
+        In this pattern, the wildcard ? represents a placeholder for any valid Python identifier. The ?var = 0 statement assigns the value 0 to a variable, which we'll refer to as x. The for ? in range(?*) loop iterates over a range of values, which we'll refer to as y. Finally, ?![ ... ] represents a strict match requirement that enforces certain code within the if statement.
+        
+        Now, let's say we have the following code snippet:
+        
+        ```python
+        def foo(bar):
+            x = 0
+            y = len(bar)
+            for i in range(y):
+                z = bar[i]
+                if z:
+                    x += 1
+            return x
+        ```
+        We want to match this code snippet with the given pattern. Let's go through each line and see how the wildcard ?![] allows for matching.
+        
+        - In the pattern, `?var = 0` matches the code `x = 0` because the wildcard `?var` represents the variable named `x`.
+        - The loop statement `for ? in range(?*)` in the pattern matches the code `for i in range(y)`. 
+        - Here, `?` corresponds to the loop variable `i`, and `?*` corresponds to the length of the bar list, which is stored in `y`.
+        - The strict match requirement `?![ ... ]` checks the code within the if statement. 
+        - In the pattern, `?` represents the condition `z`, and `?var += 1` corresponds to `x += 1` within the if block.
+        
+        As a result, the code snippet matches the pattern because all the placeholders and the strict match requirements are satisfied. 
+        However, if we have additional code within the if block, such as a print statement like `print("true")`, 
+        the pattern won't match because the strict match requirement `?![ ... ]` doesn't accommodate that extra code.
+        
+        In summary, the wildcard `?![]` allows for a combination of soft and strict matching. 
+        It provides flexibility by allowing soft matches for variables and loop structures while enforcing strict matches for 
+        specific code sections. This helps in creating adaptable code patterns that can match similar code snippets with some variations.
+        
+        ## Visualization
+        You can visualize the pattern match using the `match_details` argument and the visualiser.
+        
+        ```python
+        from src.pyhole import Visualizer
+        import Matcher
+        
+        code = "code_file.py"
+        pattern = "pattern_file.py"
+        val, match = match_files(pattern, code, strict_match=False, match_details=True)
+        
+        output_file = "example.html"
+        html = Visualizer.match_to_hml(match, code, pattern)
+        html.write(output_file)
+        ```
+        ![Visualisation of a match](match.png)
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Hole
-
-![Tests Status](https://github.com/JulienLie/python-hole/actions/workflows/python-app.yml/badge.svg?event=push)
-
-Python Hole (or PyHole) is a python library to create patterns file for Python code.
-
-## Syntax
-
-We extended the python syntax to create patterns file. Our new syntax include the following elements:
-
-| Wildcard          | Description                                       |
-|-------------------|---------------------------------------------------|
-| ?                 | Match 1 element                                   |
-| ?*                | Match 0 or more elements                          |
-| ?{name}           | Match 1 element and bind it to {``name``}         |
-| ?:                | Match 1 element with a body                       |
-| ?*:               | Match the body of the wildcard in any indentation |
-| ?![<br/>...<br/>] | Use strict match for the body of this wildcard    |
-
-## Usage
-
-```python
-
-import Matcher
-
-code = "code_file.py"
-pattern = "pattern_file.py"
-match = Matcher.match_files(pattern, code, strict_match=False, match_details=False)
-if match:
-    print("We found a match")
-else:
-    print("No match")
-```
-The `match_files` function takes 4 arguments:
-1. `pattern_file: string` The path to the file describing the pattern
-2. `code_file: string` The path to the python code file
-3. `strict_match: boolean` When strict_match is set to True, a strict match is performed. 
-A strict match requires an exact match between the code file and the pattern file, including code structure and syntax. 
-If strict_match is set to False, a "soft" match is performed, which allows for flexibility in code sections using wildcards.
-4. `match_details: boolean` If match_details is set to True, the function returns a tuple (result, details), 
-where result is a boolean value indicating whether the code matches the pattern. 
-If result is True, details contains the match details. If result is False, details contains the error that prevented the match.
-
-
-## Examples
-### Python code:
-```python
-def multiplications(n):
-    """
-    pre:  n is a positive integer
-    post: Return the number of distinct decompositions a,b 
-          such that n == a*b == b*a
-    """
-    b=n
-    a=1
-    c=0
-    while a*b==n:
-        c=a*(b/a)
-        a+=1
-    return c
-```
-### Pattern file:
-#### Soft match
-```python
-def multiplications(n):
-    ?var1 = ?       # We want to have a initial variable
-    ?*:
-        ?var1 = ?   # This variable has to be updated somewhere
-    return ?var1    # And we want to return it
-```
-#### Strict match
-```python
-def multiplications(n):
-    ?*
-    ?var1 = ?       # We want to have a initial variable
-    ?*
-    ?*:
-        ?*
-        ?var1 = ?   # This variable has to be updated somewhere
-        ?*
-    return ?var1    # And we want to return it
-```
-
-Those two piece of codes describes the same patterns. The soft match hide the multiple wildcards `?*` in the strict match.
-
-
-## Strict match / Soft match
-### Main difference
-In a soft match, there is flexibility in code structure and the possibility of including extra code, 
-as long as the main matching criteria are met. In contrast, in a strict match, precise adherence to the defined 
-code structure and syntax is necessary, and there is limited to no allowance for variations or 
-additional code outside of the specified structure.
-
-### The wildcard `?:[]`
-The wildcard `?![]` is a notation that allows for a combination of strict and soft matching in certain parts of a code pattern. It is useful when you want to perform a soft match but have a strict match requirement within a specific section of code.
-
-Let's consider an example to illustrate this. Suppose we have the following pattern:
-
-```python
-def foo(bar):
-    ?var = 0
-    for ? in range(?*):
-        ?![
-        if ?:
-           ?var += 1 
-        ]
-```
-In this pattern, the wildcard ? represents a placeholder for any valid Python identifier. The ?var = 0 statement assigns the value 0 to a variable, which we'll refer to as x. The for ? in range(?*) loop iterates over a range of values, which we'll refer to as y. Finally, ?![ ... ] represents a strict match requirement that enforces certain code within the if statement.
-
-Now, let's say we have the following code snippet:
-
-```python
-def foo(bar):
-    x = 0
-    y = len(bar)
-    for i in range(y):
-        z = bar[i]
-        if z:
-            x += 1
-    return x
-```
-We want to match this code snippet with the given pattern. Let's go through each line and see how the wildcard ?![] allows for matching.
-
-- In the pattern, `?var = 0` matches the code `x = 0` because the wildcard `?var` represents the variable named `x`.
-- The loop statement `for ? in range(?*)` in the pattern matches the code `for i in range(y)`. 
-- Here, `?` corresponds to the loop variable `i`, and `?*` corresponds to the length of the bar list, which is stored in `y`.
-- The strict match requirement `?![ ... ]` checks the code within the if statement. 
-- In the pattern, `?` represents the condition `z`, and `?var += 1` corresponds to `x += 1` within the if block.
-
-As a result, the code snippet matches the pattern because all the placeholders and the strict match requirements are satisfied. 
-However, if we have additional code within the if block, such as a print statement like `print("true")`, 
-the pattern won't match because the strict match requirement `?![ ... ]` doesn't accommodate that extra code.
-
-In summary, the wildcard `?![]` allows for a combination of soft and strict matching. 
-It provides flexibility by allowing soft matches for variables and loop structures while enforcing strict matches for 
-specific code sections. This helps in creating adaptable code patterns that can match similar code snippets with some variations.
-
-## Visualization
-You can visualize the pattern match using the `match_details` argument and the visualiser.
-
-```python
-from src.pyhole import Visualizer
-import Matcher
-
-code = "code_file.py"
-pattern = "pattern_file.py"
-val, match = match_files(pattern, code, strict_match=False, match_details=True)
-
-output_file = "example.html"
-html = Visualizer.match_to_hml(match, code, pattern)
-html.write(output_file)
-```
-![Visualisation of a match](match.png)
-
```

### Comparing `python-hole-0.0.5/src/python_hole.egg-info/SOURCES.txt` & `python-hole-0.0.6/src/python_hole.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-setup.cfg
 setup.py
 src/pyhole/AstWalker.py
 src/pyhole/HoleAST.py
 src/pyhole/Matcher.py
 src/pyhole/PatternMatch.py
 src/pyhole/PyHoleErrorListener.py
 src/pyhole/PyHoleParser.py
```

