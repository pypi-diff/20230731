# Comparing `tmp/python-libdiscid-2.0.2.tar.gz` & `tmp/python-libdiscid-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-libdiscid-2.0.2.tar", last modified: Tue Nov  1 17:20:41 2022, max compression
+gzip compressed data, was "python-libdiscid-2.0.3.tar", last modified: Mon Jul 31 20:59:33 2023, max compression
```

## Comparing `python-libdiscid-2.0.2.tar` & `python-libdiscid-2.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.042669 python-libdiscid-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-11-01 17:20:41.042669 python-libdiscid-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.034669 python-libdiscid-2.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/api.compat.rst
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5928 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      501 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2972 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2521 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.034669 python-libdiscid-2.0.2/libdiscid/
--rw-r--r--   0 runner    (1001) docker     (121)     9938 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/_discid.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     8808 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/_discid.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/cdiscid.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.038669 python-libdiscid-2.0.2/libdiscid/compat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6337 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/compat/discid.py
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/discid-wrapper.c
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/discid-wrapper.h
--rw-r--r--   0 runner    (1001) docker     (121)     1336 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.038669 python-libdiscid-2.0.2/libdiscid/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5613 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/tests/test_compat_discid.py
--rw-r--r--   0 runner    (1001) docker     (121)     5785 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/libdiscid/tests/test_libdiscid.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 17:20:41.038669 python-libdiscid-2.0.2/python_libdiscid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-11-01 17:20:40.000000 python-libdiscid-2.0.2/python_libdiscid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-11-01 17:20:41.000000 python-libdiscid-2.0.2/python_libdiscid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 17:20:40.000000 python-libdiscid-2.0.2/python_libdiscid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-01 17:20:40.000000 python-libdiscid-2.0.2/python_libdiscid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-11-01 17:20:41.042669 python-libdiscid-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1721 2022-11-01 17:20:22.000000 python-libdiscid-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/api.compat.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/libdiscid/
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/_discid.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/_discid.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/cdiscid.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/libdiscid/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/compat/discid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/discid-wrapper.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/discid-wrapper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/libdiscid/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/tests/test_compat_discid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/libdiscid/tests/test_libdiscid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/python_libdiscid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-31 20:59:33.000000 python-libdiscid-2.0.3/python_libdiscid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-31 20:59:33.000000 python-libdiscid-2.0.3/python_libdiscid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:59:33.000000 python-libdiscid-2.0.3/python_libdiscid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-31 20:59:33.000000 python-libdiscid-2.0.3/python_libdiscid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-31 20:59:33.550363 python-libdiscid-2.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1721 2023-07-31 20:59:19.000000 python-libdiscid-2.0.3/setup.py
```

### Comparing `python-libdiscid-2.0.2/CHANGELOG.md` & `python-libdiscid-2.0.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 2.0.3 (2023-07-31)
+
+* Bump required Python version to 3.8.
+* Fix compatibility with Sphinx 7.
+
 ## 2.0.2 (2022-11-01)
 
   * Remove long deprecated `libdiscid.DEFAULT_DEVICE`.
   * Bump required Python version to 3.7.
 
 ## 2.0.1 (2021-02-11)
```

### Comparing `python-libdiscid-2.0.2/LICENSE` & `python-libdiscid-2.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2013-2022 Sebastian Ramacher <sebastian+dev@ramacher.at>
+Copyright (C) 2013-2023 Sebastian Ramacher <sebastian+dev@ramacher.at>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `python-libdiscid-2.0.2/PKG-INFO` & `python-libdiscid-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: python-libdiscid
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python bindings for libdiscid
 Home-page: https://github.com/sebastinas/python-libdiscid
 Author: Sebastian Ramacher
 Author-email: sebastian@ramacher.at
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio :: CD Ripping
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libdiscid Python bindings
 
 python-libdiscid implements Python >= 3.6 bindings for libdiscid using Cython.
```

### Comparing `python-libdiscid-2.0.2/README.md` & `python-libdiscid-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/docs/conf.py` & `python-libdiscid-2.0.3/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.intersphinx", "sphinx.ext.extlinks"]
+extensions = ["sphinx.ext.autodoc", "sphinx.ext.intersphinx"]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
 
@@ -41,15 +41,15 @@
 source_encoding = "UTF-8"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "python-libdiscid"
-copyright = "2013-2022, Sebastian Ramacher"
+copyright = "2013-2023, Sebastian Ramacher"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = libdiscid.__version__
@@ -167,15 +167,11 @@
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "python-libdisciddoc"
 
 
-extlinks = {
-    "musicbrainz": ("http://musicbrainz.org/doc/%s", ""),
-}
-
 intersphinx_mapping = {
     "python": ("http://docs.python.org/", None),
     "pydiscid": ("https://python-discid.readthedocs.org/en/latest/", None),
 }
```

### Comparing `python-libdiscid-2.0.2/docs/installation.rst` & `python-libdiscid-2.0.3/docs/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ------------
 
 Dependencies
 ^^^^^^^^^^^^
 
 `python-libdiscid` depends on the following components:
 
-* :musicbrainz:`libdiscid`
+* libdiscid_
 * `Cython`__ (>= 0.15)
 * `pkgconfig`__
 
 Note that `Cython` is only required if one builds `python-libdiscid` from the
 repository. The released tarballs ship with pre-built C source files for the
 extension mdoules.
 
@@ -52,15 +52,15 @@
  python setup.py install
 
 A note for Windows users
 ~~~~~~~~~~~~~~~~~~~~~~~~
 
 There are eggs available from the same source too. With these eggs, the
 extension module comes pre-built. However, you still need to fetch
-`discid.dll` from :musicbrainz:`libdiscid` and copy the DLL to somewhere it can
+`discid.dll` from libdiscid_ and copy the DLL to somewhere it can
 be found, e.g. to ``C:\WINDOWS\system32``.
 
 .. __: https://pypi.python.org/pypi/python-libdiscid/
 .. __: https://pypi.python.org/pypi/python-libdiscid/
 
 Building python-libdiscid locally
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -87,8 +87,9 @@
     import sys, os
     sys.path.insert(0, os.path.abspath('build/lib.linux-x86_64-3.4'))
     import libdiscid
 
   Please note that modification to any file in the ``libdiscid`` directory will
   only be available after another run of ``python setup.py build``.
 
+.. _libdiscid: https://musicbrainz.org/doc/libdiscid
 .. __: http://pythonhosted.org/distribute/setuptools.html#development-mode
```

### Comparing `python-libdiscid-2.0.2/docs/misc.rst` & `python-libdiscid-2.0.3/docs/misc.rst`

 * *Files 8% similar despite different names*

```diff
@@ -9,25 +9,26 @@
 Supported libdiscid features
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 `python-libdiscid` supports all the features introduced by `libdiscid` up to
 version 0.6.0, that is:
 
 * retrieval of the disc's Media Catalogue Number and retrieving the
-  :musicbrainz:`International Standard Recording Code <ISRC>` of
+  International Standard Recording Code (ISRC) of
   the tracks if you are using `libdiscid` 0.4.0 and above.
 * selective reading support if you are using `libdiscid` 0.5.0 and above.
 * fuzzy TOC lookup if you are using `libdiscid` 0.6.0 and above.
 
 Please note that if `python-libdiscid` was built against versions of `libdiscid`
 prior to 0.4.0 or 0.5.0, `python-libdiscid` has to be rebuilt against the newer
 version to detect the features of the newer `libdiscid`.
 
 Other Python bindings
 ^^^^^^^^^^^^^^^^^^^^^
 
 There are other Python bindings available. `python-discid`__ is the most
 prominent one. For a full list of bindings (including bindings for other
-languages) check musicbrainz:`libdiscid`.
+languages) check libdiscid_.
 
 .. _GitHub: https://github.com/sebastinas/python-libdiscid
+.. _libdiscid: https://musicbrainz.org/doc/libdiscid
 .. __: https://github.com/JonnyJD/python-discid
```

### Comparing `python-libdiscid-2.0.2/docs/usage.rst` & `python-libdiscid-2.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/__init__.py` & `python-libdiscid-2.0.3/libdiscid/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2013-2021 Sebastian Ramacher <sebastian+dev@ramacher.at>
+# Copyright 2013-2023 Sebastian Ramacher <sebastian+dev@ramacher.at>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -31,30 +31,30 @@
 
 from . import _discid
 from .exceptions import DiscError
 from typing import Optional, Union, List, Tuple
 import re
 import warnings
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
 __author__ = "Sebastian Ramacher"
 __license__ = "MIT"
-__copyright__ = f"(C) 2013-2022 {__author__}"
+__copyright__ = f"(C) 2013-2023 {__author__}"
 
 FEATURES = _discid.FEATURES
 """Tuple of all available features supported by libdiscid on this platform.
 """
 FEATURE_READ = _discid.FEATURE_READ
 """Read the TOC of the disc to get the disc ID. This feature is always enabled.
 """
 FEATURE_MCN = _discid.FEATURE_MCN
 """Read the Media Catalogue Number of the disc.
 """
 FEATURE_ISRC = _discid.FEATURE_ISRC
-"""Read :musicbrainz:`International Standard Recording Codes <ISRC>` of all the
+"""Read International Standard Recording Codes (ISRC) of all the
 tracks.
 """
 FEATURES_MAPPING = _discid.FEATURES_MAPPING
 """Mapping between the constants representing a feature and their string
 representation.
 """
 __discid_version__ = _discid.__discid_version__
@@ -81,30 +81,30 @@
         self._mcn = cdiscid.mcn
         self._track_isrcs = cdiscid.track_isrcs
         self._device = cdiscid.device
         self._toc = cdiscid.toc
 
     @property
     def id(self) -> str:
-        """The MusicBrainz :musicbrainz:`Disc ID`."""
+        """The MusicBrainz Disc ID."""
 
         return self._id
 
     @property
     def freedb_id(self) -> str:
-        """The :musicbrainz:`FreeDB` Disc ID (without category)."""
+        """The FreeDB Disc ID (without category)."""
 
         return self._freedb_id
 
     @property
     def submission_url(self) -> str:
         """Disc ID / TOC Submission URL for MusicBrainz
 
         With this url you can submit the current TOC as a new MusicBrainz
-        :musicbrainz:`Disc ID`.
+        Disc ID.
         """
 
         return self._submission_url
 
     @property
     def webservice_url(self) -> str:
         """The web service URL for info about the CD
@@ -182,15 +182,15 @@
             raise NotImplementedError(
                 "MCN is not available with this version " "of libdiscid and/or platform"
             )
         return self._mcn
 
     @property
     def track_isrcs(self) -> Tuple[str]:
-        """Tuple of :musicbrainz:`ISRCs <ISRC>` of all tracks.
+        """Tuple of ISRCs of all tracks.
 
         The first element of the list corresponds to the ISRC of the
         :attr:`first_track` and so on.
 
         :raises NotImplementedError: reading ISRCs is not supported on this platform
         """
```

### Comparing `python-libdiscid-2.0.2/libdiscid/_discid.pyi` & `python-libdiscid-2.0.3/libdiscid/_discid.pyi`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/_discid.pyx` & `python-libdiscid-2.0.3/libdiscid/_discid.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -125,32 +125,32 @@
             free(coffsets)
 
     cdef str _get_error_msg(self):
         return _to_str(cdiscid.discid_get_error_msg(self._c_discid))
 
     @property
     def id(self):
-        """The MusicBrainz :musicbrainz:`Disc ID`.
+        """The MusicBrainz Disc ID.
         """
 
         return _to_str(cdiscid.discid_get_id(self._c_discid))
 
     @property
     def freedb_id(self):
-        """The :musicbrainz:`FreeDB` Disc ID (without category).
+        """The FreeDB Disc ID (without category).
         """
 
         return _to_str(cdiscid.discid_get_freedb_id(self._c_discid))
 
     @property
     def submission_url(self):
         """Disc ID / TOC Submission URL for MusicBrainz
 
         With this url you can submit the current TOC as a new MusicBrainz
-        :musicbrainz:`Disc ID`.
+        Disc ID.
         """
 
         return _to_str(cdiscid.discid_get_submission_url(self._c_discid))
 
     @property
     def webservice_url(self):
         """The web service URL for info about the CD
@@ -215,15 +215,15 @@
 
         if not _has_feature(cdiscid.DISCID_FEATURE_MCN):
             return None
         return _to_str(cdiscid.wrap_get_mcn(self._c_discid))
 
     @property
     def track_isrcs(self):
-        """Tuple of :musicbrainz:`ISRCs <ISRC>` of all tracks.
+        """Tuple of ISRCs of all tracks.
 
         The first element of the list corresponds to the ISRC of the
         :attr:`first_track` and so on.
         """
 
         if not _has_feature(cdiscid.DISCID_FEATURE_ISRC):
           return None
```

### Comparing `python-libdiscid-2.0.2/libdiscid/cdiscid.pxd` & `python-libdiscid-2.0.3/libdiscid/cdiscid.pxd`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/compat/discid.py` & `python-libdiscid-2.0.3/libdiscid/compat/discid.py`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/discid-wrapper.c` & `python-libdiscid-2.0.3/libdiscid/discid-wrapper.c`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/discid-wrapper.h` & `python-libdiscid-2.0.3/libdiscid/discid-wrapper.h`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/exceptions.py` & `python-libdiscid-2.0.3/libdiscid/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/tests/common.py` & `python-libdiscid-2.0.3/libdiscid/tests/common.py`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/tests/test_compat_discid.py` & `python-libdiscid-2.0.3/libdiscid/tests/test_compat_discid.py`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/libdiscid/tests/test_libdiscid.py` & `python-libdiscid-2.0.3/libdiscid/tests/test_libdiscid.py`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/python_libdiscid.egg-info/PKG-INFO` & `python-libdiscid-2.0.3/python_libdiscid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: python-libdiscid
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python bindings for libdiscid
 Home-page: https://github.com/sebastinas/python-libdiscid
 Author: Sebastian Ramacher
 Author-email: sebastian@ramacher.at
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: CD Audio :: CD Ripping
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # libdiscid Python bindings
 
 python-libdiscid implements Python >= 3.6 bindings for libdiscid using Cython.
```

### Comparing `python-libdiscid-2.0.2/python_libdiscid.egg-info/SOURCES.txt` & `python-libdiscid-2.0.3/python_libdiscid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-libdiscid-2.0.2/setup.cfg` & `python-libdiscid-2.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [metadata]
 name = python-libdiscid
-version = 2.0.2
+version = 2.0.3
 author = Sebastian Ramacher
 author_email = sebastian@ramacher.at
 url = https://github.com/sebastinas/python-libdiscid
 description = Python bindings for libdiscid
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Topic :: Multimedia :: Sound/Audio :: CD Audio :: CD Ripping
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 
 [build_sphinx]
 source-dir = docs
 build-dir = build
 all_files = 1
 
 [egg_info]
```

### Comparing `python-libdiscid-2.0.2/setup.py` & `python-libdiscid-2.0.3/setup.py`

 * *Files identical despite different names*

