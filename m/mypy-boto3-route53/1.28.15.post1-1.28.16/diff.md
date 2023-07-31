# Comparing `tmp/mypy-boto3-route53-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-route53-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-1.28.15.post1.tar", last modified: Sat Jul 29 10:04:01 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-1.28.16.tar", last modified: Mon Jul 31 19:32:48 2023, max compression
```

## Comparing `mypy-boto3-route53-1.28.15.post1.tar` & `mypy-boto3-route53-1.28.16.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.953368 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55401 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55315 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63068 2023-07-29 09:57:19.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62997 2023-07-29 09:57:18.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-29 09:57:17.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-29 10:04:01.000000 mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:04:01.969368 mypy-boto3-route53-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-29 09:57:16.000000 mypy-boto3-route53-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.054182 mypy-boto3-route53-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-31 19:32:48.050182 mypy-boto3-route53-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.050182 mypy-boto3-route53-1.28.16/mypy_boto3_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55546 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55460 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-07-31 19:32:35.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63068 2023-07-31 19:32:36.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62997 2023-07-31 19:32:35.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-31 19:32:34.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:48.050182 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-31 19:32:47.000000 mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:48.054182 mypy-boto3-route53-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-31 19:32:33.000000 mypy-boto3-route53-1.28.16/setup.py
```

### Comparing `mypy-boto3-route53-1.28.15.post1/LICENSE` & `mypy-boto3-route53-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/PKG-INFO` & `mypy-boto3-route53-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-route53-1.28.15.post1/README.md` & `mypy-boto3-route53-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__init__.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/__main__.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53 1.28.15\nVersion:         1.28.15.post1\nBuilder"
-        " version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.Route53 1.28.16\nVersion:         1.28.16\nBuilder version:"
+        " 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1024,15 +1024,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_comment)
         """
 
     def update_traffic_policy_instance(
         self, *, Id: str, TTL: int, TrafficPolicyId: str, TrafficPolicyVersion: int
     ) -> UpdateTrafficPolicyInstanceResponseTypeDef:
         """
-        .
+        Updates the resource record sets in a specified hosted zone that were created
+        based on the settings in a specified traffic policy version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_instance)
         """
 
     @overload
     def get_paginator(self, operation_name: Literal["list_cidr_blocks"]) -> ListCidrBlocksPaginator:
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/client.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -947,15 +947,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_comment)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_comment)
         """
     def update_traffic_policy_instance(
         self, *, Id: str, TTL: int, TrafficPolicyId: str, TrafficPolicyVersion: int
     ) -> UpdateTrafficPolicyInstanceResponseTypeDef:
         """
-        .
+        Updates the resource record sets in a specified hosted zone that were created
+        based on the settings in a specified traffic policy version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_traffic_policy_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/client/#update_traffic_policy_instance)
         """
     @overload
     def get_paginator(self, operation_name: Literal["list_cidr_blocks"]) -> ListCidrBlocksPaginator:
         """
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-gov-east-1",
     "us-gov-west-1",
@@ -163,14 +164,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
@@ -197,14 +199,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-gov-east-1",
     "us-gov-west-1",
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/literals.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-gov-east-1",
     "us-gov-west-1",
@@ -161,14 +162,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
@@ -195,14 +197,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-gov-east-1",
     "us-gov-west-1",
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/paginator.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/type_defs.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.py` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53/waiter.pyi` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/PKG-INFO` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.Route53 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-route53-1.28.15.post1/mypy_boto3_route53.egg-info/SOURCES.txt` & `mypy-boto3-route53-1.28.16/mypy_boto3_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.15.post1/setup.py` & `mypy-boto3-route53-1.28.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder"
+        "Type annotations for boto3.Route53 1.28.16 service generated with mypy-boto3-builder"
         " 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

