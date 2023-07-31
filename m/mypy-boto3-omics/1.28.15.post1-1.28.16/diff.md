# Comparing `tmp/mypy-boto3-omics-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-omics-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-omics-1.28.15.post1.tar", last modified: Sat Jul 29 10:03:47 2023, max compression
+gzip compressed data, was "mypy-boto3-omics-1.28.16.tar", last modified: Mon Jul 31 19:32:48 2023, max compression
```

## Comparing `mypy-boto3-omics-1.28.15.post1.tar` & `mypy-boto3-omics-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.697315 mypy-boto3-omics-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29032 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27547 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/
--rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61486 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61374 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15848 2023-07-29 09:52:22.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97914 2023-07-29 09:52:27.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97758 2023-07-29 09:52:26.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-29 09:52:21.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:03:47.689315 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29032 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-29 10:03:47.000000 mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:03:47.697315 mypy-boto3-omics-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-29 09:52:20.000000 mypy-boto3-omics-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29048 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.058182 mypy-boto3-omics-1.28.16/mypy_boto3_omics/
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61486 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61374 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-31 19:32:21.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-07-31 19:32:21.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21971 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21951 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    98062 2023-07-31 19:32:23.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97906 2023-07-31 19:32:22.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-07-31 19:32:20.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29048 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-31 19:32:47.000000 mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:48.066182 mypy-boto3-omics-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-31 19:32:19.000000 mypy-boto3-omics-1.28.16/setup.py
```

### Comparing `mypy-boto3-omics-1.28.15.post1/LICENSE` & `mypy-boto3-omics-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/PKG-INFO` & `mypy-boto3-omics-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -427,14 +427,15 @@
 ```python
 from mypy_boto3_omics.literals import (
     AcceleratorsType,
     AnnotationImportJobCreatedWaiterName,
     AnnotationStoreCreatedWaiterName,
     AnnotationStoreDeletedWaiterName,
     AnnotationTypeType,
+    CreationTypeType,
     EncryptionTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ListAnnotationImportJobsPaginatorName,
     ListAnnotationStoresPaginatorName,
     ListMultipartReadSetUploadsPaginatorName,
```

### Comparing `mypy-boto3-omics-1.28.15.post1/README.md` & `mypy-boto3-omics-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -395,14 +395,15 @@
 ```python
 from mypy_boto3_omics.literals import (
     AcceleratorsType,
     AnnotationImportJobCreatedWaiterName,
     AnnotationStoreCreatedWaiterName,
     AnnotationStoreDeletedWaiterName,
     AnnotationTypeType,
+    CreationTypeType,
     EncryptionTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ListAnnotationImportJobsPaginatorName,
     ListAnnotationStoresPaginatorName,
     ListMultipartReadSetUploadsPaginatorName,
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__init__.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/__main__.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Omics 1.28.15\nVersion:         1.28.15.post1\nBuilder version:"
+        "Type annotations for boto3.Omics 1.28.16\nVersion:         1.28.16\nBuilder version:"
         " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics\nOther"
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

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/client.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 __all__ = (
     "AcceleratorsType",
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationTypeType",
+    "CreationTypeType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoresPaginatorName",
     "ListMultipartReadSetUploadsPaginatorName",
@@ -101,14 +102,15 @@
     "CHR_POS_REF_ALT",
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
+CreationTypeType = Literal["IMPORT", "UPLOAD"]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/literals.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 __all__ = (
     "AcceleratorsType",
     "AnnotationImportJobCreatedWaiterName",
     "AnnotationStoreCreatedWaiterName",
     "AnnotationStoreDeletedWaiterName",
     "AnnotationTypeType",
+    "CreationTypeType",
     "EncryptionTypeType",
     "FileTypeType",
     "FormatToHeaderKeyType",
     "JobStatusType",
     "ListAnnotationImportJobsPaginatorName",
     "ListAnnotationStoresPaginatorName",
     "ListMultipartReadSetUploadsPaginatorName",
@@ -99,14 +100,15 @@
     "CHR_POS_REF_ALT",
     "CHR_START_END_ONE_BASE",
     "CHR_START_END_REF_ALT_ONE_BASE",
     "CHR_START_END_REF_ALT_ZERO_BASE",
     "CHR_START_END_ZERO_BASE",
     "GENERIC",
 ]
+CreationTypeType = Literal["IMPORT", "UPLOAD"]
 EncryptionTypeType = Literal["KMS"]
 FileTypeType = Literal["BAM", "CRAM", "FASTQ"]
 FormatToHeaderKeyType = Literal["ALT", "CHR", "END", "POS", "REF", "START"]
 JobStatusType = Literal[
     "CANCELLED", "COMPLETED", "COMPLETED_WITH_FAILURES", "FAILED", "IN_PROGRESS", "SUBMITTED"
 ]
 ListAnnotationImportJobsPaginatorName = Literal["list_annotation_import_jobs"]
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/paginator.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
+    CreationTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
     ReadSetExportJobStatusType,
@@ -1186,14 +1187,15 @@
         "status": ReadSetStatusType,
         "referenceArn": str,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "sampleId": str,
         "subjectId": str,
         "generatedFrom": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 ReferenceStoreFilterTypeDef = TypedDict(
     "ReferenceStoreFilterTypeDef",
     {
@@ -2724,14 +2726,15 @@
         "subjectId": str,
         "sampleId": str,
         "name": str,
         "description": str,
         "referenceArn": str,
         "sequenceInformation": SequenceInformationTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 
 class ReadSetListItemTypeDef(_RequiredReadSetListItemTypeDef, _OptionalReadSetListItemTypeDef):
     pass
@@ -3543,14 +3546,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/type_defs.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AnnotationTypeType,
+    CreationTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ReadSetActivationJobItemStatusType,
     ReadSetActivationJobStatusType,
     ReadSetExportJobItemStatusType,
     ReadSetExportJobStatusType,
@@ -1141,14 +1142,15 @@
         "status": ReadSetStatusType,
         "referenceArn": str,
         "createdAfter": Union[datetime, str],
         "createdBefore": Union[datetime, str],
         "sampleId": str,
         "subjectId": str,
         "generatedFrom": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 ReferenceStoreFilterTypeDef = TypedDict(
     "ReferenceStoreFilterTypeDef",
     {
@@ -2613,14 +2615,15 @@
         "subjectId": str,
         "sampleId": str,
         "name": str,
         "description": str,
         "referenceArn": str,
         "sequenceInformation": SequenceInformationTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
     },
     total=False,
 )
 
 class ReadSetListItemTypeDef(_RequiredReadSetListItemTypeDef, _OptionalReadSetListItemTypeDef):
     pass
 
@@ -3392,14 +3395,15 @@
         "description": str,
         "fileType": FileTypeType,
         "creationTime": datetime,
         "sequenceInformation": SequenceInformationTypeDef,
         "referenceArn": str,
         "files": ReadSetFilesTypeDef,
         "statusMessage": str,
+        "creationType": CreationTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReferenceMetadataResponseTypeDef = TypedDict(
     "GetReferenceMetadataResponseTypeDef",
     {
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.py` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics/waiter.pyi` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/PKG-INFO` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-omics
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-omics.svg?color=blue)](https://pypi.org/project/mypy-boto3-omics)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_omics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-omics)](https://pepy.tech/project/mypy-boto3-omics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Omics 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
+[boto3.Omics 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#Omics)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -427,14 +427,15 @@
 ```python
 from mypy_boto3_omics.literals import (
     AcceleratorsType,
     AnnotationImportJobCreatedWaiterName,
     AnnotationStoreCreatedWaiterName,
     AnnotationStoreDeletedWaiterName,
     AnnotationTypeType,
+    CreationTypeType,
     EncryptionTypeType,
     FileTypeType,
     FormatToHeaderKeyType,
     JobStatusType,
     ListAnnotationImportJobsPaginatorName,
     ListAnnotationStoresPaginatorName,
     ListMultipartReadSetUploadsPaginatorName,
```

### Comparing `mypy-boto3-omics-1.28.15.post1/mypy_boto3_omics.egg-info/SOURCES.txt` & `mypy-boto3-omics-1.28.16/mypy_boto3_omics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-omics-1.28.15.post1/setup.py` & `mypy-boto3-omics-1.28.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-omics",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_omics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Omics 1.28.15 service generated with mypy-boto3-builder 7.16.2"
+        "Type annotations for boto3.Omics 1.28.16 service generated with mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

