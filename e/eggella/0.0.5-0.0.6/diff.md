# Comparing `tmp/eggella-0.0.5.tar.gz` & `tmp/eggella-0.0.6.tar.gz`

## Comparing `eggella-0.0.5.tar` & `eggella-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/__init__.py
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/app.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/exceptions.py
--rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/handler.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/abc.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.5/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 eggella-0.0.5/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 eggella-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/__init__.py
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/exceptions.py
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/handler.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/abc.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.6/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 eggella-0.0.6/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 eggella-0.0.6/PKG-INFO
```

### Comparing `eggella-0.0.5/eggella/app.py` & `eggella-0.0.6/eggella/app.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/manager.py` & `eggella-0.0.6/eggella/manager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/command/arg_caster.py` & `eggella-0.0.6/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/command/completer.py` & `eggella-0.0.6/eggella/command/completer.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         text_arr = text_before_cursor.split(" ")
         last_words = text_arr[-1]
         completions = self.__get_current_completions(text_arr[:-1])
         if all(isinstance(d, dict) for d in completions):
             try:
                 nested, meta = completions
                 yield from NestedCommandCompleter.from_nested_dict(nested, meta).get_completions(document, complete_event)
-            except TypeError:  # unpack err
+            except (ValueError, TypeError):  # unpack err
                 yield
         else:
             # echo({'echo': None}, {})
             for completion, meta in completions:
                 if completion not in document.text_before_cursor and "=" not in last_words:
                     yield Completion(completion, -len(last_words), display_meta=meta or "")
```

### Comparing `eggella-0.0.5/eggella/command/handler.py` & `eggella-0.0.6/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/command/objects.py` & `eggella-0.0.6/eggella/command/objects.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/events/events.py` & `eggella-0.0.6/eggella/events/events.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/fsm/fsm.py` & `eggella-0.0.6/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.6/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/shortcuts/help_pager.py` & `eggella-0.0.6/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/eggella/tools/type_caster.py` & `eggella-0.0.6/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/.gitignore` & `eggella-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/README.md` & `eggella-0.0.6/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 - FSM (finite state machine) to organize a branch interface system
 - Error handlers
 - Customized events
 - Auto create commands word completer
 - Auto generate help page (like unix `man` command)
 ## Install
 
-`pip install eggella`
-## Examples:
-### Hello world
+```shell
+pip install eggella
+```
+
+## Hello world
 ```python
 from eggella import Eggella
 
 
 app = Eggella(__name__)
 
 
@@ -38,8 +40,8 @@
     return "Hello, world!"
 
 
 if __name__ == '__main__':
     app.loop()
 ```
 
-See the documentation for more examples!
+See the [documentation](https://eggella.readthedocs.io/en/latest/) and [examples](examples)!
```

### Comparing `eggella-0.0.5/pyproject.toml` & `eggella-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.5/PKG-INFO` & `eggella-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
@@ -45,17 +45,19 @@
 - FSM (finite state machine) to organize a branch interface system
 - Error handlers
 - Customized events
 - Auto create commands word completer
 - Auto generate help page (like unix `man` command)
 ## Install
 
-`pip install eggella`
-## Examples:
-### Hello world
+```shell
+pip install eggella
+```
+
+## Hello world
 ```python
 from eggella import Eggella
 
 
 app = Eggella(__name__)
 
 
@@ -64,8 +66,8 @@
     return "Hello, world!"
 
 
 if __name__ == '__main__':
     app.loop()
 ```
 
-See the documentation for more examples!
+See the [documentation](https://eggella.readthedocs.io/en/latest/) and [examples](examples)!
```

