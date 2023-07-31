# Comparing `tmp/argparse_pydantic-0.1.1.tar.gz` & `tmp/argparse_pydantic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_pydantic-0.1.1.tar", last modified: Fri Jul 28 14:56:32 2023, max compression
+gzip compressed data, was "argparse_pydantic-0.1.2.tar", last modified: Mon Jul 31 13:04:07 2023, max compression
```

## Comparing `argparse_pydantic-0.1.1.tar` & `argparse_pydantic-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 14:56:32.546223 argparse_pydantic-0.1.1/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-20 13:37:56.000000 argparse_pydantic-0.1.1/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)     3147 2023-07-28 14:56:32.546223 argparse_pydantic-0.1.1/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)     2440 2023-07-28 14:52:40.000000 argparse_pydantic-0.1.1/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      833 2023-07-28 14:56:32.546223 argparse_pydantic-0.1.1/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-20 13:39:29.000000 argparse_pydantic-0.1.1/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 14:56:32.542223 argparse_pydantic-0.1.1/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 14:56:32.542223 argparse_pydantic-0.1.1/src/argparse_pydantic/
--rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-21 12:12:36.000000 argparse_pydantic-0.1.1/src/argparse_pydantic/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5110 2023-07-26 08:49:40.000000 argparse_pydantic-0.1.1/src/argparse_pydantic/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-21 09:37:02.000000 argparse_pydantic-0.1.1/src/argparse_pydantic/helpers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-21 09:37:02.000000 argparse_pydantic-0.1.1/src/argparse_pydantic/test_tools.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-07-28 14:55:36.000000 argparse_pydantic-0.1.1/src/argparse_pydantic/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 14:56:32.546223 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)     3147 2023-07-28 14:56:32.000000 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      673 2023-07-28 14:56:32.000000 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-28 14:56:32.000000 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-07-28 14:56:32.000000 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-28 14:56:32.000000 argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-28 14:56:32.546223 argparse_pydantic-0.1.1/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-25 09:08:03.000000 argparse_pydantic-0.1.1/tests/test_add_argument_action.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-24 13:37:01.000000 argparse_pydantic-0.1.1/tests/test_add_argument_flag.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4895 2023-07-25 12:20:22.000000 argparse_pydantic-0.1.1/tests/test_add_argument_json_schema_extra.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1276 2023-07-21 13:39:35.000000 argparse_pydantic-0.1.1/tests/test_add_argument_simple.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-25 09:20:47.000000 argparse_pydantic-0.1.1/tests/test_core_base.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-21 09:37:02.000000 argparse_pydantic-0.1.1/tests/test_create_parser.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-24 13:38:31.000000 argparse_pydantic-0.1.1/tests/test_parse_args.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-21 09:37:02.000000 argparse_pydantic-0.1.1/tests/test_test_tools.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3230 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2523 2023-07-31 12:57:21.000000 argparse_pydantic-0.1.2/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      833 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.221323 argparse_pydantic-0.1.2/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.221323 argparse_pydantic-0.1.2/src/argparse_pydantic/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5294 2023-07-31 09:25:37.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-07-31 12:59:57.000000 argparse_pydantic-0.1.2/src/argparse_pydantic/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3230 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      705 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-31 13:04:07.000000 argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-31 13:04:07.225324 argparse_pydantic-0.1.2/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_add_argument_action.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1382 2023-07-31 12:34:17.000000 argparse_pydantic-0.1.2/tests/test_add_argument_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_add_argument_flag.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4752 2023-07-31 12:31:22.000000 argparse_pydantic-0.1.2/tests/test_add_argument_json_schema_extra.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2311 2023-07-31 11:01:21.000000 argparse_pydantic-0.1.2/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_core_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-28 15:19:19.000000 argparse_pydantic-0.1.2/tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.1.1/LICENSE` & `argparse_pydantic-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/PKG-INFO` & `argparse_pydantic-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse_pydantic
-Version: 0.1.1
+Version: 0.1.2
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,20 +14,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Argpare Pydantic
+# Argparse Pydantic
 
 Config for argparse with pydantic model.
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantics)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/benchmark-utils?color=blue)  
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
+![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
 [![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
 
 Simple wrapper for python argparse.  
 Use pydantic model for you app config.  
 It gives you typed config instead of default Namespace from argparse.
 
 Tested on python 3.7 - 3.11
@@ -74,45 +74,50 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
+It exactly like parser made classic way:  
+`parser.add_argument("echo")`
+
 
 ```python
 parser.print_help()
 ```
 <details open> <summary>output</summary>  
-    <pre>usage: MyApp [-h] --echo ECHO
+    <pre>usage: MyApp [-h] echo
+    
+    positional arguments:
+      echo
     
     options:
-      -h, --help   show this help message and exit
-      --echo ECHO
+      -h, --help  show this help message and exit
     </pre>
 </details>
 
 Parse command line as usual.
 
 
 ```python
-args = parser.parse_args(["--echo", "argument from command line"])
+args = parser.parse_args(["argument from command line"])
 ```
 
 When we parse command line, we got Namespace object.  
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
 ```
 
-Now we got confic with type checks / validation ont type hinting when use it at IDE.
+Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
 <details open> <summary>output</summary>  
     <pre>AppCfg(echo='argument from command line')</pre>
```

### Comparing `argparse_pydantic-0.1.1/README.md` & `argparse_pydantic-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Argpare Pydantic
+# Argparse Pydantic
 
 Config for argparse with pydantic model.
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantics)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/benchmark-utils?color=blue)  
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
+![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
 [![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
 
 Simple wrapper for python argparse.  
 Use pydantic model for you app config.  
 It gives you typed config instead of default Namespace from argparse.
 
 Tested on python 3.7 - 3.11
@@ -54,45 +54,50 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
+It exactly like parser made classic way:  
+`parser.add_argument("echo")`
+
 
 ```python
 parser.print_help()
 ```
 <details open> <summary>output</summary>  
-    <pre>usage: MyApp [-h] --echo ECHO
+    <pre>usage: MyApp [-h] echo
+    
+    positional arguments:
+      echo
     
     options:
-      -h, --help   show this help message and exit
-      --echo ECHO
+      -h, --help  show this help message and exit
     </pre>
 </details>
 
 Parse command line as usual.
 
 
 ```python
-args = parser.parse_args(["--echo", "argument from command line"])
+args = parser.parse_args(["argument from command line"])
 ```
 
 When we parse command line, we got Namespace object.  
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
 ```
 
-Now we got confic with type checks / validation ont type hinting when use it at IDE.
+Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
 <details open> <summary>output</summary>  
     <pre>AppCfg(echo='argument from command line')</pre>
```

### Comparing `argparse_pydantic-0.1.1/setup.cfg` & `argparse_pydantic-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/setup.py` & `argparse_pydantic-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/src/argparse_pydantic/core.py` & `argparse_pydantic-0.1.2/src/argparse_pydantic/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,15 +78,18 @@
     field_kwargs = {key: val for key, val in json_schema_extra.items() if key in ARG_KEYWORDS and val is not None}
     if "flag" in field_kwargs:
         field_kwargs["flag"] = process_flag(field_kwargs["flag"])
     return field_kwargs
 
 
 def add_field_arg(
-    parser: argparse.ArgumentParser, field_name: str, field_info: FieldInfo
+    parser: argparse.ArgumentParser,
+    field_name: str,
+    field_info: FieldInfo,
+    undefined_positional: bool = True,
 ) -> None:
     """add argument to parser from field_info"""
     flags = [f"--{field_name}"]
     kwargs = argument_kwargs(
         help=field_info.description,
         required=field_info.is_required(),
         default=field_info.default if field_info.default is not PydanticUndefined else None,
@@ -100,15 +103,16 @@
             **kwargs,
         }
 
     if "flag" in kwargs:
         flags.insert(0, kwargs.pop("flag"))
 
     if field_info.default is PydanticUndefined:
-        if kwargs.pop("positional", False):
+        kwargs_positional = kwargs.pop("positional", False)
+        if undefined_positional or kwargs_positional:
             kwargs["dest"] = field_name
             flags = []
             kwargs.pop("required", None)
         else:
             kwargs["required"] = True
 
     if "action" in kwargs:
@@ -135,19 +139,21 @@
     if action in ("store_true", "store_false"):
         action_default = action.split("_")[1]
         if action_default == str(default).lower():
             raise ValueError(f"action {action} doesn't match default {default}")
 
 
 def add_args_from_model(
-    parser: argparse.ArgumentParser, model: BaseModel
+    parser: argparse.ArgumentParser,
+    model: BaseModel,
+    undefined_positional: bool = True,
 ) -> argparse.ArgumentParser:
     """add args from model to parser"""
     for field_name, field_info in model.model_fields.items():
-        add_field_arg(parser, field_name, field_info)
+        add_field_arg(parser, field_name, field_info, undefined_positional)
     return parser
 
 
 def create_model_obj(model: BaseModel, args: argparse.Namespace) -> BaseModel:
     """create model from parsed args"""
     kwargs = {
         key: val for key, val in args.__dict__.items() if key in model.model_fields
```

### Comparing `argparse_pydantic-0.1.1/src/argparse_pydantic/helpers.py` & `argparse_pydantic-0.1.2/src/argparse_pydantic/helpers.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/src/argparse_pydantic/test_tools.py` & `argparse_pydantic-0.1.2/src/argparse_pydantic/test_tools.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/PKG-INFO` & `argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-pydantic
-Version: 0.1.1
+Version: 0.1.2
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -14,20 +14,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-# Argpare Pydantic
+# Argparse Pydantic
 
 Config for argparse with pydantic model.
 
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantics)](https://pypi.org/project/argparse_pydantic/)
-![PyPI](https://img.shields.io/pypi/v/benchmark-utils?color=blue)  
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/argparse_pydantic)](https://pypi.org/project/argparse_pydantic/)
+![PyPI](https://img.shields.io/pypi/v/argparse_pydantic?color=blue)  
 [![Tests](https://github.com/ayasyrev/argparse_pydantic/workflows/Tests/badge.svg)](https://github.com/ayasyrev/argparse_pydantic/actions?workflow=Tests)  [![Codecov](https://codecov.io/gh/ayasyrev/argparse_pydantic/branch/main/graph/badge.svg)](https://codecov.io/gh/ayasyrev/argparse_pydantic)  
 
 Simple wrapper for python argparse.  
 Use pydantic model for you app config.  
 It gives you typed config instead of default Namespace from argparse.
 
 Tested on python 3.7 - 3.11
@@ -74,45 +74,50 @@
 from argparse_pydantic import add_args_from_model
 
 parser = add_args_from_model(parser, AppCfg)
 ```
 
 So we got parser with arguments from config.
 
+It exactly like parser made classic way:  
+`parser.add_argument("echo")`
+
 
 ```python
 parser.print_help()
 ```
 <details open> <summary>output</summary>  
-    <pre>usage: MyApp [-h] --echo ECHO
+    <pre>usage: MyApp [-h] echo
+    
+    positional arguments:
+      echo
     
     options:
-      -h, --help   show this help message and exit
-      --echo ECHO
+      -h, --help  show this help message and exit
     </pre>
 </details>
 
 Parse command line as usual.
 
 
 ```python
-args = parser.parse_args(["--echo", "argument from command line"])
+args = parser.parse_args(["argument from command line"])
 ```
 
 When we parse command line, we got Namespace object.  
 Bat we can convert it to config object.
 
 
 ```python
 from argparse_pydantic import create_model_obj
 
 cfg = create_model_obj(AppCfg, args)
 ```
 
-Now we got confic with type checks / validation ont type hinting when use it at IDE.
+Now we got  config with type checks / validation ont type hinting when use it at IDE.
 
 
 ```python
 cfg
 ```
 <details open> <summary>output</summary>  
     <pre>AppCfg(echo='argument from command line')</pre>
```

### Comparing `argparse_pydantic-0.1.1/src/argparse_pydantic.egg-info/SOURCES.txt` & `argparse_pydantic-0.1.2/src/argparse_pydantic.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/argparse_pydantic/version.py
 src/argparse_pydantic.egg-info/PKG-INFO
 src/argparse_pydantic.egg-info/SOURCES.txt
 src/argparse_pydantic.egg-info/dependency_links.txt
 src/argparse_pydantic.egg-info/requires.txt
 src/argparse_pydantic.egg-info/top_level.txt
 tests/test_add_argument_action.py
+tests/test_add_argument_base.py
 tests/test_add_argument_flag.py
 tests/test_add_argument_json_schema_extra.py
 tests/test_add_argument_simple.py
 tests/test_core_base.py
 tests/test_create_parser.py
 tests/test_parse_args.py
 tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.1.1/tests/test_add_argument_action.py` & `argparse_pydantic-0.1.2/tests/test_add_argument_action.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/tests/test_add_argument_flag.py` & `argparse_pydantic-0.1.2/tests/test_add_argument_flag.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/tests/test_add_argument_json_schema_extra.py` & `argparse_pydantic-0.1.2/tests/test_add_argument_json_schema_extra.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,31 +38,31 @@
     parser_base.add_argument("--arg_str", type=str, default="", help="simple help")
 
     # parser from cfg
     parser_cfg = ArgumentParserCfg()
     parser = create_parser(parser_cfg=parser_cfg)
 
     # add arguments - ArgHelp
-    add_args_from_model(parser, ArgHelp)
+    add_args_from_model(parser, ArgHelp, undefined_positional=False)
     assert parsers_args_equal(parser_base, parser)
     assert not parsers_actions_diff(parser_base, parser)
     assert parsers_actions_equal(parser_base, parser)
     assert parser_base.format_help() == parser.format_help()
 
 
 def test_parser():
-    """basic parser test create dataclass instance."""
+    """basic parser test create cfg instance."""
     # create parser, add args
     parser = create_parser()
-    add_args_from_model(parser, ArgHelp)
+    add_args_from_model(parser, ArgHelp, undefined_positional=False)
     # parse
     args = parser.parse_args(["--arg_int", "10"])
     # create obj from parsed args
     dc_obj_parsed = create_model_obj(ArgHelp, args)
-    # obj same data from dataclass
+    # obj same data from cfg
     dc_obj_default = ArgHelp(arg_int=10)
     assert dc_obj_parsed == dc_obj_default
 
 
 def test_positional():
     """test positional args"""
 
@@ -70,15 +70,15 @@
         arg_1: int = Field(json_schema_extra=argument_kwargs(positional=True))
         arg_2: float
 
     parser_base = argparse.ArgumentParser()
     parser_base.add_argument("arg_1", type=int)
     parser_base.add_argument("--arg_2", type=float, required=True)
     parser = create_parser()
-    add_args_from_model(parser, ArgPos)
+    add_args_from_model(parser, ArgPos, undefined_positional=False)
     assert not parsers_actions_diff(parser_base, parser)
     assert parsers_equal(parser_base, parser)
 
 
 class ArgFlag(BaseModel):
     arg_1: int = Field(default=1, json_schema_extra=argument_kwargs("-a"))
     arg_2: int = Field(default=1, json_schema_extra=argument_kwargs(flag="b"))
@@ -99,15 +99,15 @@
     assert parsers_args_equal(parser_base, parser)
     assert not parsers_actions_diff(parser_base, parser)
     assert parsers_actions_equal(parser_base, parser)
 
     args = parser.parse_args([])
     # create obj from parsed args
     dc_obj_parsed = create_model_obj(ArgFlag, args)
-    # obj same data from dataclass
+    # obj same data from cfg
     dc_obj_default = ArgFlag()
     assert dc_obj_parsed == dc_obj_default
 
 
 class ArgTypeDef(BaseModel):
     arg_1: int = Field(default=1, json_schema_extra=argument_kwargs(type=float))  # type: ignore  - for check error
     arg_2: int = Field(default=1, json_schema_extra=argument_kwargs(default=2.0))
@@ -122,18 +122,13 @@
     parser_base.add_argument("--arg_3", type=int, default=1)
 
     parser = create_parser()
     add_args_from_model(parser, ArgTypeDef)
     assert parsers_args_equal(parser_base, parser)
     assert parsers_actions_equal(parser_base, parser)
 
-    # captured = capsys.readouterr()
-    # out = captured.out
-    # assert "arg arg_1 type is <class 'int'>, but at metadata <class 'float'>" in out
-    # assert "default=1, but at metadata=2.0" in out
-
     args = parser.parse_args([])
     # create obj from parsed args
     dc_obj_parsed = create_model_obj(ArgTypeDef, args)
-    # obj same data from dataclass
+    # obj same data from cfg
     dc_obj_default = ArgTypeDef()
     assert dc_obj_parsed == dc_obj_default
```

### Comparing `argparse_pydantic-0.1.1/tests/test_add_argument_simple.py` & `argparse_pydantic-0.1.2/tests/test_add_argument_simple.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,21 +23,48 @@
     parser_base.add_argument("--arg_int", type=int, required=True)
     parser_base.add_argument("--arg_float", type=float, default=0.0)
     parser_base.add_argument("--arg_str", type=str, default="")
 
     # parser from cfg
     parser = argparse.ArgumentParser()
 
-    # add arguments - SimpleArg
-    parser = add_args_from_model(parser, SimpleArg)
+    # add arguments - SimpleArg, undefined - as optional, required
+    parser = add_args_from_model(parser, SimpleArg, undefined_positional=False)
     assert parsers_args_equal(parser_base, parser)
     assert not parsers_actions_diff(parser_base, parser)
     assert parsers_actions_equal(parser_base, parser)
     assert parser_base.format_help() == parser.format_help()
 
     # create instance
     args = parser.parse_args(["--arg_int", "1"])
     assert args.arg_int == 1
     cfg = create_model_obj(SimpleArg, args)
     assert cfg.arg_int == 1
     base_model_obj = SimpleArg(arg_int=1)
     assert cfg == base_model_obj
+
+
+def test_add_args_simple_positional():
+    """test basic args, undefined positional"""
+    # base parser
+    parser_base = argparse.ArgumentParser()
+    parser_base.add_argument("arg_int", type=int)
+    parser_base.add_argument("--arg_float", type=float, default=0.0)
+    parser_base.add_argument("--arg_str", type=str, default="")
+
+    # parser from cfg
+    parser = argparse.ArgumentParser()
+
+    # add arguments - SimpleArg, undefined - positional, default
+    parser = add_args_from_model(parser, SimpleArg)
+    assert parsers_args_equal(parser_base, parser)
+    assert not parsers_actions_diff(parser_base, parser)
+    assert parsers_actions_equal(parser_base, parser)
+    assert parser_base.format_help() == parser.format_help()
+
+    # create instance
+    args = parser.parse_args(["1"])
+    assert args.arg_int == 1
+    cfg = create_model_obj(SimpleArg, args)
+    assert cfg.arg_int == 1
+    base_model_obj = SimpleArg(arg_int=1)
+    assert cfg == base_model_obj
```

### Comparing `argparse_pydantic-0.1.1/tests/test_core_base.py` & `argparse_pydantic-0.1.2/tests/test_core_base.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/tests/test_create_parser.py` & `argparse_pydantic-0.1.2/tests/test_create_parser.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/tests/test_parse_args.py` & `argparse_pydantic-0.1.2/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.1.1/tests/test_test_tools.py` & `argparse_pydantic-0.1.2/tests/test_test_tools.py`

 * *Files identical despite different names*

