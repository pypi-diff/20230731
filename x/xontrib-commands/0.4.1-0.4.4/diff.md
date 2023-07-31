# Comparing `tmp/xontrib-commands-0.4.1.tar.gz` & `tmp/xontrib-commands-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-commands-0.4.1.tar", max compression
+gzip compressed data, was "xontrib-commands-0.4.4.tar", last modified: Mon Jul 31 18:25:13 2023, max compression
```

## Comparing `xontrib-commands-0.4.1.tar` & `xontrib-commands-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1075 2022-02-12 06:59:46.191401 xontrib-commands-0.4.1/LICENSE
--rw-r--r--   0        0        0     3342 2022-07-02 12:11:07.083023 xontrib-commands-0.4.1/README.md
--rw-r--r--   0        0        0     1303 2022-07-02 12:11:55.767276 xontrib-commands-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-11 13:56:20.499242 xontrib-commands-0.4.1/xontrib_commands/__init__.py
--rw-r--r--   0        0        0     2359 2022-07-02 10:38:44.459336 xontrib-commands-0.4.1/xontrib_commands/argerize.py
--rw-r--r--   0        0        0        0 2022-07-02 11:48:39.155254 xontrib-commands-0.4.1/xontrib_commands/cmds/__init__.py
--rw-r--r--   0        0        0     5249 2022-07-02 10:24:28.732842 xontrib-commands-0.4.1/xontrib_commands/cmds/dev_cmd.py
--rw-r--r--   0        0        0      520 2022-02-23 16:00:09.394152 xontrib-commands-0.4.1/xontrib_commands/cmds/dotenv_cmd.py
--rw-r--r--   0        0        0     2352 2022-07-02 12:07:47.504500 xontrib-commands-0.4.1/xontrib_commands/cmds/parallex.py
--rw-r--r--   0        0        0     1376 2022-07-02 06:55:44.705727 xontrib-commands-0.4.1/xontrib_commands/cmds/reload.py
--rw-r--r--   0        0        0     2439 2022-07-02 11:49:55.424327 xontrib-commands-0.4.1/xontrib_commands/cmds/report_keys.py
--rw-r--r--   0        0        0      635 2022-07-02 11:48:58.622313 xontrib-commands-0.4.1/xontrib_commands/main.py
--rw-r--r--   0        0        0     1639 2022-07-02 07:06:24.964594 xontrib-commands-0.4.1/xontrib_commands/utils.py
--rw-r--r--   0        0        0     4521 2022-07-02 12:12:03.457268 xontrib-commands-0.4.1/setup.py
--rw-r--r--   0        0        0     4758 2022-07-02 12:12:03.457552 xontrib-commands-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2022-02-12 06:59:46.191401 xontrib-commands-0.4.4/LICENSE
+-rw-r--r--   0        0        0     3958 2023-07-31 17:56:38.781371 xontrib-commands-0.4.4/README.md
+-rw-r--r--   0        0        0     1478 2023-07-31 18:21:02.657837 xontrib-commands-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-02 06:53:58.744193 xontrib-commands-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0     1005 2022-07-02 06:54:56.644152 xontrib-commands-0.4.4/tests/test_parallex.py
+-rw-r--r--   0        0        0        0 2022-05-11 13:56:20.499242 xontrib-commands-0.4.4/xontrib_commands/__init__.py
+-rw-r--r--   0        0        0     2869 2023-07-31 17:49:17.361863 xontrib-commands-0.4.4/xontrib_commands/argerize.py
+-rw-r--r--   0        0        0        0 2022-07-02 11:48:39.155254 xontrib-commands-0.4.4/xontrib_commands/cmds/__init__.py
+-rw-r--r--   0        0        0     5249 2022-07-02 10:24:28.732842 xontrib-commands-0.4.4/xontrib_commands/cmds/dev_cmd.py
+-rw-r--r--   0        0        0      520 2022-02-23 16:00:09.394152 xontrib-commands-0.4.4/xontrib_commands/cmds/dotenv_cmd.py
+-rw-r--r--   0        0        0     2352 2022-07-02 12:07:47.504500 xontrib-commands-0.4.4/xontrib_commands/cmds/parallex.py
+-rw-r--r--   0        0        0     1376 2022-07-02 06:55:44.705727 xontrib-commands-0.4.4/xontrib_commands/cmds/reload.py
+-rw-r--r--   0        0        0     2439 2022-07-02 11:49:55.424327 xontrib-commands-0.4.4/xontrib_commands/cmds/report_keys.py
+-rw-r--r--   0        0        0      635 2022-07-02 11:48:58.622313 xontrib-commands-0.4.4/xontrib_commands/main.py
+-rw-r--r--   0        0        0     1639 2022-07-02 07:06:24.964594 xontrib-commands-0.4.4/xontrib_commands/utils.py
+-rw-r--r--   0        0        0     4952 1970-01-01 00:00:00.000000 xontrib-commands-0.4.4/PKG-INFO
```

### Comparing `xontrib-commands-0.4.1/LICENSE` & `xontrib-commands-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/README.md` & `xontrib-commands-0.4.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -15,26 +15,53 @@
 
 ``` bash
 xontrib load commands
 ```
 
 ## building alias
 
-Use [`xontrib_commands.Command`](https://github.com/jnoortheen/xontrib-commands/blob/main/xontrib/commands.py#L9) 
+Use [`xontrib_commands.argerize:Command`](https://github.com/jnoortheen/xontrib-commands/blob/1bf016e08f192478c6322b2a859ae48567372bdb/xontrib_commands/argerize.py#L21) 
 to build [arger](https://github.com/jnoortheen/arger) dispatcher
-for your functions.
+for your functions. This will create a nice alias function with auto-completions support.
 
 ```py
-from xontrib_commands.utils import Command
+from xontrib_commands.argerize import Command
+
 @Command.reg
 def record_stats(pkg_name=".", path=".local/stats.txt"):
     stat = $(scc @(pkg_name))
     echo @($(date) + stat) | tee -a @(path)
 ```
 
+- Directly passing the `Arger` instances is also supported. 
+
+```py
+from xontrib_commands.argerize import Arger, Command
+
+arger = Arger(prog="tst", description="App Description goes here")
+
+@arger.add_cmd
+def create(name: str):
+    """Create new test.
+
+    :param name: Name of the test
+    """
+    print(locals())
+
+@arger.add_cmd
+def remove(*name: str):
+    """Remove a test with variadic argument.
+
+    :param name: tests to remove
+    """
+    print(locals())
+
+Command.reg(arger)
+```
+
 Now a full CLI is ready
 ```sh
 $ record-stats --help                                                                        
 usage: xonsh [-h] [-p PKG_NAME] [-a PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
```

### Comparing `xontrib-commands-0.4.1/pyproject.toml` & `xontrib-commands-0.4.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,59 @@
-[tool.poetry]
+[project]
+authors = [
+    { name = "Noortheen Raja NJ", email = "jnoortheen@gmail.com" },
+]
+requires-python = ">=3.8"
+dependencies = [
+    "xonsh>=0.12.5",
+    "arger>=1.2.7; python_version >= \"3.6\" and python_version < \"4.0\"",
+    "rich; python_version >= \"3.6\" and python_version < \"4.0\"",
+    "python-dotenv>=0.19.1",
+]
 name = "xontrib-commands"
-version = "0.4.1"
+version = "0.4.4"
 description = "Useful xonsh-shell commands/alias functions"
-authors = ["Noortheen Raja NJ <jnoortheen@gmail.com>"]
-
-license = "MIT"
 readme = "README.md"
-
-repository = "https://github.com/jnoortheen/xontrib-commands"
-keywords = ['xontrib', 'xonsh']
+keywords = [
+    "xontrib",
+    "xonsh",
+]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: System :: Shells",
     "Topic :: System :: System Shells",
     "Topic :: Terminals",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 
-
-packages = [
-    { include = "xontrib_commands" },
+[project.optional-dependencies]
+dev = [
+    "pytest",
+    "black",
 ]
 
-[tool.poetry.urls]
+[project.license]
+text = "MIT"
+
+[project.urls]
 Documentation = "https://github.com/jnoortheen/xontrib-commands/blob/master/README.md"
 Code = "https://github.com/jnoortheen/xontrib-commands"
 "Issue tracker" = "https://github.com/jnoortheen/xontrib-commands/issues"
+repository = "https://github.com/jnoortheen/xontrib-commands"
 
+[project.entry-points."xonsh.xontribs"]
+commands = "xontrib_commands.main"
 
-[tool.poetry.dependencies]
-python = ">=3.8"
-xonsh = { version = ">=0.12.5" }
-arger = { version = ">=1.2.7", python = ">=3.6, <4.0" }
-rich = { version = "*", python = ">=3.6, <4.0" }
-python-dotenv = ">=0.19.1"
-
-[tool.poetry.dev-dependencies]
-pytest = "*"
-black = "*"
+[tool.pdm.build]
+includes = [
+    "xontrib_commands",
+]
 
-[tool.poetry.plugins."xonsh.xontribs"]
-"commands" = "xontrib_commands.main"
+[build-system]
+requires = [
+    "pdm-pep517>=1.0.0",
+]
+build-backend = "pdm.pep517.api"
```

### Comparing `xontrib-commands-0.4.1/xontrib_commands/argerize.py` & `xontrib-commands-0.4.4/xontrib_commands/argerize.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import arger
 from typing import Callable
 
+import arger
+
 from xonsh.built_ins import XSH
 from xonsh.cli_utils import get_argparse_formatter_class, ArgParserAlias
 
 
 class Arger(arger.Arger):
     def __init__(self, **kwargs):
         kwargs.setdefault("formatter_class", get_argparse_formatter_class())
@@ -17,54 +18,70 @@
             action.completer = completer
         return action
 
 
 class Command(ArgParserAlias):
     """Use arger to create commands from functions"""
 
-    def __init__(self, func: Callable, threadable=True, capturable=True, **kwargs):
+    def __init__(
+        self, func: Callable | Arger, threadable=True, capturable=True, **kwargs
+    ):
         """Convert the given function to alias and also create a argparser for its parameters"""
         super().__init__()
-        self.prog = func.__name__.strip("_").replace("_", "-")
+
+        def get_prog_name(func):
+            return func.__name__.strip("_").replace("_", "-")
+
+        if isinstance(func, Arger):
+            if func.func is not None:
+                prog = get_prog_name(func.func)
+            else:
+                prog = func.prog
+            self.arger = func
+            self.kwargs = None
+        else:
+            prog = get_prog_name(func)
+            kwargs["func"] = func
+            kwargs["prog"] = prog
+            self.kwargs = kwargs
+            self.arger = None
+
         if not threadable:
             from xonsh.tools import unthreadable
 
             unthreadable(self)
         if not capturable:
             from xonsh.tools import uncapturable
 
             uncapturable(self)
 
-        kwargs["func"] = func
-        kwargs["prog"] = self.prog
-        self.kwargs = kwargs
-
         # convert to
-        XSH.aliases[self.prog] = self
+        XSH.aliases[prog] = self
 
     @classmethod
-    def reg(cls, func, **kwargs):
+    def reg(cls, func: Callable | Arger, **kwargs):
         """pickle safe way to register alias function"""
         cls(func, **kwargs)
         return func
 
     @classmethod
-    def reg_no_thread(cls, func, **kwargs):
+    def reg_no_thread(cls, func: Callable | Arger, **kwargs):
         """pickle safe way to register alias function that is not threadable"""
         kwargs.setdefault("threadable", False)
         return cls.reg(func, **kwargs)
 
     @classmethod
-    def reg_no_cap(cls, func, **kwargs):
+    def reg_no_cap(cls, func: Callable | Arger, **kwargs):
         """pickle safe way to register alias function that is not capturable"""
         kwargs.setdefault("capturable", False)
         return cls.reg(func, **kwargs)
 
     def build(self) -> "Arger":
-        return Arger(**self.kwargs)
+        # override to return build parser
+        return Arger(**self.kwargs) if self.arger is None else self.arger
 
     def __call__(
         self, args, stdin=None, stdout=None, stderr=None, spec=None, stack=None
     ):
         self.parser.set_defaults(_stdin=stdin)
         self.parser.set_defaults(_stdout=stdout)
         self.parser.set_defaults(_stderr=stderr)
```

### Comparing `xontrib-commands-0.4.1/xontrib_commands/cmds/dev_cmd.py` & `xontrib-commands-0.4.4/xontrib_commands/cmds/dev_cmd.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/cmds/dotenv_cmd.py` & `xontrib-commands-0.4.4/xontrib_commands/cmds/dotenv_cmd.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/cmds/parallex.py` & `xontrib-commands-0.4.4/xontrib_commands/cmds/parallex.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/cmds/reload.py` & `xontrib-commands-0.4.4/xontrib_commands/cmds/reload.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/cmds/report_keys.py` & `xontrib-commands-0.4.4/xontrib_commands/cmds/report_keys.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/main.py` & `xontrib-commands-0.4.4/xontrib_commands/main.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/xontrib_commands/utils.py` & `xontrib-commands-0.4.4/xontrib_commands/utils.py`

 * *Files identical despite different names*

### Comparing `xontrib-commands-0.4.1/PKG-INFO` & `xontrib-commands-0.4.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,29 @@
 Metadata-Version: 2.1
 Name: xontrib-commands
-Version: 0.4.1
+Version: 0.4.4
 Summary: Useful xonsh-shell commands/alias functions
-Home-page: https://github.com/jnoortheen/xontrib-commands
 License: MIT
 Keywords: xontrib,xonsh
-Author: Noortheen Raja NJ
-Author-email: jnoortheen@gmail.com
+Author-email: Noortheen Raja NJ <jnoortheen@gmail.com>
 Requires-Python: >=3.8
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Classifier: Topic :: Terminals
-Requires-Dist: arger (>=1.2.7); python_version >= "3.6" and python_version < "4.0"
-Requires-Dist: python-dotenv (>=0.19.1)
-Requires-Dist: rich; python_version >= "3.6" and python_version < "4.0"
-Requires-Dist: xonsh (>=0.12.5)
+Provides-Extra: dev
 Project-URL: Code, https://github.com/jnoortheen/xontrib-commands
 Project-URL: Documentation, https://github.com/jnoortheen/xontrib-commands/blob/master/README.md
 Project-URL: Issue tracker, https://github.com/jnoortheen/xontrib-commands/issues
-Project-URL: Repository, https://github.com/jnoortheen/xontrib-commands
+Project-URL: repository, https://github.com/jnoortheen/xontrib-commands
 Description-Content-Type: text/markdown
 
 # xontrib-commands
 
 Useful xonsh-shell commands/alias/completer functions
 
 ## Installation
@@ -47,26 +39,53 @@
 
 ``` bash
 xontrib load commands
 ```
 
 ## building alias
 
-Use [`xontrib_commands.Command`](https://github.com/jnoortheen/xontrib-commands/blob/main/xontrib/commands.py#L9) 
+Use [`xontrib_commands.argerize:Command`](https://github.com/jnoortheen/xontrib-commands/blob/1bf016e08f192478c6322b2a859ae48567372bdb/xontrib_commands/argerize.py#L21) 
 to build [arger](https://github.com/jnoortheen/arger) dispatcher
-for your functions.
+for your functions. This will create a nice alias function with auto-completions support.
 
 ```py
-from xontrib_commands.utils import Command
+from xontrib_commands.argerize import Command
+
 @Command.reg
 def record_stats(pkg_name=".", path=".local/stats.txt"):
     stat = $(scc @(pkg_name))
     echo @($(date) + stat) | tee -a @(path)
 ```
 
+- Directly passing the `Arger` instances is also supported. 
+
+```py
+from xontrib_commands.argerize import Arger, Command
+
+arger = Arger(prog="tst", description="App Description goes here")
+
+@arger.add_cmd
+def create(name: str):
+    """Create new test.
+
+    :param name: Name of the test
+    """
+    print(locals())
+
+@arger.add_cmd
+def remove(*name: str):
+    """Remove a test with variadic argument.
+
+    :param name: tests to remove
+    """
+    print(locals())
+
+Command.reg(arger)
+```
+
 Now a full CLI is ready
 ```sh
 $ record-stats --help                                                                        
 usage: xonsh [-h] [-p PKG_NAME] [-a PATH]
 
 optional arguments:
   -h, --help            show this help message and exit
```

