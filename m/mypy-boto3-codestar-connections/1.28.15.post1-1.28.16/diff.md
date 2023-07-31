# Comparing `tmp/mypy-boto3-codestar-connections-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-codestar-connections-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-codestar-connections-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:48 2023, max compression
+gzip compressed data, was "mypy-boto3-codestar-connections-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-codestar-connections-1.28.15.post1.tar` & `mypy-boto3-codestar-connections-1.28.16.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.413076 mypy-boto3-codestar-connections-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-29 10:02:48.409076 mypy-boto3-codestar-connections-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.409076 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10531 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:48.409076 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-29 10:02:48.000000 mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:48.413076 mypy-boto3-codestar-connections-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-29 09:40:55.000000 mypy-boto3-codestar-connections-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-07-31 19:32:11.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-31 19:32:46.000000 mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.250207 mypy-boto3-codestar-connections-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-31 19:32:10.000000 mypy-boto3-codestar-connections-1.28.16/setup.py
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/LICENSE` & `mypy-boto3-codestar-connections-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeStarconnections 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/README.md` & `mypy-boto3-codestar-connections-1.28.16/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/__main__.py` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CodeStarconnections 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.CodeStarconnections 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/client.py` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
     ) -> CreateConnectionOutputTypeDef:
         """
-        Creates a connection that can then be given to other AWS services like
-        CodePipeline so that it can access third-party code repositories.
+        Creates a connection that can then be given to other Amazon Web Services
+        services like CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#create_connection)
         """
 
     def create_host(
         self,
@@ -201,15 +201,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#tag_resource)
         """
 
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#untag_resource)
         """
 
     def update_host(
         self,
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/client.pyi` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -83,16 +83,16 @@
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
     ) -> CreateConnectionOutputTypeDef:
         """
-        Creates a connection that can then be given to other AWS services like
-        CodePipeline so that it can access third-party code repositories.
+        Creates a connection that can then be given to other Amazon Web Services
+        services like CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#create_connection)
         """
     def create_host(
         self,
         *,
@@ -184,15 +184,15 @@
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#tag_resource)
         """
     def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
-        Removes tags from an AWS resource.
+        Removes tags from an Amazon Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/client/#untag_resource)
         """
     def update_host(
         self,
         *,
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/literals.py` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 
 ConnectionStatusType = Literal["AVAILABLE", "ERROR", "PENDING"]
-ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer"]
+ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer", "GitLab"]
 CodeStarconnectionsServiceName = Literal["codestar-connections"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/literals.pyi` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "CodeStarconnectionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ConnectionStatusType = Literal["AVAILABLE", "ERROR", "PENDING"]
-ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer"]
+ProviderTypeType = Literal["Bitbucket", "GitHub", "GitHubEnterpriseServer", "GitLab"]
 CodeStarconnectionsServiceName = Literal["codestar-connections"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/type_defs.py` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections/type_defs.pyi` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/PKG-INFO` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-codestar-connections
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.CodeStarconnections 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.CodeStarconnections 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-codestar-connections.svg?color=blue)](https://pypi.org/project/mypy-boto3-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_codestar_connections/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-codestar-connections)](https://pepy.tech/project/mypy-boto3-codestar-connections)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CodeStarconnections 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
+[boto3.CodeStarconnections 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/mypy_boto3_codestar_connections.egg-info/SOURCES.txt` & `mypy-boto3-codestar-connections-1.28.16/mypy_boto3_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-codestar-connections-1.28.15.post1/setup.py` & `mypy-boto3-codestar-connections-1.28.16/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-codestar-connections",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CodeStarconnections 1.28.15 service generated with"
+        "Type annotations for boto3.CodeStarconnections 1.28.16 service generated with"
         " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

