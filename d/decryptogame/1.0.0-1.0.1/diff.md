# Comparing `tmp/decryptogame-1.0.0.tar.gz` & `tmp/decryptogame-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decryptogame-1.0.0.tar", last modified: Sun Jul 30 21:13:06 2023, max compression
+gzip compressed data, was "decryptogame-1.0.1.tar", last modified: Mon Jul 31 00:37:35 2023, max compression
```

## Comparing `decryptogame-1.0.0.tar` & `decryptogame-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.046874 decryptogame-1.0.0/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-1.0.0/LICENSE
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-30 21:13:06.045104 decryptogame-1.0.0/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      780 2023-07-30 21:10:07.000000 decryptogame-1.0.0/README.md
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      773 2023-07-30 21:09:47.000000 decryptogame-1.0.0/pyproject.toml
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-07-30 21:13:06.047193 decryptogame-1.0.0/setup.cfg
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:05.995707 decryptogame-1.0.0/src/
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.023007 decryptogame-1.0.0/src/decryptogame/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      147 2023-07-16 21:46:14.000000 decryptogame-1.0.0/src/decryptogame/__init__.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2213 2023-07-29 07:32:34.000000 decryptogame-1.0.0/src/decryptogame/components.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     7193 2023-07-29 07:49:55.000000 decryptogame-1.0.0/src/decryptogame/end_criteria.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6833 2023-07-30 20:42:07.000000 decryptogame-1.0.0/src/decryptogame/game.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3627 2023-07-29 07:56:45.000000 decryptogame-1.0.0/src/decryptogame/generators.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.031183 decryptogame-1.0.0/src/decryptogame/official_words/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     4745 2023-07-29 06:33:23.000000 decryptogame-1.0.0/src/decryptogame/official_words/english.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3658 2023-07-30 20:36:21.000000 decryptogame-1.0.0/src/decryptogame/play.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6741 2023-07-30 20:39:38.000000 decryptogame-1.0.0/src/decryptogame/teams.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.029190 decryptogame-1.0.0/src/decryptogame.egg-info/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      504 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/SOURCES.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/dependency_links.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/top_level.txt
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.042047 decryptogame-1.0.0/tests/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1468 2023-07-29 05:55:47.000000 decryptogame-1.0.0/tests/test_components.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3926 2023-07-30 20:48:01.000000 decryptogame-1.0.0/tests/test_game.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      943 2023-07-29 07:15:17.000000 decryptogame-1.0.0/tests/test_generators.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.221417 decryptogame-1.0.1/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-1.0.1/LICENSE
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-31 00:37:35.220897 decryptogame-1.0.1/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      780 2023-07-30 21:10:07.000000 decryptogame-1.0.1/README.md
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      773 2023-07-31 00:35:49.000000 decryptogame-1.0.1/pyproject.toml
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-07-31 00:37:35.221546 decryptogame-1.0.1/setup.cfg
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.154615 decryptogame-1.0.1/src/
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.190765 decryptogame-1.0.1/src/decryptogame/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      965 2023-07-31 00:17:58.000000 decryptogame-1.0.1/src/decryptogame/__init__.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2502 2023-07-30 23:48:46.000000 decryptogame-1.0.1/src/decryptogame/components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     7193 2023-07-29 07:49:55.000000 decryptogame-1.0.1/src/decryptogame/end_criteria.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6833 2023-07-30 20:42:07.000000 decryptogame-1.0.1/src/decryptogame/game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3627 2023-07-29 07:56:45.000000 decryptogame-1.0.1/src/decryptogame/generators.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.206424 decryptogame-1.0.1/src/decryptogame/official_words/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     4745 2023-07-29 06:33:23.000000 decryptogame-1.0.1/src/decryptogame/official_words/english.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3726 2023-07-30 21:52:49.000000 decryptogame-1.0.1/src/decryptogame/play.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     8570 2023-07-31 00:12:46.000000 decryptogame-1.0.1/src/decryptogame/teams.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.204734 decryptogame-1.0.1/src/decryptogame.egg-info/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-31 00:37:35.000000 decryptogame-1.0.1/src/decryptogame.egg-info/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      504 2023-07-31 00:37:35.000000 decryptogame-1.0.1/src/decryptogame.egg-info/SOURCES.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-07-31 00:37:35.000000 decryptogame-1.0.1/src/decryptogame.egg-info/dependency_links.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-07-31 00:37:35.000000 decryptogame-1.0.1/src/decryptogame.egg-info/top_level.txt
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-31 00:37:35.217172 decryptogame-1.0.1/tests/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1468 2023-07-29 05:55:47.000000 decryptogame-1.0.1/tests/test_components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3926 2023-07-30 20:48:01.000000 decryptogame-1.0.1/tests/test_game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      943 2023-07-29 07:15:17.000000 decryptogame-1.0.1/tests/test_generators.py
```

### Comparing `decryptogame-1.0.0/LICENSE` & `decryptogame-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/PKG-INFO` & `decryptogame-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 1.0.0
+Version: 1.0.1
 Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `decryptogame-1.0.0/README.md` & `decryptogame-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/pyproject.toml` & `decryptogame-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "decryptogame"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Jaden Rodriguez", email="jadenrodriguez7@gmail.com" },
 ]
 description = "A non-official implementation of a Decrypto-style game for simulation and AI work."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `decryptogame-1.0.0/src/decryptogame/components.py` & `decryptogame-1.0.1/src/decryptogame/components.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,35 @@
     Attributes:
         WHITE (int): Team name for the White team, with a value of 0.
         BLACK (int): Team name for the Black team, with a value of 1.
     """
     WHITE = 0
     BLACK = 1
 
-    def __format__(self, spec):
-        """Custom format method for TeamName enumeration values.
+    def __repr__(self):
+        """Custom representation for TeamName enumeration values.
 
         Args:
             spec (str): Format specification.
 
         Returns:
             str: A formatted string representation of the TeamName.
         """
         return f"<{self.name}: {self.value}>"
+    
+    def __format__(self, spec):
+        """Custom formmatting method for TeamName enumeration values.
+
+        Args:
+            spec (str): Format specification.
+
+        Returns:
+            str: A formatted string representation of the TeamName.
+        """
+        return str(self.name)
 
 @dataclasses.dataclass(kw_only=True)
 class GameData:
     """Class representing the game data. It's main use would be for strategizing or simulating plies.
 
     Attributes:
         rounds_played (int, optional): The number of rounds played. Defaults to 0.
```

### Comparing `decryptogame-1.0.0/src/decryptogame/end_criteria.py` & `decryptogame-1.0.1/src/decryptogame/end_criteria.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/src/decryptogame/game.py` & `decryptogame-1.0.1/src/decryptogame/game.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/src/decryptogame/generators.py` & `decryptogame-1.0.1/src/decryptogame/generators.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/src/decryptogame/official_words/english.py` & `decryptogame-1.0.1/src/decryptogame/official_words/english.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/src/decryptogame/play.py` & `decryptogame-1.0.1/src/decryptogame/play.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from decryptogame.components import Code, Note
 from decryptogame.game import Game
 from decryptogame.generators import RandomCodes
 from decryptogame.teams import Team, TeamContext
 from functools import partial
 from typing import Optional
     
-def play_game(teams: Sequence[Team], *, game: Game = None, round_codes: Iterable[Sequence[Code]] = None, round_limit: Optional[int]=None):
+def play_game(teams: Sequence[Team], *, 
+              game: Game = None, 
+              round_codes: Iterable[Sequence[Code]] = None, 
+              round_limit: Optional[int]=None
+              ) -> Game:
     """Play a game of Decrypto. This function will change the game object as the rounds are played.
 
     Args:
         teams (Sequence[Team]): The pair of teams participating in the game.
         game (Game): The Decrypto game object. If None, a standard game will be generated.
         round_codes (Iterable[Sequence[Code]], optional): Iterable of codes for each round. If None, random codes will be generated.
         round_limit (Optional[int], optional): The maximum number of rounds to play. If None, the game continues until completion.
```

### Comparing `decryptogame-1.0.0/src/decryptogame/teams.py` & `decryptogame-1.0.1/src/decryptogame/teams.py`

 * *Files 17% similar despite different names*

```diff
@@ -71,100 +71,145 @@
 
 
 # command line players allow a developer to enter clues or code through the command line
 
 class CommandLineEncryptor(Encryptor):
     """A teammate who decides clues using the command line. """
 
+    def print_context(self, context: TeamContext):
+        """Print information for the developer to know how to interact through the command line.
+
+        Args:
+            context (TeamContext): Relevant information to the developer. 
+        """
+        print("=" * 12)
+        print(f"You are Encryptor on team {TeamName(context.team_name)}")
+        print(f"Keywords: {context.keywords}")
+        print(f"Notesheet: {context.game.notesheet}")
+        print(f"Scoresheet: {context.game.data}")
+        print(f"Number of Opponent Keywords: {context.num_opponent_keywords}")
+
     def decide_clues(self, code: Code, context: TeamContext) -> Clue:
         """Decide clues for the given code using the command line.
 
         Args:
             code (Code): The code assigned to the Encryptor to decide clues for.
             context (TeamContext): Relevant information the Encryptor's decision may be guided by.
 
         Returns:
             Clue: The clues decided by the Encryptor for each code number in the provided code.
         """
-        print(f"You are Encryptor on team {TeamName(context.team_name)}")
-        print(f"Notesheet: {context.game.notesheet}")
-        print(f"Scoresheet: {context.game.data}")
-        print(f"Keywords: {context.keywords}")
+        self.print_context(context)
         print(f"Code : {code}")
-        clues = []
-        for code_num in code:
-            clue = input(f"Clue for number {code_num}: ")
-            clues.append(clue)
-        return tuple(clues)
+        clues = tuple(input(f"Clue for number {code_num}: ") for code_num in code)
+        return clues
 
 class CommandLineIntercepter(Intercepter):
     """A teammate who attempts to decipher the opposing team's clues using the command line. """
 
+    def print_context(self, context: TeamContext):
+        """Print information for the developer to know how to interact through the command line.
+
+        Args:
+            context (TeamContext): Relevant information to the developer. 
+        """
+        print("=" * 12)
+        print(f"You are Intercepter on team {TeamName(context.team_name)}")
+        print(f"Keywords: {context.keywords}")
+        print(f"Notesheet: {context.game.notesheet}")
+        print(f"Scoresheet: {context.game.data}")
+        print(f"Number of Opponent Keywords: {context.num_opponent_keywords}")
+
+
+    def get_code_num(self, clue: str, context: TeamContext) -> int:
+        """Attempt to decipher a single opponent's clue using the command line.
+
+        Args:
+            clue (str): The clue provided by the opposing team.
+            context (TeamContext): Relevant information the Intercepter's decision may be guided by. 
+
+        Returns:
+            int: The guessed code number based on the opposing team's clue.
+        """
+        code_num = None
+        while code_num is None:
+            try:
+                code_num = int(input(f"Code number for clue {clue}: "))
+            except ValueError:
+                pass
+            if code_num is None or code_num not in range(len(context.keywords)):
+                print(f"Code num must lie in range [0 - {len(context.keywords)}).")
+                code_num = None
+        return code_num
+
     def intercept_clues(self, opponent_clues: Clue, context: TeamContext) -> Code:
         """Attempt to intercept the opposing team's clues using the command line.
 
         Args:
             opponent_clues (Clue): The clues provided by the opposing team.
             context (TeamContext): Relevant information the Interepter's decision may be guided by.
 
         Returns:
             Code: The intercepted code numbers based on the opposing team's clues.
         """
-        print(f"You are Intercepter on team {TeamName(context.team_name)}")
-        print(f"Notesheet: {context.game.notesheet}")
-        print(f"Scoresheet: {context.game.data}")
+        self.print_context(context)
         print(f"Opponent Clues : {opponent_clues}")
-        n = context.num_opponent_keywords
-        print(f"Number of Opponent Keywords: {n}")
-        code = []
-        for clue in opponent_clues:
-            code_num = None
-            while code_num is None:
-                try:
-                    code_num = int(input(f"Code number for clue {clue}: "))
-                except ValueError:
-                    pass
-                if code_num is None or code_num not in range(n):
-                    print(f"Code num must lie in range [0 - {n}).")
-                    code_num = None
-            code.append(code_num)
-        return tuple(code)
+        code = tuple(self.get_code_num(clue, context) for clue in opponent_clues)
+        return code
 
 class CommandLineGuesser(Guesser):
     """A teammate who attempts to decipher their team's clues using the command line. """
 
+    def print_context(self, context: TeamContext):
+        """Print information for the developer to know how to interact through the command line.
+
+        Args:
+            context (TeamContext): Relevant information to the developer. 
+        """
+        print("=" * 12)
+        print(f"You are Guesser on team {TeamName(context.team_name)}")
+        print(f"Keywords: {context.keywords}")
+        print(f"Notesheet: {context.game.notesheet}")
+        print(f"Scoresheet: {context.game.data}")
+
+    def get_code_num(self, clue: str, context: TeamContext) -> int:
+        """Attempt to decipher a single clue using the command line.
+
+        Args:
+            clue (str): The clue provided by the opposing team.
+            context (TeamContext): Relevant information the Guesser's decision may be guided by. 
+
+        Returns:
+            int: The guessed code number based on the team's clue.
+        """
+        code_num = None
+        while code_num is None:
+            try:
+                code_num = int(input(f"Code number for clue {clue}: "))
+            except ValueError:
+                pass
+            if code_num is None or code_num not in range(len(context.keywords)):
+                print(f"Code num must lie in range [0 - {len(context.keywords)}).")
+                code_num = None
+        return code_num
+
     def decipher_clues(self, clues: Clue, context: TeamContext) -> Code:
         """Attempt to decipher the team's clues using the command line.
 
         Args:
             clues (Clue): The clues provided by the Guesser's team.
             context (TeamContext): Relevant information the Guesser's decision may be guided by. 
 
         Returns:
             Code: The guessed code numbers based on the team's clues.
         """
-        print(f"You are Guesser on team {TeamName(context.team_name)}")
-        print(f"Notesheet: {context.game.notesheet}")
-        print(f"Scoresheet: {context.game.data}")
+        self.print_context(context)
         print(f"Clues : {clues}")
-        n = len(context.keywords)
-        print(f"Number of Keywords: {n}")
-        code = []
-        for clue in clues:
-            code_num = None
-            while code_num is None:
-                try:
-                    code_num = int(input(f"Code number for clue {clue}: "))
-                except ValueError:
-                    pass
-                if code_num is None or code_num not in range(n + 1):
-                    print(f"Code num must lie in range [0 - {n}).")
-                    code_num = None
-            code.append(code_num)
-        return tuple(code)
+        code = tuple(self.get_code_num(clue, context) for clue in clues)
+        return code
 
 CommandLineTeam = lambda keywords: Team(
                                 keywords=keywords,
                                 encryptor=CommandLineEncryptor(),
                                 intercepter=CommandLineIntercepter(),
                                 guesser=CommandLineGuesser()
                             )
```

### Comparing `decryptogame-1.0.0/src/decryptogame.egg-info/PKG-INFO` & `decryptogame-1.0.1/src/decryptogame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 1.0.0
+Version: 1.0.1
 Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
 Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
```

### Comparing `decryptogame-1.0.0/tests/test_components.py` & `decryptogame-1.0.1/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/tests/test_game.py` & `decryptogame-1.0.1/tests/test_game.py`

 * *Files identical despite different names*

### Comparing `decryptogame-1.0.0/tests/test_generators.py` & `decryptogame-1.0.1/tests/test_generators.py`

 * *Files identical despite different names*

