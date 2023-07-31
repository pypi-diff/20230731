# Comparing `tmp/meth-1.1.0.tar.gz` & `tmp/meth-1.2.0.tar.gz`

## Comparing `meth-1.1.0.tar` & `meth-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 meth-1.1.0/test.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 meth-1.1.0/examples/calculator.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 meth-1.1.0/meth/__init__.py
--rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 meth-1.1.0/meth/builtins.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 meth-1.1.0/meth/error.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 meth-1.1.0/meth/interpreter.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 meth-1.1.0/meth/lexer.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 meth-1.1.0/meth/nodes.py
--rw-r--r--   0        0        0     5996 2020-02-02 00:00:00.000000 meth-1.1.0/meth/parser.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 meth-1.1.0/meth/token.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 meth-1.1.0/meth/utils.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/__init__.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/simplify.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 meth-1.1.0/meth/functions/stringify.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 meth-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 meth-1.1.0/tests/test_evaluate.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 meth-1.1.0/tests/test_simplify.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 meth-1.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 meth-1.1.0/LICENSE
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 meth-1.1.0/README.md
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 meth-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 meth-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 meth-1.2.0/test.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 meth-1.2.0/examples/calculator.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 meth-1.2.0/meth/__init__.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 meth-1.2.0/meth/builtins.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 meth-1.2.0/meth/error.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 meth-1.2.0/meth/interpreter.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 meth-1.2.0/meth/lexer.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 meth-1.2.0/meth/nodes.py
+-rw-r--r--   0        0        0     5700 2020-02-02 00:00:00.000000 meth-1.2.0/meth/parser.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 meth-1.2.0/meth/token.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 meth-1.2.0/meth/utils.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 meth-1.2.0/meth/functions/__init__.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 meth-1.2.0/meth/functions/simplify.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 meth-1.2.0/meth/functions/stringify.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 meth-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 meth-1.2.0/tests/test_evaluate.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 meth-1.2.0/tests/test_simplify.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 meth-1.2.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 meth-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 meth-1.2.0/README.md
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 meth-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 meth-1.2.0/PKG-INFO
```

### Comparing `meth-1.1.0/meth/__init__.py` & `meth-1.2.0/meth/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     def set_var(self, name: str, value: int | float) -> None:
         """
         Set the value of a variable.
 
         Args:
             name: str
-                Name of the variable to set.
+                Name of the variable to set. Has to be a single character.
             value: int | float
                 Value to set the variable with.
 
         Returns: None
         """
         if len(name) > 1:
             raise ValueError("Name can only be of length one.")
```

### Comparing `meth-1.1.0/meth/builtins.py` & `meth-1.2.0/meth/builtins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from functools import lru_cache
 from typing import Any
 import math
 
 
 def meth_ln(x: float | int):
     return math.log(x)
 
@@ -67,35 +68,34 @@
     "floor": math.floor,
     "ceil": math.ceil,
     "round": round,
     "min": meth_min,
     "max": meth_max
 }
 
+ALL_BUILTINS = BUILTINS | CONSTANTS | SPECIAL_CONST_SYM
+
+# makes it 0.02s faster
+@lru_cache(maxsize=len(ALL_BUILTINS))
 def is_builtin(name: str) -> bool:
     """
     Checks to see if name is a builtin.
 
     Args:
         name: str
             Name to check.
 
     Returns: bool
     """
-    return name in BUILTINS or name in CONSTANTS or name in SPECIAL_CONST_SYM
+    return name in ALL_BUILTINS
 
 def get_builtin(name: str) -> Any:
     """
     Get builtin from name.
     
     Args:
         name: str
             Name of builtin.
 
     Returns: Any | None if not found
     """
-    if name in BUILTINS:
-        return BUILTINS[name]
-    elif name in CONSTANTS:
-        return CONSTANTS[name]
-    elif name in SPECIAL_CONST_SYM:
-        return SPECIAL_CONST_SYM[name]
+    return ALL_BUILTINS.get(name)
```

### Comparing `meth-1.1.0/meth/interpreter.py` & `meth-1.2.0/meth/interpreter.py`

 * *Files 22% similar despite different names*

```diff
@@ -44,56 +44,76 @@
                 Tree to interpret.
 
         Returns: int | float | None
         """
         return self._visit(ast)
 
     def _visit(self, node: BaseNode):
-        return getattr(self, "_visit_" + type(node).__name__)(node)
+        """Visit a node."""
+        try:
+            visit_func = getattr(self, "_visit_" + type(node).__name__)
+        except AttributeError:
+            raise error.NotImplError(f"Unexpected type {type(node)}.")
+
+        return visit_func(node)
 
     def _visit_Token(self, token: Token):
+        """Visit a token."""
         if token.type == TT_IDENTIFIER:
             is_var = token.value in self.vars
             if not is_var and (builtin := get_builtin(token.value)) is None:
                 raise error.VarNotDefinedError(f"{token.value} is not defined.")
 
             return self.vars[token.value] if is_var else builtin
 
         return token.value
 
+    def _math_PLUS(self, node):
+        return self._visit(node.left) + self._visit(node.right)
+
+    def _math_MINUS(self, node):
+        return self._visit(node.left) - self._visit(node.right)
+
+    def _math_MULTIPLY(self, node):
+        return self._visit(node.left) * self._visit(node.right)
+
+    def _math_DIVIDE(self, node):
+        return self._visit(node.left) / self._visit(node.right)
+
+    def _math_POWER(self, node):
+        return self._visit(node.left) ** self._visit(node.right)
+
+    def _math_MODULO(self, node):
+        return self._visit(node.left) % self._visit(node.right)
+
     def _visit_BinaryOpNode(self, node: BaseNode):
-        if node.value == TT_PLUS:
-            return self._visit(node.left) + self._visit(node.right)
-        elif node.value == TT_MINUS:
-            return self._visit(node.left) - self._visit(node.right)
-        elif node.value == TT_MUL:
-            return self._visit(node.left) * self._visit(node.right)
-        elif node.value == TT_DIV:
-            return self._visit(node.left) / self._visit(node.right)
-        elif node.value == TT_MOD:
-            return self._visit(node.left) % self._visit(node.right)
-        elif node.value == TT_POW:
-            return self._visit(node.left) ** self._visit(node.right)
-        else:
+        """Visit a binary operation node."""
+        try:
+            return getattr(self, f"_math_{node.value}")(node)
+        except AttributeError:
             raise error.NotImplError(f"{node.value} is unimplemented.")
 
     def _visit_UnaryOpNode(self, node: BaseNode):
-        value = self._visit(node.left)
-        return value if node.value == TT_PLUS else -value
+        """Visit a unary operation node."""
+        return -self._visit(node.left)
 
     def _visit_AssignNode(self, node: BaseNode):
-        if node.left == TT_IDENTIFIER:
+        """Visit a assignment node."""
+        if type(node.left) == Token and node.left.is_type(TT_IDENTIFIER):
             self.vars[node.left.value] = self._visit(node.right)
         elif type(node.left) == FunctionNode:
             self.vars[node.left.value.value] = Function(node.left, node.right)
         else:
             return self._visit(node.left)
 
     def _visit_FunctionNode(self, node: BaseNode):
-        if type(value := self._visit(node.value)) == Function:
+        """Visit a function node."""
+        value = self._visit(node.value)
+
+        if type(value) == Function:
             return value(*[self._visit(arg) for arg in node.left])
         elif callable(value):
             if (plen := len(signature(value).parameters)) != len(node.left):
                 raise error.SyntaxError(
                     f"{value}() takes in {plen} arguments but {len(node.left)} were given."
                 )
```

### Comparing `meth-1.1.0/meth/lexer.py` & `meth-1.2.0/meth/lexer.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,22 +28,22 @@
         self.expr = expr
         self.i = -1
         self._next()
 
         tokens = []
 
         while self.curr:
-            if self.curr == " ":
+            if self.curr in " \t\r\n":
                 self._next()
             elif self.curr in string.digits:
                 tokens.append(self._number())
             elif self.curr in string.ascii_letters:
                 tokens += self._identifier()
-            elif self.curr in OPERATORS:
-                tokens.append(Token(OPERATORS[self.curr]))
+            elif self.curr in SYMBOLS:
+                tokens.append(Token(SYMBOLS[self.curr]))
                 self._next()
             elif self.curr in SPECIAL_CONST_SYM:
                 tokens.append(Token(TT_IDENTIFIER, self.curr))
                 self._next()
             else:
                 raise error.SyntaxError(f"Invalid character '{self.curr}'")
```

### Comparing `meth-1.1.0/meth/nodes.py` & `meth-1.2.0/meth/nodes.py`

 * *Files identical despite different names*

### Comparing `meth-1.1.0/meth/utils.py` & `meth-1.2.0/meth/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,23 @@
         stop_at: list[TT_] = []
             List of token types to stop at.
 
     Return: Node
     """
     node = tree
 
-    while (
-        getattr((n := getattr(node, "left", None)), "left", None)
-        and n.value not in stop_at
-        and (stop_at_paren or not n.is_paren)
-    ):
-        node = node.left
+    try:
+        while (
+            (n := node.left).left
+            and n.value not in stop_at
+            and (stop_at_paren or not n.is_paren)
+        ):
+            node = node.left
+    except AttributeError:
+        pass
 
     return node
 
 
 def get_leaf_node_right(
     tree: BaseNode, stop_at_paren: bool = False, stop_at: list = []
 ) -> BaseNode:
@@ -44,20 +47,23 @@
         stop_at: list[TT_] = []
             List of token types to stop at.
 
     Return: Node
     """
     node = tree
 
-    while (
-        getattr((n := getattr(node, "right", None)), "right", None)
-        and n.value not in stop_at
-        and (stop_at_paren or not n.is_paren)
-    ):
-        node = node.right
+    try:
+        while (
+            (n := node.right).right
+            and n.value not in stop_at
+            and (stop_at_paren or not n.is_paren)
+        ):
+            node = node.right
+    except AttributeError:
+        pass
 
     return node
 
 
 def get_from_depth_left(tree: BaseNode, depth: int) -> BaseNode:
     """
     Get the leftest node of a tree using a depth.
```

### Comparing `meth-1.1.0/meth/functions/simplify.py` & `meth-1.2.0/meth/functions/simplify.py`

 * *Files identical despite different names*

### Comparing `meth-1.1.0/meth/functions/stringify.py` & `meth-1.2.0/meth/functions/stringify.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..token import *
 from ..nodes import *
+from .. import error
 
 TT_CONV = {
     TT_LBRACKET: "(",
     TT_RBRACKET: ")",
     TT_EQUAL: "=",
     TT_COMMA: ",",
     TT_PLUS: "+",
```

### Comparing `meth-1.1.0/tests/test_evaluate.py` & `meth-1.2.0/tests/test_evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,7 +33,11 @@
 
     def test_unary_mul_var(self):
         self.eval.evaluate("x = 3")
         self.assertEqual(self.eval.evaluate("-10x"), -30)
 
     def test_bracket_mul(self):
         self.assertEqual(self.eval.evaluate("(2 * 2)(2 + 1)"), 12)
+
+    def test_func(self):
+        self.eval.evaluate("f(x) = 2x + sqrt(9)")
+        self.assertEqual(self.eval.evaluate("f(5)"), 13)
```

### Comparing `meth-1.1.0/tests/test_simplify.py` & `meth-1.2.0/tests/test_simplify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from meth import *
+from meth.functions.simplify import simplify
+from meth.nodes import *
 import unittest
 
 
 class SimplifyTest(unittest.TestCase):
     def test_mul_var_same(self):
         # 2x + 3x = 5x
         self.assertEqual(
```

### Comparing `meth-1.1.0/LICENSE` & `meth-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meth-1.1.0/README.md` & `meth-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `meth-1.1.0/PKG-INFO` & `meth-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: meth
-Version: 1.1.0
+Version: 1.2.0
 Summary: A mathematical expression parser and evaluator.
 Project-URL: Homepage, https://github.com/sertdfyguhi/meth
 Project-URL: Bug Tracker, https://github.com/sertdfyguhi/meth/issues
 Author: sertdfyguhi
 License-File: LICENSE
 Keywords: evaluator,math,math evaluator,math parser,mathematical,parser,parsing
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.2
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 
 # meth: A mathematical expression parser.
 
 A python package to parse and evaluate mathematical expressions.
 
 # Installation
```

