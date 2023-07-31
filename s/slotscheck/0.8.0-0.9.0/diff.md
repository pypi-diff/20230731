# Comparing `tmp/slotscheck-0.8.0.tar.gz` & `tmp/slotscheck-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slotscheck-0.8.0.tar", max compression
+gzip compressed data, was "slotscheck-0.9.0.tar", max compression
```

## Comparing `slotscheck-0.8.0.tar` & `slotscheck-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2356 2022-01-21 21:15:44.118318 slotscheck-0.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1071 2022-01-04 09:21:37.081245 slotscheck-0.8.0/LICENSE
--rw-r--r--   0        0        0     3551 2022-01-21 21:15:44.119010 slotscheck-0.8.0/README.rst
--rw-r--r--   0        0        0     1689 2022-01-21 21:15:44.120509 slotscheck-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      325 2022-01-03 21:47:49.048980 slotscheck-0.8.0/src/slotscheck/__init__.py
--rw-r--r--   0        0        0       61 2022-01-10 20:35:10.786398 slotscheck-0.8.0/src/slotscheck/__main__.py
--rw-r--r--   0        0        0     1668 2022-01-18 17:36:32.262303 slotscheck-0.8.0/src/slotscheck/checks.py
--rw-r--r--   0        0        0    12188 2022-01-21 21:15:44.122603 slotscheck-0.8.0/src/slotscheck/cli.py
--rw-r--r--   0        0        0     2997 2022-01-18 17:47:16.397604 slotscheck-0.8.0/src/slotscheck/common.py
--rw-r--r--   0        0        0     3814 2022-01-18 17:47:16.398189 slotscheck-0.8.0/src/slotscheck/config.py
--rw-r--r--   0        0        0     8564 2022-01-21 21:15:44.124919 slotscheck-0.8.0/src/slotscheck/discovery.py
--rw-r--r--   0        0        0        0 2021-12-25 11:27:51.729907 slotscheck-0.8.0/src/slotscheck/py.typed
--rw-r--r--   0        0        0     4697 2022-01-21 21:15:52.675541 slotscheck-0.8.0/setup.py
--rw-r--r--   0        0        0     4634 2022-01-21 21:15:52.676405 slotscheck-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     2510 2022-01-25 19:00:40.478634 slotscheck-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1071 2022-01-04 09:21:37.081245 slotscheck-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3551 2022-01-21 21:15:44.119010 slotscheck-0.9.0/README.rst
+-rw-r--r--   0        0        0     1689 2022-01-25 19:00:40.479261 slotscheck-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      325 2022-01-03 21:47:49.048980 slotscheck-0.9.0/src/slotscheck/__init__.py
+-rw-r--r--   0        0        0       61 2022-01-10 20:35:10.786398 slotscheck-0.9.0/src/slotscheck/__main__.py
+-rw-r--r--   0        0        0     1668 2022-01-18 17:36:32.262303 slotscheck-0.9.0/src/slotscheck/checks.py
+-rw-r--r--   0        0        0    12585 2022-01-25 19:00:40.479764 slotscheck-0.9.0/src/slotscheck/cli.py
+-rw-r--r--   0        0        0     2997 2022-01-18 17:47:16.397604 slotscheck-0.9.0/src/slotscheck/common.py
+-rw-r--r--   0        0        0     3854 2022-01-25 19:00:40.480407 slotscheck-0.9.0/src/slotscheck/config.py
+-rw-r--r--   0        0        0     8564 2022-01-21 21:15:44.124919 slotscheck-0.9.0/src/slotscheck/discovery.py
+-rw-r--r--   0        0        0        0 2021-12-25 11:27:51.729907 slotscheck-0.9.0/src/slotscheck/py.typed
+-rw-r--r--   0        0        0     4697 2022-01-25 19:01:00.109424 slotscheck-0.9.0/setup.py
+-rw-r--r--   0        0        0     4634 2022-01-25 19:01:00.109950 slotscheck-0.9.0/PKG-INFO
```

### Comparing `slotscheck-0.8.0/CHANGELOG.rst` & `slotscheck-0.9.0/CHANGELOG.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+0.9.0 (2022-01-25)
+------------------
+
+- Support specifying the location of settings file with ``--settings`` option.
+- Improved verbose error messages.
+
 0.8.0 (2022-01-21)
 ------------------
 
 - Extension modules are now traversed.
 - Small tweaks to documentation.
 
 0.7.2 (2022-01-18)
```

### Comparing `slotscheck-0.8.0/LICENSE` & `slotscheck-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slotscheck-0.8.0/README.rst` & `slotscheck-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `slotscheck-0.8.0/pyproject.toml` & `slotscheck-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slotscheck"
-version = "0.8.0"
+version = "0.9.0"
 description = "Ensure your __slots__ are working properly."
 authors = ["Arie Bovenberg <a.c.bovenberg@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Typing :: Typed",
     "Topic :: Software Development :: Quality Assurance",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `slotscheck-0.8.0/src/slotscheck/checks.py` & `slotscheck-0.9.0/src/slotscheck/checks.py`

 * *Files identical despite different names*

### Comparing `slotscheck-0.8.0/src/slotscheck/cli.py` & `slotscheck-0.9.0/src/slotscheck/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,23 +109,30 @@
     "For example: ``app\\.config:Settings``, ``:.*(Exception|Error)``. "
     "Uses Python's verbose regex dialect, so whitespace is mostly ignored.",
     show_default="^$",
 )
 @click.option(
     "-v", "--verbose", is_flag=True, help="Display extra descriptive output."
 )
+@click.option(
+    "--settings",
+    type=click.Path(
+        path_type=Path, exists=True, resolve_path=True, dir_okay=False
+    ),
+)
 @click.version_option()
 def root(
     files: Sequence[Path],
     module: Sequence[str],
     verbose: bool,
+    settings: Optional[Path],
     **kwargs: Any,
 ) -> None:
     "Check whether your __slots__ are working properly."
-    conf = config.collect(kwargs, Path.cwd())
+    conf = config.collect(kwargs, Path.cwd(), settings)
     if not (files or module):
         print("No files or modules given. Nothing to do!")
         exit(0)
 
     try:
         classes, modules = _collect(files, module, conf)
     except ModuleNotFoundError as e:
@@ -198,15 +205,15 @@
     def for_display(self, verbose: bool) -> str:
         return (
             f"'{_class_fullname(self.cls)}' defines overlapping slots."
             + verbose
             * (
                 "\n"
                 + _bulletlist(
-                    f"{name} ({_class_fullname(base)})"
+                    f"'{name}' is also defined in '{_class_fullname(base)}'"
                     for name, base in sorted(
                         _overlapping_slots(self.cls), key=itemgetter(0)
                     )
                 )
             )
         )
 
@@ -224,15 +231,26 @@
     cls: type
 
     def for_display(self, verbose: bool) -> str:
         return (
             f"'{_class_fullname(self.cls)}' has slots "
             "but superclass does not."
             + verbose
-            * ("\n" + _class_bulletlist(_slotless_superclasses(self.cls)))
+            * (
+                "\n"
+                + _bulletlist(
+                    map(
+                        compose(
+                            "'{}' superclass has no slots.".format,
+                            _class_fullname,
+                        ),
+                        _slotless_superclasses(self.cls),
+                    )
+                )
+            )
         )
 
 
 @add_slots
 @dataclass(frozen=True)
 class ShouldHaveSlots:
     cls: type
@@ -460,17 +478,13 @@
     )
 
 
 def _class_fullname(k: type) -> str:
     return f"{k.__module__}:{k.__qualname__}"
 
 
-def _class_bulletlist(cs: Iterable[type]) -> str:
-    return _bulletlist(map(_class_fullname, cs))
-
-
 def _bulletlist(s: Iterable[str]) -> str:
     return "\n".join(map("- {}".format, s))
 
 
 def _slotless_superclasses(c: type) -> Iterable[type]:
     return filterfalse(has_slots, c.mro())
```

### Comparing `slotscheck-0.8.0/src/slotscheck/common.py` & `slotscheck-0.9.0/src/slotscheck/common.py`

 * *Files identical despite different names*

### Comparing `slotscheck-0.8.0/src/slotscheck/config.py` & `slotscheck-0.9.0/src/slotscheck/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,18 @@
     include_modules=None,
     exclude_modules=DEFAULT_MODULE_EXCLUDE_RE,
     include_classes=None,
     exclude_classes=None,
 )
 
 
-def collect(cli_kwargs: Mapping[str, Any], cwd: Path) -> Config:
-    tomlpath = find_pyproject_toml(cwd)
+def collect(
+    cli_kwargs: Mapping[str, Any], cwd: Path, config: Optional[Path]
+) -> Config:
+    tomlpath = config or find_pyproject_toml(cwd)
     toml_conf = (
         PartialConfig.from_toml(tomlpath) if tomlpath else PartialConfig.EMPTY
     )
     return Config.DEFAULT.apply(toml_conf).apply(PartialConfig(**cli_kwargs))
 
 
 def find_pyproject_toml(path: Path) -> Optional[Path]:
```

### Comparing `slotscheck-0.8.0/src/slotscheck/discovery.py` & `slotscheck-0.9.0/src/slotscheck/discovery.py`

 * *Files identical despite different names*

### Comparing `slotscheck-0.8.0/setup.py` & `slotscheck-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  ':python_version < "3.8"': ['importlib-metadata>=1,<5']}
 
 entry_points = \
 {'console_scripts': ['slotscheck = slotscheck.cli:root']}
 
 setup_kwargs = {
     'name': 'slotscheck',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Ensure your __slots__ are working properly.',
     'long_description': '🎰 Slotscheck\n=============\n\n.. image:: https://img.shields.io/pypi/v/slotscheck.svg?color=blue\n   :target: https://pypi.python.org/pypi/slotscheck\n\n.. image:: https://img.shields.io/pypi/l/slotscheck.svg\n   :target: https://pypi.python.org/pypi/slotscheck\n\n.. image:: https://img.shields.io/pypi/pyversions/slotscheck.svg\n   :target: https://pypi.python.org/pypi/slotscheck\n\n.. image:: https://img.shields.io/readthedocs/slotscheck.svg\n   :target: http://slotscheck.readthedocs.io/\n\n.. image:: https://github.com/ariebovenberg/slotscheck/actions/workflows/build.yml/badge.svg\n   :target: https://github.com/ariebovenberg/slotscheck/actions/workflows/build.yml\n\n.. image:: https://img.shields.io/codecov/c/github/ariebovenberg/slotscheck.svg\n   :target: https://codecov.io/gh/ariebovenberg/slotscheck\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n\nAdding ``__slots__`` to a class in Python is a great way to reduce memory usage.\nBut to work properly, all base classes need to implement it — without overlap!\nIt\'s easy to get wrong, and what\'s worse: there is nothing warning you that you messed up.\n\n✨ *Until now!* ✨\n\n``slotscheck`` helps you validate your slots are working properly.\nYou can even use it to enforce the use of slots across (parts of) your codebase.\n\nSee my `blog post <https://dev.arie.bovenberg.net/blog/finding-broken-slots-in-popular-python-libraries/>`_\nfor the origin story behind ``slotscheck``.\n\nQuickstart\n----------\n\nUsage is quick from the command line:\n\n.. code-block:: bash\n\n   python -m slotscheck [FILES]...\n   # or\n   slotscheck -m [MODULES]...\n\nFor example:\n\n.. code-block:: bash\n\n   $ slotscheck -m sanic\n   ERROR: \'sanic.app:Sanic\' defines overlapping slots.\n   ERROR: \'sanic.response:HTTPResponse\' has slots but superclass does not.\n   Oh no, found some problems!\n   Scanned 72 module(s), 111 class(es).\n\nNow get to fixing —\nand add ``slotscheck`` to your CI pipeline to prevent mistakes from creeping in again!\nSee `here <https://github.com/Instagram/LibCST/pull/615>`__ and\n`here <https://github.com/dry-python/returns/pull/1233>`__ for examples.\n\nFeatures\n--------\n\n- Detect broken slots inheritance\n- Detect overlapping slots\n- `Pre-commit <https://slotscheck.rtfd.io/en/latest/advanced.html#pre-commit-hook>`_ hook\n- (Optionally) enforce the use of slots\n\nSee `the documentation <https://slotscheck.rtfd.io>`_ for more details\nand configuration options.\n\nWhy not a flake8 plugin?\n------------------------\n\nFlake8 plugins need to work without running the code.\nMany libraries use conditional imports, star imports, re-exports,\nand define slots with decorators or metaclasses.\nThis all but requires running the code to determine the slots and class tree.\n\nThere\'s `an issue <https://github.com/ariebovenberg/slotscheck/issues/6>`_\nto discuss the matter.\n\nNotes\n-----\n\n- ``slotscheck`` will try to import all submodules of the given package.\n  If there are scripts without ``if __name__ == "__main__":`` blocks,\n  they may be executed.\n- Even in the case that slots are not inherited properly,\n  there may still be an advantage to using them\n  (i.e. attribute access speed and *some* memory savings).\n  However, in most cases this is unintentional.\n  ``slotscheck`` allows you to ignore specific cases.\n- Non pure-Python classes are currently assumed to have slots.\n  This is not necessarily the case, but it is nontrivial to determine.\n\nInstallation\n------------\n\nIt\'s available on PyPI.\n\n.. code-block:: bash\n\n  pip install slotscheck\n',
     'author': 'Arie Bovenberg',
     'author_email': 'a.c.bovenberg@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/ariebovenberg/slotscheck',
```

### Comparing `slotscheck-0.8.0/PKG-INFO` & `slotscheck-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slotscheck
-Version: 0.8.0
+Version: 0.9.0
 Summary: Ensure your __slots__ are working properly.
 Home-page: https://github.com/ariebovenberg/slotscheck
 License: MIT
 Author: Arie Bovenberg
 Author-email: a.c.bovenberg@gmail.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: MIT License
```

