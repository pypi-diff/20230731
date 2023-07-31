# Comparing `tmp/eggella-0.0.4.tar.gz` & `tmp/eggella-0.0.5.tar.gz`

## Comparing `eggella-0.0.4.tar` & `eggella-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/__init__.py
--rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/app.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/exceptions.py
--rw-r--r--   0        0        0     8901 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/handler.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/abc.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.4/.gitignore
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 eggella-0.0.4/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 eggella-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/__init__.py
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/app.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/exceptions.py
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4451 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/handler.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/abc.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 eggella-0.0.5/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 eggella-0.0.5/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 eggella-0.0.5/PKG-INFO
```

### Comparing `eggella-0.0.4/eggella/app.py` & `eggella-0.0.5/eggella/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 from prompt_toolkit import HTML, PromptSession
 from prompt_toolkit.completion.fuzzy_completer import FuzzyCompleter
 from prompt_toolkit.completion.nested import NestedDict
 from prompt_toolkit.formatted_text import FormattedText
 
 from eggella.command.abc import ABCCommandHandler
-from eggella.exceptions import CommandNotFoundError, CommandParseError
+from eggella.exceptions import CommandNotFoundError, CommandParseError, CommandTooManyArgumentsError, \
+    CommandArgumentValueError
 from eggella.fsm.fsm import FsmController, IntStateGroup
 from eggella.manager import CommandManager, EventManager
 from eggella.shortcuts.cmd_shortcuts import CmdShortCuts
 
 PromptLikeMsg = Union[str, FormattedText, Callable[..., Union[FormattedText, List[Tuple[str, str]]]]]
 
 _DEFAULT_INTRO_MSG = HTML(
@@ -191,12 +192,17 @@
                 if result := self._command_manager.exec(key, args):
                     self._event_manager.command_complete_event(result)
             except CommandNotFoundError:
                 self._event_manager.command_not_found_event(key, args)
                 self._event_manager.command_suggest_event(key, self._command_manager.commands.keys())
             except CommandParseError:
                 self._event_manager.command_error_event(key, args)
+            except CommandTooManyArgumentsError as exc:
+                self._event_manager.command_many_args_err_event(key, args, exc)
+            except CommandArgumentValueError as exc:
+                self._event_manager.command_argument_value_err_event(key, args, exc)
             except KeyboardInterrupt:
                 if self._event_manager.kb_interrupt_event():
                     break
             except EOFError:
-                self._event_manager.eof_event()
+                if self._event_manager.eof_event():
+                    break
```

### Comparing `eggella-0.0.4/eggella/manager.py` & `eggella-0.0.5/eggella/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 from eggella.command.objects import Command
 from eggella.events.events import (
     OnCommandCompleteSuccess,
     OnCommandError,
     OnCommandNotFound,
     OnEOFError,
     OnKeyboardInterrupt,
-    OnSuggest,
+    OnSuggest, OnCommandTooManyArgumentsError, OnCommandArgumentValueError,
 )
-from eggella.exceptions import CommandNotFoundError
+from eggella.exceptions import CommandNotFoundError, CommandTooManyArgumentsError, CommandArgumentValueError
 from eggella.shortcuts.help_pager import gen_help_pager
 
 if TYPE_CHECKING:
     from eggella.app import Eggella
 
 
 _ErrorEventsMapping = Dict[str, Tuple[Type[BaseException], ...]]
@@ -56,14 +56,21 @@
                 args.append(token)
         return tuple(args), kwargs
 
     def exec(self, key: str, args: str):
         command = self.get(key)
         try:
             return command.handle(args)
+        except TypeError as e:
+            if 'too many positional arguments' in e.args[0]:
+                raise CommandTooManyArgumentsError("Too many arguments") from e
+            else:
+                raise e
+        except ValueError as e:
+            raise CommandArgumentValueError(f"Wrong argument type passed: {e.args}")
         except BaseException as e:
             if err_handler := self.error_events.get(command.fn.__name__):
                 handle_exceptions = self.handled_exceptions.get(command.fn.__name__, None)
                 if handle_exceptions and any(e.__class__ == exc for exc in handle_exceptions):
                     _args, _kwargs = self._simple_parse_arguments(args)
                     return err_handler(key, e, *_args, **_kwargs)
                 else:
@@ -210,14 +217,16 @@
 
         self.kb_interrupt_event: Callable[..., bool] = OnKeyboardInterrupt()
         self.eof_event: Callable[..., bool] = OnEOFError()
         self.command_error_event: Callable[..., None] = OnCommandError()
         self.command_not_found_event: Callable[..., None] = OnCommandNotFound()
         self.command_complete_event: Callable[..., None] = OnCommandCompleteSuccess()
         self.command_suggest_event: Optional[Callable[..., None]] = OnSuggest()
+        self.command_many_args_err_event: Callable[..., None] = OnCommandTooManyArgumentsError()
+        self.command_argument_value_err_event: Callable[..., None] = OnCommandArgumentValueError()
 
     def register_event(
         self,
         name: Literal[
             "start", "close", "kb_interrupt", "eof", "command_not_found", "command_complete", "command_suggest"
         ],
         func: Optional[Callable],
```

### Comparing `eggella-0.0.4/eggella/command/arg_caster.py` & `eggella-0.0.5/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/command/completer.py` & `eggella-0.0.5/eggella/command/completer.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,18 +76,21 @@
         text_before_cursor = document.text_before_cursor
         if self.ignore_case:
             text_before_cursor = text_before_cursor.lower()
         text_arr = text_before_cursor.split(" ")
         last_words = text_arr[-1]
         completions = self.__get_current_completions(text_arr[:-1])
         if all(isinstance(d, dict) for d in completions):
-            nested, meta = completions
-            yield from NestedCommandCompleter.from_nested_dict(nested, meta).get_completions(document, complete_event)
-
+            try:
+                nested, meta = completions
+                yield from NestedCommandCompleter.from_nested_dict(nested, meta).get_completions(document, complete_event)
+            except TypeError:  # unpack err
+                yield
         else:
+            # echo({'echo': None}, {})
             for completion, meta in completions:
                 if completion not in document.text_before_cursor and "=" not in last_words:
                     yield Completion(completion, -len(last_words), display_meta=meta or "")
 
     def __get_current_completions(self, text_arr: List[str]):
         if not text_arr:
             return self.manager.all_completions
```

### Comparing `eggella-0.0.4/eggella/command/handler.py` & `eggella-0.0.5/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/command/objects.py` & `eggella-0.0.5/eggella/command/objects.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/events/events.py` & `eggella-0.0.5/eggella/events/events.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,7 +83,37 @@
         if result:
             print_ft(HTML(f"<out>{result}</out>"), style=self._STYLE)
 
 
 class OnCommandArgumentsException(ABCEvent):
     def __call__(self, key: str, error: BaseException, *args, **kwargs):
         pass
+
+
+class OnCommandArgumentValueError(ABCEvent):
+    _STYLE = Style.from_dict(
+        {
+            "cmd_key": "#7d7c80 italic",
+        }
+    )
+
+    def __call__(self, key: str, args: str, exc: Exception):
+        print_ft(
+            HTML(f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
+                 f"accept wrong argument type. ({', '.join(exc.args)})"),
+            style=self._STYLE,
+        )
+
+
+class OnCommandTooManyArgumentsError(ABCEvent):
+    _STYLE = Style.from_dict(
+        {
+            "cmd_key": "#7d7c80 italic",
+        }
+    )
+
+    def __call__(self, key: str, args: str, exc: Exception):
+        print_ft(
+            HTML(f"<ansired>Error!</ansired> `<cmd_key>{key}</cmd_key>` "
+                 f"too many arguments passed ({', '.join(exc.args)})"),
+            style=self._STYLE,
+        )
```

### Comparing `eggella-0.0.4/eggella/fsm/fsm.py` & `eggella-0.0.5/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.5/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/shortcuts/help_pager.py` & `eggella-0.0.5/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/eggella/tools/type_caster.py` & `eggella-0.0.5/eggella/tools/type_caster.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,18 @@
         else:
             return type_hint
 
     @classmethod
     def cast(cls, type_hint: Type, value: Any) -> Any:
         # extracted annotation from `inspect.get_annotations`
         if type_hint is inspect.Parameter.empty:
-            return value
+            return str(value)
 
         if sys.version_info >= (3, 9):
             type_hint = cls._typing_to_builtin(type_hint)
-
         origin = get_origin(type_hint)
         args = get_args(type_hint)
         # None
         if value is None and type_hint is not bool:
             return value
 
         if origin is not None and args:
```

### Comparing `eggella-0.0.4/.gitignore` & `eggella-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.4/pyproject.toml` & `eggella-0.0.5/pyproject.toml`

 * *Files identical despite different names*

