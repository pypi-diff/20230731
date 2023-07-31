# Comparing `tmp/memsparkline-0.3.0.tar.gz` & `tmp/memsparkline-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memsparkline-0.3.0.tar", max compression
+gzip compressed data, was "memsparkline-0.3.1.tar", max compression
```

## Comparing `memsparkline-0.3.0.tar` & `memsparkline-0.3.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4570 2023-07-30 10:25:52.039993 memsparkline-0.3.0/README.md
--rwxr-xr-x   0        0        0     7753 2023-07-29 21:22:56.957256 memsparkline-0.3.0/memsparkline.py
--rw-r--r--   0        0        0     1044 2023-07-30 10:23:20.070760 memsparkline-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 memsparkline-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4623 2023-07-30 12:45:20.428228 memsparkline-0.3.1/README.md
+-rwxr-xr-x   0        0        0     7768 2023-07-31 19:20:08.488276 memsparkline-0.3.1/memsparkline.py
+-rw-r--r--   0        0        0     1044 2023-07-31 18:51:30.171773 memsparkline-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5772 1970-01-01 00:00:00.000000 memsparkline-0.3.1/PKG-INFO
```

### Comparing `memsparkline-0.3.0/README.md` & `memsparkline-0.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 ## Installation
 
 memsparkline requires Python 3.7 or later.
 
 ### Installing from PyPI
 
-The recommended way to install memsparkline is with [pipx](https://github.com/pypa/pipx).
+The recommended way to install memsparkline is from [PyPI](https://pypi.org/project/memsparkline/) with [pipx](https://github.com/pypa/pipx).
 
 ```sh
 pipx install memsparkline
 ```
 
 You can also use pip:
 
@@ -70,15 +70,15 @@
 ```
 
 #### Dependencies
 
 ##### Debian/Ubuntu
 
 ```sh
-sudo apt install python3-psuti
+sudo apt install python3-psutil
 ```
 
 ##### DragonFly BSD 6.6, FreeBSD 13.1
 
 ```sh
 sudo pkg install py39-psutil
 ```
```

### Comparing `memsparkline-0.3.0/memsparkline.py` & `memsparkline-0.3.1/memsparkline.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import time
 from typing import Iterator, IO, List, Tuple
 
 import psutil
 
 SPARKLINE_TICKS = ["▁", "▂", "▃", "▄", "▅", "▆", "▇", "█"]
 USAGE_DIVISOR = 1 << 20
-VERSION = "0.3.0"
+VERSION = "0.3.1"
 
 
 def main() -> None:
     args = cli(sys.argv)
 
     with open_output(args.output_path, sys.stderr) as output:  # type: IO[str]
         try:
@@ -129,15 +129,15 @@
         help="command to run",
     )
     parser.add_argument(
         "arguments",
         default=[],
         help="arguments to command",
         metavar="arg",
-        nargs="*",
+        nargs=argparse.REMAINDER,
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version=VERSION,
     )
```

### Comparing `memsparkline-0.3.0/pyproject.toml` & `memsparkline-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memsparkline"
-version = "0.3.0"
+version = "0.3.1"
 description = "Track the RAM usage (resident set size) of a process and its descendants in real time."
 authors = ["D. Bohdan <dbohdan@dbohdan.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.com/dbohdan/memsparkline"
 keywords = ["memory", "monitoring", "performance", "RAM", "resident set size", "sparklines"]
 classifiers = [
```

### Comparing `memsparkline-0.3.0/PKG-INFO` & `memsparkline-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memsparkline
-Version: 0.3.0
+Version: 0.3.1
 Summary: Track the RAM usage (resident set size) of a process and its descendants in real time.
 Home-page: https://gitlab.com/dbohdan/memsparkline
 License: MIT
 Keywords: memory,monitoring,performance,RAM,resident set size,sparklines
 Author: D. Bohdan
 Author-email: dbohdan@dbohdan.com
 Requires-Python: >=3.7,<4.0
@@ -70,15 +70,15 @@
 
 ## Installation
 
 memsparkline requires Python 3.7 or later.
 
 ### Installing from PyPI
 
-The recommended way to install memsparkline is with [pipx](https://github.com/pypa/pipx).
+The recommended way to install memsparkline is from [PyPI](https://pypi.org/project/memsparkline/) with [pipx](https://github.com/pypa/pipx).
 
 ```sh
 pipx install memsparkline
 ```
 
 You can also use pip:
 
@@ -98,15 +98,15 @@
 ```
 
 #### Dependencies
 
 ##### Debian/Ubuntu
 
 ```sh
-sudo apt install python3-psuti
+sudo apt install python3-psutil
 ```
 
 ##### DragonFly BSD 6.6, FreeBSD 13.1
 
 ```sh
 sudo pkg install py39-psutil
 ```
```

