# Comparing `tmp/usolitaire-1.0.3.tar.gz` & `tmp/usolitaire-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usolitaire-1.0.3.tar", last modified: Fri Jul 28 23:30:10 2023, max compression
+gzip compressed data, was "usolitaire-1.1.0.tar", last modified: Sun Jul 30 23:14:24 2023, max compression
```

## Comparing `usolitaire-1.0.3.tar` & `usolitaire-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.0.3/LICENSE
--rw-rw-r--   0 elias     (1000) elias     (1000)      105 2023-07-27 12:52:48.000000 usolitaire-1.0.3/MANIFEST.in
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-28 23:30:10.981937 usolitaire-1.0.3/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-27 12:36:19.000000 usolitaire-1.0.3/README.rst
--rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.0.3/pyproject.toml
--rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-28 23:30:10.981937 usolitaire-1.0.3/setup.cfg
--rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-28 23:29:58.000000 usolitaire-1.0.3/setup.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/usolitaire/
--rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-28 23:29:58.000000 usolitaire-1.0.3/usolitaire/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)    12204 2023-07-28 23:28:02.000000 usolitaire-1.0.3/usolitaire/app.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 21:42:22.000000 usolitaire-1.0.3/usolitaire/card_render.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.0.3/usolitaire/game.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      775 2023-07-27 21:42:22.000000 usolitaire-1.0.3/usolitaire/textual_app.css
--rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 16:37:59.000000 usolitaire-1.0.3/usolitaire/textual_ui.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-28 23:30:10.981937 usolitaire-1.0.3/usolitaire.egg-info/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)      441 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/SOURCES.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/dependency_links.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/entry_points.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/not-zip-safe
--rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/requires.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-28 23:30:10.000000 usolitaire-1.0.3/usolitaire.egg-info/top_level.txt
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-30 23:14:24.632027 usolitaire-1.1.0/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1074 2023-07-23 16:38:34.000000 usolitaire-1.1.0/LICENSE
+-rw-rw-r--   0 elias     (1000) elias     (1000)      105 2023-07-27 12:52:48.000000 usolitaire-1.1.0/MANIFEST.in
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-30 23:14:24.632027 usolitaire-1.1.0/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-30 23:14:01.000000 usolitaire-1.1.0/README.rst
+-rw-rw-r--   0 elias     (1000) elias     (1000)       29 2023-07-27 12:14:41.000000 usolitaire-1.1.0/pyproject.toml
+-rw-rw-r--   0 elias     (1000) elias     (1000)      404 2023-07-30 23:14:24.632027 usolitaire-1.1.0/setup.cfg
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1282 2023-07-30 23:14:13.000000 usolitaire-1.1.0/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-30 23:14:24.632027 usolitaire-1.1.0/usolitaire/
+-rw-rw-r--   0 elias     (1000) elias     (1000)      119 2023-07-30 23:14:13.000000 usolitaire-1.1.0/usolitaire/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    15328 2023-07-30 23:11:08.000000 usolitaire-1.1.0/usolitaire/app.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2052 2023-07-27 21:42:22.000000 usolitaire-1.1.0/usolitaire/card_render.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     8662 2023-07-27 12:15:26.000000 usolitaire-1.1.0/usolitaire/game.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1159 2023-07-30 23:09:29.000000 usolitaire-1.1.0/usolitaire/textual_app.css
+-rw-rw-r--   0 elias     (1000) elias     (1000)     7543 2023-07-27 16:37:59.000000 usolitaire-1.1.0/usolitaire/textual_ui.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-07-30 23:14:24.632027 usolitaire-1.1.0/usolitaire.egg-info/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1913 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)      441 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/SOURCES.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/dependency_links.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       51 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/entry_points.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/not-zip-safe
+-rw-rw-r--   0 elias     (1000) elias     (1000)        8 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/requires.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-07-30 23:14:24.000000 usolitaire-1.1.0/usolitaire.egg-info/top_level.txt
```

### Comparing `usolitaire-1.0.3/LICENSE` & `usolitaire-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.3/PKG-INFO` & `usolitaire-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.3
+Version: 1.1.0
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `usolitaire-1.0.3/README.rst` & `usolitaire-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.3/setup.py` & `usolitaire-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 requirements = [
     "textual",
 ]
 
 setup(
     name="usolitaire",
-    version="1.0.3",
+    version="1.1.0",
     description="Solitaire in your terminal",
     long_description=readme,
     author="Elias Dorneles",
     author_email="eliasdorneles@gmail.com",
     url="https://github.com/eliasdorneles/usolitaire",
     entry_points={
         "console_scripts": {
```

### Comparing `usolitaire-1.0.3/usolitaire/app.py` & `usolitaire-1.1.0/usolitaire/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,24 @@
 from dataclasses import dataclass
 from enum import Enum
 
 from textual.app import App
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Container
+from textual.containers import Grid
+from textual.css.query import NoMatches
+from textual.screen import ModalScreen
+from textual.screen import Screen
+from textual.widgets import Button
 from textual.widgets import Footer
 from textual.widgets import Header
-from textual.widgets import Static
+from textual.widgets import Label
 from textual.widgets import Markdown
+from textual.widgets import Static
 
 from usolitaire.game import Card
 from usolitaire.game import Game
 from usolitaire.textual_ui import CardClicked
 from usolitaire.textual_ui import ClickType
 from usolitaire.textual_ui import EmptyTableauClicked
 from usolitaire.textual_ui import MoveDirection
@@ -78,74 +84,153 @@
 [USolitaire](https://github.com/eliasdorneles/usolitaire) is a Klondike
 Solitaire game made with ❤️  by [Elias Dorneles](https://github.com/eliasdorneles).
 
 It's written in Python 🐍 and uses the [Textual](https://textual.textualize.io) framework.
 """
 
 
+class EndOfGameScreen(Screen):
+    def compose(self) -> ComposeResult:
+        yield Header()
+        yield Container(Markdown(END_OF_GAME_MESSAGE))
+        yield Footer()
+
+
 class MyFooter(Static):
     def __init__(self):
         super().__init__(
             "Move with the arrow keys, [bold]SPACE[/bold] clicks and [bold]ENTER[/bold] double-clicks. Or just use the mouse."
         )
 
 
+class ConfirmNewGameScreen(ModalScreen):
+    BINDINGS = [("escape", "app.pop_screen", "Pop screen")]
+
+    def compose(self) -> ComposeResult:
+        yield Grid(
+            Label("❔    Do you want to start a new game?"),
+            Button("Yes, start new game", variant="primary", id="confirm_new_game_btn"),
+            Button("No, go back", variant="default", id="cancel"),
+            id="dialog",
+        )
+
+    def on_key(self, event):
+        if event.key in ("left", "down"):
+            self.focus_next()
+        elif event.key in ("right", "up"):
+            self.focus_previous()
+
+    def on_button_pressed(self, event: Button.Pressed) -> None:
+        self.dismiss(event.button.id == "confirm_new_game_btn")
+
+
 class USolitaire(App):
     BINDINGS = [
-        Binding("tab", "switch_row_focus", "Switch focus", priority=True, show=False),
+        Binding("tab", "switch_row_focus", "Switch focus", priority=True, show=True),
         Binding("shift-tab", "switch_row_focus", "Switch focus", priority=True, show=False),
         Binding("ctrl+d", "deal_from_stock", "Deal from stock", show=True),
+        Binding("n", "request_new_game", "New game", show=True),
         Binding("d", "toggle_dark", "Toggle 🌙 mode", show=True),
         ("q", "quit", "Quit"),
     ]
     CSS_PATH = os.path.join(os.path.dirname(__file__), "textual_app.css")
 
     def __init__(self):
         super().__init__()
         self.game = Game()
+
         self.last_focus = {
             FocusRow.TOP: FocusPosition(FocusRow.TOP, 0),
             FocusRow.BOTTOM: FocusPosition(FocusRow.BOTTOM, 0),
         }
         self._current_focus = FocusPosition(FocusRow.TOP, 0)
         self.selected_card: SelectedCardPosition | None = None
+        self.playing: bool = True
 
     @property
     def current_focus(self) -> FocusPosition:
         return self._current_focus
 
     @current_focus.setter
     def current_focus(self, value: FocusPosition):
         self._current_focus = value
         self.last_focus[value.row] = value
 
+    def action_request_new_game(self):
+        self.playing = False
+
+        def confirm_new_game(confirm):
+            if confirm:
+                self.game = Game()
+                try:
+                    self.query_one("EndOfGameScreen")
+                    self.pop_screen()
+                except NoMatches:
+                    pass
+
+                self._current_focus = FocusPosition(FocusRow.TOP, 0)
+                self.selected_card = None
+                self.refresh_contents()
+                self.playing = True
+
+        self.push_screen(ConfirmNewGameScreen(), callback=confirm_new_game)
+
     def compose(self) -> ComposeResult:
         yield Header()
 
         with Container(id="game-container"):
             yield PileWidget(self.game.stock, id="stock")
             yield PileWidget(self.game.waste, id="waste")
-            yield Static(
-                ""
-            )  # needed to occupy the space on the grid between waste and foundations
+
+            # needed to occupy the space on the grid between waste and foundations:
+            yield Static("")
 
             for i, foundation_pile in enumerate(self.game.foundations):
                 yield PileWidget(foundation_pile, id=f"foundation{i}")
 
             for i, tableau_pile in enumerate(self.game.tableau):
                 yield TableauPileWidget(tableau_pile, i, id=f"tableau{i}")
 
         yield MyFooter()
         yield Footer()
 
+    def refresh_contents(self):
+        for i, pile in enumerate(self.game.foundations):
+            pile_widget = self._get_foundation_pile(i)
+            pile_widget.pile = pile
+            pile_widget.refresh_contents()
+
+        for i, pile in enumerate(self.game.tableau):
+            pile_widget = self._get_tableau_pile(i)
+            pile_widget.pile = pile
+            pile_widget.index = i
+            pile_widget.refresh_contents()
+
+        stock_pile_widget = self._get_stock_pile()
+        stock_pile_widget.pile = self.game.stock
+        stock_pile_widget.refresh_contents()
+
+        waste_pile_widget = self._get_waste_pile()
+        waste_pile_widget.pile = self.game.waste
+        waste_pile_widget.refresh_contents()
+        self._update_focus()
+        self.refresh()
+
     def action_quit(self):
         self.exit()
 
     def action_switch_row_focus(self):
-        print(self.query_one("Footer").get_component_styles("footer--highlight").rich_style)
+        try:
+            # if in the modal screen, switch focus inside it
+            self.query_one("ConfirmNewGameScreen #dialog")
+            self.screen.focus_next()
+            return
+        except NoMatches:
+            pass
+
         if self.current_focus.row == FocusRow.TOP:
             self.current_focus = self.last_focus[FocusRow.BOTTOM]
         else:
             self.current_focus = self.last_focus[FocusRow.TOP]
         self._update_focus()
 
     def on_move_focus(self, event: MoveFocus):
@@ -205,69 +290,82 @@
                     len(self.game.tableau[self.current_focus.pile_index]) - 1
                 )
 
         if self.current_focus.card_index is not None:
             focused_pile.children[self.current_focus.card_index].focus()
 
     def action_deal_from_stock(self):
+        if not self.playing:
+            return
+
         if self.game.stock:
             self.game.deal_from_stock()
         else:
             self.game.restore_stock()
-        self.query_one("#stock").refresh_contents()
-        self.query_one("#waste").refresh_contents()
+        self._get_stock_pile().refresh_contents()
+        self._get_waste_pile().refresh_contents()
 
     def refresh_foundations(self):
         for i in range(4):
-            self.query_one(f"#foundation{i}").refresh_contents()
+            self._get_foundation_pile(i).refresh_contents()
 
     def highlight_selected_cards(self):
         self.query(".selected").remove_class("selected")
         if self.selected_card is None:
             return
         if self.selected_card.pile_id == "waste":
-            pile_widget = self.query_one("#waste")
-            pile_widget.add_class("selected")
+            self._get_waste_pile().add_class("selected")
         else:
             pile_widget = self.query_one("#" + self.selected_card.pile_id)
             for child in pile_widget.children[self.selected_card.card_index :]:
                 child.add_class("selected")
 
     def on_card_clicked(self, event: CardClicked):
         if event.sender_id == "stock":
             self.action_deal_from_stock()
         if event.sender_id == "waste":
             if (
                 event.click_type == ClickType.DOUBLE
                 and self.game.can_move_to_foundation_from_waste()
             ):
                 self.game.move_to_foundation_from_waste()
-                self.query_one("#waste").refresh_contents()
+                self._get_waste_pile().refresh_contents()
                 self.refresh_foundations()
                 self.check_if_won()
             else:
                 if not self.game.waste:
                     return
                 new_selected_card = SelectedCardPosition(
                     self.game.waste[-1], "waste", len(self.game.waste) - 1
                 )
                 if new_selected_card == self.selected_card:
                     self.selected_card = None
                 else:
                     self.selected_card = new_selected_card
                 self.highlight_selected_cards()
 
+    def _get_waste_pile(self) -> PileWidget:
+        return self.query_one("#waste", PileWidget)
+
+    def _get_stock_pile(self) -> PileWidget:
+        return self.query_one("#stock", PileWidget)
+
+    def _get_foundation_pile(self, foundation_index: int) -> PileWidget:
+        return self.query_one(f"#foundation{foundation_index}", PileWidget)
+
+    def _get_tableau_pile(self, tableau_index: int) -> TableauPileWidget:
+        return self.query_one(f"#tableau{tableau_index}", TableauPileWidget)
+
     def refresh_tableau(self, tableau_index: int):
-        self.query_one(f"#tableau{tableau_index}").refresh_contents()
+        self._get_tableau_pile(tableau_index).refresh_contents()
 
     def check_if_won(self):
         if self.game.won():
-            self.query("#game-container").remove()
-            self.query("#help-text").remove()
-            self.mount(Container(Markdown(END_OF_GAME_MESSAGE), id="end-game"))
+            self.push_screen(EndOfGameScreen())
+            self.playing = False
 
     def on_tableau_card_clicked(self, event: TableauCardClicked):
         if event.click_type == ClickType.DOUBLE:
             if self.game.can_move_to_foundation_from_tableau(event.pile_index):
                 self.game.move_to_foundation_from_tableau(event.pile_index)
                 self.refresh_tableau(event.pile_index)
                 self.refresh_foundations()
@@ -300,15 +398,15 @@
             self.highlight_selected_cards()
 
     def _try_moving_selected_card_to_tableau(self, tableau_index: int):
         src_pile_id = self.selected_card.pile_id
         if src_pile_id == "waste":
             if self.game.can_move_from_waste_to_tableau(tableau_index):
                 self.game.move_from_waste_to_tableau(tableau_index)
-                self.query_one("#waste").refresh_contents()
+                self._get_waste_pile().refresh_contents()
         else:
             src_pile_index = int(self.selected_card.pile_id[7:])
             if self.game.can_move_card_to_tableau(self.selected_card.card, tableau_index):
                 self.game.move_tableau_pile(src_pile_index, tableau_index)
                 self.refresh_tableau(src_pile_index)
         self.refresh_tableau(tableau_index)
         self.selected_card = None
```

### Comparing `usolitaire-1.0.3/usolitaire/card_render.py` & `usolitaire-1.1.0/usolitaire/card_render.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.3/usolitaire/game.py` & `usolitaire-1.1.0/usolitaire/game.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.3/usolitaire/textual_ui.py` & `usolitaire-1.1.0/usolitaire/textual_ui.py`

 * *Files identical despite different names*

### Comparing `usolitaire-1.0.3/usolitaire.egg-info/PKG-INFO` & `usolitaire-1.1.0/usolitaire.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usolitaire
-Version: 1.0.3
+Version: 1.1.0
 Summary: Solitaire in your terminal
 Home-page: https://github.com/eliasdorneles/usolitaire
 Author: Elias Dorneles
 Author-email: eliasdorneles@gmail.com
 License: MIT license
 Keywords: usolitaire
 Classifier: Development Status :: 2 - Pre-Alpha
```

