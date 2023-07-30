# Comparing `tmp/enquire-0.0.2.tar.gz` & `tmp/enquire-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enquire-0.0.2.tar", last modified: Sun Jul 30 18:59:46 2023, max compression
+gzip compressed data, was "enquire-0.0.6.tar", last modified: Sun Jul 30 22:13:59 2023, max compression
```

## Comparing `enquire-0.0.2.tar` & `enquire-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 pavelvorobyev   (503) staff       (20)        0 2023-07-30 18:59:46.536723 enquire-0.0.2/
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      348 2023-07-30 18:59:46.536586 enquire-0.0.2/PKG-INFO
-drwxr-xr-x   0 pavelvorobyev   (503) staff       (20)        0 2023-07-30 18:59:46.535173 enquire-0.0.2/enquire/
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)       27 2023-07-30 18:33:26.000000 enquire-0.0.2/enquire/__init__.py
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      566 2023-07-29 12:47:04.000000 enquire-0.0.2/enquire/prompt.py
-drwxr-xr-x   0 pavelvorobyev   (503) staff       (20)        0 2023-07-30 18:59:46.536424 enquire-0.0.2/enquire/question/
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)       84 2023-07-30 18:33:54.000000 enquire-0.0.2/enquire/question/__init__.py
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)     2687 2023-07-30 18:10:30.000000 enquire-0.0.2/enquire/question/base.py
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)     4821 2023-07-30 18:20:22.000000 enquire-0.0.2/enquire/question/radio.py
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      607 2023-07-30 18:16:24.000000 enquire-0.0.2/enquire/question/text.py
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      267 2023-07-30 18:14:35.000000 enquire-0.0.2/enquire/style.py
-drwxr-xr-x   0 pavelvorobyev   (503) staff       (20)        0 2023-07-30 18:59:46.535876 enquire-0.0.2/enquire.egg-info/
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      348 2023-07-30 18:59:46.000000 enquire-0.0.2/enquire.egg-info/PKG-INFO
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      337 2023-07-30 18:59:46.000000 enquire-0.0.2/enquire.egg-info/SOURCES.txt
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)        1 2023-07-30 18:59:46.000000 enquire-0.0.2/enquire.egg-info/dependency_links.txt
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)       15 2023-07-30 18:59:46.000000 enquire-0.0.2/enquire.egg-info/requires.txt
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)        8 2023-07-30 18:59:46.000000 enquire-0.0.2/enquire.egg-info/top_level.txt
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)      585 2023-07-30 18:59:43.000000 enquire-0.0.2/pyproject.toml
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)       38 2023-07-30 18:59:46.536764 enquire-0.0.2/setup.cfg
--rw-r--r--   0 pavelvorobyev   (503) staff       (20)       38 2023-07-30 18:38:48.000000 enquire-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-30 22:13:58.999915 enquire-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-30 22:13:47.000000 enquire-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire/question/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/question/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-30 22:13:47.000000 enquire-0.0.6/enquire/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 22:13:58.999915 enquire-0.0.6/enquire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-30 22:13:58.000000 enquire-0.0.6/enquire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-30 22:13:47.000000 enquire-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:13:58.999915 enquire-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 22:13:47.000000 enquire-0.0.6/setup.py
```

### Comparing `enquire-0.0.2/enquire/prompt.py` & `enquire-0.0.6/enquire/prompt.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.2/enquire/question/base.py` & `enquire-0.0.6/enquire/question/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, List, Callable, Dict, Any, TypeVar
+from typing import Optional, List, Callable, Dict, Any, TypeVar, Tuple
 from abc import ABC
 from enum import Enum, auto
 from prompt_toolkit.styles import Style
 
 # Validator accepts the current answers dict and the current raw answer given
 # and must return True if validation has passed and False otherwise
 Validator = TypeVar("Validator", bound=Callable[[Dict[str, Any], Any], bool])
@@ -17,27 +17,32 @@
 
 
 class Choice:
 
     name: str
     value: Any
     active: bool
+    checked: bool
 
-    def __init__(self, name: str, value: Optional[Any] = None, active: bool = True):
+    def __init__(self, name: str, value: Optional[Any] = None, active: bool = True, checked: bool = False):
         self.name = name
         self.value = value if value is not None else name
         self.active = active
+        self.checked = checked
 
 
 class Separator(Choice):
 
     def __init__(self, value: Optional[str] = None):
         if value is None:
             value = "-" * 15
-        super().__init__(value, "__separator__", active=False)
+        super().__init__(value, value, active=False)
+
+    def render(self) -> List[Tuple[str, str]]:
+        return [("class:separator", self.value)]
 
 
 class QuestionType(Enum):
 
     TEXT = auto()
     LIST = auto()
```

### Comparing `enquire-0.0.2/enquire/question/radio.py` & `enquire-0.0.6/enquire/question/radio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Callable, Any, Dict, List, Tuple
 from prompt_toolkit.layout.containers import Window
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.layout.controls import FormattedTextControl
 from prompt_toolkit.layout.containers import HSplit
 from prompt_toolkit.layout import Layout
-from prompt_toolkit.application import Application, get_app
+from prompt_toolkit.application import Application
 
 from .base import Question, Choice
 
 
 class Control(FormattedTextControl):
 
     idx: int
@@ -37,36 +37,45 @@
 
         super().__init__(self._get_tokens, show_cursor=False)
 
     @property
     def selected(self) -> Choice:
         return self.choices[self.idx]
 
-    def _get_prompt(self) -> List[Tuple[str, str]]:
+    @property
+    def _separator_tokens(self) -> Tuple[str, str]:
         prompt_len = len(self.prompt) + 8
+        return "class:separator", "-" * prompt_len
+
+    def _get_prompt(self) -> List[Tuple[str, str]]:
         tokens = [
             ("class:qmark", "?"),
             ("class:question", f" {self.prompt}  "),
             ("class:answer", self.selected.name),
             ("", "\n"),
-            ("class:separator", "-" * prompt_len),
+            self._separator_tokens,
             ("", "\n"),
         ]
         return tokens
 
     def _get_tokens(self) -> List[Tuple[str, str]]:
         tokens = self._get_prompt()
         for idx, choice in enumerate(self.choices):
             selected = idx == self.idx
-            if selected:
-                tokens.append(("class:checkbox", " \u25c9 "))
-                tokens.append(("class:selected", choice.name))
+            if hasattr(choice, "render"):
+                tokens.extend(choice.render())
+            elif selected:
+                tokens.append(("class:checkbox-selected", f" {self.checked_char} "))
+                tokens.append(("class:choice-selected", choice.name))
+            elif choice.active:
+                tokens.append(("class:checkbox-unselected", f" {self.unchecked_char} "))
+                tokens.append(("class:choice-unselected", choice.name))
             else:
-                tokens.append(("class:checkbox", " \u25ef "))
-                tokens.append(("class:unselected", choice.name))
+                tokens.append(("", "   ")),
+                tokens.append(("class:choice-unselected", choice.name))
             tokens.append(("", "\n"))
         return tokens
 
     def move_cursor_down(self) -> None:
         while True:
             self.idx = (self.idx + 1) % len(self.choices)
             if self.selected.active:
```

### Comparing `enquire-0.0.2/enquire/question/text.py` & `enquire-0.0.6/enquire/question/text.py`

 * *Files identical despite different names*

### Comparing `enquire-0.0.2/pyproject.toml` & `enquire-0.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "enquire"
-version = "0.0.2"
+version = "0.0.6"
 authors = [{name = "Pavel Vorobyev", email = "viert.ru@gmail.com"}]
 description = "PyInquirer-inspired prompt library"
 requires-python = ">=3.10"
 keywords = [
     "click",
     "PyInquirer",
     "prompt-toolkit",
@@ -22,7 +22,11 @@
 license = {text = "MIT"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "python_toolkit",
 ]
+readme = "README.md"
+
+[project.urls]
+repository = "https://github.com/viert/enquire"
```

