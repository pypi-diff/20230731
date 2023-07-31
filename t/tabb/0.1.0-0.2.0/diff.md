# Comparing `tmp/tabb-0.1.0.tar.gz` & `tmp/tabb-0.2.0.tar.gz`

## Comparing `tabb-0.1.0.tar` & `tabb-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.1.0/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.1.0/config.json
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.1.0/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.1.0/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.1.0/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.1.0/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/__init__.py
--rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/config.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/context.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/decorators.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/formatter.py
--rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/missing.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/nargs.py
--rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/py.typed
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/types.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/utils.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.1.0/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.1.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.1.0/README.md
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tabb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 tabb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.0/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.2.0/config.json
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.2.0/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.2.0/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.2.0/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.2.0/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10850 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/config.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/context.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7764 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/missing.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16402 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/py.typed
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/types.py
+-rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/utils.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    29324 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.2.0/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.2.0/README.md
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 tabb-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.2.0/PKG-INFO
```

### Comparing `tabb-0.1.0/.DS_Store` & `tabb-0.2.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/test.py` & `tabb-0.2.0/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/.DS_Store` & `tabb-0.2.0/src/.DS_Store`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 0209 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0003  ................
-00000050: 0000 0001 0000 1000 006e 0061 0075 0074  .........n.a.u.t
-00000060: 0069 0063 0000 0000 0000 0000 0000 0000  .i.c............
+00000050: 0000 0001 0000 1000 496c 6f63 626c 6f62  ........Ilocblob
+00000060: 0000 0010 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -26,35 +26,35 @@
 00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0003 0000 000b  ................
-00000210: 0061 0072 0067 006f 006e 0061 0075 0074  .a.r.g.o.n.a.u.t
-00000220: 0069 0063 0073 496c 6f63 626c 6f62 0000  .i.c.sIlocblob..
-00000230: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
-00000240: 0000 0000 000b 0061 0072 0067 006f 006e  .......a.r.g.o.n
-00000250: 0061 0075 0074 0069 0063 0073 6277 7370  .a.u.t.i.c.sbwsp
-00000260: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
-00000270: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
-00000280: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
-00000290: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
-000002a0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
-000002b0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
-000002c0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000002d0: 6261 7208 0908 095f 1018 7b7b 3338 302c  bar...._..{{380,
-000002e0: 2034 3431 7d2c 207b 3932 302c 2034 3336   441}, {920, 436
-000002f0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
-00000300: 0000 0000 0000 0101 0000 0000 0000 000d  ................
-00000310: 0000 0000 0000 0000 0000 0000 0000 008b  ................
-00000320: 0000 000b 0061 0072 0067 006f 006e 0061  .....a.r.g.o.n.a
-00000330: 0075 0074 0069 0063 0073 7653 726e 6c6f  .u.t.i.c.svSrnlo
-00000340: 6e67 0000 0001 0000 0000 0000 0000 0000  ng..............
+00000200: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00000210: 0074 0061 0062 0062 496c 6f63 626c 6f62  .t.a.b.bIlocblob
+00000220: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
+00000230: ffff 0000 0000 0004 0074 0061 0062 0062  .........t.a.b.b
+00000240: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00000250: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00000260: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00000270: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00000280: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00000290: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+000002a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+000002b0: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+000002c0: 3338 302c 2034 3431 7d2c 207b 3932 302c  380, 441}, {920,
+000002d0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+000002e0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+000002f0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00000300: 0000 008b 0000 0004 0074 0061 0062 0062  .........t.a.b.b
+00000310: 7653 726e 6c6f 6e67 0000 0001 0000 0000  vSrnlong........
+00000320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `tabb-0.1.0/src/tabb/base.py` & `tabb-0.2.0/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/callback.py` & `tabb-0.2.0/src/tabb/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,19 +206,19 @@
 
     def __init__(self, path: str, import_dependencies: str | None = None) -> None:
         object.__setattr__(self, "path", path)
         object.__setattr__(self, "import_dependencies", import_dependencies)
 
     @property
     def name(self) -> str:
-        _, _, name = self.path.rpartition(".")
+        _, _, name = self.path.rpartition(":")
         return name
 
     def resolve(self) -> Callable[P, T]:
-        module_name, _, callback_name = self.path.rpartition(".")
+        module_name, _, callback_name = self.path.rpartition(":")
 
         try:
             module = importlib.import_module(module_name)
         except ImportError as error:
             if self.import_dependencies:
                 package, _, _ = module_name.partition(".")
                 message = (
```

### Comparing `tabb-0.1.0/src/tabb/command.py` & `tabb-0.2.0/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/config.py` & `tabb-0.2.0/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/context.py` & `tabb-0.2.0/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/decorators.py` & `tabb-0.2.0/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/exceptions.py` & `tabb-0.2.0/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/formatter.py` & `tabb-0.2.0/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/group.py` & `tabb-0.2.0/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/nargs.py` & `tabb-0.2.0/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parser.py` & `tabb-0.2.0/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/types.py` & `tabb-0.2.0/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/utils.py` & `tabb-0.2.0/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/base.py` & `tabb-0.2.0/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/depends.py` & `tabb-0.2.0/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/group.py` & `tabb-0.2.0/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/parser.py` & `tabb-0.2.0/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/resolve.py` & `tabb-0.2.0/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/types.py` & `tabb-0.2.0/src/tabb/parameter/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/src/tabb/parameter/utils.py` & `tabb-0.2.0/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/.gitignore` & `tabb-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/LICENSE.txt` & `tabb-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/README.md` & `tabb-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.1.0/pyproject.toml` & `tabb-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,20 @@
 keywords = []
 authors = [
   { name = "Trevor Olson", email = "trevor@heytrevor.com" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
-  "Programming Language :: Python",
+  "License :: OSI Approved :: MIT License",
+  "Natural Language :: English",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python",
+  "Typing :: Typed",
 ]
 dependencies = []
 
 [project.urls]
 Documentation = "https://github.com/wtolson/tabb#readme"
 Issues = "https://github.com/wtolson/tabb/issues"
 Source = "https://github.com/wtolson/tabb"
```

### Comparing `tabb-0.1.0/PKG-INFO` & `tabb-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.1.0
+Version: 0.2.0
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 # TaBB
 
 > [!WARNING]
 > TaBB has an alpha devlopment status. This package is untested and the api is subject to change. Use at your own risk.
```

