# Comparing `tmp/sysplant-0.2.1.tar.gz` & `tmp/sysplant-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysplant-0.2.1.tar", max compression
+gzip compressed data, was "sysplant-0.3.0.tar", max compression
```

## Comparing `sysplant-0.2.1.tar` & `sysplant-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,56 @@
--rw-r--r--   0        0        0    35077 2023-07-18 08:13:11.961013 sysplant-0.2.1/LICENSE
--rw-r--r--   0        0        0     9423 2023-07-18 08:13:11.961013 sysplant-0.2.1/README.md
--rw-r--r--   0        0        0      886 2023-07-18 08:13:11.965013 sysplant-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/abstracts/__init__.py
--rw-r--r--   0        0        0     3492 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/abstracts/abstractFactory.py
--rw-r--r--   0        0        0     1998 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/abstracts/abstractGenerator.py
--rw-r--r--   0        0        0     3820 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/constants/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/constants/sysplantConstants.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/data/__init__.py
--rw-r--r--   0        0        0    44046 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/data/definitions.json
--rw-r--r--   0        0        0   332144 2023-07-18 08:13:11.965013 sysplant-0.2.1/sysplant/data/prototypes.json
--rw-r--r--   0        0        0   431123 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/data/windef.nim
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/managers/__init__.py
--rw-r--r--   0        0        0    12333 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/managers/nimGenerator.py
--rw-r--r--   0        0        0    12756 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/managers/templateManager.py
--rw-r--r--   0        0        0     6210 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/sysplant.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/__init__.py
--rw-r--r--   0        0        0     3018 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/base.nim
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/__init__.py
--rw-r--r--   0        0        0     3359 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/canterlot.nim
--rw-r--r--   0        0        0     2698 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/freshy.nim
--rw-r--r--   0        0        0     4461 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/halo.nim
--rw-r--r--   0        0        0     3414 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/hell.nim
--rw-r--r--   0        0        0     2561 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/syswhispers.nim
--rw-r--r--   0        0        0     2873 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/syswhispers3.nim
--rw-r--r--   0        0        0     4527 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/iterators/tartarus.nim
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/resolvers/__init__.py
--rw-r--r--   0        0        0       99 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/resolvers/basic.nim
--rw-r--r--   0        0        0      229 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/resolvers/random.nim
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/stubs/__init__.py
--rw-r--r--   0        0        0      509 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/stubs/direct_x64.nim
--rw-r--r--   0        0        0      568 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/templates/stubs/indirect_x64.nim
--rw-r--r--   0        0        0        0 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/utils/__init__.py
--rw-r--r--   0        0        0     3474 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/utils/loggerSingleton.py
--rw-r--r--   0        0        0      261 2023-07-18 08:13:11.969013 sysplant-0.2.1/sysplant/utils/singleton.py
--rw-r--r--   0        0        0     9960 1970-01-01 00:00:00.000000 sysplant-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35077 2023-07-31 09:01:25.146783 sysplant-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6670 2023-07-31 09:01:25.146783 sysplant-0.3.0/README.md
+-rw-r--r--   0        0        0     1215 2023-07-31 09:01:25.150783 sysplant-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/abstracts/__init__.py
+-rw-r--r--   0        0        0     3508 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/abstracts/abstractFactory.py
+-rw-r--r--   0        0        0     6917 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/abstracts/abstractGenerator.py
+-rw-r--r--   0        0        0     4060 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/constants/__init__.py
+-rw-r--r--   0        0        0     2298 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/constants/sysplantConstants.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/data/__init__.py
+-rw-r--r--   0        0        0    44209 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/data/definitions.json
+-rw-r--r--   0        0        0   332144 2023-07-31 09:01:25.150783 sysplant-0.3.0/sysplant/data/prototypes.json
+-rw-r--r--   0        0        0   431123 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/data/windef.nim
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/managers/__init__.py
+-rw-r--r--   0        0        0     6947 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/managers/cGenerator.py
+-rw-r--r--   0        0        0     7436 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/managers/nimGenerator.py
+-rw-r--r--   0        0        0    13209 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/managers/templateManager.py
+-rw-r--r--   0        0        0     6205 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/sysplant.py
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/__init__.py
+-rw-r--r--   0        0        0    10307 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/base.c
+-rw-r--r--   0        0        0     3634 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/base.nim
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/__init__.py
+-rw-r--r--   0        0        0     4292 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/canterlot.c
+-rw-r--r--   0        0        0     3201 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/canterlot.nim
+-rw-r--r--   0        0        0     4068 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/freshy.c
+-rw-r--r--   0        0        0     2946 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/freshy.nim
+-rw-r--r--   0        0        0     5423 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/halo.c
+-rw-r--r--   0        0        0     4692 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/halo.nim
+-rw-r--r--   0        0        0     4222 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/hell.c
+-rw-r--r--   0        0        0     3645 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/hell.nim
+-rw-r--r--   0        0        0     4113 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/syswhispers.c
+-rw-r--r--   0        0        0     2824 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/syswhispers.nim
+-rw-r--r--   0        0        0     5861 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/syswhispers3.c
+-rw-r--r--   0        0        0     2824 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/syswhispers3.nim
+-rw-r--r--   0        0        0     5501 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/tartarus.c
+-rw-r--r--   0        0        0     4758 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/iterators/tartarus.nim
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/__init__.py
+-rw-r--r--   0        0        0      375 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/basic.c
+-rw-r--r--   0        0        0      175 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/basic.nim
+-rw-r--r--   0        0        0      345 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/number.c
+-rw-r--r--   0        0        0      147 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/number.nim
+-rw-r--r--   0        0        0      741 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/random.c
+-rw-r--r--   0        0        0      608 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/resolvers/random.nim
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/__init__.py
+-rw-r--r--   0        0        0      588 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/direct_x64.c
+-rw-r--r--   0        0        0      509 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/direct_x64.nim
+-rw-r--r--   0        0        0      544 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/direct_x86.c
+-rw-r--r--   0        0        0      445 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/direct_x86.nim
+-rw-r--r--   0        0        0      568 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/indirect_x64.c
+-rw-r--r--   0        0        0      486 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/indirect_x64.nim
+-rw-r--r--   0        0        0      621 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/random_x64.c
+-rw-r--r--   0        0        0      592 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/templates/stubs/random_x64.nim
+-rw-r--r--   0        0        0        0 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/utils/__init__.py
+-rw-r--r--   0        0        0     3474 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/utils/loggerSingleton.py
+-rw-r--r--   0        0        0      261 2023-07-31 09:01:25.154783 sysplant-0.3.0/sysplant/utils/singleton.py
+-rw-r--r--   0        0        0     7207 1970-01-01 00:00:00.000000 sysplant-0.3.0/PKG-INFO
```

### Comparing `sysplant-0.2.1/LICENSE` & `sysplant-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sysplant-0.2.1/sysplant/abstracts/abstractFactory.py` & `sysplant-0.3.0/sysplant/abstracts/abstractFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding:utf-8 -*-
 
 import re
 import string
 import random
 import hashlib
+import struct
 
 from typing import Union
 
 from abc import ABC
 from sysplant.utils.loggerSingleton import LoggerSingleton
 from sysplant.constants.sysplantConstants import SysPlantConstants
 
@@ -46,15 +47,15 @@
         """
         Public method used to remove a TAG pattern in self.data var (dropping the line for clean code at the same time)
 
         Args:
             name (str): the tag name to remove
         """
         self.data = re.sub(
-            f"\s*{SysPlantConstants.TAG_START}{name}{SysPlantConstants.TAG_END}",
+            f"\s*{SysPlantConstants.TAG_START}{name}{SysPlantConstants.TAG_END}.*",
             "",
             self.data,
         )
 
     def __replace_pattern(
         self, pattern: str, content: Union[str, int], count: int = -1
     ) -> None:
```

### Comparing `sysplant-0.2.1/sysplant/constants/__init__.py` & `sysplant-0.3.0/sysplant/constants/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 DESC_HEADER = "..:: SysPlant - Your Syscall Factory ::.."
 FANCY_HEADER = """
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⠶⢤⡀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⢀⣀⡀⠀⢀⣠⣤⣴⣶⣶⡦⠤⢤⣤⣀⣀⣼⠀⠀⡽⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⠈⠫⣯⠙⡟⢿⣿⣿⡿⠁⠀⢠⣾⣿⣿⣿⡿⠀⠀⢹⠘⡆⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
-⠀⠀⣼⣿⣷⣧⡀⢱⠈⠀⠀⠀⣿⣿⣿⣿⣿⡀⠀⠀⢸⠀⢳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀..:: SysPlant - Your Syscall Factory ::..
+⠀⠀⣼⣿⣷⣧⡀⢱⠈⠀⠀⠀⣿⣿⣿⣿⣿⡀⠀⠀⢸⠀⢳⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀  ⠀⠀..:: SysPlant - Your Syscall Factory ::..
 ⠀⣼⣿⣿⣿⣿⣿⣿⡄⢀⣀⣠⣿⣿⣿⠿⢿⣷⣤⡀⠈⠀⡟⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
-⢠⣿⣿⣿⣿⣿⣿⠿⠛⠉⠉⠀⡇⣾⣿⣦⣀⣿⡄⠀⠀⢰⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀ ⠀⠀⠀⠀⠀⠀⠀⠀⠀                    ©2023 - 0x42en 
-⢸⣿⣿⣿⠿⢯⣷⢄⠀⠀⠀⠀⡄⢻⣿⣯⣻⣿⡧⠄⠀⢸⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
-⠘⣿⠟⠁⠀⠚⢻⣦⣱⣄⠀⠀⢣⠈⠛⣽⣿⠿⠭⠀⣠⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⡤⠶⠶⠶⠶⢤⣄⡀⠀⠀⠀⠀⠀⠀⠀⠀
-⠀⠁⠀⠀⠀⠀⠀⠻⣿⣿⠀⠀⠈⠂⠀⠀⢀⣄⣠⣴⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠶⠋⠁⠀⠀⠀⠀⠀⠀⠀⠉⠳⢦⡀⠀⠀⠀⠀⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⣸⠋⠄⢠⠀⠀⠀⠀⣾⣿⣿⣿⣿⣿⡀⠀⠀⠀⠀⠀⠀⠀⡴⠃⠀⣠⣤⣶⣶⣾⣶⣶⣦⣄⠀⠀⠀⠹⣆⠀⠀⠀⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⠈⠲⠴⠯⠤⠤⢶⢾⣿⣿⣿⣿⣿⠏⠷⣄⢀⣀⣀⣀⡀⣼⣠⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⡀⠀⠀⠸⣧⠀⠀⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⠏⠈⠉⣡⣾⣿⠏⠀⢰⣿⠉⣩⠀⠉⢙⣿⡿⠛⠉⠉⠙⠛⢿⣿⣿⣿⣿⣿⣿⣷⠀⠀⠀⢻⣇⠀⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡟⠀⠀⣿⣿⡿⠋⠀⢀⣾⡿⠀⣉⣀⣇⠘⠋⣿⠀⠀⠀⠀⠀⠀⠙⣿⣿⣿⣿⣿⣿⡆⠀⠀⢸⣿⡆⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠃⠀⠀⠘⢯⡀⠀⢀⣾⣿⠇⣴⠨⣿⣿⡯⠀⢸⠀⠀⠀⠀⠀⠀⠀⠘⣿⣿⣿⣿⣿⡇⠀⠀⢸⣿⣷⠀
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⡆⠀⠀⠀⠈⠻⢦⣾⣿⠏⠀⠈⢈⣝⡟⠁⣶⣾⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⣿⣿⣿⡇⠀⠀⢸⣿⣿⡀
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡀⢄⣀⡀⠀⠀⠉⠁⠀⠰⣄⠀⠁⠀⠀⢀⡏⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⣿⣿⣿⠃⠀⠀⣸⣿⣿⡇
-⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢷⡀⢹⠁⠀⢠⠶⠤⠤⢴⡾⢦⡀⠀⠀⣼⠦⡄⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⠀⠀⠀⣿⣿⣿⠇
+⢠⣿⣿⣿⣿⣿⣿⠿⠛⠉⠉⠀⡇⣾⣿⣦⣀⣿⡄⠀⠀⢰⠃⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀ ⠀⠀⠀⠀⠀⠀⠀⠀⠀              Sysplant (2023) - 0x42en 
+⢸⣿⣿⣿⠿⢯⣷⢄⠀⠀⠀⠀⡄⢻⣿⣯⣻⣿⡧⠄⠀⢸⠀
+⠘⣿⠟⠁⠀⠚⢻⣦⣱⣄⠀⠀⢣⠈⠛⣽⣿⠿⠭⠀⣠⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣠⡤⠶⠶⠶⠶⢤⣄⡀⠀⠀⠀⠀⠀ Canterlot's Gate (2022) - @MDSecLabs⠀
+⠀⠁⠀⠀⠀⠀⠀⠻⣿⣿⠀⠀⠈⠂⠀⠀⢀⣄⣠⣴⣿⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀⣠⠶⠋⠁⠀⠀⠀⠀⠀⠀⠀⠉⠳⢦⡀⠀                            @0x42en
+⠀⠀⠀⠀⠀⠀⠀⠀⣸⠋⠄⢠⠀⠀⠀⠀⣾⣿⣿⣿⣿⣿⡀⠀⠀⠀⠀⠀⠀⠀⡴⠃⠀⣠⣤⣶⣶⣾⣶⣶⣦⣄⠀⠀⠀⠹⣆⠀⠀⠀⠀  Syswhispers3 (2022) - @klezVirus
+⠀⠀⠀⠀⠀⠀⠀⠀⠈⠲⠴⠯⠤⠤⢶⢾⣿⣿⣿⣿⣿⠏⠷⣄⢀⣀⣀⣀⡀⣼⣠⣴⣿⣿⣿⣿⣿⣿⣿⣿⣿⣿⣷⡀⠀⠀⠸⣧⠀⠀   Syswhispers2 (2021) - @Jackson_T
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⠏⠈⠉⣡⣾⣿⠏⠀⢰⣿⠉⣩⠀⠉⢙⣿⡿⠛⠉⠉⠙⠛⢿⣿⣿⣿⣿⣿⣿⣷⠀⠀⠀⢻⣇⠀                         @modexpblog
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡟⠀⠀⣿⣿⡿⠋⠀⢀⣾⡿⠀⣉⣀⣇⠘⠋⣿⠀⠀⠀⠀⠀⠀⠙⣿⣿⣿⣿⣿⣿⡆⠀⠀⢸⣿⡆ Tartarus' Gate (2021) - @trickster0
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢸⠃⠀⠀⠘⢯⡀⠀⢀⣾⣿⠇⣴⠨⣿⣿⡯⠀⢸⠀⠀⠀⠀⠀⠀⠀⠘⣿⣿⣿⣿⣿⡇⠀⠀⢸⣿⣷    Halo's Gate (2021) - @Sektor7net
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⡆⠀⠀⠀⠈⠻⢦⣾⣿⠏⠀⠈⢈⣝⡟⠁⣶⣾⠀⠀⠀⠀⠀⠀⠀⠀⢹⣿⣿⣿⣿⡇⠀⠀⢸⣿⣿⡀   FreshyCalls (2020) - @crummie5
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢻⡀⢄⣀⡀⠀⠀⠉⠁⠀⠰⣄⠀⠁⠀⠀⢀⡏⠀⠀⠀⠀⠀⠀⠀⠀⠈⣿⣿⣿⣿⠃⠀⠀⣸⣿⣿⡇   Hell's Gate (2020) - @RtlMateusz
+⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⢷⡀⢹⠁⠀⢠⠶⠤⠤⢴⡾⢦⡀⠀⠀⣼⠦⡄⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⣿⠀⠀⠀⣿⣿⣿⠇                        @am0nsec
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⣷⠇⠀⠀⢸⡄⠀⠀⠀⠙⢆⠙⢦⡀⠀⠀⠙⣦⠀⠀⠀⠀⠀⠀⠀⣿⣿⣿⡇⠀⠀⢰⣿⡿⠋⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡟⠀⠀⠀⡟⢻⡀⠀⠀⠀⠈⢳⡀⢳⡀⠀⠀⠈⢧⡀⠀⠀⠀⠀⠀⣿⣿⣿⠁⠀⢀⣼⠟⠁⠀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡞⠀⠀⠀⠀⡇⠀⢧⠀⠀⠀⠀⠀⢷⠀⢳⠀⠀⠀⠈⢧⠀⠀⠀⠀⢀⣿⣿⡏⢀⣴⠟⠁⠀⠀⠀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡞⠀⠀⠀⠀⢸⠇⠀⠸⡆⠀⠀⠀⠀⢸⠀⢸⡇⠀⠀⠀⠘⣧⠀⠀⠀⢸⣿⣿⡷⠛⠁⠀⠀⠀⠀⠀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⡞⠀⠀⠀⠀⠀⣾⠀⠀⠀⣧⠀⠀⠀⠀⢸⠀⠀⡇⠀⠀⠀⠀⢸⡆⠀⠀⣿⠿⠋⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⠎⠀⠀⠀⠀⠀⣰⠇⠀⠀⠀⣿⠀⠀⠀⠀⣏⣀⣸⠇⠀⠀⠀⠀⠀⣷⠀⠈⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
 ⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠻⠤⣤⣤⣤⡤⠴⠛⠛⠛⠛⠉⠁⠀⠀⠀⠀⠈⠉⢿⣄⣀⣠⣤⡤⠶⠋⠀⠀⠀⠀⠀⠀⠀⠀
```

### Comparing `sysplant-0.2.1/sysplant/constants/sysplantConstants.py` & `sysplant-0.3.0/sysplant/constants/sysplantConstants.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,28 +4,40 @@
 class SysPlantConstants:
     """
     Simple class storing constants for SysPlant app.
 
     """
 
     SEARCH_EXT = (".h", ".c", ".cpp", ".nim")
-    TEMPLATE_EXT = "nim"
     NIM_TAB = "    "
+    C_TAB = "    "
     TAG_START = "##__"
     TAG_END = "__##"
     RANDOM_WORD_SIZE = 8
     INTERNAL_FUNCTIONS = [
+        "SPT_HEADER_H_",
         "SPT_SEED",
+        "SPT_RVA2VA",
+        "SPT_MAX_ENTRIES",
+        "SPT_SYSCALL_ENTRY",
+        "SPT_SYSCALL_LIST",
         "SPT_Iterator",
         "SPT_Syscall",
+        "SPT_DetectPadding",
         "SPT_HashSyscallName",
         "SPT_GetSyscallNumber",
-        "SPT_PopulateSyscalls",
         "SPT_GetSyscallAddress",
         "SPT_GetRandomSyscallAddress",
+        "SPT_PopulateSyscallList",
+        "SPT_PopulateSyscalls",
+        "SPT_HashContext",
+        "SPT_HashInit",
+        "SPT_HashUpdate",
+        "SPT_HashFinalize",
+        "SPT_HashStep"
     ]
     DONUT_SYSCALLS = [
         "NtCreateSection",
         "NtMapViewOfSection",
         "NtUnmapViewOfSection",
         "NtContinue",
         "NtClose",
```

### Comparing `sysplant-0.2.1/sysplant/data/definitions.json` & `sysplant-0.3.0/sysplant/data/definitions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9923708920187795%*

 * *Differences: {"'CLIENT_ID'": "OrderedDict([('dependencies', []), ('type', 'struct'), ('definition', [['HANDLE', "*

 * *                "'UniqueProcess'], ['HANDLE', 'UniqueThread']])])",*

 * * "'PIO_APC_ROUTINE'": "{'dependencies': ['IO_STATUS_BLOCK']}"}*

```diff
@@ -243,14 +243,28 @@
                 "WCHAR",
                 "HeadlessRedirection"
             ]
         ],
         "dependencies": [],
         "type": "struct"
     },
+    "CLIENT_ID": {
+        "definition": [
+            [
+                "HANDLE",
+                "UniqueProcess"
+            ],
+            [
+                "HANDLE",
+                "UniqueThread"
+            ]
+        ],
+        "dependencies": [],
+        "type": "struct"
+    },
     "DEBUGOBJECTINFOCLASS": {
         "definition": [
             "DebugObjectFlags = 1",
             "MaxDebugObjectInfoClass"
         ],
         "dependencies": [],
         "type": "enum"
@@ -1102,15 +1116,15 @@
             ],
             [
                 "ULONG",
                 "Reserved"
             ]
         ],
         "dependencies": [
-            "PIO_STATUS_BLOCK"
+            "IO_STATUS_BLOCK"
         ],
         "type": "struct"
     },
     "PLUGPLAY_CONTROL_CLASS": {
         "definition": [
             "PlugPlayControlEnumerateDevice",
             "PlugPlayControlRegisterNewDevice",
```

### Comparing `sysplant-0.2.1/sysplant/data/prototypes.json` & `sysplant-0.3.0/sysplant/data/prototypes.json`

 * *Files identical despite different names*

### Comparing `sysplant-0.2.1/sysplant/data/windef.nim` & `sysplant-0.3.0/sysplant/data/windef.nim`

 * *Files identical despite different names*

### Comparing `sysplant-0.2.1/sysplant/managers/nimGenerator.py` & `sysplant-0.3.0/sysplant/managers/templateManager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,90 @@
 # -*- coding:utf-8 -*-
-
 import json
 
 import importlib.resources as pkg_resources
 
 from sysplant import data as pkg_data
+from sysplant import templates as pkg_templates
+from sysplant.templates import iterators as pkg_iterators
+from sysplant.templates import resolvers as pkg_resolvers
+from sysplant.templates import stubs as pkg_stubs
 
-from sysplant.abstracts.abstractGenerator import AbstractGenerator
 from sysplant.constants.sysplantConstants import SysPlantConstants
+from sysplant.abstracts.abstractFactory import AbstractFactory
+from sysplant.managers.nimGenerator import NIMGenerator
+from sysplant.managers.cGenerator import CGenerator
 
 
-class NIMGenerator(AbstractGenerator):
+class TemplateManager(AbstractFactory):
     """
-    Main class responsible for NIM code generation
+    Main class responsible for template handling: tag replacement or erase with content generated by __coder bot
+
+    Args:
+        AbstractFactory (_type_): AbstractClass defining useful functions potentially reusable by other classes
     """
 
-    def __init__(self) -> None:
+    def __init__(
+        self, arch: str = "x64", syscall: str = "syscall", language: str = "nim"
+    ) -> None:
+        """
+        Init method.
+        Will instanciate appropriate self.__coder var depending on the language selected responsible for code generation
+
+        Args:
+            arch (str, optional): Code architecture to generate. Defaults to "x64".
+            syscall (str, optional): Syscall instruction to use. Defaults to "syscall".
+            language (str, optional): Language type used by code generator. Defaults to "nim".
+
+        Raises:
+            NotImplementedError: Error raised when using unsupported architecture
+            NotImplementedError: Error raised when using unsupported syscall instruction
+            NotImplementedError: Error raised when using unsupported language
+            SystemError: Error raised when unable to load protoypes.json
+            SystemError: Error raised when unable to load base template for language specify
+        """
         super().__init__()
 
-        self.__definitions: dict = {}
-        self.__winimdef = ""
+        # Define language template
+        if arch not in ["x86", "x64", "wow"]:
+            raise NotImplementedError("Sorry architecture not implemented yet")
+        if language not in ["nim", "c"]:
+            raise NotImplementedError("Sorry language not supported ... yet ?!")
+        if syscall not in ["syscall", "sysenter", "int 0x2h"]:
+            raise NotImplementedError(
+                "Sorry syscall instruction not supported ... yet ?!"
+            )
+
+        self.__lang = language
+        self.__arch = arch
+        self.__syscall = syscall
+
+        # Set coder bot
+        if self.__lang == "nim":
+            self.__coder = NIMGenerator()
+        elif self.__lang == "c":
+            self.__coder = CGenerator()
+
+        try:
+            # Always load prototypes & type definitions
+            self.__load_prototypes()
+        except Exception as err:
+            raise SystemError(f"Unable to load prototypes: {err}")
 
         try:
-            # Alaways load prototypes & typedefinitions
-            self.__load_definitions()
-            self.__load_winimdef()
+            # Always load initial template
+            self.data = self.__load_template(pkg_templates, f"base.{self.__lang}")
         except Exception as err:
-            raise SystemError(f"Unable to load mandatory data in NIM Generator: {err}")
+            raise SystemError(f"Unable to load base template: {err}")
+
+        # Initialize seed
+        self.__seed = self.generate_random_seed()
+
+    def __str__(self) -> str:
+        return self.data
 
     def __load_template(self, pkg_module: str, name: str) -> str:
         """Private method used to retrieve specific data file from package module
 
         Args:
             pkg_module (str): The package module containing filename to request
             name (str): Filename to request
@@ -42,289 +96,270 @@
         Returns:
             str: Return the file content (text mode)
         """
         if name is None:
             raise ValueError("Template name can not be null")
 
         # Check only extension dot is set
-        if not name.replace(".", "", 1).isalpha():
+        if not name.replace(".", "", 1).replace(f"_{self.__arch}", "", 1).isalnum():
             raise ValueError("Invalid template name")
 
         # Adapt module based on what to load
         raw = pkg_resources.open_text(pkg_module, name)
         return raw.read()
 
-    def __load_definitions(self) -> None:
+    def __load_prototypes(self) -> None:
         """
-        Private method used to load the definitions file containing all the windows type definitions not set by NIM or winim
+        Private method used to load the prototypes file containing all the windows functions and their parameters (name and type).
+        JSON dictionnary will be loaded once at init in private self.__prototypes for future use.
         """
-        # Load supported functions definitions
-        data = self.__load_template(pkg_data, "definitions.json")
-        self.__definitions = json.loads(data)
+        # Load supported functions prototypes
+        data = self.__load_template(pkg_data, "prototypes.json")
+        self.__prototypes: dict = json.loads(data)
 
-    def __load_winimdef(self) -> None:
+    def load_stub(self, name) -> str:
         """
-        Private method used to load the winim library file responsible for type definition. This prevent duplicate definitions.
-        This file might be updated regularly until all the types are integrated inside Winim library (PR to do)
-        """
-        # Load supported functions definitions
-        self.__winimdef = self.__load_template(pkg_data, "windef.nim")
-
-    def generate_struct(self, name: str, definition: list) -> str:
-        """
-        Public method used to generate a NIM basic structure.
-        The structure will be generated as a public object for external code usages.
-        A pointer to the structure will always be generated in the form of: P+NAME
+        Public method used to load stub pattern file from package
 
         Args:
-            name (str): Structure name
-            definition (list): Structure parameters from definitions.json
+            name (_type_): Stub name to use
+
+        Raises:
+            SystemError: Error raised if filename does not exists
 
         Returns:
-            str: NIM code for basic structure definition (except type keyword for definition chaining)
+            str: File content (text mode)
         """
-        result = f"{SysPlantConstants.NIM_TAB}{name}* " + "{.pure.} = object\n"
-        for var in definition:
-            if len(var) == 2:
-                result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]}\n"
-
-            elif len(var) == 3:
-                result += (
-                    f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]} "
-                    + "{.bitsize: "
-                    + str(var[2])
-                    + ".}: "
-                    + f"{var[0]}\n"
-                )
-        # Always add pointer
-        result += f"{SysPlantConstants.NIM_TAB}P{name}* = ptr {name}\n"
+        try:
+            # Load initial stub template
+            self.data = self.__load_template(pkg_stubs, f"{name}.{self.__lang}")
+        except Exception as err:
+            raise SystemError(f"Unable to load {name} stub: {err}")
 
-        return result
+        return self.data
 
-    def generate_union(self, name: str, definition: list) -> str:
+    def list_supported_syscalls(self) -> list:
         """
-        Public method used to generate NIM union structure when a parent needs it.
-        This structure will be generated as a private object as it won't be directly accessed by external code.
-        A pointer to the union structure will always be generated in the form of: P+NAME
-
-        Args:
-            name (str): Union structure name
-            definition (list): Union structure parameters from definitions.json
+        Public method used to retrieve all supported functions names defined in prototypes.json
 
         Returns:
-            str: NIM code for union structure definition (except type keyword for definition chaining)
+            list: List of NtFunctions names
         """
-        result = f"{SysPlantConstants.NIM_TAB}{name} " + "{.pure, union.} = object\n"
-        for var in definition:
-            if len(var) == 2:
-                result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]}: {var[0]}\n"
-            elif len(var) == 3:
-                result += (
-                    f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var[1]} "
-                    + "{.bitsize: "
-                    + var[2]
-                    + ".}: "
-                    + f"{var[0]}\n"
-                )
-        # Always add pointer
-        result += f"{SysPlantConstants.NIM_TAB}P{name} = ptr {name}\n"
+        return self.__prototypes.keys()
 
-        return result
+    def list_common_syscalls(self) -> list:
+        """
+        Public method used to retrieve most common functions names defined in prototypes.json
 
-    def generate_pointer(self, name: str, definition: list) -> str:
+        Returns:
+            list: List of NtFunctions names
         """
-        Public method used to generate NIM pointer to defined var
-        The pointer will be geneerated as a public object for external code usages.
+        return SysPlantConstants.COMMON_SYSCALLS
 
-        Args:
-            name (str): Pointer name
-            definition (list): Type definition to point to from definitions.json
+    def list_donut_syscalls(self) -> list:
+        """
+        Public method used to retrieve functions names defined in prototypes.json used by Donut project (stay tuned for HOMER project ... ;) )
 
         Returns:
-            str: NIM code for standard pointer declaration
+            list: List of NtFunctions names
         """
-        result = f"{SysPlantConstants.NIM_TAB}{name}* = ptr {definition[0]}\n"
-        return result
+        return SysPlantConstants.DONUT_SYSCALLS
 
-    def generate_standard(self, name: str, definition: list) -> str:
+    def set_debug(self) -> str:
         """
-        Public method used to generate NIM varaiable declaration.
-        The variable will be generated as a public object for external code usages.
-        A pointer to the variable will always be generated in the form of: P+NAME
-
-        Args:
-            name (str): Variable name
-            definition (list): Variable type from definitions.json
+        Public method used to generate the language specific code of DEBUG flag definition.
+        Is debug is not set it will erase the tag from template.
+        The debug definition code is then used to replace the SPT_DEBUG tag in template.
 
         Returns:
-            str: NIM code for variable definition (except type keyword for definition chaining)
+            str: Template content after modification
         """
-        result = f"{SysPlantConstants.NIM_TAB}{name}* = {definition[0]}\n"
-        # Always add pointer
-        result += f"{SysPlantConstants.NIM_TAB}P{name}* = ptr {name}\n"
-        return result
+        if self.logger.isDebug():
+            # Generate debug constant based on log level condition
+            debug_const = self.__coder.generate_debug(True)
+            self.replace_tag("SPT_DEBUG", debug_const)
+        else:
+            self.remove_tag("SPT_DEBUG")
+
+        return self.data
 
-    def generate_enum(self, name: str, definition: list) -> str:
+    def set_seed(self, seed: int = 0) -> str:
         """
-        Public method used to generate NIM enum declaration.
-        The enum structure will be generated as a public object for external code usages.
-        A pointer to the enum structure will always be generated in the form of: P+NAME
+        Public method used to generate the language specific code of SEED value definition.
+        The seed parameter is optional and if omitted it will be automatically generated with a random value.
+        The seed definition code is then used to replace the SPT_SEED tag in template.
 
         Args:
-            name (str): Enum structure name
-            definition (list): Enum structure entries from definitions.json
+            seed (int, optional): Seed value. Defaults to 0.
 
         Returns:
-            str: NIM code for enum structure (except type keyword for definition chaining)
+            str: Template content after modification
         """
-        result = f"{SysPlantConstants.NIM_TAB}{name}* " + "{.pure.} = enum\n"
-        for var in definition:
-            result += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}{var},\n"
-        # Always add pointer
-        result += f"{SysPlantConstants.NIM_TAB}P{name}* = ptr {name}\n"
+        if seed != 0:
+            self.__seed = seed
+
+        # Set SEED declaration
+        seed_code = self.__coder.generate_seed(self.__seed)
+        self.replace_tag("SPT_SEED", seed_code)
 
-        return result
+        return self.data
 
-    def generate_debug(self, debug: bool) -> str:
+    def set_iterator(self, name: str) -> str:
         """
-        Public method used to generate the SPT_DEBUG constant flag
+        Public method used to retrieve the language specific code of Syscall retrieval iterator.
+        The selected iterator is then used to replace the SPT_ITERATOR tag in template.
 
         Args:
-            debug (bool): Debug flag value
+            name (str): Iterator name to use
 
         Returns:
-            str: NIM code for template integration
+            str: Template content after modification
         """
-        return f"const SPT_DEBUG = {str(debug).lower()}"
+        # Get iterator template from package
+        data = self.__load_template(pkg_iterators, f"{name}.{self.__lang}")
+        self.replace_tag("SPT_ITERATOR", data)
+
+        return self.data
+
+    def set_method(self, name: str) -> str:
+        if name == "direct":
+            # Only Syscall number is required
+            resolver = self.__get_resolver("number")
+        elif name == "indirect":
+            # Only syscall address is required
+            resolver = self.__get_resolver("basic")
+        elif name == "random":
+            # Syscall number and instruction address are required
+            resolver = self.__get_resolver("number")
+            resolver += self.__get_resolver("random")
+        else:
+            raise NotImplementedError("Method not supported.")
+
+        # Set resolver code in template
+        self.replace_tag("SPT_RESOLVER", resolver)
+
+        # Load call stub
+        self.__set_caller(name)
+
+        # Set debug interruption on debug state
+        if self.logger.isDebug():
+            self.replace_tag("DEBUG_INT", "int 3")
+        else:
+            self.remove_tag("DEBUG_INT")
+
+        return self.data
 
-    def generate_seed(self, seed: int) -> str:
+    def __get_resolver(self, name: str) -> str:
         """
-        Public method used to generate the SPT_SEED constant value
+        Public method used to retrieve the language specific code of NtFunction resolver based on hash value.
+        The selected resolver is then used to replace the SPT_RESOLVER tag in template.
 
         Args:
-            seed (int): Seed value
+            name (str): Resolver name to use
 
         Returns:
-            str: NIM code for template integration
+            str: Template content after modification
         """
-        return f"const SPT_SEED = {hex(seed)}"
+        # Get resolver template from package
+        return self.__load_template(pkg_resolvers, f"{name}.{self.__lang}")
 
-    def generate_stub(self, name: str, params: dict, fhash: int) -> str:
+    def __set_caller(self, name: str) -> str:
         """
-        Public method used to generate stub code of syscall to hook
+        Public method used to retrieve the language specific code of the main call function.
+        The caller code is adapted with correct syscall instruction (using SYSCALL_INT tag)
+        The caller code embbed interuption (int 3) in case of DEBUG state (using DUBG_INT tag)
+        The selected caller is then used to replace the SPT_CALLER tag in template.
 
         Args:
-            name (str): NtFunction name to hook
-            params (dict): Parameters of functions defined in prototypes.json
-            fhash (int): NtFunction hash value used by ASM call
+            name (str): Caller name to use
+            resolver (str): Resolver name to use
 
         Returns:
-            str: NIM code for template integration
+            str: Template content after modification
         """
-        # Build function param declaration
-        stub = f"proc {name}*("
-        args = list()
+        # Get caller function from package
+        data = self.__load_template(pkg_stubs, f"{name}_{self.__arch}.{self.__lang}")
+        self.replace_tag("SPT_CALLER", data)
 
-        # Loop function params
-        for p in params.get("params", []):
-            # Register each type var
-            self.type_set.add(p["type"])
-            args.append(f"{p['name']}: {p['type']}")
+        # Adapt caller with proper options
+        self.replace_tag("SYSCALL_INT", self.__syscall)
 
-        # Generate NIM proc parameters
-        stub += ", ".join(args)
-        stub += ") {.asmNoStackFrame.} =\n"
+        return self.data
 
-        # Append stub code
-        stub += f'{SysPlantConstants.NIM_TAB}asm """\n'
-        stub += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}push dword ptr {hex(fhash)}\n"
-        stub += f"{SysPlantConstants.NIM_TAB}{SysPlantConstants.NIM_TAB}call `SPT_Syscall`\n"
-        stub += f'{SysPlantConstants.NIM_TAB}"""\n'
+    def __generate_definitions(self) -> str:
+        """
+        Private method used to generate the type definitions required by NtFunctions list specified to generate_stubs().
+        Generated code is then used to replace the TYPE_DEFINITIONS tag in template.
+
+        Returns:
+            str: Template content after modification
+        """
+        code = self.__coder.generate_definitions()
+        self.replace_tag("TYPE_DEFINITIONS", code)
 
-        return stub
+        return self.data
 
-    def __generate_typedefs(self, name: str, entry: dict) -> str:
+    def generate_stubs(self, names: list) -> str:
         """
-        Private method used to generate appropriate definition code based on entry type
+        Public method used to generate stubs for all the NtFunctions to hook.
+        Once generated a call is made to self.__generate_definitions() for automated type definitions.
+        Generated code is then used to replace the SPT_STUBS tag in template.
 
         Args:
-            name (str): Object name to define
-            entry (dict): Entry associated with requested name from definitions.json that gives details about the object to generate
+            names (list): List of NtFunctions to hook
 
         Raises:
-            NotImplementedError: Error raised if name is None
-            NotImplementedError: Error raised if entry type is not supported. Not in : structure|enum|union|pointer|standard
+            NotImplementedError: Error raised if NtFunction is not supported
 
         Returns:
-            str: NIM code for object declaration
+            str: Template content after modification
         """
-        typedef_code = ""
-        dependencies = entry.get("dependencies", [])
+        self.logger.debug(
+            f"\t. Hooking selected functions: {','.join(names)}", stripped=True
+        )
+        stubs_code = ""
 
-        # Resolve dependencies first
-        if len(dependencies) > 0:
-            for dep in dependencies:
-                # Avoid duplicate generation
-                if self.is_generated(dep):
-                    continue
-                # Avoid defining external types
-                if self.__definitions.get(dep) is not None:
-                    typedef_code += self.__generate_typedefs(
-                        dep, self.__definitions.get(dep)
-                    )
-
-        # Generate correct entry type
-        type_ = entry.get("type")
-        if type_ == "struct":
-            typedef_code += self.generate_struct(name, entry.get("definition", []))
-        elif type_ == "enum":
-            typedef_code += self.generate_enum(name, entry.get("definition", []))
-        elif type_ == "union":
-            typedef_code += self.generate_union(name, entry.get("definition", []))
-        elif type_ == "pointer":
-            typedef_code += self.generate_pointer(name, entry.get("definition", []))
-        elif type_ == "standard":
-            typedef_code += self.generate_standard(name, entry.get("definition", []))
-        elif type_ is None:
-            raise NotImplementedError(f"Missing {name} type")
-        else:
-            raise NotImplementedError("Unsupported definition type")
+        # Resolve all headers for functions to hook
+        for n in names:
+            params = self.__prototypes.get(n)
+            # Avoid unsupported functions
+            if params is None:
+                raise NotImplementedError(f"Unsupported syscall {n}")
 
-        # Register definitions generated
-        self.register_definition(name)
+            # Calculate function hash
+            fhash = self.get_function_hash(self.__seed, n)
 
-        return typedef_code
+            # Generate stub
+            stubs_code += self.__coder.generate_stub(n, params, fhash)
 
-    def generate_definitions(self) -> str:
-        """
-        Public method used to generate all required definitions by hooked syscall.
-        It will first loop through the required functions to hook, extract all parameters type to declare
-        and call the private __generate_typedefs function to generate the associated code block.
-        Once all chained it will return the complete code block to integrate in template
+        # Replace syscall stubs
+        self.replace_tag("SPT_STUBS", stubs_code)
 
-        Returns:
-            str: NIM code for template integration
-        """
-        code = ""
-        for name in self.type_set:
-            # If Winim already share this structure
-            if f"{name}*" in self.__winimdef:
-                continue
+        # Auto generate required definitions
+        self.__generate_definitions()
 
-            entry = self.__definitions.get(name)
+        return self.data
 
-            # Search pointer definition
-            if entry is None:
-                name = name[1:]
-                entry = self.__definitions.get(name)
+    def scramble(self) -> str:
+        """
+        Public method used to randomize fixed internal function names to avoid static analysis by EDR/AV.
+        Note: The concept behind this method is to let another project randomize the NtFunctions names as Sysplant as no view of the code using it.
 
-            # Still nothing... it might be a standard struct then
-            if entry is None:
-                continue
+        Returns:
+            str: Template content after modification
+        """
+        generated = set()
+        for name in SysPlantConstants.INTERNAL_FUNCTIONS:
+            randomized = self.generate_random_string(SysPlantConstants.RANDOM_WORD_SIZE)
+            # Avoid function collisions
+            while randomized in generated:
+                randomized = self.generate_random_string(
+                    SysPlantConstants.RANDOM_WORD_SIZE
+                )
 
-            # Avoid duplicate generation
-            if self.is_generated(name):
-                continue
+            # Store already set function name
+            generated.add(randomized)
 
-            code += self.__generate_typedefs(name, entry)
+            # Replace name in code
+            self.data = self.data.replace(name, randomized)
 
-        return code
+        return self.data
```

### Comparing `sysplant-0.2.1/sysplant/sysplant.py` & `sysplant-0.3.0/sysplant/sysplant.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         """
         # Init default vars
         self.logger = LoggerSingleton()
         self.__engine = TemplateManager(arch, syscall, language)
 
         # Init language
         self.__language = language
+        self.__arch = arch
 
     def list(self, search_path: str) -> set:
         results = set()
         # Get all supported functions
         patterns = self.__engine.list_supported_syscalls()
 
         if os.path.isdir(search_path):
@@ -63,56 +64,52 @@
                     # Check bot Nt and Zw versions
                     if (p in data) or ("Zw" + p[2:] in data):
                         results.add(p)
 
         return results
 
     def generate(
-        self, iterator: str, resolver: str, stub: str, syscalls: Union[str, list]
+        self, iterator: str, method: str, syscalls: Union[str, list]
     ) -> str:
         """
         Public method defining the generation algorithm. This method does not touch any code directly.
         It should only call TemplateManager methods in specific order.
         Modifications are let to TemplateManager class.
 
         Args:
             iterator (str): Iterator name to use (hell, halo, tartarus, freshy, syswhispers, canterlot)
-            resolver (str): Resolver name to use (basic, random)
-            stub (str): Stub type name to use (direct, indirect)
+            method (str): Stub type to use (direct, indirect, random)
             syscalls (Union[str, list]): NtFunctions list names to hook, or preset name (all|common|donut)
 
         Raises:
             ValueError: _description_
 
         Returns:
             str: Template content after generation
         """
         self.logger.info("Summary of params used")
         self.logger.debug(
             "\t. NOTE: DEBUG Interruption set in caller stub !", stripped=True
         )
         self.logger.info(f"\t. Language: {self.__language.upper()}", stripped=True)
+        self.logger.info(f"\t. Architecture: {self.__arch}", stripped=True)
 
         # Set debug flag
         self.__engine.set_debug()
 
         # Generate random seed
         self.__engine.set_seed()
 
         # Set iterator
         self.logger.info(f"\t. Selected syscall iterator: {iterator}", stripped=True)
         self.__engine.set_iterator(iterator)
 
-        # Set resolver
-        self.logger.info(f"\t. Selected syscall resolver: {resolver}", stripped=True)
-        self.__engine.set_resolver(resolver)
-
-        # Generate caller
-        self.logger.info(f"\t. Selected syscall caller stub: {stub}", stripped=True)
-        self.__engine.set_caller(stub, resolver)
+        # Generate stub call method
+        self.logger.info(f"\t. Selected syscall caller stub: {method}", stripped=True)
+        self.__engine.set_method(method)
 
         # Generate stubs
         if syscalls == "all":
             self.logger.info("\t. All supported functions selected", stripped=True)
             syscalls = self.__engine.list_supported_syscalls()
         elif syscalls == "common":
             self.logger.info("\t. Common supported functions selected", stripped=True)
@@ -152,18 +149,23 @@
 
         Args:
             output_path (str): Filename where to write generated code
 
         Returns:
             str: Template content
         """
+        # Set extension
+        ext = None
+        if self.__language == "nim":
+            ext = "nim"
+        elif self.__language == "c":
+            ext = "h"
+
         # Write file
         clean_path = (
-            output_path
-            if output_path.endswith(f".{self.__language}")
-            else f"{output_path}.{self.__language}"
+            output_path if output_path.endswith(f".{ext}") else f"{output_path}.{ext}"
         )
         with open(clean_path, "w") as o:
             o.write(str(self.__engine))
             self.logger.info(f"Syscall file written to {clean_path}")
 
         return str(self.__engine)
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/canterlot.nim` & `sysplant-0.3.0/sysplant/templates/iterators/canterlot.nim`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # Use RunTime Function table from exception directory to gather SSN: https://www.mdsec.co.uk/2022/04/resolving-system-service-numbers-using-the-exception-directory/
-# Auto calculate syscall offset
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, DWORD, PBYTE) =
     var
         i: int = 0
-        ssn: int = 0
+        ssn: DWORD = 0
     
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
     let exports = codeBase{directory.VirtualAddress}[PIMAGE_EXPORT_DIRECTORY]
     
     # Get runtime functions table
     let dirExcept = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXCEPTION]
     let rtf = codeBase{dirExcept.VirtualAddress}[PIMAGE_RUNTIME_FUNCTION_ENTRY] 
     
-    var padding = 0x0
-
     # Loop runtime function table
     while rtf[i].BeginAddress:
         let current = rtf[i].BeginAddress
         # Reset pointers
         var
             nameRef = codeBase{exports.AddressOfNames}[PDWORD]
             funcRef = codeBase{exports.AddressOfFunctions}[PDWORD]
@@ -34,22 +31,16 @@
             let
                 name = $(codeBase{nameRef[]}[LPCSTR])
                 offset = funcRef[ordinal[j][int]]
                 address = codeBase{offset}[PBYTE]
             
             # Check offset with current function, ensure this is a syscall
             if (offset == current) and name.startsWith("Zw"):
-                let hash = SPT_HashSyscallName(name)
-                # All syscall stub are identical for a Windows version
-                if padding == 0x0:
-                    # Calculate jmp address avoiding EDR hooks
-                    while (address{padding}[] != 0x0f) and (address{padding + 1}[] != 0x05):
-                        padding += 1
-                
-                yield (hash, ssn, address{padding}[int64])
+                let hash: int32 = SPT_HashSyscallName(name)
+                yield (hash, ssn, address)
                 # Increase syscall number
                 ssn += 1
                 break
 
             ++nameRef
 
         # Go next address
@@ -81,13 +72,18 @@
     while hModule.Module32Next(addr me32):
         # Detect \ntdll.dll
         if "92110116100108108461001081080" in me32.szExePath.join():
             break
     
     handle.GetModuleInformation(me32.hModule, addr mi, cast[DWORD](sizeof(mi)))
     
+    var padding = 0x0
     # Resolve ssn & address
     for hash, ssn, address in mi.SPT_Iterator():
-        var entry = Syscall(ssn: ssn, address: address)
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+        
+        var entry = Syscall(ssn: ssn, address: address[PVOID], syscallAddress: address{padding}[PVOID])
         ssdt[hash] = entry
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/freshy.nim` & `sysplant-0.3.0/sysplant/templates/iterators/freshy.nim`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Parse Export Directory and lookup syscall by name (start with Nt and not Ntdll), sort addresses to retrieve syscall number https://github.com/crummie5/FreshyCalls
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -15,20 +15,21 @@
         ordinal = codeBase{exports.AddressOfNameOrdinals}[PWORD]
     
     # Search Begin Address in Export Table
     for j in 0 ..< exports.NumberOfFunctions:
         let
             name = $(codeBase{nameRef[]}[LPCSTR])
             offset = funcRef[ordinal[j][int]]
-        
+            address = codeBase{offset}[PBYTE]
+
         # Check offset with current function, ensure this is a syscall
         if name.startsWith("Nt") and not name.startsWith("Ntdll"):
-            let hash = SPT_HashSyscallName(name)
+            let hash: int32 = SPT_HashSyscallName(name)
             # Calculate jmp address avoiding EDR hooks
-            yield (hash, codeBase{offset + 0xb2}[int64])
+            yield (hash, address)
             
         ++nameRef
 
 proc SPT_PopulateSyscalls =
     # Return short when work is already done
     if len(ssdt) > 0:
         return
@@ -40,16 +41,16 @@
     let hModule = CreateToolhelp32Snapshot(TH32CS_SNAPMODULE, pid)
     defer: CloseHandle(hModule)
 
     # Store process handle
     let handle = OpenProcess(PROCESS_ALL_ACCESS, FALSE, pid)
 
     type Entry = tuple
-        address: int64
-        hash: DWORD
+        address: PBYTE
+        hash: int32
     
     var
         me32: MODULEENTRY32
         mi: MODULEINFO
         tmp: seq[Entry]
     
     me32.dwSize = cast[DWORD](sizeof(MODULEENTRY32))
@@ -67,15 +68,21 @@
     # Resolve address
     for hash, address in mi.SPT_Iterator():
         tmp.add((address, hash))
     
     # Sort syscalls by address
     tmp.sort(system.cmp)
 
+    var padding = 0x0
     # Register syscalls
     for i in 0 ..< len(tmp):
         let
             address = tmp[i][0]
             hash = tmp[i][1]
-        ssdt[hash] = Syscall(address: address, ssn: i)
+        
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: i[int32], syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/halo.nim` & `sysplant-0.3.0/sysplant/templates/iterators/halo.nim`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     let
         high_b = address{cw + 5 + gap}[]
         low_b = address{cw + 4 + gap}[]
     
     return (high_b shl 8).bitor(low_b)[int32] - step[int32]
 
 # Parse Export Directory and lookup syscall for 1st opcodes, check up and down if hooked (unable to found initial implementation...)
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int32, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, DWORD, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -78,18 +78,18 @@
                     # Check previous syscall is Clean (UP)
                     ssn = address.isClean(cw, -i)
                     if ssn > -1:
                         break
             
             if ssn > -1:
                 let
-                    hash = SPT_HashSyscallName(name)
-                    found = address{cw}[int64]
+                    hash: int32 = SPT_HashSyscallName(name)
+                    found: PBYTE = address{cw}[PBYTE]
                 
-                yield (hash, ssn, found)
+                yield (hash, ssn[DWORD], found)
                 break
             
             cw += 1
     
         ++nameRef
 
 proc SPT_PopulateSyscalls =
@@ -119,12 +119,17 @@
     while hModule.Module32Next(addr me32):
         # Detect \ntdll.dll
         if "92110116100108108461001081080" in me32.szExePath.join():
             break
     
     handle.GetModuleInformation(me32.hModule, addr mi, cast[DWORD](sizeof(mi)))
 
+    var padding = 0x0
     # Resolve address
     for hash, ssn, address in mi.SPT_Iterator():
-        ssdt[hash] = Syscall(address: address, ssn: ssn)
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: ssn, syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/hell.nim` & `sysplant-0.3.0/sysplant/templates/iterators/hell.nim`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         if value == 0xff:
             continue
         if address{cw + i}[] != value:
             return false
     return true
 
 # Parse Export Directory and look for opcode scheme: https://github.com/am0nsec/HellsGate/blob/master/HellsGate/main.c
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int32, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, DWORD, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -43,24 +43,24 @@
 
             # check if ret, in this case we are also probaly too far
             if address{cw}[] == 0xc3:
                 break
 
             if address.isClean(cw):
                 let
-                    hash = SPT_HashSyscallName(name)
-                    found = address{cw}[int64]
+                    hash: int32 = SPT_HashSyscallName(name)
+                    found: PBYTE = address{cw}[PBYTE]
                     
                 # Retrieve the SSN taking care of the endianess 
                 let
                     high_b = address{cw + 5}[]
                     low_b = address{cw + 4}[]
                     ssn: int32 = (high_b shl 8).bitor(low_b)[int32]
                 
-                yield (hash, ssn, found)
+                yield (hash, ssn[DWORD], found)
                 break
             
             cw += 1
     
         ++nameRef
 
 proc SPT_PopulateSyscalls =
@@ -90,12 +90,17 @@
     while hModule.Module32Next(addr me32):
         # Detect \ntdll.dll
         if "92110116100108108461001081080" in me32.szExePath.join():
             break
     
     handle.GetModuleInformation(me32.hModule, addr mi, cast[DWORD](sizeof(mi)))
 
+    var padding = 0x0
     # Resolve address
     for hash, ssn, address in mi.SPT_Iterator():
-        ssdt[hash] = Syscall(address: address, ssn: ssn)
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: ssn, syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/syswhispers.nim` & `sysplant-0.3.0/sysplant/templates/iterators/syswhispers.nim`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Lookup from Export directory Nt function (and not Ntdll), and sort them by addresses to get corresponding syscall number
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -15,19 +15,20 @@
         ordinal = codeBase{exports.AddressOfNameOrdinals}[PWORD]
     
     # Search Begin Address in Export Table
     for j in 0 ..< exports.NumberOfFunctions:
         let
             name = $(codeBase{nameRef[]}[LPCSTR])
             offset = funcRef[ordinal[j][int]]
+            address = codeBase{offset}[PBYTE]
         
         # Check offset with current function, ensure this is a syscall
         if name.startsWith("Zw"):
-            let hash = SPT_HashSyscallName(name)
-            yield (hash, codeBase{offset}[int64])
+            let hash: int32 = SPT_HashSyscallName(name)
+            yield (hash, address)
             
         ++nameRef
 
 proc SPT_PopulateSyscalls =
     # Return short when work is already done
     if len(ssdt) > 0:
         return
@@ -39,16 +40,16 @@
     let hModule = CreateToolhelp32Snapshot(TH32CS_SNAPMODULE, pid)
     defer: CloseHandle(hModule)
 
     # Store process handle
     let handle = OpenProcess(PROCESS_ALL_ACCESS, FALSE, pid)
 
     type Entry = tuple
-        address: int64
-        hash: DWORD
+        address: PBYTE
+        hash: int32
     
     var
         me32: MODULEENTRY32
         mi: MODULEINFO
         tmp: seq[Entry]
     
     me32.dwSize = cast[DWORD](sizeof(MODULEENTRY32))
@@ -66,15 +67,21 @@
     # Resolve address
     for hash, address in mi.SPT_Iterator():
         tmp.add((address, hash))
     
     # Sort syscalls by address
     tmp.sort(system.cmp)
 
+    var padding = 0x0
     # Register syscalls
     for i in 0 ..< len(tmp):
         let
             address = tmp[i][0]
             hash = tmp[i][1]
-        ssdt[hash] = Syscall(address: address, ssn: i)
+        
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: i[int32], syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/syswhispers3.nim` & `sysplant-0.3.0/sysplant/templates/iterators/syswhispers3.nim`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,9 @@
-var distance_to_syscall: ULONG
-when defined(amd64):
-    # If the process is 64-bit on a 64-bit OS, we need to search for syscall
-    distance_to_syscall = 0x12
-elif defined(i386):
-    # If the process is 32-bit on a 32-bit OS, we need to search for sysenter
-    distance_to_syscall = 0x0f
-
 # Lookup from Export directory Nt function (and not Ntdll), and sort them by addresses to get corresponding syscall number
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -23,19 +15,20 @@
         ordinal = codeBase{exports.AddressOfNameOrdinals}[PWORD]
     
     # Search Begin Address in Export Table
     for j in 0 ..< exports.NumberOfFunctions:
         let
             name = $(codeBase{nameRef[]}[LPCSTR])
             offset = funcRef[ordinal[j][int]]
+            address = codeBase{offset}[PBYTE]
         
         # Check offset with current function, ensure this is a syscall
         if name.startsWith("Zw"):
-            let hash = SPT_HashSyscallName(name)
-            yield (hash, codeBase{offset + distance_to_syscall}[int64])
+            let hash: int32 = SPT_HashSyscallName(name)
+            yield (hash, address)
             
         ++nameRef
 
 proc SPT_PopulateSyscalls =
     # Return short when work is already done
     if len(ssdt) > 0:
         return
@@ -47,16 +40,16 @@
     let hModule = CreateToolhelp32Snapshot(TH32CS_SNAPMODULE, pid)
     defer: CloseHandle(hModule)
 
     # Store process handle
     let handle = OpenProcess(PROCESS_ALL_ACCESS, FALSE, pid)
 
     type Entry = tuple
-        address: int64
-        hash: DWORD
+        address: PBYTE
+        hash: int32
     
     var
         me32: MODULEENTRY32
         mi: MODULEINFO
         tmp: seq[Entry]
     
     me32.dwSize = cast[DWORD](sizeof(MODULEENTRY32))
@@ -74,15 +67,21 @@
     # Resolve address
     for hash, address in mi.SPT_Iterator():
         tmp.add((address, hash))
     
     # Sort syscalls by address
     tmp.sort(system.cmp)
 
+    var padding = 0x0
     # Register syscalls
     for i in 0 ..< len(tmp):
         let
             address = tmp[i][0]
             hash = tmp[i][1]
-        ssdt[hash] = Syscall(address: address, ssn: i)
+        
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: i[int32], syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/iterators/tartarus.nim` & `sysplant-0.3.0/sysplant/templates/iterators/tartarus.nim`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     let
         high_b = address{cw + 5 + gap}[]
         low_b = address{cw + 4 + gap}[]
     
     return (high_b shl 8).bitor(low_b)[int32] - step[int32]
     
 # Parse Export Directory and look for 1st & 3rd opcodes, check up and down if hooked https://github.com/trickster0/TartarusGate
-iterator SPT_Iterator(mi: MODULEINFO): (DWORD, int32, int64) =
+iterator SPT_Iterator(mi: MODULEINFO): (int32, DWORD, PBYTE) =
     # Extract headers
     let codeBase = mi.lpBaseOfDll
     let dosHeader = cast[PIMAGE_DOS_HEADER](codeBase)
     let ntHeader = cast[PIMAGE_NT_HEADERS](cast[DWORD_PTR](codeBase) + dosHeader.e_lfanew)
     
     # Get export table
     let directory = ntHeader.OptionalHeader.DataDirectory[IMAGE_DIRECTORY_ENTRY_EXPORT]
@@ -78,18 +78,18 @@
                     # Check previous syscall is Clean (UP)
                     ssn = address.isClean(cw, -i)
                     if ssn > -1:
                         break
                     
             if ssn > -1:
                 let
-                    hash = SPT_HashSyscallName(name)
-                    found = address{cw}[int64]
+                    hash: int32 = SPT_HashSyscallName(name)
+                    found: PBYTE = address{cw}[PBYTE]
                 
-                yield (hash, ssn, found)
+                yield (hash, ssn[DWORD], found)
                 break
             
             cw += 1
     
         ++nameRef
 
 proc SPT_PopulateSyscalls =
@@ -119,12 +119,17 @@
     while hModule.Module32Next(addr me32):
         # Detect \ntdll.dll
         if "92110116100108108461001081080" in me32.szExePath.join():
             break
     
     handle.GetModuleInformation(me32.hModule, addr mi, cast[DWORD](sizeof(mi)))
 
+    var padding = 0x0
     # Resolve address
     for hash, ssn, address in mi.SPT_Iterator():
-        ssdt[hash] = Syscall(address: address, ssn: ssn)
+        # All syscall stub are identical for a Windows version
+        if padding == 0x0:
+            padding = SPT_DetectPadding(address)
+
+        ssdt[hash] = Syscall(address: address[PVOID], ssn: ssn, syscallAddress: address{padding}[PVOID])
 
     return
```

### Comparing `sysplant-0.2.1/sysplant/templates/stubs/indirect_x64.nim` & `sysplant-0.3.0/sysplant/templates/stubs/random_x64.nim`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 proc SPT_Syscall {.asmNoStackFrame.} = 
     asm """
         pop rax
-        pop rax
+        pop r15
         mov [rsp +8], rcx
         mov [rsp+16], rdx
         mov [rsp+24], r8
         mov [rsp+32], r9
         sub rsp, 0x28
-        mov rcx, rax
+        mov rcx, r15
         ##__DEBUG_INT__##
         call `SPT_GetSyscallNumber`
+        mov rcx, r15
         mov r15, rax
-        call `##__FUNCTION_RESOLVE__##`
+        call `SPT_GetRandomSyscallAddress`
         xchg r15, rax
         add rsp, 0x28
         mov rcx, [rsp +8]
         mov rdx, [rsp+16]
         mov r8, [rsp+24]
         mov r9, [rsp+32]
         mov r10, rcx
```

### Comparing `sysplant-0.2.1/sysplant/utils/loggerSingleton.py` & `sysplant-0.3.0/sysplant/utils/loggerSingleton.py`

 * *Files identical despite different names*

