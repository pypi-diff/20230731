# Comparing `tmp/py_buzz-3.3.0.tar.gz` & `tmp/py_buzz-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_buzz-3.3.0.tar", max compression
+gzip compressed data, was "py_buzz-4.0.0.tar", max compression
```

## Comparing `py_buzz-3.3.0.tar` & `py_buzz-4.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1099 2022-03-30 16:27:40.385941 py_buzz-3.3.0/LICENSE.rst
--rw-r--r--   0        0        0     1996 2022-06-20 21:10:42.949372 py_buzz-3.3.0/README.rst
--rw-r--r--   0        0        0      394 2022-06-20 21:10:42.949372 py_buzz-3.3.0/buzz/__init__.py
--rw-r--r--   0        0        0     2535 2022-06-20 23:09:43.479472 py_buzz-3.3.0/buzz/base.py
--rw-r--r--   0        0        0        0 2022-03-30 16:27:40.385941 py_buzz-3.3.0/buzz/py.typed
--rw-r--r--   0        0        0    10824 2023-07-27 16:37:46.987907 py_buzz-3.3.0/buzz/tools.py
--rw-r--r--   0        0        0     1089 2023-07-27 16:37:46.997907 py_buzz-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 py_buzz-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-31 20:25:12.235905 py_buzz-4.0.0/LICENSE.md
+-rw-r--r--   0        0        0     1600 2023-07-31 20:25:12.235905 py_buzz-4.0.0/README.md
+-rw-r--r--   0        0        0      394 2023-07-31 20:25:12.235905 py_buzz-4.0.0/buzz/__init__.py
+-rw-r--r--   0        0        0     2616 2023-07-31 20:25:12.235905 py_buzz-4.0.0/buzz/base.py
+-rw-r--r--   0        0        0        0 2023-07-31 20:25:12.235905 py_buzz-4.0.0/buzz/py.typed
+-rw-r--r--   0        0        0    10664 2023-07-31 20:25:12.235905 py_buzz-4.0.0/buzz/tools.py
+-rw-r--r--   0        0        0     1351 2023-07-31 20:25:12.235905 py_buzz-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 py_buzz-4.0.0/PKG-INFO
```

### Comparing `py_buzz-3.3.0/LICENSE.rst` & `py_buzz-4.0.0/LICENSE.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-MIT License
-===========
+# MIT License
 
-Copyright (c) ``2016`` - ``2022`` ``Tucker Beck``
+Copyright (c) `2016` - `2022` `Tucker Beck`
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `py_buzz-3.3.0/README.rst` & `py_buzz-4.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,37 @@
-.. image::  https://badge.fury.io/py/py-buzz.svg
-   :target: https://badge.fury.io/py/py-buzz
-   :alt:    Latest Version
-
-.. image::  https://travis-ci.org/dusktreader/py-buzz.svg?branch=integration
-   :target: https://travis-ci.org/dusktreader/py-buzz
-   :alt:    Build Status
-
-.. image::  https://readthedocs.org/projects/py-buzz/badge/?version=latest
-   :target: http://py-buzz.readthedocs.io/en/latest/?badge=latest
-   :alt:    Documentation Status
-
-*********
- py-buzz
-*********
-
-------------------------------------------------------------------
-That's not flying, it's falling with style: Exceptions with extras
-------------------------------------------------------------------
+![Latest Version](https://badge.fury.io/py/py-buzz.svg)
+![Build Status](https://github.com/dusktreader/py-buzz/actions/workflows/main.yml/badge.svg)
+![Documentation Status](https://readthedocs.org/projects/py-buzz/badge/?version=latest)
+
+# py-buzz
+
+**_That's not flying, it's falling with style_: Exceptions with extras**
 
 py-buzz supplies some useful tools to use with python exceptions as well
 as a base Buzz exception class that includes them as classmethods.
 
 py-buzz is fully equipped with exception tools that are written over and over
 again in python projects such as:
 
-* checking conditions and raising errors on failure (``require_conditon``)
-* checking that values are defined and raising errors if not (``enforce_defined``)
+* checking conditions and raising errors on failure (`require_conditon`)
+* checking that values are defined and raising errors if not (`enforce_defined`)
 * catching exceptions wrapping them in clearer exception types with better error
-  messages (``handle_errors``)
+  messages (`handle_errors`)
 * checking many conditions and reporting which ones failed
-  (``check_expressions``)
+  (`check_expressions`)
 
 Buzz can be used as a stand-alone exception class, but it is best used as a
 bass class for custom exceptions within a project. This allows the user to
 focus on creating a set of Exceptions that provide complete coverage for issues
 within their application without having to re-write convenience functions
 themselves.
 
-Super-quick Start
------------------
- - requirements: `python3.6+`
- - install through pip: `$ pip install py-buzz`
- - minimal usage example: `examples/with_buzz_class.py <https://github.com/dusktreader/py-buzz/tree/master/examples/with_buzz_class.py>`_
+## Super-quick Start
+
+* requirements: `python3.6+`
+* install through pip: `$ pip install py-buzz`
+* minimal usage example: [examples/with_buzz_class.py](https://github.com/dusktreader/py-buzz/tree/main/examples/with_buzz_class.py)
 
-Documentation
--------------
+## Documentation
 
 The complete documentation can be found at the
-`py-buzz home page <http://py-buzz.readthedocs.io>`_
+[py-buzz documentation page](http://py-buzz.readthedocs.io)
```

### Comparing `py_buzz-3.3.0/buzz/base.py` & `py_buzz-4.0.0/buzz/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+"""
+This module defines the Buzz base class.
+"""
+
+from __future__ import annotations
+
 import textwrap
-from typing import Optional
 
 from buzz.tools import TNonNull, check_expressions, enforce_defined, get_traceback, handle_errors, require_condition
 
 
 class Buzz(Exception):
     """
     This provides a specialized exception class that wraps up all the buzz utility functions.
@@ -20,53 +25,56 @@
 
     def __repr__(self):
         return self.__class__.__name__
 
     @staticmethod
     def _check_kwargs(**kwargs):
         """
-        Ensure that ``raise_exc_class`` was not passed as a keyword-argument.
+        Ensure that `raise_exc_class()` was not passed as a keyword-argument.
         """
         if "raise_exc_class" in kwargs:
             raise ValueError("You may not pass the 'raise_exc_class' to Buzz-derived exception methods.")
 
     @classmethod
     def require_condition(cls, *args, **kwargs):
         """
-        Call the require_condition function with this class as the ``raise_exc_class`` kwarg.
+        Call the `require_condition()` function with this class as the `raise_exc_class` kwarg.
         """
         cls._check_kwargs(**kwargs)
         return require_condition(*args, raise_exc_class=cls, **kwargs)
 
     @classmethod
-    def enforce_defined(cls, value: Optional[TNonNull], *args, **kwargs) -> TNonNull:
+    def enforce_defined(cls, value: TNonNull | None, *args, **kwargs) -> TNonNull:
         """
-        Call the enforce_defined function with this class as the ``raise_exc_class`` kwarg.
+        Call the `enforce_defined()` function with this class as the `raise_exc_class` kwarg.
         """
         cls._check_kwargs(**kwargs)
         # This can't be passed as a kwarg, because: https://github.com/python/mypy/issues/6799
         kwargs["raise_exc_class"] = cls
         return enforce_defined(value, *args, **kwargs)
 
     @classmethod
     def check_expressions(cls, *args, **kwargs):
         """
-        Call the check_expressions context manager with this class as the ``raise_exc_class`` kwarg.
+        Call the `check_expressions()` context manager with this class as the `raise_exc_class` kwarg.
         """
         cls._check_kwargs(**kwargs)
         return check_expressions(*args, raise_exc_class=cls, **kwargs)
 
     @classmethod
     def handle_errors(cls, *args, re_raise=True, **kwargs):
         """
-        Call the handle_errors context manager with this class as the ``raise_exc_class`` kwarg.
-        If ``re_raise`` is not True, ``None`` will be passed as the ``raise_exc_class`` kwarg.
+        Call the `handle_errors()` context manager with this class as the `raise_exc_class` kwarg.
+
+        Note:
+
+            If `re_raise` is not True, `None` will be passed as the `raise_exc_class` kwarg.
         """
         cls._check_kwargs(**kwargs)
         return handle_errors(*args, raise_exc_class=cls if re_raise else None, **kwargs)
 
     @classmethod
     def get_traceback(cls, *args, **kwargs):
         """
-        Call the get_traceback function.
+        Call the `get_traceback()` function.
         """
         return get_traceback(*args, **kwargs)
```

### Comparing `py_buzz-3.3.0/buzz/tools.py` & `py_buzz-4.0.0/buzz/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,96 +1,95 @@
 """
 This module supplies the core functions of the py-buzz package.
+"""
 
-Includes:
+from __future__ import annotations
 
-* require_condition:  asserts a condition and raises an exception otherwise
-* handle_errors:      a context manager that handles exceptions
-* check_expressions:  a context manager that checks multiple expressions
-"""
 import contextlib
 import dataclasses
 import sys
 import types
-from typing import Any, Callable, Iterable, Iterator, Mapping, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, Iterable, Iterator, Mapping, Tuple, TypeVar
 
 
 def noop(*_, **__):
     pass
 
 
 TExc = TypeVar("TExc", bound=Exception)
 
 
-def default_exc_builder(exc: Type[TExc], message: str, *args, **kwargs) -> TExc:
+def default_exc_builder(exc: type[TExc], message: str, *args, **kwargs) -> TExc:
     """
     Build an exception instance using default behavior where message is passed as first positional argument.
 
     Some exception types such as FastAPI's HTTPException do not take a message as the first positional argument, so
     they will need a different exception builder.
     """
     return exc(message, *args, **kwargs)
 
 
 def require_condition(
     expr: Any,
     message: str,
-    raise_exc_class: Type[Exception] = Exception,
-    raise_args: Optional[Iterable[Any]] = None,
-    raise_kwargs: Optional[Mapping[str, Any]] = None,
+    raise_exc_class: type[Exception] = Exception,
+    raise_args: Iterable[Any] | None = None,
+    raise_kwargs: Mapping[str, Any] | None = None,
     exc_builder: Callable[..., Exception] = default_exc_builder,
 ):
     """
     Assert that an expression is truthy. If the assertion fails, raise an exception with the supplied message.
 
-    :param: message:          The failure message to attach to the raised Exception
-    :param: expr:             The value that is checked for truthiness (usually an evaluated expression)
-    :param: raise_exc_class:  The exception type to raise with the constructed message if the expression is falsey.
-
-                              Defaults to Exception.
-                              May not be None.
-
-    :param: raise_args:       Additional positional args (after the constructed message) that will passed when raising
-                              an instance of the ``raise_exc_class``.
-    :param: raise_kwargs:     Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
+    Args:
+
+        message:         The failure message to attach to the raised Exception
+        expr:            The value that is checked for truthiness (usually an evaluated expression)
+        raise_exc_class: The exception type to raise with the constructed message if the expression is falsey.
+                         Defaults to Exception.
+                         May not be None.
+        raise_args:      Additional positional args (after the constructed message) that will passed when raising
+                         an instance of the ``raise_exc_class``.
+        raise_kwargs:    Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
     """
     if raise_exc_class is None:
         raise ValueError("The raise_exc_class kwarg may not be None")
 
     if not expr:
         args = raise_args or []
         kwargs = raise_kwargs or {}
         raise exc_builder(raise_exc_class, message, *args, **kwargs)
 
 
 TNonNull = TypeVar("TNonNull")
 
 
 def enforce_defined(
-    value: Optional[TNonNull],
+    value: TNonNull | None,
     message: str = "Value was not defined (None)",
-    raise_exc_class: Type[Exception] = Exception,
-    raise_args: Optional[Iterable[Any]] = None,
-    raise_kwargs: Optional[Mapping[str, Any]] = None,
+    raise_exc_class: type[Exception] = Exception,
+    raise_args: Iterable[Any] | None = None,
+    raise_kwargs: Mapping[str, Any] | None = None,
     exc_builder: Callable[..., Exception] = default_exc_builder,
 ) -> TNonNull:
     """
     Assert that a value is not None. If the assertion fails, raise an exception with the supplied message.
 
-    :param: value:            The value that is checked to be non-null
-    :param: message:          The failure message to attach to the raised Exception
-    :param: expr:             The value that is checked for truthiness (usually an evaluated expression)
-    :param: raise_exc_class:  The exception type to raise with the constructed message if the expression is falsey.
-
-                              Defaults to Exception.
-                              May not be None.
-
-    :param: raise_args:       Additional positional args (after the constructed message) that will passed when raising
-                              an instance of the ``raise_exc_class``.
-    :param: raise_kwargs:     Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
+    Args:
+
+        value:            The value that is checked to be non-null
+        message:          The failure message to attach to the raised Exception
+        expr:             The value that is checked for truthiness (usually an evaluated expression)
+        raise_exc_class:  The exception type to raise with the constructed message if the expression is falsey.
+
+                          Defaults to Exception.
+                          May not be None.
+
+        raise_args:       Additional positional args (after the constructed message) that will passed when raising
+                          an instance of the ``raise_exc_class``.
+        raise_kwargs:     Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
     """
     if value is not None:
         return value
     else:
         args = raise_args or []
         kwargs = raise_kwargs or {}
         raise exc_builder(raise_exc_class, message, *args, **kwargs)
@@ -115,62 +114,61 @@
         else:
             return {
                 1: f"{n}st",
                 2: f"{n}nd",
                 3: f"{n}rd",
             }.get(n % 10, f"{n}th")
 
-    def check(self, evaluated_expression: Any, message: str = None):
+    def check(self, evaluated_expression: Any, message: str | None = None):
         self.expression_counter += 1
         if not evaluated_expression:
             if message is None:
                 message = "{nth} expression failed".format(nth=self.ordinalize(self.expression_counter))
             self.problems.append(f"{self.expression_counter}: {message}")
 
 
 @contextlib.contextmanager
 def check_expressions(
     main_message: str,
-    raise_exc_class: Type[Exception] = Exception,
-    raise_args: Optional[Iterable[Any]] = None,
-    raise_kwargs: Optional[Mapping[str, Any]] = None,
+    raise_exc_class: type[Exception] = Exception,
+    raise_args: Iterable[Any] | None = None,
+    raise_kwargs: Mapping[str, Any] | None = None,
     exc_builder: Callable[..., Exception] = default_exc_builder,
 ):
     """
     Check a series of expressions inside of a context manager. If any fail an exception is raised that contains a
     main message and a description of each failing expression.
 
-    :param: main message:      The main failure message to include in the constructed message that is passed to the
-                               raised Exception
-    :param: raise_exc_class:   The exception type to raise with the constructed message if the expression is falsey.
-
-                               Defaults to Exception.
-
-                               May not be None.
-    :param: raise_args:        Additional positional args (after the constructed message) that will passed when raising
-                               an instance of the ``raise_exc_class``.
-    :param: raise_kwargs:      Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
+    Args:
+        main message:      The main failure message to include in the constructed message that is passed to the
+                           raised Exception
+        raise_exc_class:   The exception type to raise with the constructed message if the expression is falsey.
+
+                           Defaults to Exception.
+
+                           May not be None.
+        raise_args:        Additional positional args (after the constructed message) that will passed when raising
+                           an instance of the ``raise_exc_class``.
+        raise_kwargs:      Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
 
     Example:
 
-    .. code-block:: python
-
-       with check_expressions("Something wasn't right") as check:
-           check(a is not None)
-           check(a > b, "a must be greater than b")
-           check(a != 1, "a must not equal 1")
-           check(b >= 0, "b must not be negative")
-
-    This would render output like:
+        The following is an example usage::
 
-    .. code-block:: bash
-
-       Checked expressions failed: Something wasn't right:
-         1: first expressoin failed
-         3: a must not equal 1
+            with check_expressions("Something wasn't right") as check:
+                check(a is not None)
+                check(a > b, "a must be greater than b")
+                check(a != 1, "a must not equal 1")
+                check(b >= 0, "b must not be negative")
+
+        This would render output like::
+
+            Checked expressions failed: Something wasn't right:
+              1: first expressoin failed
+              3: a must not equal 1
     """
     if raise_exc_class is None:
         raise ValueError("The raise_exc_class kwarg may not be None")
 
     checker = _ExpressionChecker()
     yield checker.check
     message = "\n  ".join(
@@ -193,75 +191,82 @@
 def reformat_exception(message: str, err: Exception) -> str:
     """
     Reformat an exception by adding a message to it and reporting the original exception name and message.
     """
     return f"{message} -- {type(err).__name__}: {str(err)}"
 
 
-def get_traceback() -> Union[types.TracebackType, None]:
+def get_traceback() -> types.TracebackType | None:
     """
     Retrieves the traceback after an exception has been raised.
     """
     return sys.exc_info()[2]
 
 
 @dataclasses.dataclass
 class DoExceptParams:
     """
-    Dataclass for the ``do_except`` user supplied handling method.
+    Dataclass for the `do_except` user supplied handling method.
+
+    Attributes:
+
+        err:           The exception instance itself.
+        final_message: The final, combined message
+        trace:         A traceback of the exception
     """
 
     err: Exception
     final_message: str
-    trace: Optional[types.TracebackType]
+    trace: types.TracebackType | None
 
 
 @contextlib.contextmanager
 def handle_errors(
     message: str,
-    raise_exc_class: Union[Type[Exception], None] = Exception,
-    raise_args: Optional[Iterable[Any]] = None,
-    raise_kwargs: Optional[Mapping[str, Any]] = None,
-    handle_exc_class: Union[Type[Exception], Tuple[Type[Exception], ...]] = Exception,
+    raise_exc_class: type[Exception] | None = Exception,
+    raise_args: Iterable[Any] | None = None,
+    raise_kwargs: Mapping[str, Any] | None = None,
+    handle_exc_class: type[Exception] | Tuple[type[Exception], ...] = Exception,
     do_finally: Callable[[], None] = noop,
     do_except: Callable[[DoExceptParams], None] = noop,
     do_else: Callable[[], None] = noop,
     exc_builder: Callable[..., Exception] = default_exc_builder,
 ) -> Iterator[None]:
     """
     Provide a context manager that will intercept exceptions and repackage them with a message attached:
 
-    Example:
+    Args:
+        message:           The message to attach to the raised exception.
+        raise_exc_class:   The exception type to raise with the constructed message if an exception is caught in the
+                           managed context.
+
+                           Defaults to Exception.
+
+                           If ``None`` is passed, no new exception will be raised and only the ``do_except``,
+                           ``do_else``, and ``do_finally`` functions will be called.
+        raise_args:        Additional positional args (after the constructed message) that will passed when raising
+                           an instance of the ``raise_exc_class``.
+        raise_kwargs:      Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
+        handle_exc_class:  Limits the class of exceptions that will be intercepted
+                           Any other exception types will not be caught and re-packaged.
+                           Defaults to Exception (will handle all exceptions). May also be provided as a tuple
+                           of multiple exception types to handle.
+        do_finally:        A function that should always be called at the end of the block.
+                           Should take no parameters.
+        do_except:         A function that should be called only if there was an exception. Must accept one
+                           parameter that is an instance of the ``DoExceptParams`` dataclass.
+                           Note that the ``do_except`` method is passed the *original exception*.
+        do_else:           A function that should be called only if there were no exceptions encountered.
 
-    .. code-block:: python
+    Example:
 
-       with handle_errors("It didn't work"):
-           some_code_that_might_raise_an_exception()
+        The following is an example usage::
 
-    :param: message:           The message to attach to the raised exception.
-    :param: raise_exc_class:   The exception type to raise with the constructed message if an exception is caught in the
-                               managed context.
-
-                               Defaults to Exception.
-
-                               If ``None`` is passed, no new exception will be raised and only the ``do_except``,
-                               ``do_else``, and ``do_finally`` functions will be called.
-    :param: raise_args:        Additional positional args (after the constructed message) that will passed when raising
-                               an instance of the ``raise_exc_class``.
-    :param: raise_kwargs:      Keyword args that will be passed when raising an instance of the ``raise_exc_class``.
-    :param: handle_exc_class:  Limits the class of exceptions that will be intercepted
-                               Any other exception types will not be caught and re-packaged.
-                               Defaults to Exception (will handle all exceptions). May also be provided as a tuple
-                               of multiple exception types to handle.
-    :param: do_finally:        A function that should always be called at the end of the block.
-                               Should take no parameters.
-    :param: do_except:         A function that should be called only if there was an exception. Must accept one
-                               parameter that is an instance of the ``DoExceptParams`` dataclass.
-                               Note that the ``do_except`` method is passed the *original exception*.
-    :param: do_else:           A function that should be called only if there were no exceptions encountered.
+            with handle_errors("It didn't work"):
+                some_code_that_might_raise_an_exception()
     """
     try:
         yield
     except handle_exc_class as err:
         try:
             final_message = reformat_exception(message, err)
         except Exception as msg_err:
```

### Comparing `py_buzz-3.3.0/pyproject.toml` & `py_buzz-4.0.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 [tool.poetry]
 name = "py-buzz"
-version = "3.3.0"
+version = "4.0.0"
 description = "\"That's not flying, it's falling with style\": Exceptions with extras"
 authors = ["Tucker Beck <tucker.beck@gmail.com>"]
 license = "MIT"
-readme = "README.rst"
-packages = [
-    { include = 'buzz' }
-]
+readme = "README.md"
+homepage = "https://github.com/dusktreader/py-buzz"
+repository = "https://github.com/dusktreader/py-buzz"
+documentation = "https://dusktreader.github.io/py-buzz/"
+packages = [{include = "buzz"}]
+
+[tool.poetry.urls]
+CHANGELOG = "https://github.com/dusktreader/py-buzz/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
-dataclasses = { version = "^0.8", python = "~3.6" }
+python = "^3.8"
+
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2"
-sphinx = "^2.0"
-black = "^22.1"
-isort = "^5.10.1"
-pytest-cov = "^3.0.0"
-pyproject-flake8 = "^0.0.1-alpha.2"
-pytest-random-order = "^1.0.4"
-mypy = "^0.961"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+black = "^23.7.0"
+isort = "^5.12.0"
+pytest-cov = "^4.1.0"
+flake8-pyproject = "^1.2.3"
+pytest-random-order = "^1.1.0"
+mypy = "^1.4.1"
+mkdocs-material = "^9.1.21"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 line_length = 120
 lines_after_imports = "2"
@@ -48,9 +53,9 @@
 [[tool.mypy.overrides]]
 module = [
     "dataclasses",
 ]
 ignore_missing_imports = true
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_buzz-3.3.0/PKG-INFO` & `py_buzz-4.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 Metadata-Version: 2.1
 Name: py-buzz
-Version: 3.3.0
+Version: 4.0.0
 Summary: "That's not flying, it's falling with style": Exceptions with extras
+Home-page: https://github.com/dusktreader/py-buzz
 License: MIT
 Author: Tucker Beck
 Author-email: tucker.beck@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dataclasses (>=0.8,<0.9) ; python_version >= "3.6" and python_version < "3.7"
-Description-Content-Type: text/x-rst
+Project-URL: CHANGELOG, https://github.com/dusktreader/py-buzz/blob/main/CHANGELOG.md
+Project-URL: Documentation, https://dusktreader.github.io/py-buzz/
+Project-URL: Repository, https://github.com/dusktreader/py-buzz
+Description-Content-Type: text/markdown
+
+![Latest Version](https://badge.fury.io/py/py-buzz.svg)
+![Build Status](https://github.com/dusktreader/py-buzz/actions/workflows/main.yml/badge.svg)
+![Documentation Status](https://readthedocs.org/projects/py-buzz/badge/?version=latest)
 
-.. image::  https://badge.fury.io/py/py-buzz.svg
-   :target: https://badge.fury.io/py/py-buzz
-   :alt:    Latest Version
-
-.. image::  https://travis-ci.org/dusktreader/py-buzz.svg?branch=integration
-   :target: https://travis-ci.org/dusktreader/py-buzz
-   :alt:    Build Status
-
-.. image::  https://readthedocs.org/projects/py-buzz/badge/?version=latest
-   :target: http://py-buzz.readthedocs.io/en/latest/?badge=latest
-   :alt:    Documentation Status
-
-*********
- py-buzz
-*********
-
-------------------------------------------------------------------
-That's not flying, it's falling with style: Exceptions with extras
-------------------------------------------------------------------
+# py-buzz
+
+**_That's not flying, it's falling with style_: Exceptions with extras**
 
 py-buzz supplies some useful tools to use with python exceptions as well
 as a base Buzz exception class that includes them as classmethods.
 
 py-buzz is fully equipped with exception tools that are written over and over
 again in python projects such as:
 
-* checking conditions and raising errors on failure (``require_conditon``)
-* checking that values are defined and raising errors if not (``enforce_defined``)
+* checking conditions and raising errors on failure (`require_conditon`)
+* checking that values are defined and raising errors if not (`enforce_defined`)
 * catching exceptions wrapping them in clearer exception types with better error
-  messages (``handle_errors``)
+  messages (`handle_errors`)
 * checking many conditions and reporting which ones failed
-  (``check_expressions``)
+  (`check_expressions`)
 
 Buzz can be used as a stand-alone exception class, but it is best used as a
 bass class for custom exceptions within a project. This allows the user to
 focus on creating a set of Exceptions that provide complete coverage for issues
 within their application without having to re-write convenience functions
 themselves.
 
-Super-quick Start
------------------
- - requirements: `python3.6+`
- - install through pip: `$ pip install py-buzz`
- - minimal usage example: `examples/with_buzz_class.py <https://github.com/dusktreader/py-buzz/tree/master/examples/with_buzz_class.py>`_
+## Super-quick Start
+
+* requirements: `python3.6+`
+* install through pip: `$ pip install py-buzz`
+* minimal usage example: [examples/with_buzz_class.py](https://github.com/dusktreader/py-buzz/tree/main/examples/with_buzz_class.py)
 
-Documentation
--------------
+## Documentation
 
 The complete documentation can be found at the
-`py-buzz home page <http://py-buzz.readthedocs.io>`_
+[py-buzz documentation page](http://py-buzz.readthedocs.io)
```

