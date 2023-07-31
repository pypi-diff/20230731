# Comparing `tmp/mypy-boto3-drs-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-drs-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-drs-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:59 2023, max compression
+gzip compressed data, was "mypy-boto3-drs-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-drs-1.28.15.post1.tar` & `mypy-boto3-drs-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.997113 mypy-boto3-drs-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21764 2023-07-29 10:02:58.985113 mypy-boto3-drs-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.985113 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-29 09:42:47.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17216 2023-07-29 09:42:48.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17214 2023-07-29 09:42:48.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-29 09:42:47.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-07-29 09:42:47.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56826 2023-07-29 09:42:49.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56779 2023-07-29 09:42:49.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:42:46.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:58.985113 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21764 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-29 10:02:58.000000 mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:58.997113 mypy-boto3-drs-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-29 09:42:45.000000 mypy-boto3-drs-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20287 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.266206 mypy-boto3-drs-1.28.16/mypy_boto3_drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39632 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17226 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-07-31 19:32:12.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    56826 2023-07-31 19:32:13.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56779 2023-07-31 19:32:13.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21758 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-31 19:32:46.000000 mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.270206 mypy-boto3-drs-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-31 19:32:11.000000 mypy-boto3-drs-1.28.16/setup.py
```

### Comparing `mypy-boto3-drs-1.28.15.post1/LICENSE` & `mypy-boto3-drs-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/PKG-INFO` & `mypy-boto3-drs-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-drs-1.28.15.post1/README.md` & `mypy-boto3-drs-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__init__.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__init__.pyi` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/__main__.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.drs 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        "Type annotations for boto3.drs 1.28.16\nVersion:         1.28.16\nBuilder version:"
         " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.15.post1")
+    print("1.28.16")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/client.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/client.pyi` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/literals.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
 ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
-TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
+TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/literals.pyi` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 ReplicationConfigurationDefaultLargeStagingDiskTypeType = Literal["AUTO", "GP2", "GP3", "ST1"]
 ReplicationConfigurationEbsEncryptionType = Literal["CUSTOM", "DEFAULT", "NONE"]
 ReplicationConfigurationReplicatedDiskStagingDiskTypeType = Literal[
     "AUTO", "GP2", "GP3", "IO1", "SC1", "ST1", "STANDARD"
 ]
 ReplicationDirectionType = Literal["FAILBACK", "FAILOVER"]
 ReplicationStatusType = Literal["ERROR", "IN_PROGRESS", "PROTECTED", "STOPPED"]
-TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "NONE"]
+TargetInstanceTypeRightSizingMethodType = Literal["BASIC", "IN_AWS", "NONE"]
 drsServiceName = Literal["drs"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/paginator.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/paginator.pyi` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/type_defs.py` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs/type_defs.pyi` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/PKG-INFO` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-drs
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-drs.svg?color=blue)](https://pypi.org/project/mypy-boto3-drs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_drs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-drs)](https://pepy.tech/project/mypy-boto3-drs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.drs 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
+[boto3.drs 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-drs-1.28.15.post1/mypy_boto3_drs.egg-info/SOURCES.txt` & `mypy-boto3-drs-1.28.16/mypy_boto3_drs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-drs-1.28.15.post1/setup.py` & `mypy-boto3-drs-1.28.16/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-drs",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_drs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.drs 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.drs 1.28.16 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

