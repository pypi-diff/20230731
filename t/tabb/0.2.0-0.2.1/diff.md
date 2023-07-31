# Comparing `tmp/tabb-0.2.0.tar.gz` & `tmp/tabb-0.2.1.tar.gz`

## Comparing `tabb-0.2.0.tar` & `tabb-0.2.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.0/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.2.0/config.json
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.2.0/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.2.0/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.2.0/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.0/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/__init__.py
--rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/config.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/context.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/decorators.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/formatter.py
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/missing.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/nargs.py
--rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/py.typed
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/types.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/utils.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.2.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.2.0/README.md
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 tabb-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.1/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.2.1/config.json
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.2.1/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.2.1/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.2.1/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.1/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/config.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/context.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/missing.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/py.typed
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/types.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/utils.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.2.1/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.2.1/README.md
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 tabb-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.2.1/PKG-INFO
```

### Comparing `tabb-0.2.0/.DS_Store` & `tabb-0.2.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/test.py` & `tabb-0.2.1/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/.DS_Store` & `tabb-0.2.1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/base.py` & `tabb-0.2.1/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/callback.py` & `tabb-0.2.1/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/command.py` & `tabb-0.2.1/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/config.py` & `tabb-0.2.1/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/context.py` & `tabb-0.2.1/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/decorators.py` & `tabb-0.2.1/src/tabb/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
-from collections.abc import Callable
+from collections.abc import Callable, Mapping, Sequence
 from typing import Any, ParamSpec, TypeVar, overload
 
+from tabb.base import BaseCommand
 from tabb.command import Command
 from tabb.group import Group
 
 T = TypeVar("T")
 P = ParamSpec("P")
 
 
@@ -52,14 +53,15 @@
 def group(callback: Callable[..., Any], /) -> Group[Any]:
     ...
 
 
 @overload
 def group(
     name: str | None = None,
+    commands: Mapping[str, BaseCommand[T]] | Sequence[BaseCommand[T]] | None = None,
     *,
     add_help_option: bool = True,
     deprecated: bool = False,
     epilog: str | None = None,
     help: str | None = None,
     hidden: bool = False,
     import_dependencies: str | None = None,
```

### Comparing `tabb-0.2.0/src/tabb/exceptions.py` & `tabb-0.2.1/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/formatter.py` & `tabb-0.2.1/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/group.py` & `tabb-0.2.1/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/nargs.py` & `tabb-0.2.1/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parser.py` & `tabb-0.2.1/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/types.py` & `tabb-0.2.1/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/utils.py` & `tabb-0.2.1/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/base.py` & `tabb-0.2.1/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/depends.py` & `tabb-0.2.1/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/group.py` & `tabb-0.2.1/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/parser.py` & `tabb-0.2.1/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/resolve.py` & `tabb-0.2.1/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/types.py` & `tabb-0.2.1/src/tabb/parameter/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/src/tabb/parameter/utils.py` & `tabb-0.2.1/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/.gitignore` & `tabb-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/LICENSE.txt` & `tabb-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/README.md` & `tabb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/pyproject.toml` & `tabb-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.2.0/PKG-INFO` & `tabb-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

