# Comparing `tmp/pytch-fetch-1.2.1.tar.gz` & `tmp/pytch-fetch-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.2.1.tar", last modified: Mon Jul 31 06:40:18 2023, max compression
+gzip compressed data, was "pytch-fetch-1.2.2.tar", last modified: Mon Jul 31 07:58:26 2023, max compression
```

## Comparing `pytch-fetch-1.2.1.tar` & `pytch-fetch-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.2.1/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1825 2023-07-30 05:22:13.000000 pytch-fetch-1.2.1/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1374 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.672104 pytch-fetch-1.2.1/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.673104 pytch-fetch-1.2.1/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.2.1/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    22608 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     6756 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.674104 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 07:58:26.039164 pytch-fetch-1.2.2/
+-rw-r--r--   0 krit      (1000) krit      (1001)    34893 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/LICENSE.md
+-rw-r--r--   0 krit      (1000) krit      (1001)    43726 2023-07-31 07:58:26.038164 pytch-fetch-1.2.2/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     2107 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1403 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-31 07:58:26.039164 pytch-fetch-1.2.2/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 07:58:26.034165 pytch-fetch-1.2.2/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 07:58:26.035164 pytch-fetch-1.2.2/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.2.2/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    22610 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     6783 2023-07-31 07:56:50.000000 pytch-fetch-1.2.2/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 07:58:26.038164 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)    43726 2023-07-31 07:58:26.000000 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      313 2023-07-31 07:58:26.000000 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-31 07:58:26.000000 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-31 07:58:26.000000 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-31 07:58:26.000000 pytch-fetch-1.2.2/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.2.1/pyproject.toml` & `pytch-fetch-1.2.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.2.1"
+version = "1.2.2"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
-license = { file = "LICENSE" }
+license = { file = "LICENSE.md" }
 classifiers = [
   "Development Status :: 4 - Beta",
-  "License :: OSI Approved :: MIT License",
+  "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Natural Language :: English",
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: BSD :: FreeBSD",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.7",
```

### Comparing `pytch-fetch-1.2.1/src/pytch/__main__.py` & `pytch-fetch-1.2.2/src/pytch/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="1.2.1")
+    parser.add_argument("-v", "--version", action="version", version="1.2.2")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
         {
             "name": "os",
```

### Comparing `pytch-fetch-1.2.1/src/pytch/art.py` & `pytch-fetch-1.2.2/src/pytch/art.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,10 +587,10 @@
 MMWl            ..,oOXMMMMO.        lWMM
 MMWl                 :XMMMO.        lWMM
 MMWo         .';:;.  .OMMMO.        oWMM
 MMM0;      .cONWMWXxccOMMMNl.      ;0MMM
 MMMMXxc;;;lONMMMMMMWWNNMMMMWOl;,;cxXMMMM
 MMMMMMMWWWMMMMMMMMMMMMMMMMMMMMWWWMMMMMMM
 MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
-        """
-    }
+        """,
+    },
 }
```

### Comparing `pytch-fetch-1.2.1/src/pytch/funcs.py` & `pytch-fetch-1.2.2/src/pytch/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from os.path import isfile
 from platform import release
 from sys import platform
 from subprocess import check_output, DEVNULL, CalledProcessError
 from re import search, findall, sub, split
 from pytch.art import art_dict
 
+
 def get_output(cmd):
     return check_output([cmd], shell=True, text=True, stderr=DEVNULL)
 
 
 def color(text, color):
     colors = {
         "black": 90,
@@ -136,25 +137,28 @@
             mem[line.split(":")[0]] = int(float(line.split(":")[1].strip()))
         mem_available = (
             mem["Pages wired down"] + mem["Pages active"] + mem["Pages inactive"]
         ) * int(page_size)
     elif get_name() == "FreeBSD":
         mem_total = int(get_output("sysctl -n hw.physmem")) / 1024
         page_size = int(get_output("sysctl -n hw.pagesize"))
-        mem_available = int(get_output("sysctl -n vm.stats.vm.v_free_count")) * page_size / 1024
+        mem_available = (
+            int(get_output("sysctl -n vm.stats.vm.v_free_count")) * page_size / 1024
+        )
     else:
         with open("/proc/meminfo", "r") as mem_file:
             for pair in mem_file.read().splitlines():
                 if pair.split(":")[0] == "MemTotal":
                     mem_total = pair.split(":")[1].replace("kB", "").strip()
                 elif pair.split(":")[0] == "MemAvailable":
                     mem_available = pair.split(":")[1].replace("kB", "").strip()
 
     return f"{int((int(mem_total) - int(mem_available)) * 100 / int(mem_total))}%"
 
+
 def get_packages():
     def get_lines(cmd):
         packages = get_output(cmd)
         num_pkgs = len(packages.splitlines())
         return str(num_pkgs)
 
     packages = []
@@ -175,15 +179,15 @@
     elif name in [
         "Fedora",
         "CentOS",
         "SUSE",
         "openSUSE Tumbleweed",
         "openSUSE Leap",
         "RHEL",
-        "Nobara Linux"
+        "Nobara Linux",
     ]:
         packages.append(f"{get_lines('rpm -qa')} (rpm)")
     elif name == "Void":
         packages.append(f"{get_lines('xbps-query -l')} (xbps)")
     elif name in ["Gentoo", "ChromeOS"]:
         packages.append(f"{get_lines('ls -d /var/db/pkg/*/*| cut -f5- -d/')} (portage)")
     elif name == "NixOS":
```

