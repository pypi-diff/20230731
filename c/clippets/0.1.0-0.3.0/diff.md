# Comparing `tmp/clippets-0.1.0.tar.gz` & `tmp/clippets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clippets-0.1.0.tar", last modified: Sun Jul 30 14:33:11 2023, max compression
+gzip compressed data, was "clippets-0.3.0.tar", last modified: Mon Jul 31 20:25:18 2023, max compression
```

## Comparing `clippets-0.1.0.tar` & `clippets-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/
--rw-rw-r--   0 paul      (1000) paul      (1000)    11357 2023-07-18 14:12:00.000000 clippets-0.1.0/LICENSE
--rw-rw-r--   0 paul      (1000) paul      (1000)     1508 2023-07-30 14:33:11.441364 clippets-0.1.0/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      842 2023-07-30 14:30:22.000000 clippets-0.1.0/README.md
--rw-rw-r--   0 paul      (1000) paul      (1000)     2999 2023-07-30 12:17:39.000000 clippets-0.1.0/pyproject.toml
--rw-rw-r--   0 paul      (1000) paul      (1000)      126 2023-07-30 14:33:11.441364 clippets-0.1.0/setup.cfg
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.425364 clippets-0.1.0/src/
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/src/clippets/
--rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-07-18 14:12:00.000000 clippets-0.1.0/src/clippets/__init__.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3032 2023-07-28 11:17:28.000000 clippets-0.1.0/src/clippets/clippets.css
--rw-rw-r--   0 paul      (1000) paul      (1000)      554 2023-07-18 14:12:00.000000 clippets-0.1.0/src/clippets/colors.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    43405 2023-07-30 09:22:22.000000 clippets-0.1.0/src/clippets/core.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     4185 2023-07-18 14:21:39.000000 clippets-0.1.0/src/clippets/help.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)     2288 2023-07-28 09:13:25.000000 clippets-0.1.0/src/clippets/linux.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    17787 2023-07-30 09:34:41.000000 clippets-0.1.0/src/clippets/markup.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1656 2023-07-25 14:08:25.000000 clippets-0.1.0/src/clippets/platform.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    27485 2023-07-30 09:08:02.000000 clippets-0.1.0/src/clippets/snippets.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8599 2023-07-29 09:26:25.000000 clippets-0.1.0/src/clippets/widgets.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    10053 2023-07-25 14:17:13.000000 clippets-0.1.0/src/clippets/win.py
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/src/clippets.egg-info/
--rw-rw-r--   0 paul      (1000) paul      (1000)     1508 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/PKG-INFO
--rw-rw-r--   0 paul      (1000) paul      (1000)      722 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/SOURCES.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/dependency_links.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       78 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/entry_points.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)       34 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/requires.txt
--rw-rw-r--   0 paul      (1000) paul      (1000)        9 2023-07-30 14:33:11.000000 clippets-0.1.0/src/clippets.egg-info/top_level.txt
-drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-30 14:33:11.441364 clippets-0.1.0/tests/
--rw-rw-r--   0 paul      (1000) paul      (1000)     7079 2023-07-30 09:16:09.000000 clippets-0.1.0/tests/test_clipboard.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     8905 2023-07-29 18:33:32.000000 clippets-0.1.0/tests/test_editing.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    12639 2023-07-29 12:25:52.000000 clippets-0.1.0/tests/test_filtering.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     1492 2023-07-29 09:04:39.000000 clippets-0.1.0/tests/test_help.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3402 2023-07-27 10:49:29.000000 clippets-0.1.0/tests/test_kb_selection.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     3683 2023-07-29 12:00:55.000000 clippets-0.1.0/tests/test_keywords.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     9956 2023-07-30 09:08:31.000000 clippets-0.1.0/tests/test_load_save.py
--rw-rw-r--   0 paul      (1000) paul      (1000)     2384 2023-07-29 13:06:52.000000 clippets-0.1.0/tests/test_misc_ui.py
--rw-rw-r--   0 paul      (1000) paul      (1000)    18022 2023-07-28 14:41:19.000000 clippets-0.1.0/tests/test_moving.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-31 20:25:18.884306 clippets-0.3.0/
+-rw-rw-r--   0 paul      (1000) paul      (1000)    11357 2023-07-18 14:12:00.000000 clippets-0.3.0/LICENSE
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1458 2023-07-31 20:25:18.884306 clippets-0.3.0/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      792 2023-07-31 20:23:52.000000 clippets-0.3.0/README.md
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2999 2023-07-31 20:23:15.000000 clippets-0.3.0/pyproject.toml
+-rw-rw-r--   0 paul      (1000) paul      (1000)      126 2023-07-31 20:25:18.884306 clippets-0.3.0/setup.cfg
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-31 20:25:18.876306 clippets-0.3.0/src/
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-31 20:25:18.884306 clippets-0.3.0/src/clippets/
+-rw-rw-r--   0 paul      (1000) paul      (1000)        0 2023-07-18 14:12:00.000000 clippets-0.3.0/src/clippets/__init__.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2841 2023-07-31 20:18:16.000000 clippets-0.3.0/src/clippets/clippets.css
+-rw-rw-r--   0 paul      (1000) paul      (1000)      554 2023-07-18 14:12:00.000000 clippets-0.3.0/src/clippets/colors.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    45456 2023-07-31 19:55:15.000000 clippets-0.3.0/src/clippets/core.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     4185 2023-07-18 14:21:39.000000 clippets-0.3.0/src/clippets/help.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2288 2023-07-28 09:13:25.000000 clippets-0.3.0/src/clippets/linux.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    17787 2023-07-30 09:34:41.000000 clippets-0.3.0/src/clippets/markup.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1656 2023-07-25 14:08:25.000000 clippets-0.3.0/src/clippets/platform.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    29888 2023-07-31 19:38:35.000000 clippets-0.3.0/src/clippets/snippets.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    10348 2023-07-31 20:20:46.000000 clippets-0.3.0/src/clippets/widgets.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    10053 2023-07-25 14:17:13.000000 clippets-0.3.0/src/clippets/win.py
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-31 20:25:18.884306 clippets-0.3.0/src/clippets.egg-info/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1458 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/PKG-INFO
+-rw-rw-r--   0 paul      (1000) paul      (1000)      744 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        1 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       78 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/entry_points.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)       34 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/requires.txt
+-rw-rw-r--   0 paul      (1000) paul      (1000)        9 2023-07-31 20:25:18.000000 clippets-0.3.0/src/clippets.egg-info/top_level.txt
+drwxrwxr-x   0 paul      (1000) paul      (1000)        0 2023-07-31 20:25:18.884306 clippets-0.3.0/tests/
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6909 2023-07-31 18:33:13.000000 clippets-0.3.0/tests/test_clipboard.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     8750 2023-07-31 19:41:01.000000 clippets-0.3.0/tests/test_editing.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    12470 2023-07-31 18:33:13.000000 clippets-0.3.0/tests/test_filtering.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     1492 2023-07-29 09:04:39.000000 clippets-0.3.0/tests/test_help.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3273 2023-07-31 19:50:34.000000 clippets-0.3.0/tests/test_kb_selection.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     3683 2023-07-29 12:00:55.000000 clippets-0.3.0/tests/test_keywords.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     9942 2023-07-31 11:13:11.000000 clippets-0.3.0/tests/test_load_save.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     2384 2023-07-29 13:06:52.000000 clippets-0.3.0/tests/test_misc_ui.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)     6368 2023-07-31 20:09:27.000000 clippets-0.3.0/tests/test_monitor.py
+-rw-rw-r--   0 paul      (1000) paul      (1000)    18022 2023-07-28 14:41:19.000000 clippets-0.3.0/tests/test_moving.py
```

### Comparing `clippets-0.1.0/LICENSE` & `clippets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/PKG-INFO` & `clippets-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clippets
-Version: 0.1.0
+Version: 0.3.0
 Summary: UI to build up clipboard content from (rich) text snippets.
 Author-email: Paul Ollis <paul@cleversheep.org>
 Project-URL: Homepage, https://github.com/paul-ollis/clippets
 Project-URL: Bug Tracker, https://github.com/paul-ollis/clippets/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -30,13 +30,12 @@
 - It has a fairly comprehensive test suite.
 - I hope that crashes should be rare (backup files are maintained to minimise
   the impact).
 
 However:
 
 - It still needs more tests.
-- There are areas of mouse and keyboard support that beg imrpovement.
+- There are areas of mouse and keyboard support that beg improvement.
 - Some desirable features are obviously missing, such as:
 
   - There is no proper documentation beyound the built-in help.
   - It does not yet work on MacOS.
-  - It should monitor the input file for changes.
```

### Comparing `clippets-0.1.0/README.md` & `clippets-0.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -13,13 +13,12 @@
 - It has a fairly comprehensive test suite.
 - I hope that crashes should be rare (backup files are maintained to minimise
   the impact).
 
 However:
 
 - It still needs more tests.
-- There are areas of mouse and keyboard support that beg imrpovement.
+- There are areas of mouse and keyboard support that beg improvement.
 - Some desirable features are obviously missing, such as:
 
   - There is no proper documentation beyound the built-in help.
   - It does not yet work on MacOS.
-  - It should monitor the input file for changes.
```

### Comparing `clippets-0.1.0/pyproject.toml` & `clippets-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "clippets"
-version = "0.1.0"
+version = "0.3.0"
 authors = [
   { name="Paul Ollis", email="paul@cleversheep.org" },
 ]
 description = "UI to build up clipboard content from (rich) text snippets."
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
```

### Comparing `clippets-0.1.0/src/clippets/clippets.css` & `clippets-0.3.0/src/clippets/clippets.css`

 * *Files 2% similar despite different names*

```diff
@@ -123,37 +123,27 @@
     border: solid $primary-lighten-3;
 }
 
 #view:focus {
     border: tall $accent;
 }
 
-#dialog {
-    grid-size: 4;
-    grid-gutter: 1 2;
-    grid-rows: 1 4;
-    padding: 0 1;
-    width: auto;
-    height: auto;
-    border: thick $background 80%;
-    background: $surface;
-}
 
 #question {
     height: 1;
     width: 1fr;
     column-span: 4;
     content-align: center middle;
 }
 
 Button {
     width: 100%;
 }
 
-SnippetMenu {
+.popup {
     align: center middle;
 }
 
 /* The help text. */
 .banner {
     content-align: center middle;
     padding: 0 0 0 0;
```

### Comparing `clippets-0.1.0/src/clippets/colors.py` & `clippets-0.3.0/src/clippets/colors.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets/core.py` & `clippets-0.3.0/src/clippets/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from __future__ import annotations
 
 import argparse
 import asyncio
 import collections
 import itertools
 import re
-import sys
 import subprocess
+import sys
 import threading
+import time
 from contextlib import asynccontextmanager, suppress
 from dataclasses import dataclass
 from functools import partial, wraps
 from typing import AsyncGenerator, Callable, ClassVar, Iterable, TYPE_CHECKING
 
 from rich.text import Text
 from textual._context import (
@@ -49,15 +50,15 @@
     SharedTempFile, get_editor_command, get_winpos, put_to_clipboard,
     terminal_title)
 from .snippets import (
     Group, PlaceHolder, Snippet, SnippetInsertionPointer, SnippetLike,
     id_of_element as id_of)
 from .widgets import (
     MyFooter, MyInput, MyLabel, MyMarkdown, MyTag, MyText, MyVerticalScroll,
-    SnippetMenu)
+    SnippetMenu, FileChangedMenu)
 
 if TYPE_CHECKING:
     from textual.message import Message
     from textual.widget import Widget
     from textual.events import Event
 
 HL_GROUP = ''
@@ -223,33 +224,36 @@
     if w:
         w.styles.margin = (0, 1, 0, (snippet.depth() - 1) * 4)
     return w
 
 
 async def populate(q, walk, query):
     """Background task to populate widgets."""
+    yield_period = 0.01
+    sleep_period = 0.01
+
     while True:
         while q.qsize() > 1:
             cmd = await q.get()                              # pragma: no cover
         cmd = await q.get()
         if cmd is None:
             break
 
-        n = 0
+        a = time.time()
         for snippet in walk():
             if q.qsize() > 0:
                 break                                        # pragma: no cover
             if snippet.dirty:
                 w = query(snippet)
                 if w is not None:
                     w.update(snippet.marked_text)
                     snippet.dirty = False
-                    n += 1
-                    if n % 30 == 0:
-                        await asyncio.sleep(0.5)             # pragma: no cover
+                    if (time.time() - a) >= yield_period:
+                        await asyncio.sleep(sleep_period)
+                        a = time.time()
 
 
 def populate_fg(walk, query):
     """Populate widgets."""
     for snippet in walk():
         if snippet.dirty:
             w = query(snippet)
@@ -300,29 +304,29 @@
             if name != '_default':
                 self.MODES.pop(name)
         self.chosen = []
         self.collapsed = set()
         self.edited_text = ''
         self.filter = Matcher('')
         self.groups = groups
-        self.hidden_bindings = set()
         self.hover_uid = None
         self._selected_snippets = [id_of(self.groups.first_snippet())]
         self.move_info = None
         self.redo_buffer = collections.deque(maxlen=20)
         self.sel_order = False
         self.undo_buffer = collections.deque(maxlen=20)
         self.lookup = {}
         self.walk = partial(self.groups.walk, backwards=False)
         self.walk_groups = partial(self.walk, predicate=is_group)
         self.resolver_q = asyncio.Queue()
         self.populater_q = asyncio.Queue()
 
     async def on_exit_app(self, _event):
         """Clean up when exiting the application."""
+        await self.loader.stop_monitoring()
         if self.resolver:
             self.resolver_q.put_nowait(None)
             await self.resolver
         if self.populater:
             self.populater_q.put_nowait(None)
             await self.populater
 
@@ -343,21 +347,21 @@
         """Find the widget for a given element."""
         uid = el.uid()
         if uid not in self.lookup:
             self.lookup[uid] = self.query_one(f'#{el.uid()}')
         return self.lookup[uid]
 
     ## Management of dynanmic display features.
-    def selectable_widgets(self) -> list[Widget, ...]:
-        """Create a list of selectable widgets.
+    def selectable_widgets(self) -> tuple[list[Widget], list[Widget]]:
+        """Create a lists of postential and currently selectable widgets.
 
-        To be selectable, a snippet's widget must be visible.
+        To be currently selectable, a snippet's widget must be visible.
         """
-        widgets = (self.find_widget(s) for s in self.walk_snippets())
-        return [w for w in widgets if w.display]
+        widgets = [self.find_widget(s) for s in self.walk_snippets()]
+        return [w for w in widgets if w.display], widgets
 
     def insertion_widgets(self) -> tuple[tuple[Snippet, Widget], ...]:
         """Create a tuple of widgets involved in insetion operations."""
         return tuple(
             (s, self.find_widget(s)) for s in self.walk_snippet_like())
 
     def set_visuals(self) -> None:
@@ -417,16 +421,22 @@
                 w = getattr(ev, 'snippet', None)
                 if w:
                     snippet = self.groups.find_element_by_uid(w.id)
                     if snippet:
                         self.action_start_moving_snippet(snippet.uid())
             elif not ev.meta:
                 self.on_left_click(ev)
-        elif ev.button == RIGHT_MOUSE_BUTTON and not ev.meta:
-            self.on_right_click(ev)
+        elif ev.button == RIGHT_MOUSE_BUTTON:
+            if ev.meta:                                      # pragma: no cover
+                # This can be useful for debugging.
+                w = getattr(ev, 'snippet', getattr(ev, 'group', None))
+                if w:
+                    print('CLICK ON', w.id)
+            else:
+                self.on_right_click(ev)
 
     def on_left_click(self, ev) -> None:
         """Process a mouse left-click."""
         if snippet := getattr(ev, 'snippet', None):
             self.push_undo()
             id_str = snippet.id
             if id_str in self.chosen:
@@ -463,25 +473,29 @@
             snippet = self.groups.find_element_by_uid(w.id)
             if snippet:
                 self.push_screen(SnippetMenu(id='snippet-menu'), on_close)
 
     ## Handling of keyboard operations.
     def fix_selection(self, *, kill_filter: bool = False):
         """Update the keyboard selected focus when widgets get hidden."""
-        # Do nothing is the filter input is focusses and should remain so.
+        valid_widgets, widgets = self.selectable_widgets()
+        if self.handle_no_snippets_for_selection(widgets):
+            return
+
+        # Do nothing if the filter input is focusses and should remain so.
         if self._selected_snippets[-1] == 'filter':
             if kill_filter:
                 self._selected_snippets.pop()
             else:
                 return
 
         # If the current selection is ``None`` then we cannot fix the
         # selection.
         if self.selected_snippet is None:
-            if not self.selectable_widgets():
+            if not valid_widgets:
                 return
             self._selected_snippets.pop()
 
         # If there is selection history (from previous fix-ups) try to reselect
         # the oldest entry in the history.
         for i, wid in enumerate(self._selected_snippets):
             if i > 0 and wid is not None:
@@ -492,17 +506,38 @@
                     self.screen.set_focus(None)
                     return
 
         # The selection history could not be used so find the best alternative
         # snippet to select, saving the currently selection in the history.
         self.fix_to_next_nearest_snippet()
 
+    def handle_no_snippets_for_selection(
+            self, potential_widgets: list[Widget]) -> bool:
+        """Handle selction for the special case of no snippets all."""
+        if not potential_widgets:
+            self._selected_snippets[:] = [None]
+        return not potential_widgets
+
     def fix_to_next_nearest_snippet(self):
-        """Move the snippet selection to the next nearest, if necessary."""
-        w = self.query_one(f'#{self.selected_snippet}')
+        """Move the snippet selection to the next nearest, if necessary.
+
+        This also handles the case when the selected snippet no longer exists;
+        for example after a file reload. In this case the first snippet is
+        selected.
+
+        Note that this *must not* be invoked when there are no snippets. Use
+        `handle_no_snippets_for_selection` appropriately.
+        """
+        try:
+            w = self.query_one(f'#{self.selected_snippet}')
+        except NoMatches:
+            w = self.find_widget(self.groups.first_snippet())
+            self._selected_snippets[:] = [w.id]
+            w.scroll_visible()
+
         if not w.display:
             k = self.action_select_move(inc=-1, dry_run=True)
             if k == 0:
                 k = self.action_select_move(inc=1, dry_run=False, push=True)
             else:
                 k = self.action_select_move(inc=-1, dry_run=False, push=True)
 
@@ -510,19 +545,19 @@
             if k < 0 and self._selected_snippets[-1] is not None:
                 self._selected_snippets.append(None)
 
     def action_select_move(
                 self, inc: int, *, dry_run: bool = False, push: bool = False,
             ) -> int:
         """Move the selection to the next available snippet."""
-        # Collect snippet widgets and those that are visible.
-        widgets = [self.find_widget(s) for s in self.walk_snippets()]
-        valid_widgets = [w for w in widgets if w.display]
-        valid_range = range(len(widgets))
+        valid_widgets, widgets = self.selectable_widgets()
+        if self.handle_no_snippets_for_selection(widgets):
+            return -1
 
+        valid_range = range(len(widgets))
         k = -1
         for i, w in enumerate(widgets):
             if w.id == self.selected_snippet:
                 k = i + inc
                 while k in valid_range and not widgets[k].display:
                     k += inc
                 break
@@ -649,29 +684,33 @@
                     s.extend(snippet.md_lines())
                     s.append('')
         if s:
             s.pop()
         return '\n'.join(s)
 
     ## Editing and duplicating snippets.
-    def rebuild_after_edits(self):
+    def rebuild(self):
         """Rebuild, refresh, *etc*. after changes to the snippets tree."""
-        self.backup_and_save()
         self.lookup.clear()
         self.screen.rebuild_tree_part()
         if self.resolver:
             self.resolver_q.put_nowait('rebuild')
         if self.populater:
             self.populater_q.put_nowait('pop')
         else:
             populate_fg(self.walk_snippets, self.find_widget)
 
         self.update_result()
         self.set_visuals()
 
+    def rebuild_after_edits(self):
+        """Rebuild, refresh, *etc*. after changes to the snippets tree."""
+        self.backup_and_save()
+        self.rebuild()
+
     def edit_snippet(self, id_str) -> None:
         """Invoke the user's editor on a snippet."""
         snippet = self.groups.find_element_by_uid(id_str)
         text = run_editor(snippet.text)
         if text.strip() != snippet.text.strip():
             snippet.set_text(text)
             self.rebuild_after_edits()
@@ -686,15 +725,15 @@
         self.rebuild_after_edits()
         w = self.find_widget(new_snippet)
         w.scroll_visible()
 
     def backup_and_save(self):
         """Create a new snippet file backup and then save."""
         snippets.backup_file(self.args.snippet_file)
-        snippets.save(self.args.snippet_file, self.groups)
+        self.loader.save(self.groups)
 
     ## Snippet position movement.
     def action_start_moving_snippet(self, id_str: str | None = None) -> None:
         """Start moving a snippet to a different position in the tree."""
         for i, _ in enumerate(self.walk_snippets()):
             if i == 1:
                 break
@@ -869,15 +908,16 @@
     # pylint: disable=too-many-instance-attributes
     TITLE = 'Comment snippet wrangler'
     CSS_PATH = 'clippets.css'
     SCREENS: ClassVar[dict] = {'help': HelpScreen()}
     id_to_focus: ClassVar[dict] = {'input': 'filter'}
 
     def __init__(self, args):
-        groups, title = snippets.load(args.snippet_file)
+        self.loader = snippets.Loader(args.snippet_file)
+        groups, title = self.loader.load()
         if title:
             self.TITLE = title                   # pylint: disable=invalid-name
         super().__init__(groups)
         self.args = args
         self.key_handler = KeyHandler(self)
         self.init_bindings()
         self.walk_snippets = partial(self.walk, is_snippet)
@@ -886,14 +926,25 @@
         self.populater = None
 
     def run(self, *args, **kwargs) -> int:                   # pragma: no cover
         """Wrap the standar run method, settin the terminal title."""
         with terminal_title('Snippet-wrangler'):
             return super().run()
 
+    def handle_file_changed(self):
+        """Handle when the current loaded file has changed."""
+        def on_close(v):
+            self.screen.set_focus(None)
+            if  v == 'load':
+                self.loader.load()
+                self.rebuild()
+                self.fix_selection()
+
+        self.push_screen(FileChangedMenu(id='file-changed-menu'), on_close)
+
     def context_name(self) -> str:
         """Provide a name identifying the current context."""
         if self.screen.id == 'main':
             if self.move_info is not None:
                 return 'moving'
             elif self.selected_snippet == 'filter':
                 return 'filter'
@@ -947,40 +998,45 @@
 
     def active_shown_bindings(self):
         """Provide a list of bindings used for the application Footer."""
         return self.key_handler.active_shown_bindings()
 
     def on_ready(self) -> None:
         """React to the DOM having been created."""
-        if self.args.sync_mode:
-            populate_fg(self.walk_snippets, self.find_widget)
-        else:
-            self.resolver = asyncio.create_task(resolve(
-                self.resolver_q, self.lookup, self.walk, self.query_one))
-            self.resolver_q.put_nowait('rebuild')
-            self.populater = asyncio.create_task(populate(
-                self.populater_q, self.walk_snippets, self.find_widget))
-            self.populater_q.put_nowait('pop')
-
+        self.start_population()
         self.screen.set_focus(None)
         self.set_visuals()
+        self.loader.start_monitoring(self.handle_file_changed)
 
     def action_show_help(self) -> None:
         """Show the help screen."""
         self.push_screen(HelpScreen(id='help'))
 
     async def on_key(self, event: Event) -> None:
         """Handle a top level key press."""
         await self.key_handler.handle_key(event)
         event.stop()
 
     def on_mount(self) -> None:
         """Perform app start-up actions."""
         self.dark = True
-        populate_fg(self.walk_snippets, self.find_widget)
+        self.start_population()
+
+    def start_population(self):
+        """Start the process of populating the snippet widgets."""
+        if self.args.sync_mode:
+            populate_fg(self.walk_snippets, self.find_widget)
+        else:
+            if not self.resolver:
+                self.resolver = asyncio.create_task(resolve(
+                    self.resolver_q, self.lookup, self.walk, self.query_one))
+                self.populater = asyncio.create_task(populate(
+                    self.populater_q, self.walk_snippets, self.find_widget))
+            self.resolver_q.put_nowait('rebuild')
+            self.populater_q.put_nowait('pop')
 
     @asynccontextmanager
     async def run_test(                                         # noqa: PLR0913
         self,
         *,
         headless: bool = True,
         size: tuple[int, int] | None = (80, 24),
```

### Comparing `clippets-0.1.0/src/clippets/help.txt` & `clippets-0.3.0/src/clippets/help.txt`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets/linux.py` & `clippets-0.3.0/src/clippets/linux.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets/markup.py` & `clippets-0.3.0/src/clippets/markup.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets/platform.py` & `clippets-0.3.0/src/clippets/platform.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets/snippets.py` & `clippets-0.3.0/src/clippets/snippets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Data structure used to store the snippet text."""
 from __future__ import annotations
 
+import asyncio
 import itertools
 import re
 import shutil
 import sys
 import textwrap
 import weakref
-from  contextlib import suppress
+from contextlib import suppress
 from functools import partial
 from pathlib import Path
-from typing import ClassVar
+from typing import Callable, ClassVar
 
 from markdown_strings import esc_format
 
 from . import colors, widgets
 
 
 class SnippetInsertionPointer:
@@ -201,15 +202,14 @@
     def clean(self) -> Element | None:
         """Clean the source lines.
 
         Tabs are expanded and whitespace is trimmed from the end of each line.
         """
         self.source_lines = [
             line.expandtabs().rstrip() for line in self.source_lines]
-        return None
 
     def neighbour(
             self, *, backwards: bool, within_group: bool,
             predicate=lambda _el: True) -> Snippet | None:
         """Get this element's immediate neighbour.
 
         :backwards:    If set then find preceding neighbour.
@@ -564,15 +564,15 @@
         """Remove a child element from this group."""
         with suppress(ValueError):
             self.children.remove(child)
         snippets = [el for el in self.children if isinstance(el, Snippet)]
         if not snippets:
             self.children.append(PlaceHolder(parent=self))
 
-    def clean(self):
+    def clean(self) -> Element | None:
         """Clean up this and any child groups.
 
         Empty children and groups are removed.
         """
         self.children[:] = [c for c in self.children if not c.is_empty()]
         for group in self.groups.values():
             group.clean()
@@ -681,14 +681,25 @@
         """Generate the text that should be written to a file."""
         if self.tags:
             return f'{self.full_name} [{" ".join(self.tags)}]\n'
         else:
             return f'{self.full_name}\n'
 
 
+class Root(Group):
+    """A group that acts as  the root of the snippet tree."""
+
+    def reset(self):
+        """Reset to initialised state.
+
+        This is used proir to a complet relead.
+        """
+        self.groups = {}
+
+
 def walk_group_tree(
         basic_walk, predicate=lambda _el: True, first_id: str = ''):
     """Perform a walk."""
     it = basic_walk()
     if first_id:
         for el in it:
             if el.uid() == first_id:
@@ -700,21 +711,52 @@
             yield el
 
 
 class Loader:
     """Encapsulation of snippet loading machinery."""
 
     def __init__(self, path):
-        self.path = path
+        self.path = Path(path)
         self.el: Element = PreservedText(parent=None)
-        self.root = self.cur_group = Group('<ROOT>')
-        self.title = ''
+        self.root = Root('<ROOT>')
+        self.cur_group = None
+        self.monitor_task: asyncio.Task | None = None
+        self.load_time = 0
+        self.stop_event = asyncio.Event()
+
+    def start_monitoring(self, on_change_callback: Callable):
+        """Start a task that monitors for change to the loaded file."""
+        self.monitor_task = asyncio.create_task(
+            self.monitor(on_change_callback), name='monitor_file')
+
+    async def stop_monitoring(self):
+        """Stop monitoring for changes to the loaded file."""
+        self.stop_event.set()
+        await self.monitor_task
+
+    async def monitor(self, on_change_callback: Callable):
+        """Task that monitors for change to the loaded file."""
+        async def pause(delay) -> bool:
+            await asyncio.wait([stop_waiter], timeout=delay)
+            return not self.stop_event.is_set()
+
+        stop_waiter = asyncio.create_task(
+            self.stop_event.wait(), name='monitor_stopper')
+        while True:
+            if not await pause(0.2):
+                break
+            if self.mtime > self.load_time:
+                self.load_time = self.mtime
+                on_change_callback()
+                if not await pause(2.0):
+                    break
 
     def store(self):
         """Store the current element if not empty."""
+        # pylint: disable=assignment-from-no-return
         el = self.el
         preserved_text = el.clean()
         if not el.is_empty():
             self.cur_group.add(el)
         if preserved_text:
             self.cur_group.add(preserved_text)
         self.el = PreservedText(parent=None)
@@ -771,15 +813,19 @@
                 self.el = Snippet(parent=self.cur_group)
             return True
         else:
             return False
 
     def load(self):
         """Load a tree of snippets from a file."""
-        with Path(self.path).open(mode='rt', encoding='utf8') as f:
+        self.load_time = self.mtime
+        reset_for_reload()
+        self.root.reset()
+        self.cur_group = self.root
+        with self.path.open(mode='rt', encoding='utf8') as f:
             self.el = PreservedText(parent=None)
             for rawline in f:
                 line = rawline.rstrip()
                 if not (self.handle_comment(line)
                         or self.handle_title(line)
                         or self.handle_group(line)
                         or self.handle_marker(line)):
@@ -790,14 +836,37 @@
         if not self.root.groups:
             sys.exit(f'File {self.path} contains no groups')
 
         for el in self.root.walk_snippets(backwards=False):
             el.reset()
         return self.root, self.root.title
 
+    def save(self, root):
+        """Save a snippet tree to the file."""
+        with self.path.open('wt', encoding='utf8') as f:
+            if root.title:
+                f.write(f'@title: {root.title}\n')
+            for el in root.walk(backwards=False):
+                f.write(el.file_text())
+                if isinstance(el, Group):
+                    kws = el.keyword_set()
+                    if not kws.is_empty():
+                        f.write(kws.file_text())
+        self.load_time = self.mtime
+
+    @property
+    def mtime(self) -> float | int:
+        """The modification time of the loaded file."""
+        try:
+            st = self.path.stat()
+        except OSError:
+            return -1.0
+        else:
+            return st.st_mtime
+
 
 # Conveniant types.
 SnippetLike = Snippet | PlaceHolder
 
 
 def is_snippet_like(el: Element) -> bool:
     """Test if an element is like a snippet.
@@ -808,20 +877,14 @@
 
 
 def id_of_element(obj: Element | None) -> str | None:
     """Get the unique ID of an Element."""
     return None if obj is None else obj.uid()
 
 
-def load(path):
-    """Load a tree of snippets from a file."""
-    loader = Loader(path)
-    return loader.load()
-
-
 def save(path, root):
     """Save a snippet tree to a file."""
     with Path(path).open('wt', encoding='utf8') as f:
         if root.title:
             f.write(f'@title: {root.title}\n')
         for el in root.walk(backwards=False):
             f.write(el.file_text())
@@ -848,19 +911,27 @@
             with suppress(OSError):
                 print('MOVE', src_path, dirpath / new_name)
                 shutil.move(src_path, dirpath / new_name)
     with suppress(OSError):
         shutil.copy(path, dirpath / names[0])
 
 
-def reset_for_tests():
-    """Perform a 'system' reset for test purposes.
+def reset_for_reload():
+    """Perform a 'system' reset.
 
-    This is not intended for non-testing use.
+    This is used when the entire snippet tree is be being reloaded.
     """
     Element.id_source = itertools.count()
     PlaceHolder.id_source = itertools.count()
     TextualElement.id_source = itertools.count()
     PreservedText.id_source = itertools.count()
     Snippet.id_source = itertools.count()
     KeywordSet.id_source = itertools.count()
-    Group.id_source = itertools.count()
+    Group.id_source = itertools.count(1)
+
+
+def reset_for_tests():
+    """Perform a 'system' reset for test purposes.
+
+    This is not intended for non-testing use.
+    """
+    reset_for_reload()
```

### Comparing `clippets-0.1.0/src/clippets/widgets.py` & `clippets-0.3.0/src/clippets/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Iterable
 
 import rich.repr
 from rich.style import Style
 from rich.text import Span, Text
 from textual import events
 from textual.app import App
+from textual.color import Color
 from textual.containers import Grid, VerticalScroll
 from textual.keys import (
     REPLACED_KEYS, _character_to_key, _get_unicode_name_from_key)
 from textual.screen import ModalScreen
 from textual.widgets import Button, Footer, Input, Label, Markdown, Static
 from textual.widgets._markdown import MarkdownBlock
 
@@ -79,33 +80,99 @@
     """Application specific Input widget."""
 
     def on_blur(self, _event):
         """Process a mouse click."""
         self.app.handle_blur(self)
 
 
-class SnippetMenu(ModalScreen):
+class PopupDialog(ModalScreen):
+    """Base for 'popup' dialogues."""
+
+    DEFAULT_CSS = '''
+    #dialog {
+        grid-rows: 1 3;
+        grid-gutter: 1 2;
+        padding: 0 1;
+        height: auto;
+        border: solid $primary-lighten-3;
+        margin: 0 8 0 8;
+        background: $surface;
+    }
+    #question {
+        height: 1;
+        width: 1fr;
+        content-align: center middle;
+    }
+    '''
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.add_class('popup')
+
+
+class SnippetMenu(PopupDialog):
     """Menu providing snippet action choices."""
 
+    DEFAULT_CSS = PopupDialog.DEFAULT_CSS + '''
+    .popup {
+        grid-size: 4;
+    }
+    .question {
+        column-span: 4;
+    }
+    '''
+
     def compose(self):
         """Build the widget hierarchy."""
+        styles = self.styles
+        bg = styles.background
+        styles.background = Color(bg.r, bg.g, bg.b, a=0.6)
+
         yield Grid(
-            Label('Choose action', id='question'),
+            Label('Choose action', id='question', classes='question'),
             Button('Edit', variant='primary', id='edit'),
             Button('Duplicate', variant='primary', id='duplicate'),
             Button('Move', variant='primary', id='move'),
             Button('Cancel', variant='primary', id='cancel'),
-            id='dialog',
+            id='dialog', classes='popup',
         )
 
     def on_button_pressed(self, event: Button.Pressed) -> None:
         """Process a mouse click on a button."""
         self.dismiss(event.button.id)
 
 
+class FileChangedMenu(PopupDialog):
+    """Popup for when the snippets file has been changed."""
+
+    DEFAULT_CSS = PopupDialog.DEFAULT_CSS + '''
+    .popup {
+        grid-size: 2;
+    }
+    .question {
+        column-span: 2;
+    }
+    '''
+
+    def compose(self):
+        """Build the widget hierarchy."""
+        bg = self.styles.background
+        styles = self.styles
+        styles.background = Color(bg.r, bg.g, bg.b, a=0.6)
+        yield Grid(
+            Label('Input file has changed.', id='question'),
+            Button('Load changes', variant='primary', id='load'),
+            Button('Ignore', variant='primary', id='cancel'),
+            id='dialog', classes='popup')
+
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        """Process a mouse click on a button."""
+        self.dismiss(event.button.id)
+
+
 @rich.repr.auto
 class MyFooter(Footer):
     """A simple footer docked to the bottom of the parent container."""
 
     def __init__(self) -> None:
         super().__init__()
         self._context = self.app.context_name()
@@ -241,15 +308,15 @@
             if len(key) == 1 and not key.isalnum():
                 key = _character_to_key(key)                    # noqa: PLW2901
             original_key = REPLACED_KEYS.get(key, key)
             char: str | None = None
             try:
                 char = unicodedata.lookup(
                     _get_unicode_name_from_key(original_key))
-            except KeyError:
+            except KeyError:                                    # noqa: PERF203
                 char = key if len(key) == 1 else None
             key_event = events.Key(key, char)
             key_event._set_sender(app)                           # noqa: SLF001
             driver.send_event(key_event)
 
         await app._animator.wait_until_complete()                # noqa: SLF001
```

### Comparing `clippets-0.1.0/src/clippets/win.py` & `clippets-0.3.0/src/clippets/win.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/src/clippets.egg-info/PKG-INFO` & `clippets-0.3.0/src/clippets.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clippets
-Version: 0.1.0
+Version: 0.3.0
 Summary: UI to build up clipboard content from (rich) text snippets.
 Author-email: Paul Ollis <paul@cleversheep.org>
 Project-URL: Homepage, https://github.com/paul-ollis/clippets
 Project-URL: Bug Tracker, https://github.com/paul-ollis/clippets/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
@@ -30,13 +30,12 @@
 - It has a fairly comprehensive test suite.
 - I hope that crashes should be rare (backup files are maintained to minimise
   the impact).
 
 However:
 
 - It still needs more tests.
-- There are areas of mouse and keyboard support that beg imrpovement.
+- There are areas of mouse and keyboard support that beg improvement.
 - Some desirable features are obviously missing, such as:
 
   - There is no proper documentation beyound the built-in help.
   - It does not yet work on MacOS.
-  - It should monitor the input file for changes.
```

### Comparing `clippets-0.1.0/src/clippets.egg-info/SOURCES.txt` & `clippets-0.3.0/src/clippets.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 tests/test_editing.py
 tests/test_filtering.py
 tests/test_help.py
 tests/test_kb_selection.py
 tests/test_keywords.py
 tests/test_load_save.py
 tests/test_misc_ui.py
+tests/test_monitor.py
 tests/test_moving.py
```

### Comparing `clippets-0.1.0/tests/test_clipboard.py` & `clippets-0.3.0/tests/test_clipboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,14 @@
         Snippet B2
     Third [tag-c tag-a]
       @md@
         Snippet 3
 '''
 
 
-@pytest.fixture(autouse=True)
-def set_env():
-    """Set up the environment for these tests."""
-    os.environ['CLIPPETS_EDITOR'] = f'python {HERE / "edit_helper.py"}'
-
-
 @pytest.fixture
 def infile(snippet_infile):
     """Create a standard input file for many of this module's tests."""
     populate(snippet_infile, std_infile_text)
     return snippet_infile
 
 
@@ -109,15 +103,14 @@
             ['left:snippet-1']            # Add snippet 2
             + ['left:snippet-0']          # Then snippet 1
         )
         _, snapshot_ok = await snapshot_run(infile, actions, options=['--raw'])
         assert snapshot_ok
 
 
-
 class TestKeyboardControlled:
     """Using the keyboard (mostly) to populate the clipboard."""
 
     @pytest.mark.asyncio
     async def test_snippets_use_group_order_by_default(
             self, infile, snapshot_run):
         """By default snippets show in the order thery appear in groups."""
```

### Comparing `clippets-0.1.0/tests/test_editing.py` & `clippets-0.3.0/tests/test_editing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 """Editing the snippets."""
 from __future__ import annotations
 # pylint: disable=redefined-outer-name
+# pylint: disable=no-self-use
 
 import os
 from pathlib import Path
 
 import pytest
 
 from support import clean_text, populate
 
 HERE = Path(__file__).parent
 std_infile_text = '''
+    @title: User supplied title
     Main
       @text@
         Snippet 1
       @text@
         Snippet 2
       @md@
         Snippet 3
 '''
 
 
-# TODO: Move to conftest. This is duplicated.
-@pytest.fixture(autouse=True)
-def set_env():
-    """Set up the environment for these tests."""
-    os.environ['CLIPPETS_EDITOR'] = f'python {HERE / "edit_helper.py"}'
-
-
 @pytest.fixture
 def infile(snippet_infile):
     """Create a standard input file for many of this module's tests."""
     populate(snippet_infile, std_infile_text)
     return snippet_infile
 
 
@@ -57,15 +52,14 @@
             MarkdownSnippet: 'Snippet 3'
         ''')
         runner, snapshot_ok = await snapshot_run(infile, actions)
         assert expect == runner.app.groups.full_repr()
         assert 'Snippet 2' == edit_text_file.prev_text
         assert snapshot_ok
 
-
     @pytest.mark.asyncio
     async def test_a_snippet_can_be_duplicated(
             self, infile, edit_text_file, snapshot_run):
         """A snippet's contents may be duplicated and immediately edited."""
         populate(edit_text_file, 'Snippet 4')
         actions = (
             ['down'] * 2          # Move to Snippet 3
@@ -82,15 +76,14 @@
             MarkdownSnippet: 'Snippet 4'
         ''')
         runner, snapshot_ok = await snapshot_run(infile, actions)
         assert expect == runner.app.groups.full_repr()
         assert 'Snippet 3' == edit_text_file.prev_text
         assert snapshot_ok
 
-
     @pytest.mark.asyncio
     async def test_clipboard_can_be_edited(
             self, infile, edit_text_file, snapshot_run):
         """The prepared clipboard content can be edited."""
         populate(edit_text_file, 'Snippet 2 - edited')
         actions = (
             ['down']              # Move to Snippet 2
```

### Comparing `clippets-0.1.0/tests/test_filtering.py` & `clippets-0.3.0/tests/test_filtering.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,20 +39,14 @@
     Third [tag-c tag-a]
       @text@
         Snippet 3
 '''
 
 
 @pytest.fixture(autouse=True)
-def set_env():
-    """Set up the environment for these tests."""
-    os.environ['CLIPPETS_EDITOR'] = f'python {HERE / "edit_helper.py"}'
-
-
-@pytest.fixture(autouse=True)
 def reset_app_data():
     """Reset some application data.
 
     This ensures that snippet/widget IDs can be predicted.
     """
     snippets.reset_for_tests()
     core.reset_for_tests()
```

### Comparing `clippets-0.1.0/tests/test_help.py` & `clippets-0.3.0/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/tests/test_kb_selection.py` & `clippets-0.3.0/tests/test_kb_selection.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,50 +3,15 @@
 The up and down keys change the currently selected (and highlighed) snippet.
 """
 from __future__ import annotations
 # pylint: disable=redefined-outer-name
 
 import pytest
 
-from support import populate
-
-long_infile_text = '''
-    Main
-      @text@
-        Snippet 1
-      @text@
-        Snippet 2
-      @text@
-        Snippet 3
-    Second
-      @text@
-        Snippet 4
-      @text@
-        Snippet 5
-    Third
-      @text@
-        Snippet 6
-      @text@
-        Snippet 7
-      @text@
-        Snippet 8
-      @text@
-        Snippet 9
-    Fourth
-      @text@
-        Snippet 10
-      @text@
-        Snippet 11
-      @text@
-        Snippet 12
-      @text@
-        Snippet 13
-      @text@
-        Snippet 14
-'''
+from support import long_infile_text, populate
 
 
 @pytest.fixture
 def longfile(snippet_infile):
     """Create a standard input file for scrolling tests."""
     populate(snippet_infile, long_infile_text)
     return snippet_infile
@@ -117,7 +82,20 @@
     actions = (
         ['down'] * 5                       # Move down to snippet 6.
         + ['left:group-2']                 # Close the second group.
         + ['up']                           # Move down to snippet 3.
     )
     _, snapshot_ok = await snapshot_run(longfile, actions)
     assert snapshot_ok
+
+
+@pytest.mark.asyncio
+async def test_no_snippets_is_handled(longfile, snapshot_run):
+    """An input with no snippets is gracefully handled."""
+    populate(longfile, '''
+        Main
+    ''')
+    actions = (
+        ['down']                           # Try to move down.
+    )
+    _, snapshot_ok = await snapshot_run(longfile, actions)
+    assert snapshot_ok
```

### Comparing `clippets-0.1.0/tests/test_keywords.py` & `clippets-0.3.0/tests/test_keywords.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/tests/test_load_save.py` & `clippets-0.3.0/tests/test_load_save.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,32 +58,38 @@
     print('--------')
     for text in strings:
         for line in text.splitlines(True):
             print(f'  {line!r}')
         print('--------')
 
 
+def load(path_name: str):
+    """Load snippets from a file."""
+    loader = snippets.Loader(path_name)
+    return loader.load()
+
+
 # TODO: Support empty or non-existant file.
 def test_load_empty_file(snippet_infile):
     """An empty snippet file is considered an error."""
     with pytest.raises(SystemExit) as info:
-        snippets.load(snippet_infile.name)
+        load(snippet_infile.name)
     expected = f'File {snippet_infile.name} contains no groups'
     assert str(info.value) == expected
 
 
 def test_single_empty_group(snippet_infile):
     """A file with at least one group is valid, even without any snippets.
 
     The first element in the group will be an empty keywrod set.
     """
     populate(snippet_infile, '''
         Main
     ''')
-    root, title = snippets.load(snippet_infile.name)
+    root, title = load(snippet_infile.name)
     assert title == ''
     expect = clean_text('''
         <ROOT>
         Main''')
     assert root.outline_repr() == expect
     expect = clean_text('''
         Group: <ROOT>
@@ -96,15 +102,15 @@
 def test_single_entry_group(snippet_infile):
     """A file with one snippet is valid."""
     populate(snippet_infile, '''
         Main
           @text@
             Snippet 1
     ''')
-    root, title = snippets.load(snippet_infile.name)
+    root, title = load(snippet_infile.name)
     assert title == ''
     expect = clean_text('''
         <ROOT>
         Main''')
     assert root.outline_repr() == expect
     expect = clean_text(r'''
         Group: <ROOT>
@@ -119,15 +125,15 @@
 def test_single_markdown_snipper(snippet_infile):
     """A file with one snippet is valid."""
     populate(snippet_infile, '''
         Main
           @md@
             Snippet 1
     ''')
-    root, title = snippets.load(snippet_infile.name)
+    root, title = load(snippet_infile.name)
     assert title == ''
     expect = clean_text('''
         <ROOT>
         Main''')
     assert root.outline_repr() == expect
     expect = clean_text(r'''
         Group: <ROOT>
@@ -143,15 +149,15 @@
     """A leading blank line is stored."""
     populate(snippet_infile, '''
         |
         Main
           @md@
             Snippet 1
     ''')
-    root, title = snippets.load(snippet_infile.name)
+    root, title = load(snippet_infile.name)
     assert title == ''
     expect = clean_text('''
         <ROOT>
         Main''')
     assert root.outline_repr() == expect
     expect = clean_text(r'''
         Group: <ROOT>
@@ -181,15 +187,15 @@
           @md@
             Snippet 2
           @keywords@
             three four
           @keywords@
             five three
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     expect = clean_text('''
         <ROOT>
         Main
         Second
     ''')
     assert root.outline_repr() == expect
     expect = clean_text(r'''
@@ -210,30 +216,30 @@
     """Writing a file preserves a single snippit correctly."""
     expected = clean_text('''
         Main
           @md@
             Snippet 1
     ''')
     populate(snippet_infile, expected)
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_two_snippets_are_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves two snippits correctly."""
     expected = clean_text('''
         Main
           @md@
             Snippet 1
           @md@
             Snippet 2
     ''')
     populate(snippet_infile, expected)
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_nested_groups_are_handled(snippet_infile, snippet_outfile):
     """Nested sub-groups are correcttly saved."""
     expected = clean_text('''
@@ -241,15 +247,15 @@
           @md@
             Snippet 1
         Main : Subgroup
           @md@
             Snippet 2
     ''')
     populate(snippet_infile, expected)
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_nested_groups_with_tags_are_handled(snippet_infile, snippet_outfile):
     """Nested sub-groups with tags are correcttly saved."""
     expected = clean_text('''
@@ -257,29 +263,29 @@
           @md@
             Snippet 1
         Main : Subgroup [tag-a tag-b]
           @md@
             Snippet 2
     ''')
     populate(snippet_infile, expected)
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert expected == str(snippet_outfile)
 
 
 def test_leading_comment_block_is_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves any leading block comment."""
     expected = populate(snippet_infile, '''
         # A leading
         # comment block.
         Main
           @md@
             Snippet 1
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_leading_blank_lines_are_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves leading blank lines.
 
@@ -289,15 +295,15 @@
     expected = populate(snippet_infile, '''
         |
         # Comment
         Main
           @md@
             Snippet 1
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_interspersed_text_is_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves leading blank lines."""
     expected = populate(snippet_infile, '''
@@ -306,30 +312,30 @@
             Snippet 1
 
         # Comment
 
           @md@
             Snippet 2
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_trailing_text_is_preserved(snippet_infile, snippet_outfile):
     """Writing a file preserves trailing comments and blank lines."""
     expected = populate(snippet_infile, '''
         Main
           @md@
             Snippet 1
 
         # Comment
         |
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert str(snippet_outfile) == expected
 
 
 def test_keywords_are_saved(snippet_infile, snippet_outfile):
     """Keywords are saved."""
     expected = populate(snippet_infile, '''
@@ -339,15 +345,15 @@
             two
           @md@
             Snippet 1
 
         # Comment
         |
     ''')
-    root, _ = snippets.load(snippet_infile.name)
+    root, _ = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert expected == str(snippet_outfile)
 
 
 def test_title_is_preserved(snippet_infile, snippet_outfile):
     """An user supplied title is saved."""
     expected = populate(snippet_infile, '''
@@ -358,11 +364,11 @@
             two
           @md@
             Snippet 1
 
         # Comment
         |
     ''')
-    root, title = snippets.load(snippet_infile.name)
+    root, title = load(snippet_infile.name)
     snippets.save(snippet_outfile.name, root)
     assert 'User supplied title' == title
     assert expected == str(snippet_outfile)
```

### Comparing `clippets-0.1.0/tests/test_misc_ui.py` & `clippets-0.3.0/tests/test_misc_ui.py`

 * *Files identical despite different names*

### Comparing `clippets-0.1.0/tests/test_moving.py` & `clippets-0.3.0/tests/test_moving.py`

 * *Files identical despite different names*

