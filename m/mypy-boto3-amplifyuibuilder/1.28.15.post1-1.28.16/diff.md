# Comparing `tmp/mypy-boto3-amplifyuibuilder-1.28.15.post1.tar.gz` & `tmp/mypy-boto3-amplifyuibuilder-1.28.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.15.post1.tar", last modified: Sat Jul 29 10:02:27 2023, max compression
+gzip compressed data, was "mypy-boto3-amplifyuibuilder-1.28.16.tar", last modified: Mon Jul 31 19:32:46 2023, max compression
```

## Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1.tar` & `mypy-boto3-amplifyuibuilder-1.28.16.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.740993 mypy-boto3-amplifyuibuilder-1.28.15.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-07-29 10:02:27.732993 mypy-boto3-amplifyuibuilder-1.28.15.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.724993 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58618 2023-07-29 09:37:49.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58508 2023-07-29 09:37:48.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 10:02:27.732993 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-29 10:02:27.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 10:02:27.740993 mypy-boto3-amplifyuibuilder-1.28.15.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-29 09:37:47.000000 mypy-boto3-amplifyuibuilder-1.28.15.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.242207 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22014 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21975 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10361 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-31 19:32:03.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    60153 2023-07-31 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60043 2023-07-31 19:32:04.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 19:32:46.000000 mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:32:46.246207 mypy-boto3-amplifyuibuilder-1.28.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-31 19:32:02.000000 mypy-boto3-amplifyuibuilder-1.28.16/setup.py
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/LICENSE` & `mypy-boto3-amplifyuibuilder-1.28.16/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -356,21 +356,21 @@
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
+    GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentConditionPropertyTypeDef,
     SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
     FormBindingElementTypeDef,
@@ -415,17 +415,18 @@
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateThemeDataTypeDef,
     ValueMappingTypeDef,
     ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    ApiConfigurationOutputTypeDef,
+    ApiConfigurationTypeDef,
     CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
-    CodegenJobRenderConfigTypeDef,
     ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -455,27 +456,31 @@
     FormStyleTypeDef,
     ListThemesResponseTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
     RefreshTokenRequestRequestTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
     CodegenGenericDataNonModelTypeDef,
     ListFormsResponseTypeDef,
     FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
     ComponentChildOutputTypeDef,
     ComponentTypeDef,
     ComponentChildTypeDef,
     CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
+    CodegenJobRenderConfigTypeDef,
     CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
     FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
     CreateComponentResponseTypeDef,
     ExportComponentsResponseTypeDef,
     GetComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/README.md` & `mypy-boto3-amplifyuibuilder-1.28.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -324,21 +324,21 @@
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
+    GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentConditionPropertyTypeDef,
     SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
     FormBindingElementTypeDef,
@@ -383,17 +383,18 @@
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateThemeDataTypeDef,
     ValueMappingTypeDef,
     ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    ApiConfigurationOutputTypeDef,
+    ApiConfigurationTypeDef,
     CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
-    CodegenJobRenderConfigTypeDef,
     ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -423,27 +424,31 @@
     FormStyleTypeDef,
     ListThemesResponseTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
     RefreshTokenRequestRequestTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
     CodegenGenericDataNonModelTypeDef,
     ListFormsResponseTypeDef,
     FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
     ComponentChildOutputTypeDef,
     ComponentTypeDef,
     ComponentChildTypeDef,
     CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
+    CodegenJobRenderConfigTypeDef,
     CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
     FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
     CreateComponentResponseTypeDef,
     ExportComponentsResponseTypeDef,
     GetComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__init__.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__init__.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/__main__.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.15\nVersion:        "
-        " 1.28.15.post1\nBuilder version: 7.16.2\nDocs:           "
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.16\nVersion:         1.28.16\nBuilder"
+        " version: 7.16.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/client.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify.
+        Creates a new form for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
 
     def create_theme(
         self,
@@ -371,15 +371,15 @@
         *,
         appId: str,
         environmentName: str,
         codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
-        Starts a code generation job for for a specified Amplify app and backend
+        Starts a code generation job for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#start_codegen_job)
         """
 
     def update_component(
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/client.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         *,
         appId: str,
         environmentName: str,
         formToCreate: CreateFormDataTypeDef,
         clientToken: str = ...
     ) -> CreateFormResponseTypeDef:
         """
-        Creates a new form for an Amplify.
+        Creates a new form for an Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.create_form)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#create_form)
         """
     def create_theme(
         self,
         *,
@@ -342,15 +342,15 @@
         *,
         appId: str,
         environmentName: str,
         codegenJobToCreate: StartCodegenJobDataTypeDef,
         clientToken: str = ...
     ) -> StartCodegenJobResponseTypeDef:
         """
-        Starts a code generation job for for a specified Amplify app and backend
+        Starts a code generation job for a specified Amplify app and backend
         environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder.Client.start_codegen_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/client/#start_codegen_job)
         """
     def update_component(
         self,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/literals.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/literals.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/paginator.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/paginator.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/type_defs.py` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,21 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
+    "GraphQLRenderConfigTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
     "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
@@ -97,17 +97,18 @@
     "ThemeValueTypeDef",
     "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
     "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
+    "ApiConfigurationOutputTypeDef",
+    "ApiConfigurationTypeDef",
     "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
-    "CodegenJobRenderConfigTypeDef",
     "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -137,27 +138,31 @@
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
+    "ReactStartCodegenJobDataOutputTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenGenericDataModelOutputTypeDef",
     "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
     "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
     "ComponentChildOutputTypeDef",
     "ComponentTypeDef",
     "ComponentChildTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
+    "CodegenJobRenderConfigOutputTypeDef",
+    "CodegenJobRenderConfigTypeDef",
     "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
     "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
@@ -187,14 +192,25 @@
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
 )
 
+GraphQLRenderConfigTypeDef = TypedDict(
+    "GraphQLRenderConfigTypeDef",
+    {
+        "typesFilePath": str,
+        "queriesFilePath": str,
+        "mutationsFilePath": str,
+        "subscriptionsFilePath": str,
+        "fragmentsFilePath": str,
+    },
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
@@ -276,26 +292,14 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
-    {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
-    },
-    total=False,
-)
-
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -1068,14 +1072,34 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
+ApiConfigurationOutputTypeDef = TypedDict(
+    "ApiConfigurationOutputTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Dict[str, Any],
+        "noApiConfig": Dict[str, Any],
+    },
+    total=False,
+)
+
+ApiConfigurationTypeDef = TypedDict(
+    "ApiConfigurationTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Mapping[str, Any],
+        "noApiConfig": Mapping[str, Any],
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldOutputTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -1118,22 +1142,14 @@
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
 
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
-    {
-        "react": ReactStartCodegenJobDataTypeDef,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
     "ComponentBindingPropertiesValueOutputTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
         "defaultValue": str,
     },
@@ -1659,14 +1675,40 @@
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
+ReactStartCodegenJobDataOutputTypeDef = TypedDict(
+    "ReactStartCodegenJobDataOutputTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
         "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
         "primaryKeys": List[str],
     },
 )
@@ -1909,14 +1951,30 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobRenderConfigOutputTypeDef = TypedDict(
+    "CodegenJobRenderConfigOutputTypeDef",
+    {
+        "react": ReactStartCodegenJobDataOutputTypeDef,
+    },
+    total=False,
+)
+
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": ReactStartCodegenJobDataTypeDef,
+    },
+    total=False,
+)
+
 CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaOutputTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
         "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
         "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
         "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
@@ -2088,15 +2146,15 @@
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
-        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "renderConfig": CodegenJobRenderConfigOutputTypeDef,
         "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
         "autoGenerateForms": bool,
         "features": CodegenFeatureFlagsTypeDef,
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": CodegenJobAssetTypeDef,
         "tags": Dict[str, str],
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder/type_defs.pyi` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,21 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
+    "GraphQLRenderConfigTypeDef",
     "CodegenFeatureFlagsTypeDef",
     "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
     "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
-    "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
     "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
@@ -96,17 +96,18 @@
     "ThemeValueTypeDef",
     "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
     "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
+    "ApiConfigurationOutputTypeDef",
+    "ApiConfigurationTypeDef",
     "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
-    "CodegenJobRenderConfigTypeDef",
     "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
     "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
     "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -136,27 +137,31 @@
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
+    "ReactStartCodegenJobDataOutputTypeDef",
+    "ReactStartCodegenJobDataTypeDef",
     "CodegenGenericDataModelOutputTypeDef",
     "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
     "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
     "ComponentChildOutputTypeDef",
     "ComponentTypeDef",
     "ComponentChildTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
+    "CodegenJobRenderConfigOutputTypeDef",
+    "CodegenJobRenderConfigTypeDef",
     "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
     "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
@@ -186,14 +191,25 @@
     {
         "componentName": str,
         "property": str,
         "set": "ComponentPropertyTypeDef",
     },
 )
 
+GraphQLRenderConfigTypeDef = TypedDict(
+    "GraphQLRenderConfigTypeDef",
+    {
+        "typesFilePath": str,
+        "queriesFilePath": str,
+        "mutationsFilePath": str,
+        "subscriptionsFilePath": str,
+        "fragmentsFilePath": str,
+    },
+)
+
 CodegenFeatureFlagsTypeDef = TypedDict(
     "CodegenFeatureFlagsTypeDef",
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
@@ -271,26 +287,14 @@
     "CodegenJobAssetTypeDef",
     {
         "downloadUrl": str,
     },
     total=False,
 )
 
-ReactStartCodegenJobDataTypeDef = TypedDict(
-    "ReactStartCodegenJobDataTypeDef",
-    {
-        "module": JSModuleType,
-        "target": JSTargetType,
-        "script": JSScriptType,
-        "renderTypeDeclarations": bool,
-        "inlineSourceMap": bool,
-    },
-    total=False,
-)
-
 _RequiredCodegenJobSummaryTypeDef = TypedDict(
     "_RequiredCodegenJobSummaryTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
     },
@@ -1023,14 +1027,34 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
+ApiConfigurationOutputTypeDef = TypedDict(
+    "ApiConfigurationOutputTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Dict[str, Any],
+        "noApiConfig": Dict[str, Any],
+    },
+    total=False,
+)
+
+ApiConfigurationTypeDef = TypedDict(
+    "ApiConfigurationTypeDef",
+    {
+        "graphQLConfig": GraphQLRenderConfigTypeDef,
+        "dataStoreConfig": Mapping[str, Any],
+        "noApiConfig": Mapping[str, Any],
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldOutputTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -1069,22 +1093,14 @@
 )
 
 class CodegenGenericDataFieldTypeDef(
     _RequiredCodegenGenericDataFieldTypeDef, _OptionalCodegenGenericDataFieldTypeDef
 ):
     pass
 
-CodegenJobRenderConfigTypeDef = TypedDict(
-    "CodegenJobRenderConfigTypeDef",
-    {
-        "react": ReactStartCodegenJobDataTypeDef,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
     "ComponentBindingPropertiesValueOutputTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
         "defaultValue": str,
     },
@@ -1586,14 +1602,40 @@
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
+ReactStartCodegenJobDataOutputTypeDef = TypedDict(
+    "ReactStartCodegenJobDataOutputTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+ReactStartCodegenJobDataTypeDef = TypedDict(
+    "ReactStartCodegenJobDataTypeDef",
+    {
+        "module": JSModuleType,
+        "target": JSTargetType,
+        "script": JSScriptType,
+        "renderTypeDeclarations": bool,
+        "inlineSourceMap": bool,
+        "apiConfiguration": ApiConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelOutputTypeDef",
     {
         "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
         "primaryKeys": List[str],
     },
 )
@@ -1820,14 +1862,30 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
+CodegenJobRenderConfigOutputTypeDef = TypedDict(
+    "CodegenJobRenderConfigOutputTypeDef",
+    {
+        "react": ReactStartCodegenJobDataOutputTypeDef,
+    },
+    total=False,
+)
+
+CodegenJobRenderConfigTypeDef = TypedDict(
+    "CodegenJobRenderConfigTypeDef",
+    {
+        "react": ReactStartCodegenJobDataTypeDef,
+    },
+    total=False,
+)
+
 CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaOutputTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
         "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
         "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
         "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
@@ -1991,15 +2049,15 @@
         "appId": str,
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
-        "renderConfig": CodegenJobRenderConfigTypeDef,
+        "renderConfig": CodegenJobRenderConfigOutputTypeDef,
         "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
         "autoGenerateForms": bool,
         "features": CodegenFeatureFlagsTypeDef,
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": CodegenJobAssetTypeDef,
         "tags": Dict[str, str],
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-amplifyuibuilder
-Version: 1.28.15.post1
-Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with mypy-boto3-builder 7.16.2
+Version: 1.28.16
+Summary: Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with mypy-boto3-builder 7.16.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-amplifyuibuilder.svg?color=blue)](https://pypi.org/project/mypy-boto3-amplifyuibuilder)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_amplifyuibuilder/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-amplifyuibuilder)](https://pepy.tech/project/mypy-boto3-amplifyuibuilder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AmplifyUIBuilder 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
+[boto3.AmplifyUIBuilder 1.28.16](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -356,21 +356,21 @@
 
 `mypy_boto3_amplifyuibuilder.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_amplifyuibuilder.type_defs import (
     MutationActionSetStateParameterTypeDef,
+    GraphQLRenderConfigTypeDef,
     CodegenFeatureFlagsTypeDef,
     CodegenGenericDataEnumOutputTypeDef,
     CodegenGenericDataEnumTypeDef,
     CodegenGenericDataRelationshipTypeOutputTypeDef,
     CodegenGenericDataRelationshipTypeTypeDef,
     CodegenJobAssetTypeDef,
-    ReactStartCodegenJobDataTypeDef,
     CodegenJobSummaryTypeDef,
     ComponentBindingPropertiesValuePropertiesOutputTypeDef,
     ComponentBindingPropertiesValuePropertiesTypeDef,
     ComponentConditionPropertyTypeDef,
     SortPropertyTypeDef,
     ComponentPropertyBindingPropertiesTypeDef,
     FormBindingElementTypeDef,
@@ -415,17 +415,18 @@
     ThemeValueTypeDef,
     ThemeValuesOutputTypeDef,
     ThemeValuesTypeDef,
     UpdateThemeDataTypeDef,
     ValueMappingTypeDef,
     ActionParametersOutputTypeDef,
     ActionParametersTypeDef,
+    ApiConfigurationOutputTypeDef,
+    ApiConfigurationTypeDef,
     CodegenGenericDataFieldOutputTypeDef,
     CodegenGenericDataFieldTypeDef,
-    CodegenJobRenderConfigTypeDef,
     ComponentBindingPropertiesValueOutputTypeDef,
     ComponentBindingPropertiesValueTypeDef,
     ComponentDataConfigurationOutputTypeDef,
     ComponentDataConfigurationTypeDef,
     ComponentPropertyOutputTypeDef,
     ComponentPropertyTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -455,27 +456,31 @@
     FormStyleTypeDef,
     ListThemesResponseTypeDef,
     PutMetadataFlagRequestRequestTypeDef,
     RefreshTokenRequestRequestTypeDef,
     UpdateThemeRequestRequestTypeDef,
     ComponentEventOutputTypeDef,
     ComponentEventTypeDef,
+    ReactStartCodegenJobDataOutputTypeDef,
+    ReactStartCodegenJobDataTypeDef,
     CodegenGenericDataModelOutputTypeDef,
     CodegenGenericDataNonModelOutputTypeDef,
     CodegenGenericDataModelTypeDef,
     CodegenGenericDataNonModelTypeDef,
     ListFormsResponseTypeDef,
     FormCTATypeDef,
     ValueMappingsOutputTypeDef,
     ValueMappingsTypeDef,
     ComponentChildOutputTypeDef,
     ComponentTypeDef,
     ComponentChildTypeDef,
     CreateComponentDataTypeDef,
     UpdateComponentDataTypeDef,
+    CodegenJobRenderConfigOutputTypeDef,
+    CodegenJobRenderConfigTypeDef,
     CodegenJobGenericDataSchemaOutputTypeDef,
     CodegenJobGenericDataSchemaTypeDef,
     FieldInputConfigOutputTypeDef,
     FieldInputConfigTypeDef,
     CreateComponentResponseTypeDef,
     ExportComponentsResponseTypeDef,
     GetComponentResponseTypeDef,
```

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt` & `mypy-boto3-amplifyuibuilder-1.28.16/mypy_boto3_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-amplifyuibuilder-1.28.15.post1/setup.py` & `mypy-boto3-amplifyuibuilder-1.28.16/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-amplifyuibuilder",
-    version="1.28.15.post1",
+    version="1.28.16",
     packages=["mypy_boto3_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AmplifyUIBuilder 1.28.15 service generated with"
+        "Type annotations for boto3.AmplifyUIBuilder 1.28.16 service generated with"
         " mypy-boto3-builder 7.16.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

