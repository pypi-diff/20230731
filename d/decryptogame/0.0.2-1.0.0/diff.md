# Comparing `tmp/decryptogame-0.0.2.tar.gz` & `tmp/decryptogame-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decryptogame-0.0.2.tar", last modified: Tue Jun  6 09:28:45 2023, max compression
+gzip compressed data, was "decryptogame-1.0.0.tar", last modified: Sun Jul 30 21:13:06 2023, max compression
```

## Comparing `decryptogame-0.0.2.tar` & `decryptogame-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.159469 decryptogame-0.0.2/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-0.0.2/LICENSE
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1344 2023-06-06 09:28:45.158337 decryptogame-0.0.2/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      842 2023-06-06 07:49:38.000000 decryptogame-0.0.2/README.md
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      672 2023-06-06 09:27:13.000000 decryptogame-0.0.2/pyproject.toml
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-06-06 09:28:45.159646 decryptogame-0.0.2/setup.cfg
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.141311 decryptogame-0.0.2/src/
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.146958 decryptogame-0.0.2/src/decryptogame/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        0 2023-06-04 09:04:03.000000 decryptogame-0.0.2/src/decryptogame/__init__.py
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1044 2023-06-06 09:21:53.000000 decryptogame-0.0.2/src/decryptogame/game.py
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.153987 decryptogame-0.0.2/src/decryptogame.egg-info/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1344 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/PKG-INFO
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)      265 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/SOURCES.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/dependency_links.txt
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-06-06 09:28:45.000000 decryptogame-0.0.2/src/decryptogame.egg-info/top_level.txt
-drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-06-06 09:28:45.155337 decryptogame-0.0.2/tests/
--rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2674 2023-06-06 09:20:50.000000 decryptogame-0.0.2/tests/test_game.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.046874 decryptogame-1.0.0/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)    35149 2023-06-02 04:55:47.000000 decryptogame-1.0.0/LICENSE
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-30 21:13:06.045104 decryptogame-1.0.0/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      780 2023-07-30 21:10:07.000000 decryptogame-1.0.0/README.md
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      773 2023-07-30 21:09:47.000000 decryptogame-1.0.0/pyproject.toml
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       38 2023-07-30 21:13:06.047193 decryptogame-1.0.0/setup.cfg
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:05.995707 decryptogame-1.0.0/src/
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.023007 decryptogame-1.0.0/src/decryptogame/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      147 2023-07-16 21:46:14.000000 decryptogame-1.0.0/src/decryptogame/__init__.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     2213 2023-07-29 07:32:34.000000 decryptogame-1.0.0/src/decryptogame/components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     7193 2023-07-29 07:49:55.000000 decryptogame-1.0.0/src/decryptogame/end_criteria.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6833 2023-07-30 20:42:07.000000 decryptogame-1.0.0/src/decryptogame/game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3627 2023-07-29 07:56:45.000000 decryptogame-1.0.0/src/decryptogame/generators.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.031183 decryptogame-1.0.0/src/decryptogame/official_words/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     4745 2023-07-29 06:33:23.000000 decryptogame-1.0.0/src/decryptogame/official_words/english.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3658 2023-07-30 20:36:21.000000 decryptogame-1.0.0/src/decryptogame/play.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     6741 2023-07-30 20:39:38.000000 decryptogame-1.0.0/src/decryptogame/teams.py
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.029190 decryptogame-1.0.0/src/decryptogame.egg-info/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1375 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/PKG-INFO
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      504 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/SOURCES.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)        1 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/dependency_links.txt
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)       13 2023-07-30 21:13:05.000000 decryptogame-1.0.0/src/decryptogame.egg-info/top_level.txt
+drwxr-xr-x   0 jadenrodriguez   (501) staff       (20)        0 2023-07-30 21:13:06.042047 decryptogame-1.0.0/tests/
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     1468 2023-07-29 05:55:47.000000 decryptogame-1.0.0/tests/test_components.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)     3926 2023-07-30 20:48:01.000000 decryptogame-1.0.0/tests/test_game.py
+-rw-r--r--   0 jadenrodriguez   (501) staff       (20)      943 2023-07-29 07:15:17.000000 decryptogame-1.0.0/tests/test_generators.py
```

### Comparing `decryptogame-0.0.2/LICENSE` & `decryptogame-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decryptogame-0.0.2/PKG-INFO` & `decryptogame-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 0.0.2
-Summary: A non-official implementation of a Decrypto-style game
+Version: 1.0.0
+Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
+Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
-# Source code
-
-https://github.com/YaBoiSkinnyP/decryptogame/
-
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

### Comparing `decryptogame-0.0.2/README.md` & `decryptogame-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
-# Source code
-
-https://github.com/YaBoiSkinnyP/decryptogame/
-
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

### Comparing `decryptogame-0.0.2/src/decryptogame.egg-info/PKG-INFO` & `decryptogame-1.0.0/src/decryptogame.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: decryptogame
-Version: 0.0.2
-Summary: A non-official implementation of a Decrypto-style game
+Version: 1.0.0
+Summary: A non-official implementation of a Decrypto-style game for simulation and AI work.
 Author-email: Jaden Rodriguez <jadenrodriguez7@gmail.com>
+Project-URL: Homepage, https://github.com/YaBoiSkinnyP/decryptogame/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decryptogame
 A non-official implementation of a Decrypto-style game
 
-# Source code
-
-https://github.com/YaBoiSkinnyP/decryptogame/
-
 # Official Authorization
 This implementation may be used so long as its usage satisfies the following criteria:
 
 - it does not use/reproduce, in any manner, Decrypto's logo, illustration or visual identity of the game
 
 - it does not use/reproduce, in any manner, Scorpion Masque’s logo
```

