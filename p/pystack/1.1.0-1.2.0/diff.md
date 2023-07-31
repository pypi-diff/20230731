# Comparing `tmp/pystack-1.1.0.tar.gz` & `tmp/pystack-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystack-1.1.0.tar", last modified: Tue Jul 11 16:38:52 2023, max compression
+gzip compressed data, was "pystack-1.2.0.tar", last modified: Mon Jul 31 18:08:22 2023, max compression
```

## Comparing `pystack-1.1.0.tar` & `pystack-1.2.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.356092 pystack-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 16:38:39.000000 pystack-1.1.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 16:38:39.000000 pystack-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-11 16:38:39.000000 pystack-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-11 16:38:39.000000 pystack-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-11 16:38:39.000000 pystack-1.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-11 16:38:39.000000 pystack-1.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-07-11 16:38:52.356092 pystack-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-07-11 16:38:39.000000 pystack-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-11 16:38:39.000000 pystack-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 16:38:52.356092 pystack-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-11 16:38:39.000000 pystack-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.344092 pystack-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.348092 pystack-1.1.0/src/pystack/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.352092 pystack-1.1.0/src/pystack/_pystack/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/corefile.pxd
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.356092 pystack-1.1.0/src/pystack/_pystack/cpython/
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/code.h
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/dict.h
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/float.h
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/frame.h
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/gc.h
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/int.h
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/interpreter.h
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/list.h
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/object.h
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/pthread.h
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/runtime.h
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/string.h
--rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/thread.h
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/cpython/tuple.h
--rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.h
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/elf_common.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/mem.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/native_frame.h
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/native_frame.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.h
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/process.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.h
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycode.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pycompat.h
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.h
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pyframe.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.h
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pythread.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pytypes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/pytypes.h
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/unwinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/unwinder.h
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/version.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack/version.h
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26996 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_pystack.pyx
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/process.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/traceback_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-11 16:38:39.000000 pystack-1.1.0/src/pystack/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 16:38:52.348092 pystack-1.1.0/src/pystack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 16:38:52.000000 pystack-1.1.0/src/pystack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.744197 pystack-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-31 18:08:10.000000 pystack-1.2.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-31 18:08:10.000000 pystack-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-31 18:08:10.000000 pystack-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-31 18:08:10.000000 pystack-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-07-31 18:08:10.000000 pystack-1.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-31 18:08:10.000000 pystack-1.2.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-31 18:08:22.740197 pystack-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-07-31 18:08:10.000000 pystack-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-31 18:08:10.000000 pystack-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 18:08:22.744197 pystack-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3470 2023-07-31 18:08:10.000000 pystack-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.732197 pystack-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.736197 pystack-1.2.0/src/pystack/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13858 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.740197 pystack-1.2.0/src/pystack/_pystack/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15222 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/corefile.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/corefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/corefile.pxd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.740197 pystack-1.2.0/src/pystack/_pystack/cpython/
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/code.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/dict.h
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/float.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/gc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/int.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/interpreter.h
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/list.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/object.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/pthread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/runtime.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/string.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/thread.h
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/cpython/tuple.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19274 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/elf_common.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/elf_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/elf_common.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/logging.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/mem.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/mem.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/native_frame.h
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/native_frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/process.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/process.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/process.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pycode.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pycode.h
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pycode.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pycompat.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pyframe.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pyframe.h
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pyframe.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    14347 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pythread.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pythread.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pythread.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    21389 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pytypes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/pytypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/unwinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/unwinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10465 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/version.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack/version.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27018 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_pystack.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/traceback_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-31 18:08:10.000000 pystack-1.2.0/src/pystack/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 18:08:22.736197 pystack-1.2.0/src/pystack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13227 2023-07-31 18:08:22.000000 pystack-1.2.0/src/pystack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-31 18:08:22.000000 pystack-1.2.0/src/pystack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 18:08:22.000000 pystack-1.2.0/src/pystack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-31 18:08:22.000000 pystack-1.2.0/src/pystack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 18:08:22.000000 pystack-1.2.0/src/pystack.egg-info/top_level.txt
```

### Comparing `pystack-1.1.0/.pre-commit-config.yaml` & `pystack-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/LICENSE` & `pystack-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/MANIFEST.in` & `pystack-1.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/Makefile` & `pystack-1.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/NEWS.rst` & `pystack-1.2.0/NEWS.rst`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,25 @@
    fix problems like typo corrections or such.
 
 Changelog
 =========
 
 .. towncrier release notes start
 
+pystack 1.2.0 (2023-07-31)
+--------------------------
+
+Features
+~~~~~~~~
+
+- Add support for Python 3.12 (#108)
+- Improve the performance of reading memory from running processes (#124)
+- Improve the performance of reading memory from core files (#126)
+
+
 pystack 1.1.0 (2023-07-10)
 --------------------------
 
 Bug Fixes
 ~~~~~~~~~
 
 - Allow building with older elfutils than 0.188 when building with glibc (for musl libc we still need newer versions). (#40)
```

### Comparing `pystack-1.1.0/PKG-INFO` & `pystack-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pystack
-Version: 1.1.0
+Version: 1.2.0
 Summary: Analysis of the stack of remote python processes
 Home-page: https://github.com/bloomberg/pystack
 Author: Pablo Galindo Salgado
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -66,14 +66,18 @@
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
 - 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
   PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
+## What platforms are supported?
+
+At this time only Linux is supported.
+
 ## Building from source
 
 If you wish to build PyStack from source, you need the following binary dependencies in your
 system:
 
 - libdw
 - libelf
```

### Comparing `pystack-1.1.0/README.md` & `pystack-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
 - 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
   PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
+## What platforms are supported?
+
+At this time only Linux is supported.
+
 ## Building from source
 
 If you wish to build PyStack from source, you need the following binary dependencies in your
 system:
 
 - libdw
 - libelf
```

### Comparing `pystack-1.1.0/pyproject.toml` & `pystack-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/setup.py` & `pystack-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import os
 import pathlib
 import sys
-from distutils.core import setup
+from sys import platform
 
+import setuptools
 from Cython.Build import cythonize
-from setuptools import Extension
+
+IS_LINUX = "linux" in platform
+
+if not IS_LINUX:
+    raise RuntimeError(f"memray does not support this platform ({platform})")
 
 install_requires = []
 
 
 TEST_BUILD = False
 if "--test-build" in sys.argv:
     TEST_BUILD = True
@@ -21,15 +26,14 @@
 
 COMPILER_DIRECTIVES = {
     "language_level": 3,
     "embedsignature": True,
     "boundscheck": False,
     "wraparound": False,
     "cdivision": True,
-    "linetrace": True,
     "c_string_type": "unicode",
     "c_string_encoding": "utf8",
 }
 
 DEFINE_MACROS = []
 
 if TEST_BUILD:
@@ -45,15 +49,15 @@
         "infer_types": True,
         "c_string_type": "unicode",
         "c_string_encoding": "utf8",
     }
     DEFINE_MACROS.extend([("CYTHON_TRACE", "1"), ("CYTHON_TRACE_NOGIL", "1")])
 
 
-PYSTACK_EXTENSION = Extension(
+PYSTACK_EXTENSION = setuptools.Extension(
     name="pystack._pystack",
     sources=[
         "src/pystack/_pystack.pyx",
         "src/pystack/_pystack/corefile.cpp",
         "src/pystack/_pystack/elf_common.cpp",
         "src/pystack/_pystack/logging.cpp",
         "src/pystack/_pystack/mem.cpp",
@@ -79,32 +83,32 @@
 about = {}
 with open("src/pystack/_version.py") as fp:
     exec(fp.read(), about)
 
 HERE = pathlib.Path(__file__).parent.resolve()
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf-8")
 
-setup(
+setuptools.setup(
     name="pystack",
     version=about["__version__"],
     python_requires=">=3.7.0",
     description="Analysis of the stack of remote python processes",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/bloomberg/pystack",
     author="Pablo Galindo Salgado",
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Debuggers",
     ],
     package_dir={"": "src"},
     packages=["pystack"],
     ext_modules=cythonize(
         [PYSTACK_EXTENSION],
```

### Comparing `pystack-1.1.0/src/pystack/__main__.py` & `pystack-1.2.0/src/pystack/__main__.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/CMakeLists.txt` & `pystack-1.2.0/src/pystack/_pystack/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/compat.h` & `pystack-1.2.0/src/pystack/_pystack/compat.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/corefile.cpp` & `pystack-1.2.0/src/pystack/_pystack/corefile.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/corefile.h` & `pystack-1.2.0/src/pystack/_pystack/corefile.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/corefile.pxd` & `pystack-1.2.0/src/pystack/_pystack/corefile.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/code.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/code.h`

 * *Files 16% similar despite different names*

```diff
@@ -121,16 +121,52 @@
     char* _co_linearray;
     int _co_firsttraceable;
     void* co_extra;
     char co_code_adaptive[1];
 } PyCodeObject;
 }  // namespace Python3_11
 
+namespace Python3_12 {
+typedef uint16_t _Py_CODEUNIT;
+typedef struct
+{
+    PyObject_VAR_HEAD PyObject* co_consts;
+    PyObject* co_names;
+    PyObject* co_exceptiontable;
+    int co_flags;
+    int co_argcount;
+    int co_posonlyargcount;
+    int co_kwonlyargcount;
+    int co_stacksize;
+    int co_firstlineno;
+    int co_nlocalsplus;
+    int co_framesize;
+    int co_nlocals;
+    int co_ncellvars;
+    int co_nfreevars;
+    uint32_t co_version;
+    PyObject* co_localsplusnames;
+    PyObject* co_localspluskinds;
+    PyObject* co_filename;
+    PyObject* co_name;
+    PyObject* co_qualname;
+    PyObject* co_linetable;
+    PyObject* co_weakreflist;
+    void* _co_cached;
+    uint64_t _co_instrumentation_version;
+    void* _co_monitoring;
+    int _co_firsttraceable;
+    void* co_extra;
+    char co_code_adaptive[1];
+} PyCodeObject;
+}  // namespace Python3_12
+
 typedef union {
     Python2::PyCodeObject v2;
     Python3_3::PyCodeObject v3_3;
     Python3_6::PyCodeObject v3_6;
     Python3_8::PyCodeObject v3_8;
     Python3_11::PyCodeObject v3_11;
+    Python3_12::PyCodeObject v3_12;
 } PyCodeObject;
 
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/dict.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/dict.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/frame.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/frame.h`

 * *Files 8% similar despite different names*

```diff
@@ -92,24 +92,46 @@
     PyObject* f_func;
     PyObject* f_globals;
     PyObject* f_builtins;
     PyObject* f_locals;
     PyObject* f_code;
     PyObject* frame_obj;
     struct _PyInterpreterFrame* previous;
-    _Py_CODEUNIT* f_lasti;
+    _Py_CODEUNIT* prev_instr;
     int stacktop;
     bool is_entry;
     char owner;
     PyObject* localsplus[1];
 } PyFrameObject;
 
 }  // namespace Python3_11
 
+namespace Python3_12 {
+typedef signed char PyFrameState;
+
+typedef struct _interpreter_frame
+{
+    PyCodeObject* f_code;
+    struct _interpreter_frame* previous;
+    PyObject* f_funcobj;
+    PyObject* f_globals;
+    PyObject* f_builtins;
+    PyObject* f_locals;
+    PyObject* frame_obj;
+    _Py_CODEUNIT* prev_instr;
+    int stacktop;
+    uint16_t return_offset;
+    char owner;
+    PyObject* localsplus[1];
+} PyFrameObject;
+
+}  // namespace Python3_12
+
 typedef union {
     Python2::PyFrameObject v2;
     Python3_7::PyFrameObject v3_7;
     Python3_10::PyFrameObject v3_10;
     Python3_11::PyFrameObject v3_11;
+    Python3_12::PyFrameObject v3_12;
 } PyFrameObject;
 
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/gc.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/gc.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/interpreter.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/interpreter.h`

 * *Files 21% similar despite different names*

```diff
@@ -160,16 +160,100 @@
     PyObject* modules;
     PyObject* modules_by_index;
     PyObject* sysdict;
     PyObject* builtins;
 } PyInterpreterState;
 }  // namespace Python3_11
 
+namespace Python3_12 {
+
+struct _pythreadstate; /* Forward */
+
+struct _pending_calls
+{
+    int busy;
+    PyThread_type_lock lock;
+    _Py_atomic_int calls_to_do;
+    int async_exc;
+    struct _pending_call
+    {
+        int (*func)(void*);
+        void* arg;
+    } calls[32];
+    int first;
+    int last;
+};
+
+struct _ceval_state
+{
+    _Py_atomic_int eval_breaker;
+    _Py_atomic_int gil_drop_request;
+    int recursion_limit;
+    struct _gil_runtime_state* gil;
+    int own_gil;
+    _Py_atomic_int gc_scheduled;
+    struct _pending_calls pending;
+};
+
+struct _import_state
+{
+    PyObject* modules;
+    PyObject* modules_by_index;
+    PyObject* importlib;
+    int override_frozen_modules;
+    int override_multi_interp_extensions_check;
+    int dlopenflags;
+    PyObject* import_func;
+    struct
+    {
+        PyThread_type_lock mutex;
+        unsigned long thread;
+        int level;
+    } lock;
+    struct
+    {
+        int import_level;
+        int64_t accumulated;
+        int header;
+    } find_and_load;
+};
+
+typedef struct _is
+{
+    struct _is* next;
+    int64_t id;
+    int64_t id_refcount;
+    int requires_idref;
+    PyThread_type_lock id_mutex;
+    int _initialized;
+    int finalizing;
+    uint64_t monitoring_version;
+    uint64_t last_restart_version;
+    struct pythreads
+    {
+        uint64_t next_unique_id;
+        _pythreadstate* head;
+        long count;
+        size_t stacksize;
+    } threads;
+    struct pyruntimestate* runtime;
+    uintptr_t _finalizing;
+    struct Python3_8::_gc_runtime_state gc;
+    // Dictionary of the sys module
+    PyObject* sysdict;
+    // Dictionary of the builtins module
+    PyObject* builtins;
+    struct _ceval_state ceval;
+    struct _import_state imports;
+} PyInterpreterState;
+}  // namespace Python3_12
+
 typedef union {
     Python2::PyInterpreterState v2;
     Python3_5::PyInterpreterState v3_5;
     Python3_7::PyInterpreterState v3_7;
     Python3_8::PyInterpreterState v3_8;
     Python3_9::PyInterpreterState v3_9;
     Python3_11::PyInterpreterState v3_11;
+    Python3_12::PyInterpreterState v3_12;
 } PyInterpreterState;
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/object.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/object.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/pthread.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/pthread.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/runtime.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/runtime.h`

 * *Files 5% similar despite different names*

```diff
@@ -222,15 +222,36 @@
     int nexitfuncs;
     struct Python3_9::_ceval_runtime_state ceval;
     struct Python3_9::_gilstate_runtime_state gilstate;
     int gc;  // This is fake, but is here for compatibility
 } PyRuntimeState;
 }  // namespace Python3_11
 
+namespace Python3_12 {
+typedef struct pyruntimestate
+{
+    int _initialized;
+    int preinitializing;
+    int preinitialized;
+    int core_initialized;
+    int initialized;
+    PyThreadState* finalizing;
+
+    struct pyinterpreters
+    {
+        PyThread_type_lock mutex;
+        PyInterpreterState* head;
+        PyInterpreterState* main;
+        int64_t next_id;
+    } interpreters;
+} PyRuntimeState;
+}  // namespace Python3_12
+
 typedef union {
     Python3_7::PyRuntimeState v3_7;
     Python3_8::PyRuntimeState v3_8;
     Python3_9::PyRuntimeState v3_9;
-    Python3_9::PyRuntimeState v3_11;
+    Python3_11::PyRuntimeState v3_11;
+    Python3_12::PyRuntimeState v3_12;
 } PyRuntimeState;
 
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/string.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/string.h`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,39 @@
 typedef uint8_t Py_UCS1;
 
 typedef Py_UCS4 Py_UNICODE;
 typedef Py_ssize_t Py_hash_t;
 
 typedef struct
 {
+    PyObject_VAR_HEAD Py_hash_t ob_shash;
+    char ob_sval[1];
+} PyBytesObject;
+
+namespace Python2 {
+typedef struct
+{
+    PyObject_HEAD Py_ssize_t length;
+    Py_UNICODE* str;
+    long hash;
+    PyObject* defenc;
+} PyUnicodeObject;
+
+typedef struct
+{
+    PyObject_VAR_HEAD long ob_shash;
+    int ob_sstate;
+    char ob_sval[1];
+} _PyStringObject;
+}  // namespace Python2
+
+namespace Python3 {
+
+typedef struct
+{
     PyObject_HEAD Py_ssize_t length;
     Py_hash_t hash;
     struct
     {
         unsigned int interned : 2;
         unsigned int kind : 3;
         unsigned int compact : 1;
@@ -34,47 +59,61 @@
     Py_ssize_t utf8_length;
     char* utf8;
     Py_ssize_t wstr_length;
 } PyCompactUnicodeObject;
 
 typedef struct
 {
-    PyObject_VAR_HEAD Py_hash_t ob_shash;
-    char ob_sval[1];
-} PyBytesObject;
+    PyCompactUnicodeObject _base;
+    union {
+        void* any;
+        Py_UCS1* latin1;
+        Py_UCS2* ucs2;
+        Py_UCS4* ucs4;
+    } data;
+} PyUnicodeObject;
+
+}  // namespace Python3
+
+namespace Python3_12 {
 
-namespace Python2 {
 typedef struct
 {
     PyObject_HEAD Py_ssize_t length;
-    Py_UNICODE* str;
-    long hash;
-    PyObject* defenc;
-} PyUnicodeObject;
+    Py_hash_t hash;
+    struct
+    {
+        unsigned int interned : 2;
+        unsigned int kind : 3;
+        unsigned int compact : 1;
+        unsigned int ascii : 1;
+        unsigned int ready : 1;
+        unsigned int : 24;
+    } state;
+} PyASCIIObject;
 
 typedef struct
 {
-    PyObject_VAR_HEAD long ob_shash;
-    int ob_sstate;
-    char ob_sval[1];
-} _PyStringObject;
-}  // namespace Python2
+    PyASCIIObject _base;
+    Py_ssize_t utf8_length;
+    char* utf8;
+} PyCompactUnicodeObject;
 
-namespace Python3 {
 typedef struct
 {
-    PyCompactUnicodeObject _base;
     union {
         void* any;
         Py_UCS1* latin1;
         Py_UCS2* ucs2;
         Py_UCS4* ucs4;
     } data;
 } PyUnicodeObject;
-}  // namespace Python3
+
+}  // namespace Python3_12
 
 typedef union {
     Python2::PyUnicodeObject v2;
     Python3::PyUnicodeObject v3;
+    Python3_12::PyUnicodeObject v3_12;
 } PyUnicodeObject;
 
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/cpython/thread.h` & `pystack-1.2.0/src/pystack/_pystack/cpython/thread.h`

 * *Files 26% similar despite different names*

```diff
@@ -158,15 +158,92 @@
     int gilstate_counter;
     PyObject* async_exc;
     unsigned long thread_id;
     unsigned long native_thread_id;
 } PyThreadState;
 }  // namespace Python3_11
 
+namespace Python3_12 {
+typedef struct _err_stackitem
+{
+    PyObject* exc_value;
+    struct _err_stackitem* previous_item;
+} _PyErr_StackItem;
+
+typedef struct _cframe
+{
+    struct _interpreter_frame* current_frame;
+    struct _cframe* previous;
+} CFrame;
+
+struct _py_trashcan
+{
+    int delete_nesting;
+    PyObject* delete_later;
+};
+
+typedef struct _pythreadstate
+{
+    struct _pythreadstate* prev;
+    struct _pythreadstate* next;
+    struct _is* interp;
+    struct
+    {
+        unsigned int initialized : 1;
+        unsigned int bound : 1;
+        unsigned int unbound : 1;
+        unsigned int bound_gilstate : 1;
+        unsigned int active : 1;
+        unsigned int finalizing : 1;
+        unsigned int cleared : 1;
+        unsigned int finalized : 1;
+        unsigned int : 24;
+    } _status;
+    int py_recursion_remaining;
+    int py_recursion_limit;
+    int c_recursion_remaining;
+    int recursion_headroom;
+    int tracing;
+    int what_event;
+    CFrame* cframe;
+    Py_tracefunc c_profilefunc;
+    Py_tracefunc c_tracefunc;
+    PyObject* c_profileobj;
+    PyObject* c_traceobj;
+    PyObject* current_exception;
+    _PyErr_StackItem* exc_info;
+    PyObject* dict;
+    int gilstate_counter;
+    PyObject* async_exc;
+    unsigned long thread_id;
+    unsigned long native_thread_id;
+    struct _py_trashcan trash;
+    void (*on_delete)(void*);
+    void* on_delete_data;
+    int coroutine_origin_tracking_depth;
+    PyObject* async_gen_firstiter;
+    PyObject* async_gen_finalizer;
+    PyObject* context;
+    uint64_t context_ver;
+    uint64_t id;
+    void* datastack_chunk;
+    PyObject** datastack_top;
+    PyObject** datastack_limit;
+    _PyErr_StackItem exc_state;
+    CFrame root_cframe;
+} PyThreadState;
+}  // namespace Python3_12
+
 typedef union {
     Python2::PyThreadState v2;
     Python3_4::PyThreadState v3_4;
     Python3_7::PyThreadState v3_7;
     Python3_11::PyThreadState v3_11;
+    Python3_12::PyThreadState v3_12;
 } PyThreadState;
 
+union CFrame {
+    Python3_11::CFrame v3_11;
+    Python3_12::CFrame v3_12;
+};
+
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/elf_common.cpp` & `pystack-1.2.0/src/pystack/_pystack/elf_common.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/elf_common.h` & `pystack-1.2.0/src/pystack/_pystack/elf_common.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/elf_common.pxd` & `pystack-1.2.0/src/pystack/_pystack/elf_common.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/logging.cpp` & `pystack-1.2.0/src/pystack/_pystack/logging.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/logging.h` & `pystack-1.2.0/src/pystack/_pystack/logging.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/mem.cpp` & `pystack-1.2.0/src/pystack/_pystack/mem.cpp`

 * *Files 23% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         unsigned long riovcnt,
         unsigned long flags)
 {
     return syscall(SYS_process_vm_readv, pid, lvec, liovcnt, rvec, riovcnt, flags);
 }
 
 static const std::string PERM_MESSAGE = "Operation not permitted";
+static const size_t CACHE_CAPACITY = 5e+7;  // 50MB
 
 VirtualMap::VirtualMap(
         uintptr_t start,
         uintptr_t end,
         unsigned long filesize,
         std::string flags,
         unsigned long offset,
@@ -151,58 +152,157 @@
 
 void
 MemoryMapInformation::setHeap(const VirtualMap& heap)
 {
     d_heap = heap;
 }
 
+LRUCache::LRUCache(size_t capacity)
+: d_cache_capacity(capacity)
+, d_size(0){};
+
+void
+LRUCache::put(uintptr_t key, std::vector<char>&& value)
+{
+    size_t value_size = value.size();
+
+    if (!can_fit(value_size)) {
+        return;
+    }
+
+    auto it = d_cache.find(key);
+
+    if (it != d_cache.end()) {
+        d_cache_list.erase(it->second.it);
+        d_cache.erase(it);
+    }
+
+    while (d_size + value_size > d_cache_capacity) {
+        d_cache.erase(d_cache_list.back().key);
+        d_size -= d_cache_list.back().size;
+        d_cache_list.pop_back();
+    }
+
+    d_cache_list.push_front(LRUCache::ListNode{key, value_size});
+    d_cache[key] = LRUCache::CacheValue{std::move(value), d_cache_list.begin()};
+    d_size += value_size;
+}
+
+const std::vector<char>&
+LRUCache::get(uintptr_t key)
+{
+    auto it = d_cache.find(key);
+    if (it == d_cache.end()) {
+        throw std::range_error("There is no such key in the cache");
+    } else {
+        auto node_it = it->second.it;
+        d_cache_list.splice(d_cache_list.begin(), d_cache_list, node_it);
+        return it->second.data;
+    }
+}
+
+bool
+LRUCache::exists(uintptr_t key)
+{
+    return (d_cache.find(key) != d_cache.end());
+}
+
+bool
+LRUCache::can_fit(size_t size)
+{
+    return d_cache_capacity >= size;
+}
+
+ProcessMemoryManager::ProcessMemoryManager(pid_t pid, const std::vector<VirtualMap>& vmaps)
+: d_pid(pid)
+, d_vmaps(vmaps)
+, d_lru_cache(CACHE_CAPACITY)
+{
+}
+
 ProcessMemoryManager::ProcessMemoryManager(pid_t pid)
-: d_pid(pid){};
+: d_pid(pid)
+, d_lru_cache(CACHE_CAPACITY)
+{
+}
 
 ssize_t
-ProcessMemoryManager::copyMemoryFromProcess(remote_addr_t addr, size_t len, void* buf) const
+ProcessMemoryManager::readChunk(remote_addr_t addr, size_t len, char* dst) const
 {
     struct iovec local[1];
     struct iovec remote[1];
+    ssize_t result = 0;
+    ssize_t read = 0;
 
-    local[0].iov_base = buf;
-    local[0].iov_len = len;
-    remote[0].iov_base = (void*)addr;
-    remote[0].iov_len = len;
-
-    ssize_t result = _process_vm_readv(d_pid, local, 1, remote, 1, 0);
-    if (result < 0) {
-        if (errno == EFAULT) {
-            throw InvalidRemoteAddress();
-        } else if (errno == EPERM) {
-            throw std::runtime_error(PERM_MESSAGE);
+    do {
+        local[0].iov_base = dst + result;
+        local[0].iov_len = len - result;
+        remote[0].iov_base = reinterpret_cast<uint8_t*>(addr) + result;
+        remote[0].iov_len = len - result;
+
+        read = _process_vm_readv(d_pid, local, 1, remote, 1, 0);
+        if (read < 0) {
+            if (errno == EFAULT) {
+                throw InvalidRemoteAddress();
+            } else if (errno == EPERM) {
+                throw std::runtime_error(PERM_MESSAGE);
+            }
+            throw std::system_error(errno, std::generic_category());
         }
-        throw std::system_error(errno, std::generic_category());
+
+        result += read;
+    } while ((size_t)read != local[0].iov_len);
+
+    return result;
+}
+
+ssize_t
+ProcessMemoryManager::copyMemoryFromProcess(remote_addr_t addr, size_t len, void* dst) const
+{
+    auto vmap = std::find_if(d_vmaps.begin(), d_vmaps.end(), [&](const auto& vmap) {
+        return vmap.containsAddr(addr) && vmap.containsAddr(addr + len - 1);
+    });
+
+    if (vmap == d_vmaps.end() || !d_lru_cache.can_fit(vmap->Size())) {
+        return readChunk(addr, len, reinterpret_cast<char*>(dst));
     }
 
-    if ((size_t)result != len) {
-        throw InvalidCopiedMemory();
+    uintptr_t key = vmap->Start();
+    size_t chunk_size = vmap->Size();
+    remote_addr_t vmap_start_addr = vmap->Start();
+    size_t offset_addr = addr - vmap_start_addr;
+
+    if (!d_lru_cache.exists(key)) {
+        std::vector<char> buf(chunk_size);
+        readChunk(vmap_start_addr, chunk_size, buf.data());
+        d_lru_cache.put(key, std::move(buf));
     }
-    return result;
+
+    std::memcpy(dst, d_lru_cache.get(key).data() + offset_addr, len);
+
+    return len;
 }
 
 bool
 ProcessMemoryManager::isAddressValid(remote_addr_t addr, const VirtualMap& map) const
 {
     if (addr == (uintptr_t) nullptr) {
         return false;
     }
     return map.Start() <= addr && addr < map.End();
 }
 
-BlockingProcessMemoryManager::BlockingProcessMemoryManager(pid_t pid, const std::vector<int>& tids)
-: ProcessMemoryManager(pid)
+BlockingProcessMemoryManager::BlockingProcessMemoryManager(
+        pid_t pid,
+        const std::vector<int>& tids,
+        const std::vector<VirtualMap>& vmaps)
+: ProcessMemoryManager(pid, vmaps)
 , d_tids(tids)
 {
-    for (auto& tid : tids) {
+    for (auto& tid : d_tids) {
         LOG(INFO) << "Trying to stop thread " << tid;
         long ret = ptrace(PTRACE_ATTACH, tid, nullptr, nullptr);
         if (ret < 0) {
             int error = errno;
             detachFromProcess();
             if (error == EPERM) {
                 throw std::runtime_error(PERM_MESSAGE);
@@ -240,31 +340,97 @@
         std::shared_ptr<CoreFileAnalyzer> analyzer,
         std::vector<VirtualMap>& vmaps)
 : d_analyzer(std::move(analyzer))
 , d_vmaps(vmaps)
 {
     CoreFileExtractor extractor{d_analyzer};
     d_shared_libs = extractor.ModuleInformation();
+
+    const char* filename = d_analyzer->d_filename.c_str();
+    int fd = open(filename, O_RDONLY);
+
+    if (fd == -1) {
+        LOG(ERROR) << "Failed to open a file " << filename;
+        throw RemoteMemCopyError();
+    }
+
+    StatusCode ret = readCorefile(fd, filename);
+    int close_ret = close(fd);
+
+    if (close_ret == -1) {
+        LOG(ERROR) << "Failed to close a file " << filename;
+        throw RemoteMemCopyError();
+    }
+
+    if (ret == StatusCode::ERROR) {
+        throw RemoteMemCopyError();
+    }
+}
+
+CorefileRemoteMemoryManager::StatusCode
+CorefileRemoteMemoryManager::readCorefile(int fd, const char* filename) noexcept
+{
+    struct stat fileInfo = {0};
+
+    if (fstat(fd, &fileInfo) == -1) {
+        LOG(ERROR) << "Failed to get a file size for a file " << filename;
+        return StatusCode::ERROR;
+    }
+
+    if (fileInfo.st_size == 0) {
+        LOG(ERROR) << "File " << filename << " is empty";
+        return StatusCode::ERROR;
+    }
+
+    d_corefile_size = fileInfo.st_size;
+
+    void* map = mmap(0, d_corefile_size, PROT_READ, MAP_PRIVATE, fd, 0);
+    if (map == MAP_FAILED) {
+        LOG(ERROR) << "Failed to mmap a file " << filename;
+        return StatusCode::ERROR;
+    }
+
+    d_corefile_data = std::unique_ptr<char, std::function<void(char*)>>(
+            reinterpret_cast<char*>(map),
+            [this](auto addr) {
+                if (munmap(addr, d_corefile_size) == -1) {
+                    LOG(ERROR) << "Failed to un-mmap a file " << d_analyzer->d_filename.c_str();
+                }
+            });
+
+    int madvise_result = madvise(d_corefile_data.get(), d_corefile_size, MADV_RANDOM);
+
+    if (madvise_result == -1) {
+        LOG(WARNING) << "Madvise for a file " << filename << " failed";
+    }
+
+    return StatusCode::SUCCESS;
 }
 
 ssize_t
 CorefileRemoteMemoryManager::copyMemoryFromProcess(remote_addr_t addr, size_t size, void* destination)
         const
 {
-    const std::string* filename = nullptr;
     off_t offset_in_file = 0;
 
-    StatusCode ret = getMemoryLocationFromCore(addr, &filename, &offset_in_file);
+    StatusCode ret = getMemoryLocationFromCore(addr, &offset_in_file);
 
-    if (ret == StatusCode::ERROR) {
-        // The memory may be in the data segment of some shared library
-        getMemoryLocationFromElf(addr, &filename, &offset_in_file);
+    if (ret == StatusCode::SUCCESS) {
+        if (static_cast<size_t>(offset_in_file) > d_corefile_size) {
+            throw InvalidRemoteAddress();
+        }
+        memcpy(destination, d_corefile_data.get() + offset_in_file, size);
+        return size;
     }
 
-    if (filename == nullptr) {
+    // The memory may be in the data segment of some shared library
+    const std::string* filename = nullptr;
+    ret = getMemoryLocationFromElf(addr, &filename, &offset_in_file);
+
+    if (ret == StatusCode::ERROR) {
         throw InvalidRemoteAddress();
     }
 
     std::ifstream is(*filename, std::ifstream::binary);
     if (is) {
         is.seekg(offset_in_file);
         is.read((char*)destination, size);
@@ -272,28 +438,25 @@
         LOG(ERROR) << "Failed to read memory from file " << *filename;
         throw InvalidRemoteAddress();
     }
     return size;
 }
 
 CorefileRemoteMemoryManager::StatusCode
-CorefileRemoteMemoryManager::getMemoryLocationFromCore(
-        remote_addr_t addr,
-        const std::string** filename,
-        off_t* offset_in_file) const
+CorefileRemoteMemoryManager::getMemoryLocationFromCore(remote_addr_t addr, off_t* offset_in_file) const
 {
     auto corefile_it = std::find_if(d_vmaps.cbegin(), d_vmaps.cend(), [&](auto& map) {
         return (map.Start() <= addr && addr <= map.End()) && (map.FileSize() != 0 && map.Offset() != 0);
     });
     if (corefile_it == d_vmaps.cend()) {
         return StatusCode::ERROR;
     }
+
     unsigned long base = corefile_it->Offset() - corefile_it->Start();
     *offset_in_file = base + addr;
-    *filename = &d_analyzer->d_filename;
     return StatusCode::SUCCESS;
 }
 
 CorefileRemoteMemoryManager::StatusCode
 CorefileRemoteMemoryManager::getMemoryLocationFromElf(
         remote_addr_t addr,
         const std::string** filename,
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/mem.h` & `pystack-1.2.0/src/pystack/_pystack/mem.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 #pragma once
 
 #include <cstdint>
+#include <fcntl.h>
+#include <functional>
+#include <list>
 #include <memory>
 #include <optional>
 #include <stdexcept>
 #include <string>
+#include <sys/mman.h>
+#include <sys/stat.h>
 #include <vector>
 
 #include <elf_common.h>
 
 namespace pystack {
 typedef uintptr_t remote_addr_t;
 
@@ -105,49 +110,87 @@
   private:
     // Data members
     std::optional<VirtualMap> d_main_map;
     std::optional<VirtualMap> d_bss;
     std::optional<VirtualMap> d_heap;
 };
 
+class LRUCache
+{
+  private:
+    struct ListNode
+    {
+        uintptr_t key;
+        size_t size;
+    };
+
+    struct CacheValue
+    {
+        std::vector<char> data;
+        std::list<ListNode>::iterator it;
+    };
+
+  public:
+    explicit LRUCache(size_t cache_capacity);
+
+    void put(uintptr_t key, std::vector<char>&& value);
+    const std::vector<char>& get(uintptr_t key);
+    bool exists(uintptr_t key);
+    bool can_fit(size_t size);
+
+  private:
+    std::list<ListNode> d_cache_list;
+    std::unordered_map<uintptr_t, CacheValue> d_cache;
+    size_t d_cache_capacity;
+    size_t d_size;
+};
+
 class AbstractRemoteMemoryManager
 {
   public:
     // Constructors
     explicit AbstractRemoteMemoryManager() = default;
 
     // Destructors
     virtual ~AbstractRemoteMemoryManager() = default;
 
     // Methods
     virtual ssize_t copyMemoryFromProcess(remote_addr_t addr, size_t size, void* destination) const = 0;
-
     virtual bool isAddressValid(remote_addr_t addr, const VirtualMap& map) const = 0;
 };
 
 class ProcessMemoryManager : public AbstractRemoteMemoryManager
 {
     // Constructors
   public:
     explicit ProcessMemoryManager(pid_t pid);
+    explicit ProcessMemoryManager(pid_t pid, const std::vector<VirtualMap>& vmaps);
 
     // Methods
-    ssize_t copyMemoryFromProcess(remote_addr_t addr, size_t size, void* destination) const override;
+    ssize_t copyMemoryFromProcess(remote_addr_t addr, size_t size, void* dst) const override;
     bool isAddressValid(remote_addr_t addr, const VirtualMap& map) const override;
 
   private:
     // Data members
     pid_t d_pid;
+    std::vector<VirtualMap> d_vmaps;
+    mutable LRUCache d_lru_cache;
+
+    // Methods
+    ssize_t readChunk(remote_addr_t addr, size_t len, char* dst) const;
 };
 
 class BlockingProcessMemoryManager : public ProcessMemoryManager
 {
   public:
     // Constructors
-    explicit BlockingProcessMemoryManager(pid_t pid, const std::vector<int>& tids);
+    explicit BlockingProcessMemoryManager(
+            pid_t pid,
+            const std::vector<int>& tids,
+            const std::vector<VirtualMap>& vmaps);
 
     // Destructors
     ~BlockingProcessMemoryManager() override;
 
   private:
     // Data members
     std::vector<int> d_tids;
@@ -184,18 +227,18 @@
         ERROR,
     };
 
     // Data members
     std::shared_ptr<CoreFileAnalyzer> d_analyzer;
     std::vector<VirtualMap> d_vmaps;
     std::vector<SimpleVirtualMap> d_shared_libs;
+    size_t d_corefile_size;
+    std::unique_ptr<char, std::function<void(char*)>> d_corefile_data;
 
-    StatusCode getMemoryLocationFromCore(
-            remote_addr_t addr,
-            const std::string** filename,
-            off_t* offset_in_file) const;
+    StatusCode readCorefile(int fd, const char* filename) noexcept;
+    StatusCode getMemoryLocationFromCore(remote_addr_t addr, off_t* offset_in_file) const;
     StatusCode getMemoryLocationFromElf(
             remote_addr_t addr,
             const std::string** filename,
             off_t* offset_in_file) const;
 };
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/mem.pxd` & `pystack-1.2.0/src/pystack/_pystack/mem.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/process.cpp` & `pystack-1.2.0/src/pystack/_pystack/process.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -143,16 +143,15 @@
       - As a last security check: try to construct a single frame and the
     associated code object from the executing thread and check that the results
     make sense. We need to do this because, although very rare, there may be some
     random memory regions that have the previous properties but they are still
     garbage.
 
     If any of the previous steps fail, we continue with the next memory chunk
-    until we found the PyInterpreterState or we run our of chunks.
-
+    until we find the PyInterpreterState or we run out of chunks.
     */
     if (!isAddressValid(addr)) {
         return false;
     }
 
     PyInterpreterState is;
     // The check for valid addresses may fail if the address falls in the stack
@@ -162,38 +161,37 @@
     try {
         copyObjectFromProcess(addr, &is);
     } catch (RemoteMemCopyError& ex) {
         return false;
     }
 
     PyThreadState current_thread;
-    auto current_thread_addr =
-            versionedInterpreterStateField<remote_addr_t, &py_is_v::o_tstate_head>(is);
+    auto current_thread_addr = getField(is, &py_is_v::o_tstate_head);
     if (!isAddressValid(current_thread_addr)) {
         return false;
     }
 
     try {
         copyObjectFromProcess(current_thread_addr, &current_thread);
     } catch (RemoteMemCopyError& ex) {
         return false;
     }
 
-    if (versionedThreadField<remote_addr_t, &py_thread_v::o_interp>(current_thread) != addr) {
+    if (getField(current_thread, &py_thread_v::o_interp) != addr) {
         return false;
     }
 
     LOG(DEBUG) << std::hex << std::showbase << "Possible PyInterpreterState candidate at address "
                << addr << " with tstate_head value of " << current_thread_addr;
 
     // Validate dictionaries in the interpreter state
     std::unordered_map<std::string, remote_addr_t> dictionaries(
-            {{"modules", versionedInterpreterStateField<remote_addr_t, &py_is_v::o_modules>(is)},
-             {"sysdict", versionedInterpreterStateField<remote_addr_t, &py_is_v::o_sysdict>(is)},
-             {"builtins", versionedInterpreterStateField<remote_addr_t, &py_is_v::o_builtins>(is)}});
+            {{"modules", getField(is, &py_is_v::o_modules)},
+             {"sysdict", getField(is, &py_is_v::o_sysdict)},
+             {"builtins", getField(is, &py_is_v::o_builtins)}});
     for (const auto& [dictname, addr] : dictionaries) {
         if (!isValidDictionaryObject(addr)) {
             LOG(DEBUG) << "The '" << dictname << "' dictionary object is not valid";
             return false;
         }
         LOG(DEBUG) << "The '" << dictname << "' dictionary object is valid";
     }
@@ -223,16 +221,15 @@
 AbstractProcessManager::findInterpreterStateFromPyRuntime(remote_addr_t runtime_addr) const
 {
     LOG(INFO) << "Searching for PyInterpreterState based on PyRuntime address " << std::hex
               << std::showbase << runtime_addr;
 
     PyRuntimeState py_runtime;
     copyObjectFromProcess(runtime_addr, &py_runtime);
-    remote_addr_t interp_state =
-            versionedRuntimeField<remote_addr_t, &py_runtime_v::o_interp_head>(py_runtime);
+    remote_addr_t interp_state = getField(py_runtime, &py_runtime_v::o_interp_head);
 
     if (!isValidInterpreterState(interp_state)) {
         LOG(INFO) << "Failing to resolve PyInterpreterState based on PyRuntime address " << std::hex
                   << std::showbase << runtime_addr;
         return (remote_addr_t)NULL;
     }
 
@@ -358,15 +355,22 @@
         }
         if (unicode._base._base.state.compact != 1u) {
             throw InvalidRemoteObject();
         }
         len = unicode._base._base.length;
         buffer.resize(len);
 
-        data_addr = ((remote_addr_t)((char*)addr + sizeof(PyASCIIObject)));
+        size_t offset;
+        if (d_major > 3 || (d_major == 3 && d_minor >= 12)) {
+            offset = sizeof(Python3_12::PyASCIIObject);
+        } else {
+            offset = sizeof(Python3::PyASCIIObject);
+        }
+
+        data_addr = ((remote_addr_t)((char*)addr + offset));
         LOG(DEBUG) << std::hex << std::showbase << "Copying ASCII data for unicode object from address "
                    << data_addr;
         copyMemoryFromProcess(data_addr, len, buffer.data());
     }
     return std::string(buffer.begin(), buffer.end());
 }
 
@@ -466,15 +470,15 @@
 AbstractProcessManager::InterpreterStatus
 AbstractProcessManager::isInterpreterActive() const
 {
     remote_addr_t runtime_addr = findSymbol("_PyRuntime");
     if (runtime_addr) {
         PyRuntimeState py_runtime;
         copyObjectFromProcess(runtime_addr, &py_runtime);
-        remote_addr_t p = versionedRuntimeField<remote_addr_t, &py_runtime_v::o_finalizing>(py_runtime);
+        remote_addr_t p = getField(py_runtime, &py_runtime_v::o_finalizing);
         return p == 0 ? InterpreterStatus::RUNNING : InterpreterStatus::FINALIZED;
     }
 
     return InterpreterStatus::UNKNOWN;
 }
 
 std::pair<int, int>
@@ -498,24 +502,18 @@
 {
     d_py_v = getCPythonOffsets(version.first, version.second);
     // Note: getCPythonOffsets can throw. Don't set these if it does.
     d_major = version.first;
     d_minor = version.second;
 }
 
-int
-AbstractProcessManager::majorVersion() const
-{
-    return d_major;
-}
-
-int
-AbstractProcessManager::minorVersion() const
+bool
+AbstractProcessManager::versionIsAtLeast(int required_major, int required_minor) const
 {
-    return d_minor;
+    return d_major > required_major || (d_major == required_major && d_minor >= required_minor);
 }
 
 const python_v&
 AbstractProcessManager::offsets() const
 {
     return *d_py_v;
 }
@@ -545,17 +543,17 @@
         const std::shared_ptr<ProcessAnalyzer>& analyzer,
         std::vector<VirtualMap> memory_maps,
         MemoryMapInformation map_info)
 : AbstractProcessManager(pid, std::move(memory_maps), std::move(map_info))
 , d_tids(getProcessTids(pid))
 {
     if (blocking) {
-        d_manager = std::make_unique<BlockingProcessMemoryManager>(pid, d_tids);
+        d_manager = std::make_unique<BlockingProcessMemoryManager>(pid, d_tids, d_memory_maps);
     } else {
-        d_manager = std::make_unique<ProcessMemoryManager>(pid);
+        d_manager = std::make_unique<ProcessMemoryManager>(pid, d_memory_maps);
     }
     d_analyzer = analyzer;
     d_unwinder = std::make_unique<Unwinder>(analyzer);
 }
 
 const std::vector<int>&
 ProcessManager::Tids() const
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/process.h` & `pystack-1.2.0/src/pystack/_pystack/process.h`

 * *Files 24% similar despite different names*

```diff
@@ -60,71 +60,30 @@
     remote_addr_t scanAllAnonymousMaps() const;
     remote_addr_t scanBSS() const;
     remote_addr_t scanHeap() const;
     InterpreterStatus isInterpreterActive() const;
     std::pair<int, int> findPythonVersion() const;
 
     void setPythonVersion(const std::pair<int, int>& version);
-    int majorVersion() const;
-    int minorVersion() const;
+    bool versionIsAtLeast(int required_major, int required_minor) const;
     const python_v& offsets() const;
 
-    template<typename T, typename U, auto PMD0, auto PMD1>
-    inline auto& versionedField(const U& py_obj) const
+    template<typename OffsetsStruct, typename FieldPointer>
+    inline offset_t getFieldOffset(FieldPointer OffsetsStruct::*field) const
     {
-        offset_t offset = d_py_v->*PMD0.*PMD1;
-        return (*((T*)(((char*)&py_obj) + offset)));
+        return (d_py_v->get<OffsetsStruct>().*field).offset;
     }
 
-    template<typename T, auto PMD1>
-    inline auto& versionedThreadField(const PyThreadState& py_thread) const
+    template<typename OffsetsStruct, typename FieldPointer>
+    inline const typename FieldPointer::Type&
+    getField(const typename OffsetsStruct::Structure& obj, FieldPointer OffsetsStruct::*field) const
     {
-        return versionedField<T, PyThreadState, &python_v::py_thread, PMD1>(py_thread);
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedInterpreterStateField(const PyInterpreterState& py_is) const
-    {
-        return versionedField<T, PyInterpreterState, &python_v::py_is, PMD1>(py_is);
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedGcStatesField(const GCRuntimeState& py_gc) const
-    {
-        return versionedField<T, GCRuntimeState, &python_v::py_gc, PMD1>(py_gc);
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedFrameField(const PyFrameObject& py_frame) const
-    {
-        return versionedField<T, PyFrameObject, &python_v::py_frame, PMD1>(py_frame);
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedCodeField(const PyCodeObject& py_code) const
-    {
-        return versionedField<T, PyCodeObject, &python_v::py_code, PMD1>(py_code);
-    }
-
-    template<auto PMD1>
-    inline auto versionedCodeOffset() const
-    {
-        return d_py_v->py_code.*PMD1;
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedRuntimeField(const PyRuntimeState& py_runtime) const
-    {
-        return versionedField<T, PyRuntimeState, &python_v::py_runtime, PMD1>(py_runtime);
-    }
-
-    template<typename T, auto PMD1>
-    inline auto& versionedTypeField(const PyTypeObject& py_type) const
-    {
-        return versionedField<T, PyTypeObject, &python_v::py_type, PMD1>(py_type);
+        offset_t offset = getFieldOffset(field);
+        auto address = reinterpret_cast<const char*>(&obj) + offset;
+        return *reinterpret_cast<const typename FieldPointer::Type*>(address);
     }
 
   protected:
     // Data members
     pid_t d_pid;
     std::optional<VirtualMap> d_main_map{std::nullopt};
     std::optional<VirtualMap> d_bss{std::nullopt};
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/process.pxd` & `pystack-1.2.0/src/pystack/_pystack/process.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/pycode.cpp` & `pystack-1.2.0/src/pystack/_pystack/pycode.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -103,44 +103,40 @@
 static LocationInfo
 getLocationInfo(
         const std::shared_ptr<const AbstractProcessManager>& manager,
         remote_addr_t code_addr,
         PyCodeObject& code,
         uintptr_t last_instruction_index)
 {
-    int code_lineno = manager->versionedCodeField<unsigned int, &py_code_v::o_firstlineno>(code);
-    remote_addr_t lnotab_addr = *(remote_addr_t*)((char*)&code + manager->offsets().py_code.o_lnotab);
+    int code_lineno = manager->getField(code, &py_code_v::o_firstlineno);
+    remote_addr_t lnotab_addr = manager->getField(code, &py_code_v::o_lnotab);
     LOG(DEBUG) << std::hex << std::showbase << "Copying lnotab data from address " << lnotab_addr;
     std::string lnotab = manager->getBytesFromAddress(lnotab_addr);
 
-    assert(manager->majorVersion() > 3 || manager->minorVersion() >= 11 || lnotab.size() % 2 == 0);
+    assert(manager->versionIsAtLeast(3, 11) || lnotab.size() % 2 == 0);
     std::string::size_type last_executed_instruction = last_instruction_index;
 
     LocationInfo location_info = LocationInfo{0, 0, 0, 0};
 
     // Check out https://github.com/python/cpython/blob/main/Objects/lnotab_notes.txt for the format of
     // the lnotab table in different versions of the interpreter.
-    if (manager->majorVersion() > 3 || (manager->majorVersion() == 3 && manager->minorVersion() >= 11)) {
-        uintptr_t code_adaptive =
-                code_addr + manager->versionedCodeOffset<&py_code_v::o_code_adaptive>();
+    if (manager->versionIsAtLeast(3, 11)) {
+        uintptr_t code_adaptive = code_addr + manager->getFieldOffset(&py_code_v::o_code_adaptive);
         ptrdiff_t addrq =
                 (reinterpret_cast<uint16_t*>(last_instruction_index)
                  - reinterpret_cast<uint16_t*>(code_adaptive));
         LocationInfo posinfo;
         bool ret = parse_linetable(addrq, lnotab, code_lineno, &posinfo);
         if (ret) {
             location_info.lineno = posinfo.lineno;
             location_info.end_lineno = posinfo.end_lineno;
             location_info.column = posinfo.column;
             location_info.end_column = posinfo.end_column;
         }
-    } else if (
-            manager->majorVersion() > 3
-            || (manager->majorVersion() == 3 && manager->minorVersion() == 10))
-    {
+    } else if (manager->versionIsAtLeast(3, 10)) {
         // Word-code is two bytes, so the actual limit in the table 2 * the instruction index
         last_executed_instruction <<= 1;
         for (std::string::size_type i = 0, current_instruction = 0; i < lnotab.size();) {
             unsigned char start_delta = lnotab[i++];
             signed char line_delta = lnotab[i++];
             current_instruction += start_delta;
             code_lineno += (line_delta == NO_LINE_NUMBER) ? 0 : line_delta;
@@ -170,39 +166,37 @@
         remote_addr_t addr,
         uintptr_t lasti)
 {
     PyCodeObject code;
     LOG(DEBUG) << std::hex << std::showbase << "Copying code struct from address " << addr;
     manager->copyMemoryFromProcess(addr, manager->offsets().py_code.size, &code);
 
-    remote_addr_t filename_addr =
-            *(remote_addr_t*)((char*)&code + manager->offsets().py_code.o_filename);
+    remote_addr_t filename_addr = manager->getField(code, &py_code_v::o_filename);
     LOG(DEBUG) << std::hex << std::showbase << "Copying filename Python string from address "
                << filename_addr;
     d_filename = manager->getStringFromAddress(filename_addr);
     LOG(DEBUG) << "Code object filename: " << d_filename;
 
-    remote_addr_t name_addr = *(remote_addr_t*)((char*)&code + manager->offsets().py_code.o_name);
+    remote_addr_t name_addr = manager->getField(code, &py_code_v::o_name);
     LOG(DEBUG) << std::hex << std::showbase << "Copying code name Python string from address "
                << name_addr;
     d_scope = manager->getStringFromAddress(name_addr);
     LOG(DEBUG) << "Code object scope: " << d_filename;
 
     LOG(DEBUG) << "Obtaining location info location";
     d_location_info = getLocationInfo(manager, addr, code, lasti);
     LOG(DEBUG) << "Code object location info: line_range=(" << d_location_info.lineno << ", "
                << d_location_info.end_lineno << ") column_range=(" << d_location_info.column << ", "
                << d_location_info.end_column << ")";
 
-    d_narguments = manager->versionedCodeField<unsigned int, &py_code_v::o_argcount>(code);
+    d_narguments = manager->getField(code, &py_code_v::o_argcount);
     LOG(DEBUG) << "Code object n arguments: " << d_narguments;
 
     LOG(DEBUG) << "Copying variable names";
-    remote_addr_t varnames_addr =
-            manager->versionedCodeField<remote_addr_t, &py_code_v::o_varnames>(code);
+    remote_addr_t varnames_addr = manager->getField(code, &py_code_v::o_varnames);
     TupleObject varnames(manager, varnames_addr);
     std::transform(
             varnames.Items().cbegin(),
             varnames.Items().cend(),
             std::back_inserter(d_varnames),
             [&](auto& addr) {
                 const std::string varname = manager->getStringFromAddress(addr);
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/pycode.h` & `pystack-1.2.0/src/pystack/_pystack/pycode.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/pyframe.pxd` & `pystack-1.2.0/src/pystack/_pystack/pyframe.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/pythread.cpp` & `pystack-1.2.0/src/pystack/_pystack/pythread.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -46,16 +46,15 @@
         const std::shared_ptr<const AbstractProcessManager>& manager,
         remote_addr_t interp_state_addr)
 {
     LOG(DEBUG) << "Attempting to locate tid offset in pthread structure";
     PyInterpreterState is;
     manager->copyObjectFromProcess(interp_state_addr, &is);
 
-    auto current_thread_addr =
-            manager->versionedInterpreterStateField<remote_addr_t, &py_is_v::o_tstate_head>(is);
+    auto current_thread_addr = manager->getField(is, &py_is_v::o_tstate_head);
 
     auto thread_head = current_thread_addr;
 
     // Iterate over all Python threads until we find a thread that has a tid equal to
     // the process pid. This works because in the main thread the tid is equal to the pid,
     // so when this happens it has to happen on the main thread. Note that the main thread
     // is not necessarily at the head of the Python thread linked list
@@ -63,60 +62,56 @@
 #if defined(__GLIBC__)
     // If we detect GLIBC, we can try the two main known structs for 'struct
     // pthread' that we know about to avoid having to do guess-work by doing a
     // linear scan over the struct.
     while (current_thread_addr != (remote_addr_t) nullptr) {
         PyThreadState current_thread;
         manager->copyObjectFromProcess(current_thread_addr, &current_thread);
-        auto pthread_id_addr =
-                manager->versionedThreadField<unsigned long, &py_thread_v::o_thread_id>(current_thread);
+        auto pthread_id_addr = manager->getField(current_thread, &py_thread_v::o_thread_id);
 
         pid_t the_tid;
         std::vector<off_t> glibc_pthread_offset_candidates = {
                 offsetof(_pthread_structure_with_simple_header, tid),
                 offsetof(_pthread_structure_with_tcbhead, tid)};
         for (off_t candidate : glibc_pthread_offset_candidates) {
             manager->copyObjectFromProcess((remote_addr_t)(pthread_id_addr + candidate), &the_tid);
             if (the_tid == manager->Pid()) {
                 LOG(DEBUG) << "Tid offset located using GLIBC offsets at offset " << std::showbase
                            << std::hex << candidate << " in pthread structure";
                 return candidate;
             }
         }
-        remote_addr_t next_thread_addr =
-                manager->versionedThreadField<remote_addr_t, &py_thread_v::o_next>(current_thread);
+        remote_addr_t next_thread_addr = manager->getField(current_thread, &py_thread_v::o_next);
         if (next_thread_addr == current_thread_addr) {
             break;
         }
         current_thread_addr = next_thread_addr;
     }
 #endif
 
     current_thread_addr = thread_head;
 
     while (current_thread_addr != (remote_addr_t) nullptr) {
         PyThreadState current_thread;
         manager->copyObjectFromProcess(current_thread_addr, &current_thread);
-        auto pthread_id_addr =
-                manager->versionedThreadField<unsigned long, &py_thread_v::o_thread_id>(current_thread);
+        auto pthread_id_addr = manager->getField(current_thread, &py_thread_v::o_thread_id);
 
         // Attempt to locate a field in the pthread struct that's equal to the pid.
         uintptr_t buffer[200];
         manager->copyObjectFromProcess(pthread_id_addr, &buffer);
         for (int i = 0; i < 200; i++) {
             if (static_cast<pid_t>(buffer[i]) == manager->Pid()) {
                 off_t offset = sizeof(uintptr_t) * i;
                 LOG(DEBUG) << "Tid offset located by scanning at offset " << std::showbase << std::hex
                            << offset << " in pthread structure";
                 return offset;
             }
         }
 
-        remote_addr_t next_thread_addr =
-                manager->versionedThreadField<remote_addr_t, &py_thread_v::o_next>(current_thread);
+        remote_addr_t next_thread_addr = manager->getField(current_thread, &py_thread_v::o_next);
         if (next_thread_addr == current_thread_addr) {
             break;
         }
         current_thread_addr = next_thread_addr;
     }
     LOG(ERROR) << "Could not find tid offset in pthread structure";
     return 0;
@@ -135,42 +130,41 @@
     if (frame_addr != (remote_addr_t) nullptr) {
         LOG(DEBUG) << std::hex << std::showbase << "Attempting to construct frame from address "
                    << frame_addr;
         d_first_frame = std::make_unique<FrameObject>(manager, frame_addr, 0);
     }
 
     d_addr = addr;
-    remote_addr_t candidate_next_addr =
-            manager->versionedThreadField<remote_addr_t, &py_thread_v::o_next>(ts);
+    remote_addr_t candidate_next_addr = manager->getField(ts, &py_thread_v::o_next);
     d_next_addr = candidate_next_addr == addr ? (remote_addr_t) nullptr : candidate_next_addr;
 
-    d_pthread_id = manager->versionedThreadField<unsigned long, &py_thread_v::o_thread_id>(ts);
+    d_pthread_id = manager->getField(ts, &py_thread_v::o_thread_id);
     d_tid = getThreadTid(manager, addr, d_pthread_id);
     d_next = nullptr;
 
     if (d_next_addr != (remote_addr_t)NULL) {
         LOG(DEBUG) << std::hex << std::showbase << "Attempting to construct a new thread address "
                    << d_next_addr;
         d_next = std::make_unique<PyThread>(manager, d_next_addr);
     }
 
-    d_gil_status = calculateGilStatus(manager);
+    d_gil_status = calculateGilStatus(ts, manager);
     d_gc_status = calculateGCStatus(ts, manager);
 }
 
 int
 PyThread::getThreadTid(
         const std::shared_ptr<const AbstractProcessManager>& manager,
         remote_addr_t thread_addr,
         unsigned long pthread_id)
 {
     int the_tid = -1;
-    if (manager->majorVersion() > 3 || (manager->majorVersion() == 3 && manager->minorVersion() >= 11)) {
+    if (manager->versionIsAtLeast(3, 11)) {
         manager->copyObjectFromProcess(
-                (remote_addr_t)(thread_addr + offsetof(Python3_11::PyThreadState, native_thread_id)),
+                (remote_addr_t)(thread_addr + manager->getFieldOffset(&py_thread_v::o_native_thread_id)),
                 &the_tid);
     } else {
         the_tid = inferTidFromPThreadStructure(manager, pthread_id);
     }
     return the_tid;
 }
 
@@ -212,25 +206,25 @@
 }
 
 remote_addr_t
 PyThread::getFrameAddr(
         const std::shared_ptr<const AbstractProcessManager>& manager,
         const PyThreadState& ts)
 {
-    if (manager->majorVersion() > 3 || (manager->majorVersion() == 3 && manager->minorVersion() >= 11)) {
-        Python3_11::CFrame cframe;
-        remote_addr_t cframe_addr =
-                manager->versionedThreadField<remote_addr_t, &py_thread_v::o_frame>(ts);
+    if (manager->versionIsAtLeast(3, 11)) {
+        remote_addr_t cframe_addr = manager->getField(ts, &py_thread_v::o_frame);
         if (!manager->isAddressValid(cframe_addr)) {
             return reinterpret_cast<remote_addr_t>(nullptr);
         }
+
+        CFrame cframe;
         manager->copyObjectFromProcess(cframe_addr, &cframe);
-        return reinterpret_cast<remote_addr_t>(cframe.current_frame);
+        return manager->getField(cframe, &py_cframe_v::current_frame);
     } else {
-        return manager->versionedThreadField<remote_addr_t, &py_thread_v::o_frame>(ts);
+        return manager->getField(ts, &py_thread_v::o_frame);
     }
 }
 
 std::shared_ptr<FrameObject>
 PyThread::FirstFrame() const
 {
     return d_first_frame;
@@ -250,37 +244,51 @@
 
 PyThread::GCStatus
 PyThread::isGCCollecting() const
 {
     return d_gc_status;
 }
 
-static inline bool
-supportsExactGilChecking(int major, int minor)
-{
-    return major >= 3 && minor >= 8;
-}
-
 PyThread::GilStatus
-PyThread::calculateGilStatus(const std::shared_ptr<const AbstractProcessManager>& manager) const
+PyThread::calculateGilStatus(
+        PyThreadState& ts,
+        const std::shared_ptr<const AbstractProcessManager>& manager) const
 {
     LOG(DEBUG) << "Attempting to determine GIL Status";
     remote_addr_t thread_addr;
     remote_addr_t pyruntime = manager->findSymbol("_PyRuntime");
     if (pyruntime) {
-        assert(manager->majorVersion() == 3);
+        assert(manager->versionIsAtLeast(3, 0));
         LOG(DEBUG) << "_PyRuntime symbol detected. Searching for GIL status within _PyRuntime structure";
 
-        if (supportsExactGilChecking(manager->majorVersion(), manager->minorVersion())) {
+        if (manager->versionIsAtLeast(3, 12)) {
+            // Fast, exact method supporting per-interpreter GILs:
+            // The thread state points to an interpreter state, which contains
+            // a ceval state, which points to a GIL runtime state.
+            // If that GIL state has `locked` set and `last_holder` is d_addr,
+            // then the thread represented by this PyThread holds the GIL.
+            PyInterpreterState interp;
+            auto is_addr = manager->getField(ts, &py_thread_v::o_interp);
+            manager->copyObjectFromProcess(is_addr, &interp);
+
+            auto gil_addr = manager->getField(interp, &py_is_v::o_gil_runtime_state);
+
+            Python3_9::_gil_runtime_state gil;
+            manager->copyObjectFromProcess(gil_addr, &gil);
+
+            auto locked = *reinterpret_cast<int*>(&gil.locked);
+            auto holder = *reinterpret_cast<remote_addr_t*>(&gil.last_holder);
+
+            return (locked && holder == d_addr ? GilStatus::HELD : GilStatus::NOT_HELD);
+        } else if (manager->versionIsAtLeast(3, 8)) {
             // Fast, exact method by checking the gilstate structure in _PyRuntime
             LOG(DEBUG) << "Searching for the GIL by checking the value of 'tstate_current'";
             PyRuntimeState runtime;
             manager->copyObjectFromProcess(pyruntime, &runtime);
-            uintptr_t tstate_current =
-                    manager->versionedRuntimeField<uintptr_t, &py_runtime_v::o_tstate_current>(runtime);
+            uintptr_t tstate_current = manager->getField(runtime, &py_runtime_v::o_tstate_current);
             return (tstate_current == d_addr ? GilStatus::HELD : GilStatus::NOT_HELD);
         } else {
             LOG(DEBUG) << "Searching for the GIL by scanning the _PyRuntime structure";
             // Slow, potentially unreliable method for older versions.
             // The thread object that has the GIL is stored twice at some unknown
             // offsets in the _PyRuntime structure. In order to determine if a given
             // thread has the GIL, we scan the _PyRuntime struct and check if the
@@ -319,50 +327,36 @@
 
 PyThread::GCStatus
 PyThread::calculateGCStatus(
         PyThreadState& ts,
         const std::shared_ptr<const AbstractProcessManager>& manager) const
 {
     LOG(DEBUG) << "Attempting to determine GC Status";
-    if (manager->majorVersion() < 3 || manager->minorVersion() < 7) {
-        LOG(DEBUG) << "GC Status retrieval not supported by this Python version";
-        return GCStatus::COLLECTING_UNKNOWN;
-    }
-
     GCRuntimeState gcstate;
 
-    switch (manager->minorVersion()) {
-        case 11:
-        case 10:
-        case 9: {
-            PyInterpreterState interp;
-            auto is_addr = manager->versionedThreadField<remote_addr_t, &py_thread_v::o_interp>(ts);
-            manager->copyObjectFromProcess(is_addr, &interp);
-            gcstate = manager->versionedInterpreterStateField<GCRuntimeState, &py_is_v ::o_gc>(interp);
-            break;
-        }
-        case 8:
-        case 7: {
-            remote_addr_t pyruntime = manager->findSymbol("_PyRuntime");
-            if (!pyruntime) {
-                LOG(DEBUG) << "Failed to get GC status because the _PyRuntime symbol is unavailable";
-                return GCStatus::COLLECTING_UNKNOWN;
-            }
-            PyRuntimeState runtime;
-            manager->copyObjectFromProcess(pyruntime, &runtime);
-            gcstate = manager->versionedRuntimeField<GCRuntimeState, &py_runtime_v::o_gc>(runtime);
-            break;
-        }
-        default: {
-            LOG(DEBUG) << "GC Status retrieval not supported by this Python version";
+    if (manager->versionIsAtLeast(3, 9)) {
+        PyInterpreterState interp;
+        auto is_addr = manager->getField(ts, &py_thread_v::o_interp);
+        manager->copyObjectFromProcess(is_addr, &interp);
+        gcstate = manager->getField(interp, &py_is_v ::o_gc);
+    } else if (manager->versionIsAtLeast(3, 7)) {
+        remote_addr_t pyruntime = manager->findSymbol("_PyRuntime");
+        if (!pyruntime) {
+            LOG(DEBUG) << "Failed to get GC status because the _PyRuntime symbol is unavailable";
             return GCStatus::COLLECTING_UNKNOWN;
-        };
+        }
+        PyRuntimeState runtime;
+        manager->copyObjectFromProcess(pyruntime, &runtime);
+        gcstate = manager->getField(runtime, &py_runtime_v::o_gc);
+    } else {
+        LOG(DEBUG) << "GC Status retrieval not supported by this Python version";
+        return GCStatus::COLLECTING_UNKNOWN;
     }
 
-    auto collecting = manager->versionedGcStatesField<remote_addr_t, &py_gc_v::o_collecting>(gcstate);
+    auto collecting = manager->getField(gcstate, &py_gc_v::o_collecting);
     LOG(DEBUG) << "GC status correctly retrieved: " << collecting;
     return collecting ? GCStatus::COLLECTING : GCStatus::NOT_COLLECTING;
 }
 
 // Create a similar funciton which does not pass the pointer to thread state, only the manager and the
 // tid
 std::shared_ptr<PyThread>
@@ -374,13 +368,12 @@
         tid_offset_in_pthread_struct = findPthreadTidOffset(manager, addr);
     }
 
     LOG(DEBUG) << std::hex << std::showbase << "Copying PyInterpreterState struct from address " << addr;
     PyInterpreterState is;
     manager->copyObjectFromProcess(addr, &is);
 
-    auto thread_addr =
-            manager->versionedInterpreterStateField<remote_addr_t, &py_is_v::o_tstate_head>(is);
+    auto thread_addr = manager->getField(is, &py_is_v::o_tstate_head);
     return std::make_shared<PyThread>(manager, thread_addr);
 }
 
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/pythread.h` & `pystack-1.2.0/src/pystack/_pystack/pythread.h`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,17 @@
     GCStatus d_gc_status;
     remote_addr_t d_addr;
     remote_addr_t d_next_addr;
     std::shared_ptr<PyThread> d_next;
     std::shared_ptr<FrameObject> d_first_frame;
 
     // Methods
-    GilStatus calculateGilStatus(const std::shared_ptr<const AbstractProcessManager>& manager) const;
+    GilStatus calculateGilStatus(
+            PyThreadState& ts,
+            const std::shared_ptr<const AbstractProcessManager>& manager) const;
     GCStatus calculateGCStatus(
             PyThreadState& ts,
             const std::shared_ptr<const AbstractProcessManager>& manager) const;
 
     // Static Methods
     static int inferTidFromPThreadStructure(
             const std::shared_ptr<const AbstractProcessManager>& manager,
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/pythread.pxd` & `pystack-1.2.0/src/pystack/_pystack/pythread.pxd`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/pytypes.cpp` & `pystack-1.2.0/src/pystack/_pystack/pytypes.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -158,15 +158,26 @@
     constexpr unsigned int shift = 30;
 #else
     constexpr unsigned int shift = 15;
 #endif
 
     _PyLongObject longobj;
     manager->copyObjectFromProcess(addr, &longobj);
-    ssize_t size = longobj.ob_base.ob_size;
+    ssize_t size;
+    bool negative;
+
+    if (manager->versionIsAtLeast(3, 12)) {
+        auto lv_tag = *reinterpret_cast<uintptr_t*>(&longobj.ob_base.ob_size);
+        negative = (lv_tag & 3) == 2;
+        size = lv_tag >> 3;
+    } else {
+        negative = longobj.ob_base.ob_size < 0;
+        size = std::abs(longobj.ob_base.ob_size);
+    }
+
     if (size == 0) {
         d_value = 0;
         return;
     }
 
     /* Python's Include/longobjrep.h has this declaration:
      *      struct _longobject {
@@ -182,32 +193,34 @@
      *
      *  where SHIFT can be either:
      *       #define PyLong_SHIFT        30
      *       #define PyLong_SHIFT        15
      */
 
     std::vector<digit> digits;
-    digits.resize(std::abs(size));
+    digits.resize(size);
     manager->copyMemoryFromProcess(
             addr + offsetof(_PyLongObject, ob_digit),
-            sizeof(digit) * std::abs(size),
+            sizeof(digit) * size,
             digits.data());
-    for (ssize_t i = 0; i < std::abs(size); ++i) {
+    for (ssize_t i = 0; i < size; ++i) {
         long long factor;
         if (__builtin_mul_overflow(digits[i], (1Lu << (ssize_t)(shift * i)), &factor)) {
             d_overflowed = true;
             return;
         }
         if (__builtin_add_overflow(d_value, factor, &d_value)) {
             d_overflowed = true;
             return;
         }
     }
 
-    d_value = size < 0 ? -1 * d_value : d_value;
+    if (negative) {
+        d_value = -1 * d_value;
+    }
 }
 
 std::string
 LongObject::toString(ssize_t max_size) const
 {
     if (d_is_bool) {
         if (Value() > 0) {
@@ -237,29 +250,29 @@
 getDictEntries(
         const std::shared_ptr<const AbstractProcessManager>& manager,
         const Python3::PyDictObject& dict,
         ssize_t& num_items,
         std::vector<Python3::PyDictKeyEntry>& valid_entries)
 {
     auto keys_addr = reinterpret_cast<remote_addr_t>(dict.ma_keys);
-    assert(manager->majorVersion() == 3);
+    assert(manager->versionIsAtLeast(3, 0));
     ssize_t dk_size = 0;
     int dk_kind = 0;
 
-    if (manager->minorVersion() <= 10) {
-        Python3_3::PyDictKeysObject keys;
-        manager->copyObjectFromProcess(keys_addr, &keys);
-        num_items = keys.dk_nentries;
-        dk_size = keys.dk_size;
-    } else {
+    if (manager->versionIsAtLeast(3, 11)) {
         Python3_11::PyDictKeysObject keys;
         manager->copyObjectFromProcess(keys_addr, &keys);
         num_items = keys.dk_nentries;
         dk_size = 1L << keys.dk_log2_size;
         dk_kind = keys.dk_kind;
+    } else {
+        Python3_3::PyDictKeysObject keys;
+        manager->copyObjectFromProcess(keys_addr, &keys);
+        num_items = keys.dk_nentries;
+        dk_size = keys.dk_size;
     }
     if (num_items == 0) {
         LOG(DEBUG) << std::hex << std::showbase << "There are no elements in this dict";
         return;
     }
     /*
      * The size in bytes of an indice depends on dk_size:
@@ -277,18 +290,18 @@
     } else if (dk_size <= 0xFFFFFFFF) {
         offset = 4 * dk_size;
     } else {
         offset = 8 * dk_size;
     }
 
     offset_t dk_indices_offset = 0;
-    if (manager->minorVersion() <= 10) {
-        dk_indices_offset = offsetof(Python3_3::PyDictKeysObject, dk_indices);
-    } else {
+    if (manager->versionIsAtLeast(3, 11)) {
         dk_indices_offset = offsetof(Python3_11::PyDictKeysObject, dk_indices);
+    } else {
+        dk_indices_offset = offsetof(Python3_3::PyDictKeysObject, dk_indices);
     }
 
     remote_addr_t entries_addr = keys_addr + dk_indices_offset + offset;
 
     std::vector<Python3::PyDictKeyEntry> raw_entries;
     raw_entries.resize(num_items);
 
@@ -340,20 +353,18 @@
 
 DictObject::DictObject(std::shared_ptr<const AbstractProcessManager> manager, remote_addr_t addr)
 : d_manager(std::move(manager))
 {
     // For now, the layout that we use here only allows us to get Python3.6+ dictionaries
     // as dictionaries before that have much more variability and are much harder to get.
 
-    if (d_manager->majorVersion() > 2) {
-        if (d_manager->minorVersion() < 6) {
-            d_invalid = true;
-            return;
-        }
+    if (d_manager->versionIsAtLeast(3, 6)) {
         loadFromPython3(addr);
+    } else if (d_manager->versionIsAtLeast(3, 0)) {
+        d_invalid = true;
     } else {
         loadFromPython2(addr);
     }
 }
 
 void
 DictObject::loadFromPython3(remote_addr_t addr)
@@ -512,17 +523,17 @@
     PyObject obj;
     manager->copyObjectFromProcess(d_addr, &obj);
 
     PyTypeObject cls;
     LOG(DEBUG) << std::hex << std::showbase << "Copying typeobject from address " << obj.ob_type;
     manager->copyMemoryFromProcess((remote_addr_t)obj.ob_type, manager->offsets().py_type.size, &cls);
 
-    d_flags = manager->versionedTypeField<unsigned long, &py_type_v::o_tp_flags>(cls);
+    d_flags = manager->getField(cls, &py_type_v::o_tp_flags);
 
-    remote_addr_t name_addr = manager->versionedTypeField<remote_addr_t, &py_type_v::o_tp_name>(cls);
+    remote_addr_t name_addr = manager->getField(cls, &py_type_v::o_tp_name);
     try {
         d_classname = manager->getCStringFromAddress(name_addr);
     } catch (RemoteMemCopyError& ex) {
         // If the original ELF files are not available, we can try to guess the class
         // name from other available information, specially for the types where the
         // class name is needed to categorize then.
         d_classname = guessClassName(cls);
@@ -614,15 +625,15 @@
              | Pystack_TPFLAGS_BASE_EXC_SUBCLASS
              | Pystack_TPFLAGS_TYPE_SUBCLASS);
     // clang-format on
 
     const long subclass_flags = d_flags & subclass_mask;
 
     if (subclass_flags == Pystack_TPFLAGS_BYTES_SUBCLASS) {
-        return d_manager->majorVersion() > 2 ? ObjectType::BYTES : ObjectType::STRING;
+        return d_manager->versionIsAtLeast(3, 0) ? ObjectType::BYTES : ObjectType::STRING;
     } else if (subclass_flags == Pystack_TPFLAGS_UNICODE_SUBCLASS) {
         return ObjectType::STRING;
     } else if (subclass_flags == Pystack_TPFLAGS_INT_SUBCLASS) {
         if (d_classname == "bool") {
             return ObjectType::INT_BOOL;
         }
         return ObjectType::INT;
@@ -647,20 +658,18 @@
 
 Object::PythonObject
 Object::toConcreteObject() const
 {
     try {
         switch (objectType()) {
             case Object::ObjectType::STRING:
-                if (d_manager->majorVersion() < 3) {
-                    return normalizeBytesObjectRepresentation(
-                            d_manager->getStringFromAddress(d_addr),
-                            "");
+                if (d_manager->versionIsAtLeast(3, 0)) {
+                    return '"' + d_manager->getStringFromAddress(d_addr) + '"';
                 }
-                return '"' + d_manager->getStringFromAddress(d_addr) + '"';
+                return normalizeBytesObjectRepresentation(d_manager->getStringFromAddress(d_addr), "");
             case Object::ObjectType::BYTES:
                 return normalizeBytesObjectRepresentation(d_manager->getBytesFromAddress(d_addr));
             case Object::ObjectType::NONE:
                 return NoneObject(d_addr);
             case Object::ObjectType::INT:
                 return toInteger();
             case Object::ObjectType::INT_BOOL:
@@ -685,15 +694,15 @@
     }
     return GenericObject(d_addr, d_classname);
 }
 
 std::string
 Object::guessClassName(PyTypeObject& type) const
 {
-    remote_addr_t tp_repr = d_manager->versionedTypeField<remote_addr_t, &py_type_v::o_tp_repr>(type);
+    remote_addr_t tp_repr = d_manager->getField(type, &py_type_v::o_tp_repr);
     if (tp_repr == d_manager->findSymbol("float_repr")) {
         return "float";
     }
     if (tp_repr == d_manager->findSymbol("none_repr")) {
         return "NoneType";
     }
     if (tp_repr == d_manager->findSymbol("bool_repr")) {
```

### Comparing `pystack-1.1.0/src/pystack/_pystack/pytypes.h` & `pystack-1.2.0/src/pystack/_pystack/pytypes.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/unwinder.cpp` & `pystack-1.2.0/src/pystack/_pystack/unwinder.cpp`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/unwinder.h` & `pystack-1.2.0/src/pystack/_pystack/unwinder.h`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack/version.cpp` & `pystack-1.2.0/src/pystack/_pystack/version.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -46,30 +46,46 @@
 constexpr py_frame_v
 py_frame()
 {
     return {sizeof(T),
             offsetof(T, f_back),
             offsetof(T, f_code),
             offsetof(T, f_lasti),
+            0,
             offsetof(T, f_localsplus)};
 }
 
 template<class T>
 constexpr py_frame_v
 py_framev311()
 {
     return {sizeof(T),
             offsetof(T, previous),
             offsetof(T, f_code),
-            offsetof(T, f_lasti),
+            0,
+            offsetof(T, prev_instr),
             offsetof(T, localsplus),
             offsetof(T, is_entry)};
 }
 
 template<class T>
+constexpr py_frame_v
+py_framev312()
+{
+    return {sizeof(T),
+            offsetof(T, previous),
+            offsetof(T, f_code),
+            0,
+            offsetof(T, prev_instr),
+            offsetof(T, localsplus),
+            0,
+            offsetof(T, owner)};
+}
+
+template<class T>
 constexpr py_thread_v
 py_thead_h()
 {
     /* Hack. Python 3.3 and below don't have the prev field */
     return {sizeof(T),
             offsetof(T, next),
             offsetof(T, next),
@@ -95,15 +111,16 @@
 py_threadv311()
 {
     return {sizeof(T),
             offsetof(T, prev),
             offsetof(T, next),
             offsetof(T, interp),
             offsetof(T, cframe),
-            offsetof(T, thread_id)};
+            offsetof(T, thread_id),
+            offsetof(T, native_thread_id)};
 }
 
 template<class T>
 constexpr py_is_v
 py_is()
 {
     return {sizeof(T),
@@ -125,37 +142,72 @@
             offsetof(T, gc),
             offsetof(T, modules),
             offsetof(T, sysdict),
             offsetof(T, builtins)};
 }
 
 template<class T>
+constexpr py_is_v
+py_isv312()
+{
+    return {sizeof(T),
+            offsetof(T, next),
+            offsetof(T, threads.head),
+            offsetof(T, gc),
+            offsetof(T, imports.modules),
+            offsetof(T, sysdict),
+            offsetof(T, builtins),
+            offsetof(T, ceval.gil)};
+}
+
+template<class T>
 constexpr py_gc_v
 py_gc()
 {
     return {
             sizeof(T),
             offsetof(T, collecting),
     };
 }
 
 template<class T>
+constexpr py_cframe_v
+py_cframe()
+{
+    return {
+            sizeof(T),
+            offsetof(T, current_frame),
+    };
+}
+
+template<class T>
 constexpr py_runtime_v
 py_runtime()
 {
     return {
             sizeof(T),
             offsetof(T, finalizing),
             offsetof(T, interpreters.head),
             offsetof(T, gc),
             offsetof(T, gilstate.tstate_current._value),
     };
 }
 
 template<class T>
+constexpr py_runtime_v
+py_runtimev312()
+{
+    return {
+            sizeof(T),
+            offsetof(T, finalizing),
+            offsetof(T, interpreters.head),
+    };
+}
+
+template<class T>
 constexpr py_type_v
 py_type()
 {
     return {sizeof(T), offsetof(T, tp_name), offsetof(T, tp_repr), offsetof(T, tp_flags)};
 }
 
 // ---- Python 2 --------------------------------------------------------------
@@ -252,36 +304,45 @@
         py_type<Python3_8::PyTypeObject>(),
         py_codev311<Python3_11::PyCodeObject>(),
         py_framev311<Python3_11::PyFrameObject>(),
         py_threadv311<Python3_11::PyThreadState>(),
         py_isv311<Python3_11::PyInterpreterState>(),
         py_runtime<Python3_11::PyRuntimeState>(),
         py_gc<Python3_8::_gc_runtime_state>(),
+        py_cframe<Python3_11::CFrame>(),
 };
 
-// ----------------------------------------------------------------------------
+// ---- Python 3.12 ------------------------------------------------------------
 
-const auto LATEST_VERSION = &python_v3_10;
+python_v python_v3_12 = {
+        py_type<Python3_8::PyTypeObject>(),
+        py_codev311<Python3_12::PyCodeObject>(),
+        py_framev312<Python3_12::PyFrameObject>(),
+        py_threadv311<Python3_12::PyThreadState>(),
+        py_isv312<Python3_12::PyInterpreterState>(),
+        py_runtimev312<Python3_12::PyRuntimeState>(),
+        py_gc<Python3_8::_gc_runtime_state>(),
+        py_cframe<Python3_12::CFrame>(),
+};
+
+// -----------------------------------------------------------------------------
 
 const python_v*
 getCPythonOffsets(int major, int minor)
 {
     switch (major) {
-        // ---- Python 2 ------------------------------------------------------------
+        // ---- Python 2 -------------------------------------------------------
         case 2:
-            if (minor == 7) {
-                return &python_v2;
-            } else {
+            if (minor != 7) {
                 warnAboutUnsuportedVersion(major, minor);
-                return &python_v2;
             }
+            return &python_v2;
             break;
 
-            // ---- Python 3
-            // ------------------------------------------------------------
+        // ---- Python 3 -------------------------------------------------------
         case 3:
             switch (minor) {
                 case 0:
                 case 1:
                 case 2:
                     warnAboutUnsuportedVersion(major, minor);
                     return &python_v3_3;
@@ -323,15 +384,18 @@
 
                 case 11:
                     return &python_v3_11;
                     break;
 
                 default:
                     warnAboutUnsuportedVersion(major, minor);
-                    return LATEST_VERSION;
+                    // fallthrough to latest
+                case 12:
+                    return &python_v3_12;
+                    break;
             }
             break;
         default:
             throw std::runtime_error("Invalid python version");
     }
 }
 }  // namespace pystack
```

### Comparing `pystack-1.1.0/src/pystack/_pystack.pyi` & `pystack-1.2.0/src/pystack/_pystack.pyi`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/_pystack.pyx` & `pystack-1.2.0/src/pystack/_pystack.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pathlib
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
+from typing import Set
 from typing import Tuple
 from typing import TypeVar
 
 from cython.operator import dereference
 from cython.operator import postincrement
 
 from _pystack.corefile cimport CoreFileExtractor
@@ -232,15 +233,15 @@
     def extract_ps_info(self) -> Dict[str, Any]:
         return self._core_analyzer.get().extractPSInfo()
 
     cdef _is_ignored_lib(self, object path):
         return any(prefix in str(path) for prefix in self.ignored_libs)
 
     @intercept_runtime_errors(EngineError)
-    def missing_modules(self) -> List[str]:
+    def missing_modules(self) -> Set[str]:
         cdef set result = set()
         cdef set missing_mod_names = set()
         for mod in self._core_analyzer.get().missingModules():
             path = pathlib.Path(mod)
             if not self._is_ignored_lib(path):
                 result.add(path)
                 missing_mod_names.add(path.name)
```

### Comparing `pystack-1.1.0/src/pystack/colors.py` & `pystack-1.2.0/src/pystack/colors.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/errors.py` & `pystack-1.2.0/src/pystack/errors.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/maps.py` & `pystack-1.2.0/src/pystack/maps.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/process.py` & `pystack-1.2.0/src/pystack/process.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/traceback_formatter.py` & `pystack-1.2.0/src/pystack/traceback_formatter.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack/types.py` & `pystack-1.2.0/src/pystack/types.py`

 * *Files identical despite different names*

### Comparing `pystack-1.1.0/src/pystack.egg-info/PKG-INFO` & `pystack-1.2.0/src/pystack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pystack
-Version: 1.1.0
+Version: 1.2.0
 Summary: Analysis of the stack of remote python processes
 Home-page: https://github.com/bloomberg/pystack
 Author: Pablo Galindo Salgado
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
@@ -66,14 +66,18 @@
 - 🔍 Even works with Python interpreters' binaries that do not have symbols or debug information
   (Python stack only).
 - 💥 Tolerates memory corruption well. Even if the process crashed due to memory corruption,
   PyStack can usually reconstruct the stack.
 - 💼 Self-contained: it does not depend on external tools or programs other than the Python
   interpreter used to run PyStack itself.
 
+## What platforms are supported?
+
+At this time only Linux is supported.
+
 ## Building from source
 
 If you wish to build PyStack from source, you need the following binary dependencies in your
 system:
 
 - libdw
 - libelf
```

### Comparing `pystack-1.1.0/src/pystack.egg-info/SOURCES.txt` & `pystack-1.2.0/src/pystack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

