# Comparing `tmp/miko-1.0.tar.gz` & `tmp/miko-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miko-1.0.tar", last modified: Wed Aug 10 18:40:35 2022, max compression
+gzip compressed data, was "miko-1.1.tar", max compression
```

## Comparing `miko-1.0.tar` & `miko-1.1.tar`

### file list

```diff
@@ -1,29 +1,12 @@
-drwxr-xr-x   0 animenosekai   (501) staff       (20)        0 2022-08-10 18:40:35.570234 miko-1.0/
--rw-r--r--   0 animenosekai   (501) staff       (20)     1069 2022-06-29 14:18:14.000000 miko-1.0/LICENSE
--rw-r--r--   0 animenosekai   (501) staff       (20)       32 2022-08-10 15:51:41.000000 miko-1.0/MANIFEST.in
--rw-r--r--   0 animenosekai   (501) staff       (20)    17497 2022-08-10 18:40:35.569534 miko-1.0/PKG-INFO
--rw-r--r--   0 animenosekai   (501) staff       (20)    16611 2022-08-10 16:32:01.000000 miko-1.0/README.md
-drwxr-xr-x   0 animenosekai   (501) staff       (20)        0 2022-08-10 18:40:35.563029 miko-1.0/miko/
--rw-r--r--   0 animenosekai   (501) staff       (20)      651 2022-08-10 18:18:52.000000 miko-1.0/miko/__init__.py
--rw-r--r--   0 animenosekai   (501) staff       (20)    10885 2022-08-10 18:24:33.000000 miko-1.0/miko/__main__.py
--rw-r--r--   0 animenosekai   (501) staff       (20)     9800 2022-08-10 18:23:45.000000 miko-1.0/miko/miko.py
-drwxr-xr-x   0 animenosekai   (501) staff       (20)        0 2022-08-10 18:40:35.567123 miko-1.0/miko/parser/
--rw-r--r--   0 animenosekai   (501) staff       (20)       85 2022-07-10 13:25:15.000000 miko-1.0/miko/parser/__init__.py
-drwxr-xr-x   0 animenosekai   (501) staff       (20)        0 2022-08-10 18:40:35.568919 miko-1.0/miko/parser/__pycache__/
--rw-r--r--   0 animenosekai   (501) staff       (20)      255 2022-07-10 13:35:30.000000 miko-1.0/miko/parser/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 animenosekai   (501) staff       (20)      401 2022-07-10 13:42:43.000000 miko-1.0/miko/parser/__pycache__/example.cpython-39.pyc
--rw-r--r--   0 animenosekai   (501) staff       (20)     8400 2022-07-10 20:30:47.000000 miko-1.0/miko/parser/__pycache__/list.cpython-39.pyc
--rw-r--r--   0 animenosekai   (501) staff       (20)      767 2022-07-10 16:30:59.000000 miko-1.0/miko/parser/__pycache__/parser.cpython-39.pyc
--rw-r--r--   0 animenosekai   (501) staff       (20)      599 2022-07-04 20:41:09.000000 miko-1.0/miko/parser/__pycache__/tag.cpython-39.pyc
--rw-r--r--   0 animenosekai   (501) staff       (20)      171 2022-08-10 18:19:27.000000 miko-1.0/miko/parser/example.py
--rw-r--r--   0 animenosekai   (501) staff       (20)     7055 2022-08-10 16:52:26.000000 miko-1.0/miko/parser/list.py
--rw-r--r--   0 animenosekai   (501) staff       (20)      739 2022-08-10 18:23:20.000000 miko-1.0/miko/parser/parser.py
-drwxr-xr-x   0 animenosekai   (501) staff       (20)        0 2022-08-10 18:40:35.565126 miko-1.0/miko.egg-info/
--rw-r--r--   0 animenosekai   (501) staff       (20)    17497 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/PKG-INFO
--rw-r--r--   0 animenosekai   (501) staff       (20)      572 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/SOURCES.txt
--rw-r--r--   0 animenosekai   (501) staff       (20)        1 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/dependency_links.txt
--rw-r--r--   0 animenosekai   (501) staff       (20)       44 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/entry_points.txt
--rw-r--r--   0 animenosekai   (501) staff       (20)       34 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/requires.txt
--rw-r--r--   0 animenosekai   (501) staff       (20)        5 2022-08-10 18:40:35.000000 miko-1.0/miko.egg-info/top_level.txt
--rw-r--r--   0 animenosekai   (501) staff       (20)       38 2022-08-10 18:40:35.570296 miko-1.0/setup.cfg
--rw-r--r--   0 animenosekai   (501) staff       (20)     1581 2022-08-10 15:51:41.000000 miko-1.0/setup.py
+-rw-r--r--   0        0        0     1069 2022-06-29 14:18:14.030934 miko-1.1/LICENSE
+-rw-r--r--   0        0        0    16611 2023-07-31 16:41:28.187114 miko-1.1/README.md
+-rw-r--r--   0        0        0      449 2023-07-31 16:41:31.256731 miko-1.1/miko/__info__.py
+-rw-r--r--   0        0        0      220 2023-07-31 16:41:57.554130 miko-1.1/miko/__init__.py
+-rw-r--r--   0        0        0    10885 2022-08-10 18:24:33.238367 miko-1.1/miko/__main__.py
+-rw-r--r--   0        0        0    10818 2023-07-31 16:33:28.199720 miko-1.1/miko/miko.py
+-rw-r--r--   0        0        0       85 2022-07-10 13:25:15.187340 miko-1.1/miko/parser/__init__.py
+-rw-r--r--   0        0        0      171 2022-08-10 18:19:27.861704 miko-1.1/miko/parser/example.py
+-rw-r--r--   0        0        0     7437 2023-07-26 15:42:25.708630 miko-1.1/miko/parser/list.py
+-rw-r--r--   0        0        0      739 2023-07-09 11:35:18.797965 miko-1.1/miko/parser/parser.py
+-rw-r--r--   0        0        0     1330 2023-07-31 16:43:35.378841 miko-1.1/pyproject.toml
+-rw-r--r--   0        0        0    17983 1970-01-01 00:00:00.000000 miko-1.1/PKG-INFO
```

### Comparing `miko-1.0/LICENSE` & `miko-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miko-1.0/PKG-INFO` & `miko-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 Metadata-Version: 2.1
 Name: miko
-Version: 1.0
+Version: 1.1
 Summary: See how to use a Python object at a glance!
 Home-page: https://github.com/Animenosekai/miko
-Download-URL: https://github.com/Animenosekai/miko/archive/v1.0.tar.gz
-Author: Anime no Sekai
-Author-email: niichannomail@gmail.com
-License: MIT License
-Keywords: python,documentation,miko,docs
-Classifier: Development Status :: 5 - Production/Stable
+License: MIT
+Keywords: animenosekai,miko,docs,documentation,parser
+Author: Animenosekai
+Author-email: animenosekai.mail@gmail.com
+Maintainer: Animenosekai
+Maintainer-email: animenosekai.mail@gmail.com
+Requires-Python: >=3.6,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.4, <4
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Typing :: Typed
+Project-URL: Documentation, https://github.com/Animenosekai/miko/blob/main/README.md
+Project-URL: Issue Tracker, https://github.com/Animenosekai/miko/issues
+Project-URL: Repository, https://github.com/Animenosekai/miko
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # `miko` (originally: `zero`)
 
 <img src="./assets/miko_icon_rounded.png" alt="miko" align="right" height="220px">
 
  A new Python documentation style
 
@@ -53,15 +63,15 @@
 
 #### Python
 
 You will need Python 3 to use this module
 
 ```bash
 # vermin output
-Minimum required versions: 3.4
+Minimum required versions: 3.6
 Incompatible versions:     2
 ```
 
 ## Installing
 
 ### Option 1: From PyPI
 
@@ -76,15 +86,15 @@
 ```
 
 You can check if you successfully installed it by printing out its version:
 
 ```bash
 $ python -c "import miko; print(miko.__version__)"
 # output:
-miko v1.0
+miko v1.1
 ```
 
 ```bash
 $ miko --version
 # output:
 miko v1.0
 ```
@@ -619,7 +629,8 @@
 ## Authors
 
 - **Anime no Sekai** - *Initial work* - [Animenosekai](https://github.com/Animenosekai)
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+
```

### Comparing `miko-1.0/README.md` & `miko-1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 #### Python
 
 You will need Python 3 to use this module
 
 ```bash
 # vermin output
-Minimum required versions: 3.4
+Minimum required versions: 3.6
 Incompatible versions:     2
 ```
 
 ## Installing
 
 ### Option 1: From PyPI
 
@@ -53,15 +53,15 @@
 ```
 
 You can check if you successfully installed it by printing out its version:
 
 ```bash
 $ python -c "import miko; print(miko.__version__)"
 # output:
-miko v1.0
+miko v1.1
 ```
 
 ```bash
 $ miko --version
 # output:
 miko v1.0
 ```
```

### Comparing `miko-1.0/miko/__main__.py` & `miko-1.1/miko/__main__.py`

 * *Files identical despite different names*

### Comparing `miko-1.0/miko/miko.py` & `miko-1.1/miko/miko.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import inspect
 import sys
 import types
 import typing
 
 import miko.parser.example as example_parsers
 import miko.parser.list as list_parsers
+from miko.parser.parser import Parser
 
 
 class Function:
+    """Retrieves information on a given function"""
+
     def __init__(self, func: typing.Callable) -> None:
         self.original = func
         self.name = self.original.__name__
         self.signature = inspect.signature(func)
         self.docs = Docs(
             docs=self.original.__doc__ if self.original.__doc__ is not None else "No description",
             signature=self.signature
@@ -58,14 +61,17 @@
                 or code object was expected, got {}'''.format(type(obj).__name__))
         return obj
 
     def __repr__(self) -> str:
         return "<Function '{name}'>".format(name=self.name)
 
 
+if sys.version_info >= (3, 6):
+    SECTIONS_MAP: typing.Dict[str, typing.Type[Parser]] # novermin
+
 SECTIONS_MAP = {
     "PARAMETERS": list_parsers.Parameters,
     "PARAMETER": list_parsers.Parameters,
     "PARAMS": list_parsers.Parameters,
     "PARAM": list_parsers.Parameters,
     "ARGUMENTS": list_parsers.Parameters,
     "ARGUMENT": list_parsers.Parameters,
@@ -91,58 +97,82 @@
     "COPYRIGHT": list_parsers.Copyright,
     "AUTHORS": list_parsers.Copyright,
     "AUTHOR": list_parsers.Copyright,
 
     "EXAMPLES": example_parsers.Example,
     "EXAMPLE": example_parsers.Example
 }
+"""All of the default sections and their alternative names"""
 
 
 class Docs:
-    parameters = list_parsers.Parameters()
-    returns = list_parsers.Returns()
-    raises = list_parsers.Raises()
-    changelog = list_parsers.Changelog()
-    copyright = list_parsers.Copyright()
-    example = example_parsers.Example()
-    if sys.version_info >= (3, 6):
-        warnings: typing.List[str]  # novermin
-        notes: typing.List[str]  # novermin
-    else:
-        warnings = []
-        notes = []
-
-    __elements_mapping__ = {v.__map_attribute__ for v in (list_parsers.Parameters, list_parsers.Returns,
-                                                          list_parsers.Raises, list_parsers.Changelog,
-                                                          list_parsers.Copyright, example_parsers.Example)}
+    """Parses docstrings"""
+
+    def __init__(self,
+                 docs: str,
+                 signature: typing.Optional[inspect.Signature] = None,
+                 noself: bool = False,
+                 extra_sections: typing.Optional[typing.Dict[str, typing.Type[Parser]]] = None) -> None:
+        sections_map = SECTIONS_MAP.copy()
+        sections_map.update(extra_sections or {})
+
+        #  Initializing default values
+        self.deprecated = False
+        self.parameters = list_parsers.Parameters()
+        self.returns = list_parsers.Returns()
+        self.raises = list_parsers.Raises()
+        self.changelog = list_parsers.Changelog()
+        self.copyright = list_parsers.Copyright()
+        self.example = example_parsers.Example()
+        if sys.version_info >= (3, 6):
+            # Always better to have typed attributes
+            self.warnings: typing.List[str] = []  # novermin
+            self.notes: typing.List[str] = []  # novermin
+        else:
+            self.warnings = []
+            self.notes = []
+
+        self.__elements_mapping__ = {v.__map_attribute__: v for v in (list_parsers.Parameters, list_parsers.Returns,
+                                                                      list_parsers.Raises, list_parsers.Changelog,
+                                                                      list_parsers.Copyright, example_parsers.Example)}
 
-    def __init__(self, docs: str, signature: inspect.Signature = None, noself: bool = False) -> None:
         if docs is None:
             docs = ""
+
         self.original = inspect.cleandoc(str(docs))
-        self.elements = {}
+
+        if sys.version_info >= (3, 6):
+            self.elements: typing.Dict[str, Parser] = {}
+        else:
+            self.elements = {}
 
         self.warnings = []
         self.notes = []
 
-        missing = {v.__map_attribute__: v for v in (list_parsers.Parameters, list_parsers.Returns,
-                                                    list_parsers.Raises, list_parsers.Changelog,
-                                                    list_parsers.Copyright, example_parsers.Example)}
+        # First, everything is missing
+        missing = self.__elements_mapping__.copy()
 
-        self.description = []
+        description = []
+
+        def clean_name(name: str) -> str:
+            """Cleans the string name to normalize it"""
+            return name.replace(" ", "").upper().strip()
 
         for section in self.original.split("\n\n"):
             name, _, body = section.partition("\n---")
             if not body:
-                self.description.append(name)  # name would be the content here
+                description.append(name)  # name would be the content here
                 continue
-            parse = SECTIONS_MAP.get(name.replace(" ", "").upper().strip(), None)
+
+            # Getting the parser
+            parse = sections_map.get(clean_name(name), None)
             if parse is None:
-                self.description.append("\n---".join((name, body)))
+                description.append("\n---".join((name, body)))
                 continue
+
             content = body.lstrip("-").lstrip("\n")
             try:
                 self.elements[parse.__map_attribute__].extend(content)
             except Exception:
                 self.elements[parse.__map_attribute__] = parse(content, signature=signature, noself=noself)
                 missing.pop(parse.__map_attribute__, None)
         self.original_sections = list(self.elements.keys())
@@ -156,45 +186,49 @@
                 self.elements[list_parsers.Returns.__map_attribute__] = list_parsers.Returns(signature=signature)
                 missing.pop(list_parsers.Returns.__map_attribute__, None)
 
         for attr, parse in missing.items():
             self.elements[attr] = parse()
 
         # HANDLING TAGS
-        for index, line in enumerate(self.description):
+        for index, line in enumerate(description):
             start, _, content = str(line).partition(":")
-            start = start.replace(" ", "").upper().strip()
+            start = clean_name(start)
             content = content.strip()
             if start in {"WARNING", "WARNINGS"}:
                 self.warnings.append(content)
-                self.description[index] = "Warning: {content}".format(content=content)
+                description[index] = "Warning: {content}".format(content=content)
             elif start in {"NOTE", "NOTES", "SEEALSO", "INFORMATION"}:
                 self.notes.append(content)
-                self.description[index] = "Note: {content}".format(content=content)
+                description[index] = "Note: {content}".format(content=content)
 
-        if len(self.description) > 0:
-            checking = str(self.description[0]).replace(" ", "").upper()
+        if len(description) > 0:
+            checking = str(description[0]).replace(" ", "").upper()
             self.deprecated = checking.startswith("!DEPRECATED!") or checking.startswith(
                 "!DEPRECATION!") or checking.startswith("!DEPRECATE!") or checking.startswith("!DEPRECATIONNOTICE!")
             if self.deprecated:
-                index = self.description[0].find("!")
-                second_index = index + self.description[0][index + 1:].find("!") + 2
-                self.description[0] = "! DEPRECATED !" + self.description[0][second_index:]
+                index = description[0].find("!")
+                second_index = index + description[0][index + 1:].find("!") + 2
+                description[0] = "! DEPRECATED !" + description[0][second_index:]
 
-        self.description = "\n\n".join(self.description)
+        self.description = "\n\n".join(description)
 
     def __repr__(self) -> str:
         return "<Docs sections={sections}>".format(sections=self.original_sections)
 
-    def __getattr__(self, key: str):
-        if key in self.__elements_mapping__:
-            return self.elements.__getitem__(key)
-        raise AttributeError
+    def __getattribute__(self, key: str):
+        if key in super().__getattribute__("__elements_mapping__"):
+            return self.__getitem__(key)
+        return super().__getattribute__(key)
+
+    def __getitem__(self, key: str):
+        return self.elements[key]
 
     def dumps(self, indent=4):
+        """Returns a clean docstring"""
         result = ""
         if self.description.replace(" ", ""):
             result += self.description
             result += "\n\n"
         sections = []
         for section in self.elements.values():
             if not isinstance(section, example_parsers.Example) and len(section) <= 0:
@@ -242,14 +276,15 @@
 
         if result.endswith("\n\n"):
             result = result.removesuffix("\n")
 
         return result
 
     def as_dict(self, camelCase: bool = False):
+        """Returns the parsed docstring information as a dictionary"""
         results = {
             "description": self.description,
             "notes": self.notes,
             "warnings": self.warnings,
             "deprecated": self.deprecated
         }
         results.update({k: v.as_dict(camelCase) for k, v in self.elements.items()})
```

### Comparing `miko-1.0/miko/parser/list.py` & `miko-1.1/miko/parser/list.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 class ListElement:
     def __init__(self, name: str, options: list = None, content: list = None, signature: inspect.Signature = None) -> None:
         self.name = name.__name__ if isinstance(name, type) else str(name)
         self.options = [v for v in options if v] if options else []
         self.content = [c for c in content if c] if content else []
         self.signature = signature
 
+    @property
+    def body(self) -> str:
+        return "\n".join(self.content)
+
     def __repr__(self) -> str:
         return "<ListElement options={options}, content={content} lines>".format(options=", ".join(self.options) if len(self.options) > 1 else "None", content=len(self.content))
 
     def as_dict(self, camelCase: bool = False):
         return {
             "name": self.name,
             "options": self.options,
@@ -67,24 +71,33 @@
         if add_to_original:
             self.original += "\n" + content
 
     def __repr__(self) -> str:
         return "<{name} elements={elements}>".format(name=self.__class__.__name__, elements=list(self.elements.keys()))
 
     def __getattr__(self, key: str):
+        return self[key]
+
+    def __getitem__(self, key: str):
         return self.elements.__getitem__(key)
 
 
 class Parameter(ListElement):
     @property
     def deprecated(self) -> bool:
         return "deprecated" in [str(v).lower() for v in self.options]
 
     @property
     def optional(self) -> bool:
+        try:
+            result = self.signature.parameters[self.name].default
+            if not isinstance(result, inspect._empty) and not result is inspect._empty:
+                return True
+        except Exception:
+            pass
         options = [str(v).lower() for v in self.options]
         return "optional" in options or any(v.startswith("default") for v in options)
 
     @property
     def default(self) -> typing.Optional[str]:
         for opt in self.options:
             opt = str(opt)
```

### Comparing `miko-1.0/miko/parser/parser.py` & `miko-1.1/miko/parser/parser.py`

 * *Files identical despite different names*

