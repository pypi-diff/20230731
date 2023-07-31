# Comparing `tmp/svcs-23.5.0.tar.gz` & `tmp/svcs-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jul 26 13:05:49 2023, max compression
+gzip compressed data, last modified: Mon Jul 31 07:59:54 2023, max compression
```

## Comparing `svcs-23.5.0.tar` & `svcs-23.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      125 2023-07-26 13:05:49.000000 svcs-23.5.0/.git_archival.txt
--rw-r--r--   0        0        0      131 2023-07-26 13:05:49.000000 svcs-23.5.0/.gitattributes
--rw-r--r--   0        0        0      596 2023-07-26 13:05:49.000000 svcs-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-07-26 13:05:49.000000 svcs-23.5.0/.python-version-default
--rw-r--r--   0        0        0     2609 2023-07-26 13:05:49.000000 svcs-23.5.0/CHANGELOG.md
--rw-r--r--   0        0        0    15836 2023-07-26 13:05:49.000000 svcs-23.5.0/README.md
--rw-r--r--   0        0        0      841 2023-07-26 13:05:49.000000 svcs-23.5.0/conftest.py
--rw-r--r--   0        0        0      840 2023-07-26 13:05:49.000000 svcs-23.5.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      285 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4136 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1642 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     1094 2023-07-26 13:05:49.000000 svcs-23.5.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      476 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/__init__.py
--rw-r--r--   0        0        0     9492 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/_core.py
--rw-r--r--   0        0        0      234 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/exceptions.py
--rw-r--r--   0        0        0     3458 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/flask.py
--rw-r--r--   0        0        0        0 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/py.typed
--rw-r--r--   0        0        0       91 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/__init__.py
--rw-r--r--   0        0        0     4555 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_async.py
--rw-r--r--   0        0        0    10959 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_core.py
--rw-r--r--   0        0        0     6426 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_flask.py
--rw-r--r--   0        0        0     1366 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/typing/core.py
--rw-r--r--   0        0        0      935 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      112 2023-07-26 13:05:49.000000 svcs-23.5.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-07-26 13:05:49.000000 svcs-23.5.0/LICENSE
--rw-r--r--   0        0        0     4274 2023-07-26 13:05:49.000000 svcs-23.5.0/pyproject.toml
--rw-r--r--   0        0        0     6743 2023-07-26 13:05:49.000000 svcs-23.5.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-31 07:59:54.000000 svcs-23.6.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-07-31 07:59:54.000000 svcs-23.6.0/.gitattributes
+-rw-r--r--   0        0        0      596 2023-07-31 07:59:54.000000 svcs-23.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-07-31 07:59:54.000000 svcs-23.6.0/.python-version-default
+-rw-r--r--   0        0        0     2887 2023-07-31 07:59:54.000000 svcs-23.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0    16213 2023-07-31 07:59:54.000000 svcs-23.6.0/README.md
+-rw-r--r--   0        0        0      841 2023-07-31 07:59:54.000000 svcs-23.6.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-07-31 07:59:54.000000 svcs-23.6.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      285 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4136 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1610 2023-07-31 07:59:54.000000 svcs-23.6.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     1094 2023-07-31 07:59:54.000000 svcs-23.6.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      476 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/__init__.py
+-rw-r--r--   0        0        0     9466 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/_core.py
+-rw-r--r--   0        0        0      234 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/exceptions.py
+-rw-r--r--   0        0        0     3509 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/flask.py
+-rw-r--r--   0        0        0        0 2023-07-31 07:59:54.000000 svcs-23.6.0/src/svcs/py.typed
+-rw-r--r--   0        0        0       91 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     4555 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_async.py
+-rw-r--r--   0        0        0    10917 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_core.py
+-rw-r--r--   0        0        0     6426 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/test_flask.py
+-rw-r--r--   0        0        0     1366 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/typing/core.py
+-rw-r--r--   0        0        0     1018 2023-07-31 07:59:54.000000 svcs-23.6.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      112 2023-07-31 07:59:54.000000 svcs-23.6.0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-07-31 07:59:54.000000 svcs-23.6.0/LICENSE
+-rw-r--r--   0        0        0     4531 2023-07-31 07:59:54.000000 svcs-23.6.0/pyproject.toml
+-rw-r--r--   0        0        0     7031 2023-07-31 07:59:54.000000 svcs-23.6.0/PKG-INFO
```

### Comparing `svcs-23.5.0/.pre-commit-config.yaml` & `svcs-23.6.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 repos:
   - repo: https://github.com/psf/black
     rev: 23.7.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.0.278
+    rev: v0.0.280
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
 
   - repo: https://github.com/econchick/interrogate
     rev: 1.5.0
     hooks:
```

### Comparing `svcs-23.5.0/CHANGELOG.md` & `svcs-23.6.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,26 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svcs/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [23.6.0](https://github.com/hynek/svcs/compare/23.5.0...23.6.0) - 2023-07-31
+
+### Changed
+
+- Renamed `Container.forget_service_type()` to `Container.forget_about()`.
+
+
+### Fixed
+
+- `svcs.flask.init_app()`'s type hints now take into account custom `flask.Flask` subclasses.
+
+
 ## [23.5.0](https://github.com/hynek/svcs/compare/23.4.0...23.5.0) - 2023-07-26
 
 ### Added
 
 - Registered factory/value clean up!
   It is now possible to register an `on_registry_close` hook that is called once the `Registry`'s `(a)close()` method is called.
```

### Comparing `svcs-23.5.0/README.md` & `svcs-23.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-<!-- begin-pypi -->
-
-
+<!-- begin-logo -->
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
     <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
   </a>
 </p>
-
+<!-- end-logo -->
 
 # *svcs*: A Lightweight Service Locator for Python
 
+<!-- begin-pypi -->
+
 > **Warning**
 > ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
@@ -21,29 +21,30 @@
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
 ---
 
-**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way.**
+**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way without worrying about *cleaning them up*.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
-That:
+Benefits:
 
+- Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
-- and allows for **easy health** checks across *all* resources.
+- and allows for easy **health checks** across *all* resources.
 
 No global mutable state is necessary – but possible for extra comfort.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
@@ -72,21 +73,23 @@
 
 from sqlalchemy import Connection, create_engine
 
 ...
 
 engine = create_engine("postgresql://localhost")
 
-def engine_factory():
+def connection_factory():
     with engine.connect() as conn:
         yield conn
 
 registry = svcs.Registry()
 registry.register_factory(
-    Connection, engine_factory, on_registry_close=engine.dispose
+    Connection,
+    connection_factory,
+    on_registry_close=engine.dispose
 )
 
 @atexit.register
 def cleanup():
     registry.close()  # calls engine.dispose()
 ```
 
@@ -96,15 +99,18 @@
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
 
 ## Is this Dependency Injection!?
 
 No.
 
-Unlike [dependency injection](https://en.wikipedia.org/wiki/Dependency_injection), which passes your dependencies as arguments, you actively ask a service locator for them. This usually requires less opaque magic since nothing meddles with your function/method definitions. But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
+Although the concepts are related and share the idea of having a central registry of services, the ways they provide those services are fundamentally different:
+[Dependency injection](https://en.wikipedia.org/wiki/Dependency_injection) always passes your dependencies as arguments while you actively ask a service locator for them when you need them.
+That usually requires less opaque magic since nothing meddles with your function/method definitions.
+But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
 
 The active acquisition of resources by calling `get()` when you *know* for sure you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool – which also puts the onus of cleanup on you) or eagerly creating resources that you never use:
 
 <!--
 ; skip: next
 -->
 ```python
@@ -187,15 +193,15 @@
 >>> container.get(str)
 'Hello World'
 ```
 
 A container lives as long as you want the instances to live – e.g., as long as a request lives.
 
 Importantly: It is possible to overwrite registered service factories later – e.g., for testing – **without monkey-patching**.
-You have to remove possibly cached instances from the container though (`Container.forget_service_type()`).
+You have to remove possibly cached instances from the container though (`Container.forget_about()`).
 The Flask integration takes care of this for you.
 
 How to achieve this in other frameworks elegantly is TBD.
 
 
 #### Cleanup
 
@@ -437,30 +443,30 @@
 
 🧑‍🍳💋
 
 
 ## Caveats
 
 One would expect the the `Container.get()` method would have a type signature like `get(type: type[T]) -> T`.
-Unfortunately, that's currently impossible because it [precludes the usage of `Protocols` as service types](https://github.com/python/mypy/issues/4717), making this package pointless.
+Unfortunately, that's currently impossible because it [precludes the usage of `Protocols` and *abstract base classes* as service types](https://github.com/python/mypy/issues/4717), making this package pointless.
 
 Therefore it returns `Any`, and until Mypy changes its stance, you have to use it like this:
 
 ```python
 conn: Connection = container.get(Connection)
 ```
 
 If types are more important to you than a unified interface, you can always wrap it:
 
 ```python
 def get_connection() -> Connection:
     return svcs.flask.get(Connection)
 ```
 
-Or, if you don't care about `Protocols`:
+Or, if you don't care about `Protocols` and abstract base classes:
 
 ```python
 def get(svc_type: type[T]) -> T:
     return svcs.flask.get(svc_type)
 ```
```

### Comparing `svcs-23.5.0/conftest.py` & `svcs-23.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/tox.ini` & `svcs-23.6.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/.github/CODE_OF_CONDUCT.md` & `svcs-23.6.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/.github/SECURITY.md` & `svcs-23.6.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/.github/workflows/ci.yml` & `svcs-23.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/.github/workflows/codeql-analysis.yml` & `svcs-23.6.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/.github/workflows/pypi-package.yml` & `svcs-23.6.0/.github/workflows/pypi-package.yml`

 * *Files 10% similar despite different names*

```diff
@@ -24,32 +24,32 @@
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - uses: hynek/build-and-inspect-python-package@v1
 
   # Upload to Test PyPI on every commit on main.
-  # release-test-pypi:
-  #   name: Publish in-dev package to test.pypi.org
-  #   environment: release-test-pypi
-  #   if: github.event_name == 'push' && github.ref == 'refs/heads/main'
-  #   runs-on: ubuntu-latest
-  #   needs: build-package
+  release-test-pypi:
+    name: Publish in-dev package to test.pypi.org
+    environment: release-test-pypi
+    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
+    runs-on: ubuntu-latest
+    needs: build-package
 
-  #   steps:
-  #     - name: Download packages built by build-and-inspect-python-package
-  #       uses: actions/download-artifact@v3
-  #       with:
-  #         name: Packages
-  #         path: dist
+    steps:
+      - name: Download packages built by build-and-inspect-python-package
+        uses: actions/download-artifact@v3
+        with:
+          name: Packages
+          path: dist
 
-  #     - name: Upload package to Test PyPI
-  #       uses: pypa/gh-action-pypi-publish@release/v1
-  #       with:
-  #         repository-url: https://test.pypi.org/legacy/
+      - name: Upload package to Test PyPI
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          repository-url: https://test.pypi.org/legacy/
 
   # Upload to real PyPI on GitHub Releases.
   release-pypi:
     name: Publish released package to pypi.org
     environment: release-pypi
     if: github.event.action == 'published'
     runs-on: ubuntu-latest
```

### Comparing `svcs-23.5.0/docs/_static/logo.svg` & `svcs-23.6.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/src/svcs/_core.py` & `svcs-23.6.0/src/svcs/_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,22 +30,22 @@
 class Container:
     """
     A per-context container for instantiated services & cleanups.
     """
 
     registry: Registry
     _instantiated: dict[type, object] = attrs.Factory(dict)
-    _cleanups: list[
-        tuple[RegisteredService, Generator | AsyncGenerator]
-    ] = attrs.Factory(list)
+    _on_close: list[tuple[str, Generator | AsyncGenerator]] = attrs.Factory(
+        list
+    )
 
     def __repr__(self) -> str:
         return (
             f"<Container(instantiated={len(self._instantiated)}, "
-            f"cleanups={len(self._cleanups)})>"
+            f"cleanups={len(self._on_close)})>"
         )
 
     def get(self, svc_type: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it if necessary and register its cleanup.
@@ -56,15 +56,15 @@
         if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
         svc = rs.factory()
 
         if isinstance(svc, Generator):
-            self._cleanups.append((rs, svc))
+            self._on_close.append((rs.name, svc))
             svc = next(svc)
 
         self._instantiated[rs.svc_type] = svc
 
         return svc
 
     async def aget(self, svc_type: type) -> Any:
@@ -79,93 +79,93 @@
         if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
         svc = rs.factory()
 
         if isinstance(svc, AsyncGenerator):
-            self._cleanups.append((rs, svc))
+            self._on_close.append((rs.name, svc))
             svc = await anext(svc)
         elif isawaitable(svc):
             svc = await svc
 
         self._instantiated[rs.svc_type] = svc
 
         return svc
 
-    def forget_service_type(self, svc_type: type) -> None:
+    def forget_about(self, svc_type: type) -> None:
         """
-        Remove all traces of *svc_type* in ourselves.
+        Remove all traces of *svc_type* from ourselves.
         """
         with suppress(KeyError):
             del self._instantiated[svc_type]
 
     def close(self) -> None:
         """
         Run all registered *synchronous* cleanups.
 
         Async closes are *not* awaited.
         """
-        for rs, gen in reversed(self._cleanups):
+        for name, gen in reversed(self._on_close):
             try:
                 if isinstance(gen, AsyncGenerator):
                     warnings.warn(
-                        f"Skipped async cleanup for {rs.name!r}. "
+                        f"Skipped async cleanup for {name!r}. "
                         "Use aclose() instead.",
                         # stacklevel doesn't matter here; it's coming from a framework.
                         stacklevel=1,
                     )
                     continue
 
                 next(gen)
 
                 warnings.warn(
-                    f"Container clean up for {rs.name!r} didn't stop iterating.",
+                    f"Container clean up for {name!r} didn't stop iterating.",
                     stacklevel=1,
                 )
             except StopIteration:  # noqa: PERF203
                 pass
             except Exception:  # noqa: BLE001
                 log.warning(
                     "Container clean up failed for %r.",
-                    rs.name,
+                    name,
                     exc_info=True,
-                    extra={"svcs_service_name": rs.name},
+                    extra={"svcs_service_name": name},
                 )
 
-        self._cleanups.clear()
+        self._on_close.clear()
         self._instantiated.clear()
 
     async def aclose(self) -> None:
         """
         Run *all* registered cleanups -- synchronous **and** asynchronous.
         """
-        for rs, gen in reversed(self._cleanups):
+        for name, gen in reversed(self._on_close):
             try:
                 if isinstance(gen, AsyncGenerator):
                     await anext(gen)
                 else:
                     next(gen)
 
                 warnings.warn(
-                    f"Container clean up for {rs.name!r} didn't stop iterating.",
+                    f"Container clean up for {name!r} didn't stop iterating.",
                     stacklevel=1,
                 )
 
             except (StopAsyncIteration, StopIteration):  # noqa: PERF203
                 pass
             except Exception:  # noqa: BLE001
                 log.warning(
                     "Container clean up failed for %r.",
-                    rs.name,
+                    name,
                     exc_info=True,
-                    extra={"svcs_service_name": rs.name},
+                    extra={"svcs_service_name": name},
                 )
 
-        self._cleanups.clear()
+        self._on_close.clear()
         self._instantiated.clear()
 
     def get_pings(self) -> list[ServicePing]:
         """
         Get all pingable services and bind them to ourselves for cleanups.
         """
         return [
```

### Comparing `svcs-23.5.0/src/svcs/flask.py` & `svcs-23.6.0/src/svcs/flask.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 # SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from collections.abc import Callable
-from typing import Any
+from typing import Any, TypeVar
 
 from flask import Flask, current_app, g, has_app_context
 
 from ._core import Container, Registry, ServicePing
 
 
-def init_app(app: Flask, registry: Registry | None = None) -> Flask:
+FlaskAppT = TypeVar("FlaskAppT", bound=Flask)
+
+
+def init_app(app: FlaskAppT, registry: Registry | None = None) -> FlaskAppT:
     """
     Initialize *app* for *svcs*.
 
     Creates a registry for you if you don't provide one.
     """
     if registry is None:
         registry = Registry()
@@ -77,15 +80,15 @@
     on_registry_close: Callable | None = None,
 ) -> None:
     """
     Register *factory* for *svc_type* and clear any cached values for it.
     """
     registry, container = _ensure_req_data()
 
-    container.forget_service_type(svc_type)
+    container.forget_about(svc_type)
     registry.register_factory(
         svc_type, factory, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def replace_value(
     svc_type: type,
@@ -95,15 +98,15 @@
     on_registry_close: Callable | None = None,
 ) -> None:
     """
     Register *instance* for *svc_type* and clear any cached values for it.
     """
     registry, container = _ensure_req_data()
 
-    container.forget_service_type(svc_type)
+    container.forget_about(svc_type)
     registry.register_value(
         svc_type, instance, ping=ping, on_registry_close=on_registry_close
     )
 
 
 def get_pings() -> list[ServicePing]:
     """
```

### Comparing `svcs-23.5.0/tests/test_async.py` & `svcs-23.6.0/tests/test_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,23 +73,23 @@
             await asyncio.sleep(0)
             cleaned_up = True
 
         registry.register_factory(Service, factory)
 
         svc = await container.aget(Service)
 
-        assert 1 == len(container._cleanups)
+        assert 1 == len(container._on_close)
         assert Service() == svc
         assert not cleaned_up
 
         await container.aclose()
 
         assert cleaned_up
         assert not container._instantiated
-        assert not container._cleanups
+        assert not container._on_close
 
     @pytest.mark.asyncio()
     async def test_aclose_resilient(self, container, registry, caplog):
         """
         Failing cleanups are logged and ignored. They do not break the
         cleanup process.
         """
@@ -129,15 +129,15 @@
             == caplog.records[0].svcs_service_name
         )
         assert (
             "tests.test_async.Service" == caplog.records[1].svcs_service_name
         )
         assert cleaned_up
         assert not container._instantiated
-        assert not container._cleanups
+        assert not container._on_close
 
     async def test_warns_if_generator_does_not_stop_after_cleanup(
         self, registry, container
     ):
         """
         If a generator doesn't stop after cleanup, a warning is emitted.
         """
```

### Comparing `svcs-23.5.0/tests/test_core.py` & `svcs-23.6.0/tests/test_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,30 +86,30 @@
         registry.register_factory(AnotherService, AnotherService)
         registry.register_value(Service, svc, ping=lambda _: None)
 
         assert [Service] == [
             ping._rs.svc_type for ping in container.get_pings()
         ]
 
-    def test_forget_service_type_nothing_registered(self, container):
+    def test_forget_about_nothing_registered(self, container):
         """
-        forget_service_type does nothing if nothing has been registered.
+        forget_about does nothing if nothing has been registered.
         """
-        container.forget_service_type(Service)
+        container.forget_about(Service)
 
-    def test_forget_service_type_no_cleanup(self, container, rs, svc):
+    def test_forget_about_no_cleanup(self, container, rs, svc):
         """
-        forget_service_type removes the registered service from the container.
+        forget_about removes the registered service from the container.
         """
         container._instantiated[rs.svc_type] = (rs, svc)
 
-        container.forget_service_type(Service)
+        container.forget_about(Service)
 
         assert {} == container._instantiated
-        assert [] == container._cleanups
+        assert [] == container._on_close
 
     @pytest.mark.asyncio()
     async def test_repr(self, registry, container):
         """
         The repr counts correctly.
         """
 
@@ -144,15 +144,15 @@
 
         assert not cleaned_up
 
         container.close()
 
         assert cleaned_up
         assert not container._instantiated
-        assert not container._cleanups
+        assert not container._on_close
 
     def test_close_resilient(self, container, registry, caplog):
         """
         Failing cleanups are logged and ignored. They do not break the
         cleanup process.
         """
 
@@ -287,15 +287,15 @@
 
         assert not cleaned_up
 
         container.close()
 
         assert cleaned_up
         assert not container._instantiated
-        assert not container._cleanups
+        assert not container._on_close
 
 
 class TestRegistry:
     def test_empty_close(self):
         """
         Closing an empty registry does nothing.
         """
```

### Comparing `svcs-23.5.0/tests/test_flask.py` & `svcs-23.6.0/tests/test_flask.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         svcs.flask.replace_factory(Service2, factory2)
 
         svc1 = svcs.flask.get(Service1)
         svc2 = svcs.flask.get(Service2)
 
         assert isinstance(svc1, Service1)
         assert isinstance(svc2, Service2)
-        assert 2 == len(flask.g.svcs_container._cleanups)
+        assert 2 == len(flask.g.svcs_container._on_close)
 
         teardown(None)
 
         cleanup1.assert_called_once_with()
         cleanup2.assert_called_once_with()
 
     def test_overwrite_value(self, registry):
@@ -147,25 +147,25 @@
 
         svcs.flask.replace_factory(Service1, factory1)
         svcs.flask.replace_factory(Service2, factory2)
 
         svcs.flask.get(Service1)
         svcs.flask.get(Service2)
 
-        assert 2 == len(container._cleanups)
+        assert 2 == len(container._on_close)
 
         svcs.flask.replace_factory(Service1, Interface)
 
         svcs.flask.get(Service1)
         svcs.flask.get(Service2)
 
-        assert 2 == len(container._cleanups)
+        assert 2 == len(container._on_close)
 
     @pytest.mark.asyncio()
-    async def test_teardown_warns_on_async_cleanups(self, container):
+    async def test_teardown_warns_on_async_on_close(self, container):
         """
         teardown() warns if there are async cleanups.
         """
 
         async def factory():
             yield Service1()
```

### Comparing `svcs-23.5.0/tests/typing/core.py` & `svcs-23.6.0/tests/typing/core.py`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/tests/typing/flask_.py` & `svcs-23.6.0/tests/typing/flask_.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,7 +33,14 @@
 svcs.flask.register_value(app, str, str, ping=lambda: None)
 
 # The type checker believes whatever we tell it.
 o1: object = svcs.flask.get(object)
 o2: int = svcs.flask.get(object)
 
 svcs.flask.close_registry(app)
+
+
+class CustomApp(Flask):
+    pass
+
+
+app = svcs.flask.init_app(CustomApp("tests"))
```

### Comparing `svcs-23.5.0/LICENSE` & `svcs-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svcs-23.5.0/pyproject.toml` & `svcs-23.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 
 [project]
 dynamic = ["version", "readme"]
 name = "svcs"
-description = "A Lightweight Service Locator for Python"
+description = "A Lightweight Service Locator"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["dependency injection"]
 authors = [{ name = "Hynek Schlawack", email = "hs@ox.cx" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -40,14 +40,22 @@
 raw-options = { local_scheme = "no-local-version" }
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
+start-after = "<!-- begin-logo -->\n"
+end-before = "\n<!-- end-logo -->"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+text = "\n\n# *svcs*: A Lightweight Service Locator\n\n"
+
+[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
+path = "README.md"
 start-after = "<!-- begin-pypi -->\n"
 end-before = "\n<!-- end-pypi -->"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 text = """
 
 ---
@@ -153,21 +161,20 @@
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = [
   "ARG005", # we need stub lambdas
   "S101",   # assert
   "SIM300", # Yoda rocks in asserts
-  "PT005",  # we always add underscores and explicit name
+  "PT005",  # we always add underscores and explicit names
   "PT011",  # broad is fine
   "TRY002", # stock exceptions are fine in tests
   "EM101",  # no need for exception msg hygiene in tests
 ]
 
 "conftest.py" = [
-  "PT005", # we always add underscores and explicit name
+  "PT005", # we always add underscores and explicit names
 ]
 
-
 [tool.ruff.isort]
 lines-between-types = 1
 lines-after-imports = 2
```

### Comparing `svcs-23.5.0/PKG-INFO` & `svcs-23.6.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.5.0
-Summary: A Lightweight Service Locator for Python
+Version: 23.6.0
+Summary: A Lightweight Service Locator
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
 License-File: LICENSE
@@ -29,24 +29,22 @@
 Requires-Dist: pytest-asyncio; extra == 'tests'
 Requires-Dist: sybil; extra == 'tests'
 Provides-Extra: typing
 Requires-Dist: flask; extra == 'typing'
 Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
-
-
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
     <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
   </a>
 </p>
 
+# *svcs*: A Lightweight Service Locator
 
-# *svcs*: A Lightweight Service Locator for Python
 
 > **Warning**
 > ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
@@ -55,29 +53,30 @@
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
 ---
 
-**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way.**
+**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way without worrying about *cleaning them up*.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
 All of this happens *within* your application – service locators are **not** related to service discovery.
 
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
-That:
+Benefits:
 
+- Eliminates tons of repetitive **boilerplate** code,
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
-- and allows for **easy health** checks across *all* resources.
+- and allows for easy **health checks** across *all* resources.
 
 No global mutable state is necessary – but possible for extra comfort.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
@@ -106,21 +105,23 @@
 
 from sqlalchemy import Connection, create_engine
 
 ...
 
 engine = create_engine("postgresql://localhost")
 
-def engine_factory():
+def connection_factory():
     with engine.connect() as conn:
         yield conn
 
 registry = svcs.Registry()
 registry.register_factory(
-    Connection, engine_factory, on_registry_close=engine.dispose
+    Connection,
+    connection_factory,
+    on_registry_close=engine.dispose
 )
 
 @atexit.register
 def cleanup():
     registry.close()  # calls engine.dispose()
 ```
 
@@ -130,15 +131,18 @@
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
 
 ## Is this Dependency Injection!?
 
 No.
 
-Unlike [dependency injection](https://en.wikipedia.org/wiki/Dependency_injection), which passes your dependencies as arguments, you actively ask a service locator for them. This usually requires less opaque magic since nothing meddles with your function/method definitions. But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
+Although the concepts are related and share the idea of having a central registry of services, the ways they provide those services are fundamentally different:
+[Dependency injection](https://en.wikipedia.org/wiki/Dependency_injection) always passes your dependencies as arguments while you actively ask a service locator for them when you need them.
+That usually requires less opaque magic since nothing meddles with your function/method definitions.
+But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
 
 The active acquisition of resources by calling `get()` when you *know* for sure you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool – which also puts the onus of cleanup on you) or eagerly creating resources that you never use:
 
 <!--
 ; skip: next
 -->
 ```python
@@ -159,18 +163,22 @@
 ---
 
 For now, please refer to the [GitHub README](https://github.com/hynek/svcs/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
-### Added
+### Changed
+
+- Renamed `Container.forget_service_type()` to `Container.forget_about()`.
+
+
+### Fixed
 
-- Registered factory/value clean up!
-  It is now possible to register an `on_registry_close` hook that is called once the `Registry`'s `(a)close()` method is called.
+- `svcs.flask.init_app()`'s type hints now take into account custom `flask.Flask` subclasses.
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svcs/blob/main/CHANGELOG.md)
```

