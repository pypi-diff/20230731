# Comparing `tmp/types-pyflakes-3.0.0.5.tar.gz` & `tmp/types-pyflakes-3.1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyflakes-3.0.0.5.tar", last modified: Thu Jul 20 15:20:35 2023, max compression
+gzip compressed data, was "types-pyflakes-3.1.0.0.tar", last modified: Mon Jul 31 01:15:53 2023, max compression
```

## Comparing `types-pyflakes-3.0.0.5.tar` & `types-pyflakes-3.1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/pyflakes-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/reporter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:15:53.680527 types-pyflakes-3.1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-07-31 01:15:47.000000 types-pyflakes-3.1.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-31 01:15:47.000000 types-pyflakes-3.1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 01:15:53.680527 types-pyflakes-3.1.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:15:53.680527 types-pyflakes-3.1.0.0/pyflakes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-31 01:15:47.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 01:15:31.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-31 01:15:31.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-07-31 01:15:31.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-31 01:15:31.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-31 01:15:31.000000 types-pyflakes-3.1.0.0/pyflakes-stubs/reporter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 01:15:53.680527 types-pyflakes-3.1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-31 01:15:47.000000 types-pyflakes-3.1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 01:15:53.680527 types-pyflakes-3.1.0.0/types_pyflakes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-31 01:15:53.000000 types-pyflakes-3.1.0.0/types_pyflakes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-31 01:15:53.000000 types-pyflakes-3.1.0.0/types_pyflakes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 01:15:53.000000 types-pyflakes-3.1.0.0/types_pyflakes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 01:15:53.000000 types-pyflakes-3.1.0.0/types_pyflakes.egg-info/top_level.txt
```

### Comparing `types-pyflakes-3.0.0.5/CHANGELOG.md` & `types-pyflakes-3.1.0.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.0 (2023-07-31)
+
+Update pyflakes stubs for v3.1.* (#10518)
+
 ## 3.0.0.5 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 3.0.0.4 (2023-05-10)
```

### Comparing `types-pyflakes-3.0.0.5/PKG-INFO` & `types-pyflakes-3.1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.0.0.5
+Version: 3.1.0.0
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `a079b0de6e703fcb615a1169a32bc2186efee9bd` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

### Comparing `types-pyflakes-3.0.0.5/pyflakes-stubs/api.pyi` & `types-pyflakes-3.1.0.0/pyflakes-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.5/pyflakes-stubs/checker.pyi` & `types-pyflakes-3.1.0.0/pyflakes-stubs/checker.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import ast
 import sys
 from collections.abc import Callable, Iterable, Iterator
+from contextlib import contextmanager
 from re import Pattern
 from typing import Any, ClassVar, TypeVar, overload
 from typing_extensions import Literal, ParamSpec, TypeAlias
 
 from pyflakes.messages import Message
 
 _AnyFunction: TypeAlias = Callable[..., Any]
 _F = TypeVar("_F", bound=_AnyFunction)
 _P = ParamSpec("_P")
 _T = TypeVar("_T")
 
-PY38_PLUS: bool
 PYPY: bool
 
 def getAlternatives(n: ast.If | ast.Try) -> list[ast.AST]: ...
 
 FOR_TYPES: tuple[type[ast.For], type[ast.AsyncFor]]
 MAPPING_KEY_RE: Pattern[str]
 CONVERSION_FLAG_RE: Pattern[str]
@@ -116,14 +116,15 @@
     globals: set[str]
     returnValue: Any
     isGenerator: bool
     def __init__(self) -> None: ...
     def unused_assignments(self) -> Iterator[tuple[str, Binding]]: ...
     def unused_annotations(self) -> Iterator[tuple[str, Annotation]]: ...
 
+class TypeScope(Scope): ...
 class GeneratorScope(Scope): ...
 class ModuleScope(Scope): ...
 class DoctestScope(ModuleScope): ...
 
 class DetectClassScopedMagic:
     names: list[str]
 
@@ -165,14 +166,21 @@
     _MatchSequence: TypeAlias = Any
     _MatchStar: TypeAlias = Any
     _MatchMapping: TypeAlias = Any
     _MatchClass: TypeAlias = Any
     _MatchAs: TypeAlias = Any
     _MatchOr: TypeAlias = Any
 
+if sys.version_info >= (3, 12):
+    _TypeVar: TypeAlias = ast.TypeVar
+    _TypeAlias: TypeAlias = ast.TypeAlias
+else:
+    _TypeVar: TypeAlias = Any
+    _TypeAlias: TypeAlias = Any
+
 class Checker:
     nodeDepth: int
     offset: tuple[int, int] | None
     builtIns: set[str]
     deadScopes: list[Any]
     messages: list[Any]
     filename: str
@@ -185,29 +193,27 @@
         tree: ast.AST,
         filename: str = "(none)",
         builtins: Iterable[str] | None = None,
         withDoctest: bool = False,
         file_tokens: tuple[Any, ...] = (),
     ) -> None: ...
     def deferFunction(self, callable: _AnyFunction) -> None: ...
-    def deferAssignment(self, callable: _AnyFunction) -> None: ...
-    def runDeferred(self, deferred: _AnyFunction) -> None: ...
     @property
     def futuresAllowed(self) -> bool: ...
     @futuresAllowed.setter
     def futuresAllowed(self, value: Literal[False]) -> None: ...
     @property
     def annotationsFutureEnabled(self) -> bool: ...
     @annotationsFutureEnabled.setter
     def annotationsFutureEnabled(self, value: Literal[True]) -> None: ...
     @property
     def scope(self) -> Scope: ...
-    def popScope(self) -> None: ...
+    @contextmanager
+    def in_scope(self, cls: Callable[[], Scope]) -> Iterator[None]: ...
     def checkDeadScopes(self) -> None: ...
-    def pushScope(self, scopeClass: type[Scope] = ...) -> None: ...
     def report(self, messageClass: Callable[_P, Message], *args: _P.args, **kwargs: _P.kwargs) -> None: ...
     def getParent(self, node: ast.AST) -> ast.AST: ...
     def getCommonAncestor(self, lnode: ast.AST, rnode: ast.AST, stop: ast.AST) -> ast.AST: ...
     def descendantOf(self, node: ast.AST, ancestors: ast.AST, stop: ast.AST) -> bool: ...
     def getScopeNode(self, node: ast.AST) -> ast.AST | None: ...
     def differentForks(self, lnode: ast.AST, rnode: ast.AST) -> bool: ...
     def addBinding(self, node: ast.AST, value: Binding) -> None: ...
@@ -218,14 +224,15 @@
     def handleChildren(self, tree: ast.AST, omit: _OmitType = None) -> None: ...
     def isLiteralTupleUnpacking(self, node: ast.AST) -> bool | None: ...
     def isDocstring(self, node: ast.AST) -> bool: ...
     def getDocstring(self, node: ast.AST) -> tuple[str, int] | tuple[None, None]: ...
     def handleNode(self, node: ast.AST | None, parent) -> None: ...
     def handleDoctests(self, node: ast.AST) -> None: ...
     def handleStringAnnotation(self, s: str, node: ast.AST, ref_lineno: int, ref_col_offset: int, err: type[Message]) -> None: ...
+    def handle_annotation_always_deferred(self, annotation: ast.AST, parent: ast.AST) -> None: ...
     def handleAnnotation(self, annotation: ast.AST, node: ast.AST) -> None: ...
     def ignore(self, node: ast.AST) -> None: ...
     def DELETE(self, tree: ast.Delete, omit: _OmitType = None) -> None: ...
     def FOR(self, tree: ast.For, omit: _OmitType = None) -> None: ...
     def ASYNCFOR(self, tree: ast.AsyncFor, omit: _OmitType = None) -> None: ...
     def WHILE(self, tree: ast.While, omit: _OmitType = None) -> None: ...
     def WITH(self, tree: ast.With, omit: _OmitType = None) -> None: ...
@@ -241,20 +248,14 @@
     def STARRED(self, tree: ast.Starred, omit: _OmitType = None) -> None: ...
     def NAMECONSTANT(self, tree: ast.NameConstant, omit: _OmitType = None) -> None: ...
     def NAMEDEXPR(self, tree: _NamedExpr, omit: _OmitType = None) -> None: ...
     def SUBSCRIPT(self, node: ast.Subscript) -> None: ...
     def CALL(self, node: ast.Call) -> None: ...
     def BINOP(self, node: ast.BinOp) -> None: ...
     def CONSTANT(self, node: ast.Constant) -> None: ...
-    if sys.version_info < (3, 8):
-        def NUM(self, node: ast.Num) -> None: ...
-        def BYTES(self, node: ast.Bytes) -> None: ...
-        def ELLIPSIS(self, node: ast.Ellipsis) -> None: ...
-
-    def STR(self, node: ast.Str) -> None: ...
     def SLICE(self, tree: ast.Slice, omit: _OmitType = None) -> None: ...
     def EXTSLICE(self, tree: ast.ExtSlice, omit: _OmitType = None) -> None: ...
     def INDEX(self, tree: ast.Index, omit: _OmitType = None) -> None: ...
     def LOAD(self, node: ast.Load) -> None: ...
     def STORE(self, node: ast.Store) -> None: ...
     def DEL(self, node: ast.Del) -> None: ...
     def AUGLOAD(self, node: ast.AugLoad) -> None: ...
@@ -332,7 +333,9 @@
     def MATCHOR(self, tree: _MatchOr, omit: _OmitType = None) -> None: ...
     def MATCHSEQUENCE(self, tree: _MatchSequence, omit: _OmitType = None) -> None: ...
     def MATCHSINGLETON(self, tree: _MatchSingleton, omit: _OmitType = None) -> None: ...
     def MATCHVALUE(self, tree: _MatchValue, omit: _OmitType = None) -> None: ...
     def MATCHAS(self, node: _MatchAs) -> None: ...
     def MATCHMAPPING(self, node: _MatchMapping) -> None: ...
     def MATCHSTAR(self, node: _MatchStar) -> None: ...
+    def TYPEVAR(self, node: _TypeVar) -> None: ...
+    def TYPEALIAS(self, node: _TypeAlias) -> None: ...
```

### Comparing `types-pyflakes-3.0.0.5/pyflakes-stubs/messages.pyi` & `types-pyflakes-3.1.0.0/pyflakes-stubs/messages.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     message_args: tuple[Any]
     def __init__(self, filename, loc: ast.AST, names) -> None: ...
 
 class ReturnOutsideFunction(Message): ...
 class YieldOutsideFunction(Message): ...
 class ContinueOutsideLoop(Message): ...
 class BreakOutsideLoop(Message): ...
-class ContinueInFinally(Message): ...
 class DefaultExceptNotLast(Message): ...
 class TwoStarredExpressions(Message): ...
 class TooManyExpressionsInStarredAssignment(Message): ...
 class IfTuple(Message): ...
 class AssertTuple(Message): ...
 
 class ForwardAnnotationSyntaxError(Message):
```

### Comparing `types-pyflakes-3.0.0.5/setup.py` & `types-pyflakes-3.1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `a079b0de6e703fcb615a1169a32bc2186efee9bd` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.5",
+      version="3.1.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md",
```

### Comparing `types-pyflakes-3.0.0.5/types_pyflakes.egg-info/PKG-INFO` & `types-pyflakes-3.1.0.0/types_pyflakes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.0.0.5
+Version: 3.1.0.0
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `a079b0de6e703fcb615a1169a32bc2186efee9bd` and was tested
+with mypy 1.4.1, pyright 1.1.319, and
+pytype 2023.7.21.
```

