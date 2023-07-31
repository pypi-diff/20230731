# Comparing `tmp/inline_snapshot-0.3.1.tar.gz` & `tmp/inline_snapshot-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inline_snapshot-0.3.1.tar", max compression
+gzip compressed data, was "inline_snapshot-0.3.2.tar", max compression
```

## Comparing `inline_snapshot-0.3.1.tar` & `inline_snapshot-0.3.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.3.1/LICENSE
--rw-r--r--   0        0        0     3075 2023-07-13 22:23:21.207977 inline_snapshot-0.3.1/README.md
--rw-r--r--   0        0        0       86 2023-07-14 07:14:59.218737 inline_snapshot-0.3.1/inline_snapshot/__init__.py
--rw-r--r--   0        0        0      248 2023-07-12 20:13:28.911699 inline_snapshot-0.3.1/inline_snapshot/_format.py
--rw-r--r--   0        0        0    14999 2023-07-14 07:01:48.261328 inline_snapshot-0.3.1/inline_snapshot/_inline_snapshot.py
--rw-r--r--   0        0        0     5448 2023-07-13 18:14:22.460873 inline_snapshot-0.3.1/inline_snapshot/_rewrite_code.py
--rw-r--r--   0        0        0     5445 2023-07-09 14:55:53.631461 inline_snapshot-0.3.1/inline_snapshot/pytest_plugin.py
--rw-r--r--   0        0        0     1620 2023-07-14 07:14:59.218737 inline_snapshot-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4455 1970-01-01 00:00:00.000000 inline_snapshot-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-20 18:24:16.714717 inline_snapshot-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3150 2023-07-31 17:24:39.895919 inline_snapshot-0.3.2/README.md
+-rw-r--r--   0        0        0       86 2023-07-31 20:43:59.217532 inline_snapshot-0.3.2/inline_snapshot/__init__.py
+-rw-r--r--   0        0        0      248 2023-07-19 06:20:13.370509 inline_snapshot-0.3.2/inline_snapshot/_format.py
+-rw-r--r--   0        0        0    16124 2023-07-31 20:43:59.217532 inline_snapshot-0.3.2/inline_snapshot/_inline_snapshot.py
+-rw-r--r--   0        0        0     5468 2023-07-31 17:24:39.919919 inline_snapshot-0.3.2/inline_snapshot/_rewrite_code.py
+-rw-r--r--   0        0        0     5445 2023-07-19 06:48:44.626465 inline_snapshot-0.3.2/inline_snapshot/pytest_plugin.py
+-rw-r--r--   0        0        0     1862 2023-07-31 20:43:59.217532 inline_snapshot-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 inline_snapshot-0.3.2/PKG-INFO
```

### Comparing `inline_snapshot-0.3.1/LICENSE` & `inline_snapshot-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.1/README.md` & `inline_snapshot-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # inline-snapshot
 
 [![Docs](https://img.shields.io/badge/docs-mkdocs-green)](https://15r10nk.github.io/inline-snapshot/)
 [![pypi version](https://img.shields.io/pypi/v/inline-snapshot.svg)](https://pypi.org/project/inline-snapshot/)
+![Python Versions](https://img.shields.io/pypi/pyversions/inline-snapshot)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/inline-snapshot)
 [![coverage](https://img.shields.io/badge/coverage-100%25-blue)](https://15r10nk.github.io/inline-snapshot/contributing/#coverage)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
 
 > *create and update inline snapshots in your code.*
 
 ## Installation
```

### Comparing `inline_snapshot-0.3.1/inline_snapshot/_inline_snapshot.py` & `inline_snapshot-0.3.2/inline_snapshot/_inline_snapshot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import ast
 import contextlib
 import copy
 import inspect
 import io
 import token
 import tokenize
+from collections import namedtuple
 from pathlib import Path
 from typing import Any
 from typing import Dict  # noqa
 from typing import overload
 from typing import Tuple  # noqa
 from typing import TypeVar
 
@@ -159,15 +160,17 @@
 
         return self._visible_value() == other
 
     def _needs_fix(self):
         return self._old_value is not undefined and self._old_value != self._new_value
 
     def get_result(self, flags):
-        return self._new_value
+        if flags.fix and self._needs_fix() or flags.create and self._needs_create():
+            return self._new_value
+        return self._old_value
 
 
 class MinMaxValue(GenericValue):
     """generic implementation for <=, >="""
 
     @staticmethod
     def cmp(a, b):
@@ -193,21 +196,15 @@
 
     def _needs_fix(self):
         if self._old_value is undefined:
             return False
         return not self.cmp(self._old_value, self._new_value)
 
     def get_result(self, flags):
-        if (
-            flags.fix
-            and flags.trim
-            or flags.create
-            and self._old_value == undefined
-            or flags.update
-        ):
+        if flags.create and self._needs_create():
             return self._new_value
 
         if flags.fix and self._needs_fix():
             return self._new_value
 
         if flags.trim and self._needs_trim():
             return self._new_value
@@ -283,33 +280,27 @@
 
     def _needs_fix(self):
         if self._old_value is undefined:
             return False
         return any(item not in self._old_value for item in self._new_value)
 
     def get_result(self, flags):
-        if (
-            flags.fix
-            and flags.trim
-            or flags.create
-            and self._old_value == undefined
-            or flags.update
-        ):
+        if (flags.fix and flags.trim) or (flags.create and self._needs_create()):
             return self._new_value
 
         if self._old_value is not undefined:
             if flags.fix:
                 return self._old_value + [
                     v for v in self._new_value if v not in self._old_value
                 ]
 
             if flags.trim:
                 return [v for v in self._old_value if v in self._new_value]
 
-        assert False, "unreachable"
+        return self._old_value
 
 
 class DictValue(GenericValue):
     def __getitem__(self, index):
         if self._new_value is undefined:
             self._new_value = {}
 
@@ -431,15 +422,15 @@
             assert node.func.id == "snapshot"
             snapshots[key] = Snapshot(obj, expr)
         found_snapshots.append(snapshots[key])
 
     return snapshots[key]._value
 
 
-ignore_tokens = (token.NEWLINE, token.ENDMARKER)
+ignore_tokens = (token.NEWLINE, token.ENDMARKER, token.NL)
 
 
 # based on ast.unparse
 def _str_literal_helper(string, *, quote_types):
     """Helper for writing string literals, minimizing escapes.
 
     Returns the tuple (string literal to write, possible quote types).
@@ -480,14 +471,17 @@
     """Write string literal value with a best effort attempt to avoid
     backslashes."""
     string, quote_types = _str_literal_helper(string, quote_types=['"""', "'''"])
     quote_type = quote_types[0]
     return f"{quote_type}{string}{quote_type}"
 
 
+simple_token = namedtuple("simple_token", "type,string")
+
+
 class Snapshot:
     def __init__(self, value, expr):
         self._expr = expr
         self._value = Value(value)
 
     @property
     def _filename(self):
@@ -506,17 +500,17 @@
                 if isinstance(s, str) and "\n" in s:
                     # unparse creates a triple quoted string here,
                     # because it thinks that the string should be a docstring
                     tripple_quoted_string = triple_quote(s)
 
                     assert ast.literal_eval(tripple_quoted_string) == s
 
-                    return tok.type, tripple_quoted_string
+                    return simple_token(tok.type, tripple_quoted_string)
 
-            return (tok.type, tok.string)
+            return simple_token(tok.type, tok.string)
 
         return [
             map_string(t)
             for t in tokenize.generate_tokens(input.readline)
             if t.type not in ignore_tokens
         ]
 
@@ -531,18 +525,19 @@
         assert tokens[-1].string == ")"
 
         change.set_tags("inline_snapshot")
 
         needs_fix = self._value._needs_fix()
         needs_create = self._value._needs_create()
         needs_trim = self._value._needs_trim()
+        needs_update = self._needs_update()
 
         if (
             _update_flags.update
-            and not (needs_fix or needs_create or needs_trim)
+            and needs_update
             or _update_flags.fix
             and needs_fix
             or _update_flags.create
             and needs_create
             or _update_flags.trim
             and needs_trim
         ):
@@ -555,31 +550,63 @@
             change.replace(
                 (end_of(tokens[1]), start_of(tokens[-1])),
                 text,
                 filename=self._filename,
             )
 
     def _current_tokens(self):
+        if not self._expr.node.args:
+            return []
+
         return [
-            (t.type, t.string)
+            simple_token(t.type, t.string)
             for t in self._expr.source.asttokens().get_tokens(self._expr.node.args[0])
             if t.type not in ignore_tokens
         ]
 
+    def _normalize_strings(self, token_sequence):
+        """Normalize string concattenanion.
+
+        "a" "b" -> "ab"
+        """
+
+        current_string = None
+        for t in token_sequence:
+            if (
+                t.type == token.STRING
+                and not t.string.startswith(("'''", '"""', "b'''", 'b"""'))
+                and t.string.startswith(("'", '"', "b'", 'b"'))
+            ):
+                if current_string is None:
+                    current_string = ast.literal_eval(t.string)
+                else:
+                    current_string += ast.literal_eval(t.string)
+
+                continue
+
+            if current_string is not None:
+                yield (token.STRING, repr(current_string))
+                current_string = None
+
+            yield t
+
+        if current_string is not None:
+            yield (token.STRING, repr(current_string))
+
+    def _needs_update(self):
+        return self._expr is not None and [] != list(
+            self._normalize_strings(self._current_tokens())
+        ) != list(self._normalize_strings(self._value_to_token(self._value._old_value)))
+
     @property
     def _flags(self):
         s = set()
         if self._value._needs_fix():
             s.add("fix")
         if self._value._needs_trim():
             s.add("trim")
         if self._value._needs_create():
             s.add("create")
-
-        if (
-            "create" not in s
-            and self._expr is not None
-            and self._current_tokens() != self._value_to_token(self._value._old_value)
-        ):
+        if self._value._old_value is not undefined and self._needs_update():
             s.add("update")
 
         return s
```

### Comparing `inline_snapshot-0.3.1/inline_snapshot/_rewrite_code.py` & `inline_snapshot-0.3.2/inline_snapshot/_rewrite_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
             changes.update(change.change_id for change in file.replacements)
         return len(changes)
 
     def fix_all(self, tags=()):
         for file in self._source_files.values():
             file.rewrite()
 
-    def dump(self):
+    def dump(self):  # pragma: no cover
         for file in self._source_files.values():
             print("file:", file.filename)
             for change in file.replacements:
                 print("  change:", change)
 
 
 global_recorder = ChangeRecorder()
```

### Comparing `inline_snapshot-0.3.1/inline_snapshot/pytest_plugin.py` & `inline_snapshot-0.3.2/inline_snapshot/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `inline_snapshot-0.3.1/pyproject.toml` & `inline_snapshot-0.3.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
+[tool.commitizen]
+changelog_incremental = true
+major_version_zero = true
+tag_format = "v$major.$minor.$patch$prerelease"
+update_changelog_on_bump = true
+version_files = [
+  "inline_snapshot/__init__.py:version"
+]
+version_provider = "poetry"
+
 [tool.coverage.report]
 exclude_lines = ["pragma: no cover", "assert False", "raise NotImplemented", "\\.\\.\\."]
 
 [tool.coverage.run]
 branch = true
 data_file = "$TOP/.coverage"
 parallel = true
@@ -24,15 +34,15 @@
   "Framework :: Pytest"
 ]
 description = "golden master/snapshot/approval testing library which puts the values right into your source code"
 license = "MIT"
 name = "inline-snapshot"
 readme = "README.md"
 repository = "https://github.com/15r10nk/inline-snapshots"
-version = "0.3.1"
+version = "0.3.2"
 
 [tool.poetry.dependencies]
 asttokens = "^2.0.5"
 black = "^23.3.0"
 click = "^8.1.4"
 executing = "^1.2.0"
 python = "^3.7"
```

### Comparing `inline_snapshot-0.3.1/PKG-INFO` & `inline_snapshot-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inline-snapshot
-Version: 0.3.1
+Version: 0.3.2
 Summary: golden master/snapshot/approval testing library which puts the values right into your source code
 Home-page: https://github.com/15r10nk/inline-snapshots
 License: MIT
 Author: Frank Hoffmann
 Author-email: 15r10nk@polarbit.de
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -29,14 +29,15 @@
 Project-URL: Repository, https://github.com/15r10nk/inline-snapshots
 Description-Content-Type: text/markdown
 
 # inline-snapshot
 
 [![Docs](https://img.shields.io/badge/docs-mkdocs-green)](https://15r10nk.github.io/inline-snapshot/)
 [![pypi version](https://img.shields.io/pypi/v/inline-snapshot.svg)](https://pypi.org/project/inline-snapshot/)
+![Python Versions](https://img.shields.io/pypi/pyversions/inline-snapshot)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/inline-snapshot)
 [![coverage](https://img.shields.io/badge/coverage-100%25-blue)](https://15r10nk.github.io/inline-snapshot/contributing/#coverage)
 [![GitHub Sponsors](https://img.shields.io/github/sponsors/15r10nk)](https://github.com/sponsors/15r10nk)
 
 > *create and update inline snapshots in your code.*
 
 ## Installation
```

