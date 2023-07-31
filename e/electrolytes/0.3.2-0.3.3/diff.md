# Comparing `tmp/electrolytes-0.3.2.tar.gz` & `tmp/electrolytes-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrolytes-0.3.2.tar", last modified: Sun Jul 30 22:54:56 2023, max compression
+gzip compressed data, was "electrolytes-0.3.3.tar", last modified: Mon Jul 31 00:06:29 2023, max compression
```

## Comparing `electrolytes-0.3.2.tar` & `electrolytes-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-30 22:54:43.000000 electrolytes-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-30 22:54:56.430830 electrolytes-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-07-30 22:54:43.000000 electrolytes-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/electrolytes/
--rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/db1.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:43.000000 electrolytes-0.3.2/electrolytes/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/electrolytes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-30 22:54:56.000000 electrolytes-0.3.2/electrolytes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-30 22:54:43.000000 electrolytes-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:54:56.430830 electrolytes-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:54:56.430830 electrolytes-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-30 22:54:43.000000 electrolytes-0.3.2/tests/test_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:06:29.955849 electrolytes-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35130 2023-07-31 00:06:14.000000 electrolytes-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-31 00:06:29.955849 electrolytes-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-07-31 00:06:14.000000 electrolytes-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:06:29.955849 electrolytes-0.3.3/electrolytes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-31 00:06:14.000000 electrolytes-0.3.3/electrolytes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-31 00:06:14.000000 electrolytes-0.3.3/electrolytes/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174238 2023-07-31 00:06:14.000000 electrolytes-0.3.3/electrolytes/db1.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 00:06:14.000000 electrolytes-0.3.3/electrolytes/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:06:29.955849 electrolytes-0.3.3/electrolytes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-31 00:06:29.000000 electrolytes-0.3.3/electrolytes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 00:06:14.000000 electrolytes-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 00:06:29.955849 electrolytes-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 00:06:29.955849 electrolytes-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-31 00:06:14.000000 electrolytes-0.3.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-31 00:06:14.000000 electrolytes-0.3.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-31 00:06:14.000000 electrolytes-0.3.3/tests/test_lock.py
```

### Comparing `electrolytes-0.3.2/LICENSE.txt` & `electrolytes-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.2/PKG-INFO` & `electrolytes-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.2
+Version: 0.3.3
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -36,15 +36,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
-**electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
+**electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
 
 # Installation
```

### Comparing `electrolytes-0.3.2/README.md` & `electrolytes-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
-**electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
+**electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
 
 # Installation
```

### Comparing `electrolytes-0.3.2/electrolytes/__init__.py` & `electrolytes-0.3.3/electrolytes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from contextlib import ContextDecorator
 from warnings import warn
 
 from pydantic import BaseModel, Field, field_validator, FieldValidationInfo, model_validator, TypeAdapter
 from filelock import FileLock
 from typer import get_app_dir
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 
 class Constituent(BaseModel, populate_by_name=True, frozen=True):
     id: Optional[int] = None
     name: str
     u_neg: Annotated[List[float], Field(alias="uNeg")] = [] # [-neg_count, -neg_count+1, -neg_count+2, ..., -1]
     u_pos: Annotated[List[float], Field(alias="uPos")] = [] # [+1, +2, +3, ..., +pos_count]
```

### Comparing `electrolytes-0.3.2/electrolytes/__main__.py` & `electrolytes-0.3.3/electrolytes/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,17 @@
             assert len(charges) == len(uu) == len(pkas)
 
             if not first:
                 typer.echo()
             typer.echo(f"Component: {name}")
             if database.is_user_defined(name):
                 typer.echo("[user-defined]")
-            typer.echo( "                 " + " ".join(f"{c:^+8d}" for c in charges))
-            typer.echo( "Mobilities *1e-9:" + " ".join(f"{u:^8.2f}" for u in uu))
-            typer.echo( "pKas:            " + " ".join(f"{p:^8.2f}" for p in pkas))
+            typer.echo( "                    " + " ".join(f"{c:^+8d}" for c in charges))
+            typer.echo( "Mobilities (*1e-9): " + " ".join(f"{u:^8.2f}" for u in uu))
+            typer.echo( "pKas:               " + " ".join(f"{p:^8.2f}" for p in pkas))
             typer.echo(f"Diffusivity: {constituent.diffusivity():.4e}")
 
             first = False
 
         if errors_ocurred:
             raise typer.Exit(code=1)
```

### Comparing `electrolytes-0.3.2/electrolytes/db1.json` & `electrolytes-0.3.3/electrolytes/db1.json`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.2/electrolytes.egg-info/PKG-INFO` & `electrolytes-0.3.3/electrolytes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: electrolytes
-Version: 0.3.2
+Version: 0.3.3
 Summary: Electrolyte database manager
 Author-email: "Gabriel S. Gerlero" <ggerlero@cimec.unl.edu.ar>
 Project-URL: Homepage, https://github.com/microfluidica/electrolytes
 Project-URL: Repository, https://github.com/microfluidica/electrolytes
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: Pydantic :: 2
@@ -36,15 +36,15 @@
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Pydantic v2](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/pydantic/pydantic/5697b1e4c4a9790ece607654e6c02a160620c7e1/docs/badge/v2.json)](https://pydantic.dev)
 [![PyPI](https://img.shields.io/pypi/v/electrolytes)](https://pypi.org/project/electrolytes/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/electrolytes)](https://pypi.org/project/electrolytes/)
 [![Docker image](https://img.shields.io/badge/docker%20image-microfluidica%2Felectrolytes-0085a0)](https://hub.docker.com/r/microfluidica/electrolytes/)
 
 
-**electrolytes** provides command-line and programatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
+**electrolytes** provides command-line and programmatic access to a database of electrolytes and their properties. It includes 518 components by default (see [credits](#data-credits)). The package covers basic management of the database, including support for storing user-defined electrolytes.
 
 ## [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport)
 
 **electrolytes** is primarily developed as a utility to assist in preparing simulation cases for the [_electroMicroTransport_](https://gitlab.com/santiagomarquezd/electroMicroTransport) toolbox for electromigrative separations. However, it is an independent package and can be installed and used separately.
 
 # Installation
```

### Comparing `electrolytes-0.3.2/pyproject.toml` & `electrolytes-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.2/tests/test_api.py` & `electrolytes-0.3.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.2/tests/test_cli.py` & `electrolytes-0.3.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `electrolytes-0.3.2/tests/test_lock.py` & `electrolytes-0.3.3/tests/test_lock.py`

 * *Files identical despite different names*

