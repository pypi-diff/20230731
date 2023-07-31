# Comparing `tmp/tuiview-0.1.0a1.tar.gz` & `tmp/tuiview-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuiview-0.1.0a1.tar", last modified: Fri Jul 28 07:17:29 2023, max compression
+gzip compressed data, was "tuiview-0.1.0a2.tar", last modified: Mon Jul 31 03:15:06 2023, max compression
```

## Comparing `tuiview-0.1.0a1.tar` & `tuiview-0.1.0a2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.041591 tuiview-0.1.0a1/
--rw-r--r--   0 root         (0) root         (0)    34487 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    45390 2023-07-28 07:17:29.037591 tuiview-0.1.0a1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5003 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/README.md
--rw-r--r--   0 root         (0) root         (0)     4673 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 07:17:29.041591 tuiview-0.1.0a1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.029591 tuiview-0.1.0a1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.033591 tuiview-0.1.0a1/src/tuiview/
--rw-r--r--   0 root         (0) root         (0)       64 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.033591 tuiview-0.1.0a1/src/tuiview/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      183 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1295 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/__pycache__/__main__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-28 07:17:08.000000 tuiview-0.1.0a1/src/tuiview/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-28 07:17:08.000000 tuiview-0.1.0a1/src/tuiview/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.037591 tuiview-0.1.0a1/src/tuiview/cmd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.037591 tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/
--rw-r--r--   0 root         (0) root         (0)    10871 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/git.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2268 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/grep.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     9640 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/pastel.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2161 2023-07-28 07:10:27.000000 tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/rsync.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    14040 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/cmd/git.py
--rw-r--r--   0 root         (0) root         (0)     3185 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/cmd/grep.py
--rw-r--r--   0 root         (0) root         (0)    14479 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/cmd/pastel.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/cmd/rsync.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/src/tuiview/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.033591 tuiview-0.1.0a1/src/tuiview.egg-info/
--rw-r--r--   0 root         (0) root         (0)    45390 2023-07-28 07:17:28.000000 tuiview-0.1.0a1/src/tuiview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      805 2023-07-28 07:17:29.000000 tuiview-0.1.0a1/src/tuiview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 07:17:28.000000 tuiview-0.1.0a1/src/tuiview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-07-28 07:17:28.000000 tuiview-0.1.0a1/src/tuiview.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      560 2023-07-28 07:17:28.000000 tuiview-0.1.0a1/src/tuiview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-28 07:17:28.000000 tuiview-0.1.0a1/src/tuiview.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 07:17:29.037591 tuiview-0.1.0a1/tests/
--rw-r--r--   0 root         (0) root         (0)      608 2023-07-28 07:09:39.000000 tuiview-0.1.0a1/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.349070 tuiview-0.1.0a2/
+-rw-r--r--   0 root         (0) root         (0)    34487 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    45336 2023-07-31 03:15:06.349070 tuiview-0.1.0a2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4949 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/README.md
+-rw-r--r--   0 root         (0) root         (0)     4673 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 03:15:06.349070 tuiview-0.1.0a2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.341070 tuiview-0.1.0a2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.341070 tuiview-0.1.0a2/src/tuiview/
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.345070 tuiview-0.1.0a2/src/tuiview/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-31 03:08:02.000000 tuiview-0.1.0a2/src/tuiview/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-07-31 03:08:02.000000 tuiview-0.1.0a2/src/tuiview/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-31 03:14:45.000000 tuiview-0.1.0a2/src/tuiview/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-31 03:14:45.000000 tuiview-0.1.0a2/src/tuiview/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.345070 tuiview-0.1.0a2/src/tuiview/cmd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.349070 tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)    10732 2023-07-31 03:08:03.000000 tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/git.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-31 03:08:03.000000 tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/grep.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     9501 2023-07-31 03:08:03.000000 tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/pastel.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-31 03:08:03.000000 tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/rsync.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    13924 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/cmd/git.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/cmd/grep.py
+-rw-r--r--   0 root         (0) root         (0)    14362 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/cmd/pastel.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/cmd/rsync.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/src/tuiview/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.345070 tuiview-0.1.0a2/src/tuiview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    45336 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      805 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 03:15:06.000000 tuiview-0.1.0a2/src/tuiview.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:15:06.349070 tuiview-0.1.0a2/tests/
+-rw-r--r--   0 root         (0) root         (0)      608 2023-07-31 03:07:02.000000 tuiview-0.1.0a2/tests/test_main.py
```

### Comparing `tuiview-0.1.0a1/LICENSE` & `tuiview-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuiview-0.1.0a1/PKG-INFO` & `tuiview-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuiview
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A TUI for every CLI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -737,30 +737,27 @@
 
 ```
 ________________________________________________________________________________
 
 $ tv
 ________________________________________________________________________________
 
-Helpful Parameters:
-  -h, --help            Show this help message.
-  --help-all            Show help for all commands.
-  --version             Show the program version number.
-  --print-shell-completion {bash,zsh,tcsh}
-                        Print shell completion script.
-
-Optional Parameters:
-  -f, --from-file <value>
-                        > Type: Path, Default: None
+helpful parameters:
+  -h, --help  Show this help message.
+  --tui       Show Textual User Interface (TUI).
+  --help-all  Show help for all commands.
+  --version   Show the program version number.
 
-Commands:
+commands:
   <COMMAND>
-    git
+    from-file
     rsync
     grep
+    pastel
+    git
 ```
 
 ### Built-in Tools
 
 Launch the TUI of a known tool by providing its name:
 
 ```
@@ -775,14 +772,20 @@
 
 Notice how `git` has subcommands (`commit`, `merge`, ...). The TUI can be limited to a specific command by giving its name:
 
 ```
 tv git commit
 ```
 
+Any other arguments are parsed and passed-through to the TUI:
+
+```
+tv git commit -m 'hello' -m 'world'
+```
+
 ### Load from File
 
 Recall that argparse-tui allows us to use argparse as a specification language for Textual UIs. So, given a file defining and populating an argparse ArgumentParser with the variable name `parser`, you can feed it into `tuiview` and view the tui, dude :metal:
 
 For example, save the following to `echo.py`:
 
 ```python
@@ -797,20 +800,18 @@
     action="store_true",
     help="do not output the trailing newline",
 )
 ```
 
 > Hint: see this, and `ping.py` in the `examples/` folder
 
-Now display the TUI using: `tv -f echo.py`
+Now display the TUI using: `tv from-file echo.py`
 
-## Contribute
+## Support
 
 If you think this is as cool as I do and want to contribute and help curate files of argparse parsers for various CLI tools, rock on :metal:
 
-## Support
-
 If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/tuiview/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
 
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

### Comparing `tuiview-0.1.0a1/README.md` & `tuiview-0.1.0a2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,30 +46,27 @@
 
 ```
 ________________________________________________________________________________
 
 $ tv
 ________________________________________________________________________________
 
-Helpful Parameters:
-  -h, --help            Show this help message.
-  --help-all            Show help for all commands.
-  --version             Show the program version number.
-  --print-shell-completion {bash,zsh,tcsh}
-                        Print shell completion script.
-
-Optional Parameters:
-  -f, --from-file <value>
-                        > Type: Path, Default: None
+helpful parameters:
+  -h, --help  Show this help message.
+  --tui       Show Textual User Interface (TUI).
+  --help-all  Show help for all commands.
+  --version   Show the program version number.
 
-Commands:
+commands:
   <COMMAND>
-    git
+    from-file
     rsync
     grep
+    pastel
+    git
 ```
 
 ### Built-in Tools
 
 Launch the TUI of a known tool by providing its name:
 
 ```
@@ -84,14 +81,20 @@
 
 Notice how `git` has subcommands (`commit`, `merge`, ...). The TUI can be limited to a specific command by giving its name:
 
 ```
 tv git commit
 ```
 
+Any other arguments are parsed and passed-through to the TUI:
+
+```
+tv git commit -m 'hello' -m 'world'
+```
+
 ### Load from File
 
 Recall that argparse-tui allows us to use argparse as a specification language for Textual UIs. So, given a file defining and populating an argparse ArgumentParser with the variable name `parser`, you can feed it into `tuiview` and view the tui, dude :metal:
 
 For example, save the following to `echo.py`:
 
 ```python
@@ -106,20 +109,18 @@
     action="store_true",
     help="do not output the trailing newline",
 )
 ```
 
 > Hint: see this, and `ping.py` in the `examples/` folder
 
-Now display the TUI using: `tv -f echo.py`
+Now display the TUI using: `tv from-file echo.py`
 
-## Contribute
+## Support
 
 If you think this is as cool as I do and want to contribute and help curate files of argparse parsers for various CLI tools, rock on :metal:
 
-## Support
-
 If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/tuiview/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
 
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

### Comparing `tuiview-0.1.0a1/pyproject.toml` & `tuiview-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
 dependencies = [
     "typing-extensions; python_version<'3.10'",
-    "yapx[tui]>=0.2.2,<1",
+    "yapx[tui]>=0.2.4,<1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "python-lsp-server[rope]==1.*",
     "pylint==2.*",
     "pylint-pytest==1.*",
```

### Comparing `tuiview-0.1.0a1/src/tuiview/__pycache__/__main__.cpython-310.pyc` & `tuiview-0.1.0a2/src/tuiview/__pycache__/__main__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 07:09:39 2023 UTC, .py size: 1112 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-00000000: 6f0d 0d0a 0000 0000 b369 c364 5804 0000  o........i.dX...
+00000000: 6f0d 0d0a 0000 0000 5625 c764 1c04 0000  o.......V%.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 ac00 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 9e00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 6d08 5a08  d.l.m.Z.m.Z.m.Z.
-00000060: 6d09 5a09 0100 6400 6401 6c0a 5a0a 6400  m.Z...d.d.l.Z.d.
-00000070: 6405 6c0b 6d0c 5a0c 0100 6400 6406 6c0d  d.l.m.Z...d.d.l.
-00000080: 6d0e 5a0e 0100 6407 6408 6c0f 6d0f 5a0f  m.Z...d.d.l.m.Z.
-00000090: 0100 6409 650e 6509 6504 1900 650a 6a10  ..d.e.e.e...e.j.
-000000a0: 6401 640a 640b 6702 640c 8d02 6602 1900  d.d.d.g.d...f...
-000000b0: 6602 640d 640e 8404 5a11 6413 6410 6411  f.d.d...Z.d.d.d.
-000000c0: 8404 5a12 6513 6412 6b02 7254 6512 8300  ..Z.e.d.k.rTe...
-000000d0: 0100 6401 5300 6401 5300 2914 e900 0000  ..d.S.d.S.).....
-000000e0: 004e 2901 da0d 696d 706f 7274 5f6d 6f64  .N)...import_mod
-000000f0: 756c 6529 01da 0450 6174 6829 04da 0341  ule)...Path)...A
-00000100: 6e79 da08 4361 6c6c 6162 6c65 da04 4469  ny..Callable..Di
-00000110: 6374 da08 4f70 7469 6f6e 616c 2901 da0a  ct..Optional)...
-00000120: 696e 766f 6b65 5f74 7569 2901 da09 416e  invoke_tui)...An
-00000130: 6e6f 7461 7465 64e9 0100 0000 2901 da0b  notated.....)...
-00000140: 5f5f 7665 7273 696f 6e5f 5fda 0966 726f  __version__..fro
-00000150: 6d5f 6669 6c65 7a02 2d66 7a0b 2d2d 6672  m_filez.-fz.--fr
-00000160: 6f6d 2d66 696c 6529 01da 0566 6c61 6773  om-file)...flags
-00000170: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000180: 0004 0000 0043 0000 0073 3c00 0000 7c00  .....C...s<...|.
-00000190: 721c 7400 6a01 a002 7403 7c00 6a04 8301  r.t.j...t.|.j...
-000001a0: a101 0100 7405 7c00 6a06 8301 7d01 7407  ....t.|.j...}.t.
-000001b0: 7c01 6a08 8301 0100 7400 a009 6401 a101  |.j.....t...d...
-000001c0: 0100 6400 5300 6400 5300 2902 4e72 0100  ..d.S.d.S.).Nr..
-000001d0: 0000 290a da03 7379 73da 0470 6174 68da  ..)...sys..path.
-000001e0: 0661 7070 656e 64da 0373 7472 da06 7061  .append..str..pa
-000001f0: 7265 6e74 7202 0000 00da 0473 7465 6d72  rentr......stemr
-00000200: 0800 0000 da06 7061 7273 6572 da04 6578  ......parser..ex
-00000210: 6974 2902 720c 0000 00da 066d 6f64 756c  it).r......modul
-00000220: 65a9 0072 1700 0000 fa22 2f64 726f 6e65  e..r....."/drone
-00000230: 2f73 7263 2f73 7263 2f74 7569 7669 6577  /src/src/tuiview
-00000240: 2f5f 5f6d 6169 6e5f 5f2e 7079 da05 7365  /__main__.py..se
-00000250: 7475 700d 0000 0073 0c00 0000 0403 1201  tup....s........
-00000260: 0a01 0a02 0e02 04fa 7219 0000 00da 0672  ........r......r
-00000270: 6574 7572 6e63 0000 0000 0000 0000 0000  eturnc..........
-00000280: 0000 0300 0000 0700 0000 4300 0000 7376  ..........C...sv
-00000290: 0000 0069 007d 0074 0074 0183 016a 0264  ...i.}.t.t...j.d
-000002a0: 011b 00a0 0364 02a1 0144 005d 217d 017c  .....d...D.]!}.|
-000002b0: 016a 04a0 0564 03a1 0173 2d74 0664 047c  .j...d...s-t.d.|
-000002c0: 016a 026a 079b 0064 047c 016a 079b 009d  .j.j...d.|.j....
-000002d0: 0474 0864 058d 027d 027c 026a 097c 007c  .t.d...}.|.j.|.|
-000002e0: 016a 07a0 0a64 0364 06a1 023c 0071 0c74  .j...d.d...<.q.t
-000002f0: 0b6a 0c74 0d7c 0074 0e64 0767 0167 0064  .j.t.|.t.d.g.g.d
-00000300: 088d 0501 0064 0053 0029 094e da03 636d  .....d.S.).N..cm
-00000310: 647a 042a 2e70 79da 015f da01 2e29 01da  dz.*.py.._...)..
-00000320: 0770 6163 6b61 6765 da01 2d7a 062d 2d68  .package..-z.--h
-00000330: 656c 7029 04da 116e 616d 6564 5f73 7562  elp)...named_sub
-00000340: 636f 6d6d 616e 6473 5a0c 7072 6f67 5f76  commandsZ.prog_v
-00000350: 6572 7369 6f6e 5a0c 6465 6661 756c 745f  ersionZ.default_
-00000360: 6172 6773 5a09 7475 695f 666c 6167 7329  argsZ.tui_flags)
-00000370: 0f72 0300 0000 da08 5f5f 6669 6c65 5f5f  .r......__file__
-00000380: 7212 0000 00da 0467 6c6f 62da 046e 616d  r......glob..nam
-00000390: 65da 0a73 7461 7274 7377 6974 6872 0200  e..startswithr..
-000003a0: 0000 7213 0000 00da 0b5f 5f70 6163 6b61  ..r......__packa
-000003b0: 6765 5f5f da04 6d61 696e da07 7265 706c  ge__..main..repl
-000003c0: 6163 65da 0479 6170 78da 0372 756e 7219  ace..yapx..runr.
-000003d0: 0000 0072 0b00 0000 2903 7220 0000 00da  ...r....).r ....
-000003e0: 0178 5a0a 636d 645f 6d6f 6475 6c65 7217  .xZ.cmd_moduler.
-000003f0: 0000 0072 1700 0000 7218 0000 0072 2600  ...r....r....r&.
-00000400: 0000 1900 0000 7320 0000 0004 0118 020c  ......s ........
-00000410: 0102 0114 0102 0106 fe14 0402 8004 0202  ................
-00000420: 0102 0102 0104 0102 010a fb72 2600 0000  ...........r&...
-00000430: da08 5f5f 6d61 696e 5f5f 2902 721a 0000  ..__main__).r...
-00000440: 004e 2914 720e 0000 00da 0969 6d70 6f72  .N).r......impor
-00000450: 746c 6962 7202 0000 00da 0770 6174 686c  tlibr......pathl
-00000460: 6962 7203 0000 00da 0674 7970 696e 6772  ibr......typingr
-00000470: 0400 0000 7205 0000 0072 0600 0000 7207  ....r....r....r.
-00000480: 0000 0072 2800 0000 5a0c 6172 6770 6172  ...r(...Z.argpar
-00000490: 7365 5f74 7569 7208 0000 005a 0a79 6170  se_tuir....Z.yap
-000004a0: 782e 7479 7065 7372 0900 0000 720b 0000  x.typesr....r...
-000004b0: 00da 0361 7267 7219 0000 0072 2600 0000  ...argr....r&...
-000004c0: da08 5f5f 6e61 6d65 5f5f 7217 0000 0072  ..__name__r....r
-000004d0: 1700 0000 7217 0000 0072 1800 0000 da08  ....r....r......
-000004e0: 3c6d 6f64 756c 653e 0100 0000 731e 0000  <module>....s...
-000004f0: 0008 000c 010c 0118 0108 020c 010c 010c  ................
-00000500: 0202 031c 010a ff0a 0c08 140a 0104 ff    ...............
+00000060: 0100 6400 6401 6c09 5a09 6400 6405 6c0a  ..d.d.l.Z.d.d.l.
+00000070: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
+00000080: 0100 6407 6408 6c0e 6d0e 5a0e 0100 6409  ..d.d.l.m.Z...d.
+00000090: 650d 6504 6509 6a0f 640a 640b 8d01 6602  e.e.e.j.d.d...f.
+000000a0: 1900 6602 640c 640d 8404 5a10 6412 640f  ..f.d.d...Z.d.d.
+000000b0: 6410 8404 5a11 6512 6411 6b02 724d 6511  d...Z.e.d.k.rMe.
+000000c0: 8300 0100 6401 5300 6401 5300 2913 e900  ....d.S.d.S.)...
+000000d0: 0000 004e 2901 da0d 696d 706f 7274 5f6d  ...N)...import_m
+000000e0: 6f64 756c 6529 01da 0450 6174 6829 03da  odule)...Path)..
+000000f0: 0341 6e79 da08 4361 6c6c 6162 6c65 da04  .Any..Callable..
+00000100: 4469 6374 2901 da0a 696e 766f 6b65 5f74  Dict)...invoke_t
+00000110: 7569 2901 da09 416e 6e6f 7461 7465 64e9  ui)...Annotated.
+00000120: 0100 0000 2901 da0b 5f5f 7665 7273 696f  ....)...__versio
+00000130: 6e5f 5fda 0470 6174 6854 2901 da03 706f  n__..pathT)...po
+00000140: 7363 0000 0000 0000 0000 0100 0000 0300  sc..............
+00000150: 0000 0400 0000 4700 0000 7338 0000 0074  ......G...s8...t
+00000160: 006a 01a0 0274 037c 006a 0483 01a1 0101  .j...t.|.j......
+00000170: 0074 057c 006a 0683 017d 0274 077c 026a  .t.|.j...}.t.|.j
+00000180: 087c 0164 018d 0201 0074 00a0 0964 02a1  .|.d.....t...d..
+00000190: 0101 0064 0053 0029 034e 2901 5a08 636c  ...d.S.).N).Z.cl
+000001a0: 695f 6172 6773 7201 0000 0029 0ada 0373  i_argsr....)...s
+000001b0: 7973 720b 0000 00da 0661 7070 656e 64da  ysr......append.
+000001c0: 0373 7472 da06 7061 7265 6e74 7202 0000  .str..parentr...
+000001d0: 00da 0473 7465 6d72 0700 0000 da06 7061  ...stemr......pa
+000001e0: 7273 6572 da04 6578 6974 2903 720b 0000  rser..exit).r...
+000001f0: 00da 0461 7267 73da 066d 6f64 756c 65a9  ...args..module.
+00000200: 0072 1600 0000 fa22 2f64 726f 6e65 2f73  .r....."/drone/s
+00000210: 7263 2f73 7263 2f74 7569 7669 6577 2f5f  rc/src/tuiview/_
+00000220: 5f6d 6169 6e5f 5f2e 7079 da09 6672 6f6d  _main__.py..from
+00000230: 5f66 696c 650d 0000 0073 0800 0000 1201  _file....s......
+00000240: 0a01 0e02 0e02 7218 0000 00da 0672 6574  ......r......ret
+00000250: 7572 6e63 0000 0000 0000 0000 0000 0000  urnc............
+00000260: 0300 0000 0700 0000 4300 0000 7378 0000  ........C...sx..
+00000270: 0069 007d 0074 0074 0183 016a 0264 011b  .i.}.t.t...j.d..
+00000280: 00a0 0364 02a1 0144 005d 217d 017c 016a  ...d...D.]!}.|.j
+00000290: 04a0 0564 03a1 0173 2d74 0664 047c 016a  ...d...s-t.d.|.j
+000002a0: 026a 079b 0064 047c 016a 079b 009d 0474  .j...d.|.j.....t
+000002b0: 0864 058d 027d 027c 026a 097c 007c 016a  .d...}.|.j.|.|.j
+000002c0: 07a0 0a64 0364 06a1 023c 0071 0c74 0b6a  ...d.d...<.q.t.j
+000002d0: 0c74 0d67 017c 0074 0e64 0767 0167 0064  .t.g.|.t.d.g.g.d
+000002e0: 088d 0501 0064 0053 0029 094e da03 636d  .....d.S.).N..cm
+000002f0: 647a 042a 2e70 79da 015f da01 2e29 01da  dz.*.py.._...)..
+00000300: 0770 6163 6b61 6765 da01 2d7a 062d 2d68  .package..-z.--h
+00000310: 656c 7029 04da 116e 616d 6564 5f73 7562  elp)...named_sub
+00000320: 636f 6d6d 616e 6473 5a0c 7072 6f67 5f76  commandsZ.prog_v
+00000330: 6572 7369 6f6e 5a0c 6465 6661 756c 745f  ersionZ.default_
+00000340: 6172 6773 5a09 7475 695f 666c 6167 7329  argsZ.tui_flags)
+00000350: 0f72 0300 0000 da08 5f5f 6669 6c65 5f5f  .r......__file__
+00000360: 7210 0000 00da 0467 6c6f 62da 046e 616d  r......glob..nam
+00000370: 65da 0a73 7461 7274 7377 6974 6872 0200  e..startswithr..
+00000380: 0000 7211 0000 00da 0b5f 5f70 6163 6b61  ..r......__packa
+00000390: 6765 5f5f da04 6d61 696e da07 7265 706c  ge__..main..repl
+000003a0: 6163 65da 0479 6170 785a 0c72 756e 5f63  ace..yapxZ.run_c
+000003b0: 6f6d 6d61 6e64 7372 1800 0000 720a 0000  ommandsr....r...
+000003c0: 0029 0372 1f00 0000 da01 785a 0a63 6d64  .).r......xZ.cmd
+000003d0: 5f6d 6f64 756c 6572 1600 0000 7216 0000  _moduler....r...
+000003e0: 0072 1700 0000 7225 0000 0016 0000 0073  .r....r%.......s
+000003f0: 2000 0000 0401 1802 0c01 0201 1401 0201   ...............
+00000400: 06fe 1404 0280 0402 0401 0201 0201 0401  ................
+00000410: 0201 0afb 7225 0000 00da 085f 5f6d 6169  ....r%.....__mai
+00000420: 6e5f 5f29 0272 1900 0000 4e29 1372 0d00  n__).r....N).r..
+00000430: 0000 da09 696d 706f 7274 6c69 6272 0200  ....importlibr..
+00000440: 0000 da07 7061 7468 6c69 6272 0300 0000  ....pathlibr....
+00000450: da06 7479 7069 6e67 7204 0000 0072 0500  ..typingr....r..
+00000460: 0000 7206 0000 0072 2700 0000 5a0c 6172  ..r....r'...Z.ar
+00000470: 6770 6172 7365 5f74 7569 7207 0000 005a  gparse_tuir....Z
+00000480: 0a79 6170 782e 7479 7065 7372 0800 0000  .yapx.typesr....
+00000490: 720a 0000 00da 0361 7267 7218 0000 0072  r......argr....r
+000004a0: 2500 0000 da08 5f5f 6e61 6d65 5f5f 7216  %.....__name__r.
+000004b0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
+000004c0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+000004d0: 731a 0000 0008 000c 010c 0114 0108 020c  s...............
+000004e0: 010c 010c 021e 030a 0908 140a 0104 ff    ...............
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/git.cpython-310.pyc` & `tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/git.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 07:09:39 2023 UTC, .py size: 14040 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,680 +1,671 @@
-00000000: 6f0d 0d0a 0000 0000 b369 c364 d836 0000  o........i.d.6..
+00000000: 6f0d 0d0a 0000 0000 5625 c764 6436 0000  o.......V%.dd6..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
-00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6401 6c03 5a03 6400 6403 6c04  ..d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6405 6406 8400 5a08 6407 6408 8400  ..d.d...Z.d.d...
-00000070: 5a09 6409 640a 8400 5a0a 640b 6507 6502  Z.d.d...Z.d.e.e.
-00000080: 650b 1900 6503 6a0c 6401 640c 640d 8d02  e...e.j.d.d.d...
-00000090: 6602 1900 6602 640e 640f 8404 5a0d 6401  f...f.d.d...Z.d.
-000000a0: 5300 2910 e900 0000 004e 2901 da08 4f70  S.)......N)...Op
-000000b0: 7469 6f6e 616c 2901 da0a 696e 766f 6b65  tional)...invoke
-000000c0: 5f74 7569 2901 da09 416e 6e6f 7461 7465  _tui)...Annotate
-000000d0: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-000000e0: 0000 0700 0000 4300 0000 730a 0100 0064  ......C...s....d
-000000f0: 017c 005f 0064 027c 005f 017c 006a 0264  .|._.d.|._.|.j.d
-00000100: 0364 0464 0564 0664 0764 088d 0501 007c  .d.d.d.d.d.....|
-00000110: 006a 0264 0964 0a64 0b64 0c64 0d64 0e8d  .j.d.d.d.d.d.d..
-00000120: 0501 007c 006a 0264 0f64 1064 118d 0201  ...|.j.d.d.d....
-00000130: 007c 006a 0264 1264 1364 118d 0201 007c  .|.j.d.d.d.....|
-00000140: 006a 0264 1464 1564 0b64 0c64 1664 0e8d  .j.d.d.d.d.d.d..
-00000150: 0501 007c 006a 0264 1764 1864 1964 1a8d  ...|.j.d.d.d.d..
-00000160: 0301 007c 006a 0264 1b64 1c64 1d64 1a8d  ...|.j.d.d.d.d..
-00000170: 0301 007c 006a 0264 1e64 0b64 0c64 1f64  ...|.j.d.d.d.d.d
-00000180: 0e8d 0401 007c 006a 0264 2064 2164 0b64  .....|.j.d d!d.d
-00000190: 0c64 2264 0e8d 0501 007c 006a 0264 2364  .d"d.....|.j.d#d
-000001a0: 0b64 0c64 2464 0e8d 0401 007c 006a 0264  .d.d$d.....|.j.d
-000001b0: 2564 0b64 0c64 2664 0e8d 0401 007c 006a  %d.d.d&d.....|.j
-000001c0: 0264 2764 0b64 0c64 2864 0e8d 0401 007c  .d'd.d.d(d.....|
-000001d0: 006a 0264 2964 2a64 0b64 0c64 2b64 0e8d  .j.d)d*d.d.d+d..
-000001e0: 0501 007c 006a 0264 2c64 0b64 0c64 2d64  ...|.j.d,d.d.d-d
-000001f0: 0e8d 0401 0064 0053 0029 2e4e 7a0a 6769  .....d.S.).Nz.gi
-00000200: 742d 636f 6d6d 6974 7a20 5265 636f 7264  t-commitz Record
-00000210: 2063 6861 6e67 6573 2074 6f20 7468 6520   changes to the 
-00000220: 7265 706f 7369 746f 7279 7a02 2d6d 7a09  repositoryz.-mz.
-00000230: 2d2d 6d65 7373 6167 657a 053c 6d73 673e  --messagez.<msg>
-00000240: da06 6170 7065 6e64 7a82 5573 6520 7468  ..appendz.Use th
-00000250: 6520 6769 7665 6e20 3c6d 7367 3e20 6173  e given <msg> as
-00000260: 2074 6865 2063 6f6d 6d69 7420 6d65 7373   the commit mess
-00000270: 6167 652e 2049 6620 6d75 6c74 6970 6c65  age. If multiple
-00000280: 202d 6d20 6f70 7469 6f6e 7320 6172 6520   -m options are 
-00000290: 6769 7665 6e2c 2074 6865 6972 2076 616c  given, their val
-000002a0: 7565 7320 6172 6520 636f 6e63 6174 656e  ues are concaten
-000002b0: 6174 6564 2061 7320 7365 7061 7261 7465  ated as separate
-000002c0: 2070 6172 6167 7261 7068 732e 2903 da07   paragraphs.)...
-000002d0: 6d65 7461 7661 72da 0661 6374 696f 6eda  metavar..action.
-000002e0: 0468 656c 707a 022d 617a 052d 2d61 6c6c  .helpz.-az.--all
-000002f0: da0a 7374 6f72 655f 7472 7565 467a 8e54  ..store_trueFz.T
-00000300: 656c 6c20 7468 6520 636f 6d6d 616e 6420  ell the command 
-00000310: 746f 2061 7574 6f6d 6174 6963 616c 6c79  to automatically
-00000320: 2073 7461 6765 2066 696c 6573 2074 6861   stage files tha
-00000330: 7420 6861 7665 2062 6565 6e20 6d6f 6469  t have been modi
-00000340: 6669 6564 2061 6e64 2064 656c 6574 6564  fied and deleted
-00000350: 2c20 6275 7420 6e65 7720 6669 6c65 7320  , but new files 
-00000360: 796f 7520 6861 7665 206e 6f74 2074 6f6c  you have not tol
-00000370: 6420 4769 7420 6162 6f75 7420 6172 6520  d Git about are 
-00000380: 6e6f 7420 6166 6665 6374 6564 2e29 0372  not affected.).r
-00000390: 0700 0000 da07 6465 6661 756c 7472 0800  ......defaultr..
-000003a0: 0000 7a07 2d2d 6669 7875 707a 195b 2861  ..z.--fixupz.[(a
-000003b0: 6d65 6e64 7c72 6577 6f72 6429 3a5d 3c63  mend|reword):]<c
-000003c0: 6f6d 6d69 743e 2901 7206 0000 00fa 082d  ommit>).r......-
-000003d0: 2d73 7175 6173 687a 083c 636f 6d6d 6974  -squashz.<commit
-000003e0: 3efa 022d 6efa 0b2d 2d6e 6f2d 7665 7269  >..-n..--no-veri
-000003f0: 6679 7a8a 4279 2064 6566 6175 6c74 2c20  fyz.By default, 
-00000400: 7468 6520 7072 652d 636f 6d6d 6974 2061  the pre-commit a
-00000410: 6e64 2063 6f6d 6d69 742d 6d73 6720 686f  nd commit-msg ho
-00000420: 6f6b 7320 6172 6520 7275 6e2e 2057 6865  oks are run. Whe
-00000430: 6e20 616e 7920 6f66 202d 2d6e 6f2d 7665  n any of --no-ve
-00000440: 7269 6679 206f 7220 2d6e 2069 7320 6769  rify or -n is gi
-00000450: 7665 6e2c 2074 6865 7365 2061 7265 2062  ven, these are b
-00000460: 7970 6173 7365 642e 2053 6565 2061 6c73  ypassed. See als
-00000470: 6f20 6769 7468 6f6f 6b73 2835 292e fa08  o githooks(5)...
-00000480: 2d2d 6175 7468 6f72 7a08 3c61 7574 686f  --authorz.<autho
-00000490: 723e 6148 0100 004f 7665 7272 6964 6520  r>aH...Override 
-000004a0: 7468 6520 636f 6d6d 6974 2061 7574 686f  the commit autho
-000004b0: 722e 2053 7065 6369 6679 2061 6e20 6578  r. Specify an ex
-000004c0: 706c 6963 6974 2061 7574 686f 7220 7573  plicit author us
-000004d0: 696e 6720 7468 6520 7374 616e 6461 7264  ing the standard
-000004e0: 2041 2055 2054 686f 7220 3c61 7574 686f   A U Thor <autho
-000004f0: 7240 6578 616d 706c 652e 636f 6d3e 2066  r@example.com> f
-00000500: 6f72 6d61 742e 204f 7468 6572 7769 7365  ormat. Otherwise
-00000510: 203c 6175 7468 6f72 3e20 6973 2061 7373   <author> is ass
-00000520: 756d 6564 2074 6f20 6265 2061 2070 6174  umed to be a pat
-00000530: 7465 726e 2061 6e64 2069 7320 7573 6564  tern and is used
-00000540: 2074 6f20 7365 6172 6368 2066 6f72 2061   to search for a
-00000550: 6e20 6578 6973 7469 6e67 2063 6f6d 6d69  n existing commi
-00000560: 7420 6279 2074 6861 7420 6175 7468 6f72  t by that author
-00000570: 2028 692e 652e 2072 6576 2d6c 6973 7420   (i.e. rev-list 
-00000580: 2d2d 616c 6c20 2d69 202d 2d61 7574 686f  --all -i --autho
-00000590: 723d 3c61 7574 686f 723e 293b 2074 6865  r=<author>); the
-000005a0: 2063 6f6d 6d69 7420 6175 7468 6f72 2069   commit author i
-000005b0: 7320 7468 656e 2063 6f70 6965 6420 6672  s then copied fr
-000005c0: 6f6d 2074 6865 2066 6972 7374 2073 7563  om the first suc
-000005d0: 6820 636f 6d6d 6974 2066 6f75 6e64 2e29  h commit found.)
-000005e0: 0272 0600 0000 7208 0000 00fa 062d 2d64  .r....r......--d
-000005f0: 6174 657a 063c 6461 7465 3e7a 2c4f 7665  atez.<date>z,Ove
-00000600: 7272 6964 6520 7468 6520 6175 7468 6f72  rride the author
-00000610: 2064 6174 6520 7573 6564 2069 6e20 7468   date used in th
-00000620: 6520 636f 6d6d 6974 2e7a 0d2d 2d61 6c6c  e commit.z.--all
-00000630: 6f77 2d65 6d70 7479 7af3 5573 7561 6c6c  ow-emptyz.Usuall
-00000640: 7920 7265 636f 7264 696e 6720 6120 636f  y recording a co
-00000650: 6d6d 6974 2074 6861 7420 6861 7320 7468  mmit that has th
-00000660: 6520 6578 6163 7420 7361 6d65 2074 7265  e exact same tre
-00000670: 6520 6173 2069 7473 2073 6f6c 6520 7061  e as its sole pa
-00000680: 7265 6e74 2063 6f6d 6d69 7420 6973 2061  rent commit is a
-00000690: 206d 6973 7461 6b65 2c20 616e 6420 7468   mistake, and th
-000006a0: 6520 636f 6d6d 616e 6420 7072 6576 656e  e command preven
-000006b0: 7473 2079 6f75 2066 726f 6d20 6d61 6b69  ts you from maki
-000006c0: 6e67 2073 7563 6820 6120 636f 6d6d 6974  ng such a commit
-000006d0: 2e20 5468 6973 206f 7074 696f 6e20 6279  . This option by
-000006e0: 7061 7373 6573 2074 6865 2073 6166 6574  passes the safet
-000006f0: 792c 2061 6e64 2069 7320 7072 696d 6172  y, and is primar
-00000700: 696c 7920 666f 7220 7573 6520 6279 2066  ily for use by f
-00000710: 6f72 6569 676e 2053 434d 2069 6e74 6572  oreign SCM inter
-00000720: 6661 6365 2073 6372 6970 7473 2e7a 022d  face scripts.z.-
-00000730: 657a 062d 2d65 6469 747a d854 6865 206d  ez.--editz.The m
-00000740: 6573 7361 6765 2074 616b 656e 2066 726f  essage taken fro
-00000750: 6d20 6669 6c65 2077 6974 6820 2d46 2c20  m file with -F, 
-00000760: 636f 6d6d 616e 6420 6c69 6e65 2077 6974  command line wit
-00000770: 6820 2d6d 2c20 616e 6420 6672 6f6d 2063  h -m, and from c
-00000780: 6f6d 6d69 7420 6f62 6a65 6374 2077 6974  ommit object wit
-00000790: 6820 2d43 2061 7265 2075 7375 616c 6c79  h -C are usually
-000007a0: 2075 7365 6420 6173 2074 6865 2063 6f6d   used as the com
-000007b0: 6d69 7420 6c6f 6720 6d65 7373 6167 6520  mit log message 
-000007c0: 756e 6d6f 6469 6669 6564 2e20 5468 6973  unmodified. This
-000007d0: 206f 7074 696f 6e20 6c65 7473 2079 6f75   option lets you
-000007e0: 2066 7572 7468 6572 2065 6469 7420 7468   further edit th
-000007f0: 6520 6d65 7373 6167 6520 7461 6b65 6e20  e message taken 
-00000800: 6672 6f6d 2074 6865 7365 2073 6f75 7263  from these sourc
-00000810: 6573 2efa 092d 2d6e 6f2d 6564 6974 7a9b  es...--no-editz.
-00000820: 5573 6520 7468 6520 7365 6c65 6374 6564  Use the selected
-00000830: 2063 6f6d 6d69 7420 6d65 7373 6167 6520   commit message 
-00000840: 7769 7468 6f75 7420 6c61 756e 6368 696e  without launchin
-00000850: 6720 616e 2065 6469 746f 722e 2046 6f72  g an editor. For
-00000860: 2065 7861 6d70 6c65 2c20 6769 7420 636f   example, git co
-00000870: 6d6d 6974 202d 2d61 6d65 6e64 202d 2d6e  mmit --amend --n
-00000880: 6f2d 6564 6974 2061 6d65 6e64 7320 6120  o-edit amends a 
-00000890: 636f 6d6d 6974 2077 6974 686f 7574 2063  commit without c
-000008a0: 6861 6e67 696e 6720 6974 7320 636f 6d6d  hanging its comm
-000008b0: 6974 206d 6573 7361 6765 2e7a 072d 2d61  it message.z.--a
-000008c0: 6d65 6e64 6152 0300 0052 6570 6c61 6365  mendaR...Replace
-000008d0: 2074 6865 2074 6970 206f 6620 7468 6520   the tip of the 
-000008e0: 6375 7272 656e 7420 6272 616e 6368 2062  current branch b
-000008f0: 7920 6372 6561 7469 6e67 2061 206e 6577  y creating a new
-00000900: 2063 6f6d 6d69 742e 2054 6865 2072 6563   commit. The rec
-00000910: 6f72 6465 6420 7472 6565 2069 7320 7072  orded tree is pr
-00000920: 6570 6172 6564 2061 7320 7573 7561 6c20  epared as usual 
-00000930: 2869 6e63 6c75 6469 6e67 2074 6865 2065  (including the e
-00000940: 6666 6563 7420 6f66 2074 6865 202d 6920  ffect of the -i 
-00000950: 616e 6420 2d6f 206f 7074 696f 6e73 2061  and -o options a
-00000960: 6e64 2065 7870 6c69 6369 7420 7061 7468  nd explicit path
-00000970: 7370 6563 292c 2061 6e64 2074 6865 206d  spec), and the m
-00000980: 6573 7361 6765 2066 726f 6d20 7468 6520  essage from the 
-00000990: 6f72 6967 696e 616c 2063 6f6d 6d69 7420  original commit 
-000009a0: 6973 2075 7365 6420 6173 2074 6865 2073  is used as the s
-000009b0: 7461 7274 696e 6720 706f 696e 742c 2069  tarting point, i
-000009c0: 6e73 7465 6164 206f 6620 616e 2065 6d70  nstead of an emp
-000009d0: 7479 206d 6573 7361 6765 2c20 7768 656e  ty message, when
-000009e0: 206e 6f20 6f74 6865 7220 6d65 7373 6167   no other messag
-000009f0: 6520 6973 2073 7065 6369 6669 6564 2066  e is specified f
-00000a00: 726f 6d20 7468 6520 636f 6d6d 616e 6420  rom the command 
-00000a10: 6c69 6e65 2076 6961 206f 7074 696f 6e73  line via options
-00000a20: 2073 7563 6820 6173 202d 6d2c 202d 462c   such as -m, -F,
-00000a30: 202d 632c 2065 7463 2e20 5468 6520 6e65   -c, etc. The ne
-00000a40: 7720 636f 6d6d 6974 2068 6173 2074 6865  w commit has the
-00000a50: 2073 616d 6520 7061 7265 6e74 7320 616e   same parents an
-00000a60: 6420 6175 7468 6f72 2061 7320 7468 6520  d author as the 
-00000a70: 6375 7272 656e 7420 6f6e 6520 2874 6865  current one (the
-00000a80: 202d 2d72 6573 6574 2d61 7574 686f 7220   --reset-author 
-00000a90: 6f70 7469 6f6e 2063 616e 2063 6f75 6e74  option can count
-00000aa0: 6572 6d61 6e64 2074 6869 7329 2e20 4974  ermand this). It
-00000ab0: 2069 7320 6120 726f 7567 6820 6571 7569   is a rough equi
-00000ac0: 7661 6c65 6e74 2066 6f72 3a20 2420 6769  valent for: $ gi
-00000ad0: 7420 7265 7365 7420 2d2d 736f 6674 2048  t reset --soft H
-00000ae0: 4541 445e 2024 202e 2e2e 2064 6f20 736f  EAD^ $ ... do so
-00000af0: 6d65 7468 696e 6720 656c 7365 2074 6f20  mething else to 
-00000b00: 636f 6d65 2075 7020 7769 7468 2074 6865  come up with the
-00000b10: 2072 6967 6874 2074 7265 6520 2e2e 2e20   right tree ... 
-00000b20: 2420 6769 7420 636f 6d6d 6974 202d 6320  $ git commit -c 
-00000b30: 4f52 4947 5f48 4541 4420 6275 7420 6361  ORIG_HEAD but ca
-00000b40: 6e20 6265 2075 7365 6420 746f 2061 6d65  n be used to ame
-00000b50: 6e64 2061 206d 6572 6765 2063 6f6d 6d69  nd a merge commi
-00000b60: 742e 2059 6f75 2073 686f 756c 6420 756e  t. You should un
-00000b70: 6465 7273 7461 6e64 2074 6865 2069 6d70  derstand the imp
-00000b80: 6c69 6361 7469 6f6e 7320 6f66 2072 6577  lications of rew
-00000b90: 7269 7469 6e67 2068 6973 746f 7279 2069  riting history i
-00000ba0: 6620 796f 7520 616d 656e 6420 6120 636f  f you amend a co
-00000bb0: 6d6d 6974 2074 6861 7420 6861 7320 616c  mmit that has al
-00000bc0: 7265 6164 7920 6265 656e 2070 7562 6c69  ready been publi
-00000bd0: 7368 6564 2e20 2853 6565 2074 6865 2022  shed. (See the "
-00000be0: 5245 434f 5645 5249 4e47 2046 524f 4d20  RECOVERING FROM 
-00000bf0: 5550 5354 5245 414d 2052 4542 4153 4522  UPSTREAM REBASE"
-00000c00: 2073 6563 7469 6f6e 2069 6e20 6769 742d   section in git-
-00000c10: 7265 6261 7365 2831 292e 297a 112d 2d6e  rebase(1).)z.--n
-00000c20: 6f2d 706f 7374 2d72 6577 7269 7465 7a1d  o-post-rewritez.
-00000c30: 4279 7061 7373 2074 6865 2070 6f73 742d  Bypass the post-
-00000c40: 7265 7772 6974 6520 686f 6f6b 2efa 022d  rewrite hook...-
-00000c50: 71fa 072d 2d71 7569 6574 7a20 5375 7070  q..--quietz Supp
-00000c60: 7265 7373 2063 6f6d 6d69 7420 7375 6d6d  ress commit summ
-00000c70: 6172 7920 6d65 7373 6167 652e 7a09 2d2d  ary message.z.--
-00000c80: 6472 792d 7275 6e7a 9f44 6f20 6e6f 7420  dry-runz.Do not 
-00000c90: 6372 6561 7465 2061 2063 6f6d 6d69 742c  create a commit,
-00000ca0: 2062 7574 2073 686f 7720 6120 6c69 7374   but show a list
-00000cb0: 206f 6620 7061 7468 7320 7468 6174 2061   of paths that a
-00000cc0: 7265 2074 6f20 6265 2063 6f6d 6d69 7474  re to be committ
-00000cd0: 6564 2c20 7061 7468 7320 7769 7468 206c  ed, paths with l
-00000ce0: 6f63 616c 2063 6861 6e67 6573 2074 6861  ocal changes tha
-00000cf0: 7420 7769 6c6c 2062 6520 6c65 6674 2075  t will be left u
-00000d00: 6e63 6f6d 6d69 7474 6564 2061 6e64 2070  ncommitted and p
-00000d10: 6174 6873 2074 6861 7420 6172 6520 756e  aths that are un
-00000d20: 7472 6163 6b65 642e 2903 da04 7072 6f67  tracked.)...prog
-00000d30: da0b 6465 7363 7269 7074 696f 6eda 0c61  ..description..a
-00000d40: 6464 5f61 7267 756d 656e 74a9 01da 0670  dd_argument....p
-00000d50: 6172 7365 72a9 0072 1800 0000 fa21 2f64  arser..r.....!/d
-00000d60: 726f 6e65 2f73 7263 2f73 7263 2f74 7569  rone/src/src/tui
-00000d70: 7669 6577 2f63 6d64 2f67 6974 2e70 79da  view/cmd/git.py.
-00000d80: 0a67 6974 5f63 6f6d 6d69 7409 0000 0073  .git_commit....s
-00000d90: aa00 0000 0601 0601 0403 0201 0201 0201  ................
-00000da0: 0201 0201 06fb 0407 0201 0201 0201 0201  ................
-00000db0: 0201 06fb 0407 0201 0201 06fe 0404 0201  ................
-00000dc0: 0201 06fe 0404 0201 0201 0201 0201 0201  ................
-00000dd0: 06fb 0407 0201 0201 0201 06fd 0405 0201  ................
-00000de0: 0201 0201 06fd 0405 0201 0201 0201 0201  ................
-00000df0: 06fc 0406 0201 0201 0201 0201 0201 06fb  ................
-00000e00: 0407 0201 0201 0201 0201 06fc 0406 0201  ................
-00000e10: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
-00000e20: 0201 06fc 0406 0201 0201 0201 0201 0201  ................
-00000e30: 06fb 0407 0201 0201 0201 0201 0afc 721a  ..............r.
-00000e40: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000e50: 0100 0000 0600 0000 4300 0000 73d2 0000  ........C...s...
-00000e60: 0064 017c 005f 0064 027c 005f 017c 006a  .d.|._.d.|._.|.j
-00000e70: 0264 0364 0464 0564 068d 0301 007c 006a  .d.d.d.d.....|.j
-00000e80: 0264 0764 0864 0964 0a64 0b8d 0401 007c  .d.d.d.d.d.....|
-00000e90: 006a 0264 0c64 0964 0d64 0b8d 0301 007c  .j.d.d.d.d.....|
-00000ea0: 006a 0264 0e64 0964 0f64 0b8d 0301 007c  .j.d.d.d.d.....|
-00000eb0: 006a 0264 1064 1164 0964 1264 138d 0401  .j.d.d.d.d.d....
-00000ec0: 007c 006a 0264 1464 1564 0964 1664 138d  .|.j.d.d.d.d.d..
-00000ed0: 0401 007c 006a 0264 1764 1864 0964 1964  ...|.j.d.d.d.d.d
-00000ee0: 138d 0401 007c 006a 0264 1a64 1b64 0964  .....|.j.d.d.d.d
-00000ef0: 1c64 0b8d 0401 007c 006a 0264 1d64 1e64  .d.....|.j.d.d.d
-00000f00: 0964 1f64 0b8d 0401 007c 006a 0264 2074  .d.d.....|.j.d t
-00000f10: 036a 046a 0564 2164 2264 238d 0401 007c  .j.j.d!d"d#....|
-00000f20: 006a 0264 2464 0964 2564 0b8d 0301 0064  .j.d$d.d%d.....d
-00000f30: 0053 0029 264e 7a09 6769 742d 6d65 7267  .S.)&Nz.git-merg
-00000f40: 657a 2f4a 6f69 6e20 7477 6f20 6f72 206d  ez/Join two or m
-00000f50: 6f72 6520 6465 7665 6c6f 706d 656e 7420  ore development 
-00000f60: 6869 7374 6f72 6965 7320 746f 6765 7468  histories togeth
-00000f70: 6572 da06 636f 6d6d 6974 da01 2a7a 2043  er..commit..*z C
-00000f80: 6f6d 6d69 7473 2074 6f20 6d65 7267 6520  ommits to merge 
-00000f90: 696e 746f 206f 7572 2062 7261 6e63 68a9  into our branch.
-00000fa0: 02da 056e 6172 6773 7208 0000 0072 0c00  ...nargsr....r..
-00000fb0: 0000 7a0b 2d2d 6e6f 2d63 6f6d 6d69 7472  ..z.--no-commitr
-00000fc0: 0900 0000 7a2f 5065 7266 6f72 6d20 7468  ....z/Perform th
-00000fd0: 6520 6d65 7267 6520 7769 7468 6f75 7420  e merge without 
-00000fe0: 636f 6d6d 6974 7469 6e67 2074 6865 2072  committing the r
-00000ff0: 6573 756c 74a9 0272 0700 0000 7208 0000  esult..r....r...
-00001000: 0072 0b00 0000 7a67 5072 6f64 7563 6520  .r....zgProduce 
-00001010: 7468 6520 776f 726b 696e 6720 7472 6565  the working tree
-00001020: 2061 6e64 2069 6e64 6578 2073 7461 7465   and index state
-00001030: 2061 7320 6966 2061 2072 6561 6c20 6d65   as if a real me
-00001040: 7267 6520 6861 7070 656e 6564 2c20 6275  rge happened, bu
-00001050: 7420 646f 206e 6f74 2061 6374 7561 6c6c  t do not actuall
-00001060: 7920 6d61 6b65 2061 2063 6f6d 6d69 747a  y make a commitz
-00001070: 062d 2d73 7461 747a 2753 686f 7720 6120  .--statz'Show a 
-00001080: 6469 6666 7374 6174 2061 7420 7468 6520  diffstat at the 
-00001090: 656e 6420 6f66 2074 6865 206d 6572 6765  end of the merge
-000010a0: 7210 0000 00da 0465 6469 747a 3e49 6e76  r......editz>Inv
-000010b0: 6f6b 6520 616e 2065 6469 746f 7220 6265  oke an editor be
-000010c0: 666f 7265 2063 6f6d 6d69 7474 696e 6720  fore committing 
-000010d0: 7375 6363 6573 7366 756c 206d 6563 6861  successful mecha
-000010e0: 6e69 6361 6c20 6d65 7267 65a9 03da 0464  nical merge....d
-000010f0: 6573 7472 0700 0000 7208 0000 0072 0d00  estr....r....r..
-00001100: 0000 da06 7665 7269 6679 7a23 536b 6970  ....verifyz#Skip
-00001110: 2070 7265 2d6d 6572 6765 2061 6e64 2063   pre-merge and c
-00001120: 6f6d 6d69 742d 6d73 6720 686f 6f6b 737a  ommit-msg hooksz
-00001130: 132d 2d76 6572 6966 792d 7369 676e 6174  .--verify-signat
-00001140: 7572 6573 5a11 7665 7269 6679 5f73 6967  uresZ.verify_sig
-00001150: 6e61 7475 7265 737a 5556 6572 6966 7920  natureszUVerify 
-00001160: 7468 6174 2074 6865 2074 6970 2063 6f6d  that the tip com
-00001170: 6d69 7420 6f66 2074 6865 2073 6964 6520  mit of the side 
-00001180: 6272 616e 6368 2062 6569 6e67 206d 6572  branch being mer
-00001190: 6765 6420 6973 2073 6967 6e65 6420 7769  ged is signed wi
-000011a0: 7468 2061 2076 616c 6964 206b 6579 7212  th a valid keyr.
-000011b0: 0000 0072 1100 0000 7a0f 4f70 6572 6174  ...r....z.Operat
-000011c0: 6520 7175 6965 746c 797a 092d 2d76 6572  e quietlyz.--ver
-000011d0: 626f 7365 7a02 2d76 7a0a 4265 2076 6572  bosez.-vz.Be ver
-000011e0: 626f 7365 7a0a 2d2d 7072 6f67 7265 7373  bosez.--progress
-000011f0: 7a10 5475 726e 2070 726f 6772 6573 7320  z.Turn progress 
-00001200: 6f6e 4629 0372 0700 0000 7208 0000 0072  onF).r....r....r
-00001210: 0a00 0000 7a0b 2d2d 6175 746f 7374 6173  ....z.--autostas
-00001220: 687a 4841 7574 6f6d 6174 6963 616c 6c79  hzHAutomatically
-00001230: 2063 7265 6174 6520 6120 7465 6d70 6f72   create a tempor
-00001240: 6172 7920 7374 6173 6820 656e 7472 7920  ary stash entry 
-00001250: 6265 666f 7265 2074 6865 206f 7065 7261  before the opera
-00001260: 7469 6f6e 2062 6567 696e 7329 0672 1300  tion begins).r..
-00001270: 0000 7214 0000 0072 1500 0000 da04 7961  ..r....r......ya
-00001280: 7078 da07 6163 7469 6f6e 73da 1542 6f6f  px..actions..Boo
-00001290: 6c65 616e 4f70 7469 6f6e 616c 4163 7469  leanOptionalActi
-000012a0: 6f6e 7216 0000 0072 1800 0000 7218 0000  onr....r....r...
-000012b0: 0072 1900 0000 da09 6769 745f 6d65 7267  .r......git_merg
-000012c0: 6563 0000 0073 6400 0000 0601 0601 1002  ec...sd.........
-000012d0: 0402 0201 0201 0201 0201 06fc 0406 0201  ................
-000012e0: 0201 0201 06fd 0405 0201 0201 0201 06fd  ................
-000012f0: 0405 0201 0201 0201 0201 06fc 0406 0201  ................
-00001300: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
-00001310: 0201 06fc 1206 1201 0401 0201 0601 0201  ................
-00001320: 0201 06fc 0406 0201 0201 0201 0afd 7227  ..............r'
-00001330: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00001340: 0100 0000 0700 0000 4300 0000 7394 0200  ........C...s...
-00001350: 0064 017c 005f 0064 027c 005f 017c 006a  .d.|._.d.|._.|.j
-00001360: 0264 0364 0464 0564 068d 0301 007c 006a  .d.d.d.d.....|.j
-00001370: 0264 0764 0464 0864 068d 0301 007c 006a  .d.d.d.d.....|.j
-00001380: 0264 0964 0a67 0064 0ba2 0164 0c64 0d64  .d.d.g.d...d.d.d
-00001390: 0e8d 0501 007c 006a 0264 0f64 1064 0464  .....|.j.d.d.d.d
-000013a0: 0d64 118d 0401 007c 006a 0264 1264 1364  .d.....|.j.d.d.d
-000013b0: 1464 158d 0301 007c 006a 0264 1664 1764  .d.....|.j.d.d.d
-000013c0: 1464 158d 0301 007c 006a 0264 1864 0464  .d.....|.j.d.d.d
-000013d0: 1964 068d 0301 007c 006a 0264 1a64 0464  .d.....|.j.d.d.d
-000013e0: 1b64 068d 0301 007c 006a 0264 1c74 0364  .d.....|.j.d.t.d
-000013f0: 1d64 1e64 1f8d 0401 007c 006a 0264 2074  .d.d.....|.j.d t
-00001400: 0364 2164 228d 0301 007c 006a 0264 2364  .d!d"....|.j.d#d
-00001410: 2464 2564 2664 158d 0401 007c 006a 0264  $d%d&d.....|.j.d
-00001420: 2764 2864 2964 2a64 158d 0401 007c 006a  'd(d)d*d.....|.j
-00001430: 0264 2b64 2c64 2d64 2e8d 0301 007c 006a  .d+d,d-d.....|.j
-00001440: 0264 2f64 2c64 3064 2e8d 0301 007c 006a  .d/d,d0d.....|.j
-00001450: 0264 3164 2c64 3264 2e8d 0301 007c 006a  .d1d,d2d.....|.j
-00001460: 0264 3364 2c64 3464 2e8d 0301 007c 006a  .d3d,d4d.....|.j
-00001470: 0264 3564 0464 3664 068d 0301 007c 006a  .d5d.d6d.....|.j
-00001480: 0264 3764 0464 3864 068d 0301 007c 006a  .d7d.d8d.....|.j
-00001490: 0264 3964 3a64 0464 3b64 068d 0401 007c  .d9d:d.d;d.....|
-000014a0: 006a 0264 3c64 0464 3d64 068d 0301 007c  .j.d<d.d=d.....|
-000014b0: 006a 0264 3e64 3f64 0464 4064 068d 0401  .j.d>d?d.d@d....
-000014c0: 007c 006a 0264 4164 4264 0464 4364 068d  .|.j.dAdBd.dCd..
-000014d0: 0401 007c 006a 0264 4464 4564 0464 4664  ...|.j.dDdEd.dFd
-000014e0: 068d 0401 007c 006a 0264 4764 0464 4864  .....|.j.dGd.dHd
-000014f0: 068d 0301 007c 006a 0264 4964 0464 4a64  .....|.j.dId.dJd
-00001500: 068d 0301 007c 006a 0264 4b64 2c64 4c64  .....|.j.dKd,dLd
-00001510: 2e8d 0301 007c 006a 0264 4d64 0464 4e64  .....|.j.dMd.dNd
-00001520: 068d 0301 007c 006a 0264 4f64 0464 5064  .....|.j.dOd.dPd
-00001530: 068d 0301 007c 006a 0264 5164 0464 5264  .....|.j.dQd.dRd
-00001540: 068d 0301 007c 006a 0264 5364 0464 5464  .....|.j.dSd.dTd
-00001550: 068d 0301 007c 006a 0264 5564 0a64 5664  .....|.j.dUd.dVd
-00001560: 5764 588d 0401 007c 006a 0264 5964 0464  WdX....|.j.dYd.d
-00001570: 5a64 068d 0301 007c 006a 0264 5b64 0464  Zd.....|.j.d[d.d
-00001580: 5c8d 0201 007c 006a 0264 5d64 0464 5e64  \....|.j.d]d.d^d
-00001590: 068d 0301 007c 006a 0264 5f64 0464 6064  .....|.j.d_d.d`d
-000015a0: 068d 0301 007c 006a 0264 6164 6264 638d  .....|.j.dadbdc.
-000015b0: 0201 007c 006a 0264 6464 0464 6564 068d  ...|.j.ddd.ded..
-000015c0: 0301 007c 006a 0264 6664 0a64 678d 0201  ...|.j.dfd.dg...
-000015d0: 007c 006a 0264 6874 046a 0564 678d 0201  .|.j.dht.j.dg...
-000015e0: 0064 0053 0029 694e 7a07 6769 742d 6c6f  .d.S.)iNz.git-lo
-000015f0: 677a 1053 686f 7720 636f 6d6d 6974 206c  gz.Show commit l
-00001600: 6f67 737a 072d 2d67 7261 7068 7209 0000  ogsz.--graphr...
-00001610: 007a 6444 7261 7720 6120 7465 7874 2d62  .zdDraw a text-b
-00001620: 6173 6564 2067 7261 7068 6963 616c 2072  ased graphical r
-00001630: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-00001640: 2074 6865 2063 6f6d 6d69 7420 6869 7374   the commit hist
-00001650: 6f72 7920 6f6e 2074 6865 206c 6566 7420  ory on the left 
-00001660: 6861 6e64 2073 6964 6520 6f66 2074 6865  hand side of the
-00001670: 206f 7574 7075 7472 1f00 0000 7a08 2d2d   outputr....z.--
-00001680: 666f 6c6c 6f77 7a54 436f 6e74 696e 7565  followzTContinue
-00001690: 206c 6973 7469 6e67 2074 6865 2068 6973   listing the his
-000016a0: 746f 7279 206f 6620 6120 6669 6c65 2062  tory of a file b
-000016b0: 6579 6f6e 6420 7265 6e61 6d65 7320 2877  eyond renames (w
-000016c0: 6f72 6b73 206f 6e6c 7920 666f 7220 6120  orks only for a 
-000016d0: 7369 6e67 6c65 2066 696c 6529 7a0a 2d2d  single file)z.--
-000016e0: 6465 636f 7261 7465 fa01 3f29 04da 0573  decorate..?)...s
-000016f0: 686f 7274 da04 6675 6c6c da04 6175 746f  hort..full..auto
-00001700: da02 6e6f 7229 0000 007a 3550 7269 6e74  ..nor)...z5Print
-00001710: 206f 7574 2074 6865 2072 6566 206e 616d   out the ref nam
-00001720: 6573 206f 6620 616e 7920 636f 6d6d 6974  es of any commit
-00001730: 7320 7468 6174 2061 7265 2073 686f 776e  s that are shown
-00001740: 2904 721e 0000 00da 0763 686f 6963 6573  ).r......choices
-00001750: da05 636f 6e73 7472 0800 0000 7a0d 2d2d  ..constr....z.--
-00001760: 6e6f 2d64 6563 6f72 6174 65da 0864 6563  no-decorate..dec
-00001770: 6f72 6174 6572 2100 0000 7a0f 2d2d 6465  orater!...z.--de
-00001780: 636f 7261 7465 2d72 6566 735a 0d64 6563  corate-refsZ.dec
-00001790: 6f72 6174 655f 7265 6673 7a44 4966 206e  orate_refszDIf n
-000017a0: 6f20 2d2d 6465 636f 7261 7465 2d72 6566  o --decorate-ref
-000017b0: 7320 6973 2067 6976 656e 2c20 7072 6574  s is given, pret
-000017c0: 656e 6420 6173 2069 6620 616c 6c20 7265  end as if all re
-000017d0: 6673 2077 6572 6520 696e 636c 7564 6564  fs were included
-000017e0: 2902 7222 0000 0072 0800 0000 7a17 2d2d  ).r"...r....z.--
-000017f0: 6465 636f 7261 7465 2d72 6566 732d 6578  decorate-refs-ex
-00001800: 636c 7564 655a 1564 6563 6f72 6174 655f  cludeZ.decorate_
-00001810: 7265 6673 5f65 7863 6c75 6465 7a08 2d2d  refs_excludez.--
-00001820: 736f 7572 6365 7a51 5072 696e 7420 6f75  sourcezQPrint ou
-00001830: 7420 7468 6520 7265 6620 6e61 6d65 2067  t the ref name g
-00001840: 6976 656e 206f 6e20 7468 6520 636f 6d6d  iven on the comm
-00001850: 616e 6420 6c69 6e65 2062 7920 7768 6963  and line by whic
-00001860: 6820 6561 6368 2063 6f6d 6d69 7420 7761  h each commit wa
-00001870: 7320 7265 6163 6865 647a 0b2d 2d66 756c  s reachedz.--ful
-00001880: 6c2d 6469 6666 7529 0100 0057 6974 686f  l-diffu)...Witho
-00001890: 7574 2074 6869 7320 666c 6167 2c20 6769  ut this flag, gi
-000018a0: 7420 6c6f 6720 2d70 203c 7061 7468 3e2e  t log -p <path>.
-000018b0: 2e2e 2073 686f 7773 2063 6f6d 6d69 7473  .. shows commits
-000018c0: 2074 6861 7420 746f 7563 6820 7468 6520   that touch the 
-000018d0: 7370 6563 6966 6965 6420 7061 7468 732c  specified paths,
-000018e0: 2061 6e64 2064 6966 6673 2061 626f 7574   and diffs about
-000018f0: 2074 6865 2073 616d 6520 7370 6563 6966   the same specif
-00001900: 6965 6420 7061 7468 732e 2057 6974 6820  ied paths. With 
-00001910: 7468 6973 2c20 7468 6520 6675 6c6c 2064  this, the full d
-00001920: 6966 6620 6973 2073 686f 776e 2066 6f72  iff is shown for
-00001930: 2063 6f6d 6d69 7473 2074 6861 7420 746f   commits that to
-00001940: 7563 6820 7468 6520 7370 6563 6966 6965  uch the specifie
-00001950: 6420 7061 7468 733b 2074 6869 7320 6d65  d paths; this me
-00001960: 616e 7320 7468 6174 2022 3c70 6174 683e  ans that "<path>
-00001970: 2e2e 2e22 206c 696d 6974 7320 6f6e 6c79  ..." limits only
-00001980: 2063 6f6d 6d69 7473 2c20 616e 6420 646f   commits, and do
-00001990: 6573 6ee2 8099 7420 6c69 6d69 7420 6469  esn...t limit di
-000019a0: 6666 2066 6f72 2074 686f 7365 2063 6f6d  ff for those com
-000019b0: 6d69 7473 720c 0000 00da 096d 6178 5f63  mitsr......max_c
-000019c0: 6f75 6e74 7a25 4c69 6d69 7420 7468 6520  ountz%Limit the 
-000019d0: 6e75 6d62 6572 206f 6620 636f 6d6d 6974  number of commit
-000019e0: 7320 746f 206f 7574 7075 7429 03da 0474  s to output)...t
-000019f0: 7970 6572 2200 0000 7208 0000 007a 062d  yper"...r....z.-
-00001a00: 2d73 6b69 707a 3d53 6b69 7020 6e75 6d62  -skipz=Skip numb
-00001a10: 6572 2063 6f6d 6d69 7473 2062 6566 6f72  er commits befor
-00001a20: 6520 7374 6172 7469 6e67 2074 6f20 7368  e starting to sh
-00001a30: 6f77 2074 6865 2063 6f6d 6d69 7420 6f75  ow the commit ou
-00001a40: 7470 7574 2902 7231 0000 0072 0800 0000  tput).r1...r....
-00001a50: 7a07 2d2d 7369 6e63 657a 072d 2d61 6674  z.--sincez.--aft
-00001a60: 6572 5a0a 7369 6e63 655f 6461 7465 7a2d  erZ.since_datez-
-00001a70: 5368 6f77 2063 6f6d 6d69 7473 206d 6f72  Show commits mor
-00001a80: 6520 7265 6365 6e74 2074 6861 6e20 6120  e recent than a 
-00001a90: 7370 6563 6966 6963 2064 6174 657a 072d  specific datez.-
-00001aa0: 2d75 6e74 696c 7a08 2d2d 6265 666f 7265  -untilz.--before
-00001ab0: 5a0a 756e 7469 6c5f 6461 7465 7a27 5368  Z.until_datez'Sh
-00001ac0: 6f77 2063 6f6d 6d69 7473 206f 6c64 6572  ow commits older
-00001ad0: 2074 6861 6e20 6120 7370 6563 6966 6963   than a specific
-00001ae0: 2064 6174 6572 0e00 0000 fa01 2b7a 6f4c   dater......+zoL
-00001af0: 696d 6974 2074 6865 2063 6f6d 6d69 7473  imit the commits
-00001b00: 206f 7574 7075 7420 746f 206f 6e65 7320   output to ones 
-00001b10: 7769 7468 2061 7574 686f 7220 6865 6164  with author head
-00001b20: 6572 206c 696e 6573 2074 6861 7420 6d61  er lines that ma
-00001b30: 7463 6820 7468 6520 7370 6563 6966 6965  tch the specifie
-00001b40: 6420 7061 7474 6572 6e20 2872 6567 756c  d pattern (regul
-00001b50: 6172 2065 7870 7265 7373 696f 6e29 721d  ar expression)r.
-00001b60: 0000 007a 0b2d 2d63 6f6d 6d69 7474 6572  ...z.--committer
-00001b70: 7a72 4c69 6d69 7420 7468 6520 636f 6d6d  zrLimit the comm
-00001b80: 6974 7320 6f75 7470 7574 2074 6f20 6f6e  its output to on
-00001b90: 6573 2077 6974 6820 636f 6d6d 6974 7465  es with committe
-00001ba0: 7220 6865 6164 6572 206c 696e 6573 2074  r header lines t
-00001bb0: 6861 7420 6d61 7463 6820 7468 6520 7370  hat match the sp
-00001bc0: 6563 6966 6965 6420 7061 7474 6572 6e20  ecified pattern 
-00001bd0: 2872 6567 756c 6172 2065 7870 7265 7373  (regular express
-00001be0: 696f 6e29 7a0d 2d2d 6772 6570 2d72 6566  ion)z.--grep-ref
-00001bf0: 6c6f 677a ad4c 696d 6974 2074 6865 2063  logz.Limit the c
-00001c00: 6f6d 6d69 7473 206f 7574 7075 7420 746f  ommits output to
-00001c10: 206f 6e65 7320 7769 7468 2072 6566 6c6f   ones with reflo
-00001c20: 6720 656e 7472 6965 7320 7468 6174 206d  g entries that m
-00001c30: 6174 6368 2074 6865 2073 7065 6369 6669  atch the specifi
-00001c40: 6564 2070 6174 7465 726e 2028 7265 6775  ed pattern (regu
-00001c50: 6c61 7220 6578 7072 6573 7369 6f6e 292e  lar expression).
-00001c60: 2049 7420 6973 2061 6e20 6572 726f 7220   It is an error 
-00001c70: 746f 2075 7365 2074 6869 7320 6f70 7469  to use this opti
-00001c80: 6f6e 2075 6e6c 6573 7320 2d2d 7761 6c6b  on unless --walk
-00001c90: 2d72 6566 6c6f 6773 2069 7320 696e 2075  -reflogs is in u
-00001ca0: 7365 7a06 2d2d 6772 6570 7ad1 4c69 6d69  sez.--grepz.Limi
-00001cb0: 7420 7468 6520 636f 6d6d 6974 7320 6f75  t the commits ou
-00001cc0: 7470 7574 2074 6f20 6f6e 6573 2077 6974  tput to ones wit
-00001cd0: 6820 6c6f 6720 6d65 7373 6167 6520 7468  h log message th
-00001ce0: 6174 206d 6174 6368 6573 2074 6865 2073  at matches the s
-00001cf0: 7065 6369 6669 6564 2070 6174 7465 726e  pecified pattern
-00001d00: 2028 7265 6775 6c61 7220 6578 7072 6573   (regular expres
-00001d10: 7369 6f6e 292e 2057 6865 6e20 2d2d 6e6f  sion). When --no
-00001d20: 7465 7320 6973 2069 6e20 6566 6665 6374  tes is in effect
-00001d30: 2c20 7468 6520 6d65 7373 6167 6520 6672  , the message fr
-00001d40: 6f6d 2074 6865 206e 6f74 6573 2069 7320  om the notes is 
-00001d50: 6d61 7463 6865 6420 6173 2069 6620 6974  matched as if it
-00001d60: 2077 6572 6520 7061 7274 206f 6620 7468   were part of th
-00001d70: 6520 6c6f 6720 6d65 7373 6167 657a 0b2d  e log messagez.-
-00001d80: 2d61 6c6c 2d6d 6174 6368 7a65 4c69 6d69  -all-matchzeLimi
-00001d90: 7420 7468 6520 636f 6d6d 6974 7320 6f75  t the commits ou
-00001da0: 7470 7574 2074 6f20 6f6e 6573 2074 6861  tput to ones tha
-00001db0: 7420 6d61 7463 6820 616c 6c20 6769 7665  t match all give
-00001dc0: 6e20 2d2d 6772 6570 2c20 696e 7374 6561  n --grep, instea
-00001dd0: 6420 6f66 206f 6e65 7320 7468 6174 206d  d of ones that m
-00001de0: 6174 6368 2061 7420 6c65 6173 7420 6f6e  atch at least on
-00001df0: 657a 0d2d 2d69 6e76 6572 742d 6772 6570  ez.--invert-grep
-00001e00: 7a65 4c69 6d69 7420 7468 6520 636f 6d6d  zeLimit the comm
-00001e10: 6974 7320 6f75 7470 7574 2074 6f20 6f6e  its output to on
-00001e20: 6573 2077 6974 6820 6c6f 6720 6d65 7373  es with log mess
-00001e30: 6167 6520 7468 6174 2064 6f20 6e6f 7420  age that do not 
-00001e40: 6d61 7463 6820 7468 6520 7061 7474 6572  match the patter
-00001e50: 6e20 7370 6563 6966 6965 6420 7769 7468  n specified with
-00001e60: 202d 2d67 7265 707a 022d 697a 142d 2d72   --grepz.-iz.--r
-00001e70: 6567 6578 702d 6967 6e6f 7265 2d63 6173  egexp-ignore-cas
-00001e80: 657a 4c4d 6174 6368 2074 6865 2072 6567  ezLMatch the reg
-00001e90: 756c 6172 2065 7870 7265 7373 696f 6e20  ular expression 
-00001ea0: 6c69 6d69 7469 6e67 2070 6174 7465 726e  limiting pattern
-00001eb0: 7320 7769 7468 6f75 7420 7265 6761 7264  s without regard
-00001ec0: 2074 6f20 6c65 7474 6572 2063 6173 657a   to letter casez
-00001ed0: 0e2d 2d62 6173 6963 2d72 6567 6578 707a  .--basic-regexpz
-00001ee0: 5343 6f6e 7369 6465 7220 7468 6520 6c69  SConsider the li
-00001ef0: 6d69 7469 6e67 2070 6174 7465 726e 7320  miting patterns 
-00001f00: 746f 2062 6520 6261 7369 6320 7265 6775  to be basic regu
-00001f10: 6c61 7220 6578 7072 6573 7369 6f6e 733b  lar expressions;
-00001f20: 2074 6869 7320 6973 2074 6865 2064 6566   this is the def
-00001f30: 6175 6c74 7a02 2d45 7a11 2d2d 6578 7465  aultz.-Ez.--exte
-00001f40: 6e64 6564 2d72 6567 6578 707a 7243 6f6e  nded-regexpzrCon
-00001f50: 7369 6465 7220 7468 6520 6c69 6d69 7469  sider the limiti
-00001f60: 6e67 2070 6174 7465 726e 7320 746f 2062  ng patterns to b
-00001f70: 6520 6578 7465 6e64 6564 2072 6567 756c  e extended regul
-00001f80: 6172 2065 7870 7265 7373 696f 6e73 2069  ar expressions i
-00001f90: 6e73 7465 6164 206f 6620 7468 6520 6465  nstead of the de
-00001fa0: 6661 756c 7420 6261 7369 6320 7265 6775  fault basic regu
-00001fb0: 6c61 7220 6578 7072 6573 7369 6f6e 737a  lar expressionsz
-00001fc0: 022d 467a 0f2d 2d66 6978 6564 2d73 7472  .-Fz.--fixed-str
-00001fd0: 696e 6773 7566 0000 0043 6f6e 7369 6465  ingsuf...Conside
-00001fe0: 7220 7468 6520 6c69 6d69 7469 6e67 2070  r the limiting p
-00001ff0: 6174 7465 726e 7320 746f 2062 6520 6669  atterns to be fi
-00002000: 7865 6420 7374 7269 6e67 7320 2864 6f6e  xed strings (don
-00002010: e280 9974 2069 6e74 6572 7072 6574 2070  ...t interpret p
-00002020: 6174 7465 726e 2061 7320 6120 7265 6775  attern as a regu
-00002030: 6c61 7220 6578 7072 6573 7369 6f6e 297a  lar expression)z
-00002040: 022d 507a 0d2d 2d70 6572 6c2d 7265 6765  .-Pz.--perl-rege
-00002050: 7870 7a48 436f 6e73 6964 6572 2074 6865  xpzHConsider the
-00002060: 206c 696d 6974 696e 6720 7061 7474 6572   limiting patter
-00002070: 6e73 2074 6f20 6265 2050 6572 6c2d 636f  ns to be Perl-co
-00002080: 6d70 6174 6962 6c65 2072 6567 756c 6172  mpatible regular
-00002090: 2065 7870 7265 7373 696f 6e73 7a08 2d2d   expressionsz.--
-000020a0: 6d65 7267 6573 7a45 5072 696e 7420 6f6e  mergeszEPrint on
-000020b0: 6c79 206d 6572 6765 2063 6f6d 6d69 7473  ly merge commits
-000020c0: 2e20 5468 6973 2069 7320 6578 6163 746c  . This is exactl
-000020d0: 7920 7468 6520 7361 6d65 2061 7320 2d2d  y the same as --
-000020e0: 6d69 6e2d 7061 7265 6e74 733d 327a 0b2d  min-parents=2z.-
-000020f0: 2d6e 6f2d 6d65 7267 6573 7a5b 446f 206e  -no-mergesz[Do n
-00002100: 6f74 2070 7269 6e74 2063 6f6d 6d69 7473  ot print commits
-00002110: 2077 6974 6820 6d6f 7265 2074 6861 6e20   with more than 
-00002120: 6f6e 6520 7061 7265 6e74 2e20 5468 6973  one parent. This
-00002130: 2069 7320 6578 6163 746c 7920 7468 6520   is exactly the 
-00002140: 7361 6d65 2061 7320 2d2d 6d61 782d 7061  same as --max-pa
-00002150: 7265 6e74 733d 317a 092d 2d65 7863 6c75  rents=1z.--exclu
-00002160: 6465 6102 0100 0044 6f20 6e6f 7420 696e  dea....Do not in
-00002170: 636c 7564 6520 7265 6673 206d 6174 6368  clude refs match
-00002180: 696e 6720 3c67 6c6f 622d 7061 7474 6572  ing <glob-patter
-00002190: 6e3e 2074 6861 7420 7468 6520 6e65 7874  n> that the next
-000021a0: 202d 2d61 6c6c 2c20 2d2d 6272 616e 6368   --all, --branch
-000021b0: 6573 2c20 2d2d 7461 6773 2c20 2d2d 7265  es, --tags, --re
-000021c0: 6d6f 7465 732c 206f 7220 2d2d 676c 6f62  motes, or --glob
-000021d0: 2077 6f75 6c64 206f 7468 6572 7769 7365   would otherwise
-000021e0: 2063 6f6e 7369 6465 722e 2052 6570 6574   consider. Repet
-000021f0: 6974 696f 6e73 206f 6620 7468 6973 206f  itions of this o
-00002200: 7074 696f 6e20 6163 6375 6d75 6c61 7465  ption accumulate
-00002210: 2065 7863 6c75 7369 6f6e 2070 6174 7465   exclusion patte
-00002220: 726e 7320 7570 2074 6f20 7468 6520 6e65  rns up to the ne
-00002230: 7874 202d 2d61 6c6c 2c20 2d2d 6272 616e  xt --all, --bran
-00002240: 6368 6573 2c20 2d2d 7461 6773 2c20 2d2d  ches, --tags, --
-00002250: 7265 6d6f 7465 732c 206f 7220 2d2d 676c  remotes, or --gl
-00002260: 6f62 206f 7074 696f 6e7a 0c2d 2d64 6174  ob optionz.--dat
-00002270: 652d 6f72 6465 727a 6e53 686f 7720 6e6f  e-orderznShow no
-00002280: 2070 6172 656e 7473 2062 6566 6f72 6520   parents before 
-00002290: 616c 6c20 6f66 2069 7473 2063 6869 6c64  all of its child
-000022a0: 7265 6e20 6172 6520 7368 6f77 6e2c 2062  ren are shown, b
-000022b0: 7574 206f 7468 6572 7769 7365 2073 686f  ut otherwise sho
-000022c0: 7720 636f 6d6d 6974 7320 696e 2074 6865  w commits in the
-000022d0: 2063 6f6d 6d69 7420 7469 6d65 7374 616d   commit timestam
-000022e0: 7020 6f72 6465 727a 132d 2d61 7574 686f  p orderz.--autho
-000022f0: 722d 6461 7465 2d6f 7264 6572 7a6e 5368  r-date-orderznSh
-00002300: 6f77 206e 6f20 7061 7265 6e74 7320 6265  ow no parents be
-00002310: 666f 7265 2061 6c6c 206f 6620 6974 7320  fore all of its 
-00002320: 6368 696c 6472 656e 2061 7265 2073 686f  children are sho
-00002330: 776e 2c20 6275 7420 6f74 6865 7277 6973  wn, but otherwis
-00002340: 6520 7368 6f77 2063 6f6d 6d69 7473 2069  e show commits i
-00002350: 6e20 7468 6520 6175 7468 6f72 2074 696d  n the author tim
-00002360: 6573 7461 6d70 206f 7264 6572 7a0c 2d2d  estamp orderz.--
-00002370: 746f 706f 2d6f 7264 6572 7a77 5368 6f77  topo-orderzwShow
-00002380: 206e 6f20 7061 7265 6e74 7320 6265 666f   no parents befo
-00002390: 7265 2061 6c6c 206f 6620 6974 7320 6368  re all of its ch
-000023a0: 696c 6472 656e 2061 7265 2073 686f 776e  ildren are shown
-000023b0: 2c20 616e 6420 6176 6f69 6420 7368 6f77  , and avoid show
-000023c0: 696e 6720 636f 6d6d 6974 7320 6f6e 206d  ing commits on m
-000023d0: 756c 7469 706c 6520 6c69 6e65 7320 6f66  ultiple lines of
-000023e0: 2068 6973 746f 7279 2069 6e74 6572 6d69   history intermi
-000023f0: 7865 647a 092d 2d72 6576 6572 7365 7a5e  xedz.--reversez^
-00002400: 4f75 7470 7574 2074 6865 2063 6f6d 6d69  Output the commi
-00002410: 7473 2063 686f 7365 6e20 746f 2062 6520  ts chosen to be 
-00002420: 7368 6f77 6e20 696e 2072 6576 6572 7365  shown in reverse
-00002430: 206f 7264 6572 2e20 4361 6e6e 6f74 2062   order. Cannot b
-00002440: 6520 636f 6d62 696e 6564 2077 6974 6820  e combined with 
-00002450: 2d2d 7761 6c6b 2d72 6566 6c6f 6773 7a08  --walk-reflogsz.
-00002460: 2d2d 7072 6574 7479 7a09 666f 726d 6174  --prettyz.format
-00002470: 3a25 487a 3e50 7265 7474 792d 7072 696e  :%Hz>Pretty-prin
-00002480: 7420 7468 6520 636f 6e74 656e 7473 206f  t the contents o
-00002490: 6620 7468 6520 636f 6d6d 6974 206c 6f67  f the commit log
-000024a0: 7320 696e 2061 2067 6976 656e 2066 6f72  s in a given for
-000024b0: 6d61 7429 0372 1e00 0000 722e 0000 0072  mat).r....r....r
-000024c0: 0800 0000 7a0f 2d2d 6162 6272 6576 2d63  ....z.--abbrev-c
-000024d0: 6f6d 6d69 747a 7049 6e73 7465 6164 206f  ommitzpInstead o
-000024e0: 6620 7368 6f77 696e 6720 7468 6520 6675  f showing the fu
-000024f0: 6c6c 2034 302d 6279 7465 2068 6578 6164  ll 40-byte hexad
-00002500: 6563 696d 616c 2063 6f6d 6d69 7420 6f62  ecimal commit ob
-00002510: 6a65 6374 206e 616d 652c 2073 686f 7720  ject name, show 
-00002520: 6120 7072 6566 6978 2074 6861 7420 6e61  a prefix that na
-00002530: 6d65 7320 7468 6520 6f62 6a65 6374 2075  mes the object u
-00002540: 6e69 7175 656c 797a 122d 2d6e 6f2d 6162  niquelyz.--no-ab
-00002550: 6272 6576 2d63 6f6d 6d69 7429 0172 0700  brev-commit).r..
-00002560: 0000 7a09 2d2d 6f6e 656c 696e 657a 3053  ..z.--onelinez0S
-00002570: 686f 7274 6861 6e64 2066 6f72 2022 2d2d  horthand for "--
-00002580: 7072 6574 7479 3d6f 6e65 6c69 6e65 202d  pretty=oneline -
-00002590: 2d61 6262 7265 762d 636f 6d6d 6974 227a  -abbrev-commit"z
-000025a0: 102d 2d73 686f 772d 7369 676e 6174 7572  .--show-signatur
-000025b0: 657a 6943 6865 636b 2074 6865 2076 616c  eziCheck the val
-000025c0: 6964 6974 7920 6f66 2061 2073 6967 6e65  idity of a signe
-000025d0: 6420 636f 6d6d 6974 206f 626a 6563 7420  d commit object 
-000025e0: 6279 2070 6173 7369 6e67 2074 6865 2073  by passing the s
-000025f0: 6967 6e61 7475 7265 2074 6f20 6770 6720  ignature to gpg 
-00002600: 2d2d 7665 7269 6679 2061 6e64 2073 686f  --verify and sho
-00002610: 7720 7468 6520 6f75 7470 7574 720f 0000  w the outputr...
-00002620: 007a 574f 6e6c 7920 7461 6b65 7320 6566  .zWOnly takes ef
-00002630: 6665 6374 2066 6f72 2064 6174 6573 2073  fect for dates s
-00002640: 686f 776e 2069 6e20 6875 6d61 6e2d 7265  hown in human-re
-00002650: 6164 6162 6c65 2066 6f72 6d61 742c 2073  adable format, s
-00002660: 7563 6820 6173 2077 6865 6e20 7573 696e  uch as when usin
-00002670: 6720 2d2d 7072 6574 7479 2901 7208 0000  g --pretty).r...
-00002680: 007a 0f2d 2d72 656c 6174 6976 652d 6461  .z.--relative-da
-00002690: 7465 7a1b 5379 6e6f 6e79 6d20 666f 7220  tez.Synonym for 
-000026a0: 2d2d 6461 7465 3d72 656c 6174 6976 655a  --date=relativeZ
-000026b0: 0e72 6576 6973 696f 6e5f 7261 6e67 6529  .revision_range)
-000026c0: 0172 1e00 0000 da04 7061 7468 2906 7213  .r......path).r.
-000026d0: 0000 0072 1400 0000 7215 0000 00da 0369  ...r....r......i
-000026e0: 6e74 da08 6172 6770 6172 7365 da09 5245  nt..argparse..RE
-000026f0: 4d41 494e 4445 5272 1600 0000 7218 0000  MAINDERr....r...
-00002700: 0072 1800 0000 7219 0000 00da 0767 6974  .r....r......git
-00002710: 5f6c 6f67 9a00 0000 7386 0100 0006 0106  _log....s.......
-00002720: 0104 0202 0102 0102 0106 fd04 0502 0102  ................
-00002730: 0102 0106 fd04 0502 0102 0106 0102 0102  ................
-00002740: 0106 fb04 0702 0102 0102 0102 0106 fc04  ................
-00002750: 0602 0102 0102 0106 fd04 0502 0102 0102  ................
-00002760: 0106 fd04 0502 0102 0102 0106 fd04 0502  ................
-00002770: 0102 0102 0106 fd04 0502 0102 0102 0102  ................
-00002780: 0106 fc04 0602 0102 0102 0106 fd04 0502  ................
-00002790: 0102 0102 0102 0106 fc04 0602 0102 0102  ................
-000027a0: 0102 0106 fc04 0602 0102 0102 0106 fd04  ................
-000027b0: 0502 0102 0102 0106 fd04 0502 0102 0102  ................
-000027c0: 0106 fd04 0502 0102 0102 0106 fd04 0502  ................
-000027d0: 0102 0102 0106 fd04 0502 0102 0102 0106  ................
-000027e0: fd04 0502 0102 0102 0102 0106 fc04 0602  ................
-000027f0: 0102 0102 0106 fd04 0502 0102 0102 0102  ................
-00002800: 0106 fc04 0602 0102 0102 0102 0106 fc04  ................
-00002810: 0602 0102 0102 0102 0106 fc04 0602 0102  ................
-00002820: 0102 0106 fd04 0502 0102 0102 0106 fd04  ................
-00002830: 0502 0102 0102 0106 fd04 0502 0102 0102  ................
-00002840: 0106 fd04 0502 0102 0102 0106 fd04 0502  ................
-00002850: 0102 0102 0106 fd04 0502 0102 0102 0106  ................
-00002860: fd04 0502 0102 0102 0102 0106 fc04 0602  ................
-00002870: 0102 0102 0106 fd0e 0504 0102 0102 0102  ................
-00002880: 0106 fd04 0502 0102 0102 0106 fd04 0502  ................
-00002890: 0102 0106 fe04 0402 0102 0102 0106 fd0e  ................
-000028a0: 0614 0172 3700 0000 da03 636d 6454 2901  ...r7.....cmdT).
-000028b0: da03 706f 7363 0100 0000 0000 0000 0000  ..posc..........
-000028c0: 0000 0300 0000 0400 0000 4300 0000 734e  ..........C...sN
-000028d0: 0000 0074 006a 0164 0164 028d 017d 017c  ...t.j.d.d...}.|
-000028e0: 01a0 02a1 007d 0274 037c 02a0 0464 03a1  .....}.t.|...d..
-000028f0: 0183 0101 0074 057c 02a0 0464 04a1 0183  .....t.|...d....
-00002900: 0101 0074 067c 02a0 0464 05a1 0183 0101  ...t.|...d......
-00002910: 0074 077c 017c 0064 068d 0201 0064 0053  .t.|.|.d.....d.S
-00002920: 0029 074e da03 6769 7429 0172 1300 0000  .).N..git).r....
-00002930: 721b 0000 00da 036c 6f67 da05 6d65 7267  r......log..merg
-00002940: 6529 01da 0e63 6f6d 6d61 6e64 5f66 696c  e)...command_fil
-00002950: 7465 7229 0872 2400 0000 da0e 4172 6775  ter).r$.....Argu
-00002960: 6d65 6e74 5061 7273 6572 da0e 6164 645f  mentParser..add_
-00002970: 7375 6270 6172 7365 7273 721a 0000 00da  subparsersr.....
-00002980: 0a61 6464 5f70 6172 7365 7272 3700 0000  .add_parserr7...
-00002990: 7227 0000 0072 0300 0000 2903 7238 0000  r'...r....).r8..
-000029a0: 0072 1700 0000 da0a 7375 6270 6172 7365  .r......subparse
-000029b0: 7273 7218 0000 0072 1800 0000 7219 0000  rsr....r....r...
-000029c0: 00da 046d 6169 6e62 0100 0073 0c00 0000  ...mainb...s....
-000029d0: 0c01 0802 0e02 0e01 0e01 1002 7242 0000  ............rB..
-000029e0: 0029 0e72 3500 0000 da06 7479 7069 6e67  .).r5.....typing
-000029f0: 7202 0000 0072 2400 0000 da0c 6172 6770  r....r$.....argp
-00002a00: 6172 7365 5f74 7569 7203 0000 00da 0a79  arse_tuir......y
-00002a10: 6170 782e 7479 7065 7372 0400 0000 721a  apx.typesr....r.
-00002a20: 0000 0072 2700 0000 7237 0000 00da 0373  ...r'...r7.....s
-00002a30: 7472 da03 6172 6772 4200 0000 7218 0000  tr..argrB...r...
-00002a40: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-00002a50: da08 3c6d 6f64 756c 653e 0100 0000 7314  ..<module>....s.
-00002a60: 0000 0008 000c 0108 020c 010c 0108 0308  ................
-00002a70: 5a08 3700 7f28 49                        Z.7..(I
+00000020: 0002 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
+00000040: 6402 6c02 6d03 5a03 0100 6403 6404 8400  d.l.m.Z...d.d...
+00000050: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
+00000060: 5a06 6409 640a 8400 5a07 6401 5300 290b  Z.d.d...Z.d.S.).
+00000070: e900 0000 004e 2901 da0a 696e 766f 6b65  .....N)...invoke
+00000080: 5f74 7569 6301 0000 0000 0000 0000 0000  _tuic...........
+00000090: 0001 0000 0007 0000 0043 0000 0073 0a01  .........C...s..
+000000a0: 0000 6401 7c00 5f00 6402 7c00 5f01 7c00  ..d.|._.d.|._.|.
+000000b0: 6a02 6403 6404 6405 6406 6407 6408 8d05  j.d.d.d.d.d.d...
+000000c0: 0100 7c00 6a02 6409 640a 640b 640c 640d  ..|.j.d.d.d.d.d.
+000000d0: 640e 8d05 0100 7c00 6a02 640f 6410 6411  d.....|.j.d.d.d.
+000000e0: 8d02 0100 7c00 6a02 6412 6413 6411 8d02  ....|.j.d.d.d...
+000000f0: 0100 7c00 6a02 6414 6415 640b 640c 6416  ..|.j.d.d.d.d.d.
+00000100: 640e 8d05 0100 7c00 6a02 6417 6418 6419  d.....|.j.d.d.d.
+00000110: 641a 8d03 0100 7c00 6a02 641b 641c 641d  d.....|.j.d.d.d.
+00000120: 641a 8d03 0100 7c00 6a02 641e 640b 640c  d.....|.j.d.d.d.
+00000130: 641f 640e 8d04 0100 7c00 6a02 6420 6421  d.d.....|.j.d d!
+00000140: 640b 640c 6422 640e 8d05 0100 7c00 6a02  d.d.d"d.....|.j.
+00000150: 6423 640b 640c 6424 640e 8d04 0100 7c00  d#d.d.d$d.....|.
+00000160: 6a02 6425 640b 640c 6426 640e 8d04 0100  j.d%d.d.d&d.....
+00000170: 7c00 6a02 6427 640b 640c 6428 640e 8d04  |.j.d'd.d.d(d...
+00000180: 0100 7c00 6a02 6429 642a 640b 640c 642b  ..|.j.d)d*d.d.d+
+00000190: 640e 8d05 0100 7c00 6a02 642c 640b 640c  d.....|.j.d,d.d.
+000001a0: 642d 640e 8d04 0100 6400 5300 292e 4e7a  d-d.....d.S.).Nz
+000001b0: 0a67 6974 2d63 6f6d 6d69 747a 2052 6563  .git-commitz Rec
+000001c0: 6f72 6420 6368 616e 6765 7320 746f 2074  ord changes to t
+000001d0: 6865 2072 6570 6f73 6974 6f72 797a 022d  he repositoryz.-
+000001e0: 6d7a 092d 2d6d 6573 7361 6765 7a05 3c6d  mz.--messagez.<m
+000001f0: 7367 3eda 0661 7070 656e 647a 8255 7365  sg>..appendz.Use
+00000200: 2074 6865 2067 6976 656e 203c 6d73 673e   the given <msg>
+00000210: 2061 7320 7468 6520 636f 6d6d 6974 206d   as the commit m
+00000220: 6573 7361 6765 2e20 4966 206d 756c 7469  essage. If multi
+00000230: 706c 6520 2d6d 206f 7074 696f 6e73 2061  ple -m options a
+00000240: 7265 2067 6976 656e 2c20 7468 6569 7220  re given, their 
+00000250: 7661 6c75 6573 2061 7265 2063 6f6e 6361  values are conca
+00000260: 7465 6e61 7465 6420 6173 2073 6570 6172  tenated as separ
+00000270: 6174 6520 7061 7261 6772 6170 6873 2e29  ate paragraphs.)
+00000280: 03da 076d 6574 6176 6172 da06 6163 7469  ...metavar..acti
+00000290: 6f6e da04 6865 6c70 7a02 2d61 7a05 2d2d  on..helpz.-az.--
+000002a0: 616c 6cda 0a73 746f 7265 5f74 7275 6546  all..store_trueF
+000002b0: 7a8e 5465 6c6c 2074 6865 2063 6f6d 6d61  z.Tell the comma
+000002c0: 6e64 2074 6f20 6175 746f 6d61 7469 6361  nd to automatica
+000002d0: 6c6c 7920 7374 6167 6520 6669 6c65 7320  lly stage files 
+000002e0: 7468 6174 2068 6176 6520 6265 656e 206d  that have been m
+000002f0: 6f64 6966 6965 6420 616e 6420 6465 6c65  odified and dele
+00000300: 7465 642c 2062 7574 206e 6577 2066 696c  ted, but new fil
+00000310: 6573 2079 6f75 2068 6176 6520 6e6f 7420  es you have not 
+00000320: 746f 6c64 2047 6974 2061 626f 7574 2061  told Git about a
+00000330: 7265 206e 6f74 2061 6666 6563 7465 642e  re not affected.
+00000340: 2903 7205 0000 00da 0764 6566 6175 6c74  ).r......default
+00000350: 7206 0000 007a 072d 2d66 6978 7570 7a19  r....z.--fixupz.
+00000360: 5b28 616d 656e 647c 7265 776f 7264 293a  [(amend|reword):
+00000370: 5d3c 636f 6d6d 6974 3e29 0172 0400 0000  ]<commit>).r....
+00000380: fa08 2d2d 7371 7561 7368 7a08 3c63 6f6d  ..--squashz.<com
+00000390: 6d69 743e fa02 2d6e fa0b 2d2d 6e6f 2d76  mit>..-n..--no-v
+000003a0: 6572 6966 797a 8a42 7920 6465 6661 756c  erifyz.By defaul
+000003b0: 742c 2074 6865 2070 7265 2d63 6f6d 6d69  t, the pre-commi
+000003c0: 7420 616e 6420 636f 6d6d 6974 2d6d 7367  t and commit-msg
+000003d0: 2068 6f6f 6b73 2061 7265 2072 756e 2e20   hooks are run. 
+000003e0: 5768 656e 2061 6e79 206f 6620 2d2d 6e6f  When any of --no
+000003f0: 2d76 6572 6966 7920 6f72 202d 6e20 6973  -verify or -n is
+00000400: 2067 6976 656e 2c20 7468 6573 6520 6172   given, these ar
+00000410: 6520 6279 7061 7373 6564 2e20 5365 6520  e bypassed. See 
+00000420: 616c 736f 2067 6974 686f 6f6b 7328 3529  also githooks(5)
+00000430: 2efa 082d 2d61 7574 686f 727a 083c 6175  ...--authorz.<au
+00000440: 7468 6f72 3e61 4801 0000 4f76 6572 7269  thor>aH...Overri
+00000450: 6465 2074 6865 2063 6f6d 6d69 7420 6175  de the commit au
+00000460: 7468 6f72 2e20 5370 6563 6966 7920 616e  thor. Specify an
+00000470: 2065 7870 6c69 6369 7420 6175 7468 6f72   explicit author
+00000480: 2075 7369 6e67 2074 6865 2073 7461 6e64   using the stand
+00000490: 6172 6420 4120 5520 5468 6f72 203c 6175  ard A U Thor <au
+000004a0: 7468 6f72 4065 7861 6d70 6c65 2e63 6f6d  thor@example.com
+000004b0: 3e20 666f 726d 6174 2e20 4f74 6865 7277  > format. Otherw
+000004c0: 6973 6520 3c61 7574 686f 723e 2069 7320  ise <author> is 
+000004d0: 6173 7375 6d65 6420 746f 2062 6520 6120  assumed to be a 
+000004e0: 7061 7474 6572 6e20 616e 6420 6973 2075  pattern and is u
+000004f0: 7365 6420 746f 2073 6561 7263 6820 666f  sed to search fo
+00000500: 7220 616e 2065 7869 7374 696e 6720 636f  r an existing co
+00000510: 6d6d 6974 2062 7920 7468 6174 2061 7574  mmit by that aut
+00000520: 686f 7220 2869 2e65 2e20 7265 762d 6c69  hor (i.e. rev-li
+00000530: 7374 202d 2d61 6c6c 202d 6920 2d2d 6175  st --all -i --au
+00000540: 7468 6f72 3d3c 6175 7468 6f72 3e29 3b20  thor=<author>); 
+00000550: 7468 6520 636f 6d6d 6974 2061 7574 686f  the commit autho
+00000560: 7220 6973 2074 6865 6e20 636f 7069 6564  r is then copied
+00000570: 2066 726f 6d20 7468 6520 6669 7273 7420   from the first 
+00000580: 7375 6368 2063 6f6d 6d69 7420 666f 756e  such commit foun
+00000590: 642e 2902 7204 0000 0072 0600 0000 fa06  d.).r....r......
+000005a0: 2d2d 6461 7465 7a06 3c64 6174 653e 7a2c  --datez.<date>z,
+000005b0: 4f76 6572 7269 6465 2074 6865 2061 7574  Override the aut
+000005c0: 686f 7220 6461 7465 2075 7365 6420 696e  hor date used in
+000005d0: 2074 6865 2063 6f6d 6d69 742e 7a0d 2d2d   the commit.z.--
+000005e0: 616c 6c6f 772d 656d 7074 797a f355 7375  allow-emptyz.Usu
+000005f0: 616c 6c79 2072 6563 6f72 6469 6e67 2061  ally recording a
+00000600: 2063 6f6d 6d69 7420 7468 6174 2068 6173   commit that has
+00000610: 2074 6865 2065 7861 6374 2073 616d 6520   the exact same 
+00000620: 7472 6565 2061 7320 6974 7320 736f 6c65  tree as its sole
+00000630: 2070 6172 656e 7420 636f 6d6d 6974 2069   parent commit i
+00000640: 7320 6120 6d69 7374 616b 652c 2061 6e64  s a mistake, and
+00000650: 2074 6865 2063 6f6d 6d61 6e64 2070 7265   the command pre
+00000660: 7665 6e74 7320 796f 7520 6672 6f6d 206d  vents you from m
+00000670: 616b 696e 6720 7375 6368 2061 2063 6f6d  aking such a com
+00000680: 6d69 742e 2054 6869 7320 6f70 7469 6f6e  mit. This option
+00000690: 2062 7970 6173 7365 7320 7468 6520 7361   bypasses the sa
+000006a0: 6665 7479 2c20 616e 6420 6973 2070 7269  fety, and is pri
+000006b0: 6d61 7269 6c79 2066 6f72 2075 7365 2062  marily for use b
+000006c0: 7920 666f 7265 6967 6e20 5343 4d20 696e  y foreign SCM in
+000006d0: 7465 7266 6163 6520 7363 7269 7074 732e  terface scripts.
+000006e0: 7a02 2d65 7a06 2d2d 6564 6974 7ad8 5468  z.-ez.--editz.Th
+000006f0: 6520 6d65 7373 6167 6520 7461 6b65 6e20  e message taken 
+00000700: 6672 6f6d 2066 696c 6520 7769 7468 202d  from file with -
+00000710: 462c 2063 6f6d 6d61 6e64 206c 696e 6520  F, command line 
+00000720: 7769 7468 202d 6d2c 2061 6e64 2066 726f  with -m, and fro
+00000730: 6d20 636f 6d6d 6974 206f 626a 6563 7420  m commit object 
+00000740: 7769 7468 202d 4320 6172 6520 7573 7561  with -C are usua
+00000750: 6c6c 7920 7573 6564 2061 7320 7468 6520  lly used as the 
+00000760: 636f 6d6d 6974 206c 6f67 206d 6573 7361  commit log messa
+00000770: 6765 2075 6e6d 6f64 6966 6965 642e 2054  ge unmodified. T
+00000780: 6869 7320 6f70 7469 6f6e 206c 6574 7320  his option lets 
+00000790: 796f 7520 6675 7274 6865 7220 6564 6974  you further edit
+000007a0: 2074 6865 206d 6573 7361 6765 2074 616b   the message tak
+000007b0: 656e 2066 726f 6d20 7468 6573 6520 736f  en from these so
+000007c0: 7572 6365 732e fa09 2d2d 6e6f 2d65 6469  urces...--no-edi
+000007d0: 747a 9b55 7365 2074 6865 2073 656c 6563  tz.Use the selec
+000007e0: 7465 6420 636f 6d6d 6974 206d 6573 7361  ted commit messa
+000007f0: 6765 2077 6974 686f 7574 206c 6175 6e63  ge without launc
+00000800: 6869 6e67 2061 6e20 6564 6974 6f72 2e20  hing an editor. 
+00000810: 466f 7220 6578 616d 706c 652c 2067 6974  For example, git
+00000820: 2063 6f6d 6d69 7420 2d2d 616d 656e 6420   commit --amend 
+00000830: 2d2d 6e6f 2d65 6469 7420 616d 656e 6473  --no-edit amends
+00000840: 2061 2063 6f6d 6d69 7420 7769 7468 6f75   a commit withou
+00000850: 7420 6368 616e 6769 6e67 2069 7473 2063  t changing its c
+00000860: 6f6d 6d69 7420 6d65 7373 6167 652e 7a07  ommit message.z.
+00000870: 2d2d 616d 656e 6461 5203 0000 5265 706c  --amendaR...Repl
+00000880: 6163 6520 7468 6520 7469 7020 6f66 2074  ace the tip of t
+00000890: 6865 2063 7572 7265 6e74 2062 7261 6e63  he current branc
+000008a0: 6820 6279 2063 7265 6174 696e 6720 6120  h by creating a 
+000008b0: 6e65 7720 636f 6d6d 6974 2e20 5468 6520  new commit. The 
+000008c0: 7265 636f 7264 6564 2074 7265 6520 6973  recorded tree is
+000008d0: 2070 7265 7061 7265 6420 6173 2075 7375   prepared as usu
+000008e0: 616c 2028 696e 636c 7564 696e 6720 7468  al (including th
+000008f0: 6520 6566 6665 6374 206f 6620 7468 6520  e effect of the 
+00000900: 2d69 2061 6e64 202d 6f20 6f70 7469 6f6e  -i and -o option
+00000910: 7320 616e 6420 6578 706c 6963 6974 2070  s and explicit p
+00000920: 6174 6873 7065 6329 2c20 616e 6420 7468  athspec), and th
+00000930: 6520 6d65 7373 6167 6520 6672 6f6d 2074  e message from t
+00000940: 6865 206f 7269 6769 6e61 6c20 636f 6d6d  he original comm
+00000950: 6974 2069 7320 7573 6564 2061 7320 7468  it is used as th
+00000960: 6520 7374 6172 7469 6e67 2070 6f69 6e74  e starting point
+00000970: 2c20 696e 7374 6561 6420 6f66 2061 6e20  , instead of an 
+00000980: 656d 7074 7920 6d65 7373 6167 652c 2077  empty message, w
+00000990: 6865 6e20 6e6f 206f 7468 6572 206d 6573  hen no other mes
+000009a0: 7361 6765 2069 7320 7370 6563 6966 6965  sage is specifie
+000009b0: 6420 6672 6f6d 2074 6865 2063 6f6d 6d61  d from the comma
+000009c0: 6e64 206c 696e 6520 7669 6120 6f70 7469  nd line via opti
+000009d0: 6f6e 7320 7375 6368 2061 7320 2d6d 2c20  ons such as -m, 
+000009e0: 2d46 2c20 2d63 2c20 6574 632e 2054 6865  -F, -c, etc. The
+000009f0: 206e 6577 2063 6f6d 6d69 7420 6861 7320   new commit has 
+00000a00: 7468 6520 7361 6d65 2070 6172 656e 7473  the same parents
+00000a10: 2061 6e64 2061 7574 686f 7220 6173 2074   and author as t
+00000a20: 6865 2063 7572 7265 6e74 206f 6e65 2028  he current one (
+00000a30: 7468 6520 2d2d 7265 7365 742d 6175 7468  the --reset-auth
+00000a40: 6f72 206f 7074 696f 6e20 6361 6e20 636f  or option can co
+00000a50: 756e 7465 726d 616e 6420 7468 6973 292e  untermand this).
+00000a60: 2049 7420 6973 2061 2072 6f75 6768 2065   It is a rough e
+00000a70: 7175 6976 616c 656e 7420 666f 723a 2024  quivalent for: $
+00000a80: 2067 6974 2072 6573 6574 202d 2d73 6f66   git reset --sof
+00000a90: 7420 4845 4144 5e20 2420 2e2e 2e20 646f  t HEAD^ $ ... do
+00000aa0: 2073 6f6d 6574 6869 6e67 2065 6c73 6520   something else 
+00000ab0: 746f 2063 6f6d 6520 7570 2077 6974 6820  to come up with 
+00000ac0: 7468 6520 7269 6768 7420 7472 6565 202e  the right tree .
+00000ad0: 2e2e 2024 2067 6974 2063 6f6d 6d69 7420  .. $ git commit 
+00000ae0: 2d63 204f 5249 475f 4845 4144 2062 7574  -c ORIG_HEAD but
+00000af0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+00000b00: 616d 656e 6420 6120 6d65 7267 6520 636f  amend a merge co
+00000b10: 6d6d 6974 2e20 596f 7520 7368 6f75 6c64  mmit. You should
+00000b20: 2075 6e64 6572 7374 616e 6420 7468 6520   understand the 
+00000b30: 696d 706c 6963 6174 696f 6e73 206f 6620  implications of 
+00000b40: 7265 7772 6974 696e 6720 6869 7374 6f72  rewriting histor
+00000b50: 7920 6966 2079 6f75 2061 6d65 6e64 2061  y if you amend a
+00000b60: 2063 6f6d 6d69 7420 7468 6174 2068 6173   commit that has
+00000b70: 2061 6c72 6561 6479 2062 6565 6e20 7075   already been pu
+00000b80: 626c 6973 6865 642e 2028 5365 6520 7468  blished. (See th
+00000b90: 6520 2252 4543 4f56 4552 494e 4720 4652  e "RECOVERING FR
+00000ba0: 4f4d 2055 5053 5452 4541 4d20 5245 4241  OM UPSTREAM REBA
+00000bb0: 5345 2220 7365 6374 696f 6e20 696e 2067  SE" section in g
+00000bc0: 6974 2d72 6562 6173 6528 3129 2e29 7a11  it-rebase(1).)z.
+00000bd0: 2d2d 6e6f 2d70 6f73 742d 7265 7772 6974  --no-post-rewrit
+00000be0: 657a 1d42 7970 6173 7320 7468 6520 706f  ez.Bypass the po
+00000bf0: 7374 2d72 6577 7269 7465 2068 6f6f 6b2e  st-rewrite hook.
+00000c00: fa02 2d71 fa07 2d2d 7175 6965 747a 2053  ..-q..--quietz S
+00000c10: 7570 7072 6573 7320 636f 6d6d 6974 2073  uppress commit s
+00000c20: 756d 6d61 7279 206d 6573 7361 6765 2e7a  ummary message.z
+00000c30: 092d 2d64 7279 2d72 756e 7a9f 446f 206e  .--dry-runz.Do n
+00000c40: 6f74 2063 7265 6174 6520 6120 636f 6d6d  ot create a comm
+00000c50: 6974 2c20 6275 7420 7368 6f77 2061 206c  it, but show a l
+00000c60: 6973 7420 6f66 2070 6174 6873 2074 6861  ist of paths tha
+00000c70: 7420 6172 6520 746f 2062 6520 636f 6d6d  t are to be comm
+00000c80: 6974 7465 642c 2070 6174 6873 2077 6974  itted, paths wit
+00000c90: 6820 6c6f 6361 6c20 6368 616e 6765 7320  h local changes 
+00000ca0: 7468 6174 2077 696c 6c20 6265 206c 6566  that will be lef
+00000cb0: 7420 756e 636f 6d6d 6974 7465 6420 616e  t uncommitted an
+00000cc0: 6420 7061 7468 7320 7468 6174 2061 7265  d paths that are
+00000cd0: 2075 6e74 7261 636b 6564 2e29 03da 0470   untracked.)...p
+00000ce0: 726f 67da 0b64 6573 6372 6970 7469 6f6e  rog..description
+00000cf0: da0c 6164 645f 6172 6775 6d65 6e74 a901  ..add_argument..
+00000d00: da06 7061 7273 6572 a900 7216 0000 00fa  ..parser..r.....
+00000d10: 212f 6472 6f6e 652f 7372 632f 7372 632f  !/drone/src/src/
+00000d20: 7475 6976 6965 772f 636d 642f 6769 742e  tuiview/cmd/git.
+00000d30: 7079 da0a 6769 745f 636f 6d6d 6974 0700  py..git_commit..
+00000d40: 0000 73aa 0000 0006 0106 0104 0302 0102  ..s.............
+00000d50: 0102 0102 0102 0106 fb04 0702 0102 0102  ................
+00000d60: 0102 0102 0106 fb04 0702 0102 0106 fe04  ................
+00000d70: 0402 0102 0106 fe04 0402 0102 0102 0102  ................
+00000d80: 0102 0106 fb04 0702 0102 0102 0106 fd04  ................
+00000d90: 0502 0102 0102 0106 fd04 0502 0102 0102  ................
+00000da0: 0102 0106 fc04 0602 0102 0102 0102 0102  ................
+00000db0: 0106 fb04 0702 0102 0102 0102 0106 fc04  ................
+00000dc0: 0602 0102 0102 0102 0106 fc04 0602 0102  ................
+00000dd0: 0102 0102 0106 fc04 0602 0102 0102 0102  ................
+00000de0: 0102 0106 fb04 0702 0102 0102 0102 010a  ................
+00000df0: fc72 1800 0000 6301 0000 0000 0000 0000  .r....c.........
+00000e00: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
+00000e10: d200 0000 6401 7c00 5f00 6402 7c00 5f01  ....d.|._.d.|._.
+00000e20: 7c00 6a02 6403 6404 6405 6406 8d03 0100  |.j.d.d.d.d.....
+00000e30: 7c00 6a02 6407 6408 6409 640a 640b 8d04  |.j.d.d.d.d.d...
+00000e40: 0100 7c00 6a02 640c 6409 640d 640b 8d03  ..|.j.d.d.d.d...
+00000e50: 0100 7c00 6a02 640e 6409 640f 640b 8d03  ..|.j.d.d.d.d...
+00000e60: 0100 7c00 6a02 6410 6411 6409 6412 6413  ..|.j.d.d.d.d.d.
+00000e70: 8d04 0100 7c00 6a02 6414 6415 6409 6416  ....|.j.d.d.d.d.
+00000e80: 6413 8d04 0100 7c00 6a02 6417 6418 6409  d.....|.j.d.d.d.
+00000e90: 6419 6413 8d04 0100 7c00 6a02 641a 641b  d.d.....|.j.d.d.
+00000ea0: 6409 641c 640b 8d04 0100 7c00 6a02 641d  d.d.d.....|.j.d.
+00000eb0: 641e 6409 641f 640b 8d04 0100 7c00 6a02  d.d.d.d.....|.j.
+00000ec0: 6420 7403 6a04 6a05 6421 6422 6423 8d04  d t.j.j.d!d"d#..
+00000ed0: 0100 7c00 6a02 6424 6409 6425 640b 8d03  ..|.j.d$d.d%d...
+00000ee0: 0100 6400 5300 2926 4e7a 0967 6974 2d6d  ..d.S.)&Nz.git-m
+00000ef0: 6572 6765 7a2f 4a6f 696e 2074 776f 206f  ergez/Join two o
+00000f00: 7220 6d6f 7265 2064 6576 656c 6f70 6d65  r more developme
+00000f10: 6e74 2068 6973 746f 7269 6573 2074 6f67  nt histories tog
+00000f20: 6574 6865 72da 0663 6f6d 6d69 74da 012a  ether..commit..*
+00000f30: 7a20 436f 6d6d 6974 7320 746f 206d 6572  z Commits to mer
+00000f40: 6765 2069 6e74 6f20 6f75 7220 6272 616e  ge into our bran
+00000f50: 6368 a902 da05 6e61 7267 7372 0600 0000  ch....nargsr....
+00000f60: 720a 0000 007a 0b2d 2d6e 6f2d 636f 6d6d  r....z.--no-comm
+00000f70: 6974 7207 0000 007a 2f50 6572 666f 726d  itr....z/Perform
+00000f80: 2074 6865 206d 6572 6765 2077 6974 686f   the merge witho
+00000f90: 7574 2063 6f6d 6d69 7474 696e 6720 7468  ut committing th
+00000fa0: 6520 7265 7375 6c74 a902 7205 0000 0072  e result..r....r
+00000fb0: 0600 0000 7209 0000 007a 6750 726f 6475  ....r....zgProdu
+00000fc0: 6365 2074 6865 2077 6f72 6b69 6e67 2074  ce the working t
+00000fd0: 7265 6520 616e 6420 696e 6465 7820 7374  ree and index st
+00000fe0: 6174 6520 6173 2069 6620 6120 7265 616c  ate as if a real
+00000ff0: 206d 6572 6765 2068 6170 7065 6e65 642c   merge happened,
+00001000: 2062 7574 2064 6f20 6e6f 7420 6163 7475   but do not actu
+00001010: 616c 6c79 206d 616b 6520 6120 636f 6d6d  ally make a comm
+00001020: 6974 7a06 2d2d 7374 6174 7a27 5368 6f77  itz.--statz'Show
+00001030: 2061 2064 6966 6673 7461 7420 6174 2074   a diffstat at t
+00001040: 6865 2065 6e64 206f 6620 7468 6520 6d65  he end of the me
+00001050: 7267 6572 0e00 0000 da04 6564 6974 7a3e  rger......editz>
+00001060: 496e 766f 6b65 2061 6e20 6564 6974 6f72  Invoke an editor
+00001070: 2062 6566 6f72 6520 636f 6d6d 6974 7469   before committi
+00001080: 6e67 2073 7563 6365 7373 6675 6c20 6d65  ng successful me
+00001090: 6368 616e 6963 616c 206d 6572 6765 a903  chanical merge..
+000010a0: da04 6465 7374 7205 0000 0072 0600 0000  ..destr....r....
+000010b0: 720b 0000 00da 0676 6572 6966 797a 2353  r......verifyz#S
+000010c0: 6b69 7020 7072 652d 6d65 7267 6520 616e  kip pre-merge an
+000010d0: 6420 636f 6d6d 6974 2d6d 7367 2068 6f6f  d commit-msg hoo
+000010e0: 6b73 7a13 2d2d 7665 7269 6679 2d73 6967  ksz.--verify-sig
+000010f0: 6e61 7475 7265 735a 1176 6572 6966 795f  naturesZ.verify_
+00001100: 7369 676e 6174 7572 6573 7a55 5665 7269  signatureszUVeri
+00001110: 6679 2074 6861 7420 7468 6520 7469 7020  fy that the tip 
+00001120: 636f 6d6d 6974 206f 6620 7468 6520 7369  commit of the si
+00001130: 6465 2062 7261 6e63 6820 6265 696e 6720  de branch being 
+00001140: 6d65 7267 6564 2069 7320 7369 676e 6564  merged is signed
+00001150: 2077 6974 6820 6120 7661 6c69 6420 6b65   with a valid ke
+00001160: 7972 1000 0000 720f 0000 007a 0f4f 7065  yr....r....z.Ope
+00001170: 7261 7465 2071 7569 6574 6c79 7a09 2d2d  rate quietlyz.--
+00001180: 7665 7262 6f73 657a 022d 767a 0a42 6520  verbosez.-vz.Be 
+00001190: 7665 7262 6f73 657a 0a2d 2d70 726f 6772  verbosez.--progr
+000011a0: 6573 737a 1054 7572 6e20 7072 6f67 7265  essz.Turn progre
+000011b0: 7373 206f 6e46 2903 7205 0000 0072 0600  ss onF).r....r..
+000011c0: 0000 7208 0000 007a 0b2d 2d61 7574 6f73  ..r....z.--autos
+000011d0: 7461 7368 7a48 4175 746f 6d61 7469 6361  tashzHAutomatica
+000011e0: 6c6c 7920 6372 6561 7465 2061 2074 656d  lly create a tem
+000011f0: 706f 7261 7279 2073 7461 7368 2065 6e74  porary stash ent
+00001200: 7279 2062 6566 6f72 6520 7468 6520 6f70  ry before the op
+00001210: 6572 6174 696f 6e20 6265 6769 6e73 2906  eration begins).
+00001220: 7211 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00001230: 0479 6170 78da 0761 6374 696f 6e73 da15  .yapx..actions..
+00001240: 426f 6f6c 6561 6e4f 7074 696f 6e61 6c41  BooleanOptionalA
+00001250: 6374 696f 6e72 1400 0000 7216 0000 0072  ctionr....r....r
+00001260: 1600 0000 7217 0000 00da 0967 6974 5f6d  ....r......git_m
+00001270: 6572 6765 6100 0000 7364 0000 0006 0106  ergea...sd......
+00001280: 0110 0204 0202 0102 0102 0102 0106 fc04  ................
+00001290: 0602 0102 0102 0106 fd04 0502 0102 0102  ................
+000012a0: 0106 fd04 0502 0102 0102 0102 0106 fc04  ................
+000012b0: 0602 0102 0102 0102 0106 fc04 0602 0102  ................
+000012c0: 0102 0102 0106 fc12 0612 0104 0102 0106  ................
+000012d0: 0102 0102 0106 fc04 0602 0102 0102 010a  ................
+000012e0: fd72 2500 0000 6301 0000 0000 0000 0000  .r%...c.........
+000012f0: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
+00001300: 9402 0000 6401 7c00 5f00 6402 7c00 5f01  ....d.|._.d.|._.
+00001310: 7c00 6a02 6403 6404 6405 6406 8d03 0100  |.j.d.d.d.d.....
+00001320: 7c00 6a02 6407 6404 6408 6406 8d03 0100  |.j.d.d.d.d.....
+00001330: 7c00 6a02 6409 640a 6700 640b a201 640c  |.j.d.d.g.d...d.
+00001340: 640d 640e 8d05 0100 7c00 6a02 640f 6410  d.d.....|.j.d.d.
+00001350: 6404 640d 6411 8d04 0100 7c00 6a02 6412  d.d.d.....|.j.d.
+00001360: 6413 6414 6415 8d03 0100 7c00 6a02 6416  d.d.d.....|.j.d.
+00001370: 6417 6414 6415 8d03 0100 7c00 6a02 6418  d.d.d.....|.j.d.
+00001380: 6404 6419 6406 8d03 0100 7c00 6a02 641a  d.d.d.....|.j.d.
+00001390: 6404 641b 6406 8d03 0100 7c00 6a02 641c  d.d.d.....|.j.d.
+000013a0: 7403 641d 641e 641f 8d04 0100 7c00 6a02  t.d.d.d.....|.j.
+000013b0: 6420 7403 6421 6422 8d03 0100 7c00 6a02  d t.d!d"....|.j.
+000013c0: 6423 6424 6425 6426 6415 8d04 0100 7c00  d#d$d%d&d.....|.
+000013d0: 6a02 6427 6428 6429 642a 6415 8d04 0100  j.d'd(d)d*d.....
+000013e0: 7c00 6a02 642b 642c 642d 642e 8d03 0100  |.j.d+d,d-d.....
+000013f0: 7c00 6a02 642f 642c 6430 642e 8d03 0100  |.j.d/d,d0d.....
+00001400: 7c00 6a02 6431 642c 6432 642e 8d03 0100  |.j.d1d,d2d.....
+00001410: 7c00 6a02 6433 642c 6434 642e 8d03 0100  |.j.d3d,d4d.....
+00001420: 7c00 6a02 6435 6404 6436 6406 8d03 0100  |.j.d5d.d6d.....
+00001430: 7c00 6a02 6437 6404 6438 6406 8d03 0100  |.j.d7d.d8d.....
+00001440: 7c00 6a02 6439 643a 6404 643b 6406 8d04  |.j.d9d:d.d;d...
+00001450: 0100 7c00 6a02 643c 6404 643d 6406 8d03  ..|.j.d<d.d=d...
+00001460: 0100 7c00 6a02 643e 643f 6404 6440 6406  ..|.j.d>d?d.d@d.
+00001470: 8d04 0100 7c00 6a02 6441 6442 6404 6443  ....|.j.dAdBd.dC
+00001480: 6406 8d04 0100 7c00 6a02 6444 6445 6404  d.....|.j.dDdEd.
+00001490: 6446 6406 8d04 0100 7c00 6a02 6447 6404  dFd.....|.j.dGd.
+000014a0: 6448 6406 8d03 0100 7c00 6a02 6449 6404  dHd.....|.j.dId.
+000014b0: 644a 6406 8d03 0100 7c00 6a02 644b 642c  dJd.....|.j.dKd,
+000014c0: 644c 642e 8d03 0100 7c00 6a02 644d 6404  dLd.....|.j.dMd.
+000014d0: 644e 6406 8d03 0100 7c00 6a02 644f 6404  dNd.....|.j.dOd.
+000014e0: 6450 6406 8d03 0100 7c00 6a02 6451 6404  dPd.....|.j.dQd.
+000014f0: 6452 6406 8d03 0100 7c00 6a02 6453 6404  dRd.....|.j.dSd.
+00001500: 6454 6406 8d03 0100 7c00 6a02 6455 640a  dTd.....|.j.dUd.
+00001510: 6456 6457 6458 8d04 0100 7c00 6a02 6459  dVdWdX....|.j.dY
+00001520: 6404 645a 6406 8d03 0100 7c00 6a02 645b  d.dZd.....|.j.d[
+00001530: 6404 645c 8d02 0100 7c00 6a02 645d 6404  d.d\....|.j.d]d.
+00001540: 645e 6406 8d03 0100 7c00 6a02 645f 6404  d^d.....|.j.d_d.
+00001550: 6460 6406 8d03 0100 7c00 6a02 6461 6462  d`d.....|.j.dadb
+00001560: 6463 8d02 0100 7c00 6a02 6464 6404 6465  dc....|.j.ddd.de
+00001570: 6406 8d03 0100 7c00 6a02 6466 640a 6467  d.....|.j.dfd.dg
+00001580: 8d02 0100 7c00 6a02 6468 7404 6a05 6467  ....|.j.dht.j.dg
+00001590: 8d02 0100 6400 5300 2969 4e7a 0767 6974  ....d.S.)iNz.git
+000015a0: 2d6c 6f67 7a10 5368 6f77 2063 6f6d 6d69  -logz.Show commi
+000015b0: 7420 6c6f 6773 7a07 2d2d 6772 6170 6872  t logsz.--graphr
+000015c0: 0700 0000 7a64 4472 6177 2061 2074 6578  ....zdDraw a tex
+000015d0: 742d 6261 7365 6420 6772 6170 6869 6361  t-based graphica
+000015e0: 6c20 7265 7072 6573 656e 7461 7469 6f6e  l representation
+000015f0: 206f 6620 7468 6520 636f 6d6d 6974 2068   of the commit h
+00001600: 6973 746f 7279 206f 6e20 7468 6520 6c65  istory on the le
+00001610: 6674 2068 616e 6420 7369 6465 206f 6620  ft hand side of 
+00001620: 7468 6520 6f75 7470 7574 721d 0000 007a  the outputr....z
+00001630: 082d 2d66 6f6c 6c6f 777a 5443 6f6e 7469  .--followzTConti
+00001640: 6e75 6520 6c69 7374 696e 6720 7468 6520  nue listing the 
+00001650: 6869 7374 6f72 7920 6f66 2061 2066 696c  history of a fil
+00001660: 6520 6265 796f 6e64 2072 656e 616d 6573  e beyond renames
+00001670: 2028 776f 726b 7320 6f6e 6c79 2066 6f72   (works only for
+00001680: 2061 2073 696e 676c 6520 6669 6c65 297a   a single file)z
+00001690: 0a2d 2d64 6563 6f72 6174 65fa 013f 2904  .--decorate..?).
+000016a0: da05 7368 6f72 74da 0466 756c 6cda 0461  ..short..full..a
+000016b0: 7574 6fda 026e 6f72 2700 0000 7a35 5072  uto..nor'...z5Pr
+000016c0: 696e 7420 6f75 7420 7468 6520 7265 6620  int out the ref 
+000016d0: 6e61 6d65 7320 6f66 2061 6e79 2063 6f6d  names of any com
+000016e0: 6d69 7473 2074 6861 7420 6172 6520 7368  mits that are sh
+000016f0: 6f77 6e29 0472 1c00 0000 da07 6368 6f69  own).r......choi
+00001700: 6365 73da 0563 6f6e 7374 7206 0000 007a  ces..constr....z
+00001710: 0d2d 2d6e 6f2d 6465 636f 7261 7465 da08  .--no-decorate..
+00001720: 6465 636f 7261 7465 721f 0000 007a 0f2d  decorater....z.-
+00001730: 2d64 6563 6f72 6174 652d 7265 6673 5a0d  -decorate-refsZ.
+00001740: 6465 636f 7261 7465 5f72 6566 737a 4449  decorate_refszDI
+00001750: 6620 6e6f 202d 2d64 6563 6f72 6174 652d  f no --decorate-
+00001760: 7265 6673 2069 7320 6769 7665 6e2c 2070  refs is given, p
+00001770: 7265 7465 6e64 2061 7320 6966 2061 6c6c  retend as if all
+00001780: 2072 6566 7320 7765 7265 2069 6e63 6c75   refs were inclu
+00001790: 6465 6429 0272 2000 0000 7206 0000 007a  ded).r ...r....z
+000017a0: 172d 2d64 6563 6f72 6174 652d 7265 6673  .--decorate-refs
+000017b0: 2d65 7863 6c75 6465 5a15 6465 636f 7261  -excludeZ.decora
+000017c0: 7465 5f72 6566 735f 6578 636c 7564 657a  te_refs_excludez
+000017d0: 082d 2d73 6f75 7263 657a 5150 7269 6e74  .--sourcezQPrint
+000017e0: 206f 7574 2074 6865 2072 6566 206e 616d   out the ref nam
+000017f0: 6520 6769 7665 6e20 6f6e 2074 6865 2063  e given on the c
+00001800: 6f6d 6d61 6e64 206c 696e 6520 6279 2077  ommand line by w
+00001810: 6869 6368 2065 6163 6820 636f 6d6d 6974  hich each commit
+00001820: 2077 6173 2072 6561 6368 6564 7a0b 2d2d   was reachedz.--
+00001830: 6675 6c6c 2d64 6966 6675 2901 0000 5769  full-diffu)...Wi
+00001840: 7468 6f75 7420 7468 6973 2066 6c61 672c  thout this flag,
+00001850: 2067 6974 206c 6f67 202d 7020 3c70 6174   git log -p <pat
+00001860: 683e 2e2e 2e20 7368 6f77 7320 636f 6d6d  h>... shows comm
+00001870: 6974 7320 7468 6174 2074 6f75 6368 2074  its that touch t
+00001880: 6865 2073 7065 6369 6669 6564 2070 6174  he specified pat
+00001890: 6873 2c20 616e 6420 6469 6666 7320 6162  hs, and diffs ab
+000018a0: 6f75 7420 7468 6520 7361 6d65 2073 7065  out the same spe
+000018b0: 6369 6669 6564 2070 6174 6873 2e20 5769  cified paths. Wi
+000018c0: 7468 2074 6869 732c 2074 6865 2066 756c  th this, the ful
+000018d0: 6c20 6469 6666 2069 7320 7368 6f77 6e20  l diff is shown 
+000018e0: 666f 7220 636f 6d6d 6974 7320 7468 6174  for commits that
+000018f0: 2074 6f75 6368 2074 6865 2073 7065 6369   touch the speci
+00001900: 6669 6564 2070 6174 6873 3b20 7468 6973  fied paths; this
+00001910: 206d 6561 6e73 2074 6861 7420 223c 7061   means that "<pa
+00001920: 7468 3e2e 2e2e 2220 6c69 6d69 7473 206f  th>..." limits o
+00001930: 6e6c 7920 636f 6d6d 6974 732c 2061 6e64  nly commits, and
+00001940: 2064 6f65 736e e280 9974 206c 696d 6974   doesn...t limit
+00001950: 2064 6966 6620 666f 7220 7468 6f73 6520   diff for those 
+00001960: 636f 6d6d 6974 7372 0a00 0000 da09 6d61  commitsr......ma
+00001970: 785f 636f 756e 747a 254c 696d 6974 2074  x_countz%Limit t
+00001980: 6865 206e 756d 6265 7220 6f66 2063 6f6d  he number of com
+00001990: 6d69 7473 2074 6f20 6f75 7470 7574 2903  mits to output).
+000019a0: da04 7479 7065 7220 0000 0072 0600 0000  ..typer ...r....
+000019b0: 7a06 2d2d 736b 6970 7a3d 536b 6970 206e  z.--skipz=Skip n
+000019c0: 756d 6265 7220 636f 6d6d 6974 7320 6265  umber commits be
+000019d0: 666f 7265 2073 7461 7274 696e 6720 746f  fore starting to
+000019e0: 2073 686f 7720 7468 6520 636f 6d6d 6974   show the commit
+000019f0: 206f 7574 7075 7429 0272 2f00 0000 7206   output).r/...r.
+00001a00: 0000 007a 072d 2d73 696e 6365 7a07 2d2d  ...z.--sincez.--
+00001a10: 6166 7465 725a 0a73 696e 6365 5f64 6174  afterZ.since_dat
+00001a20: 657a 2d53 686f 7720 636f 6d6d 6974 7320  ez-Show commits 
+00001a30: 6d6f 7265 2072 6563 656e 7420 7468 616e  more recent than
+00001a40: 2061 2073 7065 6369 6669 6320 6461 7465   a specific date
+00001a50: 7a07 2d2d 756e 7469 6c7a 082d 2d62 6566  z.--untilz.--bef
+00001a60: 6f72 655a 0a75 6e74 696c 5f64 6174 657a  oreZ.until_datez
+00001a70: 2753 686f 7720 636f 6d6d 6974 7320 6f6c  'Show commits ol
+00001a80: 6465 7220 7468 616e 2061 2073 7065 6369  der than a speci
+00001a90: 6669 6320 6461 7465 720c 0000 00fa 012b  fic dater......+
+00001aa0: 7a6f 4c69 6d69 7420 7468 6520 636f 6d6d  zoLimit the comm
+00001ab0: 6974 7320 6f75 7470 7574 2074 6f20 6f6e  its output to on
+00001ac0: 6573 2077 6974 6820 6175 7468 6f72 2068  es with author h
+00001ad0: 6561 6465 7220 6c69 6e65 7320 7468 6174  eader lines that
+00001ae0: 206d 6174 6368 2074 6865 2073 7065 6369   match the speci
+00001af0: 6669 6564 2070 6174 7465 726e 2028 7265  fied pattern (re
+00001b00: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00001b10: 2972 1b00 0000 7a0b 2d2d 636f 6d6d 6974  )r....z.--commit
+00001b20: 7465 727a 724c 696d 6974 2074 6865 2063  terzrLimit the c
+00001b30: 6f6d 6d69 7473 206f 7574 7075 7420 746f  ommits output to
+00001b40: 206f 6e65 7320 7769 7468 2063 6f6d 6d69   ones with commi
+00001b50: 7474 6572 2068 6561 6465 7220 6c69 6e65  tter header line
+00001b60: 7320 7468 6174 206d 6174 6368 2074 6865  s that match the
+00001b70: 2073 7065 6369 6669 6564 2070 6174 7465   specified patte
+00001b80: 726e 2028 7265 6775 6c61 7220 6578 7072  rn (regular expr
+00001b90: 6573 7369 6f6e 297a 0d2d 2d67 7265 702d  ession)z.--grep-
+00001ba0: 7265 666c 6f67 7aad 4c69 6d69 7420 7468  reflogz.Limit th
+00001bb0: 6520 636f 6d6d 6974 7320 6f75 7470 7574  e commits output
+00001bc0: 2074 6f20 6f6e 6573 2077 6974 6820 7265   to ones with re
+00001bd0: 666c 6f67 2065 6e74 7269 6573 2074 6861  flog entries tha
+00001be0: 7420 6d61 7463 6820 7468 6520 7370 6563  t match the spec
+00001bf0: 6966 6965 6420 7061 7474 6572 6e20 2872  ified pattern (r
+00001c00: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001c10: 6e29 2e20 4974 2069 7320 616e 2065 7272  n). It is an err
+00001c20: 6f72 2074 6f20 7573 6520 7468 6973 206f  or to use this o
+00001c30: 7074 696f 6e20 756e 6c65 7373 202d 2d77  ption unless --w
+00001c40: 616c 6b2d 7265 666c 6f67 7320 6973 2069  alk-reflogs is i
+00001c50: 6e20 7573 657a 062d 2d67 7265 707a d14c  n usez.--grepz.L
+00001c60: 696d 6974 2074 6865 2063 6f6d 6d69 7473  imit the commits
+00001c70: 206f 7574 7075 7420 746f 206f 6e65 7320   output to ones 
+00001c80: 7769 7468 206c 6f67 206d 6573 7361 6765  with log message
+00001c90: 2074 6861 7420 6d61 7463 6865 7320 7468   that matches th
+00001ca0: 6520 7370 6563 6966 6965 6420 7061 7474  e specified patt
+00001cb0: 6572 6e20 2872 6567 756c 6172 2065 7870  ern (regular exp
+00001cc0: 7265 7373 696f 6e29 2e20 5768 656e 202d  ression). When -
+00001cd0: 2d6e 6f74 6573 2069 7320 696e 2065 6666  -notes is in eff
+00001ce0: 6563 742c 2074 6865 206d 6573 7361 6765  ect, the message
+00001cf0: 2066 726f 6d20 7468 6520 6e6f 7465 7320   from the notes 
+00001d00: 6973 206d 6174 6368 6564 2061 7320 6966  is matched as if
+00001d10: 2069 7420 7765 7265 2070 6172 7420 6f66   it were part of
+00001d20: 2074 6865 206c 6f67 206d 6573 7361 6765   the log message
+00001d30: 7a0b 2d2d 616c 6c2d 6d61 7463 687a 654c  z.--all-matchzeL
+00001d40: 696d 6974 2074 6865 2063 6f6d 6d69 7473  imit the commits
+00001d50: 206f 7574 7075 7420 746f 206f 6e65 7320   output to ones 
+00001d60: 7468 6174 206d 6174 6368 2061 6c6c 2067  that match all g
+00001d70: 6976 656e 202d 2d67 7265 702c 2069 6e73  iven --grep, ins
+00001d80: 7465 6164 206f 6620 6f6e 6573 2074 6861  tead of ones tha
+00001d90: 7420 6d61 7463 6820 6174 206c 6561 7374  t match at least
+00001da0: 206f 6e65 7a0d 2d2d 696e 7665 7274 2d67   onez.--invert-g
+00001db0: 7265 707a 654c 696d 6974 2074 6865 2063  repzeLimit the c
+00001dc0: 6f6d 6d69 7473 206f 7574 7075 7420 746f  ommits output to
+00001dd0: 206f 6e65 7320 7769 7468 206c 6f67 206d   ones with log m
+00001de0: 6573 7361 6765 2074 6861 7420 646f 206e  essage that do n
+00001df0: 6f74 206d 6174 6368 2074 6865 2070 6174  ot match the pat
+00001e00: 7465 726e 2073 7065 6369 6669 6564 2077  tern specified w
+00001e10: 6974 6820 2d2d 6772 6570 7a02 2d69 7a14  ith --grepz.-iz.
+00001e20: 2d2d 7265 6765 7870 2d69 676e 6f72 652d  --regexp-ignore-
+00001e30: 6361 7365 7a4c 4d61 7463 6820 7468 6520  casezLMatch the 
+00001e40: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+00001e50: 6f6e 206c 696d 6974 696e 6720 7061 7474  on limiting patt
+00001e60: 6572 6e73 2077 6974 686f 7574 2072 6567  erns without reg
+00001e70: 6172 6420 746f 206c 6574 7465 7220 6361  ard to letter ca
+00001e80: 7365 7a0e 2d2d 6261 7369 632d 7265 6765  sez.--basic-rege
+00001e90: 7870 7a53 436f 6e73 6964 6572 2074 6865  xpzSConsider the
+00001ea0: 206c 696d 6974 696e 6720 7061 7474 6572   limiting patter
+00001eb0: 6e73 2074 6f20 6265 2062 6173 6963 2072  ns to be basic r
+00001ec0: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001ed0: 6e73 3b20 7468 6973 2069 7320 7468 6520  ns; this is the 
+00001ee0: 6465 6661 756c 747a 022d 457a 112d 2d65  defaultz.-Ez.--e
+00001ef0: 7874 656e 6465 642d 7265 6765 7870 7a72  xtended-regexpzr
+00001f00: 436f 6e73 6964 6572 2074 6865 206c 696d  Consider the lim
+00001f10: 6974 696e 6720 7061 7474 6572 6e73 2074  iting patterns t
+00001f20: 6f20 6265 2065 7874 656e 6465 6420 7265  o be extended re
+00001f30: 6775 6c61 7220 6578 7072 6573 7369 6f6e  gular expression
+00001f40: 7320 696e 7374 6561 6420 6f66 2074 6865  s instead of the
+00001f50: 2064 6566 6175 6c74 2062 6173 6963 2072   default basic r
+00001f60: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001f70: 6e73 7a02 2d46 7a0f 2d2d 6669 7865 642d  nsz.-Fz.--fixed-
+00001f80: 7374 7269 6e67 7375 6600 0000 436f 6e73  stringsuf...Cons
+00001f90: 6964 6572 2074 6865 206c 696d 6974 696e  ider the limitin
+00001fa0: 6720 7061 7474 6572 6e73 2074 6f20 6265  g patterns to be
+00001fb0: 2066 6978 6564 2073 7472 696e 6773 2028   fixed strings (
+00001fc0: 646f 6ee2 8099 7420 696e 7465 7270 7265  don...t interpre
+00001fd0: 7420 7061 7474 6572 6e20 6173 2061 2072  t pattern as a r
+00001fe0: 6567 756c 6172 2065 7870 7265 7373 696f  egular expressio
+00001ff0: 6e29 7a02 2d50 7a0d 2d2d 7065 726c 2d72  n)z.-Pz.--perl-r
+00002000: 6567 6578 707a 4843 6f6e 7369 6465 7220  egexpzHConsider 
+00002010: 7468 6520 6c69 6d69 7469 6e67 2070 6174  the limiting pat
+00002020: 7465 726e 7320 746f 2062 6520 5065 726c  terns to be Perl
+00002030: 2d63 6f6d 7061 7469 626c 6520 7265 6775  -compatible regu
+00002040: 6c61 7220 6578 7072 6573 7369 6f6e 737a  lar expressionsz
+00002050: 082d 2d6d 6572 6765 737a 4550 7269 6e74  .--mergeszEPrint
+00002060: 206f 6e6c 7920 6d65 7267 6520 636f 6d6d   only merge comm
+00002070: 6974 732e 2054 6869 7320 6973 2065 7861  its. This is exa
+00002080: 6374 6c79 2074 6865 2073 616d 6520 6173  ctly the same as
+00002090: 202d 2d6d 696e 2d70 6172 656e 7473 3d32   --min-parents=2
+000020a0: 7a0b 2d2d 6e6f 2d6d 6572 6765 737a 5b44  z.--no-mergesz[D
+000020b0: 6f20 6e6f 7420 7072 696e 7420 636f 6d6d  o not print comm
+000020c0: 6974 7320 7769 7468 206d 6f72 6520 7468  its with more th
+000020d0: 616e 206f 6e65 2070 6172 656e 742e 2054  an one parent. T
+000020e0: 6869 7320 6973 2065 7861 6374 6c79 2074  his is exactly t
+000020f0: 6865 2073 616d 6520 6173 202d 2d6d 6178  he same as --max
+00002100: 2d70 6172 656e 7473 3d31 7a09 2d2d 6578  -parents=1z.--ex
+00002110: 636c 7564 6561 0201 0000 446f 206e 6f74  cludea....Do not
+00002120: 2069 6e63 6c75 6465 2072 6566 7320 6d61   include refs ma
+00002130: 7463 6869 6e67 203c 676c 6f62 2d70 6174  tching <glob-pat
+00002140: 7465 726e 3e20 7468 6174 2074 6865 206e  tern> that the n
+00002150: 6578 7420 2d2d 616c 6c2c 202d 2d62 7261  ext --all, --bra
+00002160: 6e63 6865 732c 202d 2d74 6167 732c 202d  nches, --tags, -
+00002170: 2d72 656d 6f74 6573 2c20 6f72 202d 2d67  -remotes, or --g
+00002180: 6c6f 6220 776f 756c 6420 6f74 6865 7277  lob would otherw
+00002190: 6973 6520 636f 6e73 6964 6572 2e20 5265  ise consider. Re
+000021a0: 7065 7469 7469 6f6e 7320 6f66 2074 6869  petitions of thi
+000021b0: 7320 6f70 7469 6f6e 2061 6363 756d 756c  s option accumul
+000021c0: 6174 6520 6578 636c 7573 696f 6e20 7061  ate exclusion pa
+000021d0: 7474 6572 6e73 2075 7020 746f 2074 6865  tterns up to the
+000021e0: 206e 6578 7420 2d2d 616c 6c2c 202d 2d62   next --all, --b
+000021f0: 7261 6e63 6865 732c 202d 2d74 6167 732c  ranches, --tags,
+00002200: 202d 2d72 656d 6f74 6573 2c20 6f72 202d   --remotes, or -
+00002210: 2d67 6c6f 6220 6f70 7469 6f6e 7a0c 2d2d  -glob optionz.--
+00002220: 6461 7465 2d6f 7264 6572 7a6e 5368 6f77  date-orderznShow
+00002230: 206e 6f20 7061 7265 6e74 7320 6265 666f   no parents befo
+00002240: 7265 2061 6c6c 206f 6620 6974 7320 6368  re all of its ch
+00002250: 696c 6472 656e 2061 7265 2073 686f 776e  ildren are shown
+00002260: 2c20 6275 7420 6f74 6865 7277 6973 6520  , but otherwise 
+00002270: 7368 6f77 2063 6f6d 6d69 7473 2069 6e20  show commits in 
+00002280: 7468 6520 636f 6d6d 6974 2074 696d 6573  the commit times
+00002290: 7461 6d70 206f 7264 6572 7a13 2d2d 6175  tamp orderz.--au
+000022a0: 7468 6f72 2d64 6174 652d 6f72 6465 727a  thor-date-orderz
+000022b0: 6e53 686f 7720 6e6f 2070 6172 656e 7473  nShow no parents
+000022c0: 2062 6566 6f72 6520 616c 6c20 6f66 2069   before all of i
+000022d0: 7473 2063 6869 6c64 7265 6e20 6172 6520  ts children are 
+000022e0: 7368 6f77 6e2c 2062 7574 206f 7468 6572  shown, but other
+000022f0: 7769 7365 2073 686f 7720 636f 6d6d 6974  wise show commit
+00002300: 7320 696e 2074 6865 2061 7574 686f 7220  s in the author 
+00002310: 7469 6d65 7374 616d 7020 6f72 6465 727a  timestamp orderz
+00002320: 0c2d 2d74 6f70 6f2d 6f72 6465 727a 7753  .--topo-orderzwS
+00002330: 686f 7720 6e6f 2070 6172 656e 7473 2062  how no parents b
+00002340: 6566 6f72 6520 616c 6c20 6f66 2069 7473  efore all of its
+00002350: 2063 6869 6c64 7265 6e20 6172 6520 7368   children are sh
+00002360: 6f77 6e2c 2061 6e64 2061 766f 6964 2073  own, and avoid s
+00002370: 686f 7769 6e67 2063 6f6d 6d69 7473 206f  howing commits o
+00002380: 6e20 6d75 6c74 6970 6c65 206c 696e 6573  n multiple lines
+00002390: 206f 6620 6869 7374 6f72 7920 696e 7465   of history inte
+000023a0: 726d 6978 6564 7a09 2d2d 7265 7665 7273  rmixedz.--revers
+000023b0: 657a 5e4f 7574 7075 7420 7468 6520 636f  ez^Output the co
+000023c0: 6d6d 6974 7320 6368 6f73 656e 2074 6f20  mmits chosen to 
+000023d0: 6265 2073 686f 776e 2069 6e20 7265 7665  be shown in reve
+000023e0: 7273 6520 6f72 6465 722e 2043 616e 6e6f  rse order. Canno
+000023f0: 7420 6265 2063 6f6d 6269 6e65 6420 7769  t be combined wi
+00002400: 7468 202d 2d77 616c 6b2d 7265 666c 6f67  th --walk-reflog
+00002410: 737a 082d 2d70 7265 7474 797a 0966 6f72  sz.--prettyz.for
+00002420: 6d61 743a 2548 7a3e 5072 6574 7479 2d70  mat:%Hz>Pretty-p
+00002430: 7269 6e74 2074 6865 2063 6f6e 7465 6e74  rint the content
+00002440: 7320 6f66 2074 6865 2063 6f6d 6d69 7420  s of the commit 
+00002450: 6c6f 6773 2069 6e20 6120 6769 7665 6e20  logs in a given 
+00002460: 666f 726d 6174 2903 721c 0000 0072 2c00  format).r....r,.
+00002470: 0000 7206 0000 007a 0f2d 2d61 6262 7265  ..r....z.--abbre
+00002480: 762d 636f 6d6d 6974 7a70 496e 7374 6561  v-commitzpInstea
+00002490: 6420 6f66 2073 686f 7769 6e67 2074 6865  d of showing the
+000024a0: 2066 756c 6c20 3430 2d62 7974 6520 6865   full 40-byte he
+000024b0: 7861 6465 6369 6d61 6c20 636f 6d6d 6974  xadecimal commit
+000024c0: 206f 626a 6563 7420 6e61 6d65 2c20 7368   object name, sh
+000024d0: 6f77 2061 2070 7265 6669 7820 7468 6174  ow a prefix that
+000024e0: 206e 616d 6573 2074 6865 206f 626a 6563   names the objec
+000024f0: 7420 756e 6971 7565 6c79 7a12 2d2d 6e6f  t uniquelyz.--no
+00002500: 2d61 6262 7265 762d 636f 6d6d 6974 2901  -abbrev-commit).
+00002510: 7205 0000 007a 092d 2d6f 6e65 6c69 6e65  r....z.--oneline
+00002520: 7a30 5368 6f72 7468 616e 6420 666f 7220  z0Shorthand for 
+00002530: 222d 2d70 7265 7474 793d 6f6e 656c 696e  "--pretty=onelin
+00002540: 6520 2d2d 6162 6272 6576 2d63 6f6d 6d69  e --abbrev-commi
+00002550: 7422 7a10 2d2d 7368 6f77 2d73 6967 6e61  t"z.--show-signa
+00002560: 7475 7265 7a69 4368 6563 6b20 7468 6520  tureziCheck the 
+00002570: 7661 6c69 6469 7479 206f 6620 6120 7369  validity of a si
+00002580: 676e 6564 2063 6f6d 6d69 7420 6f62 6a65  gned commit obje
+00002590: 6374 2062 7920 7061 7373 696e 6720 7468  ct by passing th
+000025a0: 6520 7369 676e 6174 7572 6520 746f 2067  e signature to g
+000025b0: 7067 202d 2d76 6572 6966 7920 616e 6420  pg --verify and 
+000025c0: 7368 6f77 2074 6865 206f 7574 7075 7472  show the outputr
+000025d0: 0d00 0000 7a57 4f6e 6c79 2074 616b 6573  ....zWOnly takes
+000025e0: 2065 6666 6563 7420 666f 7220 6461 7465   effect for date
+000025f0: 7320 7368 6f77 6e20 696e 2068 756d 616e  s shown in human
+00002600: 2d72 6561 6461 626c 6520 666f 726d 6174  -readable format
+00002610: 2c20 7375 6368 2061 7320 7768 656e 2075  , such as when u
+00002620: 7369 6e67 202d 2d70 7265 7474 7929 0172  sing --pretty).r
+00002630: 0600 0000 7a0f 2d2d 7265 6c61 7469 7665  ....z.--relative
+00002640: 2d64 6174 657a 1b53 796e 6f6e 796d 2066  -datez.Synonym f
+00002650: 6f72 202d 2d64 6174 653d 7265 6c61 7469  or --date=relati
+00002660: 7665 5a0e 7265 7669 7369 6f6e 5f72 616e  veZ.revision_ran
+00002670: 6765 2901 721c 0000 00da 0470 6174 6829  ge).r......path)
+00002680: 0672 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00002690: da03 696e 74da 0861 7267 7061 7273 65da  ..int..argparse.
+000026a0: 0952 454d 4149 4e44 4552 7214 0000 0072  .REMAINDERr....r
+000026b0: 1600 0000 7216 0000 0072 1700 0000 da07  ....r....r......
+000026c0: 6769 745f 6c6f 6798 0000 0073 8601 0000  git_log....s....
+000026d0: 0601 0601 0402 0201 0201 0201 06fd 0405  ................
+000026e0: 0201 0201 0201 06fd 0405 0201 0201 0601  ................
+000026f0: 0201 0201 06fb 0407 0201 0201 0201 0201  ................
+00002700: 06fc 0406 0201 0201 0201 06fd 0405 0201  ................
+00002710: 0201 0201 06fd 0405 0201 0201 0201 06fd  ................
+00002720: 0405 0201 0201 0201 06fd 0405 0201 0201  ................
+00002730: 0201 0201 06fc 0406 0201 0201 0201 06fd  ................
+00002740: 0405 0201 0201 0201 0201 06fc 0406 0201  ................
+00002750: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
+00002760: 06fd 0405 0201 0201 0201 06fd 0405 0201  ................
+00002770: 0201 0201 06fd 0405 0201 0201 0201 06fd  ................
+00002780: 0405 0201 0201 0201 06fd 0405 0201 0201  ................
+00002790: 0201 06fd 0405 0201 0201 0201 0201 06fc  ................
+000027a0: 0406 0201 0201 0201 06fd 0405 0201 0201  ................
+000027b0: 0201 0201 06fc 0406 0201 0201 0201 0201  ................
+000027c0: 06fc 0406 0201 0201 0201 0201 06fc 0406  ................
+000027d0: 0201 0201 0201 06fd 0405 0201 0201 0201  ................
+000027e0: 06fd 0405 0201 0201 0201 06fd 0405 0201  ................
+000027f0: 0201 0201 06fd 0405 0201 0201 0201 06fd  ................
+00002800: 0405 0201 0201 0201 06fd 0405 0201 0201  ................
+00002810: 0201 06fd 0405 0201 0201 0201 0201 06fc  ................
+00002820: 0406 0201 0201 0201 06fd 0e05 0401 0201  ................
+00002830: 0201 0201 06fd 0405 0201 0201 0201 06fd  ................
+00002840: 0405 0201 0201 06fe 0404 0201 0201 0201  ................
+00002850: 06fd 0e06 1401 7235 0000 0063 0000 0000  ......r5...c....
+00002860: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00002870: 4700 0000 734e 0000 0074 006a 0164 0164  G...sN...t.j.d.d
+00002880: 028d 017d 017c 01a0 02a1 007d 0274 037c  ...}.|.....}.t.|
+00002890: 02a0 0464 03a1 0183 0101 0074 057c 02a0  ...d.......t.|..
+000028a0: 0464 04a1 0183 0101 0074 067c 02a0 0464  .d.......t.|...d
+000028b0: 05a1 0183 0101 0074 077c 017c 0064 068d  .......t.|.|.d..
+000028c0: 0201 0064 0053 0029 074e da03 6769 7429  ...d.S.).N..git)
+000028d0: 0172 1100 0000 7219 0000 00da 036c 6f67  .r....r......log
+000028e0: da05 6d65 7267 6529 01da 0863 6c69 5f61  ..merge)...cli_a
+000028f0: 7267 7329 0872 2200 0000 da0e 4172 6775  rgs).r".....Argu
+00002900: 6d65 6e74 5061 7273 6572 da0e 6164 645f  mentParser..add_
+00002910: 7375 6270 6172 7365 7273 7218 0000 00da  subparsersr.....
+00002920: 0a61 6464 5f70 6172 7365 7272 3500 0000  .add_parserr5...
+00002930: 7225 0000 0072 0200 0000 2903 da04 6172  r%...r....)...ar
+00002940: 6773 7215 0000 00da 0a73 7562 7061 7273  gsr......subpars
+00002950: 6572 7372 1600 0000 7216 0000 0072 1700  ersr....r....r..
+00002960: 0000 da04 6d61 696e 6001 0000 730c 0000  ....main`...s...
+00002970: 000c 0108 020e 020e 010e 0110 0272 3f00  .............r?.
+00002980: 0000 2908 7233 0000 0072 2200 0000 da0c  ..).r3...r".....
+00002990: 6172 6770 6172 7365 5f74 7569 7202 0000  argparse_tuir...
+000029a0: 0072 1800 0000 7225 0000 0072 3500 0000  .r....r%...r5...
+000029b0: 723f 0000 0072 1600 0000 7216 0000 0072  r?...r....r....r
+000029c0: 1600 0000 7217 0000 00da 083c 6d6f 6475  ....r......<modu
+000029d0: 6c65 3e01 0000 0073 1000 0000 0800 0802  le>....s........
+000029e0: 0c01 0803 085a 0837 007f 0c49            .....Z.7...I
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/grep.cpython-310.pyc` & `tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/grep.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 07:09:39 2023 UTC, .py size: 3185 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b369 c364 710c 0000  o........i.dq...
+00000000: 6f0d 0d0a 0000 0000 5625 c764 850c 0000  o.......V%.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6500 6a03 6602 6404 6405 8404  ..d.e.j.f.d.d...
 00000050: 5a04 6406 6407 8400 5a05 6401 5300 2908  Z.d.d...Z.d.S.).
 00000060: e900 0000 004e 2901 da0a 696e 766f 6b65  .....N)...invoke
 00000070: 5f74 7569 da06 7265 7475 726e 6300 0000  _tui..returnc...
@@ -124,19 +124,20 @@
 000007b0: 06fc 0406 0201 0201 0201 0201 06fc 0406  ................
 000007c0: 0201 0201 0201 0201 06fc 0c08 0401 0201  ................
 000007d0: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
 000007e0: 0201 06fc 0406 0201 0201 0201 0201 06fc  ................
 000007f0: 0c08 0401 0201 0201 0201 0201 0201 06fb  ................
 00000800: 0407 0201 0201 0201 0201 06fc 0406 0201  ................
 00000810: 0201 0201 0201 06fc 0407 7204 0000 0063  ..........r....c
-00000820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000830: 0200 0000 4300 0000 730e 0000 0074 0074  ....C...s....t.t
-00000840: 0183 0083 0101 0064 0053 0029 014e 2902  .......d.S.).N).
-00000850: 7202 0000 0072 0400 0000 721e 0000 0072  r....r....r....r
-00000860: 1e00 0000 721e 0000 0072 1f00 0000 da04  ....r....r......
-00000870: 6d61 696e 8200 0000 7302 0000 000e 0172  main....s......r
-00000880: 2000 0000 2906 7214 0000 00da 0c61 7267   ...).r......arg
-00000890: 7061 7273 655f 7475 6972 0200 0000 7215  parse_tuir....r.
-000008a0: 0000 0072 0400 0000 7220 0000 0072 1e00  ...r....r ...r..
-000008b0: 0000 721e 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-000008c0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-000008d0: 0800 0000 0800 0c01 1003 0c7d            ...........}
+00000820: 0000 0000 0000 0000 0000 0000 0100 0000  ................
+00000830: 0400 0000 4700 0000 7312 0000 0074 0074  ....G...s....t.t
+00000840: 0183 007c 0064 018d 0201 0064 0053 0029  ...|.d.....d.S.)
+00000850: 024e 2901 da08 636c 695f 6172 6773 2902  .N)...cli_args).
+00000860: 7202 0000 0072 0400 0000 2901 da04 6172  r....r....)...ar
+00000870: 6773 721e 0000 0072 1e00 0000 721f 0000  gsr....r....r...
+00000880: 00da 046d 6169 6e82 0000 0073 0200 0000  ...main....s....
+00000890: 1201 7222 0000 0029 0672 1400 0000 da0c  ..r"...).r......
+000008a0: 6172 6770 6172 7365 5f74 7569 7202 0000  argparse_tuir...
+000008b0: 0072 1500 0000 7204 0000 0072 2200 0000  .r....r....r"...
+000008c0: 721e 0000 0072 1e00 0000 721e 0000 0072  r....r....r....r
+000008d0: 1f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+000008e0: 0000 7308 0000 0008 000c 0110 030c 7d    ..s...........}
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/pastel.cpython-310.pyc` & `tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/pastel.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 07:09:39 2023 UTC, .py size: 14479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,603 +1,594 @@
-00000000: 6f0d 0d0a 0000 0000 b369 c364 8f38 0000  o........i.d.8..
+00000000: 6f0d 0d0a 0000 0000 5625 c764 1a38 0000  o.......V%.d.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 f400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a02 6400 6403 6c03 6d04 5a04 0100 6400  Z.d.d.l.m.Z...d.
-00000050: 6404 6c05 6d06 5a06 0100 6405 6406 8400  d.l.m.Z...d.d...
-00000060: 5a07 6407 6408 8400 5a08 6409 640a 8400  Z.d.d...Z.d.d...
-00000070: 5a09 640b 640c 8400 5a0a 640d 640e 8400  Z.d.d...Z.d.d...
-00000080: 5a0b 640f 6410 8400 5a0c 6411 6412 8400  Z.d.d...Z.d.d...
-00000090: 5a0d 6413 6414 8400 5a0e 6415 6416 8400  Z.d.d...Z.d.d...
-000000a0: 5a0f 6417 6418 8400 5a10 6419 641a 8400  Z.d.d...Z.d.d...
-000000b0: 5a11 641b 641c 8400 5a12 641d 641e 8400  Z.d.d...Z.d.d...
-000000c0: 5a13 641f 6420 8400 5a14 6421 6422 8400  Z.d.d ..Z.d!d"..
-000000d0: 5a15 6423 6424 8400 5a16 6425 6426 8400  Z.d#d$..Z.d%d&..
-000000e0: 5a17 6427 6428 8400 5a18 6429 642a 8400  Z.d'd(..Z.d)d*..
-000000f0: 5a19 642b 642c 8400 5a1a 642d 6506 6501  Z.d+d,..Z.d-e.e.
-00000100: 651b 1900 6502 6a1c 6402 642e 642f 8d02  e...e.j.d.d.d/..
-00000110: 6602 1900 6602 6430 6431 8404 5a1d 6402  f...f.d0d1..Z.d.
-00000120: 5300 2932 e900 0000 0029 01da 084f 7074  S.)2.....)...Opt
-00000130: 696f 6e61 6c4e 2901 da0a 696e 766f 6b65  ionalN)...invoke
-00000140: 5f74 7569 2901 da09 416e 6e6f 7461 7465  _tui)...Annotate
-00000150: 6463 0100 0000 0000 0000 0000 0000 0100  dc..............
-00000160: 0000 0500 0000 4300 0000 f320 0000 0064  ......C.... ...d
-00000170: 017c 005f 0064 027c 005f 017c 006a 0264  .|._.d.|._.|.j.d
-00000180: 0364 0464 0564 068d 0301 0064 0053 0029  .d.d.d.....d.S.)
-00000190: 074e 7a0c 7061 7374 656c 2063 6f6c 6f72  .Nz.pastel color
-000001a0: 7a3a 5368 6f77 2061 6e64 2064 6973 706c  z:Show and displ
-000001b0: 6179 2073 6f6d 6520 696e 666f 726d 6174  ay some informat
-000001c0: 696f 6e20 6162 6f75 7420 7468 6520 6769  ion about the gi
-000001d0: 7665 6e20 636f 6c6f 7228 7329 da05 636f  ven color(s)..co
-000001e0: 6c6f 72fa 012b f5ad 0000 0043 6f6c 6f72  lor..+.....Color
-000001f0: 7320 6361 6e20 6265 2073 7065 6369 6669  s can be specifi
-00000200: 6564 2069 6e20 6d61 6e79 2064 6966 6665  ed in many diffe
-00000210: 7265 6e74 2066 6f72 6d61 7473 2c20 7375  rent formats, su
-00000220: 6368 2061 7320 2352 5247 4742 422c 2052  ch as #RRGGBB, R
-00000230: 5247 4742 422c 2023 5247 422c 2027 7267  RGGBB, #RGB, 'rg
-00000240: 6228 e280 a62c 20e2 80a6 2c20 e280 a629  b(..., ..., ...)
-00000250: 272c 2027 6873 6c28 e280 a62c 20e2 80a6  ', 'hsl(..., ...
-00000260: 2c20 e280 a629 272c 2027 6772 6179 28e2  , ...)', 'gray(.
-00000270: 80a6 2927 206f 7220 7369 6d70 6c79 2062  ..)' or simply b
-00000280: 7920 7468 6520 6e61 6d65 206f 6620 7468  y the name of th
-00000290: 6520 636f 6c6f 722e a902 da05 6e61 7267  e color.....narg
-000002a0: 73da 0468 656c 70a9 03da 0470 726f 67da  s..help....prog.
-000002b0: 0b64 6573 6372 6970 7469 6f6e da0c 6164  .description..ad
-000002c0: 645f 6172 6775 6d65 6e74 a901 da06 7061  d_argument....pa
-000002d0: 7273 6572 a900 7212 0000 00fa 242f 6472  rser..r.....$/dr
-000002e0: 6f6e 652f 7372 632f 7372 632f 7475 6976  one/src/src/tuiv
-000002f0: 6965 772f 636d 642f 7061 7374 656c 2e70  iew/cmd/pastel.p
-00000300: 79da 0c70 6173 7465 6c5f 636f 6c6f 7208  y..pastel_color.
-00000310: 0000 00f3 0e00 0000 0601 0601 0402 0201  ................
-00000320: 0201 0201 0afd 7214 0000 0063 0100 0000  ......r....c....
-00000330: 0000 0000 0000 0000 0100 0000 0800 0000  ................
-00000340: 4300 0000 732a 0000 0064 017c 005f 0064  C...s*...d.|._.d
-00000350: 027c 005f 017c 006a 0264 0364 0464 0564  .|._.|.j.d.d.d.d
-00000360: 0667 0064 07a2 0164 0864 098d 0601 0064  .g.d...d.d.....d
-00000370: 0053 0029 0a4e 7a0b 7061 7374 656c 206c  .S.).Nz.pastel l
-00000380: 6973 747a 2453 686f 7720 6120 6c69 7374  istz$Show a list
-00000390: 206f 6620 6176 6169 6c61 626c 6520 636f   of available co
-000003a0: 6c6f 7220 6e61 6d65 73fa 022d 737a 062d  lor names..-sz.-
-000003b0: 2d73 6f72 74da 0a73 6f72 745f 6f72 6465  -sort..sort_orde
-000003c0: 72da 0368 7565 a905 da0a 6272 6967 6874  r..hue....bright
-000003d0: 6e65 7373 da09 6c75 6d69 6e61 6e63 6572  ness..luminancer
-000003e0: 1800 0000 da06 6368 726f 6d61 da06 7261  ......chroma..ra
-000003f0: 6e64 6f6d 7a0a 536f 7274 206f 7264 6572  ndomz.Sort order
-00000400: a904 da04 6465 7374 da07 6465 6661 756c  ....dest..defaul
-00000410: 74da 0763 686f 6963 6573 720b 0000 0072  t..choicesr....r
-00000420: 0c00 0000 7210 0000 0072 1200 0000 7212  ....r....r....r.
-00000430: 0000 0072 1300 0000 da0b 7061 7374 656c  ...r......pastel
-00000440: 5f6c 6973 7413 0000 0073 1400 0000 0601  _list....s......
-00000450: 0601 0402 0201 0201 0201 0201 0601 0201  ................
-00000460: 0afa 7222 0000 0063 0100 0000 0000 0000  ..r"...c........
-00000470: 0000 0000 0100 0000 0800 0000 4300 0000  ............C...
-00000480: 7340 0000 0064 017c 005f 0064 027c 005f  s@...d.|._.d.|._
-00000490: 017c 006a 0264 0364 0464 0564 0667 0064  .|.j.d.d.d.d.g.d
-000004a0: 07a2 0164 0864 098d 0601 007c 006a 0264  ...d.d.....|.j.d
-000004b0: 0a64 0b64 0c74 0364 0d64 0e64 0f8d 0601  .d.d.t.d.d.d....
-000004c0: 0064 0053 0029 104e 7a0d 7061 7374 656c  .d.S.).Nz.pastel
-000004d0: 2072 616e 646f 6d7a 2047 656e 6572 6174   randomz Generat
-000004e0: 6520 6120 6c69 7374 206f 6620 7261 6e64  e a list of rand
-000004f0: 6f6d 2063 6f6c 6f72 7372 1600 0000 7a0a  om colorsr....z.
-00000500: 2d2d 7374 7261 7465 6779 5a0f 7261 6e64  --strategyZ.rand
-00000510: 6f6d 5f73 7472 6174 6567 79da 0576 6976  om_strategy..viv
-00000520: 6964 2904 7223 0000 00da 0372 6762 da04  id).r#.....rgb..
-00000530: 6772 6179 5a07 6c63 685f 6875 657a 1652  grayZ.lch_huez.R
-00000540: 616e 646f 6d69 7a61 7469 6f6e 2073 7472  andomization str
-00000550: 6174 6567 7972 1e00 0000 fa02 2d6e fa08  ategyr......-n..
-00000560: 2d2d 6e75 6d62 6572 5a0b 636f 6c6f 725f  --numberZ.color_
-00000570: 636f 756e 74e9 0a00 0000 7a1c 4e75 6d62  count.....z.Numb
-00000580: 6572 206f 6620 636f 6c6f 7273 2074 6f20  er of colors to 
-00000590: 6765 6e65 7261 7465 2904 721f 0000 00da  generate).r.....
-000005a0: 0474 7970 6572 2000 0000 720b 0000 00a9  .typer ...r.....
-000005b0: 0472 0d00 0000 720e 0000 0072 0f00 0000  .r....r....r....
-000005c0: da03 696e 7472 1000 0000 7212 0000 0072  ..intr....r....r
-000005d0: 1200 0000 7213 0000 00da 0d70 6173 7465  ....r......paste
-000005e0: 6c5f 7261 6e64 6f6d 2100 0000 7324 0000  l_random!...s$..
-000005f0: 0006 0106 0104 0202 0102 0102 0102 0106  ................
-00000600: 0102 0106 fa04 0802 0102 0102 0102 0102  ................
-00000610: 0102 010a fa72 2c00 0000 6301 0000 0000  .....r,...c.....
-00000620: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
-00000630: 0000 0073 5e00 0000 6401 7c00 5f00 6402  ...s^...d.|._.d.
-00000640: 7c00 5f01 7c00 6a02 6403 7403 6404 6405  |._.|.j.d.t.d.d.
-00000650: 6406 8d04 0100 7c00 6a02 6407 6408 6409  d.....|.j.d.d.d.
-00000660: 640a 8d03 0100 7c00 6a02 640b 640c 640d  d.....|.j.d.d.d.
-00000670: 640e 640f 640e 6702 6410 6411 8d06 0100  d.d.d.g.d.d.....
-00000680: 7c00 6a02 6412 6413 6414 6415 6416 8d04  |.j.d.d.d.d.d...
-00000690: 0100 6400 5300 2917 4e7a 0f70 6173 7465  ..d.S.).Nz.paste
-000006a0: 6c20 6469 7374 696e 6374 7a6f 4765 6e65  l distinctzoGene
-000006b0: 7261 7465 2061 2073 6574 206f 6620 7669  rate a set of vi
-000006c0: 7375 616c 6c79 2064 6973 7469 6e63 7420  sually distinct 
-000006d0: 636f 6c6f 7273 2062 7920 6d61 7869 6d69  colors by maximi
-000006e0: 7a69 6e67 2074 6865 2070 6572 6365 6976  zing the perceiv
-000006f0: 6564 2063 6f6c 6f72 2064 6966 6665 7265  ed color differe
-00000700: 6e63 6520 6265 7477 6565 6e20 7061 6972  nce between pair
-00000710: 7320 6f66 2063 6f6c 6f72 73da 0563 6f75  s of colors..cou
-00000720: 6e74 7228 0000 007a 244e 756d 6265 7220  ntr(...z$Number 
-00000730: 6f66 2064 6973 7469 6e63 7420 636f 6c6f  of distinct colo
-00000740: 7273 2069 6e20 7468 6520 7365 74a9 0372  rs in the set..r
-00000750: 2900 0000 7220 0000 0072 0b00 0000 7206  )...r ...r....r.
-00000760: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00000770: 0000 7a02 2d6d 7a08 2d2d 6d65 7472 6963  ..z.-mz.--metric
-00000780: 5a0f 6469 7374 616e 6365 5f6d 6574 7269  Z.distance_metri
-00000790: 635a 0543 4945 3736 5a09 4349 4544 4532  cZ.CIE76Z.CIEDE2
-000007a0: 3030 307a 3144 6973 7461 6e63 6520 6d65  000z1Distance me
-000007b0: 7472 6963 2074 6f20 636f 6d70 7574 6520  tric to compute 
-000007c0: 6d75 7475 616c 2063 6f6c 6f72 2064 6973  mutual color dis
-000007d0: 7461 6e63 6573 721e 0000 007a 022d 767a  tancesr....z.-vz
-000007e0: 092d 2d76 6572 626f 7365 da0a 7374 6f72  .--verbose..stor
-000007f0: 655f 7472 7565 7a21 5072 696e 7420 7369  e_truez!Print si
-00000800: 6d75 6c61 7469 6f6e 206f 7574 7075 7420  mulation output 
-00000810: 746f 2053 5444 4552 52a9 02da 0661 6374  to STDERR....act
-00000820: 696f 6e72 0b00 0000 722a 0000 0072 1000  ionr....r*...r..
-00000830: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00000840: 00da 0f70 6173 7465 6c5f 6469 7374 696e  ...pastel_distin
-00000850: 6374 3700 0000 7336 0000 0006 0106 0104  ct7...s6........
-00000860: 0202 0102 0102 0102 0106 fc04 0602 0102  ................
-00000870: 0102 0106 fd04 0602 0102 0102 0102 0106  ................
-00000880: 0102 0106 fa04 0802 0102 0102 0102 010a  ................
-00000890: fc72 3200 0000 6301 0000 0000 0000 0000  .r2...c.........
-000008a0: 0000 0001 0000 0007 0000 0043 0000 0073  ...........C...s
-000008b0: 5c00 0000 6401 7c00 5f00 6402 7c00 5f01  \...d.|._.d.|._.
-000008c0: 7c00 6a02 6403 6404 6700 6405 a201 6406  |.j.d.d.g.d...d.
-000008d0: 6407 6408 8d05 0100 7c00 6a02 6409 640a  d.d.....|.j.d.d.
-000008e0: 640b 640c 8d03 0100 7c00 6a02 640d 640e  d.d.....|.j.d.d.
-000008f0: 640f 6410 6411 8d04 0100 7c00 6a02 6412  d.d.d.....|.j.d.
-00000900: 6413 640f 6414 6411 8d04 0100 6400 5300  d.d.d.d.....d.S.
-00000910: 2915 4e7a 0e70 6173 7465 6c20 736f 7274  ).Nz.pastel sort
-00000920: 2d62 797a 2c53 6f72 7420 6120 6c69 7374  -byz,Sort a list
-00000930: 206f 6620 636f 6c6f 7273 2062 7920 7468   of colors by th
-00000940: 6520 6769 7665 6e20 7072 6f70 6572 7479  e given property
-00000950: 2e72 1700 0000 fa01 3f72 1900 0000 7218  .r......?r....r.
-00000960: 0000 007a 1953 6f72 7420 6f72 6465 7220  ...z.Sort order 
-00000970: 5b64 6566 6175 6c74 3a20 6875 655d 2904  [default: hue]).
-00000980: 720a 0000 0072 2100 0000 7220 0000 0072  r....r!...r ...r
-00000990: 0b00 0000 7206 0000 0072 0700 0000 7a41  ....r....r....zA
-000009a0: 436f 6c6f 7273 2074 6f20 736f 7274 2e20  Colors to sort. 
-000009b0: 5573 6520 7661 7269 6f75 7320 666f 726d  Use various form
-000009c0: 6174 7320 2868 6578 2c20 7267 622c 2068  ats (hex, rgb, h
-000009d0: 736c 2c20 6e61 6d65 6420 636f 6c6f 7229  sl, named color)
-000009e0: 2e72 0900 0000 7a02 2d72 7a09 2d2d 7265  .r....z.-rz.--re
-000009f0: 7665 7273 6572 2f00 0000 7a16 5265 7665  verser/...z.Reve
-00000a00: 7273 6520 7468 6520 736f 7274 206f 7264  rse the sort ord
-00000a10: 6572 7230 0000 00fa 022d 757a 082d 2d75  err0.....-uz.--u
-00000a20: 6e69 7175 657a 1752 656d 6f76 6520 6475  niquez.Remove du
-00000a30: 706c 6963 6174 6520 636f 6c6f 7273 720c  plicate colorsr.
-00000a40: 0000 0072 1000 0000 7212 0000 0072 1200  ...r....r....r..
-00000a50: 0000 7213 0000 00da 0e70 6173 7465 6c5f  ..r......pastel_
-00000a60: 736f 7274 5f62 7957 0000 0073 3400 0000  sort_byW...s4...
-00000a70: 0601 0601 0402 0201 0201 0601 0201 0201  ................
-00000a80: 06fb 0407 0201 0201 0201 06fd 0405 0201  ................
-00000a90: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
-00000aa0: 0201 0afc 7235 0000 0063 0100 0000 0000  ....r5...c......
-00000ab0: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
-00000ac0: 0000 734a 0000 0064 017c 005f 0064 027c  ..sJ...d.|._.d.|
-00000ad0: 005f 017c 006a 0264 0367 0064 04a2 0164  ._.|.j.d.g.d...d
-00000ae0: 0564 0664 0764 088d 0501 007c 006a 0264  .d.d.d.....|.j.d
-00000af0: 0964 0a64 0b64 0c8d 0301 007c 006a 0264  .d.d.d.....|.j.d
-00000b00: 0d64 0e74 0364 0f64 108d 0401 0064 0053  .d.t.d.d.....d.S
-00000b10: 0029 114e 7a0d 7061 7374 656c 2066 6f72  .).Nz.pastel for
-00000b20: 6d61 747a 3043 6f6e 7665 7274 2074 6865  matz0Convert the
-00000b30: 2067 6976 656e 2063 6f6c 6f72 2873 2920   given color(s) 
-00000b40: 746f 2061 2073 7065 6369 6669 6320 666f  to a specific fo
-00000b50: 726d 6174 2e72 2900 0000 2916 7224 0000  rmat.r)...).r$..
-00000b60: 007a 0972 6762 2d66 6c6f 6174 da03 6865  .z.rgb-float..he
-00000b70: 78da 0368 736c fa07 6873 6c2d 6875 65fa  x..hsl..hsl-hue.
-00000b80: 0e68 736c 2d73 6174 7572 6174 696f 6efa  .hsl-saturation.
-00000b90: 0d68 736c 2d6c 6967 6874 6e65 7373 5a03  .hsl-lightnessZ.
-00000ba0: 6c63 687a 0d6c 6368 2d6c 6967 6874 6e65  lchz.lch-lightne
-00000bb0: 7373 7a0a 6c63 682d 6368 726f 6d61 7a07  ssz.lch-chromaz.
-00000bc0: 6c63 682d 6875 65da 036c 6162 fa05 6c61  lch-hue..lab..la
-00000bd0: 622d 61fa 056c 6162 2d62 721b 0000 0072  b-a..lab-br....r
-00000be0: 1a00 0000 7a09 616e 7369 2d38 6269 747a  ....z.ansi-8bitz
-00000bf0: 0a61 6e73 692d 3234 6269 747a 1461 6e73  .ansi-24bitz.ans
-00000c00: 692d 3862 6974 2d65 7363 6170 6563 6f64  i-8bit-escapecod
-00000c10: 657a 1561 6e73 692d 3234 6269 742d 6573  ez.ansi-24bit-es
-00000c20: 6361 7065 636f 6465 5a04 636d 796b da04  capecodeZ.cmyk..
-00000c30: 6e61 6d65 7233 0000 0072 3600 0000 7a13  namer3...r6...z.
-00000c40: 4f75 7470 7574 2066 6f72 6d61 7420 7479  Output format ty
-00000c50: 7065 2e29 0472 2100 0000 720a 0000 0072  pe.).r!...r....r
-00000c60: 2000 0000 720b 0000 0072 0600 0000 7207   ...r....r....r.
-00000c70: 0000 007a 2a43 6f6c 6f72 7320 746f 2063  ...z*Colors to c
-00000c80: 6f6e 7665 7274 2074 6f20 7468 6520 7370  onvert to the sp
-00000c90: 6563 6966 6965 6420 666f 726d 6174 2e72  ecified format.r
-00000ca0: 0900 0000 7226 0000 00da 014e 7a1d 4e75  ....r&.....Nz.Nu
-00000cb0: 6d62 6572 206f 6620 636f 6c6f 7273 2074  mber of colors t
-00000cc0: 6f20 6765 6e65 7261 7465 2e29 03da 076d  o generate.)...m
-00000cd0: 6574 6176 6172 7229 0000 0072 0b00 0000  etavarr)...r....
-00000ce0: 722a 0000 0072 1000 0000 7212 0000 0072  r*...r....r....r
-00000cf0: 1200 0000 7213 0000 00da 0d70 6173 7465  ....r......paste
-00000d00: 6c5f 666f 726d 6174 7500 0000 7328 0000  l_formatu...s(..
-00000d10: 0006 0106 0104 0202 0106 0102 1802 0102  ................
-00000d20: 0106 e404 2002 0102 0102 0106 fd04 0702  .... ...........
-00000d30: 0102 0102 0102 010a fc72 4100 0000 6301  .........rA...c.
-00000d40: 0000 0000 0000 0000 0000 0001 0000 0006  ................
-00000d50: 0000 0043 0000 0073 8800 0000 6401 7c00  ...C...s....d.|.
-00000d60: 5f00 6402 7c00 5f01 7c00 6a02 6403 6404  _.d.|._.|.j.d.d.
-00000d70: 6405 8d02 0100 7c00 6a02 6406 6407 6408  d.....|.j.d.d.d.
-00000d80: 6409 8d03 0100 7c00 6a02 640a 640b 640c  d.....|.j.d.d.d.
-00000d90: 640d 640e 8d04 0100 7c00 6a02 640f 6410  d.d.....|.j.d.d.
-00000da0: 6411 6412 6413 8d04 0100 7c00 6a02 6414  d.d.d.....|.j.d.
-00000db0: 6415 6411 6416 6413 8d04 0100 7c00 6a02  d.d.d.d.....|.j.
-00000dc0: 6417 6418 6411 6419 6413 8d04 0100 7c00  d.d.d.d.d.....|.
-00000dd0: 6a02 641a 641b 6411 641c 6413 8d04 0100  j.d.d.d.d.d.....
-00000de0: 6400 5300 291d 4e7a 0c70 6173 7465 6c20  d.S.).Nz.pastel 
-00000df0: 7061 696e 747a 2e50 7269 6e74 2063 6f6c  paintz.Print col
-00000e00: 6f72 6564 2074 6578 7420 7573 696e 6720  ored text using 
-00000e10: 414e 5349 2065 7363 6170 6520 7365 7175  ANSI escape sequ
-00000e20: 656e 6365 7372 0600 0000 7a15 5468 6520  encesr....z.The 
-00000e30: 666f 7265 6772 6f75 6e64 2063 6f6c 6f72  foreground color
-00000e40: 2ea9 0172 0b00 0000 da04 7465 7874 7207  ...r......textr.
-00000e50: 0000 007a 2054 6865 2074 6578 7420 746f  ...z The text to
-00000e60: 2062 6520 7072 696e 7465 6420 696e 2063   be printed in c
-00000e70: 6f6c 6f72 2e72 0900 0000 7a02 2d6f 7a04  olor.r....z.-oz.
-00000e80: 2d2d 6f6e 7a08 6267 2d63 6f6c 6f72 7a22  --onz.bg-colorz"
-00000e90: 5573 6520 7468 6520 7370 6563 6966 6965  Use the specifie
-00000ea0: 6420 6261 636b 6772 6f75 6e64 2063 6f6c  d background col
-00000eb0: 6f72 2902 7240 0000 0072 0b00 0000 7a02  or).r@...r....z.
-00000ec0: 2d62 7a06 2d2d 626f 6c64 722f 0000 007a  -bz.--boldr/...z
-00000ed0: 1b50 7269 6e74 2074 6865 2074 6578 7420  .Print the text 
-00000ee0: 696e 2062 6f6c 6420 6661 6365 7230 0000  in bold facer0..
-00000ef0: 007a 022d 697a 082d 2d69 7461 6c69 637a  .z.-iz.--italicz
-00000f00: 1d50 7269 6e74 2074 6865 2074 6578 7420  .Print the text 
-00000f10: 696e 2069 7461 6c69 6320 666f 6e74 7234  in italic fontr4
-00000f20: 0000 007a 0b2d 2d75 6e64 6572 6c69 6e65  ...z.--underline
-00000f30: 7a1a 4472 6177 2061 206c 696e 6520 6265  z.Draw a line be
-00000f40: 6c6f 7720 7468 6520 7465 7874 7226 0000  low the textr&..
-00000f50: 007a 0c2d 2d6e 6f2d 6e65 776c 696e 657a  .z.--no-newlinez
-00000f60: 2944 6f20 6e6f 7420 7072 696e 7420 6120  )Do not print a 
-00000f70: 7472 6169 6c69 6e67 206e 6577 6c69 6e65  trailing newline
-00000f80: 2063 6861 7261 6374 6572 720c 0000 0072   characterr....r
-00000f90: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00000fa0: 0000 00da 0c70 6173 7465 6c5f 7061 696e  .....pastel_pain
-00000fb0: 74a8 0000 0073 5200 0000 0601 0601 0403  t....sR.........
-00000fc0: 0201 0201 06fe 0404 0201 0201 0201 06fd  ................
-00000fd0: 0407 0201 0201 0201 0201 06fc 0406 0201  ................
-00000fe0: 0201 0201 0201 06fc 0406 0201 0201 0201  ................
-00000ff0: 0201 06fc 0406 0201 0201 0201 0201 06fc  ................
-00001000: 0406 0201 0201 0201 0201 0afc 7244 0000  ............rD..
-00001010: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
-00001020: 0000 0700 0000 4300 0000 734c 0000 0064  ......C...sL...d
-00001030: 017c 005f 0064 027c 005f 017c 006a 0264  .|._.d.|._.|.j.d
-00001040: 0364 0464 0564 068d 0301 007c 006a 0264  .d.d.d.....|.j.d
-00001050: 0764 0874 0364 0964 0a64 0b8d 0501 007c  .d.t.d.d.d.....|
-00001060: 006a 0264 0c64 0d67 0064 0ea2 0164 0f64  .j.d.d.g.d...d.d
-00001070: 1064 118d 0501 0064 0053 0029 124e 7a0f  .d.....d.S.).Nz.
-00001080: 7061 7374 656c 2067 7261 6469 656e 747a  pastel gradientz
-00001090: 4d47 656e 6572 6174 6520 6120 7365 7175  MGenerate a sequ
-000010a0: 656e 6365 206f 6620 636f 6c6f 7273 2074  ence of colors t
-000010b0: 6861 7420 696e 7465 7270 6f6c 6174 6573  hat interpolates
-000010c0: 2062 6574 7765 656e 2074 6865 2073 7065   between the spe
-000010d0: 6369 6669 6564 2063 6f6c 6f72 732e 7206  cified colors.r.
-000010e0: 0000 0072 0700 0000 7a21 436f 6c6f 7220  ...r....z!Color 
-000010f0: 7374 6f70 7320 696e 2074 6865 2063 6f6c  stops in the col
-00001100: 6f72 2067 7261 6469 656e 7472 0900 0000  or gradientr....
-00001110: 7226 0000 0072 2700 0000 7228 0000 007a  r&...r'...r(...z
-00001120: 2a4e 756d 6265 7220 6f66 2063 6f6c 6f72  *Number of color
-00001130: 7320 746f 2067 656e 6572 6174 6520 5b64  s to generate [d
-00001140: 6566 6175 6c74 3a20 3130 5d72 2e00 0000  efault: 10]r....
-00001150: 7216 0000 00fa 0c2d 2d63 6f6c 6f72 7370  r......--colorsp
-00001160: 6163 65a9 04da 034c 6162 5a03 4c43 68da  ace....LabZ.LCh.
-00001170: 0352 4742 da03 4853 4c72 4700 0000 7a35  .RGB..HSLrG...z5
-00001180: 5468 6520 636f 6c6f 7273 7061 6365 2069  The colorspace i
-00001190: 6e20 7768 6963 6820 746f 2069 6e74 6572  n which to inter
-000011a0: 706f 6c61 7465 205b 6465 6661 756c 743a  polate [default:
-000011b0: 204c 6162 5da9 0372 2100 0000 7220 0000   Lab]..r!...r ..
-000011c0: 0072 0b00 0000 722a 0000 0072 1000 0000  .r....r*...r....
-000011d0: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-000011e0: 0f70 6173 7465 6c5f 6772 6164 6965 6e74  .pastel_gradient
-000011f0: d800 0000 7324 0000 0006 0102 0204 ff10  ....s$..........
-00001200: 0404 0102 0102 0102 0102 0102 0106 fb04  ................
-00001210: 0702 0102 0106 0102 0102 010a fb72 4b00  .............rK.
-00001220: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00001230: 0000 0007 0000 0043 0000 0073 5a00 0000  .......C...sZ...
-00001240: 6401 7c00 5f00 6402 7c00 5f01 7c00 6a02  d.|._.d.|._.|.j.
-00001250: 6403 6404 6405 8d02 0100 7c00 6a02 6406  d.d.d.....|.j.d.
-00001260: 6407 6408 6409 8d03 0100 7c00 6a02 640a  d.d.d.....|.j.d.
-00001270: 640b 6700 640c a201 640d 640e 640f 8d05  d.g.d...d.d.d...
-00001280: 0100 7c00 6a02 6410 6411 7403 6412 6413  ..|.j.d.d.t.d.d.
-00001290: 6414 8d05 0100 6400 5300 2915 4e7a 0a70  d.....d.S.).Nz.p
-000012a0: 6173 7465 6c20 6d69 787a 4d43 7265 6174  astel mixzMCreat
-000012b0: 6520 6e65 7720 636f 6c6f 7273 2062 7920  e new colors by 
-000012c0: 696e 7465 7270 6f6c 6174 696e 6720 6265  interpolating be
-000012d0: 7477 6565 6e20 7477 6f20 636f 6c6f 7273  tween two colors
-000012e0: 2069 6e20 7468 6520 6769 7665 6e20 636f   in the given co
-000012f0: 6c6f 7273 7061 6365 7206 0000 007a 3854  lorspacer....z8T
-00001300: 6865 2062 6173 6520 636f 6c6f 7220 7768  he base color wh
-00001310: 6963 6820 7769 6c6c 2062 6520 6d69 7865  ich will be mixe
-00001320: 6420 7769 7468 2074 6865 206f 7468 6572  d with the other
-00001330: 2063 6f6c 6f72 7372 4200 0000 5a0c 6f74   colorsrB...Z.ot
-00001340: 6865 725f 636f 6c6f 7273 7207 0000 0072  her_colorsr....r
-00001350: 0800 0000 7209 0000 0072 1600 0000 7245  ....r....r....rE
-00001360: 0000 0072 4600 0000 7247 0000 007a 2654  ...rF...rG...z&T
-00001370: 6865 2063 6f6c 6f72 7370 6163 6520 696e  he colorspace in
-00001380: 2077 6869 6368 2074 6f20 696e 7465 7270   which to interp
-00001390: 6f6c 6174 6572 4a00 0000 7a02 2d66 7a0a  olaterJ...z.-fz.
-000013a0: 2d2d 6672 6163 7469 6f6e 6700 0000 0000  --fractiong.....
-000013b0: 00e0 3f7a 5154 6865 206e 756d 6265 7220  ..?zQThe number 
-000013c0: 6265 7477 6565 6e20 302e 3020 616e 6420  between 0.0 and 
-000013d0: 312e 3020 6465 7465 726d 696e 696e 6720  1.0 determining 
-000013e0: 686f 7720 6d75 6368 2074 6f20 6d69 7820  how much to mix 
-000013f0: 696e 2066 726f 6d20 7468 6520 6261 7365  in from the base
-00001400: 2063 6f6c 6f72 722e 0000 00a9 0472 0d00   colorr......r..
-00001410: 0000 720e 0000 0072 0f00 0000 da05 666c  ..r....r......fl
-00001420: 6f61 7472 1000 0000 7212 0000 0072 1200  oatr....r....r..
-00001430: 0000 7213 0000 00da 0a70 6173 7465 6c5f  ..r......pastel_
-00001440: 6d69 78ef 0000 0073 3400 0000 0601 0202  mix....s4.......
-00001450: 04ff 0404 0201 0201 06fe 0404 0201 0201  ................
-00001460: 0201 06fd 0405 0201 0201 0601 0201 0201  ................
-00001470: 06fb 0407 0201 0201 0201 0201 0201 0afb  ................
-00001480: 724e 0000 0063 0100 0000 0000 0000 0000  rN...c..........
-00001490: 0000 0100 0000 0500 0000 4300 0000 7334  ..........C...s4
-000014a0: 0000 0064 017c 005f 0064 027c 005f 017c  ...d.|._.d.|._.|
-000014b0: 006a 0264 0367 0064 04a2 0164 0564 068d  .j.d.g.d...d.d..
-000014c0: 0301 007c 006a 0264 0764 0864 0964 0a8d  ...|.j.d.d.d.d..
-000014d0: 0301 0064 0053 0029 0b4e 7a11 7061 7374  ...d.S.).Nz.past
-000014e0: 656c 2063 6f6c 6f72 626c 696e 647a 6543  el colorblindzeC
-000014f0: 6f6e 7665 7274 2074 6865 2067 6976 656e  onvert the given
-00001500: 2063 6f6c 6f72 2074 6f20 686f 7720 6974   color to how it
-00001510: 2077 6f75 6c64 206c 6f6f 6b20 746f 2061   would look to a
-00001520: 2070 6572 736f 6e20 7769 7468 2070 726f   person with pro
-00001530: 7461 6e6f 7069 612c 2064 6575 7465 7261  tanopia, deutera
-00001540: 6e6f 7069 612c 206f 7220 7472 6974 616e  nopia, or tritan
-00001550: 6f70 6961 7229 0000 0029 035a 0470 726f  opiar)...).Z.pro
-00001560: 745a 0664 6575 7465 725a 0474 7269 747a  tZ.deuterZ.tritz
-00001570: 5a54 6865 2074 7970 6520 6f66 2063 6f6c  ZThe type of col
-00001580: 6f72 626c 696e 646e 6573 7320 7468 6174  orblindness that
-00001590: 2073 686f 756c 6420 6265 2073 696d 756c   should be simul
-000015a0: 6174 6564 2028 7072 6f74 616e 6f70 6961  ated (protanopia
-000015b0: 2c20 6465 7574 6572 616e 6f70 6961 2c20  , deuteranopia, 
-000015c0: 7472 6974 616e 6f70 6961 29a9 0272 2100  tritanopia)..r!.
-000015d0: 0000 720b 0000 0072 0600 0000 7207 0000  ..r....r....r...
-000015e0: 0072 0800 0000 7209 0000 0072 0c00 0000  .r....r....r....
-000015f0: 7210 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00001600: 1300 0000 da11 7061 7374 656c 5f63 6f6c  ......pastel_col
-00001610: 6f72 626c 696e 640e 0100 0073 1800 0000  orblind....s....
-00001620: 0601 0601 0402 0201 0601 0201 06fd 0405  ................
-00001630: 0201 0201 0201 0afd 7250 0000 0063 0100  ........rP...c..
-00001640: 0000 0000 0000 0000 0000 0100 0000 0500  ................
-00001650: 0000 4300 0000 7342 0000 0064 017c 005f  ..C...sB...d.|._
-00001660: 0064 027c 005f 017c 006a 0264 0367 0064  .d.|._.|.j.d.g.d
-00001670: 04a2 0164 0564 068d 0301 007c 006a 0264  ...d.d.....|.j.d
-00001680: 0764 0864 098d 0201 007c 006a 0264 0a64  .d.d.....|.j.d.d
-00001690: 0b64 0c64 0d8d 0301 0064 0053 0029 0e4e  .d.d.....d.S.).N
-000016a0: 7a0a 7061 7374 656c 2073 6574 7a2a 5365  z.pastel setz*Se
-000016b0: 7420 7468 6520 6769 7665 6e20 7072 6f70  t the given prop
-000016c0: 6572 7479 2074 6f20 6120 7370 6563 6966  erty to a specif
-000016d0: 6963 2076 616c 7565 da08 7072 6f70 6572  ic value..proper
-000016e0: 7479 290b da09 6c69 6768 746e 6573 7372  ty)...lightnessr
-000016f0: 1800 0000 721c 0000 0072 3c00 0000 723d  ....r....r<...r=
-00001700: 0000 00da 0372 6564 da05 6772 6565 6eda  .....red..green.
-00001710: 0462 6c75 6572 3800 0000 7239 0000 0072  .bluer8...r9...r
-00001720: 3a00 0000 7a23 5468 6520 7072 6f70 6572  :...z#The proper
-00001730: 7479 2074 6861 7420 7368 6f75 6c64 2062  ty that should b
-00001740: 6520 6368 616e 6765 6472 4f00 0000 da05  e changedrO.....
-00001750: 7661 6c75 657a 2754 6865 206e 6577 206e  valuez'The new n
-00001760: 756d 6572 6963 616c 2076 616c 7565 206f  umerical value o
-00001770: 6620 7468 6520 7072 6f70 6572 7479 7242  f the propertyrB
-00001780: 0000 0072 0600 0000 7207 0000 0072 0800  ...r....r....r..
-00001790: 0000 7209 0000 0072 0c00 0000 7210 0000  ..r....r....r...
-000017a0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000017b0: da0a 7061 7374 656c 5f73 6574 1e01 0000  ..pastel_set....
-000017c0: 731a 0000 0006 0106 0104 0202 0106 0102  s...............
-000017d0: 0d06 f10e 1104 0102 0102 0102 010a fd72  ...............r
-000017e0: 5700 0000 6301 0000 0000 0000 0000 0000  W...c...........
-000017f0: 0001 0000 0005 0000 0043 0000 00f3 3000  .........C....0.
-00001800: 0000 6401 7c00 5f00 6402 7c00 5f01 7c00  ..d.|._.d.|._.|.
-00001810: 6a02 6403 7403 6404 6405 8d03 0100 7c00  j.d.t.d.d.....|.
-00001820: 6a02 6406 6407 6408 6409 8d03 0100 6400  j.d.d.d.d.....d.
-00001830: 5300 290a 4e7a 0f70 6173 7465 6c20 7361  S.).Nz.pastel sa
-00001840: 7475 7261 7465 7a5c 496e 6372 6561 7365  turatez\Increase
-00001850: 2074 6865 2073 6174 7572 6174 696f 6e20   the saturation 
-00001860: 6f66 2061 2063 6f6c 6f72 2062 7920 6164  of a color by ad
-00001870: 6469 6e67 2061 2063 6572 7461 696e 2061  ding a certain a
-00001880: 6d6f 756e 7420 746f 2074 6865 2048 534c  mount to the HSL
-00001890: 2073 6174 7572 6174 696f 6e20 6368 616e   saturation chan
-000018a0: 6e65 6c2e da06 616d 6f75 6e74 fa38 416d  nel...amount.8Am
-000018b0: 6f75 6e74 206f 6620 7361 7475 7261 7469  ount of saturati
-000018c0: 6f6e 2074 6f20 6164 6420 286e 756d 6265  on to add (numbe
-000018d0: 7220 6265 7477 6565 6e20 302e 3020 616e  r between 0.0 an
-000018e0: 6420 312e 3029 a902 7229 0000 0072 0b00  d 1.0)..r)...r..
-000018f0: 0000 7206 0000 0072 0700 0000 7208 0000  ..r....r....r...
-00001900: 0072 0900 0000 724c 0000 0072 1000 0000  .r....rL...r....
-00001910: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00001920: 0f70 6173 7465 6c5f 7361 7475 7261 7465  .pastel_saturate
-00001930: 3b01 0000 f318 0000 0006 0106 0104 0202  ;...............
-00001940: 0102 0102 0106 fd04 0502 0102 0102 010a  ................
-00001950: fd72 5c00 0000 6301 0000 0000 0000 0000  .r\...c.........
-00001960: 0000 0001 0000 0005 0000 0043 0000 0072  ...........C...r
-00001970: 5800 0000 290a 4e7a 1170 6173 7465 6c20  X...).Nz.pastel 
-00001980: 6465 7361 7475 7261 7465 7a63 4465 6372  desaturatezcDecr
-00001990: 6561 7365 2074 6865 2073 6174 7572 6174  ease the saturat
-000019a0: 696f 6e20 6f66 2061 2063 6f6c 6f72 2062  ion of a color b
-000019b0: 7920 7375 6274 7261 6374 696e 6720 6120  y subtracting a 
-000019c0: 6365 7274 6169 6e20 616d 6f75 6e74 2066  certain amount f
-000019d0: 726f 6d20 7468 6520 4853 4c20 7361 7475  rom the HSL satu
-000019e0: 7261 7469 6f6e 2063 6861 6e6e 656c 2e72  ration channel.r
-000019f0: 5900 0000 725a 0000 0072 5b00 0000 7206  Y...rZ...r[...r.
-00001a00: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00001a10: 0000 724c 0000 0072 1000 0000 7212 0000  ..rL...r....r...
-00001a20: 0072 1200 0000 7213 0000 00da 1170 6173  .r....r......pas
-00001a30: 7465 6c5f 6465 7361 7475 7261 7465 4b01  tel_desaturateK.
-00001a40: 0000 725d 0000 0072 5e00 0000 6301 0000  ..r]...r^...c...
-00001a50: 0000 0000 0000 0000 0001 0000 0005 0000  ................
-00001a60: 0043 0000 0072 5800 0000 290a 4e7a 0e70  .C...rX...).Nz.p
-00001a70: 6173 7465 6c20 6c69 6768 7465 6e7a 484c  astel lightenzHL
-00001a80: 6967 6874 656e 2061 2063 6f6c 6f72 2062  ighten a color b
-00001a90: 7920 6164 6469 6e67 2061 2063 6572 7461  y adding a certa
-00001aa0: 696e 2061 6d6f 756e 7420 746f 2074 6865  in amount to the
-00001ab0: 2048 534c 206c 6967 6874 6e65 7373 2063   HSL lightness c
-00001ac0: 6861 6e6e 656c 2e72 5900 0000 725a 0000  hannel.rY...rZ..
-00001ad0: 0072 5b00 0000 7206 0000 0072 0700 0000  .r[...r....r....
-00001ae0: 7208 0000 0072 0900 0000 724c 0000 0072  r....r....rL...r
-00001af0: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001b00: 0000 00da 0e70 6173 7465 6c5f 6c69 6768  .....pastel_ligh
-00001b10: 7465 6e5b 0100 00f3 1a00 0000 0601 0202  ten[............
-00001b20: 04ff 0404 0201 0201 0201 06fd 0405 0201  ................
-00001b30: 0201 0201 0afd 725f 0000 0063 0100 0000  ......r_...c....
-00001b40: 0000 0000 0000 0000 0100 0000 0500 0000  ................
-00001b50: 4300 0000 7258 0000 0029 0a4e 7a0d 7061  C...rX...).Nz.pa
-00001b60: 7374 656c 2064 6172 6b65 6e7a 4a44 6172  stel darkenzJDar
-00001b70: 6b65 6e20 6120 636f 6c6f 7220 6279 2073  ken a color by s
-00001b80: 7562 7472 6163 7469 6e67 2061 2063 6572  ubtracting a cer
-00001b90: 7461 696e 2061 6d6f 756e 7420 6672 6f6d  tain amount from
-00001ba0: 2074 6865 206c 6967 6874 6e65 7373 2063   the lightness c
-00001bb0: 6861 6e6e 656c 2e72 5900 0000 725a 0000  hannel.rY...rZ..
-00001bc0: 0072 5b00 0000 7206 0000 0072 0700 0000  .r[...r....r....
-00001bd0: 7208 0000 0072 0900 0000 724c 0000 0072  r....r....rL...r
-00001be0: 1000 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001bf0: 0000 00da 0d70 6173 7465 6c5f 6461 726b  .....pastel_dark
-00001c00: 656e 6d01 0000 7260 0000 0072 6100 0000  enm...r`...ra...
-00001c10: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001c20: 0005 0000 0043 0000 0072 5800 0000 290a  .....C...rX...).
-00001c30: 4e7a 0d70 6173 7465 6c20 726f 7461 7465  Nz.pastel rotate
-00001c40: 75b2 0000 0052 6f74 6174 6520 7468 6520  u....Rotate the 
-00001c50: 4853 4c20 6875 6520 6368 616e 6e65 6c20  HSL hue channel 
-00001c60: 6f66 2061 2063 6f6c 6f72 2062 7920 7468  of a color by th
-00001c70: 6520 7370 6563 6966 6965 6420 616e 676c  e specified angl
-00001c80: 6520 2869 6e20 6465 6772 6565 7329 2e20  e (in degrees). 
-00001c90: 4120 726f 7461 7469 6f6e 2062 7920 3138  A rotation by 18
-00001ca0: 30c2 b020 7265 7475 726e 7320 7468 6520  0.. returns the 
-00001cb0: 636f 6d70 6c65 6d65 6e74 6172 7920 636f  complementary co
-00001cc0: 6c6f 722e 2041 2072 6f74 6174 696f 6e20  lor. A rotation 
-00001cd0: 6279 2033 3630 c2b0 2072 6574 7572 6e73  by 360.. returns
-00001ce0: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
-00001cf0: 2063 6f6c 6f72 2eda 0764 6567 7265 6573   color...degrees
-00001d00: 7a36 616e 676c 6520 6279 2077 6869 6368  z6angle by which
-00001d10: 2074 6f20 726f 7461 7465 2028 696e 2064   to rotate (in d
-00001d20: 6567 7265 6573 2c20 6361 6e20 6265 206e  egrees, can be n
-00001d30: 6567 6174 6976 6529 725b 0000 0072 0600  egative)r[...r..
-00001d40: 0000 7207 0000 0072 0800 0000 7209 0000  ..r....r....r...
-00001d50: 0072 4c00 0000 7210 0000 0072 1200 0000  .rL...r....r....
-00001d60: 7212 0000 0072 1300 0000 da0d 7061 7374  r....r......past
-00001d70: 656c 5f72 6f74 6174 657f 0100 0072 5d00  el_rotate....r].
-00001d80: 0000 7263 0000 0063 0100 0000 0000 0000  ..rc...c........
-00001d90: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00001da0: 7205 0000 0029 074e 7a11 7061 7374 656c  r....).Nz.pastel
-00001db0: 2063 6f6d 706c 656d 656e 7475 4900 0000   complementuI...
-00001dc0: 436f 6d70 7574 6520 7468 6520 636f 6d70  Compute the comp
-00001dd0: 6c65 6d65 6e74 6172 7920 636f 6c6f 7220  lementary color 
-00001de0: 6279 2072 6f74 6174 696e 6720 7468 6520  by rotating the 
-00001df0: 4853 4c20 6875 6520 6368 616e 6e65 6c20  HSL hue channel 
-00001e00: 6279 2031 3830 c2b0 2e72 0600 0000 7207  by 180...r....r.
-00001e10: 0000 0072 0800 0000 7209 0000 0072 0c00  ...r....r....r..
-00001e20: 0000 7210 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00001e30: 0072 1300 0000 da11 7061 7374 656c 5f63  .r......pastel_c
-00001e40: 6f6d 706c 656d 656e 748f 0100 00f3 1000  omplement.......
-00001e50: 0000 0601 0202 04ff 0404 0201 0201 0201  ................
-00001e60: 0afd 7264 0000 0063 0100 0000 0000 0000  ..rd...c........
-00001e70: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
-00001e80: 7320 0000 0064 017c 005f 0064 027c 005f  s ...d.|._.d.|._
-00001e90: 017c 006a 0264 0374 0364 0464 058d 0301  .|.j.d.t.d.d....
-00001ea0: 0064 0053 0029 064e 7a0b 7061 7374 656c  .d.S.).Nz.pastel
-00001eb0: 2067 7261 797a 3043 7265 6174 6520 6120   grayz0Create a 
-00001ec0: 6772 6179 2074 6f6e 6520 6672 6f6d 2061  gray tone from a
-00001ed0: 2067 6976 656e 206c 6967 6874 6e65 7373   given lightness
-00001ee0: 2076 616c 7565 2e72 5200 0000 7a3f 4c69   value.rR...z?Li
-00001ef0: 6768 746e 6573 7320 6f66 2074 6865 2063  ghtness of the c
-00001f00: 7265 6174 6564 2067 7261 7920 746f 6e65  reated gray tone
-00001f10: 2028 6e75 6d62 6572 2062 6574 7765 656e   (number between
-00001f20: 2030 2e30 2061 6e64 2031 2e30 2972 5b00   0.0 and 1.0)r[.
-00001f30: 0000 724c 0000 0072 1000 0000 7212 0000  ..rL...r....r...
-00001f40: 0072 1200 0000 7213 0000 00da 0b70 6173  .r....r......pas
-00001f50: 7465 6c5f 6772 6179 9c01 0000 7215 0000  tel_gray....r...
-00001f60: 0072 6600 0000 6301 0000 0000 0000 0000  .rf...c.........
-00001f70: 0000 0001 0000 0005 0000 0043 0000 0072  ...........C...r
-00001f80: 0500 0000 2907 4e7a 0e70 6173 7465 6c20  ....).Nz.pastel 
-00001f90: 746f 2d67 7261 797a 4543 6f6d 706c 6574  to-grayzEComplet
-00001fa0: 656c 7920 6465 7361 7475 7261 7465 2074  ely desaturate t
-00001fb0: 6865 2067 6976 656e 2063 6f6c 6f72 2077  he given color w
-00001fc0: 6869 6c65 2070 7265 7365 7276 696e 6720  hile preserving 
-00001fd0: 7468 6520 6c75 6d69 6e61 6e63 652e 7206  the luminance.r.
-00001fe0: 0000 0072 0700 0000 7208 0000 0072 0900  ...r....r....r..
-00001ff0: 0000 720c 0000 0072 1000 0000 7212 0000  ..r....r....r...
-00002000: 0072 1200 0000 7213 0000 00da 0e70 6173  .r....r......pas
-00002010: 7465 6c5f 746f 5f67 7261 79a7 0100 0072  tel_to_gray....r
-00002020: 6500 0000 7267 0000 0063 0100 0000 0000  e...rg...c......
-00002030: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
-00002040: 0000 7205 0000 0029 074e 7a10 7061 7374  ..r....).Nz.past
-00002050: 656c 2074 6578 7463 6f6c 6f72 7ac2 5265  el textcolorz.Re
-00002060: 7475 726e 2061 2072 6561 6461 626c 6520  turn a readable 
-00002070: 666f 7265 6772 6f75 6e64 2074 6578 7420  foreground text 
-00002080: 636f 6c6f 7220 2865 6974 6865 7220 626c  color (either bl
-00002090: 6163 6b20 6f72 2077 6869 7465 2920 666f  ack or white) fo
-000020a0: 7220 6120 6769 7665 6e20 6261 636b 6772  r a given backgr
-000020b0: 6f75 6e64 2063 6f6c 6f72 2e20 5468 6973  ound color. This
-000020c0: 2063 616e 2061 6c73 6f20 6265 2075 7365   can also be use
-000020d0: 6420 696e 2074 6865 206f 7070 6f73 6974  d in the opposit
-000020e0: 6520 7761 792c 2069 2e65 2e20 746f 2063  e way, i.e. to c
-000020f0: 7265 6174 6520 6120 6261 636b 6772 6f75  reate a backgrou
-00002100: 6e64 2063 6f6c 6f72 2066 6f72 2061 2067  nd color for a g
-00002110: 6976 656e 2074 6578 7420 636f 6c6f 722e  iven text color.
-00002120: 7206 0000 0072 0700 0000 7208 0000 0072  r....r....r....r
-00002130: 0900 0000 720c 0000 0072 1000 0000 7212  ....r....r....r.
-00002140: 0000 0072 1200 0000 7213 0000 00da 1070  ...r....r......p
-00002150: 6173 7465 6c5f 7465 7874 636f 6c6f 72b4  astel_textcolor.
-00002160: 0100 0072 1500 0000 7268 0000 00da 0363  ...r....rh.....c
-00002170: 6d64 5429 01da 0370 6f73 6301 0000 0000  mdT)...posc.....
-00002180: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00002190: 0000 0073 3c01 0000 7400 6a01 6401 6402  ...s<...t.j.d.d.
-000021a0: 8d01 7d01 7c01 a002 a100 7d02 7403 7c02  ..}.|.....}.t.|.
-000021b0: a004 6403 a101 8301 0100 7405 7c02 a004  ..d.......t.|...
-000021c0: 6404 a101 8301 0100 7406 7c02 a004 6405  d.......t.|...d.
-000021d0: a101 8301 0100 7407 7c02 a004 6406 a101  ......t.|...d...
-000021e0: 8301 0100 7408 7c02 a004 6407 a101 8301  ....t.|...d.....
-000021f0: 0100 7409 7c02 a004 6408 a101 8301 0100  ..t.|...d.......
-00002200: 740a 7c02 a004 6409 a101 8301 0100 740b  t.|...d.......t.
-00002210: 7c02 a004 640a a101 8301 0100 740c 7c02  |...d.......t.|.
-00002220: a004 640b a101 8301 0100 740d 7c02 a004  ..d.......t.|...
-00002230: 640c a101 8301 0100 740e 7c02 a004 640d  d.......t.|...d.
-00002240: a101 8301 0100 740f 7c02 a004 640e a101  ......t.|...d...
-00002250: 8301 0100 7410 7c02 a004 640f a101 8301  ....t.|...d.....
-00002260: 0100 7411 7c02 a004 6410 a101 8301 0100  ..t.|...d.......
-00002270: 7412 7c02 a004 6411 a101 8301 0100 7413  t.|...d.......t.
-00002280: 7c02 a004 6412 a101 8301 0100 7414 7c02  |...d.......t.|.
-00002290: a004 6413 a101 8301 0100 7415 7c02 a004  ..d.......t.|...
-000022a0: 6414 a101 8301 0100 7416 7c02 a004 6415  d.......t.|...d.
-000022b0: a101 8301 0100 7417 7c02 a004 6416 a101  ......t.|...d...
-000022c0: 8301 0100 7418 7c01 7c00 6417 8d02 0100  ....t.|.|.d.....
-000022d0: 6400 5300 2918 4e5a 0670 6173 7465 6c29  d.S.).NZ.pastel)
-000022e0: 0172 0d00 0000 7206 0000 00da 046c 6973  .r....r......lis
-000022f0: 7472 1d00 0000 5a08 6469 7374 696e 6374  tr....Z.distinct
-00002300: 7a07 736f 7274 2d62 79da 0666 6f72 6d61  z.sort-by..forma
-00002310: 745a 0570 6169 6e74 5a08 6772 6164 6965  tZ.paintZ.gradie
-00002320: 6e74 5a03 6d69 785a 0a63 6f6c 6f72 626c  ntZ.mixZ.colorbl
-00002330: 696e 64da 0373 6574 5a08 7361 7475 7261  ind..setZ.satura
-00002340: 7465 5a0a 6465 7361 7475 7261 7465 da07  teZ.desaturate..
-00002350: 6c69 6768 7465 6eda 0664 6172 6b65 6eda  lighten..darken.
-00002360: 0672 6f74 6174 655a 0a63 6f6d 706c 656d  .rotateZ.complem
-00002370: 656e 7472 2500 0000 7a07 746f 2d67 7261  entr%...z.to-gra
-00002380: 795a 0974 6578 7463 6f6c 6f72 2901 da0e  yZ.textcolor)...
-00002390: 636f 6d6d 616e 645f 6669 6c74 6572 2919  command_filter).
-000023a0: da04 7961 7078 da0e 4172 6775 6d65 6e74  ..yapx..Argument
-000023b0: 5061 7273 6572 da0e 6164 645f 7375 6270  Parser..add_subp
-000023c0: 6172 7365 7273 7214 0000 00da 0a61 6464  arsersr......add
-000023d0: 5f70 6172 7365 7272 2200 0000 722c 0000  _parserr"...r,..
-000023e0: 0072 3200 0000 7235 0000 0072 4100 0000  .r2...r5...rA...
-000023f0: 7244 0000 0072 4b00 0000 724e 0000 0072  rD...rK...rN...r
-00002400: 5000 0000 7257 0000 0072 5c00 0000 725e  P...rW...r\...r^
-00002410: 0000 0072 5f00 0000 7261 0000 0072 6300  ...r_...ra...rc.
-00002420: 0000 7264 0000 0072 6600 0000 7267 0000  ..rd...rf...rg..
-00002430: 0072 6800 0000 7203 0000 0029 0372 6900  .rh...r....).ri.
-00002440: 0000 7211 0000 00da 0a73 7562 7061 7273  ..r......subpars
-00002450: 6572 7372 1200 0000 7212 0000 0072 1300  ersr....r....r..
-00002460: 0000 da04 6d61 696e bf01 0000 732e 0000  ....main....s...
-00002470: 000c 0108 020e 020e 010e 010e 010e 010e  ................
-00002480: 010e 010e 010e 010e 010e 010e 010e 010e  ................
-00002490: 010e 010e 010e 010e 010e 010e 0110 0272  ...............r
-000024a0: 7700 0000 291e da06 7479 7069 6e67 7202  w...)...typingr.
-000024b0: 0000 0072 7200 0000 da0c 6172 6770 6172  ...rr.....argpar
-000024c0: 7365 5f74 7569 7203 0000 00da 0a79 6170  se_tuir......yap
-000024d0: 782e 7479 7065 7372 0400 0000 7214 0000  x.typesr....r...
-000024e0: 0072 2200 0000 722c 0000 0072 3200 0000  .r"...r,...r2...
-000024f0: 7235 0000 0072 4100 0000 7244 0000 0072  r5...rA...rD...r
-00002500: 4b00 0000 724e 0000 0072 5000 0000 7257  K...rN...rP...rW
-00002510: 0000 0072 5c00 0000 725e 0000 0072 5f00  ...r\...r^...r_.
-00002520: 0000 7261 0000 0072 6300 0000 7264 0000  ..ra...rc...rd..
-00002530: 0072 6600 0000 7267 0000 0072 6800 0000  .rf...rg...rh...
-00002540: da03 7374 72da 0361 7267 7277 0000 0072  ..str..argrw...r
-00002550: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00002560: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00002570: 0073 3200 0000 0c00 0802 0c01 0c01 0803  .s2.............
-00002580: 080b 080e 0816 0820 081e 0833 0830 0817  ....... ...3.0..
-00002590: 081f 0810 081d 0810 0810 0812 0812 0810  ................
-000025a0: 080d 080b 080d 280b                      ......(.
+00000020: 0002 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
+00000040: 0100 6403 6404 8400 5a03 6405 6406 8400  ..d.d...Z.d.d...
+00000050: 5a04 6407 6408 8400 5a05 6409 640a 8400  Z.d.d...Z.d.d...
+00000060: 5a06 640b 640c 8400 5a07 640d 640e 8400  Z.d.d...Z.d.d...
+00000070: 5a08 640f 6410 8400 5a09 6411 6412 8400  Z.d.d...Z.d.d...
+00000080: 5a0a 6413 6414 8400 5a0b 6415 6416 8400  Z.d.d...Z.d.d...
+00000090: 5a0c 6417 6418 8400 5a0d 6419 641a 8400  Z.d.d...Z.d.d...
+000000a0: 5a0e 641b 641c 8400 5a0f 641d 641e 8400  Z.d.d...Z.d.d...
+000000b0: 5a10 641f 6420 8400 5a11 6421 6422 8400  Z.d.d ..Z.d!d"..
+000000c0: 5a12 6423 6424 8400 5a13 6425 6426 8400  Z.d#d$..Z.d%d&..
+000000d0: 5a14 6427 6428 8400 5a15 6429 642a 8400  Z.d'd(..Z.d)d*..
+000000e0: 5a16 642b 642c 8400 5a17 6401 5300 292d  Z.d+d,..Z.d.S.)-
+000000f0: e900 0000 004e 2901 da0a 696e 766f 6b65  .....N)...invoke
+00000100: 5f74 7569 6301 0000 0000 0000 0000 0000  _tuic...........
+00000110: 0001 0000 0005 0000 0043 0000 00f3 2000  .........C.... .
+00000120: 0000 6401 7c00 5f00 6402 7c00 5f01 7c00  ..d.|._.d.|._.|.
+00000130: 6a02 6403 6404 6405 6406 8d03 0100 6400  j.d.d.d.d.....d.
+00000140: 5300 2907 4e7a 0c70 6173 7465 6c20 636f  S.).Nz.pastel co
+00000150: 6c6f 727a 3a53 686f 7720 616e 6420 6469  lorz:Show and di
+00000160: 7370 6c61 7920 736f 6d65 2069 6e66 6f72  splay some infor
+00000170: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+00000180: 2067 6976 656e 2063 6f6c 6f72 2873 29da   given color(s).
+00000190: 0563 6f6c 6f72 fa01 2bf5 ad00 0000 436f  .color..+.....Co
+000001a0: 6c6f 7273 2063 616e 2062 6520 7370 6563  lors can be spec
+000001b0: 6966 6965 6420 696e 206d 616e 7920 6469  ified in many di
+000001c0: 6666 6572 656e 7420 666f 726d 6174 732c  fferent formats,
+000001d0: 2073 7563 6820 6173 2023 5252 4747 4242   such as #RRGGBB
+000001e0: 2c20 5252 4747 4242 2c20 2352 4742 2c20  , RRGGBB, #RGB, 
+000001f0: 2772 6762 28e2 80a6 2c20 e280 a62c 20e2  'rgb(..., ..., .
+00000200: 80a6 2927 2c20 2768 736c 28e2 80a6 2c20  ..)', 'hsl(..., 
+00000210: e280 a62c 20e2 80a6 2927 2c20 2767 7261  ..., ...)', 'gra
+00000220: 7928 e280 a629 2720 6f72 2073 696d 706c  y(...)' or simpl
+00000230: 7920 6279 2074 6865 206e 616d 6520 6f66  y by the name of
+00000240: 2074 6865 2063 6f6c 6f72 2ea9 02da 056e   the color.....n
+00000250: 6172 6773 da04 6865 6c70 a903 da04 7072  args..help....pr
+00000260: 6f67 da0b 6465 7363 7269 7074 696f 6eda  og..description.
+00000270: 0c61 6464 5f61 7267 756d 656e 74a9 01da  .add_argument...
+00000280: 0670 6172 7365 72a9 0072 1000 0000 fa24  .parser..r.....$
+00000290: 2f64 726f 6e65 2f73 7263 2f73 7263 2f74  /drone/src/src/t
+000002a0: 7569 7669 6577 2f63 6d64 2f70 6173 7465  uiview/cmd/paste
+000002b0: 6c2e 7079 da0c 7061 7374 656c 5f63 6f6c  l.py..pastel_col
+000002c0: 6f72 0500 0000 f30e 0000 0006 0106 0104  or..............
+000002d0: 0202 0102 0102 010a fd72 1200 0000 6301  .........r....c.
+000002e0: 0000 0000 0000 0000 0000 0001 0000 0008  ................
+000002f0: 0000 0043 0000 0073 2a00 0000 6401 7c00  ...C...s*...d.|.
+00000300: 5f00 6402 7c00 5f01 7c00 6a02 6403 6404  _.d.|._.|.j.d.d.
+00000310: 6405 6406 6700 6407 a201 6408 6409 8d06  d.d.g.d...d.d...
+00000320: 0100 6400 5300 290a 4e7a 0b70 6173 7465  ..d.S.).Nz.paste
+00000330: 6c20 6c69 7374 7a24 5368 6f77 2061 206c  l listz$Show a l
+00000340: 6973 7420 6f66 2061 7661 696c 6162 6c65  ist of available
+00000350: 2063 6f6c 6f72 206e 616d 6573 fa02 2d73   color names..-s
+00000360: 7a06 2d2d 736f 7274 da0a 736f 7274 5f6f  z.--sort..sort_o
+00000370: 7264 6572 da03 6875 65a9 05da 0a62 7269  rder..hue....bri
+00000380: 6768 746e 6573 73da 096c 756d 696e 616e  ghtness..luminan
+00000390: 6365 7216 0000 00da 0663 6872 6f6d 61da  cer......chroma.
+000003a0: 0672 616e 646f 6d7a 0a53 6f72 7420 6f72  .randomz.Sort or
+000003b0: 6465 72a9 04da 0464 6573 74da 0764 6566  der....dest..def
+000003c0: 6175 6c74 da07 6368 6f69 6365 7372 0900  ault..choicesr..
+000003d0: 0000 720a 0000 0072 0e00 0000 7210 0000  ..r....r....r...
+000003e0: 0072 1000 0000 7211 0000 00da 0b70 6173  .r....r......pas
+000003f0: 7465 6c5f 6c69 7374 1000 0000 7314 0000  tel_list....s...
+00000400: 0006 0106 0104 0202 0102 0102 0102 0106  ................
+00000410: 0102 010a fa72 2000 0000 6301 0000 0000  .....r ...c.....
+00000420: 0000 0000 0000 0001 0000 0008 0000 0043  ...............C
+00000430: 0000 0073 4000 0000 6401 7c00 5f00 6402  ...s@...d.|._.d.
+00000440: 7c00 5f01 7c00 6a02 6403 6404 6405 6406  |._.|.j.d.d.d.d.
+00000450: 6700 6407 a201 6408 6409 8d06 0100 7c00  g.d...d.d.....|.
+00000460: 6a02 640a 640b 640c 7403 640d 640e 640f  j.d.d.d.t.d.d.d.
+00000470: 8d06 0100 6400 5300 2910 4e7a 0d70 6173  ....d.S.).Nz.pas
+00000480: 7465 6c20 7261 6e64 6f6d 7a20 4765 6e65  tel randomz Gene
+00000490: 7261 7465 2061 206c 6973 7420 6f66 2072  rate a list of r
+000004a0: 616e 646f 6d20 636f 6c6f 7273 7214 0000  andom colorsr...
+000004b0: 007a 0a2d 2d73 7472 6174 6567 795a 0f72  .z.--strategyZ.r
+000004c0: 616e 646f 6d5f 7374 7261 7465 6779 da05  andom_strategy..
+000004d0: 7669 7669 6429 0472 2100 0000 da03 7267  vivid).r!.....rg
+000004e0: 62da 0467 7261 795a 076c 6368 5f68 7565  b..grayZ.lch_hue
+000004f0: 7a16 5261 6e64 6f6d 697a 6174 696f 6e20  z.Randomization 
+00000500: 7374 7261 7465 6779 721c 0000 00fa 022d  strategyr......-
+00000510: 6efa 082d 2d6e 756d 6265 725a 0b63 6f6c  n..--numberZ.col
+00000520: 6f72 5f63 6f75 6e74 e90a 0000 007a 1c4e  or_count.....z.N
+00000530: 756d 6265 7220 6f66 2063 6f6c 6f72 7320  umber of colors 
+00000540: 746f 2067 656e 6572 6174 6529 0472 1d00  to generate).r..
+00000550: 0000 da04 7479 7065 721e 0000 0072 0900  ....typer....r..
+00000560: 0000 a904 720b 0000 0072 0c00 0000 720d  ....r....r....r.
+00000570: 0000 00da 0369 6e74 720e 0000 0072 1000  .....intr....r..
+00000580: 0000 7210 0000 0072 1100 0000 da0d 7061  ..r....r......pa
+00000590: 7374 656c 5f72 616e 646f 6d1e 0000 0073  stel_random....s
+000005a0: 2400 0000 0601 0601 0402 0201 0201 0201  $...............
+000005b0: 0201 0601 0201 06fa 0408 0201 0201 0201  ................
+000005c0: 0201 0201 0201 0afa 722a 0000 0063 0100  ........r*...c..
+000005d0: 0000 0000 0000 0000 0000 0100 0000 0800  ................
+000005e0: 0000 4300 0000 735e 0000 0064 017c 005f  ..C...s^...d.|._
+000005f0: 0064 027c 005f 017c 006a 0264 0374 0364  .d.|._.|.j.d.t.d
+00000600: 0464 0564 068d 0401 007c 006a 0264 0764  .d.d.....|.j.d.d
+00000610: 0864 0964 0a8d 0301 007c 006a 0264 0b64  .d.d.....|.j.d.d
+00000620: 0c64 0d64 0e64 0f64 0e67 0264 1064 118d  .d.d.d.d.g.d.d..
+00000630: 0601 007c 006a 0264 1264 1364 1464 1564  ...|.j.d.d.d.d.d
+00000640: 168d 0401 0064 0053 0029 174e 7a0f 7061  .....d.S.).Nz.pa
+00000650: 7374 656c 2064 6973 7469 6e63 747a 6f47  stel distinctzoG
+00000660: 656e 6572 6174 6520 6120 7365 7420 6f66  enerate a set of
+00000670: 2076 6973 7561 6c6c 7920 6469 7374 696e   visually distin
+00000680: 6374 2063 6f6c 6f72 7320 6279 206d 6178  ct colors by max
+00000690: 696d 697a 696e 6720 7468 6520 7065 7263  imizing the perc
+000006a0: 6569 7665 6420 636f 6c6f 7220 6469 6666  eived color diff
+000006b0: 6572 656e 6365 2062 6574 7765 656e 2070  erence between p
+000006c0: 6169 7273 206f 6620 636f 6c6f 7273 da05  airs of colors..
+000006d0: 636f 756e 7472 2600 0000 7a24 4e75 6d62  countr&...z$Numb
+000006e0: 6572 206f 6620 6469 7374 696e 6374 2063  er of distinct c
+000006f0: 6f6c 6f72 7320 696e 2074 6865 2073 6574  olors in the set
+00000700: a903 7227 0000 0072 1e00 0000 7209 0000  ..r'...r....r...
+00000710: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00000720: 7207 0000 007a 022d 6d7a 082d 2d6d 6574  r....z.-mz.--met
+00000730: 7269 635a 0f64 6973 7461 6e63 655f 6d65  ricZ.distance_me
+00000740: 7472 6963 5a05 4349 4537 365a 0943 4945  tricZ.CIE76Z.CIE
+00000750: 4445 3230 3030 7a31 4469 7374 616e 6365  DE2000z1Distance
+00000760: 206d 6574 7269 6320 746f 2063 6f6d 7075   metric to compu
+00000770: 7465 206d 7574 7561 6c20 636f 6c6f 7220  te mutual color 
+00000780: 6469 7374 616e 6365 7372 1c00 0000 7a02  distancesr....z.
+00000790: 2d76 7a09 2d2d 7665 7262 6f73 65da 0a73  -vz.--verbose..s
+000007a0: 746f 7265 5f74 7275 657a 2150 7269 6e74  tore_truez!Print
+000007b0: 2073 696d 756c 6174 696f 6e20 6f75 7470   simulation outp
+000007c0: 7574 2074 6f20 5354 4445 5252 a902 da06  ut to STDERR....
+000007d0: 6163 7469 6f6e 7209 0000 0072 2800 0000  actionr....r(...
+000007e0: 720e 0000 0072 1000 0000 7210 0000 0072  r....r....r....r
+000007f0: 1100 0000 da0f 7061 7374 656c 5f64 6973  ......pastel_dis
+00000800: 7469 6e63 7434 0000 0073 3600 0000 0601  tinct4...s6.....
+00000810: 0601 0402 0201 0201 0201 0201 06fc 0406  ................
+00000820: 0201 0201 0201 06fd 0406 0201 0201 0201  ................
+00000830: 0201 0601 0201 06fa 0408 0201 0201 0201  ................
+00000840: 0201 0afc 7230 0000 0063 0100 0000 0000  ....r0...c......
+00000850: 0000 0000 0000 0100 0000 0700 0000 4300  ..............C.
+00000860: 0000 735c 0000 0064 017c 005f 0064 027c  ..s\...d.|._.d.|
+00000870: 005f 017c 006a 0264 0364 0467 0064 05a2  ._.|.j.d.d.g.d..
+00000880: 0164 0664 0764 088d 0501 007c 006a 0264  .d.d.d.....|.j.d
+00000890: 0964 0a64 0b64 0c8d 0301 007c 006a 0264  .d.d.d.....|.j.d
+000008a0: 0d64 0e64 0f64 1064 118d 0401 007c 006a  .d.d.d.d.....|.j
+000008b0: 0264 1264 1364 0f64 1464 118d 0401 0064  .d.d.d.d.d.....d
+000008c0: 0053 0029 154e 7a0e 7061 7374 656c 2073  .S.).Nz.pastel s
+000008d0: 6f72 742d 6279 7a2c 536f 7274 2061 206c  ort-byz,Sort a l
+000008e0: 6973 7420 6f66 2063 6f6c 6f72 7320 6279  ist of colors by
+000008f0: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
+00000900: 7274 792e 7215 0000 00fa 013f 7217 0000  rty.r......?r...
+00000910: 0072 1600 0000 7a19 536f 7274 206f 7264  .r....z.Sort ord
+00000920: 6572 205b 6465 6661 756c 743a 2068 7565  er [default: hue
+00000930: 5d29 0472 0800 0000 721f 0000 0072 1e00  ]).r....r....r..
+00000940: 0000 7209 0000 0072 0400 0000 7205 0000  ..r....r....r...
+00000950: 007a 4143 6f6c 6f72 7320 746f 2073 6f72  .zAColors to sor
+00000960: 742e 2055 7365 2076 6172 696f 7573 2066  t. Use various f
+00000970: 6f72 6d61 7473 2028 6865 782c 2072 6762  ormats (hex, rgb
+00000980: 2c20 6873 6c2c 206e 616d 6564 2063 6f6c  , hsl, named col
+00000990: 6f72 292e 7207 0000 007a 022d 727a 092d  or).r....z.-rz.-
+000009a0: 2d72 6576 6572 7365 722d 0000 007a 1652  -reverser-...z.R
+000009b0: 6576 6572 7365 2074 6865 2073 6f72 7420  everse the sort 
+000009c0: 6f72 6465 7272 2e00 0000 fa02 2d75 7a08  orderr......-uz.
+000009d0: 2d2d 756e 6971 7565 7a17 5265 6d6f 7665  --uniquez.Remove
+000009e0: 2064 7570 6c69 6361 7465 2063 6f6c 6f72   duplicate color
+000009f0: 7372 0a00 0000 720e 0000 0072 1000 0000  sr....r....r....
+00000a00: 7210 0000 0072 1100 0000 da0e 7061 7374  r....r......past
+00000a10: 656c 5f73 6f72 745f 6279 5400 0000 7334  el_sort_byT...s4
+00000a20: 0000 0006 0106 0104 0202 0102 0106 0102  ................
+00000a30: 0102 0106 fb04 0702 0102 0102 0106 fd04  ................
+00000a40: 0502 0102 0102 0102 0106 fc04 0602 0102  ................
+00000a50: 0102 0102 010a fc72 3300 0000 6301 0000  .......r3...c...
+00000a60: 0000 0000 0000 0000 0001 0000 0007 0000  ................
+00000a70: 0043 0000 0073 4a00 0000 6401 7c00 5f00  .C...sJ...d.|._.
+00000a80: 6402 7c00 5f01 7c00 6a02 6403 6700 6404  d.|._.|.j.d.g.d.
+00000a90: a201 6405 6406 6407 6408 8d05 0100 7c00  ..d.d.d.d.....|.
+00000aa0: 6a02 6409 640a 640b 640c 8d03 0100 7c00  j.d.d.d.d.....|.
+00000ab0: 6a02 640d 640e 7403 640f 6410 8d04 0100  j.d.d.t.d.d.....
+00000ac0: 6400 5300 2911 4e7a 0d70 6173 7465 6c20  d.S.).Nz.pastel 
+00000ad0: 666f 726d 6174 7a30 436f 6e76 6572 7420  formatz0Convert 
+00000ae0: 7468 6520 6769 7665 6e20 636f 6c6f 7228  the given color(
+00000af0: 7329 2074 6f20 6120 7370 6563 6966 6963  s) to a specific
+00000b00: 2066 6f72 6d61 742e 7227 0000 0029 1672   format.r'...).r
+00000b10: 2200 0000 7a09 7267 622d 666c 6f61 74da  "...z.rgb-float.
+00000b20: 0368 6578 da03 6873 6cfa 0768 736c 2d68  .hex..hsl..hsl-h
+00000b30: 7565 fa0e 6873 6c2d 7361 7475 7261 7469  ue..hsl-saturati
+00000b40: 6f6e fa0d 6873 6c2d 6c69 6768 746e 6573  on..hsl-lightnes
+00000b50: 735a 036c 6368 7a0d 6c63 682d 6c69 6768  sZ.lchz.lch-ligh
+00000b60: 746e 6573 737a 0a6c 6368 2d63 6872 6f6d  tnessz.lch-chrom
+00000b70: 617a 076c 6368 2d68 7565 da03 6c61 62fa  az.lch-hue..lab.
+00000b80: 056c 6162 2d61 fa05 6c61 622d 6272 1900  .lab-a..lab-br..
+00000b90: 0000 7218 0000 007a 0961 6e73 692d 3862  ..r....z.ansi-8b
+00000ba0: 6974 7a0a 616e 7369 2d32 3462 6974 7a14  itz.ansi-24bitz.
+00000bb0: 616e 7369 2d38 6269 742d 6573 6361 7065  ansi-8bit-escape
+00000bc0: 636f 6465 7a15 616e 7369 2d32 3462 6974  codez.ansi-24bit
+00000bd0: 2d65 7363 6170 6563 6f64 655a 0463 6d79  -escapecodeZ.cmy
+00000be0: 6bda 046e 616d 6572 3100 0000 7234 0000  k..namer1...r4..
+00000bf0: 007a 134f 7574 7075 7420 666f 726d 6174  .z.Output format
+00000c00: 2074 7970 652e 2904 721f 0000 0072 0800   type.).r....r..
+00000c10: 0000 721e 0000 0072 0900 0000 7204 0000  ..r....r....r...
+00000c20: 0072 0500 0000 7a2a 436f 6c6f 7273 2074  .r....z*Colors t
+00000c30: 6f20 636f 6e76 6572 7420 746f 2074 6865  o convert to the
+00000c40: 2073 7065 6369 6669 6564 2066 6f72 6d61   specified forma
+00000c50: 742e 7207 0000 0072 2400 0000 da01 4e7a  t.r....r$.....Nz
+00000c60: 1d4e 756d 6265 7220 6f66 2063 6f6c 6f72  .Number of color
+00000c70: 7320 746f 2067 656e 6572 6174 652e 2903  s to generate.).
+00000c80: da07 6d65 7461 7661 7272 2700 0000 7209  ..metavarr'...r.
+00000c90: 0000 0072 2800 0000 720e 0000 0072 1000  ...r(...r....r..
+00000ca0: 0000 7210 0000 0072 1100 0000 da0d 7061  ..r....r......pa
+00000cb0: 7374 656c 5f66 6f72 6d61 7472 0000 0073  stel_formatr...s
+00000cc0: 2800 0000 0601 0601 0402 0201 0601 0218  (...............
+00000cd0: 0201 0201 06e4 0420 0201 0201 0201 06fd  ....... ........
+00000ce0: 0407 0201 0201 0201 0201 0afc 723f 0000  ............r?..
+00000cf0: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000d00: 0000 0600 0000 4300 0000 7388 0000 0064  ......C...s....d
+00000d10: 017c 005f 0064 027c 005f 017c 006a 0264  .|._.d.|._.|.j.d
+00000d20: 0364 0464 058d 0201 007c 006a 0264 0664  .d.d.....|.j.d.d
+00000d30: 0764 0864 098d 0301 007c 006a 0264 0a64  .d.d.....|.j.d.d
+00000d40: 0b64 0c64 0d64 0e8d 0401 007c 006a 0264  .d.d.d.....|.j.d
+00000d50: 0f64 1064 1164 1264 138d 0401 007c 006a  .d.d.d.d.....|.j
+00000d60: 0264 1464 1564 1164 1664 138d 0401 007c  .d.d.d.d.d.....|
+00000d70: 006a 0264 1764 1864 1164 1964 138d 0401  .j.d.d.d.d.d....
+00000d80: 007c 006a 0264 1a64 1b64 1164 1c64 138d  .|.j.d.d.d.d.d..
+00000d90: 0401 0064 0053 0029 1d4e 7a0c 7061 7374  ...d.S.).Nz.past
+00000da0: 656c 2070 6169 6e74 7a2e 5072 696e 7420  el paintz.Print 
+00000db0: 636f 6c6f 7265 6420 7465 7874 2075 7369  colored text usi
+00000dc0: 6e67 2041 4e53 4920 6573 6361 7065 2073  ng ANSI escape s
+00000dd0: 6571 7565 6e63 6573 7204 0000 007a 1554  equencesr....z.T
+00000de0: 6865 2066 6f72 6567 726f 756e 6420 636f  he foreground co
+00000df0: 6c6f 722e a901 7209 0000 00da 0474 6578  lor...r......tex
+00000e00: 7472 0500 0000 7a20 5468 6520 7465 7874  tr....z The text
+00000e10: 2074 6f20 6265 2070 7269 6e74 6564 2069   to be printed i
+00000e20: 6e20 636f 6c6f 722e 7207 0000 007a 022d  n color.r....z.-
+00000e30: 6f7a 042d 2d6f 6e7a 0862 672d 636f 6c6f  oz.--onz.bg-colo
+00000e40: 727a 2255 7365 2074 6865 2073 7065 6369  rz"Use the speci
+00000e50: 6669 6564 2062 6163 6b67 726f 756e 6420  fied background 
+00000e60: 636f 6c6f 7229 0272 3e00 0000 7209 0000  color).r>...r...
+00000e70: 007a 022d 627a 062d 2d62 6f6c 6472 2d00  .z.-bz.--boldr-.
+00000e80: 0000 7a1b 5072 696e 7420 7468 6520 7465  ..z.Print the te
+00000e90: 7874 2069 6e20 626f 6c64 2066 6163 6572  xt in bold facer
+00000ea0: 2e00 0000 7a02 2d69 7a08 2d2d 6974 616c  ....z.-iz.--ital
+00000eb0: 6963 7a1d 5072 696e 7420 7468 6520 7465  icz.Print the te
+00000ec0: 7874 2069 6e20 6974 616c 6963 2066 6f6e  xt in italic fon
+00000ed0: 7472 3200 0000 7a0b 2d2d 756e 6465 726c  tr2...z.--underl
+00000ee0: 696e 657a 1a44 7261 7720 6120 6c69 6e65  inez.Draw a line
+00000ef0: 2062 656c 6f77 2074 6865 2074 6578 7472   below the textr
+00000f00: 2400 0000 7a0c 2d2d 6e6f 2d6e 6577 6c69  $...z.--no-newli
+00000f10: 6e65 7a29 446f 206e 6f74 2070 7269 6e74  nez)Do not print
+00000f20: 2061 2074 7261 696c 696e 6720 6e65 776c   a trailing newl
+00000f30: 696e 6520 6368 6172 6163 7465 7272 0a00  ine characterr..
+00000f40: 0000 720e 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00000f50: 0072 1100 0000 da0c 7061 7374 656c 5f70  .r......pastel_p
+00000f60: 6169 6e74 a500 0000 7352 0000 0006 0106  aint....sR......
+00000f70: 0104 0302 0102 0106 fe04 0402 0102 0102  ................
+00000f80: 0106 fd04 0702 0102 0102 0102 0106 fc04  ................
+00000f90: 0602 0102 0102 0102 0106 fc04 0602 0102  ................
+00000fa0: 0102 0102 0106 fc04 0602 0102 0102 0102  ................
+00000fb0: 0106 fc04 0602 0102 0102 0102 010a fc72  ...............r
+00000fc0: 4200 0000 6301 0000 0000 0000 0000 0000  B...c...........
+00000fd0: 0001 0000 0007 0000 0043 0000 0073 4c00  .........C...sL.
+00000fe0: 0000 6401 7c00 5f00 6402 7c00 5f01 7c00  ..d.|._.d.|._.|.
+00000ff0: 6a02 6403 6404 6405 6406 8d03 0100 7c00  j.d.d.d.d.....|.
+00001000: 6a02 6407 6408 7403 6409 640a 640b 8d05  j.d.d.t.d.d.d...
+00001010: 0100 7c00 6a02 640c 640d 6700 640e a201  ..|.j.d.d.g.d...
+00001020: 640f 6410 6411 8d05 0100 6400 5300 2912  d.d.d.....d.S.).
+00001030: 4e7a 0f70 6173 7465 6c20 6772 6164 6965  Nz.pastel gradie
+00001040: 6e74 7a4d 4765 6e65 7261 7465 2061 2073  ntzMGenerate a s
+00001050: 6571 7565 6e63 6520 6f66 2063 6f6c 6f72  equence of color
+00001060: 7320 7468 6174 2069 6e74 6572 706f 6c61  s that interpola
+00001070: 7465 7320 6265 7477 6565 6e20 7468 6520  tes between the 
+00001080: 7370 6563 6966 6965 6420 636f 6c6f 7273  specified colors
+00001090: 2e72 0400 0000 7205 0000 007a 2143 6f6c  .r....r....z!Col
+000010a0: 6f72 2073 746f 7073 2069 6e20 7468 6520  or stops in the 
+000010b0: 636f 6c6f 7220 6772 6164 6965 6e74 7207  color gradientr.
+000010c0: 0000 0072 2400 0000 7225 0000 0072 2600  ...r$...r%...r&.
+000010d0: 0000 7a2a 4e75 6d62 6572 206f 6620 636f  ..z*Number of co
+000010e0: 6c6f 7273 2074 6f20 6765 6e65 7261 7465  lors to generate
+000010f0: 205b 6465 6661 756c 743a 2031 305d 722c   [default: 10]r,
+00001100: 0000 0072 1400 0000 fa0c 2d2d 636f 6c6f  ...r......--colo
+00001110: 7273 7061 6365 a904 da03 4c61 625a 034c  rspace....LabZ.L
+00001120: 4368 da03 5247 42da 0348 534c 7245 0000  Ch..RGB..HSLrE..
+00001130: 007a 3554 6865 2063 6f6c 6f72 7370 6163  .z5The colorspac
+00001140: 6520 696e 2077 6869 6368 2074 6f20 696e  e in which to in
+00001150: 7465 7270 6f6c 6174 6520 5b64 6566 6175  terpolate [defau
+00001160: 6c74 3a20 4c61 625d a903 721f 0000 0072  lt: Lab]..r....r
+00001170: 1e00 0000 7209 0000 0072 2800 0000 720e  ....r....r(...r.
+00001180: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+00001190: 0000 da0f 7061 7374 656c 5f67 7261 6469  ....pastel_gradi
+000011a0: 656e 74d5 0000 0073 2400 0000 0601 0202  ent....s$.......
+000011b0: 04ff 1004 0401 0201 0201 0201 0201 0201  ................
+000011c0: 06fb 0407 0201 0201 0601 0201 0201 0afb  ................
+000011d0: 7249 0000 0063 0100 0000 0000 0000 0000  rI...c..........
+000011e0: 0000 0100 0000 0700 0000 4300 0000 735a  ..........C...sZ
+000011f0: 0000 0064 017c 005f 0064 027c 005f 017c  ...d.|._.d.|._.|
+00001200: 006a 0264 0364 0464 058d 0201 007c 006a  .j.d.d.d.....|.j
+00001210: 0264 0664 0764 0864 098d 0301 007c 006a  .d.d.d.d.....|.j
+00001220: 0264 0a64 0b67 0064 0ca2 0164 0d64 0e64  .d.d.g.d...d.d.d
+00001230: 0f8d 0501 007c 006a 0264 1064 1174 0364  .....|.j.d.d.t.d
+00001240: 1264 1364 148d 0501 0064 0053 0029 154e  .d.d.....d.S.).N
+00001250: 7a0a 7061 7374 656c 206d 6978 7a4d 4372  z.pastel mixzMCr
+00001260: 6561 7465 206e 6577 2063 6f6c 6f72 7320  eate new colors 
+00001270: 6279 2069 6e74 6572 706f 6c61 7469 6e67  by interpolating
+00001280: 2062 6574 7765 656e 2074 776f 2063 6f6c   between two col
+00001290: 6f72 7320 696e 2074 6865 2067 6976 656e  ors in the given
+000012a0: 2063 6f6c 6f72 7370 6163 6572 0400 0000   colorspacer....
+000012b0: 7a38 5468 6520 6261 7365 2063 6f6c 6f72  z8The base color
+000012c0: 2077 6869 6368 2077 696c 6c20 6265 206d   which will be m
+000012d0: 6978 6564 2077 6974 6820 7468 6520 6f74  ixed with the ot
+000012e0: 6865 7220 636f 6c6f 7273 7240 0000 005a  her colorsr@...Z
+000012f0: 0c6f 7468 6572 5f63 6f6c 6f72 7372 0500  .other_colorsr..
+00001300: 0000 7206 0000 0072 0700 0000 7214 0000  ..r....r....r...
+00001310: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
+00001320: 7a26 5468 6520 636f 6c6f 7273 7061 6365  z&The colorspace
+00001330: 2069 6e20 7768 6963 6820 746f 2069 6e74   in which to int
+00001340: 6572 706f 6c61 7465 7248 0000 007a 022d  erpolaterH...z.-
+00001350: 667a 0a2d 2d66 7261 6374 696f 6e67 0000  fz.--fractiong..
+00001360: 0000 0000 e03f 7a51 5468 6520 6e75 6d62  .....?zQThe numb
+00001370: 6572 2062 6574 7765 656e 2030 2e30 2061  er between 0.0 a
+00001380: 6e64 2031 2e30 2064 6574 6572 6d69 6e69  nd 1.0 determini
+00001390: 6e67 2068 6f77 206d 7563 6820 746f 206d  ng how much to m
+000013a0: 6978 2069 6e20 6672 6f6d 2074 6865 2062  ix in from the b
+000013b0: 6173 6520 636f 6c6f 7272 2c00 0000 a904  ase colorr,.....
+000013c0: 720b 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+000013d0: 0566 6c6f 6174 720e 0000 0072 1000 0000  .floatr....r....
+000013e0: 7210 0000 0072 1100 0000 da0a 7061 7374  r....r......past
+000013f0: 656c 5f6d 6978 ec00 0000 7334 0000 0006  el_mix....s4....
+00001400: 0102 0204 ff04 0402 0102 0106 fe04 0402  ................
+00001410: 0102 0102 0106 fd04 0502 0102 0106 0102  ................
+00001420: 0102 0106 fb04 0702 0102 0102 0102 0102  ................
+00001430: 010a fb72 4c00 0000 6301 0000 0000 0000  ...rL...c.......
+00001440: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00001450: 0073 3400 0000 6401 7c00 5f00 6402 7c00  .s4...d.|._.d.|.
+00001460: 5f01 7c00 6a02 6403 6700 6404 a201 6405  _.|.j.d.g.d...d.
+00001470: 6406 8d03 0100 7c00 6a02 6407 6408 6409  d.....|.j.d.d.d.
+00001480: 640a 8d03 0100 6400 5300 290b 4e7a 1170  d.....d.S.).Nz.p
+00001490: 6173 7465 6c20 636f 6c6f 7262 6c69 6e64  astel colorblind
+000014a0: 7a65 436f 6e76 6572 7420 7468 6520 6769  zeConvert the gi
+000014b0: 7665 6e20 636f 6c6f 7220 746f 2068 6f77  ven color to how
+000014c0: 2069 7420 776f 756c 6420 6c6f 6f6b 2074   it would look t
+000014d0: 6f20 6120 7065 7273 6f6e 2077 6974 6820  o a person with 
+000014e0: 7072 6f74 616e 6f70 6961 2c20 6465 7574  protanopia, deut
+000014f0: 6572 616e 6f70 6961 2c20 6f72 2074 7269  eranopia, or tri
+00001500: 7461 6e6f 7069 6172 2700 0000 2903 5a04  tanopiar'...).Z.
+00001510: 7072 6f74 5a06 6465 7574 6572 5a04 7472  protZ.deuterZ.tr
+00001520: 6974 7a5a 5468 6520 7479 7065 206f 6620  itzZThe type of 
+00001530: 636f 6c6f 7262 6c69 6e64 6e65 7373 2074  colorblindness t
+00001540: 6861 7420 7368 6f75 6c64 2062 6520 7369  hat should be si
+00001550: 6d75 6c61 7465 6420 2870 726f 7461 6e6f  mulated (protano
+00001560: 7069 612c 2064 6575 7465 7261 6e6f 7069  pia, deuteranopi
+00001570: 612c 2074 7269 7461 6e6f 7069 6129 a902  a, tritanopia)..
+00001580: 721f 0000 0072 0900 0000 7204 0000 0072  r....r....r....r
+00001590: 0500 0000 7206 0000 0072 0700 0000 720a  ....r....r....r.
+000015a0: 0000 0072 0e00 0000 7210 0000 0072 1000  ...r....r....r..
+000015b0: 0000 7211 0000 00da 1170 6173 7465 6c5f  ..r......pastel_
+000015c0: 636f 6c6f 7262 6c69 6e64 0b01 0000 7318  colorblind....s.
+000015d0: 0000 0006 0106 0104 0202 0106 0102 0106  ................
+000015e0: fd04 0502 0102 0102 010a fd72 4e00 0000  ...........rN...
+000015f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001600: 0005 0000 0043 0000 0073 4200 0000 6401  .....C...sB...d.
+00001610: 7c00 5f00 6402 7c00 5f01 7c00 6a02 6403  |._.d.|._.|.j.d.
+00001620: 6700 6404 a201 6405 6406 8d03 0100 7c00  g.d...d.d.....|.
+00001630: 6a02 6407 6408 6409 8d02 0100 7c00 6a02  j.d.d.d.....|.j.
+00001640: 640a 640b 640c 640d 8d03 0100 6400 5300  d.d.d.d.....d.S.
+00001650: 290e 4e7a 0a70 6173 7465 6c20 7365 747a  ).Nz.pastel setz
+00001660: 2a53 6574 2074 6865 2067 6976 656e 2070  *Set the given p
+00001670: 726f 7065 7274 7920 746f 2061 2073 7065  roperty to a spe
+00001680: 6369 6669 6320 7661 6c75 65da 0870 726f  cific value..pro
+00001690: 7065 7274 7929 0bda 096c 6967 6874 6e65  perty)...lightne
+000016a0: 7373 7216 0000 0072 1a00 0000 723a 0000  ssr....r....r:..
+000016b0: 0072 3b00 0000 da03 7265 64da 0567 7265  .r;.....red..gre
+000016c0: 656e da04 626c 7565 7236 0000 0072 3700  en..bluer6...r7.
+000016d0: 0000 7238 0000 007a 2354 6865 2070 726f  ..r8...z#The pro
+000016e0: 7065 7274 7920 7468 6174 2073 686f 756c  perty that shoul
+000016f0: 6420 6265 2063 6861 6e67 6564 724d 0000  d be changedrM..
+00001700: 00da 0576 616c 7565 7a27 5468 6520 6e65  ...valuez'The ne
+00001710: 7720 6e75 6d65 7269 6361 6c20 7661 6c75  w numerical valu
+00001720: 6520 6f66 2074 6865 2070 726f 7065 7274  e of the propert
+00001730: 7972 4000 0000 7204 0000 0072 0500 0000  yr@...r....r....
+00001740: 7206 0000 0072 0700 0000 720a 0000 0072  r....r....r....r
+00001750: 0e00 0000 7210 0000 0072 1000 0000 7211  ....r....r....r.
+00001760: 0000 00da 0a70 6173 7465 6c5f 7365 741b  .....pastel_set.
+00001770: 0100 0073 1a00 0000 0601 0601 0402 0201  ...s............
+00001780: 0601 020d 06f1 0e11 0401 0201 0201 0201  ................
+00001790: 0afd 7255 0000 0063 0100 0000 0000 0000  ..rU...c........
+000017a0: 0000 0000 0100 0000 0500 0000 4300 0000  ............C...
+000017b0: f330 0000 0064 017c 005f 0064 027c 005f  .0...d.|._.d.|._
+000017c0: 017c 006a 0264 0374 0364 0464 058d 0301  .|.j.d.t.d.d....
+000017d0: 007c 006a 0264 0664 0764 0864 098d 0301  .|.j.d.d.d.d....
+000017e0: 0064 0053 0029 0a4e 7a0f 7061 7374 656c  .d.S.).Nz.pastel
+000017f0: 2073 6174 7572 6174 657a 5c49 6e63 7265   saturatez\Incre
+00001800: 6173 6520 7468 6520 7361 7475 7261 7469  ase the saturati
+00001810: 6f6e 206f 6620 6120 636f 6c6f 7220 6279  on of a color by
+00001820: 2061 6464 696e 6720 6120 6365 7274 6169   adding a certai
+00001830: 6e20 616d 6f75 6e74 2074 6f20 7468 6520  n amount to the 
+00001840: 4853 4c20 7361 7475 7261 7469 6f6e 2063  HSL saturation c
+00001850: 6861 6e6e 656c 2eda 0661 6d6f 756e 74fa  hannel...amount.
+00001860: 3841 6d6f 756e 7420 6f66 2073 6174 7572  8Amount of satur
+00001870: 6174 696f 6e20 746f 2061 6464 2028 6e75  ation to add (nu
+00001880: 6d62 6572 2062 6574 7765 656e 2030 2e30  mber between 0.0
+00001890: 2061 6e64 2031 2e30 29a9 0272 2700 0000   and 1.0)..r'...
+000018a0: 7209 0000 0072 0400 0000 7205 0000 0072  r....r....r....r
+000018b0: 0600 0000 7207 0000 0072 4a00 0000 720e  ....r....rJ...r.
+000018c0: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
+000018d0: 0000 da0f 7061 7374 656c 5f73 6174 7572  ....pastel_satur
+000018e0: 6174 6538 0100 00f3 1800 0000 0601 0601  ate8............
+000018f0: 0402 0201 0201 0201 06fd 0405 0201 0201  ................
+00001900: 0201 0afd 725a 0000 0063 0100 0000 0000  ....rZ...c......
+00001910: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00001920: 0000 7256 0000 0029 0a4e 7a11 7061 7374  ..rV...).Nz.past
+00001930: 656c 2064 6573 6174 7572 6174 657a 6344  el desaturatezcD
+00001940: 6563 7265 6173 6520 7468 6520 7361 7475  ecrease the satu
+00001950: 7261 7469 6f6e 206f 6620 6120 636f 6c6f  ration of a colo
+00001960: 7220 6279 2073 7562 7472 6163 7469 6e67  r by subtracting
+00001970: 2061 2063 6572 7461 696e 2061 6d6f 756e   a certain amoun
+00001980: 7420 6672 6f6d 2074 6865 2048 534c 2073  t from the HSL s
+00001990: 6174 7572 6174 696f 6e20 6368 616e 6e65  aturation channe
+000019a0: 6c2e 7257 0000 0072 5800 0000 7259 0000  l.rW...rX...rY..
+000019b0: 0072 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+000019c0: 7207 0000 0072 4a00 0000 720e 0000 0072  r....rJ...r....r
+000019d0: 1000 0000 7210 0000 0072 1100 0000 da11  ....r....r......
+000019e0: 7061 7374 656c 5f64 6573 6174 7572 6174  pastel_desaturat
+000019f0: 6548 0100 0072 5b00 0000 725c 0000 0063  eH...r[...r\...c
+00001a00: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001a10: 0500 0000 4300 0000 7256 0000 0029 0a4e  ....C...rV...).N
+00001a20: 7a0e 7061 7374 656c 206c 6967 6874 656e  z.pastel lighten
+00001a30: 7a48 4c69 6768 7465 6e20 6120 636f 6c6f  zHLighten a colo
+00001a40: 7220 6279 2061 6464 696e 6720 6120 6365  r by adding a ce
+00001a50: 7274 6169 6e20 616d 6f75 6e74 2074 6f20  rtain amount to 
+00001a60: 7468 6520 4853 4c20 6c69 6768 746e 6573  the HSL lightnes
+00001a70: 7320 6368 616e 6e65 6c2e 7257 0000 0072  s channel.rW...r
+00001a80: 5800 0000 7259 0000 0072 0400 0000 7205  X...rY...r....r.
+00001a90: 0000 0072 0600 0000 7207 0000 0072 4a00  ...r....r....rJ.
+00001aa0: 0000 720e 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00001ab0: 0072 1100 0000 da0e 7061 7374 656c 5f6c  .r......pastel_l
+00001ac0: 6967 6874 656e 5801 0000 f31a 0000 0006  ightenX.........
+00001ad0: 0102 0204 ff04 0402 0102 0102 0106 fd04  ................
+00001ae0: 0502 0102 0102 010a fd72 5d00 0000 6301  .........r]...c.
+00001af0: 0000 0000 0000 0000 0000 0001 0000 0005  ................
+00001b00: 0000 0043 0000 0072 5600 0000 290a 4e7a  ...C...rV...).Nz
+00001b10: 0d70 6173 7465 6c20 6461 726b 656e 7a4a  .pastel darkenzJ
+00001b20: 4461 726b 656e 2061 2063 6f6c 6f72 2062  Darken a color b
+00001b30: 7920 7375 6274 7261 6374 696e 6720 6120  y subtracting a 
+00001b40: 6365 7274 6169 6e20 616d 6f75 6e74 2066  certain amount f
+00001b50: 726f 6d20 7468 6520 6c69 6768 746e 6573  rom the lightnes
+00001b60: 7320 6368 616e 6e65 6c2e 7257 0000 0072  s channel.rW...r
+00001b70: 5800 0000 7259 0000 0072 0400 0000 7205  X...rY...r....r.
+00001b80: 0000 0072 0600 0000 7207 0000 0072 4a00  ...r....r....rJ.
+00001b90: 0000 720e 0000 0072 1000 0000 7210 0000  ..r....r....r...
+00001ba0: 0072 1100 0000 da0d 7061 7374 656c 5f64  .r......pastel_d
+00001bb0: 6172 6b65 6e6a 0100 0072 5e00 0000 725f  arkenj...r^...r_
+00001bc0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001bd0: 0100 0000 0500 0000 4300 0000 7256 0000  ........C...rV..
+00001be0: 0029 0a4e 7a0d 7061 7374 656c 2072 6f74  .).Nz.pastel rot
+00001bf0: 6174 6575 b200 0000 526f 7461 7465 2074  ateu....Rotate t
+00001c00: 6865 2048 534c 2068 7565 2063 6861 6e6e  he HSL hue chann
+00001c10: 656c 206f 6620 6120 636f 6c6f 7220 6279  el of a color by
+00001c20: 2074 6865 2073 7065 6369 6669 6564 2061   the specified a
+00001c30: 6e67 6c65 2028 696e 2064 6567 7265 6573  ngle (in degrees
+00001c40: 292e 2041 2072 6f74 6174 696f 6e20 6279  ). A rotation by
+00001c50: 2031 3830 c2b0 2072 6574 7572 6e73 2074   180.. returns t
+00001c60: 6865 2063 6f6d 706c 656d 656e 7461 7279  he complementary
+00001c70: 2063 6f6c 6f72 2e20 4120 726f 7461 7469   color. A rotati
+00001c80: 6f6e 2062 7920 3336 30c2 b020 7265 7475  on by 360.. retu
+00001c90: 726e 7320 746f 2074 6865 206f 7269 6769  rns to the origi
+00001ca0: 6e61 6c20 636f 6c6f 722e da07 6465 6772  nal color...degr
+00001cb0: 6565 737a 3661 6e67 6c65 2062 7920 7768  eesz6angle by wh
+00001cc0: 6963 6820 746f 2072 6f74 6174 6520 2869  ich to rotate (i
+00001cd0: 6e20 6465 6772 6565 732c 2063 616e 2062  n degrees, can b
+00001ce0: 6520 6e65 6761 7469 7665 2972 5900 0000  e negative)rY...
+00001cf0: 7204 0000 0072 0500 0000 7206 0000 0072  r....r....r....r
+00001d00: 0700 0000 724a 0000 0072 0e00 0000 7210  ....rJ...r....r.
+00001d10: 0000 0072 1000 0000 7211 0000 00da 0d70  ...r....r......p
+00001d20: 6173 7465 6c5f 726f 7461 7465 7c01 0000  astel_rotate|...
+00001d30: 725b 0000 0072 6100 0000 6301 0000 0000  r[...ra...c.....
+00001d40: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00001d50: 0000 0072 0300 0000 2907 4e7a 1170 6173  ...r....).Nz.pas
+00001d60: 7465 6c20 636f 6d70 6c65 6d65 6e74 7549  tel complementuI
+00001d70: 0000 0043 6f6d 7075 7465 2074 6865 2063  ...Compute the c
+00001d80: 6f6d 706c 656d 656e 7461 7279 2063 6f6c  omplementary col
+00001d90: 6f72 2062 7920 726f 7461 7469 6e67 2074  or by rotating t
+00001da0: 6865 2048 534c 2068 7565 2063 6861 6e6e  he HSL hue chann
+00001db0: 656c 2062 7920 3138 30c2 b02e 7204 0000  el by 180...r...
+00001dc0: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
+00001dd0: 720a 0000 0072 0e00 0000 7210 0000 0072  r....r....r....r
+00001de0: 1000 0000 7211 0000 00da 1170 6173 7465  ....r......paste
+00001df0: 6c5f 636f 6d70 6c65 6d65 6e74 8c01 0000  l_complement....
+00001e00: f310 0000 0006 0102 0204 ff04 0402 0102  ................
+00001e10: 0102 010a fd72 6200 0000 6301 0000 0000  .....rb...c.....
+00001e20: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+00001e30: 0000 0073 2000 0000 6401 7c00 5f00 6402  ...s ...d.|._.d.
+00001e40: 7c00 5f01 7c00 6a02 6403 7403 6404 6405  |._.|.j.d.t.d.d.
+00001e50: 8d03 0100 6400 5300 2906 4e7a 0b70 6173  ....d.S.).Nz.pas
+00001e60: 7465 6c20 6772 6179 7a30 4372 6561 7465  tel grayz0Create
+00001e70: 2061 2067 7261 7920 746f 6e65 2066 726f   a gray tone fro
+00001e80: 6d20 6120 6769 7665 6e20 6c69 6768 746e  m a given lightn
+00001e90: 6573 7320 7661 6c75 652e 7250 0000 007a  ess value.rP...z
+00001ea0: 3f4c 6967 6874 6e65 7373 206f 6620 7468  ?Lightness of th
+00001eb0: 6520 6372 6561 7465 6420 6772 6179 2074  e created gray t
+00001ec0: 6f6e 6520 286e 756d 6265 7220 6265 7477  one (number betw
+00001ed0: 6565 6e20 302e 3020 616e 6420 312e 3029  een 0.0 and 1.0)
+00001ee0: 7259 0000 0072 4a00 0000 720e 0000 0072  rY...rJ...r....r
+00001ef0: 1000 0000 7210 0000 0072 1100 0000 da0b  ....r....r......
+00001f00: 7061 7374 656c 5f67 7261 7999 0100 0072  pastel_gray....r
+00001f10: 1300 0000 7264 0000 0063 0100 0000 0000  ....rd...c......
+00001f20: 0000 0000 0000 0100 0000 0500 0000 4300  ..............C.
+00001f30: 0000 7203 0000 0029 074e 7a0e 7061 7374  ..r....).Nz.past
+00001f40: 656c 2074 6f2d 6772 6179 7a45 436f 6d70  el to-grayzEComp
+00001f50: 6c65 7465 6c79 2064 6573 6174 7572 6174  letely desaturat
+00001f60: 6520 7468 6520 6769 7665 6e20 636f 6c6f  e the given colo
+00001f70: 7220 7768 696c 6520 7072 6573 6572 7669  r while preservi
+00001f80: 6e67 2074 6865 206c 756d 696e 616e 6365  ng the luminance
+00001f90: 2e72 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
+00001fa0: 7207 0000 0072 0a00 0000 720e 0000 0072  r....r....r....r
+00001fb0: 1000 0000 7210 0000 0072 1100 0000 da0e  ....r....r......
+00001fc0: 7061 7374 656c 5f74 6f5f 6772 6179 a401  pastel_to_gray..
+00001fd0: 0000 7263 0000 0072 6500 0000 6301 0000  ..rc...re...c...
+00001fe0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00001ff0: 0043 0000 0072 0300 0000 2907 4e7a 1070  .C...r....).Nz.p
+00002000: 6173 7465 6c20 7465 7874 636f 6c6f 727a  astel textcolorz
+00002010: c252 6574 7572 6e20 6120 7265 6164 6162  .Return a readab
+00002020: 6c65 2066 6f72 6567 726f 756e 6420 7465  le foreground te
+00002030: 7874 2063 6f6c 6f72 2028 6569 7468 6572  xt color (either
+00002040: 2062 6c61 636b 206f 7220 7768 6974 6529   black or white)
+00002050: 2066 6f72 2061 2067 6976 656e 2062 6163   for a given bac
+00002060: 6b67 726f 756e 6420 636f 6c6f 722e 2054  kground color. T
+00002070: 6869 7320 6361 6e20 616c 736f 2062 6520  his can also be 
+00002080: 7573 6564 2069 6e20 7468 6520 6f70 706f  used in the oppo
+00002090: 7369 7465 2077 6179 2c20 692e 652e 2074  site way, i.e. t
+000020a0: 6f20 6372 6561 7465 2061 2062 6163 6b67  o create a backg
+000020b0: 726f 756e 6420 636f 6c6f 7220 666f 7220  round color for 
+000020c0: 6120 6769 7665 6e20 7465 7874 2063 6f6c  a given text col
+000020d0: 6f72 2e72 0400 0000 7205 0000 0072 0600  or.r....r....r..
+000020e0: 0000 7207 0000 0072 0a00 0000 720e 0000  ..r....r....r...
+000020f0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00002100: da10 7061 7374 656c 5f74 6578 7463 6f6c  ..pastel_textcol
+00002110: 6f72 b101 0000 7213 0000 0072 6600 0000  or....r....rf...
+00002120: 6300 0000 0000 0000 0000 0000 0003 0000  c...............
+00002130: 0004 0000 0047 0000 0073 3c01 0000 7400  .....G...s<...t.
+00002140: 6a01 6401 6402 8d01 7d01 7c01 a002 a100  j.d.d...}.|.....
+00002150: 7d02 7403 7c02 a004 6403 a101 8301 0100  }.t.|...d.......
+00002160: 7405 7c02 a004 6404 a101 8301 0100 7406  t.|...d.......t.
+00002170: 7c02 a004 6405 a101 8301 0100 7407 7c02  |...d.......t.|.
+00002180: a004 6406 a101 8301 0100 7408 7c02 a004  ..d.......t.|...
+00002190: 6407 a101 8301 0100 7409 7c02 a004 6408  d.......t.|...d.
+000021a0: a101 8301 0100 740a 7c02 a004 6409 a101  ......t.|...d...
+000021b0: 8301 0100 740b 7c02 a004 640a a101 8301  ....t.|...d.....
+000021c0: 0100 740c 7c02 a004 640b a101 8301 0100  ..t.|...d.......
+000021d0: 740d 7c02 a004 640c a101 8301 0100 740e  t.|...d.......t.
+000021e0: 7c02 a004 640d a101 8301 0100 740f 7c02  |...d.......t.|.
+000021f0: a004 640e a101 8301 0100 7410 7c02 a004  ..d.......t.|...
+00002200: 640f a101 8301 0100 7411 7c02 a004 6410  d.......t.|...d.
+00002210: a101 8301 0100 7412 7c02 a004 6411 a101  ......t.|...d...
+00002220: 8301 0100 7413 7c02 a004 6412 a101 8301  ....t.|...d.....
+00002230: 0100 7414 7c02 a004 6413 a101 8301 0100  ..t.|...d.......
+00002240: 7415 7c02 a004 6414 a101 8301 0100 7416  t.|...d.......t.
+00002250: 7c02 a004 6415 a101 8301 0100 7417 7c02  |...d.......t.|.
+00002260: a004 6416 a101 8301 0100 7418 7c01 7c00  ..d.......t.|.|.
+00002270: 6417 8d02 0100 6400 5300 2918 4e5a 0670  d.....d.S.).NZ.p
+00002280: 6173 7465 6c29 0172 0b00 0000 7204 0000  astel).r....r...
+00002290: 00da 046c 6973 7472 1b00 0000 5a08 6469  ...listr....Z.di
+000022a0: 7374 696e 6374 7a07 736f 7274 2d62 79da  stinctz.sort-by.
+000022b0: 0666 6f72 6d61 745a 0570 6169 6e74 5a08  .formatZ.paintZ.
+000022c0: 6772 6164 6965 6e74 5a03 6d69 785a 0a63  gradientZ.mixZ.c
+000022d0: 6f6c 6f72 626c 696e 64da 0373 6574 5a08  olorblind..setZ.
+000022e0: 7361 7475 7261 7465 5a0a 6465 7361 7475  saturateZ.desatu
+000022f0: 7261 7465 da07 6c69 6768 7465 6eda 0664  rate..lighten..d
+00002300: 6172 6b65 6eda 0672 6f74 6174 655a 0a63  arken..rotateZ.c
+00002310: 6f6d 706c 656d 656e 7472 2300 0000 7a07  omplementr#...z.
+00002320: 746f 2d67 7261 795a 0974 6578 7463 6f6c  to-grayZ.textcol
+00002330: 6f72 2901 da08 636c 695f 6172 6773 2919  or)...cli_args).
+00002340: da04 7961 7078 da0e 4172 6775 6d65 6e74  ..yapx..Argument
+00002350: 5061 7273 6572 da0e 6164 645f 7375 6270  Parser..add_subp
+00002360: 6172 7365 7273 7212 0000 00da 0a61 6464  arsersr......add
+00002370: 5f70 6172 7365 7272 2000 0000 722a 0000  _parserr ...r*..
+00002380: 0072 3000 0000 7233 0000 0072 3f00 0000  .r0...r3...r?...
+00002390: 7242 0000 0072 4900 0000 724c 0000 0072  rB...rI...rL...r
+000023a0: 4e00 0000 7255 0000 0072 5a00 0000 725c  N...rU...rZ...r\
+000023b0: 0000 0072 5d00 0000 725f 0000 0072 6100  ...r]...r_...ra.
+000023c0: 0000 7262 0000 0072 6400 0000 7265 0000  ..rb...rd...re..
+000023d0: 0072 6600 0000 7202 0000 0029 03da 0461  .rf...r....)...a
+000023e0: 7267 7372 0f00 0000 da0a 7375 6270 6172  rgsr......subpar
+000023f0: 7365 7273 7210 0000 0072 1000 0000 7211  sersr....r....r.
+00002400: 0000 00da 046d 6169 6ebc 0100 0073 2e00  .....main....s..
+00002410: 0000 0c01 0802 0e02 0e01 0e01 0e01 0e01  ................
+00002420: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 0e01  ................
+00002430: 0e01 0e01 0e01 0e01 0e01 0e01 0e01 1002  ................
+00002440: 7274 0000 0029 1872 6e00 0000 da0c 6172  rt...).rn.....ar
+00002450: 6770 6172 7365 5f74 7569 7202 0000 0072  gparse_tuir....r
+00002460: 1200 0000 7220 0000 0072 2a00 0000 7230  ....r ...r*...r0
+00002470: 0000 0072 3300 0000 723f 0000 0072 4200  ...r3...r?...rB.
+00002480: 0000 7249 0000 0072 4c00 0000 724e 0000  ..rI...rL...rN..
+00002490: 0072 5500 0000 725a 0000 0072 5c00 0000  .rU...rZ...r\...
+000024a0: 725d 0000 0072 5f00 0000 7261 0000 0072  r]...r_...ra...r
+000024b0: 6200 0000 7264 0000 0072 6500 0000 7266  b...rd...re...rf
+000024c0: 0000 0072 7400 0000 7210 0000 0072 1000  ...rt...r....r..
+000024d0: 0000 7210 0000 0072 1100 0000 da08 3c6d  ..r....r......<m
+000024e0: 6f64 756c 653e 0100 0000 732e 0000 0008  odule>....s.....
+000024f0: 000c 0108 0308 0b08 0e08 1608 2008 1e08  ............ ...
+00002500: 3308 3008 1708 1f08 1008 1d08 1008 1008  3.0.............
+00002510: 1208 1208 1008 0d08 0b08 0d0c 0b         .............
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/__pycache__/rsync.cpython-310.pyc` & `tuiview-0.1.0a2/src/tuiview/cmd/__pycache__/rsync.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Jul 28 07:09:39 2023 UTC, .py size: 2890 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b369 c364 4a0b 0000  o........i.dJ...
+00000000: 6f0d 0d0a 0000 0000 5625 c764 5e0b 0000  o.......V%.d^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6500 6a03 6602 6404 6405 8404  ..d.e.j.f.d.d...
 00000050: 5a04 6406 6407 8400 5a05 6401 5300 2908  Z.d.d...Z.d.S.).
 00000060: e900 0000 004e 2901 da0a 696e 766f 6b65  .....N)...invoke
 00000070: 5f74 7569 da06 7265 7475 726e 6300 0000  _tui..returnc...
@@ -118,19 +118,20 @@
 00000750: 0102 0106 fc04 0602 0102 0102 0102 0106  ................
 00000760: fc04 0602 0102 0102 0102 0106 fc04 0602  ................
 00000770: 0102 0102 0106 fd04 0502 0102 0102 0102  ................
 00000780: 0106 fc04 0602 0102 0102 0106 fd04 0502  ................
 00000790: 0102 0102 0106 fd04 0502 0102 0102 0102  ................
 000007a0: 0106 fc04 0602 0102 0102 0106 fd04 0672  ...............r
 000007b0: 0400 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000007c0: 0000 0000 0002 0000 0043 0000 0073 0e00  .........C...s..
-000007d0: 0000 7400 7401 8300 8301 0100 6400 5300  ..t.t.......d.S.
-000007e0: 2901 4e29 0272 0200 0000 7204 0000 0072  ).N).r....r....r
-000007f0: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
-00000800: 0000 00da 046d 6169 6e73 0000 0073 0200  .....mains...s..
-00000810: 0000 0e01 7219 0000 0029 0672 1300 0000  ....r....).r....
-00000820: da0c 6172 6770 6172 7365 5f74 7569 7202  ..argparse_tuir.
-00000830: 0000 0072 1400 0000 7204 0000 0072 1900  ...r....r....r..
-00000840: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
-00000850: 0072 1800 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-00000860: 0100 0000 7308 0000 0008 000c 0110 030c  ....s...........
-00000870: 6e                                       n
+000007c0: 0001 0000 0004 0000 0047 0000 0073 1200  .........G...s..
+000007d0: 0000 7400 7401 8300 7c00 6401 8d02 0100  ..t.t...|.d.....
+000007e0: 6400 5300 2902 4e29 01da 0863 6c69 5f61  d.S.).N)...cli_a
+000007f0: 7267 7329 0272 0200 0000 7204 0000 0029  rgs).r....r....)
+00000800: 01da 0461 7267 7372 1700 0000 7217 0000  ...argsr....r...
+00000810: 0072 1800 0000 da04 6d61 696e 7300 0000  .r......mains...
+00000820: 7302 0000 0012 0172 1b00 0000 2906 7213  s......r....).r.
+00000830: 0000 00da 0c61 7267 7061 7273 655f 7475  .....argparse_tu
+00000840: 6972 0200 0000 7214 0000 0072 0400 0000  ir....r....r....
+00000850: 721b 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000860: 1700 0000 7218 0000 00da 083c 6d6f 6475  ....r......<modu
+00000870: 6c65 3e01 0000 0073 0800 0000 0800 0c01  le>....s........
+00000880: 1003 0c6e                                ...n
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/git.py` & `tuiview-0.1.0a2/src/tuiview/cmd/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import argparse
-from typing import Optional
 
 import yapx
 from argparse_tui import invoke_tui
-from yapx.types import Annotated
 
 
 def git_commit(parser):
     parser.prog = "git-commit"
     parser.description = "Record changes to the repository"
 
     # Add arguments
@@ -347,17 +345,17 @@
         help="Synonym for --date=relative",
     )
 
     parser.add_argument("revision_range", nargs="?")
     parser.add_argument("path", nargs=argparse.REMAINDER)
 
 
-def main(cmd: Annotated[Optional[str], yapx.arg(None, pos=True)]):
+def main(*args):
     parser = yapx.ArgumentParser(prog="git")
 
     subparsers = parser.add_subparsers()
 
     git_commit(subparsers.add_parser("commit"))
     git_log(subparsers.add_parser("log"))
     git_merge(subparsers.add_parser("merge"))
 
-    invoke_tui(parser, command_filter=cmd)
+    invoke_tui(parser, cli_args=args)
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/grep.py` & `tuiview-0.1.0a2/src/tuiview/cmd/grep.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,9 +123,9 @@
         action="store_true",
         help="print line number with output lines",
     )
 
     return parser
 
 
-def main():
-    invoke_tui(grep())
+def main(*args):
+    invoke_tui(grep(), cli_args=args)
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/pastel.py` & `tuiview-0.1.0a2/src/tuiview/cmd/pastel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,9 @@
-from typing import Optional
-
 import yapx
 from argparse_tui import invoke_tui
-from yapx.types import Annotated
 
 
 def pastel_color(parser):
     parser.prog = "pastel color"
     parser.description = "Show and display some information about the given color(s)"
 
     parser.add_argument(
@@ -440,15 +437,15 @@
     parser.add_argument(
         "color",
         nargs="+",
         help="Colors can be specified in many different formats, such as #RRGGBB, RRGGBB, #RGB, 'rgb(…, …, …)', 'hsl(…, …, …)', 'gray(…)' or simply by the name of the color.",
     )
 
 
-def main(cmd: Annotated[Optional[str], yapx.arg(None, pos=True)]):
+def main(*args):
     parser = yapx.ArgumentParser(prog="pastel")
 
     subparsers = parser.add_subparsers()
 
     pastel_color(subparsers.add_parser("color"))
     pastel_list(subparsers.add_parser("list"))
     pastel_random(subparsers.add_parser("random"))
@@ -466,8 +463,8 @@
     pastel_darken(subparsers.add_parser("darken"))
     pastel_rotate(subparsers.add_parser("rotate"))
     pastel_complement(subparsers.add_parser("complement"))
     pastel_gray(subparsers.add_parser("gray"))
     pastel_to_gray(subparsers.add_parser("to-gray"))
     pastel_textcolor(subparsers.add_parser("textcolor"))
 
-    invoke_tui(parser, command_filter=cmd)
+    invoke_tui(parser, cli_args=args)
```

### Comparing `tuiview-0.1.0a1/src/tuiview/cmd/rsync.py` & `tuiview-0.1.0a2/src/tuiview/cmd/rsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,9 +108,9 @@
         action="store_true",
         help="update destination files in-place",
     )
 
     return parser
 
 
-def main():
-    invoke_tui(rsync())
+def main(*args):
+    invoke_tui(rsync(), cli_args=args)
```

### Comparing `tuiview-0.1.0a1/src/tuiview.egg-info/PKG-INFO` & `tuiview-0.1.0a2/src/tuiview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuiview
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: A TUI for every CLI.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
         Everyone is permitted to copy and distribute verbatim copies
@@ -737,30 +737,27 @@
 
 ```
 ________________________________________________________________________________
 
 $ tv
 ________________________________________________________________________________
 
-Helpful Parameters:
-  -h, --help            Show this help message.
-  --help-all            Show help for all commands.
-  --version             Show the program version number.
-  --print-shell-completion {bash,zsh,tcsh}
-                        Print shell completion script.
-
-Optional Parameters:
-  -f, --from-file <value>
-                        > Type: Path, Default: None
+helpful parameters:
+  -h, --help  Show this help message.
+  --tui       Show Textual User Interface (TUI).
+  --help-all  Show help for all commands.
+  --version   Show the program version number.
 
-Commands:
+commands:
   <COMMAND>
-    git
+    from-file
     rsync
     grep
+    pastel
+    git
 ```
 
 ### Built-in Tools
 
 Launch the TUI of a known tool by providing its name:
 
 ```
@@ -775,14 +772,20 @@
 
 Notice how `git` has subcommands (`commit`, `merge`, ...). The TUI can be limited to a specific command by giving its name:
 
 ```
 tv git commit
 ```
 
+Any other arguments are parsed and passed-through to the TUI:
+
+```
+tv git commit -m 'hello' -m 'world'
+```
+
 ### Load from File
 
 Recall that argparse-tui allows us to use argparse as a specification language for Textual UIs. So, given a file defining and populating an argparse ArgumentParser with the variable name `parser`, you can feed it into `tuiview` and view the tui, dude :metal:
 
 For example, save the following to `echo.py`:
 
 ```python
@@ -797,20 +800,18 @@
     action="store_true",
     help="do not output the trailing newline",
 )
 ```
 
 > Hint: see this, and `ping.py` in the `examples/` folder
 
-Now display the TUI using: `tv -f echo.py`
+Now display the TUI using: `tv from-file echo.py`
 
-## Contribute
+## Support
 
 If you think this is as cool as I do and want to contribute and help curate files of argparse parsers for various CLI tools, rock on :metal:
 
-## Support
-
 If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/tuiview/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
 
 *Brought to you by...*
 
 <a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

### Comparing `tuiview-0.1.0a1/src/tuiview.egg-info/SOURCES.txt` & `tuiview-0.1.0a2/src/tuiview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuiview-0.1.0a1/src/tuiview.egg-info/requires.txt` & `tuiview-0.1.0a2/src/tuiview.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-yapx[tui]<1,>=0.2.2
+yapx[tui]<1,>=0.2.4
 
 [:python_version < "3.10"]
 typing-extensions
 
 [dev]
 python-lsp-server[rope]==1.*
 pylint==2.*
```

### Comparing `tuiview-0.1.0a1/tests/test_main.py` & `tuiview-0.1.0a2/tests/test_main.py`

 * *Files identical despite different names*

