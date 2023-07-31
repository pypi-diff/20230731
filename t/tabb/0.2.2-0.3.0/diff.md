# Comparing `tmp/tabb-0.2.2.tar.gz` & `tmp/tabb-0.3.0.tar.gz`

## Comparing `tabb-0.2.2.tar` & `tabb-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.2/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.2.2/config.json
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.2.2/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.2.2/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.2.2/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.2/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/__about__.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/__init__.py
--rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/config.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/context.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/decorators.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/formatter.py
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/missing.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/nargs.py
--rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/py.typed
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/types.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/utils.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.2.2/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.2.2/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.2.2/README.md
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 tabb-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.0/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.3.0/config.json
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.3.0/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.3.0/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.3.0/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.0/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/config.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/context.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/missing.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/types.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.3.0/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.3.0/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.3.0/PKG-INFO
```

### Comparing `tabb-0.2.2/.DS_Store` & `tabb-0.3.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/test.py` & `tabb-0.3.0/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/.DS_Store` & `tabb-0.3.0/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/__init__.py` & `tabb-0.3.0/src/tabb/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,20 +6,34 @@
 from tabb.exceptions import (
     Abort,
     BadParameter,
     Exit,
     Help,
     MissingParameter,
     TabbError,
-    UnexpetedParameter,
+    UnexpectedParameter,
     UsageError,
 )
 from tabb.group import Group
 from tabb.missing import MISSING, is_missing
 from tabb.nargs import NArgs, NArgsLiteral
+from tabb.parameter import (
+    Bool,
+    Counter,
+    Dict,
+    File,
+    Flag,
+    Float,
+    Int,
+    List,
+    Optional,
+    Path,
+    String,
+    Tuple,
+)
 from tabb.types import (
     Argument,
     Choices,
     Depends,
     Greedy,
     Length,
     Matches,
@@ -30,33 +44,45 @@
 )
 
 __all__ = [
     "__version__",
     "Abort",
     "Argument",
     "BadParameter",
+    "Bool",
     "Choices",
     "command",
     "Command",
     "Config",
     "Context",
+    "Counter",
     "Depends",
+    "Dict",
     "Exit",
+    "File",
+    "Flag",
+    "Float",
     "Greedy",
     "group",
     "Group",
     "Help",
+    "Int",
     "is_missing",
     "Length",
+    "List",
     "Matches",
     "MISSING",
     "MissingParameter",
     "NArgs",
     "NArgsLiteral",
     "Option",
+    "Optional",
+    "Path",
     "Range",
     "Secret",
+    "String",
     "TabbError",
-    "UnexpetedParameter",
+    "Tuple",
+    "UnexpectedParameter",
     "UsageError",
     "Validate",
 ]
```

### Comparing `tabb-0.2.2/src/tabb/base.py` & `tabb-0.3.0/src/tabb/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     TypeVar,
 )
 
 from tabb.callback import Callback, create_callback
 from tabb.context import Context
 from tabb.exceptions import (
     Abort,
-    TabbError,
     Exit,
     Help,
+    TabbError,
 )
 from tabb.formatter import HelpFormatter, make_default_short_help
 from tabb.parameter import OptionParameter, ParameterGroup
 from tabb.parameter.types import HelpFlag
 from tabb.parser import parse_args
 from tabb.utils import detect_program_name, pacify_flush
 
@@ -288,15 +288,17 @@
             prog_name,
             args,
             environ,
             config,
             auto_config_prefix=auto_config_prefix,
             auto_envvar_prefix=auto_envvar_prefix,
         )
-        return self.invoke(ctx)
+
+        with ctx:
+            return self.invoke(ctx)
 
     def main(
         self,
         args: list[str] | None = None,
         *,
         prog_name: str | None = None,
         environ: Mapping[str, str] | None = None,
```

### Comparing `tabb-0.2.2/src/tabb/callback.py` & `tabb-0.3.0/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/command.py` & `tabb-0.3.0/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/config.py` & `tabb-0.3.0/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/decorators.py` & `tabb-0.3.0/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/exceptions.py` & `tabb-0.3.0/src/tabb/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
         if self.param:
             return f"Missing {self.param_type}: {self.param.name}"
 
         return f"Missing {self.param_type}."
 
 
-class UnexpetedParameter(UsageError):  # noqa: N818
+class UnexpectedParameter(UsageError):  # noqa: N818
     def __init__(
         self,
         arg: str,
         message: str | None = None,
         possibilities: Sequence[str] | None = None,
         ctx: Context[Any] | None = None,
     ) -> None:
```

### Comparing `tabb-0.2.2/src/tabb/formatter.py` & `tabb-0.3.0/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/group.py` & `tabb-0.3.0/src/tabb/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,9 +245,12 @@
                 msg += f" Did you mean {possibilities[0]!r}?"
             elif possibilities:
                 options = ", ".join(sorted(possibilities))
                 msg += f" (Possible options: {options})"
 
             ctx.fail(msg)
 
+
         sub_ctx = command.make_context(command_name, args, ctx.environ, ctx.config, ctx)
-        return command.invoke(sub_ctx)
+
+        with sub_ctx:
+            return command.invoke(sub_ctx)
```

### Comparing `tabb-0.2.2/src/tabb/nargs.py` & `tabb-0.3.0/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parser.py` & `tabb-0.3.0/src/tabb/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import functools
 import itertools
 from collections.abc import Iterator, Sequence
 from difflib import get_close_matches
 from typing import Any, Generic, Literal, NoReturn, TypeVar
 
 from tabb.context import Context
-from tabb.exceptions import UnexpetedParameter
+from tabb.exceptions import UnexpectedParameter
 from tabb.nargs import IntNArgs, NArgs, VariadicNArgs
 from tabb.parameter import (
     ArgumentParameter,
     DependsParameter,
     OptionParameter,
     ParameterValue,
     ParserParameter,
@@ -271,15 +271,15 @@
             value = param.process_args(ctx, captured_args.get(param, []))
             values.append(value)
 
         if (state.args or state.unused_args) and raise_on_unexpected:
             if not state.args:
                 state.reset_unused_args()
             possibilities = self._get_possible_matches(ctx, state)
-            raise UnexpetedParameter(state.args.peek(), possibilities=possibilities)
+            raise UnexpectedParameter(state.args.peek(), possibilities=possibilities)
 
         state.reset_unused_args()
         return values, list(state.args)
 
     def _get_possible_matches(self, ctx: Context[Any], state: State) -> list[str]:
         flag, _, _ = state.args.peek().partition("=")
         if is_short_flag(flag):
@@ -315,15 +315,15 @@
                 )
 
             except MatchError:
                 if state.loss() < best_match.loss():
                     best_match = state
                 continue
 
-            except UnexpetedParameter as error:
+            except UnexpectedParameter as error:
                 state.push_arg(error.arg)
 
             return state
 
         return best_match
 
     def _parse_thread(
@@ -526,15 +526,15 @@
     ) -> None:
         for index, short_name in enumerate(reversed(flag[1:])):
             short_flag = f"-{short_name}"
 
             try:
                 param = self.short_flags[short_flag]
             except KeyError:
-                raise UnexpetedParameter(arg) from None
+                raise UnexpectedParameter(arg) from None
 
             self._push_frame(
                 ctx=ctx,
                 threads=threads,
                 state=state,
                 param=param,
                 nargs=param.nargs,
@@ -551,15 +551,15 @@
         arg: str,
         flag: str,
         value: str | None,
     ) -> None:
         try:
             param = self.long_flags[flag]
         except KeyError:
-            raise UnexpetedParameter(arg) from None
+            raise UnexpectedParameter(arg) from None
 
         self._push_frame(
             ctx=ctx,
             threads=threads,
             state=state,
             param=param,
             nargs=param.nargs,
```

### Comparing `tabb-0.2.2/src/tabb/types.py` & `tabb-0.3.0/src/tabb/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
     def __repr__(self) -> str:
         return f'{type(self).__name__}("**********")'
 
 
 @dataclasses.dataclass()
 class Length:
-    min: int | None = None  # noqa: A003
-    max: int | None = None  # noqa: A003
+    min: int | None = None
+    max: int | None = None
 
 
 @dataclasses.dataclass()
 class Range:
-    min: int | float | None = None  # noqa: A003
-    max: int | float | None = None  # noqa: A003
+    min: int | float | None = None
+    max: int | float | None = None
     max_open: bool = False
     min_open: bool = False
     clamp: bool = False
 
 
 @dataclasses.dataclass()
 class Choices(Generic[ValueType]):
```

### Comparing `tabb-0.2.2/src/tabb/utils.py` & `tabb-0.3.0/src/tabb/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from __future__ import annotations
 
 import os
 import sys
+from collections.abc import Callable
+from functools import update_wrapper
 from shlex import shlex
 from types import ModuleType
-from typing import Any, TextIO, cast
+from typing import Any, ParamSpec, TextIO, TypeVar, cast
+
+P = ParamSpec("P")
+R = TypeVar("R")
+D = TypeVar("D")
 
 
 def to_kebab(name: str) -> str:
     return name.translate(str.maketrans("_ ", "--"))
 
 
 def to_snake(name: str) -> str:
@@ -84,7 +90,23 @@
 
 
 def pacify_flush(file: TextIO) -> TextIO:
     """Return a wrapper around the given file that will suppress BrokenPipeErrors
     resulting from ``.flush()`` being called on a broken pipe.
     """
     return cast(TextIO, PacifyFlushWrapper(file))
+
+
+def safecall(
+    fn: Callable[P, R],
+    default: D = None,
+    exceptions: tuple[type[BaseException], ...] = (Exception,),
+) -> Callable[P, R | D]:
+    "Wraps a function so that it swallows exceptions."
+
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> R | D:
+        try:
+            return fn(*args, **kwargs)
+        except exceptions:
+            return default
+
+    return update_wrapper(wrapper, fn)
```

### Comparing `tabb-0.2.2/src/tabb/parameter/base.py` & `tabb-0.3.0/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parameter/depends.py` & `tabb-0.3.0/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parameter/group.py` & `tabb-0.3.0/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parameter/parser.py` & `tabb-0.3.0/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parameter/resolve.py` & `tabb-0.3.0/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/src/tabb/parameter/types.py` & `tabb-0.3.0/src/tabb/parameter/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import abc
 import dataclasses
 import operator
 import os
 import pathlib
+import sys
 import typing
 from collections.abc import Callable, Hashable, Mapping, Sequence, Sized
+from os import PathLike
 from types import UnionType
 from typing import (
+    IO,
     TYPE_CHECKING,
     Any,
     Generic,
     NoReturn,
     TypeAlias,
     TypeGuard,
     TypeVar,
@@ -20,15 +23,15 @@
     cast,
     overload,
 )
 
 from tabb.exceptions import BadParameter, Help
 from tabb.missing import _MISSING_TYPE, MISSING
 from tabb.nargs import IntNArgs, NArgs, NArgsLiteral, VariadicNArgs
-from tabb.utils import split_csv
+from tabb.utils import safecall, split_csv
 
 if TYPE_CHECKING:
     from tabb.context import Context
     from tabb.parameter import ParserParameter
 
 KeyType = TypeVar("KeyType", bound=Hashable)
 SizedValueType = TypeVar("SizedValueType", bound=Sized)
@@ -712,20 +715,29 @@
         return result
 
     def process_config(self, value: object) -> object:
         if not isinstance(value, str):
             return value
         return self.parse(value)
 
+    def _validate_dash(self) -> bool:
+        if not self.allow_dash:
+            self.fail("'-' is not allowed.")
+
+        if self.executable:
+            self.fail("Path must be executable.")
+
+        return True
+
     def validate(self, value: Any) -> TypeGuard[pathlib.Path]:
         if not isinstance(value, pathlib.Path):
             self.fail("Expected path value.")
 
-        if not self.allow_dash and value == pathlib.Path("-"):
-            self.fail("'-' is not allowed.")
+        if value == pathlib.Path("-"):
+            return self._validate_dash()
 
         if self.exists and not value.exists():
             self.fail("Path must exist.")
 
         if not self.file_okay and value.is_file():
             self.fail("Path must not be a file.")
 
@@ -740,14 +752,98 @@
 
         if self.executable and not os.access(value, os.X_OK):
             self.fail("Path must be executable.")
 
         return True
 
 
+class File(ParameterType[IO[Any]]):
+    def __init__(
+        self,
+        mode: str = "r",
+        encoding: str = "utf-8",
+        errors: str = "strict",
+        default: int | str | bytes | PathLike[str] | PathLike[bytes] | None = None,
+        allow_overwrite: bool = True,
+        close: bool | None = None,
+    ) -> None:
+        super().__init__()
+        self.mode = mode
+        self.encoding = encoding
+        self.errors = errors
+        self.default = default
+        self.allow_overwrite = allow_overwrite
+        self.close = close
+
+    @property
+    def name(self) -> str:
+        return f"File[{self.mode!r}]"
+
+    def format_value(self, value: IO[Any]) -> str:
+        if hasattr(value, "name"):
+            if value.name in ("<stdin>", "<stdout>"):
+                return "-"
+
+            return value.name
+
+        return repr(value)
+
+    def has_default(self) -> bool:
+        return self.default is not None
+
+    def matches(self, arg: ParameterArg) -> bool:
+        return arg.value is not None
+
+    def open(self, value: str) -> IO[Any]:
+        if os.fsdecode(value) == "-":
+            if any(m in self.mode for m in ["w", "a", "x"]):
+                if "b" in self.mode:
+                    return sys.stdout.buffer
+                return sys.stdout
+
+            if "b" in self.mode:
+                return sys.stdin.buffer
+            return sys.stdin
+
+        result = open(value, self.mode, encoding=self.encoding, errors=self.errors)
+
+        from tabb.context import get_current_context
+
+        ctx = get_current_context(silent=True)
+
+        if ctx is not None:
+            ctx.call_on_close(safecall(result.close))
+
+        return result
+
+    def process_args(self, args: list[ParameterArg]) -> IO[Any] | _MISSING_TYPE:
+        if not args:
+            if not self.default:
+                return MISSING
+            return self.open(self.default)
+
+        if len(args) != 1 and not self.allow_overwrite:
+            self.fail("Parameter already set.")
+
+        return self.open(args[-1])
+
+    def process_config(self, value: object) -> IO[Any]:
+        if not isinstance(value, str):
+            self.fail("Config value must be a string.")
+        return self.open(value)
+
+    def parse_envvar(self, value: str) -> IO[Any]:
+        return self.open(value)
+
+    def validate(self, value: Any) -> TypeGuard[IO[Any]]:
+        if not (hasattr(value, "read") or hasattr(value, "write")):
+            self.fail("Expected file-like object.")
+        return True
+
+
 class Validator(TypeAdapter[ValueType]):
     def __init__(
         self,
         type: ParameterType[ValueType],
         validator: Callable[[ValueType], bool],
     ) -> None:
         self.validator = validator
@@ -965,11 +1061,10 @@
         raise Help()
 
     def validate(self, value: Any) -> TypeGuard[NoReturn]:
         raise Help()
 
 
 # TODO: add types:
-# - file
 # - url
 # - uuid
 # - enum
```

### Comparing `tabb-0.2.2/src/tabb/parameter/utils.py` & `tabb-0.3.0/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/.gitignore` & `tabb-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/LICENSE.txt` & `tabb-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/README.md` & `tabb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.2.2/pyproject.toml` & `tabb-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
   "TID",
   "UP",
   "W",
   "YTT",
 ]
 ignore = [
   # Allow shadowing builtins
-  "A002",
+  "A002", "A003",
   # Allow unused arguments
   "ARG002",
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow using literal strings in exceptions
   "EM101",
   # Ignore checks for possible passwords
```

### Comparing `tabb-0.2.2/PKG-INFO` & `tabb-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.2.2
+Version: 0.3.0
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

