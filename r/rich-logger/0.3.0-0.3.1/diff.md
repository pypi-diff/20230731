# Comparing `tmp/rich_logger-0.3.0.tar.gz` & `tmp/rich-logger-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich_logger-0.3.0.tar", max compression
+gzip compressed data, was "rich-logger-0.3.1.tar", last modified: Mon Jul 31 19:42:06 2023, max compression
```

## Comparing `rich_logger-0.3.0.tar` & `rich-logger-0.3.1.tar`

### file list

```diff
@@ -1,9 +1,21 @@
--rw-r--r--   0        0        0     1525 2022-12-05 10:54:29.294732 rich_logger-0.3.0/LICENSE
--rw-r--r--   0        0        0     2191 2022-12-05 10:54:29.294732 rich_logger-0.3.0/README.md
--rw-r--r--   0        0        0     1157 2022-12-05 10:54:29.298733 rich_logger-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      407 2022-12-05 10:54:29.298733 rich_logger-0.3.0/rich_logger/__init__.py
--rw-r--r--   0        0        0     2801 2022-12-05 10:54:29.298733 rich_logger-0.3.0/rich_logger/pl_logger.py
--rw-r--r--   0        0        0     3668 2022-12-05 10:54:29.298733 rich_logger-0.3.0/rich_logger/spacy_logger.py
--rw-r--r--   0        0        0    18604 2022-12-05 10:54:29.298733 rich_logger-0.3.0/rich_logger/table_printer.py
--rw-r--r--   0        0        0     3047 1970-01-01 00:00:00.000000 rich_logger-0.3.0/setup.py
--rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 rich_logger-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:42:06.569024 rich-logger-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-31 19:41:50.000000 rich-logger-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-31 19:42:06.569024 rich-logger-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-31 19:41:50.000000 rich-logger-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-31 19:41:50.000000 rich-logger-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:42:06.565024 rich-logger-0.3.1/rich_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-31 19:41:50.000000 rich-logger-0.3.1/rich_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-31 19:41:50.000000 rich-logger-0.3.1/rich_logger/pl_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-31 19:41:50.000000 rich-logger-0.3.1/rich_logger/spacy_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-31 19:41:50.000000 rich-logger-0.3.1/rich_logger/table_printer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:42:06.569024 rich-logger-0.3.1/rich_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 19:42:06.000000 rich-logger-0.3.1/rich_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 19:42:06.569024 rich-logger-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:42:06.569024 rich-logger-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-07-31 19:41:50.000000 rich-logger-0.3.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-31 19:41:50.000000 rich-logger-0.3.1/tests/test_pytorch_lightning.py
```

### Comparing `rich_logger-0.3.0/LICENSE` & `rich-logger-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_logger-0.3.0/README.md` & `rich-logger-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rich_logger-0.3.0/pyproject.toml` & `rich-logger-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,75 @@
-[tool.poetry]
+[project]
 name = "rich-logger"
-version = "0.3.0"
+version = "0.3.1"
 description = "Table logger using Rich"
-authors = ["Perceval Wajsbürt <perceval.wajsburt@sorbonne-universite.fr>"]
-license = "BSD 3-Clause"
+authors = [
+    { name = "Perceval Wajsburt", email = "perceval.wajsburt@gmail.com" }
+]
+license = { file = "LICENSE" }
 readme = "README.md"
-packages = [{ include = "rich_logger" }]
+requires-python = ">=3.7,<4.0"
 
-[tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-rich = ">=10.11.0"
-pydantic = ">=1.0.0"
-tqdm = { version = ">=2.0.0", optional = true }
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.1.3"
-coverage = "^6.5.0"
-pytest-cov = "^4.0.0"
-pre-commit = "^2.20.0"
-tqdm = ">=2.0.0"
-pytorch-lightning = ">=1.0.0"
+dependencies = [
+    "rich>=10.11.0",
+    "pydantic>=1.0.0",
+]
 
-[tool.poetry.plugins."spacy_loggers"]
-"rich-logger" = "rich_logger.spacy:rich_logger"
+[project.optional-dependencies]
+dev = [
+    "pytest>=7.1.3",
+    "coverage>=6.5.0",
+    "pytest-cov>=4.0.0",
+    "pre-commit>=2.20.0",
+    "tqdm>=2.0.0",
+    "pytorch-lightning>=1.0.0",
+]
 
+[tool.setuptools.packages.find]
+where = ["."]
+include = ["rich_logger*"]
+namespaces = false
+
+[project.entry-points."spacy_loggers"]
+"rich-logger" = "rich_logger.spacy_logger:rich_logger"
+
+# ----- Documentation -----
 [tool.interrogate]
-ignore-init-method = true
-ignore-init-module = true
+ignore-init-method = false
+ignore-init-module = false
 ignore-magic = false
-ignore-semiprivate = false
+ignore-semiprivate = true
 ignore-private = false
 ignore-property-decorators = false
 ignore-module = true
-ignore-nested-functions = false
+ignore-nested-functions = true
 ignore-nested-classes = true
 ignore-setters = false
-fail-under = 10
+fail-under = 8
 exclude = ["docs", "build", "tests"]
 verbose = 0
 quiet = false
 whitelist-regex = []
+ignore-regex = ['__(?!init).*__']
 color = true
 omit-covered-files = false
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+# ----- Linting & Testing -----
+[tool.ruff]
+fix = true
+exclude = [
+    ".git",
+    "__pycache__",
+    "__init__.py",
+    ".mypy_cache",
+    ".pytest_cache",
+    ".venv",
+    "build",
+]
+line-length = 200
+select = [
+    "E",
+    "F",
+    "W",
+    "I001"
+]
+fixable = ["E", "F", "W", "I"]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rich_logger-0.3.0/rich_logger/pl_logger.py` & `rich-logger-0.3.1/rich_logger/pl_logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from typing import Dict, Optional, Union
 
-from pytorch_lightning.loggers import LightningLoggerBase
-from pytorch_lightning.loggers.base import rank_zero_experiment
+try:
+    from pytorch_lightning.loggers import LightningLoggerBase
+    from pytorch_lightning.loggers.base import rank_zero_experiment
+except ImportError:
+    from pytorch_lightning.loggers.logger import Logger as LightningLoggerBase
+    from pytorch_lightning.loggers.logger import rank_zero_experiment
+
 from pytorch_lightning.utilities import rank_zero_only
 
 from .table_printer import RichTablePrinter
 
 
 class RichTableLogger(LightningLoggerBase):
     def __init__(
```

### Comparing `rich_logger-0.3.0/rich_logger/spacy_logger.py` & `rich-logger-0.3.1/rich_logger/spacy_logger.py`

 * *Files identical despite different names*

### Comparing `rich_logger-0.3.0/rich_logger/table_printer.py` & `rich-logger-0.3.1/rich_logger/table_printer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import time
 import typing
 from collections import OrderedDict
 from enum import Enum
 from numbers import Number
 from typing import Any, Dict, Iterable, Optional, Sequence, Union
 
 from pydantic import BaseModel, Extra
@@ -81,15 +82,14 @@
                 try:
                     from IPython.display import display
                 except ImportError:
                     import warnings
 
                     warnings.warn('install "ipywidgets" for Jupyter support')
                 else:
-
                     if self.ipy_widget is None:
                         self.ipy_widget = display(None, display_id=True)
 
                     self.ipy_widget.update(
                         RichToHTML(
                             renderable=self._live_render.renderable,
                             console=self.console,
@@ -171,15 +171,19 @@
         _text = task.fields.get("postfix", "")
         text = Text(_text)
         return text
 
 
 class RichTablePrinter(Progress):
     def __init__(
-        self, fields: Dict[str, Union[Dict, bool]] = {}, key: Optional[str] = None
+        self,
+        fields: Dict[str, Union[Dict, bool]] = {},
+        key: Optional[str] = None,
+        auto_refresh: bool = False,
+        **rich_kwargs,
     ):
         """
         Logger based on `rich` tables
 
         Parameters
         ----------
         key: Optional[str]
@@ -189,14 +193,18 @@
              format and display name
             The key is a regex that will be used to match the fields to log
             Each entry of the dictionary should match the following scheme:
             - key: a regex to match columns
             - value: either a Dict or False to hide the column, the dict format is
                 - name: the name of the column
                 - goal: "lower_is_better" or "higher_is_better"
+        auto_refresh: bool
+            Should the display auto-refresh ?
+        rich_kwargs: Dict[str, Any]
+            Any parameter to pass on to the `rich.Progress` instance
         """
 
         # Logging attributes
         self.key: str = key
         self.key_to_row_idx: Dict[str, int] = {}
         self.name_to_column_idx: Dict[str, int] = {}
         self.best = {}
@@ -212,14 +220,16 @@
 
         super().__init__(
             TextColumn("[progress.description]{task.description}"),
             BarColumn(),
             TaskProgressColumn(),
             TimeRemainingColumn(),
             PostfixColumn(),
+            auto_refresh=auto_refresh,
+            **rich_kwargs,
         )
         self.live.__class__ = FixedLive
 
     def get_renderables(self) -> Iterable[RenderableType]:
         """Get a number of renderables for the progress display."""
         if self.logger_table is not None:
             yield self.logger_table
@@ -335,17 +345,19 @@
                 self.key_to_row_idx[info[self.key]] = idx
         for name, value in info.items():
             if self.name_to_column_idx[name] < 0:
                 continue
             prev_count = len(
                 self.logger_table.columns[self.name_to_column_idx[name]]._cells
             )
-            formatted_value = get_last_matching_value(self.rules, name, "format", "{}")[
-                1
-            ].format(value)
+            formatter = get_last_matching_value(self.rules, name, "format", "{}")[1]
+            try:
+                formatted_value = formatter.format(value)
+            except ValueError:
+                formatted_value = str(value)
             goal = get_last_matching_value(self.rules, name, "goal", None)[1]
             goal_wait = get_last_matching_value(self.rules, name, "goal_wait", 1)[1]
             if goal is not None:
                 if name not in self.best or prev_count <= goal_wait:
                     self.best[name] = value
                 else:
                     diff = (value - self.best[name]) * (
@@ -431,23 +443,22 @@
             lock_args=None,
             nrows=None,
             colour=None,
             delay=0,
             gui=False,
             **kwargs,
         ):
-            logger.ensure_live()
-
             return TqdmShim(
                 iterable=iterable,
                 description=desc,
                 total=total,
                 leave=leave,
                 disable=disable,
                 printer=logger,
+                min_interval=mininterval,
             )
 
         tqdm.tqdm.__new__ = __new__
 
     def __enter__(self) -> "RichTablePrinter":
         self.hijack_tqdm()
         self.ensure_live()
@@ -462,21 +473,26 @@
         self,
         total,
         iterable,
         disable,
         description,
         leave,
         printer: "RichTablePrinter",
+        min_interval=0.1,
     ):
         self.total = total
         self.iterable = iterable
         self.disable = disable
         self.description = description
         self.leave = leave
         self.printer = printer
+        self.last_tick = time.time()
+        self.min_interval = min_interval
+
+        printer.ensure_live()
 
         if self.disable:
             self.task = self.task_id = None
         else:
             if self.total is None:
                 try:
                     self.total = len(self.iterable)
@@ -495,37 +511,42 @@
     def __iter__(self):
         if self.disable:
             yield from self.iterable
         else:
             try:
                 for item in self.iterable:
                     yield item
-                    self.printer.update(self.task_id, advance=1)
+                    self.update(1)
             finally:
                 if not self.leave:
                     self.task["disposable"] = True
 
     def reset(self, total=0):
         if self.task_id is None:
             return
         self.printer.reset(self.task_id, total=total)
 
     def update(self, n=1):
         if self.task_id is None:
             return
         self.printer.update(self.task_id, advance=n)
+        self.refresh()
 
     def set_description(self, desc, refresh=True):
         if self.task_id is None:
             return
         self.printer.update(self.task_id, description=desc)
         if refresh:
-            self.printer.refresh()
+            self.refresh()
 
     def refresh(self):
+        tick = time.time()
+        if tick - self.last_tick < self.min_interval:
+            return
+        self.last_tick = tick
         if self.task_id is None:
             return
         self.printer.refresh()
 
     @staticmethod
     def format_num(n):
         """
@@ -578,13 +599,20 @@
         self.printer.update(
             self.task_id,
             postfix=", ".join(
                 key + "=" + postfix[key].strip() for key in postfix.keys()
             ),
         )
         if refresh:
-            self.printer.refresh()
+            self.refresh()
 
     def close(self):
+        self.refresh()
         if self.task is not None:
             self.task["disposable"] = True
         self.printer.prune_tasks()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.close()
```

