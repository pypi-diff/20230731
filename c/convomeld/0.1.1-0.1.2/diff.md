# Comparing `tmp/convomeld-0.1.1.tar.gz` & `tmp/convomeld-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convomeld-0.1.1.tar", max compression
+gzip compressed data, was "convomeld-0.1.2.tar", max compression
```

## Comparing `convomeld-0.1.1.tar` & `convomeld-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,24 @@
--rw-r--r--   0        0        0    34336 2023-06-28 21:12:02.672170 convomeld-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      226 2023-06-28 22:23:03.047884 convomeld-0.1.1/README.md
--rw-r--r--   0        0        0      697 2023-06-28 21:18:33.697718 convomeld-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-28 20:11:28.121324 convomeld-0.1.1/src/convomeld/__init__.py
--rw-r--r--   0        0        0     8728 2023-06-28 21:02:27.154853 convomeld-0.1.1/src/convomeld/validators.py
--rw-r--r--   0        0        0     1218 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/cli.py
--rw-r--r--   0        0        0       58 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/convomerge.py
--rw-r--r--   0        0        0     1094 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/matchers.py
--rw-r--r--   0        0        0     3155 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/mergers.py
--rw-r--r--   0        0        0     2511 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/parsers.py
--rw-r--r--   0        0        0     7372 2023-06-28 19:18:13.055238 convomeld-0.1.1/src/convomerge/path.py
--rw-r--r--   0        0        0    13609 2023-06-28 19:18:13.059238 convomeld-0.1.1/src/convomerge/script.py
--rw-r--r--   0        0        0     7687 2023-06-28 19:18:13.059238 convomeld-0.1.1/src/convomerge/state.py
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 convomeld-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34336 2023-07-31 16:58:18.192409 convomeld-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      226 2023-07-31 16:58:18.196410 convomeld-0.1.2/README.md
+-rw-r--r--   0        0        0      834 2023-07-31 17:01:53.731839 convomeld-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/__init__.py
+-rw-r--r--   0        0        0       36 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/__main__.py
+-rw-r--r--   0        0        0     5408 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/api.py
+-rw-r--r--   0        0        0     1223 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/cli.py
+-rw-r--r--   0        0        0      102 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/constants.py
+-rw-r--r--   0        0        0     1761 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/convocat.py
+-rw-r--r--   0        0        0     1575 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/convoparse.py
+-rw-r--r--   0        0        0     6868 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/data_factory.py
+-rw-r--r--   0        0        0     2602 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/df_to_convograph.py
+-rw-r--r--   0        0        0    17528 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/graph.py
+-rw-r--r--   0        0        0     1268 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/matchers.py
+-rw-r--r--   0        0        0    10570 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/merge.py
+-rw-r--r--   0        0        0     2512 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/parsers.py
+-rw-r--r--   0        0        0     2905 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/sorters.py
+-rw-r--r--   0        0        0     8061 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/state.py
+-rw-r--r--   0        0        0     5182 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/states.py
+-rw-r--r--   0        0        0     6960 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/thread.py
+-rw-r--r--   0        0        0     1278 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/utils.py
+-rw-r--r--   0        0        0     8730 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/validators.py
+-rw-r--r--   0        0        0     4239 2023-07-31 16:58:18.212411 convomeld-0.1.2/src/convomeld/xlsx_csv_parsers.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 convomeld-0.1.2/PKG-INFO
```

### Comparing `convomeld-0.1.1/LICENSE.md` & `convomeld-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convomeld-0.1.1/pyproject.toml` & `convomeld-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 [tool.poetry]
 name = "convomeld"
-version = "0.1.1"
+version = "0.1.2"
 description = "Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)"
 authors = [
     "Ruslan Borysov <borysov.ruslan98@gmail.com>",
     "Hobson Lane <hobson@tangibleai.com>",
     "Vlad Snisar <vlad@tangibleai.com>",
     "Cetin Czeckr <cetin@tangibleai.com>",
 ]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
-    {include="convomerge", from="src"},
     {include="convomeld", from="src"},
-    ]
+]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 PyYAML = ">=6.0"
+openpyxl = "*"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
+pytest = ">=7.4.0"
+build = "*"
+pip = "*"
+wheel = "*"
+poetry = "*"
+virtualenv = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+convocat = "convomeld.convocat:main"
+convoparse = "convomeld.convoparse:main"
```

### Comparing `convomeld-0.1.1/src/convomeld/validators.py` & `convomeld-0.1.2/src/convomeld/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,8 +197,8 @@
             self.are_target_states_exist,
             self.are_key_lengths_allowed,
         ]
         for check in checks_to_pass:
             invoked_check = check()
             if not isinstance(invoked_check, bool):
                 raise invoked_check
-        return ""
+        return True
```

### Comparing `convomeld-0.1.1/src/convomerge/parsers.py` & `convomeld-0.1.2/src/convomeld/parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 class SimpleScriptParser(ScriptParser):
     def __init__(self, parse_line_regex: str = None, collapse_lines: bool = False) -> None:
         super().__init__()
         
         if parse_line_regex is None:
-            parse_line_regex = '(?P<author>\w+):\s(?P<text>.+)'
+            parse_line_regex = r'(?P<author>\w+):\s(?P<text>.+)'
 
         self.parse_line_pattern = re.compile(parse_line_regex)
         self.collapse_lines = collapse_lines
         self.default_lang_group = 'en'
 
     def parse_lines(self, raw_lines: Sequence[str]) -> Sequence[ScriptLine]:
         if self.collapse_lines:
```

### Comparing `convomeld-0.1.1/src/convomerge/path.py` & `convomeld-0.1.2/src/convomeld/thread.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from __future__ import annotations
 from typing import Iterator, Optional, Union
 from collections.abc import Iterator
-from convomerge.state import Action, State, Trigger, TriggerPlaceholder
+from convomeld.state import Action, State, Trigger, TriggerPlaceholder
 from uuid import uuid4
 
 
-class LinearScriptPath:
+class ConvoThread:
     def __init__(self) -> None:
         self._states: dict[str, State] = {}
         self._uuid = uuid4().hex[-6:]
         self._first_state = None
         self._last_state = None
         self._state_count = 0
 
     def __repr__(self) -> str:
-        return f'LinearScriptPath(states={repr(self._states)}, first_state_name={repr(self._first_state and self._first_state.name)})'
+        return f'ConvoThread(states={repr(self._states)}, first_state_name={repr(self._first_state and self._first_state.name)})'
     
     def __str__(self) -> str:
         res = ''
 
         for state in self.iter_states():
             trigger_str =  f'--{state.triggers[0].value}-->' if len(state.triggers) == 1 else ''
             res += f'{str(state)} {trigger_str} '
 
         return res
 
-    def iter_states(self, with_prev_trigger: bool = False) -> LinearScriptPathIterator:
+    def iter_states(self, with_prev_trigger: bool = False) -> ConvoThreadIterator:
         self.validate()
-        return LinearScriptPathIterator(self._states, self._first_state and self._first_state.name, with_prev_trigger=with_prev_trigger)
+        return ConvoThreadIterator(self._states, self._first_state and self._first_state.name, with_prev_trigger=with_prev_trigger)
 
     def copy(self):
         self.validate()
-        copy = LinearScriptPath()
+        copy = ConvoThread()
         
         for state, prev_trigger in self.iter_states(with_prev_trigger=True):
             if prev_trigger is None:
                 tp = TriggerPlaceholder.empty()
             else:
                 tp = TriggerPlaceholder.from_trigger(prev_trigger)
                 
-            copy = copy.append_state(state.actions, tp, **state.kwargs)
+            copy = copy.append_state(state.actions, tp, **state.attrs)
 
         return copy
         
     # Utils section
 
     def num_states(self) -> int:
         self.validate()
@@ -57,51 +57,42 @@
         self.validate()
         return self._first_state and self._first_state.copy()
 
     def get_last_state(self) -> Optional[State]:
         self.validate()
         return self._last_state and self._last_state.copy()
     
-    def append_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_kwargs) -> LinearScriptPath:
+    def append_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
         self.validate()
         if isinstance(actions, Action):
             actions = [actions]
 
         self._state_count += 1
-        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_kwargs)
+        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
         self._states[new_state.name] = new_state
 
         if len(self._states) == 1:
             self._first_state = new_state
             self._last_state = new_state
             self.validate()
             return self
         
         prev_trigger = tp.create_trigger(new_state.name)
         self._last_state.triggers.append(prev_trigger)
         self._last_state = new_state
         self.validate()
         return self
     
-    def append_path(self, path: LinearScriptPath, tp: TriggerPlaceholder) -> LinearScriptPath:
-        result_path = self
-
-        for state, prev_trigger in path.iter_states(with_prev_trigger=True):
-            prev_tp = tp if prev_trigger is None else TriggerPlaceholder.from_trigger(prev_trigger)
-            result_path = result_path.append_state(state.actions, prev_tp)
-
-        return result_path
-    
-    def prepend_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_kwargs) -> LinearScriptPath:
+    def prepend_state(self, actions: Union[Action, list[Action]], tp: TriggerPlaceholder, **state_attrs) -> ConvoThread:
         self.validate()
         if isinstance(actions, Action):
             actions = [actions]
 
         self._state_count += 1
-        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_kwargs)
+        new_state = State(f'path_{self._uuid}/state_{self._state_count}', actions, **state_attrs)
         self._states[new_state.name] = new_state
 
         if len(self._states) == 1:
             self._first_state = new_state
             self._last_state = new_state
             self.validate()
             return self
@@ -132,19 +123,19 @@
     def validate(self) -> None:
         self._validate_state_names()
         self._validate_linear()
 
     def _validate_state_names(self) -> None:
         for state_name, state in self._states.items():
             if state_name != state.name:
-                raise RuntimeError('State names constraint of LinearScriptPath violated')
+                raise RuntimeError('State names constraint of ConvoThread violated')
             
             for trigger in state.triggers:
                 if trigger.state_name not in self._states:
-                    raise RuntimeError('State names constraint of LinearScriptPath violated')
+                    raise RuntimeError('State names constraint of ConvoThread violated')
     
     def _validate_linear(self) -> None:
         if len(self._states) == 0:
             return
 
         current_state = self._first_state
         num_states = 0
@@ -153,31 +144,31 @@
             if len(current_state.triggers) == 0:
                 # Reached end
                 current_state = None
             elif len(current_state.triggers) == 1:
                 next_state_name = current_state.triggers[0].state_name
                 current_state = self._states[next_state_name]
             else:
-                raise RuntimeError('Linearity constraint of LinearScriptPath violated')
+                raise RuntimeError('Linearity constraint of ConvoThread violated')
 
             num_states += 1
 
         if num_states != len(self._states):
             # print(self)
-            raise RuntimeError('Linearity constraint of LinearScriptPath violated')
+            raise RuntimeError('Linearity constraint of ConvoThread violated')
 
 
-class LinearScriptPathIterator(Iterator[Union[State, tuple[State, Trigger]]]):
+class ConvoThreadIterator(Iterator[Union[State, tuple[State, Trigger]]]):
         def __init__(self, states: dict[str, State], first_state_name: Optional[str], with_prev_trigger: bool) -> None:
             self._states = {state_name: state.copy() for state_name, state in states.items()}
             self._first_state = self._states.get(first_state_name, None)
             self._with_prev_trigger = with_prev_trigger
 
             self._current_state = self._first_state
-            self._current_trigger = None
+            self._current_trigger = TriggerPlaceholder.none().create_trigger(self._current_state.name)
 
         def __next__(self) -> State:
             if self._current_state is None:
                 raise StopIteration()
             
             current_state = self._current_state
             current_trigger = self._current_trigger
```

### Comparing `convomeld-0.1.1/src/convomerge/script.py` & `convomeld-0.1.2/src/convomeld/graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,327 +1,423 @@
 from __future__ import annotations
 from typing import Optional, TextIO, Union, Any
 from collections.abc import Sequence
-from convomerge.state import Action, State, Trigger, TriggerPlaceholder
-from convomerge.path import LinearScriptPath
-from convomerge.parsers import ScriptParser, SimpleScriptParser
-from convomerge.matchers import ActionMatcher, SimpleActionComparator, TriggerValueMatcher, SimpleTriggerValueMatcher
-from convomerge.mergers import PathMergeStrategy, BackPropagationPathMergeStrategy, PathMergeResult
+from convomeld.state import Action, State, Trigger, TriggerPlaceholder
+from convomeld.thread import ConvoThread
+from convomeld.parsers import ScriptParser, SimpleScriptParser
+from convomeld.matchers import ActionMatcher, SimpleActionMatcher, TriggerValueMatcher, SimpleTriggerValueMatcher
+from convomeld.merge import MergeHandler, MergeValidator, StopEarlyHandler, DefaultTriggerHandler, SubthreadAppendHandler, SubthreadMergeHandler
 import os
 import yaml
 from uuid import uuid4
 
 
-class Script:
+class ConvoGraph:
     def __init__(
         self, 
+        action_matcher: ActionMatcher,
+        trigger_matcher: TriggerValueMatcher,
         states: Optional[dict[str, State]] = None, 
-        action_comparator: Optional[ActionMatcher] = None,
-        trigger_comparator: Optional[TriggerValueMatcher] = None,
-        merge_strategy: Optional[PathMergeStrategy] = None,
         convo_name: Optional[str] = None,
-        convo_description: Optional[str] = None
-    ) -> None:
+        convo_description: Optional[str] = None,
+        nlp: Optional[str] = None,
+        use_uuid: bool = True
+    ) -> None:        
+        self._states: dict[str, State] = {}
+        self._action_matcher = action_matcher
+        self._trigger_matcher = trigger_matcher
+        self._uuid = uuid4().hex[-6:]
+        self._state_count = 0
+        self._use_uuid = use_uuid
+        self._merge_handlers: list[MergeHandler] = [
+            MergeValidator(self._trigger_matcher),
+            DefaultTriggerHandler(self._trigger_matcher),
+            SubthreadMergeHandler(self._action_matcher, self._trigger_matcher),
+            SubthreadAppendHandler(self._trigger_matcher),
+            StopEarlyHandler(self._trigger_matcher),
+            MergeValidator(self._trigger_matcher),
+        ]
+
         if states is None:
             if convo_name is None:
                 raise RuntimeError('convo_name must be provided')
             if convo_description is None:
-                convo_description = ''
-
-            self._states: dict[str, State] = {
-                'start': State('start', triggers=[TriggerPlaceholder.next().create_trigger('stop')], convo_name=convo_name, convo_description=convo_description),
-                'stop': State('stop')
+                convo_description = 'empty'
+            if nlp is None:
+                nlp = 'case_insensitive'
+
+            states = {
+                'start': State('start', triggers=[TriggerPlaceholder.timeout().create_trigger('stop')], convo_name=convo_name, convo_description=convo_description, nlp=nlp),
+                'stop': State('stop', triggers=[TriggerPlaceholder.default().create_trigger('start')])
             }
-            # self._max_level = 0
-        else:
-            self._states: dict[str, State] = {state_name: state.copy() for state_name, state in states.items()}
-            # self._max_level = max([state.kwargs.get('level', 0) for state in self._states.values()])
-        
-        self._start_state: State = self._states['start']
-        self._current_state: State = self._start_state
-        self._stop_state: State = self._states['stop']
-
-        self._action_comparator = action_comparator or SimpleActionComparator()
-        self._trigger_comparator = trigger_comparator or SimpleTriggerValueMatcher()
-        self._merge_strategy = merge_strategy or BackPropagationPathMergeStrategy(self._action_comparator, self._trigger_comparator)
-        self._uuid = uuid4().hex[-6:]
-        self._state_count = 0
+
+        for state in states.values():
+            state_attrs = dict(state.attrs)
+
+            if state.name == 'start':
+                if convo_name is not None:
+                    state_attrs['convo_name'] = convo_name
+                if convo_description is not None:
+                    state_attrs['convo_description'] = convo_description
+                if nlp is not None:
+                    state_attrs['nlp'] = nlp
+            elif state.name == 'stop':
+                pass
+            else:
+                self._state_count += 1
+
+            self._states[state.name] = state.copy(**state_attrs)
 
     # Graph section
 
-    def _find_state(
+    def _generate_state_name(self):
+        if self._use_uuid:
+            return f'script_{self._uuid}/state_{self._state_count}'
+        else:
+            return f'{self._states["start"].attrs["convo_name"]}/state_{self._state_count}'
+
+    def create_state(self, src: State) -> State:
+        self._state_count += 1
+        new_state_name = self._generate_state_name()
+        new_state = src.copy(name=new_state_name, triggers=[])
+        self._states[new_state.name] = new_state
+        return new_state
+
+    def find_state(
         self,
         name: Optional[str]=None,
         actions: Optional[Sequence[Action]]=None,
         many: bool=False
-    ) -> Optional[State] | Sequence[State]:
+    ) -> Union[Optional[State], Sequence[State]]:
         if name is not None:
             states = [self._states[name]] if name in self._states else []
         else:
             states = list(self._states.values())
 
         if actions is not None:
-            states = [state for state in states if self._action_comparator.match_seq(state.actions, actions)]
+            states = [state for state in states if self._action_matcher.match(state.actions, actions)]
 
         if many:
             return states
         else:
             return states[0] if len(states) else None
         
-    def _find_paths(self, from_state: State, to_state: Optional[State], many: bool = False) -> Union[LinearScriptPath, list[LinearScriptPath]]:
-        states_queue: list[tuple[State, LinearScriptPath]] = [
-            (from_state, LinearScriptPath().append_state(from_state.actions, TriggerPlaceholder.empty()))
-        ]
-        processed_states = set()
-        discovered_paths = []
-
-        while len(states_queue) > 0:
-            current_state, current_path = states_queue.pop(0)
-
-            if current_state is to_state and current_path.num_triggers() > 0:
-                if not many:
-                    return current_path
-                
-                discovered_paths.append(current_path)
-
-                if current_state.find_trigger(TriggerPlaceholder.default().create_trigger(current_state.name), self._trigger_comparator):
-                    discovered_paths.append(current_path.copy().append_state(current_state.actions, TriggerPlaceholder.default()))
-
+    def num_states(self) -> int:
+        return len(self._states)
+        
+    def _merge_next_subthread(self, current_state: State, tp: TriggerPlaceholder, next_subthread: ConvoThread, merge_state: Optional[State]) -> State:
+        # current_state: already existing State of the ConvoGraph
+        # tp: generates trigger to connect existing state with the next_subthread
+        # next_subthread: follows trigger generated from tp, can be merged with already existing "next subthreads" triggered from current_state
+        # merge_state: final state which is the end of next_subthread, should be created if is None, can be already existing State, can also equal current_state
+
+        for merge_handler in self._merge_handlers:
+            merge_handler_result = merge_handler.merge(self, current_state, tp, next_subthread, merge_state)
+
+            if merge_handler_result is not None:
+                # merge_state <- merge_handler_result
+                if merge_state is not None and merge_handler_result is not merge_state:
+                    raise RuntimeError(f'Merge error: merge_handler_result {merge_handler_result} is expected to be target merge_state f{merge_state}')
+
+                merge_state = merge_handler_result 
+
+        if merge_state is None:
+            raise RuntimeError('Merge error: merge_state is None after all merge handlers')
+
+        return merge_state
+
+    def merge_thread(self, thread: ConvoThread) -> ConvoGraph:
+        if not thread.get_first_state().attrs.get('is_start', False):
+            raise RuntimeError('Merge error: target thread must begin with "start" state')
+        if not thread.get_last_state().attrs.get('is_stop', False):
+            raise RuntimeError('Merge error: target thread must end with "stop" state')
+        # Pop "start" state
+        thread.pop_first_state()
+
+        current_state = self._states['start']
+        current_tp = TriggerPlaceholder.next()
+
+        next_subthread = ConvoThread()
+
+        for state, prev_trigger in thread.iter_states(with_prev_trigger=True):
+            next_subthread.append_state(state.actions, TriggerPlaceholder.from_trigger(prev_trigger), **state.attrs)
+            
+            # Check whether "next_subthread" should be accumulate or processed
+            if len(state.triggers) == 0:
+                self._merge_next_subthread(current_state, current_tp, next_subthread, self._states['stop'])
                 continue
-            if current_state in processed_states:
-                if to_state is None:
-                    discovered_paths.append(current_path)
 
-                continue
+            state_trigger = state.triggers[0]
+            merge_state = self.find_state(actions=state.actions)
 
-            processed_states.add(current_state)
-            next_states = [
-                self._find_state(name=trigger.state_name) 
-                for trigger in current_state.triggers
-            ]
-            next_paths = [
-                current_path.copy().append_state(next_state.actions, TriggerPlaceholder.from_trigger(trigger)) 
-                for next_state, trigger in zip(next_states, current_state.triggers)
-            ]
-            states_queue += zip(next_states, next_paths)
+            if state_trigger.is_next():
+                if merge_state is None:
+                    continue
+                elif merge_state.find_trigger(TriggerPlaceholder.next(), self._trigger_matcher) is not None:
+                    continue
+                else:
+                    state_trigger = TriggerPlaceholder.timeout().create_trigger(state_trigger.state_name)
+
+            current_state = self._merge_next_subthread(current_state, current_tp, next_subthread, merge_state)
+            current_tp = TriggerPlaceholder.from_trigger(state_trigger)
+            next_subthread = ConvoThread()
 
-        return discovered_paths
-    
-    def append_state(self, actions: list[Action], tp: TriggerPlaceholder, **state_kwargs: dict[str, Any]) -> None:
-        if self._current_state is self._start_state:
-            tp = TriggerPlaceholder.next()
+        return self
 
-        self._state_count += 1
-        new_state = State(f'script_{self._uuid}/state_{self._state_count}', actions, **state_kwargs)
-        self._states[new_state.name] = new_state
-        self._current_state.triggers.append(tp.create_trigger(new_state.name))
-        self._current_state = new_state
+    def to_threads(self) -> list[ConvoThread]:
+        start_state = self._states['start']
 
-    def move_to_state(self, state_name: str, tp: TriggerPlaceholder, **state_kwargs: dict[str, Any]) -> None:
-        if state_name not in self._states:
-            raise RuntimeError(f'State name error: target state name "{state_name}" not found in {list(self._states.keys())}')
-        
-        state = self._states[state_name]
-        state.kwargs.update(state_kwargs)
-        self._current_state.triggers.append(tp.create_trigger(state_name))
-        self._current_state = state
-
-    def merge_or_append_branch(self, branch: LinearScriptPath, tp: TriggerPlaceholder, mark_stop: bool = False) -> None:
-        # Remove stop trigger from current state
-        stop_trigger = None
-        for trigger in self._current_state.triggers:
-            if trigger.state_name == 'stop':
-                stop_trigger = trigger.copy()
-                break
-        else:
-            raise RuntimeError('Stop trigger not found in current state')
-        
-        self._current_state.remove_trigger(trigger, self._trigger_comparator)
-    
-        if branch.num_states() == 0:
-            stop_trigger = tp.create_trigger('stop')
-        elif self.try_merge_branch(branch, tp):
-            stop_trigger = TriggerPlaceholder.none().create_trigger('stop')
-        else:
-            self.append_branch(branch, tp, mark_stop)
-            stop_trigger = TriggerPlaceholder.next().create_trigger('stop')
-        
-        self._current_state.triggers.append(stop_trigger)
-    
-    def try_merge_branch(self, branch: LinearScriptPath, tp: TriggerPlaceholder) -> bool:
-        extended_branch = (LinearScriptPath()
-                .append_state(self._current_state.actions, TriggerPlaceholder.empty())
-                .append_path(branch, tp))
-
-        merge_result = self._find_optimal_merge_path(extended_branch)
-        if merge_result is None:
-            return False
+        complete_threads = []
+        state_queue: list[tuple[State, ConvoThread, set[State]]] = [
+            (start_state, ConvoThread().append_state(start_state.actions, TriggerPlaceholder.none(), **start_state.attrs, is_start=True), set())
+        ]
 
-        self._perform_merge(merge_result)
-        return True
+        while len(state_queue):
+            current_state, thread, processed_states = state_queue.pop(0)
 
-    def append_branch(self, branch: LinearScriptPath, tp: TriggerPlaceholder, mark_stop: bool = False) -> None:
-        for state, prev_trigger in branch.iter_states(with_prev_trigger=True):
-            state_tp = tp if prev_trigger is None else TriggerPlaceholder.from_trigger(prev_trigger)
-            self.append_state(state.actions, state_tp, **state.kwargs)
+            if current_state in processed_states:
+                continue
+            if current_state.name == 'stop':
+                complete_threads.append(thread)
+                continue
 
-        if mark_stop:
-            return self
-        
-        # Create loopback
-        loopback_trigger = TriggerPlaceholder.default().create_trigger(self._current_state.name)
-        if self._current_state.find_trigger(loopback_trigger, self._trigger_comparator) is None:
-            self._current_state.triggers.append(loopback_trigger)
+            next_subthreads: list[tuple[Trigger, ConvoThread, State]] = []
 
-        return self
+            for trigger in current_state.triggers:
+                state = self._states[trigger.state_name]
+                state_attrs = {**state.attrs, 'is_start': True} if state.name == 'start' else {**state.attrs, 'is_stop': True} if state.name == 'stop' else state.attrs
+                subthread_states = ConvoThread().append_state(state.actions, TriggerPlaceholder.none(), **state_attrs)
+
+                while state.find_trigger(TriggerPlaceholder.next(), self._trigger_matcher) is not None:
+                    prev_trigger = state.triggers[0]
+                    state = self._states[prev_trigger.state_name]
+                    state_attrs = {**state.attrs, 'is_start': True} if state.name == 'start' else {**state.attrs, 'is_stop': True} if state.name == 'stop' else state.attrs
+                    subthread_states.append_state(state.actions, TriggerPlaceholder.from_trigger(prev_trigger), **state_attrs)
+                
+                if state is not current_state:
+                    # Trigger doesn't lead to loopback
+                    next_subthreads.append((trigger, subthread_states, state))
+                    continue
+
+                # Trigger leads to a loopback
+                for subthread_state, prev_trigger in subthread_states.iter_states(with_prev_trigger=True):
+                    if prev_trigger.is_none():
+                        prev_trigger = trigger
+                    thread.append_state(subthread_state.actions, TriggerPlaceholder.from_trigger(prev_trigger), **subthread_state.attrs)
 
-    def _find_optimal_merge_path(self, branch: LinearScriptPath) -> Optional[PathMergeResult]:
-        potential_merge_points = self._find_state(actions=branch.get_last_state().actions, many=True)
-        best_merge_result = None
+            processed_states.add(current_state)
+            
+            for trigger, subthread_states, state in next_subthreads:
+                next_thread = thread.copy()
+
+                for subthread_state, prev_trigger in subthread_states.iter_states(with_prev_trigger=True):
+                    if prev_trigger.is_none():
+                        prev_trigger = trigger
+                    next_thread.append_state(subthread_state.actions, TriggerPlaceholder.from_trigger(prev_trigger), **subthread_state.attrs)
+                
+                state_queue.append((state, next_thread, processed_states.copy()))
 
-        for merge_point in potential_merge_points:
-            potential_merge_paths = self._find_paths(self._current_state, merge_point, many=True)
+        return complete_threads
 
-            for base_path in potential_merge_paths:
-                merge_result = self._merge_strategy.merge(base_path, branch)
+    def merge_graph(self, graph: ConvoGraph) -> ConvoGraph:
+        result = self
 
-                if best_merge_result is None or len(merge_result.merged_states_mapping) > len(best_merge_result.merged_states_mapping):
-                    best_merge_result = merge_result
-        
-        return best_merge_result
+        for thread in graph.to_threads():
+            result = result.merge_thread(thread)
+
+        return result
     
-    def _perform_merge(self, merge_result: PathMergeResult):
-        current_base_state = self._current_state
-        base_state = merge_result.base_path.pop_first_state()
-
-        for state, prev_trigger in merge_result.merge_path.iter_states(with_prev_trigger=True):
-            if state.name not in merge_result.merged_states_mapping:
-                # The state is not in base path (existing part of script) and should be appended
-                self.append_state(state.actions, TriggerPlaceholder.from_trigger(prev_trigger), **state.kwargs)
-            else:
-                # The state should be merged to existing state
+    def compare(self, other: ConvoGraph) -> bool:
+        state_queue = [(self._states['start'], other.find_state(name='start'))]
+        processed_states = set()
 
-                while base_state.name != merge_result.merged_states_mapping[state.name]:
-                    current_base_trigger = current_base_state.find_trigger(TriggerPlaceholder.from_trigger(base_state.triggers[0]), self._trigger_comparator)
-                    current_base_state = self._states[current_base_trigger.state_name]
-                    current_base_state.kwargs.update(base_state.kwargs)
-                    base_state = merge_result.base_path.pop_first_state()
+        while len(state_queue):
+            state1, state2 = state_queue.pop(0)
+
+            if state1 in processed_states:
+                continue
+            if (state1.name == 'start') ^ (state2.name == 'start'):
+                return False
+            if (state1.name == 'stop') ^ (state2.name == 'stop'):
+                return False
+            if state1.attrs != state2.attrs:
+                return False
+            if not self._action_matcher.match(state1.actions, state2.actions):
+                return False
+            if len(state1.triggers) != len(state2.triggers):
+                return False
+            
+            for trigger1 in state1.triggers:
+                trigger2 = state2.find_trigger(TriggerPlaceholder.from_trigger(trigger1), self._trigger_matcher)
                 
-                if prev_trigger is not None:
-                    self.move_to_state(current_base_state.name, TriggerPlaceholder.from_trigger(prev_trigger), **base_state.kwargs)
+                if trigger2 is None:
+                    return False
+                
+                state_queue.append((self._states[trigger1.state_name], other.find_state(name=trigger2.state_name)))
+                
+            processed_states.add(state1)
+
+        return True
 
     # Export section
 
-    def to_list(self) -> list:
+    def to_states_list(self) -> list:
+        stop_state = self._states.pop('stop')
+        self._states['stop'] = stop_state
         return [state.to_dict() for state in self._states.values()]
     
-    def to_yaml(self, fp: str | TextIO) -> None:
+    def to_yaml(self, fp: Union[str, TextIO]) -> None:
         if isinstance(fp, str):
             if not fp.endswith('.yml') :
                 fp += '.yml'
             dir = os.path.dirname(fp)
             if not os.path.exists(dir):
                 os.makedirs(dir)
             fp = open(fp, 'w', encoding='utf-8')
 
-        script_list = self.to_list()
-        yaml.safe_dump(script_list, fp, sort_keys=False, encoding='utf-8')
+        state_list = self.to_states_list()
+        yaml.safe_dump(state_list, fp, sort_keys=False, encoding='utf-8')
         fp.close()
 
     # Import section
 
     @classmethod
-    def from_list(cls, states_list: list) -> Script:
+    def from_states_list(
+        cls, 
+        states_list: list[dict], 
+        convo_name: Optional[str] = None,
+        convo_description: Optional[str] = None,
+        nlp: Optional[str] = None,
+        action_matcher: Optional[ActionMatcher] = None, 
+        trigger_matcher: Optional[TriggerValueMatcher] = None,
+        use_uuid: Optional[bool] = None
+    ) -> ConvoGraph:
         states = {
             state_dict['name']: State.from_dict(state_dict)
             for state_dict in states_list
         }
 
-        script = cls(states=states)
-        return script
+        if action_matcher is None:
+            action_matcher = SimpleActionMatcher()
+        if trigger_matcher is None:
+            trigger_matcher = SimpleTriggerValueMatcher()
+        if use_uuid is None:
+            use_uuid = True
+
+        graph = cls(action_matcher, trigger_matcher, states, convo_name=convo_name, convo_description=convo_description, nlp=nlp, use_uuid=use_uuid)
+        return graph
 
     @classmethod
     def from_file(
         cls, 
-        fp: str | TextIO, 
-        text_script_parser: Optional[ScriptParser] = None, 
-        action_comparator: Optional[ActionMatcher] = None,
+        fp: Union[str, TextIO], 
         convo_name: Optional[str] = None,
         convo_description: Optional[str] = None,
-        base_author: str = 'teacher'
-    ) -> Script:
+        nlp: Optional[str] = None,
+        text_script_parser: Optional[ScriptParser] = None, 
+        base_author: Optional[str] = None,
+        action_matcher: Optional[ActionMatcher] = None,
+        trigger_matcher: Optional[TriggerValueMatcher] = None,
+        use_uuid: Optional[bool] = None
+    ) -> ConvoGraph:
         if isinstance(fp, str) and (fp.endswith('.yml') or fp.endswith('.yaml')):
-            return cls.from_yaml_file(fp)
+            return cls.from_yaml_file(fp, action_matcher, trigger_matcher, use_uuid)
         else:
             # Assume text file by default
-            if text_script_parser is None:
-                text_script_parser = SimpleScriptParser()
-            if action_comparator is None:
-                action_comparator = SimpleActionComparator()
-            if convo_name is None:
-                convo_name = 'convo_name'
-            if convo_description is None:
-                convo_description = ''
-
-            return cls.from_text_file(fp, text_script_parser, action_comparator, convo_name, convo_description, base_author)
+            return cls.from_text_file(fp, convo_name, convo_description, nlp, text_script_parser, base_author, action_matcher, trigger_matcher, use_uuid)
         
     @classmethod
-    def from_yaml_file(cls, fp: str | TextIO):
+    def from_yaml_file(
+        cls, 
+        fp: Union[str, TextIO], 
+        action_matcher: Optional[ActionMatcher] = None,
+        trigger_matcher: Optional[TriggerValueMatcher] = None, 
+        use_uuid: Optional[bool] = None
+    ) -> ConvoGraph:
         if isinstance(fp, str): 
             fp = open(fp, 'r', encoding='utf-8')
 
         script_list = yaml.safe_load(fp)
         fp.close()
-        return cls.from_list(script_list)
+        return cls.from_states_list(script_list, action_matcher, trigger_matcher, use_uuid=use_uuid)
     
     @classmethod
     def from_text_file(
         cls, 
-        fp: str | TextIO, 
-        text_script_parser: ScriptParser, 
-        action_comparator: ActionMatcher,
-        convo_name: str,
-        convo_description: str,
-        base_author: str
-    ) -> Script:
+        fp: Union[str, TextIO], 
+        convo_name: Optional[str] = None,
+        convo_description: Optional[str] = None,
+        nlp: Optional[str] = None,
+        script_parser: Optional[ScriptParser] = None, 
+        base_author: Optional[str] = None,
+        action_matcher: Optional[ActionMatcher] = None,
+        trigger_matcher: Optional[TriggerValueMatcher] = None,
+        use_uuid: Optional[bool] = None
+    ) -> ConvoGraph:
         if isinstance(fp, str): 
             fp = open(fp, encoding='utf-8')
 
         raw_lines = fp.readlines()
         fp.close()
 
-        # Build script
-        script = cls(action_comparator=action_comparator, convo_name=convo_name, convo_description=convo_description)
-        branch = LinearScriptPath()
-        tp = TriggerPlaceholder.next()
-        script_lines = text_script_parser.parse_lines(raw_lines)
+        return cls.from_script_lines(
+            raw_lines,
+            convo_name,
+            convo_description,
+            nlp,
+            script_parser,
+            base_author,
+            action_matcher, 
+            trigger_matcher,
+            use_uuid
+        )
+    
+    @classmethod
+    def from_script_lines(
+        cls,
+        text_lines: list[str],
+        convo_name: Optional[str] = None,
+        convo_description: Optional[str] = None,
+        nlp: Optional[str] = None,
+        script_parser: Optional[ScriptParser] = None,
+        base_author: Optional[str] = None,
+        action_matcher: Optional[ActionMatcher] = None,
+        trigger_matcher: Optional[TriggerValueMatcher] = None,
+        use_uuid: Optional[bool] = None
+    ) -> ConvoGraph:
+        if convo_name is None:
+            convo_name = 'convo_name'
+        if convo_description is None:
+            convo_description = 'empty'
+        if nlp is None:
+            nlp = 'case_insensitive'
+        if script_parser is None:
+            script_parser = SimpleScriptParser()
+        if base_author is None:
+            base_author = 'teacher'
+        if action_matcher is None:
+            action_matcher = SimpleActionMatcher()
+        if trigger_matcher is None:
+            trigger_matcher = SimpleTriggerValueMatcher()
+        if use_uuid is None:
+            use_uuid = True
+
+        script_lines = script_parser.parse_lines(text_lines)
+        
+        graph = cls(action_matcher, trigger_matcher, convo_name=convo_name, convo_description=convo_description, nlp=nlp, use_uuid=use_uuid)
+        graph_start_state = graph.find_state(name='start')
+        graph_stop_state = graph.find_state(name='stop')
+
+        thread = ConvoThread().append_state(graph_start_state.actions, TriggerPlaceholder.none(), **graph_start_state.attrs, is_start=True)
+        tp = None
 
         for line in script_lines:
             if line.author == base_author:
                 action = Action(line.text, line.lang_group)
-                branch.append_state(action, TriggerPlaceholder.next())
+                thread = thread.append_state(action, tp or TriggerPlaceholder.next())
+                tp = None
             else:
-                script.merge_or_append_branch(branch, tp)
-                branch = LinearScriptPath()
                 tp = TriggerPlaceholder(line.text, line.lang_group)
 
-        script.merge_or_append_branch(branch, tp, mark_stop=True)
-
-        return script
-
+        thread = thread.append_state(graph_stop_state.actions, tp or TriggerPlaceholder.next(), **graph_stop_state.attrs, is_stop=True)
+        return graph.merge_thread(thread)
 
-def read_file(
-    fp: str | TextIO, 
-    text_script_parser: Optional[ScriptParser] = None, 
-    action_comparator: Optional[ActionMatcher] = None,
-    convo_name: Optional[str] = None,
-    convo_description: Optional[str] = None,
-    base_author: str = 'teacher',
-) -> Script:
-    return Script.from_file(
-        fp, 
-        text_script_parser=text_script_parser, 
-        action_comparator=action_comparator, 
-        convo_name=convo_name,
-        convo_description=convo_description,
-        base_author=base_author
-    )
```

### Comparing `convomeld-0.1.1/src/convomerge/state.py` & `convomeld-0.1.2/src/convomeld/state.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional, Union
 
 if TYPE_CHECKING:
-    from convomerge.matchers import TriggerValueMatcher
+    from convomeld.matchers import TriggerValueMatcher
 
 
 class Action:
     def __init__(self, value: str, group_name: str) -> None:
         self.value = value
         self.group_name = group_name
 
@@ -22,14 +22,15 @@
 
         return Action(value, group_name)
 
 
 class Trigger:
     value_default = '__default__'
     value_next = '__next__'
+    value_timeout = '__timeout__'
     value_empty = ''
     value_none = None
 
     default_group_name = 'en'
 
     def __init__(self, value: str, state_name: str, group_name: str) -> None:
         self.value = value
@@ -51,21 +52,19 @@
     
     def is_default(self) -> bool:
         return self.value == Trigger.value_default
 
     def is_next(self) -> bool:
         return self.value == Trigger.value_next
     
-    @classmethod
-    def default(cls, state_name: str) -> Trigger:
-        return cls(cls.value_default, state_name, cls.default_group_name)
+    def is_none(self) -> bool:
+        return self.value == Trigger.value_none
     
-    @classmethod
-    def next(cls, state_name: str) -> Trigger:
-        return cls(cls.value_next, state_name, cls.default_group_name)
+    def is_timeout(self) -> bool:
+        return self.value == Trigger.value_timeout
 
 
 class TriggerPlaceholder:
     def __init__(self, value: str, group_name: str) -> None:
         self.value = value
         self.group_name = group_name
 
@@ -91,125 +90,134 @@
         return cls(Trigger.value_default, Trigger.default_group_name)
     
     @classmethod
     def next(cls) -> TriggerPlaceholder:
         return cls(Trigger.value_next, Trigger.default_group_name)
     
     @classmethod
+    def timeout(cls) -> TriggerPlaceholder:
+        return cls(Trigger.value_timeout, Trigger.default_group_name)
+    
+    @classmethod
     def from_trigger(cls, trigger: Trigger) -> TriggerPlaceholder:
         return cls(trigger.value, trigger.group_name)
 
 
 class State:
-    def __init__(self, name: str, actions: Optional[list[Action]] = None, triggers: Optional[list[Trigger]] = None, **kwargs) -> None:
+    def __init__(self, name: str, actions: Optional[list[Action]] = None, triggers: Optional[list[Trigger]] = None, **attrs) -> None:
         self.name = name
-        self.kwargs = kwargs
+        self.attrs = attrs
 
         if actions is None:
             self.actions: list[Action] = []
         else:
             self.actions: list[Action] = [action.copy() for action in actions]
 
         if triggers is None:
             self.triggers: list[Trigger] = []
         else:
             self.triggers: list[Trigger] = [trigger.copy() for trigger in triggers]
         
     def __repr__(self) -> str:
-        return f'State(name={repr(self.name)}, actions={repr(self.actions)}, triggers={repr(self.triggers)}, **{repr(self.kwargs)})'
+        return f'State(name={repr(self.name)}, actions={repr(self.actions)}, triggers={repr(self.triggers)}, **{repr(self.attrs)})'
     
     def __str__(self) -> str:
         return f'State("{" ".join(map(lambda a: a.value, self.actions))}", name={self.name})'
     
-    def copy(self, name: Optional[str] = None, actions: Optional[list[Action]] = None, triggers: Optional[list[Trigger]] = None, **kwargs) -> State:
+    def copy(self, name: Optional[str] = None, actions: Optional[list[Action]] = None, triggers: Optional[list[Trigger]] = None, **attrs) -> State:
         if name is None:
             name = self.name
         if actions is None:
             actions = self.actions
         if triggers is None:
             triggers = self.triggers
 
-        kwargs = {**self.kwargs, **kwargs}
+        attrs = {**self.attrs, **attrs}
 
-        new_state = State(name, **kwargs)
+        new_state = State(name, **attrs)
         new_state.actions =  [action.copy() for action in actions]
         new_state.triggers = [trigger.copy() for trigger in triggers]
         return new_state
     
-    def find_trigger(self, target: Union[Trigger, TriggerPlaceholder], comparator: TriggerValueMatcher, index: bool = False) -> Optional[Union[Trigger, int]]:
+    def find_trigger(self, target: Union[Trigger, TriggerPlaceholder], matcher: TriggerValueMatcher, index: bool = False, ensure_unique_state_name: bool = False) -> Optional[Union[Trigger, int]]:
         if isinstance(target, Trigger):
             target_value = target.value
             target_group_name = target.group_name
             target_state_name = target.state_name
         elif isinstance(target, TriggerPlaceholder):
             target_value = target.value
             target_group_name = target.group_name
             target_state_name = None
 
         for i, trigger in enumerate(self.triggers):
             if (
                 trigger.group_name == target_group_name
                 and (
                     trigger.value == target_value
-                    or comparator.match(trigger.value, target_value)
+                    or matcher.match(trigger.value, target_value)
                 )
             ):
                 if target_state_name is not None and trigger.state_name != target_state_name:
-                    raise RuntimeError('Inconsistent state name for trigger')
+                    if ensure_unique_state_name:
+                        raise RuntimeError(f'Inconsistent state name for trigger {repr(target)}')
+                    else:
+                        continue
                 
                 if index:
                     return i
                 else:
                     return trigger.copy()
             
         return None
     
-    def remove_trigger(self, target: Union[Trigger, TriggerPlaceholder], comparator: TriggerValueMatcher) -> Optional[Trigger]:
-        index = self.find_trigger(target, comparator, index=True)        
+    def remove_trigger(self, target: Union[Trigger, TriggerPlaceholder], matcher: TriggerValueMatcher) -> Optional[Trigger]:
+        index = self.find_trigger(target, matcher, index=True)        
         return self.triggers.pop(index).copy() if index is not None else None
     
     # Export section
 
-    def to_dict(self) -> dict:
+    def to_dict(self, use_unique_triggers: bool = True) -> dict:
         state_dict = {
             'name': self.name,
-            **self.kwargs,
+            **self.attrs,
         }
 
-        if len(self.actions):
-            actions_dict: dict[str, list[str]] = {}
-
-            for action in self.actions:
-                actions_dict.setdefault(action.group_name, [])
-                actions_dict[action.group_name].append(action.value)
+        # if len(self.actions):
+        actions_dict = state_dict['actions'] = {}
 
-            state_dict['actions'] = actions_dict
-        
-        if len(self.triggers):
-            triggers_dict: dict[str, dict[str, str]] = {}
-
-            for trigger in self.triggers:
-                triggers_dict.setdefault(trigger.group_name, {})
+        for action in self.actions:
+            actions_dict.setdefault(action.group_name, [])
+            actions_dict[action.group_name].append(action.value)
+
+        # if len(self.triggers):
+        state_dict['triggers'] = triggers_dict = {}
+
+        for trigger in self.triggers:
+            triggers_dict.setdefault(trigger.group_name, {})
+            if use_unique_triggers:
                 triggers_dict[trigger.group_name][trigger.value] = trigger.state_name
-
-            state_dict['triggers'] = triggers_dict
+            else:
+                triggers_dict[trigger.group_name].setdefault(trigger.value, [])
+                triggers_dict[trigger.group_name][trigger.value].append(trigger.state_name)
 
         return state_dict
     
     # Import section
 
     @classmethod
     def from_dict(cls, state_dict: dict) -> State:
+        state_dict = state_dict.copy()
         actions = state_dict.pop('actions', {})
         triggers = state_dict.pop('triggers', {})
 
         state = cls(name=state_dict.pop('name'), **state_dict)
             
         for action_group_name, action_group in actions.items():
             for action_value in action_group:
                 state.actions.append(Action(action_value, action_group_name))
         
         for trigger_group_name, trigger_group in triggers.items():
             for trigger_value, next_state_name in trigger_group.items():
                 state.triggers.append(Trigger(trigger_value, next_state_name, trigger_group_name))
             
-        return state
+        return state
+
```

### Comparing `convomeld-0.1.1/PKG-INFO` & `convomeld-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: convomeld
-Version: 0.1.1
+Version: 0.1.2
 Summary: Parse text scripts or chatbot message logs and merge conversation graphs (Convographs)
 License: AGPL-3.0-or-later
 Author: Ruslan Borysov
 Author-email: borysov.ruslan98@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0)
+Requires-Dist: openpyxl
 Description-Content-Type: text/markdown
 
 # Convomeld
 
 Tools for composing, validating, merging and simplifying the graph data structures that define the a conversational agent's behavior - a program that can be run by a conversation manager to interact with humans.
```

