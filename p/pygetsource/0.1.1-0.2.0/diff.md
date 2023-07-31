# Comparing `tmp/pygetsource-0.1.1.tar.gz` & `tmp/pygetsource-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygetsource-0.1.1.tar", last modified: Fri Jul 28 23:34:23 2023, max compression
+gzip compressed data, was "pygetsource-0.2.0.tar", last modified: Mon Jul 31 08:13:08 2023, max compression
```

## Comparing `pygetsource-0.1.1.tar` & `pygetsource-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-28 23:34:13.000000 pygetsource-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 23:34:23.655079 pygetsource-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-28 23:34:13.000000 pygetsource-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/pygetsource/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/ast_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    67241 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/decompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pygetsource/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/pygetsource.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 23:34:23.000000 pygetsource-0.1.1/pygetsource.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 23:34:13.000000 pygetsource-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 23:34:23.655079 pygetsource-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 23:34:23.655079 pygetsource-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_dev.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_py37.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-28 23:34:13.000000 pygetsource-0.1.1/tests/test_rebuild.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:13:08.695691 pygetsource-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-31 08:12:54.000000 pygetsource-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-31 08:13:08.695691 pygetsource-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-31 08:12:54.000000 pygetsource-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:13:08.695691 pygetsource-0.2.0/pygetsource/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pygetsource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pygetsource/ast_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67986 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pygetsource/decompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pygetsource/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pygetsource/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:13:08.695691 pygetsource-0.2.0/pygetsource.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-31 08:13:08.000000 pygetsource-0.2.0/pygetsource.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-31 08:13:08.000000 pygetsource-0.2.0/pygetsource.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:13:08.000000 pygetsource-0.2.0/pygetsource.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-31 08:13:08.000000 pygetsource-0.2.0/pygetsource.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 08:13:08.000000 pygetsource-0.2.0/pygetsource.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-31 08:12:54.000000 pygetsource-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:13:08.695691 pygetsource-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:13:08.695691 pygetsource-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 08:12:54.000000 pygetsource-0.2.0/tests/test_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15081 2023-07-31 08:12:54.000000 pygetsource-0.2.0/tests/test_py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-31 08:12:54.000000 pygetsource-0.2.0/tests/test_rebuild.py
```

### Comparing `pygetsource-0.1.1/LICENSE` & `pygetsource-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pygetsource-0.1.1/PKG-INFO` & `pygetsource-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.1.1
-Summary: Decompiler written in Python for Python
+Version: 0.2.0
+Summary: A Python 3 decompiler
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,29 +23,44 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Disassemblers
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Utilities
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Codecov](https://img.shields.io/codecov/c/github/percevalw/pygetsource?logo=codecov&style=flat-square)](https://codecov.io/gh/percevalw/pygetsource)
 [![PyPI](https://img.shields.io/pypi/v/pygetsource?color=blue&style=flat-square)](https://pypi.org/project/pygetsource/)
 ![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
+`pygetsource` is a decompiler for Python 3, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -58,15 +73,15 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.11. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
 
 Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
@@ -120,23 +135,24 @@
 
 ## When is this useful ?
 
 `pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
-[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
+[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above. At the moment, it supports a larger range of Python syntaxes (such as with blocks or try/excepts).
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
 
 ## How does it work ?
 
 `pygetsource` uses a distinct approach. The bytecode instructions are initially converted into a directed graph, representing the program's flow. This graph is then iteratively reduced, processing each node based on its opcode, argument, and position and generating the [AST](https://docs.python.org/3/library/ast.html) as it goes.
-This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements.
+This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements, and handle Python versions from 3.7 to 3.11 with the same codebase.
+
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
```

### Comparing `pygetsource-0.1.1/README.md` & `pygetsource-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
+`pygetsource` is a decompiler for Python 3, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -24,15 +24,15 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.11. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
 
 Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
@@ -86,23 +86,24 @@
 
 ## When is this useful ?
 
 `pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
-[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
+[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above. At the moment, it supports a larger range of Python syntaxes (such as with blocks or try/excepts).
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
 
 ## How does it work ?
 
 `pygetsource` uses a distinct approach. The bytecode instructions are initially converted into a directed graph, representing the program's flow. This graph is then iteratively reduced, processing each node based on its opcode, argument, and position and generating the [AST](https://docs.python.org/3/library/ast.html) as it goes.
-This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements.
+This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements, and handle Python versions from 3.7 to 3.11 with the same codebase.
+
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
```

### Comparing `pygetsource-0.1.1/pygetsource/ast_utils.py` & `pygetsource-0.2.0/pygetsource/ast_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -114,15 +114,14 @@
             )
 
 
 class RemoveLastContinue(ast.NodeTransformer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.can_remove_continue = False
-        self.current_loops = []
 
     def generic_visit(self, node):
         for field, old_value in ast.iter_fields(node):
             if field in ("body", "orelse") and isinstance(old_value, list):
                 new_body = []
                 last_val = self.can_remove_continue
                 for last_in_body, split in [
@@ -138,47 +137,103 @@
                         )
                     )
                     for value in split:
                         if isinstance(value, ast.AST):
                             value = self.visit(value)
                             if value is None:
                                 continue
-                            elif not isinstance(value, ast.AST):
-                                new_body.extend(value)
-                                continue
                         new_body.append(value)
                 self.can_remove_continue = last_val
                 old_value[:] = new_body
             elif isinstance(old_value, list):
                 new_values = []
                 for value in old_value:
                     if isinstance(value, ast.AST):
                         value = self.visit(value)
                         if value is None:
                             continue
-                        elif not isinstance(value, ast.AST):
-                            new_values.extend(value)
-                            continue
                     new_values.append(value)
                 old_value[:] = new_values
-            elif isinstance(old_value, ast.AST):
-                new_node = self.visit(old_value)
-                if new_node is None:
-                    delattr(node, field)
-                else:
-                    setattr(node, field, new_node)
         return node
 
     def visit_Continue(self, node):
         if self.can_remove_continue:
             return None
         return node
 
 
 class WhileBreakFixer(ast.NodeTransformer):
     def __init__(self, while_fusions):
         self.while_fusions = while_fusions
 
     def visit_Break(self, node):
-        if hasattr(node, "_loop_node") and node._loop_node in self.while_fusions:
-            return ast.Continue()
+        if hasattr(node, "_loop_node"):
+            if node._loop_node in self.while_fusions:
+                return ast.Continue()
         return node
+
+
+def negate(node):
+    if isinstance(node, ast.UnaryOp) and isinstance(node.op, ast.Not):
+        return node.operand
+    if isinstance(node, ast.BoolOp) and isinstance(node.op, ast.Or):
+        # num_neg = sum(isinstance(n, ast.UnaryOp) and isinstance(n.op, ast.Not) for n in node.values)
+        # if num_neg > len(node.values) / 2:
+        return ast.BoolOp(op=ast.And(), values=[negate(n) for n in node.values])
+    if isinstance(node, ast.BoolOp) and isinstance(node.op, ast.And):
+        # num_neg = sum(isinstance(n, ast.UnaryOp) and isinstance(n.op, ast.Not) for n in node.values)
+        # if num_neg > len(node.values) / 2:
+        return ast.BoolOp(op=ast.Or(), values=[negate(n) for n in node.values])
+    return ast.UnaryOp(op=ast.Not(), operand=node)
+
+
+def get_origin(trees: ast.AST):
+    origin = None
+    offset = None
+    if isinstance(trees, ast.AST):
+        trees = [trees]
+    for tree in trees:
+        for node in ast.walk(tree):
+            try:
+                if offset is None or node._origin.offset < offset:
+                    origin = node._origin_node
+            except AttributeError:
+                pass
+        return origin
+
+
+def walk_with_parent(node):
+    """
+    Recursively yield all descendant nodes in the tree starting at *node*
+    (including *node* itself), in no specified order.  This is useful if you
+    only want to modify nodes in place and don't care about the context.
+    """
+    from collections import deque
+
+    todo = deque([(None, node)])
+    while todo:
+        parent, node = todo.popleft()
+        todo.extend((node, child) for child in ast.iter_child_nodes(node))
+        yield parent, node
+
+
+def remove_from_parent(item: ast.AST, parent: ast.AST):
+    for field, old_value in ast.iter_fields(parent):
+        if isinstance(old_value, list):
+            if item in old_value:
+                old_value.remove(item)
+                return True
+        elif old_value is item:
+            delattr(parent, field)
+            return True
+    return False
+
+
+def make_bool_op(op, values):
+    assert len(values) > 0 and isinstance(op, (ast.And, ast.Or))
+    new_values = []
+    for v in values:
+        if isinstance(v, ast.BoolOp) and isinstance(v.op, op.__class__):
+            new_values.extend(v.values)
+        else:
+            new_values.append(v)
+    return ast.BoolOp(op=op, values=new_values)
```

### Comparing `pygetsource-0.1.1/pygetsource/decompiler.py` & `pygetsource-0.2.0/pygetsource/decompiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 from typing import List, Optional, Set, Tuple
 
 from IPython.display import display
 
 from .ast_utils import (
     ComprehensionBody,
     ExceptionMatch,
-    ExceptionPlaceholder,
     ForTargetPlaceholder,
     RemoveLastContinue,
     Reraise,
     RewriteComprehensionArgs,
     Unpacking,
     WhileBreakFixer,
+    get_origin,
+    make_bool_op,
+    negate,
+    remove_from_parent,
+    walk_with_parent,
 )
 from .utils import (
     binop_to_ast,
     compareop_to_ast,
-    get_origin,
     graph_sort,
     hasjabs,
     inplace_to_ast,
-    lowest_common_successors,
+    nb_binary_ops_to_ast,
+    nb_inplace_ops_to_ast,
+    no_ops,
     unaryop_to_ast,
 )
 
 try:
     import ast as astunparse
 
     assert hasattr(astunparse, "unparse")
@@ -81,22 +86,33 @@
         self.stack: List[ast.AST] = None
 
         # The node's position in the topological sort
         self.index: int = -1
         self.visited: bool = False
         self.loops = set()
         self.is_conditional_while = False
-        self.jump_test = None
         self._container = self
 
+        # To build boolean expressions
+        self.test_wip = None
+
     @property
     def container(self):
-        if self._container is not self:
-            self._container = self._container.container
-        return self._container
+        if self._container is self:
+            return self
+        return self._container.container
+
+    @property
+    def successors(self):
+        return set((self.next, *self.jumps) if self.next else self.jumps)
+
+    @property
+    def jump(self):
+        [jump] = self.jumps
+        return jump
 
     def add_stmt(self, stmt):
         if DEBUG:
             print("Add stmt", self, ":", stmt)
         try:
             if DEBUG:
                 print(
@@ -106,46 +122,99 @@
                 )
         except Exception:
             warn("Could not unparse", stmt, "in", self)
         self.stmts.append(stmt)
 
     def add_stack(self, item):
         if DEBUG:
-            print("Add stack", self, ":", item)
+            print("Add stack", self, end=": ")
+            if item:
+                try:
+                    print(astunparse.unparse(ast.fix_missing_locations(item)))
+                except Exception:
+                    warn("Could not unparse", ast.dump(item), "in", self)
+            else:
+                print(item)
         self.stack.append(item)
 
     def pop_stack(self):
         return self.stack.pop()
 
+    def remove(self):
+        """
+        Remove the node from the graph
+        """
+        if DEBUG:
+            print(
+                "Remove node",
+                self,
+                "| next=",
+                self.next,
+                "jumps=",
+                self.jumps,
+                "| prev=",
+                self.prev,
+            )
+        successors = set((self.next, *self.jumps) if self.next else self.jumps)
+        successors.discard(self)
+        for succ in successors:
+            if not succ:
+                continue
+            succ.prev.remove(self)
+            for pred in self.prev:
+                if pred is not self:
+                    succ.prev.add(pred)
+            if DEBUG:
+                print("Now", succ, "predecessors are", succ.prev)
+        for pred in self.prev:
+            pred.jumps |= successors
+            pred.jumps.discard(self)
+            if pred.next is self:
+                pred.next = self.next
+                pred.jumps.discard(pred.next)
+            pred.jumps.discard(pred.next)
+
+    def unlink_successor(self, other):
+        self.jumps.discard(other)
+        if self.next is other:
+            self.next = None
+        other.prev.discard(self)
+
     def contract_backward(self):
         """
         Merge the node with its predecessor
         """
 
         # If the node has a single predecessor, merge it with that node
 
         prev_node = next((n for n in self.prev if n.next is self), None)
-        assert prev_node and (
-            (len(self.prev) == 1)
-            or prev_node.opname in ("NOP",)  # and not prev_node.jumps) or
-        )
+        assert prev_node and len(self.prev) == 1
 
         prev_node._container = self._container
         if DEBUG:
             print(
-                "Contract backward",
-                prev_node,
-                "<<<",
+                "Contract",
                 self,
-                "|",
+                "| next=",
                 self.next,
+                "jumps=",
                 self.jumps,
-                "|",
+                "| prev=",
                 self.prev,
             )
+            print(
+                "<<< into",
+                prev_node,
+                "| next=",
+                prev_node.next,
+                "jumps=",
+                prev_node.jumps,
+                "| prev=",
+                prev_node.prev,
+            )
         self.prev.remove(prev_node)
         for pred_pred in prev_node.prev:
             if pred_pred.next is prev_node:
                 pred_pred.next = self
             pred_pred.jumps = {
                 self if jump is prev_node else jump for jump in pred_pred.jumps
             }
@@ -160,15 +229,24 @@
                 continue
             if prev_node in succ.prev:
                 succ.prev.remove(prev_node)
                 succ.prev.add(self)
 
         self.stmts = prev_node.stmts + self.stmts
         if DEBUG:
-            print("After contraction", self, "|", self.next, self.jumps, "|", self.prev)
+            print(
+                "After contraction",
+                self,
+                "| next=",
+                self.next,
+                "jump=",
+                self.jumps,
+                "| prev=",
+                self.prev,
+            )
 
         return prev_node
 
     @classmethod
     def from_code(cls, code: CodeType, prune: bool = False):
         bytes = code.co_code
         offset = 0
@@ -196,38 +274,57 @@
             for i in range(op_idx, offset, 2):
                 graph[i] = block
 
         for block in graph.values():
             opname = block.opname
             arg = block.arg
 
-            if opname in ("RETURN_VALUE",):
+            if opname == "RETURN_VALUE":
                 pass
             elif opname == "JUMP_FORWARD":
                 block.jumps.add(graph[block.offset + arg])
+            elif opname == "JUMP_BACKWARD":
+                block.jumps.add(graph[block.offset - arg])
             elif opname == "JUMP_ABSOLUTE":
                 block.jumps.add(graph[arg])
             elif opname in (
                 "POP_JUMP_IF_TRUE",
                 "POP_JUMP_IF_FALSE",
                 "JUMP_IF_NOT_EXC_MATCH",
             ):
                 block.next = graph[block.offset]
                 block.jumps.add(graph[arg])
             elif opname in (
+                "JUMP_IF_TRUE_OR_POP",
+                "JUMP_IF_FALSE_OR_POP",
+            ):
+                block.next = graph[block.offset]
+                if sys.version_info < (3, 11):
+                    block.jumps.add(graph[arg])
+                else:
+                    block.jumps.add(graph[block.offset + arg])
+            elif opname in (
                 "FOR_ITER",
                 "SETUP_FINALLY",
                 "SETUP_LOOP",
+                "POP_JUMP_FORWARD_IF_FALSE",
+                "POP_JUMP_FORWARD_IF_TRUE",
             ):
                 block.next = graph[block.offset]
 
                 if graph[block.offset + arg].opname == "POP_BLOCK":
                     block.jumps.add(graph[block.offset + arg + 2])
                 else:
                     block.jumps.add(graph[block.offset + arg])
+            elif opname in (
+                "POP_JUMP_BACKWARD_IF_FALSE",
+                "POP_JUMP_BACKWARD_IF_TRUE",
+            ):
+                block.next = graph[block.offset]
+                block.jumps.add(graph[block.offset - arg])
             else:
                 if block.offset in graph:
                     block.next = graph[block.offset]
 
             if block.next:
                 block.next.prev.add(block)
             for jump in block.jumps:
@@ -235,21 +332,15 @@
 
         root = graph[0]
         root = rewire_break_loop(root)
 
         index = 0
         sorted_nodes = []
         for node in graph_sort(root):
-            if (
-                node.opname == "NOP"
-                or node.opname == "RERAISE"
-                and node.arg == 0
-                or node.opname == "POP_BLOCK"
-                or node.opname == "SETUP_LOOP"
-            ):
+            if node.opname in no_ops or node.opname == "RERAISE" and node.arg == 0:
                 if node.next:
                     for n in node.prev:
                         if n.next is node:
                             n.next = node.next
                         n.jumps = {node.next if j is node else j for j in n.jumps} - {
                             n.next
                         }
@@ -258,44 +349,62 @@
                 node.index = index
                 index += 1
                 sorted_nodes.append(node)
 
         graph_nodes = set(sorted_nodes)
         for node in sorted_nodes:
             node.prev &= graph_nodes
+            node._origin_jumps = node.jumps
+            node._origin_next = node.next
+
+            if "JUMP_" in node.opname and "_IF_" in node.opname:
+                if node.next in node.jumps or len(node.jumps) == 0:
+                    node.jumps = {node.next}
         # detect_loops(sorted_nodes[0])
 
         root = sorted_nodes[0]
 
         if prune:
             root = contract_jumps(root)
 
         return root
 
     def __repr__(self):
-        return f"[{self.op_idx}]({self.opname}, {self.arg})"
+        return f"[{self.op_idx}]{self.opname}({self.arg_value})"
 
     @property
     def arg_value(self):
         opname = self.opname
         if opname.startswith("LOAD_") or opname.startswith("STORE_"):
             opname = opname[5:] if opname.startswith("LOAD_") else opname[6:]
 
             if opname == "FAST":
                 return self.code.co_varnames[self.arg]
             elif opname in ("NAME", "GLOBAL"):
+                if opname == "GLOBAL" and sys.version_info >= (3, 11):
+                    return ("NULL+" if self.arg & 1 else "") + self.code.co_names[
+                        self.arg >> 1
+                    ]
                 return self.code.co_names[self.arg]
             elif opname == "DEREF":
-                return (self.code.co_cellvars + self.code.co_freevars)[self.arg]
+                if sys.version_info < (3, 11):
+                    return (self.code.co_cellvars + self.code.co_freevars)[self.arg]
+                else:
+                    return (self.code.co_cellvars + self.code.co_freevars)[
+                        self.arg - len(self.code.co_varnames)
+                    ]
+
             elif opname == "CONST":
                 return repr(self.code.co_consts[self.arg])
             elif opname in ("ATTR", "METHOD"):
                 return self.code.co_names[self.arg]
         elif opname.startswith("COMPARE_OP"):
             return dis.cmp_op[self.arg]
+        elif opname.startswith("BINARY_OP"):
+            return dis._nb_ops[self.arg][1]
         else:
             return self.arg
 
     def draw(self, prog=None):
         import networkx as nx
         from IPython.core.display import HTML
 
@@ -366,55 +475,79 @@
     def last_stmts(self):
         if self.stmts:
             return self.stmts
         prev_visited = [n for n in self.prev if n.visited]
         if len(prev_visited) != 1:
             return self.stmts
         prev = next(iter(prev_visited), None)
-        return prev.last_stmts()
+        if prev is self:
+            return prev.last_stmts()
+
+    @property
+    def is_ready(self):
+        if sum([prev.visited for prev in self.prev if prev is not self]) > 1:
+            return False
+        if any(not prev.visited and prev.index < self.index for prev in self.prev):
+            return False
+        return True
 
     # noinspection PyMethodParameters,PyMethodFirstArgAssignment
     def _run(
         node: "Node",
-        stop_nodes: Set["Node"] = frozenset(),
         loop_heads: Tuple["Node"] = (),
-        while_fusions={},
+        while_fusions=set(),
         stop_on_jump: bool = False,
+        bool_stack=(),
     ):
         """
         Convert the graph into an AST
         """
         root = node
+        kw_names = ()
 
-        if node.visited or node in stop_nodes:
+        if not node.is_ready or node.visited:
             return None
 
         while True:
             if DEBUG:
                 print(
-                    "::: Processing",
-                    node,
-                    "|",
-                    node.next,
-                    node.jumps,
-                    "|",
-                    node.prev,
-                    "Ø",
-                    loop_heads,
+                    f"::: Processing {node} | next={node.next} jumps={node.jumps} | prev={node.prev} Ø=loop_heads"
                 )
+
             node.visited = True
             prev_visited = [n for n in node.prev if n.visited]
             if len(prev_visited) > 1:
                 raise Exception(f"Too many visited predecessors for {node}")
             if node.stack is None:
                 if prev_visited and prev_visited[0].stack is not None:
                     node.stack = list(prev_visited[0].stack)
                 else:
                     node.stack = []
 
+            prev_visited = [n for n in node.prev if n.visited]
+            prev_unvisited = [n for n in node.prev if not n.visited]
+            while (
+                len(prev_visited) == 1
+                and len(prev_unvisited) == 0
+                and prev_visited[0].successors == {node}
+            ):
+                if root.container is not node:
+                    prev = node.contract_backward()
+                else:
+                    prev = None
+                if not prev:
+                    break
+                if loop_heads and loop_heads[-1] is prev:
+                    loop_heads = (*loop_heads[:-1], node)
+                prev_visited = [n for n in node.prev if n.visited]
+                prev_unvisited = [n for n in node.prev if not n.visited]
+
+                if DEBUG:
+                    display(node.draw())
+
             prev_unvisited = [n for n in node.prev if not n.visited]
             if len(prev_unvisited):
                 loop_heads = (*loop_heads, node)
 
             if node.opname == "LOAD_CLOSURE":
                 node.add_stack(None)
             elif node.opname.startswith("LOAD_"):
@@ -422,346 +555,375 @@
             elif node.opname.startswith("STORE_"):
                 process_store_(node)
             elif node.opname.startswith("DELETE_") or node.opname.startswith("DEL_"):
                 process_binding_(node)
                 node.add_stmt(ast.Delete([node.pop_stack()]))
             elif node.opname == "RETURN_VALUE":
                 node.add_stmt(ast.Return(node.pop_stack()))
-            elif node.opname in ("JUMP_FORWARD", "JUMP_ABSOLUTE"):
+            elif node.opname in ("JUMP_FORWARD", "JUMP_ABSOLUTE", "JUMP_BACKWARD"):
                 jump = next(iter(node.jumps))
 
                 # If we don't leave any loop
-                loop_head = explore_until(jump, loop_heads)
+                loop_head = explore_until(jump, stop_nodes=loop_heads[::-1])
                 same_context = (
                     not loop_heads
                     or loop_head is loop_heads[-1]
                     or loop_head is None
                     and len(jump.prev) == 1
                 )
                 if jump.visited:
                     if same_context:
+                        if DEBUG:
+                            print(
+                                "JUMP",
+                                node,
+                                "VISITED SAME CONTEXT",
+                                loop_head,
+                                "vs",
+                                loop_heads,
+                            )
                         node.add_stmt(ast.Continue(_loop_node=jump))
                     else:
+                        if DEBUG:
+                            print(
+                                "JUMP",
+                                node,
+                                "VISITED NOT SAME CONTEXT",
+                                loop_head,
+                                "vs",
+                                loop_heads,
+                            )
                         node.add_stmt(ast.Break(_loop_node=jump))
                 else:
                     if not same_context:
+                        if DEBUG:
+                            print(
+                                "JUMP",
+                                node,
+                                "NOT VISITED NOT SAME CONTEXT",
+                                loop_head,
+                                "vs",
+                                loop_heads,
+                            )
                         node.add_stmt(ast.Break(_loop_node=jump))
-            elif node.opname in (
-                "POP_JUMP_IF_TRUE",
-                "POP_JUMP_IF_FALSE",
-                "JUMP_IF_NOT_EXC_MATCH",
+            elif node.opname.startswith("POP_JUMP") or node.opname.startswith(
+                "JUMP_IF"
             ):
                 if node.opname == "JUMP_IF_NOT_EXC_MATCH":
                     test = ExceptionMatch(node.pop_stack())
                     node.pop_stack()
                 else:
                     test = node.pop_stack()
-                node.jump_test = test
+
+                if DEBUG:
+                    print("BASE TEST", astunparse.unparse(test))
+                test = negate(test) if "IF_TRUE" in node.opname else test
+                if DEBUG:
+                    print("MOD  TEST", astunparse.unparse(test))
+
+                node.test_wip = test
+                test_origin = get_origin(test).container
+                test_prev = next(iter(test_origin.prev), None)
+
+                # if test_origin.stmts and isinstance(test_origin.stmts[-1], ast.Assign):
+                #     stmt = test_origin.stmts.pop()
+                #     test = ast.NamedExpr(
+                #         stmt.targets[0],
+                #         stmt.value,
+                #     )
 
                 if_node = node.next
                 [else_node] = node.jumps
 
-                old_if_node = if_node
+                if_node = if_node._run(
+                    loop_heads=loop_heads,
+                    while_fusions=while_fusions,
+                )
+                else_node = else_node._run(
+                    loop_heads=loop_heads,
+                    while_fusions=while_fusions,
+                )
+
+                if_node = node.next if if_node else None
+                else_node = node.jump if else_node else None
+                while True:
+                    keep_going = False
+                    if node.next.is_ready and not node.next.visited:
+                        if_node = node.next._run(
+                            loop_heads=loop_heads,
+                            while_fusions=while_fusions,
+                        )
+                        keep_going = True
+                    if node.jump.is_ready and not node.jump.visited:
+                        else_node = node.jump._run(
+                            loop_heads=loop_heads,
+                            while_fusions=while_fusions,
+                        )
+                        keep_going = True
+                    if not keep_going:
+                        break
 
-                ################
-                # SPECIAL CASE #
-                ################
                 if DEBUG:
-                    print(
-                        "IF/ELSE BLOCK",
-                        node,
-                        "LOOP HEADS",
-                        loop_heads,
-                        "IF",
-                        if_node,
-                        "ELSE",
-                        else_node,
-                    )
-
-                real_branch = (
-                    next(
-                        (n for n in loop_heads[-1].prev if n.next is loop_heads[-1]),
-                        None,
-                    )
-                    if loop_heads
+                    print("DONE processing branches", node)
+                    print(">> if_node", if_node, node.next)
+                    print(">> else_node", else_node, node.jump)
+
+                if_node = (
+                    node.next
+                    if node.next.is_ready
+                    and node.next.visited
+                    and node.next.index > node.index
+                    else None
+                )
+                else_node = (
+                    node.jump
+                    if node.jump.is_ready
+                    and node.jump.visited
+                    and node.jump.index > node.index
                     else None
                 )
-                if (
-                    real_branch
-                    and real_branch.jump_test
-                    and real_branch.opname
-                    == (
-                        "POP_JUMP_IF_FALSE"
-                        if node.opname == "POP_JUMP_IF_TRUE"
-                        else "POP_JUMP_IF_TRUE"
-                    )
-                    and ast.dump(real_branch.jump_test) == ast.dump(test)
-                ):
-                    real_head = get_origin(real_branch.jump_test)[0].container
 
-                    if DEBUG:
-                        print("THIS SHOULD BE A CONDITIONAL WHILE LOOP", ast.dump(test))
-                    # node.add_stmt(ast.Continue())
-                    node.next.prev.discard(node)
-                    node.next = None
-                    node.jumps = {real_head}
-                    node.add_stmt(ast.Continue())
-                    else_node.prev.remove(node)
-                    real_head.prev.add(node)
-                    real_branch.is_conditional_while = True
-                    while_fusions[real_head] = else_node
-                    loop_heads = loop_heads[:-1]
-                    if loop_heads and loop_heads[-1] is not real_head:
-                        loop_heads = (*loop_heads, real_head)
-                ################
-                else:
-                    meet_nodes = lowest_common_successors(
-                        if_node,
-                        else_node,
-                        stop_nodes={*stop_nodes, node},
-                    )
-                    if DEBUG:
-                        print(
-                            "IF/ELSE BLOCK",
-                            node,
-                            "MEET",
-                            meet_nodes,
-                            "(STOP at",
-                            {*stop_nodes, node},
-                            ")",
-                        )
-                    assert len(meet_nodes) <= 1
+                branches_meet = (
+                    if_node
+                    and else_node
+                    and if_node.next is else_node.next
+                    and if_node.next
+                    and else_node.next
+                )
 
-                    before = (if_node, else_node)
-                    if_loop_head = (
-                        explore_until(if_node, loop_heads) if loop_heads else None
-                    )
-                    else_loop_head = (
-                        explore_until(else_node, loop_heads) if loop_heads else None
-                    )
+                test = node.test_wip
+                node.test_wip = None
 
-                    if_node = if_node._run(
-                        stop_nodes={*stop_nodes, *meet_nodes, node},
-                        loop_heads=loop_heads,
-                        while_fusions=while_fusions,
-                    )
-                    else_node = else_node._run(
-                        stop_nodes={*stop_nodes, *meet_nodes, node},
-                        loop_heads=loop_heads,
-                        while_fusions=while_fusions,
-                    )
-                    if DEBUG:
-                        print("IF/ELSE", node, "MEET", meet_nodes)
+                if (
+                    test_prev
+                    and test_prev.test_wip
+                    and len(node.jumps) == 1
+                    # and node.jump not in node.prev
+                    and node not in node.successors
+                    and test_prev.index < node.index
+                ):
                     if DEBUG:
                         print(
-                            "IF/ELSE",
+                            "BOOL OP !",
                             node,
-                            "BEFORE succ",
-                            before,
-                            "-> AFTER succ",
-                            if_node,
-                            else_node,
+                            test_prev,
+                            astunparse.unparse(test_prev.test_wip),
                         )
-                    if DEBUG:
-                        display(node.draw())
-
-                    if_item = (
-                        if_node.pop_stack()
-                        if if_node and len(if_node.stack) > len(node.stack)
-                        else None
-                    )
-                    else_item = (
-                        else_node.pop_stack()
-                        if else_node and len(else_node.stack) > len(node.stack)
-                        else None
-                    )
+                    if next(
+                        iter(node.jumps)
+                    ) in test_prev.jumps and node.opname.startswith("POP_JUMP"):
+                        node.remove()
+                        if "IF_TRUE" in node.opname:
+                            test_prev.opname = test_prev.opname.replace(
+                                "IF_FALSE", "IF_TRUE"
+                            )
+                        else:
+                            test_prev.opname = test_prev.opname.replace(
+                                "IF_TRUE", "IF_FALSE"
+                            )
 
-                    test_origin = get_origin(test)[0].container
-                    has_been_unparsed = False
-                    was_a_loop = False
-                    if (
-                        loop_heads
-                        and if_loop_head is loop_heads[-1]
-                        and test_origin is if_loop_head
-                        and (
-                            (if_node or old_if_node).next is if_loop_head
-                            or old_if_node.next is if_loop_head
+                        node._container = test_prev
+                        test_prev.test_wip = make_bool_op(
+                            ast.And(),
+                            [test_prev.test_wip, test],
                         )
-                        and else_loop_head is not loop_heads[-1]
-                    ) or node.is_conditional_while:
                         if DEBUG:
-                            print(
-                                "THIS IS A WHILE X LOOP",
-                                node,
-                                "LOOP HEAD",
-                                if_loop_head,
+                            print(">>", node, astunparse.unparse(test_prev.test_wip))
+                            display(node.draw())
+                        return if_node
+                    elif node.next in test_prev.jumps:
+                        node.remove()
+                        if "IF_TRUE" in node.opname:
+                            test_prev.opname = test_prev.opname.replace(
+                                "IF_FALSE", "IF_TRUE"
                             )
-                        # while node.contract_backward():
-                        #     print("NODE IS CONTRACTED", node, "==?", if_node.next)
-                        #     if DEBUG:
-                        #         display(node.draw())
-                        #     pass
-                        body_stmts = if_node.stmts if if_node else []
-                        if isinstance(body_stmts[-1], ast.Continue):
-                            body_stmts = body_stmts[:-1]
-                        body_stmts = body_stmts or [ast.Pass()]
-                        node.add_stmt(
-                            ast.While(
-                                test=(
-                                    test
-                                    if node.opname != "POP_JUMP_IF_TRUE"
-                                    else ast.UnaryOp(
-                                        op=ast.Not(),
-                                        operand=test,
-                                    )
-                                ),
-                                body=body_stmts,
-                                orelse=[],
-                                _loop_head=if_loop_head,
+                        else:
+                            test_prev.opname = test_prev.opname.replace(
+                                "IF_TRUE", "IF_FALSE"
                             )
+                        node._container = test_prev
+                        test_prev.test_wip = make_bool_op(
+                            ast.Or(),
+                            [
+                                negate(
+                                    test_prev.test_wip
+                                ),  # if node.opname.startswith("POP_JUMP") else test_prev.test_wip,
+                                test,
+                            ],
                         )
-                        if (
-                            else_node
-                            and else_node.stmts
-                            and not isinstance(else_node.stmts[-1], ast.Break)
-                        ):
-                            node.stmts.extend(else_node.stmts)
-                        if if_node.next:
-                            if_node.next.prev.discard(if_node)
-                            if_node.next = None
-                        has_been_unparsed = True
-                        was_a_loop = True
-                    if not has_been_unparsed:
-                        if if_item is None or not if_node or if_node.stmts:
-                            body_stmts = (
-                                if_node.stmts
-                                if if_node and if_node.stmts
-                                else [
-                                    ast.Continue()
-                                    if loop_heads and old_if_node is loop_heads[-1]
-                                    else ast.Pass()
-                                ]
-                                if not loop_heads
-                                or if_loop_head in (loop_heads[-1], None)
-                                # else [ast.Break(_loop_node=get_origin(test)[0])]
-                                else [ast.Break(_loop_node=if_loop_head)]
-                            )
-                            orelse_stmts = (
-                                else_node.stmts
-                                if else_node and else_node.stmts
-                                else []
-                                if meet_nodes
-                                or not loop_heads
-                                or else_loop_head is loop_heads[-1]
-                                else [ast.Break(_loop_node=else_loop_head)]
-                            )
-                            has_else = bool(meet_nodes) or else_loop_head is not None
-                            node.add_stmt(
+                        if DEBUG:
+                            print(">>", node, astunparse.unparse(test_prev.test_wip))
+                            display(node.draw())
+                        return else_node
+                if (
+                    if_node
+                    and if_node.stmts
+                    and isinstance(if_node.stmts[0], ast.While)
+                    # if_node.stmts and isinstance(if_node.stmts[-1].body[], ast.If)
+                ):
+                    stmt = if_node.stmts[0]
+                    if ast.dump(stmt.test) != ast.dump(ast.Constant(True)):
+                        stmt = ast.While(
+                            test=ast.Constant(True),
+                            body=[
                                 ast.If(
-                                    test=(
-                                        test
-                                        if node.opname != "POP_JUMP_IF_TRUE"
-                                        else ast.UnaryOp(
-                                            op=ast.Not(),
-                                            operand=test,
-                                        )
-                                    ),
-                                    body=body_stmts,
-                                    orelse=orelse_stmts if has_else else [],
+                                    test=stmt.test,
+                                    body=stmt.body,
+                                    orelse=if_node.stmts[1:],
                                 )
-                            )
-                            if not has_else:
-                                node.stmts.extend(orelse_stmts)
-                        if if_item:
-                            ternary_expr = ast.IfExp(
-                                test=(
-                                    test
-                                    if node.opname == "POP_JUMP_IF_FALSE"
-                                    else ast.UnaryOp(
-                                        op=ast.Not(),
-                                        operand=test,
+                            ],
+                        )
+
+                    found = False
+                    for parent, tree in walk_with_parent(stmt):
+                        if not isinstance(tree, ast.If):
+                            continue
+                        try:
+                            jump = next(iter(tree._origin_node._origin_jumps))
+                            if not any(n.container is not node for n in jump.prev):
+                                continue
+
+                            if ast.dump(negate(test)) != ast.dump(tree.test):
+                                if DEBUG:
+                                    print("DO WHILE PY310 TEST DID NOT MATCH:")
+                                    print(
+                                        (
+                                            ast.unparse(test),
+                                            ast.unparse(negate(tree.test)),
+                                        )
                                     )
-                                ),
-                                body=if_item,
-                                orelse=else_item,
-                            )
-                            # for item in if_node.stack:
-                            #    node.add_stack(item)
-                            node.add_stack(ternary_expr)
-
-                    # noinspection PyTypeChecker
-                    successors: Set[Node] = {
-                        *((if_node.next, *if_node.jumps) if if_node else (node.next,)),
-                        *(
-                            (else_node.next, *else_node.jumps)
-                            if else_node
-                            else node.jumps
-                        ),
-                    } - {
-                        None
-                    }  # type: ignore
-                    discarded_successors = {
-                        n
-                        for n in (if_node, else_node)
-                        + ((test_origin,) if was_a_loop else ())
-                        if n and n.visited
-                    }
+                                continue
+
+                            remove_from_parent(tree, parent)
+                            while_fusions.add(node)  # [tree._origin_node] = node
+                            found = True
+
+                        except (AttributeError, ValueError):
+                            pass
+
+                    if found:
+                        node.is_conditional_while = True
+                        if_node.stmts = stmt.body
+                        # if_node.jumps.discard(if_node)
+                        if_node.jumps.add(node)
+                        node.prev.add(if_node)
+
+                if DEBUG:
+                    display(node.draw())
+
+                if_item = (
+                    if_node.pop_stack()
+                    if if_node and len(if_node.stack) > len(node.stack)
+                    else None
+                )
+                else_item = (
+                    else_node.pop_stack()
+                    if else_node and len(else_node.stack) > len(node.stack)
+                    else None
+                )
+
+                if_loop_head = (
+                    explore_until(node.next, loop_heads[::-1]) if loop_heads else None
+                )
+                else_loop_head = (
+                    explore_until(node.jump, loop_heads[::-1]) if loop_heads else None
+                )
+
+                if if_item is None or not if_node or if_node.stmts:
+
+                    is_loop = node.is_conditional_while or node in node.next.successors
+
+                    body_stmts = []
+                    if if_node and if_node.stmts:
+                        body_stmts.extend(if_node.stmts)
+                    else:
+                        body_stmts.append(ast.Pass())
+
+                    orelse_stmts = []
+                    if else_node and else_node.stmts:
+                        orelse_stmts.extend(else_node.stmts)
+                    # elif (
+                    #     not branches_meet
+                    #     and loop_heads
+                    #     and else_loop_head is not loop_heads[-1]
+                    #     and not is_loop
+                    # ):
+                    #     orelse_stmts.append(
+                    #         ast.Break(_loop_node=else_loop_head)
+                    #     )
+
+                    if is_loop:
+                        if len(orelse_stmts) == 1 and isinstance(
+                            orelse_stmts[0], ast.Break
+                        ):
+                            orelse_stmts = []
+
+                    has_else = bool(branches_meet) or else_loop_head is not if_loop_head
+
                     if DEBUG:
+                        print("IS THIS WHILE ?")
                         print(
-                            "IF/ELSE SUCC BEFORE CONTRACT",
-                            successors,
-                            "-",
-                            discarded_successors,
+                            "CHECK: node in node.next.successors",
+                            node in node.next.successors,
                         )
-                    if DEBUG:
-                        print("IF/ELSE PREV BEFORE CONTRACT", node.prev)
-                    successors = successors - discarded_successors
-
-                    jump_nodes = successors
-                    for succ in successors:
-                        if DEBUG:
-                            print(
-                                "IF/ELSE",
-                                node,
-                                ": REBINDING SUCCESSOR",
-                                succ,
-                                "=>",
-                                succ.prev,
-                                "->",
-                                succ.prev - {if_node, else_node} | {node},
+                        print("ELSE LOOP HEAD", else_loop_head, loop_heads)
+                    if is_loop and (len(orelse_stmts) == 0 or else_loop_head is None):
+                        node.add_stmt(
+                            ast.While(
+                                test=test,
+                                body=body_stmts,
+                                orelse=[],
+                                _origin_node=node,
+                            )
+                        )
+                        has_else = False
+                        if_node.unlink_successor(node)
+                        if_node.unlink_successor(if_node)
+                    else:
+                        node.add_stmt(
+                            ast.If(
+                                test=test,
+                                body=body_stmts,
+                                orelse=orelse_stmts if has_else else [],
+                                _origin_node=node,
                             )
-                        succ.prev = (succ.prev - discarded_successors) | {node}
-                    for n in discarded_successors:
-                        for p in n.prev:
-                            if p.next in discarded_successors:
-                                p.next = node
-                            p.jumps = {
-                                node if j in discarded_successors else j
-                                for j in p.jumps
-                            }
-                        n.prev = n.prev - discarded_successors
-                    node.next = None
-                    node.jumps = jump_nodes
-                    if DEBUG:
-                        print("IF/ELSE", node, node.stack)
-                    if DEBUG:
-                        print("IF/ELSE SUCC AFTER CONTRACT", successors)
-                    if DEBUG:
-                        print(
-                            "IF/ELSE PREV AFTER CONTRACT",
-                            node.prev,
-                            "prevs successor:",
-                            [(n.next, *n.jumps) for n in node.prev],
                         )
+                    if not has_else:
+                        node.stmts.extend(orelse_stmts)
 
-                    if DEBUG:
-                        display(node.draw())
+                if if_item:
+                    if else_item:
+                        ternary_expr = ast.IfExp(
+                            test=test,
+                            body=if_item,
+                            orelse=else_item,
+                        )
+                        node.add_stack(ternary_expr)
+                    else:
+                        bool_expr = make_bool_op(
+                            op=ast.Or() if "IF_TRUE" in node.opname else ast.And(),
+                            values=[
+                                test if "IF_FALSE" in node.opname else negate(test),
+                                if_item,
+                            ],
+                        )
+                        node.add_stack(bool_expr)
+
+                if if_node:
+                    if_node._container = node
+                    if_node.remove()
+                if else_node:
+                    else_node._container = node
+                    else_node.remove()
+
+                if DEBUG:
+                    display(node.draw())
 
             elif node.opname == "SETUP_FINALLY":
-                process_try_(node, loop_heads, stop_nodes, while_fusions)
+                raise NotImplementedError()
             elif node.opname == "RERAISE":
                 # ("REMOVING RERAISE", node, "STOP NODES", stop_nodes)
                 # for n in node.prev:
                 #    if n.next is node:
                 #        n.next = node.next
                 #    n.jumps = {node.next if j is node else j for j in n.jumps} - {n.next}
                 # node.next.prev = (node.next.prev | node.prev) - {node}
@@ -775,26 +937,22 @@
                 old_body_node = body_node = node.next
                 (jump_node,) = node.jumps
 
                 iter_item = node.pop_stack()
                 iter_item._dumped = True
 
                 placeholder = ForTargetPlaceholder()
-                placeholder._origin_offset = node.op_idx
                 placeholder._origin_node = node
 
                 body_node.stack = [*node.stack, iter_item, placeholder]
                 body_node = body_node._run(
-                    stop_nodes={*stop_nodes, node, jump_node},
                     loop_heads=loop_heads,
                     while_fusions=while_fusions,
                 )
-                body_loop_head = explore_until(
-                    body_node, (node, jump_node, *stop_nodes)
-                )
+                body_loop_head = explore_until(body_node, (node, jump_node))
                 if DEBUG:
                     print("FOR LOOP HEAD", body_loop_head)
                 if DEBUG:
                     print("BODY", [ast.dump(x) for x in body_node.stmts])
                 target = body_node.stmts.pop(0).targets[0]
 
                 body_stmts = (body_node.stmts if body_node else []) + (
@@ -830,28 +988,42 @@
                         }
                 node.next.prev.discard(node)
                 node.next = None
                 node.jumps = jump_nodes
                 node.prev -= discarded_successors
                 loop_heads = loop_heads[:-1]
             elif node.opname == "COMPARE_OP":
-                if compareop_to_ast[node.arg] != "exception match":
-                    right = node.pop_stack()
-                    left = node.pop_stack()
-                else:
-                    left = node.pop_stack()
-                    # right = stack.pop()[1]
-                    right = None
+                right = (
+                    node.pop_stack()
+                    if compareop_to_ast[node.arg] != "exception match"
+                    else None
+                )
+                left = node.pop_stack()
                 node.add_stack(
                     ast.Compare(
                         left=left,
                         ops=[compareop_to_ast[node.arg]],
                         comparators=[right],
                     ),
                 )
+            elif node.opname == "BINARY_OP":
+                right = node.pop_stack()
+                left = node.pop_stack()
+                if node.arg in nb_binary_ops_to_ast:
+                    node.add_stack(
+                        ast.BinOp(
+                            left=left, op=nb_binary_ops_to_ast[node.arg], right=right
+                        ),
+                    )
+                else:
+                    node.add_stack(
+                        ast.AugAssign(
+                            target=left, op=nb_inplace_ops_to_ast[node.arg], value=right
+                        ),
+                    )
             elif node.opname in binop_to_ast:
                 right = node.pop_stack()
                 left = node.pop_stack()
                 node.add_stack(
                     ast.BinOp(left=left, op=binop_to_ast[node.opname], right=right),
                 )
             elif node.opname == "CONTAINS_OP":
@@ -1006,15 +1178,16 @@
             # TODO: check in for/while loop ?
             elif node.opname in ("LIST_APPEND", "SET_ADD"):
                 value = node.pop_stack()
                 collection = node.stack[-node.arg]
                 # if we can loop to the collection beginning
                 if (
                     loop_heads
-                    and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]
+                    and explore_until(node, (*loop_heads[::-1], collection))
+                    is loop_heads[-1]
                 ):
                     node.add_stmt(ComprehensionBody(value, collection))
                 else:
                     assert hasattr(collection, "elts")
                     collection = type(collection)(elts=[*collection.elts, value])
                     node.stack[-node.arg] = collection
             elif node.opname == "MAP_ADD":
@@ -1025,29 +1198,31 @@
                 # Before, those were reversed.
                 if sys.version_info < (3, 8):
                     key, value = value, key
                 collection = node.stack[-node.arg]
                 # if we can loop to the collection beginning
                 if (
                     loop_heads
-                    and explore_until(node, {*loop_heads, collection}) is loop_heads[-1]
+                    and explore_until(node, (*loop_heads[::-1], collection))
+                    is loop_heads[-1]
                 ):
                     node.add_stmt(ComprehensionBody((key, value), collection))
                 else:
                     assert hasattr(collection, "elts")
                     collection = type(collection)(
                         keys=[*collection.keys, key],
                         values=[*collection.values, value],
                     )
                     node.stack[-node.arg] = collection
             elif node.opname == "YIELD_VALUE":
                 node.add_stmt(ast.Expr(ast.Yield(node.pop_stack())))
             elif node.opname == "MAKE_FUNCTION":
                 assert node.arg in (0, 8), node.arg
-                node.pop_stack()  # function name
+                if sys.version_info < (3, 11):
+                    node.pop_stack()  # function name
                 func_code: ast.Constant = node.pop_stack()
                 if node.arg == 8:
                     node.pop_stack()
                 assert isinstance(func_code, ast.Constant)
                 code = func_code.value
                 function_node = Node.from_code(code)
                 if DEBUG:
@@ -1070,33 +1245,49 @@
                             posonlyargs=[],
                         ),
                         body=sub_function_body,
                         decorator_list=[],
                         returns=None,
                     )
                 )
-            elif node.opname in ("CALL_FUNCTION", "CALL_METHOD"):
+            elif node.opname == "KW_NAMES":
+                kw_names = node.code.co_consts[node.arg]
+                print("KWNAMES", kw_names)
+            elif node.opname in ("CALL_FUNCTION", "CALL_METHOD", "CALL"):
+                if (
+                    node.arg == 0
+                    and node.opname == "CALL"
+                    and sys.version_info >= (3, 11)
+                    and len(node.stack) >= 2
+                    and isinstance(node.stack[-2], ast.FunctionDef)
+                ):
+                    # WEIRD python 3.11 behavior with lambdas ?
+                    node.arg = 1
                 args = [node.pop_stack() for _ in range(node.arg)][::-1]
                 func = node.pop_stack()
                 if isinstance(func, ast.FunctionDef):
 
                     assert len(func.body) == 2
                     tree = RewriteComprehensionArgs(args=args).visit(func)
 
                     if len(func.body) == 1 or isinstance(func.body[1], ast.Return):
                         tree = func.body[0]
                     node.add_stack(tree)
                 else:
                     node.add_stack(
                         ast.Call(
                             func=func,
-                            args=args,
-                            keywords=[],
+                            args=args[: len(args) - len(kw_names)],
+                            keywords=[
+                                ast.keyword(arg=key, value=value)
+                                for key, value in zip(kw_names, args[-len(kw_names) :])
+                            ],
                         ),
                     )
+                    kw_names = ()
             elif node.opname == "CALL_FUNCTION_KW":
                 keys = node.pop_stack().value
                 values = [node.pop_stack() for _ in range(len(keys))][::-1]
                 args = [node.pop_stack() for _ in range(node.arg - len(keys))][::-1]
                 func = node.pop_stack()
                 node.add_stack(
                     ast.Call(
@@ -1145,16 +1336,25 @@
             elif node.opname == "ROT_FOUR":
                 s = node.stack
                 s[-1], s[-2], s[-3], s[-4] = s[-2], s[-3], s[-4], s[-1]
             elif node.opname == "POP_TOP":
                 item = node.pop_stack()
                 if item and not getattr(item, "_dumped", False):
                     node.add_stmt(ast.Expr(item))
+            elif node.opname == "COPY":
+                node.stack.append(node.stack[-node.arg])
+            elif node.opname == "SWAP":
+                (node.stack[-1], node.stack[-node.arg]) = (
+                    node.stack[-node.arg],
+                    node.stack[-1],
+                )
             elif node.opname == "POP_EXCEPT":
                 node.pop_stack()
+            elif node.opname == "RETURN_GENERATOR":
+                node.add_stack(None)
             elif node.opname == "FORMAT_VALUE":
                 fmt_spec = None
                 conversion = -1
                 if node.arg & 0x03 == 0x00:
                     conversion = -1
                 elif node.arg & 0x03 == 0x01:
                     conversion = 115
@@ -1198,37 +1398,26 @@
             else:
                 raise NotImplementedError(node.opname)
 
             # Handle while loops by detecting cycles of length 1
             prev_visited = [n for n in node.prev if n.visited]
             if DEBUG:
                 print(
-                    "STACKS",
-                    "node",
-                    node,
-                    len(node.stack),
-                    node.stack,
-                    "prev",
-                    prev_visited,
-                    len(prev_visited[-1].stack) if prev_visited else 0,
-                    prev_visited[-1].stack if prev_visited else None,
+                    f"STACKS {node} (LEN {len(node.stack)}) prev visited {prev_visited}"
                 )
             if DEBUG:
                 print("LOOP HEADS", "node", node, "PREV", node.prev, "=>", loop_heads)
             while not prev_visited or len(node.stack) <= len(prev_visited[-1].stack):
-                if root.container is not node:
-                    prev = node.contract_backward()
-                else:
-                    prev = None
-                if not prev and not node.prev == {node}:
-                    break
-                if loop_heads and loop_heads[-1] is prev:
-                    loop_heads = (*loop_heads[:-1], node)
-                if node in node.jumps:
-                    node.jumps.remove(node)
+                if node in node.successors:
+                    if DEBUG:
+                        print("THIS IS A WHILE LOOP")
+                        display(node.draw())
+                    if node is node.next:
+                        node.next = None
+                    node.jumps.discard(node)
                     node.prev.remove(node)
                     body = node.stmts
                     node.stmts = []
                     node.add_stmt(
                         ast.While(
                             test=ast.Constant(value=True, kind=None),
                             body=body,
@@ -1239,63 +1428,57 @@
 
                     if loop_heads and loop_heads[-1] is node:
                         loop_heads = loop_heads[:-1]
 
                     prev_unvisited = [n for n in node.prev if not n.visited]
                     if len(prev_unvisited):
                         loop_heads = (*loop_heads, node)
+
+                if root.container is not node:
+                    prev = node.contract_backward()
+                else:
+                    prev = None
+                if not prev and not node.prev == {node}:
+                    break
+                if loop_heads and loop_heads[-1] is prev:
+                    loop_heads = (*loop_heads[:-1], node)
+
                 prev_visited = [n for n in node.prev if n.visited]
+
                 if DEBUG:
                     display(node.draw())
                 if DEBUG:
                     print(
-                        "STACKS",
-                        "node",
-                        node,
-                        len(node.stack),
-                        "prev",
-                        prev_visited,
-                        len(prev_visited[-1].stack) if prev_visited else 0,
+                        f"STACKS {node} (LEN {len(node.stack)}) prev visited {prev_visited}"
                     )
 
             if DEBUG:
                 display(node.draw())
 
             if DEBUG:
                 print("::: done", node, "|", node.next, node.jumps, "|", node.prev)
 
             if not node.next and not stop_on_jump:
                 if loop_heads:
                     jump_to_head = {
-                        n: explore_until(n, (*loop_heads, *stop_nodes))
-                        for n in node.jumps
+                        n: explore_until(n, loop_heads[::-1]) for n in node.jumps
                     }
                     if DEBUG:
                         print(
-                            "CANDIDATE JUMPS",
-                            node,
-                            "=>",
-                            jump_to_head,
-                            "LOOP HEADS",
-                            loop_heads,
+                            f"CANDIDATE JUMPS {node} => {jump_to_head} LOOP HEADS {loop_heads}"
                         )
                     same_level_jumps = [
                         jump
                         for jump, head in jump_to_head.items()
                         if head is loop_heads[-1]
                         or (head is None and len(jump.prev) == 1)
                     ]
                     if DEBUG:
                         print(
-                            "SAME LEVEL JUMPS",
-                            node,
-                            "=>",
-                            same_level_jumps,
-                            "LOOP HEADS",
-                            loop_heads,
+                            f"SAME LEVEL JUMPS {node} => {same_level_jumps} LOOP HEADS {loop_heads}"
                         )
                 else:
                     same_level_jumps = list(node.jumps)
 
                 if len(same_level_jumps) > 1:
                     warn("MULTIPLE CHOICE FOR JUMP", same_level_jumps)
                 if same_level_jumps:
@@ -1306,46 +1489,41 @@
                     node.jumps.remove(node.next)
                 # ARE WE SURE OF THIS ?
                 # If there is only one outgoing edge, jumping on a different level
                 # set it as next but don't continue exploring
                 elif len(node.jumps) == 1:
                     node.next = next(iter(node.jumps))
                     node.jumps.remove(node.next)
-                    # if node.is_virtual:
-                    #    node.next.prev.discard(node)
                     if DEBUG:
                         print("Stop after", node, "because not same level")
                     break
 
-            # if node.is_virtual:
-            #     for succ in node.jumps:
-            #         succ.prev.discard(node)
-            if node.next and not node.next.visited and node.next not in stop_nodes:
+            if node.next and not node.next.visited and node.next.is_ready:
                 node: Node = node.next
             else:
                 # if node.is_virtual and node.next:
                 #     node.next.prev.discard(node)
                 if DEBUG:
                     print(
                         "Stop after",
                         node,
                         ": next=",
                         node.next,
                         "is visited",
                         node.next.visited if node.next else "-",
-                        "| stop nodes: ",
-                        stop_nodes,
+                        "IS READY",
+                        node.next.is_ready if node.next else None,
                     )
                 break
 
         return node
 
     def run(self) -> "Node":
         """Decompile a code object"""
-        while_fusions = {}
+        while_fusions = set()
         node = self._run(while_fusions=while_fusions)
         node.stmts = [
             WhileBreakFixer(while_fusions).visit(RemoveLastContinue().visit(stmt))
             for stmt in node.stmts
         ]
 
         return node
@@ -1391,72 +1569,84 @@
             rec(succ)
 
     rec(root)
 
     return best
 
 
-def explore_until(root, stops):
-    if not stops:
+def explore_until(root, stop_nodes):
+    if not stop_nodes:
         return None
 
-    stops = list(stops)
+    stop_nodes = list(stop_nodes)
     visited = set()
 
     def rec(node):
-        if node in stops:
+        if node in stop_nodes:
             return node
 
         if node in visited:
             return None
 
         visited.add(node)
 
         results = [rec(succ) for succ in (node.next, *node.jumps) if succ is not None]
-        res = min(filter(bool, results), key=stops.index, default=None)
+        res = min(filter(bool, results), key=stop_nodes.index, default=None)
         return res
 
     return rec(root)
 
 
 def process_binding_(node, save_origin=True):
     # assert len(block.pred) <= 1
     opname = node.opname
     arg = node.arg
     code = node.code
-    idx = node.op_idx
     opname = opname.split("_")[1]
 
     origin = (
         dict(
-            _origin_offset=idx,
             _origin_node=node,
         )
         if save_origin
         else {}
     )
 
     if opname == "FAST":
         node.add_stack(
             ast.Name(
                 id=code.co_varnames[arg],
                 **origin,
             )
         )
     elif opname in ("NAME", "GLOBAL"):
-        node.add_stack(
-            ast.Name(
-                id=code.co_names[arg],
-                **origin,
+        if opname == "GLOBAL" and sys.version_info >= (3, 11):
+            # if arg & 1:
+            #    node.add_stack(ast.Constant(None))
+            node.add_stack(
+                ast.Name(
+                    id=code.co_names[arg >> 1],
+                    **origin,
+                )
+            )
+        else:
+            node.add_stack(
+                ast.Name(
+                    id=code.co_names[arg],
+                    **origin,
+                )
             )
-        )
     elif opname == "DEREF":
+        if sys.version_info < (3, 11):
+            name = (code.co_cellvars + code.co_freevars)[arg]
+        else:
+            name = (code.co_cellvars + code.co_freevars)[arg - len(code.co_varnames)]
         node.add_stack(
             ast.Name(
-                id=(code.co_cellvars + code.co_freevars)[arg],
+                id=name,
                 **origin,
             )
         )
     elif opname == "CONST":
         const_value = code.co_consts[arg]
         if isinstance(const_value, frozenset):
             const_value = set(const_value)
@@ -1511,22 +1701,23 @@
         else:
             multi_targets = [target]
 
         try:
             is_multi_assignment = (
                 len(last_stmts)
                 and isinstance(last_stmts[-1], ast.Assign)
-                and get_origin(value)[1] <= get_origin(last_stmts[-1].targets)[1]
+                and get_origin(value).op_idx
+                <= get_origin(last_stmts[-1].targets).op_idx
             )
             if DEBUG:
                 print(
                     f"ORIGIN of {ast.dump(value)}",
-                    get_origin(value)[1],
+                    get_origin(value),
                     f"vs ORIGIN of last {ast.dump(last_stmts[-1])}",
-                    get_origin(last_stmts[-1].targets)[1],
+                    get_origin(last_stmts[-1].targets),
                 )
         except Exception:
             is_multi_assignment = False
 
         if DEBUG:
             print(
                 "VALUE",
@@ -1580,194 +1771,14 @@
             ast.Assign(
                 targets=multi_targets,
                 value=value,
             ),
         )
 
 
-def process_try_(node, loop_heads, stop_nodes, while_fusions):
-    next_node = node.next
-    [jump_node] = node.jumps
-
-    old_next_node = next_node
-    old_jump_node = jump_node
-    jump_node.stack = [
-        *node.stack,
-        None,
-        None,
-        ExceptionPlaceholder(_dumped=True),
-        None,
-    ]
-
-    meet_nodes = list(
-        lowest_common_successors(
-            next_node,
-            jump_node,
-            stop_nodes={*stop_nodes, node},
-        )
-    )
-    if DEBUG:
-        print(
-            "TRY BLOCK", node, "MEET", meet_nodes, "(STOP at", {*stop_nodes, node}, ")"
-        )
-    assert len(meet_nodes) <= 1
-
-    before = (next_node, jump_node)
-    next_node = next_node._run(
-        stop_nodes={*stop_nodes, *meet_nodes, node},
-        loop_heads=loop_heads,
-        while_fusions=while_fusions,
-    )
-    jump_node = jump_node._run(
-        stop_nodes={*stop_nodes, *meet_nodes, node},
-        loop_heads=loop_heads,
-        while_fusions=while_fusions,
-    )
-    if (
-        len(meet_nodes)
-        and meet_nodes[0].opname == "POP_BLOCK"
-        and meet_nodes[0] not in stop_nodes
-    ):
-        finally_node = meet_nodes[0]
-        old_finally_node = finally_node
-        old_prev, finally_node.prev = finally_node.prev, {node}
-        print("FOUND FINALLY", finally_node, "STOP AT", {*stop_nodes, node})
-        finally_node = finally_node._run(
-            stop_nodes={*stop_nodes, node},
-            loop_heads=loop_heads,
-            while_fusions=while_fusions,
-            stop_on_jump=True,
-        )
-        finally_node.prev = old_prev
-    else:
-        finally_node = old_finally_node = None
-
-    if DEBUG:
-        print("TRY", node, "MEET", meet_nodes)
-    if DEBUG:
-        print("TRY", node, "BEFORE succ", before, "-> AFTER succ", next_node, jump_node)
-
-    handlers = []
-    finalbody = []
-    if (
-        jump_node.stmts
-        and isinstance(jump_node.stmts[0], ast.If)
-        and isinstance(jump_node.stmts[0].test, ExceptionMatch)
-    ):
-        except_stmts = list(jump_node.stmts[0].body)
-        if isinstance(except_stmts[0], ast.Assign) and isinstance(
-            except_stmts[0].value, ExceptionPlaceholder
-        ):
-            name = except_stmts.pop(0).targets[0].id
-            # To handle auto-generated try/finally block
-            # with e = None; del e; instruction at the end of the generated try body
-            except_stmts = list(except_stmts[0].body)
-            i = next(
-                i
-                for i, s in enumerate(except_stmts)
-                if isinstance(s, ast.Delete) and s.targets[0].id == name
-            )
-            except_stmts = except_stmts[: i - 1] + except_stmts[i + 1 :]
-        else:
-            name = None
-        handlers.append(
-            ast.ExceptHandler(
-                type=jump_node.stmts[0].test.value,
-                name=name,
-                body=except_stmts,
-            )
-        )
-    elif isinstance(jump_node.stmts[-1], Reraise):
-        finalbody = jump_node.stmts[:-1]
-    else:
-        handlers.append(
-            ast.ExceptHandler(
-                type=None,
-                name=None,
-                body=jump_node.stmts,
-            )
-        )
-    if finally_node:
-        finalbody = finally_node.stmts
-
-    if (
-        next_node.stmts
-        and isinstance(next_node.stmts[0], ast.Try)
-        and not getattr(next_node.stmts[0], "_try_was_deduplicated", False)
-        and next_node.stmts[0].handlers
-        and next_node.stmts[0].finalbody
-    ):
-        print("DEDUPLICATING TRY", next_node.stmts[0], "WITH", node)
-        next_node.stmts[0]._try_was_deduplicated = True
-        node.stmts.extend(next_node.stmts)
-    else:
-        node.add_stmt(
-            ast.Try(
-                body=next_node.stmts if next_node else [ast.Pass()],
-                handlers=handlers,
-                orelse=[],  # TODO
-                finalbody=finalbody,  # TODO
-            )
-        )
-
-    # noinspection PyTypeChecker
-    successors: Set[Node] = {
-        *((next_node.next, *next_node.jumps) if next_node else (node.next,)),
-        *((jump_node.next, *jump_node.jumps) if jump_node else node.jumps),
-        *((finally_node.next, *finally_node.jumps) if finally_node else ()),
-    } - {
-        None
-    }  # type: ignore
-    discarded_successors = {
-        n
-        for n in (
-            next_node,
-            jump_node,
-            old_next_node,
-            old_jump_node,
-            finally_node,
-            old_finally_node,
-        )
-        if n and n.visited
-    }
-    if DEBUG:
-        print("TRY SUCC", successors, "-", discarded_successors)
-    if DEBUG:
-        print("TRY PREV", node.prev)
-    successors = successors - discarded_successors
-
-    jump_nodes = successors
-    for succ in successors:
-        if DEBUG:
-            print(
-                "TRY",
-                node,
-                ": REBINDING SUCCESSOR",
-                succ,
-                "=>",
-                succ.prev,
-                "->",
-                succ.prev - {next_node, jump_node} | {node},
-            )
-        succ.prev = (succ.prev - discarded_successors) | {node}
-    for n in discarded_successors:
-        for p in n.prev:
-            if p.next in discarded_successors:
-                p.next = node
-            p.jumps = {node if j in discarded_successors else j for j in p.jumps}
-        n.prev = n.prev - discarded_successors
-    node.next = None
-    node.jumps = jump_nodes
-    if DEBUG:
-        print("TRY", node, node.stack)
-
-    if DEBUG:
-        display(node.draw())
-
-
 def contract_jumps(root):
     queue = [root]
     seen = set()
 
     while queue:
         node = queue.pop(0)
```

### Comparing `pygetsource-0.1.1/pygetsource/factory.py` & `pygetsource-0.2.0/pygetsource/factory.py`

 * *Files identical despite different names*

### Comparing `pygetsource-0.1.1/pygetsource.egg-info/PKG-INFO` & `pygetsource-0.2.0/pygetsource.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pygetsource
-Version: 0.1.1
-Summary: Decompiler written in Python for Python
+Version: 0.2.0
+Summary: A Python 3 decompiler
 Author-email: Perceval Wajsburt <perceval.wajsburt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Perceval Wajsburt
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,29 +23,44 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/perceval/pygetsource/
 Project-URL: repository, https://github.com/perceval/pygetsource/
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Disassemblers
+Classifier: Topic :: Software Development :: Pre-processors
+Classifier: Topic :: Utilities
 Requires-Python: <4.0,>=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Codecov](https://img.shields.io/codecov/c/github/percevalw/pygetsource?logo=codecov&style=flat-square)](https://codecov.io/gh/percevalw/pygetsource)
 [![PyPI](https://img.shields.io/pypi/v/pygetsource?color=blue&style=flat-square)](https://pypi.org/project/pygetsource/)
 ![Tests](https://img.shields.io/github/actions/workflow/status/percevalw/pygetsource/tests.yml?branch=main&label=tests&style=flat-square)
 [![Code style: black](https://img.shields.io/badge/code_style-black-black?style=flat-square)](https://github.com/psf/black)
 [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat-square)](https://opensource.org/licenses/MIT)
 
 
 # pygetsource
 
-`pygetsource` is a Python decompiler, aiming to convert compiled bytecode instructions back into Python code.
+`pygetsource` is a decompiler for Python 3, aiming to convert compiled bytecode instructions back into Python code.
 
 ## Overview
 
 When Python reads code, it first converts the instructions into bytecode. For instance:
 
 ```python
 a = 2
@@ -58,15 +73,15 @@
 STORE_FAST 0
 ```
 
 The latter form is typically stored in `.pyc` files and in the `__code__` attribute of function objects. The goal of `pygetsource` is to reverse this process.
 
 The project takes its name from the `inspect.getsource` function, which returns the source code of a function, but it is not always applicable, as explained above.
 
-`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.10. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
+`pygetsource` is still in development. It should be able to recover the source code of simple functions for various programs from Python 3.7 to Python 3.11. It is not yet able to recover the source code of classes, import statements, try/except/match/with blocks, and does not support Python 2. While functional, the codebase has not been optimized and is in need of significant refactoring.
 
 Finally, this software is distributed under the permissive MIT license.
 
 ## Installation
 
 Install the package using pip:
 
@@ -120,23 +135,24 @@
 
 ## When is this useful ?
 
 `pygetsource` proves useful when you need to recover the source code from a `.pyc` file, or when you want to get the source code of a function created through an eval statement or a lambda syntax. Indeed, running `inspect.getsource` fail in the latter case since the origin file of the function is either not available, or Python does not provide the exact boundaries, which are required in the case of lambda functions.
 
 ## Alternatives
 
-[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above.
+[uncompyle6](https://github.com/rocky/python-uncompyle6) is a Python decompiler that supports Python 2 and 3 up to Python 3.8. It uses a grammar-based approach to rebuild code from bytecode patterns. This approach is less effective for higher versions that introduce various bytecode optimizations, especially regarding complex control structures like loops, or the example given above. At the moment, it supports a larger range of Python syntaxes (such as with blocks or try/excepts).
 It is also licensed under a copyleft GPL license, making it less suitable for larger projects with permissive licenses.
 
 [decompyle++ (pycdc)](https://github.com/zrax/pycdc) uses a state machine approach to build an AST iteratively by processing bytecode instructions. It's written in C++ and supports more Python versions than uncompyle6, but has more trouble decompiling  complex control structures like nested loops, break patterns, comprehensions, or the example given above. It also uses the copyleft GPL license.
 
 ## How does it work ?
 
 `pygetsource` uses a distinct approach. The bytecode instructions are initially converted into a directed graph, representing the program's flow. This graph is then iteratively reduced, processing each node based on its opcode, argument, and position and generating the [AST](https://docs.python.org/3/library/ast.html) as it goes.
-This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements.
+This method allows us to rely more on high-level patterns and less on Python’s idiosyncrasies when recreating complex structures like nested loops or break/return statements, and handle Python versions from 3.7 to 3.11 with the same codebase.
+
 In constrast with [uncompyle6](https://github.com/rocky/python-uncompyle6) and [pycdc](https://github.com/zrax/pycdc), `pygetsource` uses the `ast` and `astunparse` libraries to generate the source code from the generated AST.
 
 Here is an example of a graph being reduced:
 
 ![Graph reduction](./docs/graph-example.svg)
```

### Comparing `pygetsource-0.1.1/tests/test_py37.py` & `pygetsource-0.2.0/tests/test_py37.py`

 * *Files 11% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 def test_if():
     a = 1
     if a == 1:
         a = 2
 
 
 @make_test_idem
+def test_empty_if():
+    a = 1
+    if a == 1:
+        pass
+
+
+@make_test_idem
 def test_if_not():
     a = 1
     if not a == 1:
         a = 2
 
 
 @make_test_idem
@@ -819,7 +826,147 @@
 @make_test_idem
 def test_while_true_if_if_continue():
     while True:
         if x:
             if y:
                 continue
         return line
+
+
+@make_test_idem
+def test_while_test_if_else_break():
+    while test:
+        if a:
+            x = 2
+        else:
+            x = 3
+            break
+    return "a"
+
+
+@make_test_idem
+def test_while_if_if_elif_else():
+    while test:
+        if a:
+            if i == 0:
+                x = 1
+            elif i == 1:
+                x = 0
+                break
+            else:
+                i = 3
+                continue
+
+    x = 2
+    y = 3
+    return "a"
+
+
+@make_test_idem
+def test_while_while_if():
+    while z:
+        while test:
+            if i == 0:
+                x = 1
+            elif i == 1:
+                x = 0
+                continue
+            else:
+                i = 3
+                continue
+
+    u = 3
+    return u
+
+
+@make_test_idem
+def test_if_and_else():
+    if x and y:
+        x = 3
+    else:
+        y = 3
+
+    a = 3
+    return a
+
+
+@make_test_idem
+def test_if_and():
+    if x and y:
+        return 1
+
+
+@make_test_idem
+def test_if_or_else():
+    if x or y:
+        x = 3
+    else:
+        y = 3
+
+    a = 3
+    return a
+
+
+@make_test_idem
+def test_if_or():
+    if x or y:
+        return 1
+
+
+@make_test_idem
+def test_if_mix_bool_else():
+    if (x or y or z) and (a or b):
+        x = 3
+    else:
+        y = 3
+
+
+@make_test_idem
+def test_if_mix_bool_2_else():
+    if (x and y and z) or (a and b):
+        x = 3
+    else:
+        y = 3
+
+
+@make_test_idem
+def test_while_bool():
+    while a and b:
+        x = 2
+
+    u = 3
+    return "u"
+
+
+@make_test_idem
+def test_while_while_bool():
+    while a and b:
+        while test:
+            x = 2
+
+    u = 3
+    return "u"
+
+
+@make_test_idem
+def test_while_while_bool_mix():
+    while (x and y and z) or (a and b):
+        while test:
+            x = 2
+
+    u = 3
+    return "u"
+
+
+@make_test_idem
+def test_bool_and_of_or_assign():
+    z = (x and y and z) or (a and b) or (c and d)
+
+
+@make_test_idem
+def test_bool_or_of_and_assign():
+    z = (x or y or z) and (a or b) and (c or d)
+
+
+@make_test_idem
+def test_bool_target_in_comprehension():
+    return [(x or y or z) and (a or b) and (c or d) for i in range(10)]
```

### Comparing `pygetsource-0.1.1/tests/test_rebuild.py` & `pygetsource-0.2.0/tests/test_rebuild.py`

 * *Files identical despite different names*

