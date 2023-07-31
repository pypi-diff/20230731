# Comparing `tmp/pytch-fetch-1.2.0.tar.gz` & `tmp/pytch-fetch-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytch-fetch-1.2.0.tar", last modified: Sun Jul 30 05:23:38 2023, max compression
+gzip compressed data, was "pytch-fetch-1.2.1.tar", last modified: Mon Jul 31 06:40:18 2023, max compression
```

## Comparing `pytch-fetch-1.2.0.tar` & `pytch-fetch-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/
--rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.2.0/LICENSE
--rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)     1825 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/README.md
--rw-r--r--   0 krit      (1000) krit      (1001)     1374 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/pyproject.toml
--rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/setup.cfg
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.022762 pytch-fetch-1.2.0/src/
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.023762 pytch-fetch-1.2.0/src/pytch/
--rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.2.0/src/pytch/__init__.py
--rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/__main__.py
--rw-r--r--   0 krit      (1000) krit      (1001)    21693 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/art.py
--rw-r--r--   0 krit      (1000) krit      (1001)     6733 2023-07-30 05:22:13.000000 pytch-fetch-1.2.0/src/pytch/funcs.py
-drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-30 05:23:38.025762 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/
--rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/PKG-INFO
--rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/entry_points.txt
--rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-30 05:23:38.000000 pytch-fetch-1.2.0/src/pytch_fetch.egg-info/top_level.txt
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/
+-rw-r--r--   0 krit      (1000) krit      (1001)     1066 2023-07-24 09:11:38.000000 pytch-fetch-1.2.1/LICENSE
+-rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)     1825 2023-07-30 05:22:13.000000 pytch-fetch-1.2.1/README.md
+-rw-r--r--   0 krit      (1000) krit      (1001)     1374 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/pyproject.toml
+-rw-r--r--   0 krit      (1000) krit      (1001)       38 2023-07-31 06:40:18.675104 pytch-fetch-1.2.1/setup.cfg
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.672104 pytch-fetch-1.2.1/src/
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.673104 pytch-fetch-1.2.1/src/pytch/
+-rw-r--r--   0 krit      (1000) krit      (1001)        0 2023-07-24 09:11:38.000000 pytch-fetch-1.2.1/src/pytch/__init__.py
+-rwxr-xr-x   0 krit      (1000) krit      (1001)     3505 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/__main__.py
+-rw-r--r--   0 krit      (1000) krit      (1001)    22608 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/art.py
+-rw-r--r--   0 krit      (1000) krit      (1001)     6756 2023-07-31 06:40:06.000000 pytch-fetch-1.2.1/src/pytch/funcs.py
+drwxr-xr-x   0 krit      (1000) krit      (1001)        0 2023-07-31 06:40:18.674104 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/
+-rw-r--r--   0 krit      (1000) krit      (1001)     4356 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/PKG-INFO
+-rw-r--r--   0 krit      (1000) krit      (1001)      310 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/SOURCES.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        1 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/dependency_links.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)       46 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/entry_points.txt
+-rw-r--r--   0 krit      (1000) krit      (1001)        6 2023-07-31 06:40:18.000000 pytch-fetch-1.2.1/src/pytch_fetch.egg-info/top_level.txt
```

### Comparing `pytch-fetch-1.2.0/LICENSE` & `pytch-fetch-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.2.0/PKG-INFO` & `pytch-fetch-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
```

### Comparing `pytch-fetch-1.2.0/README.md` & `pytch-fetch-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pytch-fetch-1.2.0/pyproject.toml` & `pytch-fetch-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytch-fetch"
-version = "1.2.0"
+version = "1.2.1"
 description="Pytch Yields Technical Characteristics Hastily"
 readme = "README.md"
 authors = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 maintainers = [{ name = "Krit Dass", email = "dasskrit@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `pytch-fetch-1.2.0/src/pytch/__main__.py` & `pytch-fetch-1.2.1/src/pytch/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "-l",
         "--logo",
         metavar="DISTRO",
         dest="logo",
         help="use an alternate distribution's logo",
     )
 
-    parser.add_argument("-v", "--version", action="version", version="1.2.0")
+    parser.add_argument("-v", "--version", action="version", version="1.2.1")
 
     args = parser.parse_args()
 
     attrs = [
         {"name": "user", "value": getlogin(), "icon": "", "color": "red"},
         {
             "name": "os",
```

### Comparing `pytch-fetch-1.2.0/src/pytch/art.py` & `pytch-fetch-1.2.1/src/pytch/art.py`

 * *Files 2% similar despite different names*

```diff
@@ -564,8 +564,33 @@
 ${c2}   .-                        ${c1}-.
 ${c2}    --                      ${c1}-.
 ${c2}     `:`                  ${c1}`:`
        .--             `--.
           .---.....----.
         """,
     },
+    "nobara linux": {
+        "colors": ["cyan"],
+        "ascii": r"""
+${c1}MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
+MMMMMN0kkOXWMWNK0OkkkkO0KNWMMMMMMMMMMMMM
+MMMNx,.   .:l:'.        .':okXMMMMMMMMMM
+MMWx.                        'l0WMMMMMMM
+MMWl                           .cKMMMMMM
+MMWl                             'kWMMMM
+MMWl            .;:cc:;.          .kWMMM
+MMWl          ,xXWWNNWWXx,         ,KMMM
+MMWl         :KMKo,'',oKMX:        .dWMM
+MMWl        .kMNc      cNMNOd:.     lWMM
+MMWl        .kMWx.    .xWMKl,.      lWMM
+MMWl        .xWMWKkddkKWMMO.        lWMM
+MMWl         .oOKXNMMMMMMMO.        lWMM
+MMWl            ..,oOXMMMMO.        lWMM
+MMWl                 :XMMMO.        lWMM
+MMWo         .';:;.  .OMMMO.        oWMM
+MMM0;      .cONWMWXxccOMMMNl.      ;0MMM
+MMMMXxc;;;lONMMMMMMWWNNMMMMWOl;,;cxXMMMM
+MMMMMMMWWWMMMMMMMMMMMMMMMMMMMMWWWMMMMMMM
+MMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMMM
+        """
+    }
 }
```

### Comparing `pytch-fetch-1.2.0/src/pytch/funcs.py` & `pytch-fetch-1.2.1/src/pytch/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,14 +175,15 @@
     elif name in [
         "Fedora",
         "CentOS",
         "SUSE",
         "openSUSE Tumbleweed",
         "openSUSE Leap",
         "RHEL",
+        "Nobara Linux"
     ]:
         packages.append(f"{get_lines('rpm -qa')} (rpm)")
     elif name == "Void":
         packages.append(f"{get_lines('xbps-query -l')} (xbps)")
     elif name in ["Gentoo", "ChromeOS"]:
         packages.append(f"{get_lines('ls -d /var/db/pkg/*/*| cut -f5- -d/')} (portage)")
     elif name == "NixOS":
```

### Comparing `pytch-fetch-1.2.0/src/pytch_fetch.egg-info/PKG-INFO` & `pytch-fetch-1.2.1/src/pytch_fetch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytch-fetch
-Version: 1.2.0
+Version: 1.2.1
 Summary: Pytch Yields Technical Characteristics Hastily
 Author-email: Krit Dass <dasskrit@gmail.com>
 Maintainer-email: Krit Dass <dasskrit@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Krit Dass
```

