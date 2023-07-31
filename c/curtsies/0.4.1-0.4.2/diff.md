# Comparing `tmp/curtsies-0.4.1.tar.gz` & `tmp/curtsies-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curtsies-0.4.1.tar", last modified: Wed Oct  5 21:47:31 2022, max compression
+gzip compressed data, was "curtsies-0.4.2.tar", last modified: Mon Jul 31 20:18:29 2023, max compression
```

## Comparing `curtsies-0.4.1.tar` & `curtsies-0.4.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:31.333721 curtsies-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-10-05 21:47:27.000000 curtsies-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-10-05 21:47:27.000000 curtsies-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-10-05 21:47:31.333721 curtsies-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-10-05 21:47:27.000000 curtsies-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:31.325720 curtsies-0.4.1/curtsies/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/configfile_keynames.py
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/curtsieskeys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5220 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/escseqparse.py
--rw-r--r--   0 runner    (1001) docker     (121)    12131 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1045 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/fmtfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31553 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/formatstring.py
--rw-r--r--   0 runner    (1001) docker     (121)    10977 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/formatstringarray.py
--rw-r--r--   0 runner    (1001) docker     (121)    15187 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/input.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/termformatconstants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/termhelpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    21412 2022-10-05 21:47:27.000000 curtsies-0.4.1/curtsies/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:31.329720 curtsies-0.4.1/curtsies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-05 21:47:31.000000 curtsies-0.4.1/curtsies.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:31.333721 curtsies-0.4.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2519 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/chat.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/curses_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_fullscreen_window.py
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_fullscreen_with_input.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_input_paste.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_input_timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_scrolling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/demo_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/fps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3495 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/gameexample.py
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/initial_input.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/initial_input_with_cursor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/quickstart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/realtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/snake.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/sumtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1329 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/testcache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4470 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/tictactoeexample.py
--rw-r--r--   0 runner    (1001) docker     (121)     6403 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/tron.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6791 2022-10-05 21:47:27.000000 curtsies-0.4.1/examples/tttplaybitboard.py
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-10-05 21:47:27.000000 curtsies-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-05 21:47:31.337720 curtsies-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-10-05 21:47:27.000000 curtsies-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-05 21:47:31.333721 curtsies-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_configfile_keynames.py
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)    23709 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_fmtstr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4156 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (121)     6007 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     1742 2022-10-05 21:47:27.000000 curtsies-0.4.1/tests/test_window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:29.564929 curtsies-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-31 20:18:21.000000 curtsies-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-31 20:18:21.000000 curtsies-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-31 20:18:29.564929 curtsies-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-31 20:18:21.000000 curtsies-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:29.560928 curtsies-0.4.2/curtsies/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/configfile_keynames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/curtsieskeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/escseqparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/fmtfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31543 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/formatstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/formatstringarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/termformatconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/termhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-07-31 20:18:21.000000 curtsies-0.4.2/curtsies/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:29.560928 curtsies-0.4.2/curtsies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-31 20:18:29.000000 curtsies-0.4.2/curtsies.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:29.564929 curtsies-0.4.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/curses_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_fullscreen_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_fullscreen_with_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_input_paste.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_input_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_scrolling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/demo_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/fps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/gameexample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/initial_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/initial_input_with_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/quickstart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/snake.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/sumtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/testcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/tictactoeexample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/tron.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6791 2023-07-31 20:18:21.000000 curtsies-0.4.2/examples/tttplaybitboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-31 20:18:21.000000 curtsies-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-31 20:18:29.568929 curtsies-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-31 20:18:21.000000 curtsies-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 20:18:29.564929 curtsies-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_configfile_keynames.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23658 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_fmtstr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-31 20:18:21.000000 curtsies-0.4.2/tests/test_window.py
```

### Comparing `curtsies-0.4.1/LICENSE` & `curtsies-0.4.2/LICENSE`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 The MIT License (MIT)
 
 Copyright (c) 2014 Thomas Ballinger
+Copyright (c) 2020-2023 Sebastian Ramacher
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `curtsies-0.4.1/PKG-INFO` & `curtsies-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtsies
-Version: 0.4.1
+Version: 0.4.2
 Summary: Curses-like terminal wrapper, with colored strings!
 Home-page: https://github.com/bpython/curtsies
 Author: Thomas Ballinger
 Author-email: thomasballinger@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `curtsies-0.4.1/README.md` & `curtsies-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/configfile_keynames.py` & `curtsies-0.4.2/curtsies/configfile_keynames.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 SPECIALS = {
     "C-[": "<ESC>",
     "C-^": "<Ctrl-6>",
     "C-_": "<Ctrl-/>",
 }
 
+
 # TODO make a precalculated version of this
 class KeyMap:
     """Maps config file key syntax to Curtsies names"""
 
     def __getitem__(self, key: str) -> Tuple[str, ...]:
         if not key:  # Unbound key
             return ()
```

### Comparing `curtsies-0.4.1/curtsies/curtsieskeys.py` & `curtsies-0.4.2/curtsies/curtsieskeys.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/escseqparse.py` & `curtsies-0.4.2/curtsies/escseqparse.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/events.py` & `curtsies-0.4.2/curtsies/events.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/fmtfuncs.py` & `curtsies-0.4.2/curtsies/fmtfuncs.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/formatstring.py` & `curtsies-0.4.2/curtsies/formatstring.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,20 +69,18 @@
     "bg": lambda s, v: seq(v) + s + seq(RESET_BG),
 }
 
 
 class FrozenAttributes(Dict[str, Union[int, bool]]):
     """Immutable dictionary class for format string attributes"""
 
-    @no_type_check
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Union[int, bool]) -> None:
         raise Exception("Cannot change value.")
 
-    @no_type_check
-    def update(self, *args, **kwds):
+    def update(self, *args: Any, **kwds: Any) -> None:
         raise Exception("Cannot change value.")
 
     def extend(self, dictlike: Mapping[str, Union[int, bool]]) -> "FrozenAttributes":
         return FrozenAttributes(chain(self.items(), dictlike.items()))
 
     def remove(self, *keys: str) -> "FrozenAttributes":
         return FrozenAttributes((k, v) for k, v in self.items() if k not in keys)
@@ -201,27 +199,27 @@
 
 class ChunkSplitter:
     """
     View of a Chunk for breaking it into smaller Chunks.
     """
 
     def __init__(self, chunk: Chunk) -> None:
+        self.reinit(chunk)
+
+    def reinit(self, chunk: Chunk) -> None:
+        """Reuse an existing Splitter instance for speed."""
+        # TODO benchmark to prove this is worthwhile
         self.chunk = chunk
         self.internal_offset = 0  # index into chunk.s
         self.internal_width = 0  # width of chunks.s[:self.internal_offset]
         divides = [0]
         for c in self.chunk.s:
             divides.append(divides[-1] + wcwidth(c))
         self.divides = divides
 
-    def reinit(self, chunk: Chunk) -> None:
-        """Reuse an existing Splitter instance for speed."""
-        # TODO benchmark to prove this is worthwhile
-        self.__init__(chunk)  # type: ignore
-
     def request(self, max_width: int) -> Optional[Tuple[int, Chunk]]:
         """Requests a sub-chunk of max_width or shorter. Returns None if no chunks left."""
         if max_width < 1:
             raise ValueError("requires positive integer max_width")
 
         s = self.chunk.s
         length = len(s)
@@ -559,15 +557,15 @@
             return sum((self for _ in range(other)), FmtStr())
 
         return NotImplemented
 
     # TODO ensure empty FmtStr isn't a problem
 
     @property
-    def shared_atts(self) -> Mapping[str, Union[int, bool]]:
+    def shared_atts(self) -> Dict[str, Union[int, bool]]:
         """Gets atts shared among all nonzero length component Chunks"""
         # TODO cache this, could get ugly for large FmtStrs
         atts = {}
         first = self.chunks[0]
         for att in sorted(first.atts):
             # TODO how to write this without the '???'?
             if all(
```

### Comparing `curtsies-0.4.1/curtsies/formatstringarray.py` & `curtsies-0.4.2/curtsies/formatstringarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from .formatstring import fmtstr
 from .formatstring import normalize_slice
 from .formatstring import FmtStr
 
 from typing import (
     Any,
+    Optional,
     Union,
     List,
     Sequence,
     overload,
     Tuple,
     cast,
     no_type_check,
@@ -245,38 +246,42 @@
             for a_line, b_line, a_len, b_len in zip(
                 a_rows, b_rows, a_lengths, b_lengths
             )
         )
 
 
 def fsarray(
-    strings: Sequence[Union[FmtStr, str]], *args: Any, **kwargs: Any
+    strings: Sequence[Union[FmtStr, str]],
+    width: Optional[int] = None,
+    *args: Any,
+    **kwargs: Any,
 ) -> FSArray:
     """fsarray(list_of_FmtStrs_or_strings, width=None) -> FSArray
 
     Returns a new FSArray of width of the maximum size of the provided
     strings, or width provided, and height of the number of strings provided.
     If a width is provided, raises a ValueError if any of the strings
     are of length greater than this width"""
 
     strings = list(strings)
-    if "width" in kwargs:
-        width = kwargs["width"]
-        del kwargs["width"]
+    if width is not None:
         if strings and any(len(s) > width for s in strings):
             raise ValueError(f"Those strings won't fit for width {width}")
     else:
         width = max(len(s) for s in strings) if strings else 0
-    fstrings = [
-        s if isinstance(s, FmtStr) else fmtstr(s, *args, **kwargs) for s in strings
-    ]
-    arr = FSArray(len(fstrings), width, *args, **kwargs)
+    arr = FSArray(len(strings), width, *args, **kwargs)
     rows = [
         fs.setslice_with_length(0, len(s), s, width)
-        for fs, s in zip(arr.rows, fstrings)
+        for fs, s in zip(
+            arr.rows,
+            (
+                s if isinstance(s, FmtStr) else fmtstr(s, *args, **kwargs)
+                for s in strings
+            ),
+        )
     ]
     arr.rows = rows
     return arr
 
 
 def simple_format(x: Union[FSArray, Sequence[FmtStr]]) -> str:
     return "\n".join(str(l) for l in x)
```

### Comparing `curtsies-0.4.1/curtsies/input.py` & `curtsies-0.4.2/curtsies/input.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/termformatconstants.py` & `curtsies-0.4.2/curtsies/termformatconstants.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/termhelpers.py` & `curtsies-0.4.2/curtsies/termhelpers.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies/window.py` & `curtsies-0.4.2/curtsies/window.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/curtsies.egg-info/PKG-INFO` & `curtsies-0.4.2/curtsies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curtsies
-Version: 0.4.1
+Version: 0.4.2
 Summary: Curses-like terminal wrapper, with colored strings!
 Home-page: https://github.com/bpython/curtsies
 Author: Thomas Ballinger
 Author-email: thomasballinger@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `curtsies-0.4.1/curtsies.egg-info/SOURCES.txt` & `curtsies-0.4.2/curtsies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/chat.py` & `curtsies-0.4.2/examples/chat.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/demo_fullscreen_with_input.py` & `curtsies-0.4.2/examples/demo_fullscreen_with_input.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/demo_input_paste.py` & `curtsies-0.4.2/examples/demo_input_paste.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/demo_input_timeout.py` & `curtsies-0.4.2/examples/demo_input_timeout.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/demo_scrolling.py` & `curtsies-0.4.2/examples/demo_scrolling.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/demo_window.py` & `curtsies-0.4.2/examples/demo_window.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/fps.py` & `curtsies-0.4.2/examples/fps.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/gameexample.py` & `curtsies-0.4.2/examples/gameexample.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/initial_input_with_cursor.py` & `curtsies-0.4.2/examples/initial_input_with_cursor.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/quickstart.py` & `curtsies-0.4.2/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/realtime.py` & `curtsies-0.4.2/examples/realtime.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/simple.py` & `curtsies-0.4.2/examples/simple.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/snake.py` & `curtsies-0.4.2/examples/snake.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/testcache.py` & `curtsies-0.4.2/examples/testcache.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/tictactoeexample.py` & `curtsies-0.4.2/examples/tictactoeexample.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/tron.py` & `curtsies-0.4.2/examples/tron.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/examples/tttplaybitboard.py` & `curtsies-0.4.2/examples/tttplaybitboard.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/setup.cfg` & `curtsies-0.4.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = Curses-like terminal wrapper, with colored strings!
 long_description = file: README.md,
 long_description_content_type = text/markdown
 url = https://github.com/bpython/curtsies
 author = Thomas Ballinger
 author_email = thomasballinger@gmail.com
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: POSIX
 	Programming Language :: Python
```

### Comparing `curtsies-0.4.1/tests/test_configfile_keynames.py` & `curtsies-0.4.2/tests/test_configfile_keynames.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/tests/test_events.py` & `curtsies-0.4.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/tests/test_fmtstr.py` & `curtsies-0.4.2/tests/test_fmtstr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import sys
 import unittest
 from curtsies.formatstring import (
     FmtStr,
     fmtstr,
     Chunk,
     linesplit,
     normalize_slice,
@@ -368,15 +367,15 @@
     def test_normal_chars(self) -> None:
         fmtstr("a", "blue")
         str(fmtstr("a", "blue"))
         self.assertTrue(True)
 
     def test_funny_chars(self) -> None:
         fmtstr("⁇", "blue")
-        str(Chunk("⁇", {"fg": "blue"}))
+        str(Chunk("⁇", {"fg": 34}))
         str(fmtstr("⁇", "blue"))
         self.assertTrue(True)
 
     def test_right_sequence_in_py3(self) -> None:
         red_on_blue = fmtstr("hello", "red", "on_blue")
         blue_on_red = fmtstr("there", fg="blue", bg="red")
         green_s = fmtstr("!", "green")
@@ -397,15 +396,14 @@
         self.assertEqual(len(fmtstr(fmtstr("┌─"))), len(fmtstr("┌─")))
         self.assertEqual(fmtstr(fmtstr("┌─")), fmtstr("┌─"))
         # TODO should we make this one work?
         # always coerce everything to unicode?
         # self.assertEqual(len(fmtstr('┌─')), 2)
 
     def test_len_of_unicode_in_fsarray(self) -> None:
-
         fsa = FSArray(3, 2)
         fsa.rows[0] = fsa.rows[0].setslice_with_length(0, 2, "┌─", 2)
         self.assertEqual(fsa.shape, (3, 2))
         fsa.rows[0] = fsa.rows[0].setslice_with_length(0, 2, fmtstr("┌─", "blue"), 2)
         self.assertEqual(fsa.shape, (3, 2))
 
     def test_add_unicode_to_byte(self) -> None:
@@ -555,16 +553,15 @@
     def test_no_hanging_space(self) -> None:
         a = FSArray(4, 2)
         self.assertEqual(len(a.rows[0]), 0)
 
     def test_assignment_working(self) -> None:
         t = FSArray(10, 10)
         t[2, 2] = "a"
-        # TODO: is this supposed to check something?
-        t[2, 2] == "a"
+        self.assertEqual(t[2, 2], ["a"])
 
     def test_normalize_slice(self) -> None:
         class SliceBuilder:
             def __getitem__(self, slice: slice) -> slice:
                 return slice
 
         Slice = SliceBuilder()
```

### Comparing `curtsies-0.4.1/tests/test_input.py` & `curtsies-0.4.2/tests/test_input.py`

 * *Files identical despite different names*

### Comparing `curtsies-0.4.1/tests/test_terminal.py` & `curtsies-0.4.2/tests/test_terminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import functools
 import locale
 import os
 import sys
 import unittest
 
 from io import StringIO
 from unittest import skipUnless, skipIf, expectedFailure
@@ -150,15 +149,14 @@
         with self.window:
             self.window.render_to_terminal(["hi", "there"], cursor_pos=(2, 4))
             self.assertEqual(self.window.get_cursor_position(), (2, 4))
 
     # This isn't passing locally for me anymore :/
     @expectedFailure
     def test_inital_cursor_position(self):
-
         self.screen.cursor.y += 1
         with self.window:
             self.assertEqual(self.window.top_usable_row, 1)
             self.window.render_to_terminal(["hi", "there"])
             self.assertEqual(self.screen.display, ["      ", "hi    ", "there "])
```

### Comparing `curtsies-0.4.1/tests/test_window.py` & `curtsies-0.4.2/tests/test_window.py`

 * *Files identical despite different names*

