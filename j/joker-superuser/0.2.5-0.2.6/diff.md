# Comparing `tmp/joker-superuser-0.2.5.tar.gz` & `tmp/joker-superuser-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joker-superuser-0.2.5.tar", last modified: Wed May 18 12:30:17 2022, max compression
+gzip compressed data, was "joker-superuser-0.2.6.tar", last modified: Mon Jul 31 08:29:27 2023, max compression
```

## Comparing `joker-superuser-0.2.5.tar` & `joker-superuser-0.2.6.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.403764 joker-superuser-0.2.5/
--rw-r--r--   0 Hailong    (502) staff       (20)       88 2021-09-11 09:03:34.000000 joker-superuser-0.2.5/MANIFEST.in
--rw-r--r--   0 Hailong    (502) staff       (20)     1220 2022-05-18 12:30:17.403365 joker-superuser-0.2.5/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)      533 2022-05-18 12:29:30.000000 joker-superuser-0.2.5/README.md
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.376114 joker-superuser-0.2.5/joker/
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.381455 joker-superuser-0.2.5/joker/superuser/
--rw-r--r--   0 Hailong    (502) staff       (20)       73 2022-05-18 12:29:39.000000 joker-superuser-0.2.5/joker/superuser/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)      724 2022-05-18 12:23:44.000000 joker-superuser-0.2.5/joker/superuser/__main__.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.383840 joker-superuser-0.2.5/joker/superuser/asset/
--rw-r--r--   0 Hailong    (502) staff       (20)      718 2021-09-19 15:17:43.000000 joker-superuser-0.2.5/joker/superuser/asset/gitignore.txt
--rw-r--r--   0 Hailong    (502) staff       (20)     2536 2021-07-03 06:34:49.000000 joker-superuser-0.2.5/joker/superuser/asset/setup.txt
--rw-r--r--   0 Hailong    (502) staff       (20)      287 2019-07-30 02:44:18.000000 joker-superuser-0.2.5/joker/superuser/asset/simple.yml
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.385595 joker-superuser-0.2.5/joker/superuser/cli/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2022-05-17 14:47:03.000000 joker-superuser-0.2.5/joker/superuser/cli/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)      575 2022-05-18 12:22:44.000000 joker-superuser-0.2.5/joker/superuser/cli/chksumdirs.py
--rw-r--r--   0 Hailong    (502) staff       (20)      485 2022-05-18 12:05:24.000000 joker-superuser-0.2.5/joker/superuser/cli/locators.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.387025 joker-superuser-0.2.5/joker/superuser/desktop/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-21 05:03:33.000000 joker-superuser-0.2.5/joker/superuser/desktop/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1312 2021-09-21 14:42:45.000000 joker-superuser-0.2.5/joker/superuser/desktop/chrome.py
--rw-r--r--   0 Hailong    (502) staff       (20)      290 2022-02-05 13:31:57.000000 joker-superuser-0.2.5/joker/superuser/environ.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.389861 joker-superuser-0.2.5/joker/superuser/experimental/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2022-01-23 01:15:56.000000 joker-superuser-0.2.5/joker/superuser/experimental/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1547 2022-01-23 01:26:30.000000 joker-superuser-0.2.5/joker/superuser/experimental/deploy.py
--rw-r--r--   0 Hailong    (502) staff       (20)      156 2022-01-23 00:47:23.000000 joker-superuser-0.2.5/joker/superuser/experimental/firefox.py
--rw-r--r--   0 Hailong    (502) staff       (20)      405 2021-08-04 03:01:05.000000 joker-superuser-0.2.5/joker/superuser/experimental/hexify.py
--rw-r--r--   0 Hailong    (502) staff       (20)      260 2020-02-05 15:57:33.000000 joker-superuser-0.2.5/joker/superuser/extern.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.398582 joker-superuser-0.2.5/joker/superuser/tools/
--rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-03 04:37:50.000000 joker-superuser-0.2.5/joker/superuser/tools/__init__.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2927 2021-01-28 06:33:27.000000 joker-superuser-0.2.5/joker/superuser/tools/apt.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1515 2020-01-11 14:29:32.000000 joker-superuser-0.2.5/joker/superuser/tools/cases.py
--rw-r--r--   0 Hailong    (502) staff       (20)     5384 2020-02-24 02:21:05.000000 joker-superuser-0.2.5/joker/superuser/tools/dedup.py
--rw-r--r--   0 Hailong    (502) staff       (20)       97 2022-01-23 01:19:13.000000 joker-superuser-0.2.5/joker/superuser/tools/experimental.py
--rw-r--r--   0 Hailong    (502) staff       (20)      697 2021-07-03 06:31:51.000000 joker-superuser-0.2.5/joker/superuser/tools/power.py
--rw-r--r--   0 Hailong    (502) staff       (20)     7457 2022-02-09 13:17:20.000000 joker-superuser-0.2.5/joker/superuser/tools/pydir.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2285 2019-08-07 11:23:42.000000 joker-superuser-0.2.5/joker/superuser/tools/pyentry.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2965 2021-07-11 15:13:22.000000 joker-superuser-0.2.5/joker/superuser/tools/remove.py
--rw-r--r--   0 Hailong    (502) staff       (20)      294 2020-03-18 03:34:34.000000 joker-superuser-0.2.5/joker/superuser/tools/setop.py
--rw-r--r--   0 Hailong    (502) staff       (20)     2810 2022-02-09 13:15:53.000000 joker-superuser-0.2.5/joker/superuser/tools/unsource.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1321 2022-05-18 12:24:38.000000 joker-superuser-0.2.5/joker/superuser/tools/urls.py
--rw-r--r--   0 Hailong    (502) staff       (20)     1613 2022-05-17 14:40:53.000000 joker-superuser-0.2.5/joker/superuser/utils.py
-drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2022-05-18 12:30:17.402677 joker-superuser-0.2.5/joker_superuser.egg-info/
--rw-r--r--   0 Hailong    (502) staff       (20)     1220 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/PKG-INFO
--rw-r--r--   0 Hailong    (502) staff       (20)     1316 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/SOURCES.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/dependency_links.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       59 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/entry_points.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/namespace_packages.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-05-13 07:10:18.000000 joker-superuser-0.2.5/joker_superuser.egg-info/not-zip-safe
--rw-r--r--   0 Hailong    (502) staff       (20)      166 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/requires.txt
--rw-r--r--   0 Hailong    (502) staff       (20)        6 2022-05-18 12:30:17.000000 joker-superuser-0.2.5/joker_superuser.egg-info/top_level.txt
--rw-r--r--   0 Hailong    (502) staff       (20)      165 2022-05-18 12:10:08.000000 joker-superuser-0.2.5/requirements.txt
--rw-r--r--   0 Hailong    (502) staff       (20)       38 2022-05-18 12:30:17.403897 joker-superuser-0.2.5/setup.cfg
--rw-r--r--   0 Hailong    (502) staff       (20)     2235 2022-05-17 14:51:55.000000 joker-superuser-0.2.5/setup.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.787192 joker-superuser-0.2.6/
+-rw-r--r--   0 Hailong    (502) staff       (20)       88 2021-09-11 09:03:34.000000 joker-superuser-0.2.6/MANIFEST.in
+-rw-r--r--   0 Hailong    (502) staff       (20)     1658 2023-07-31 08:29:27.786937 joker-superuser-0.2.6/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)      990 2022-05-22 10:01:20.000000 joker-superuser-0.2.6/README.md
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.773968 joker-superuser-0.2.6/joker/
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.776768 joker-superuser-0.2.6/joker/superuser/
+-rw-r--r--   0 Hailong    (502) staff       (20)       73 2023-07-31 08:27:03.000000 joker-superuser-0.2.6/joker/superuser/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1028 2023-07-31 08:29:13.000000 joker-superuser-0.2.6/joker/superuser/__main__.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.777553 joker-superuser-0.2.6/joker/superuser/asset/
+-rw-r--r--   0 Hailong    (502) staff       (20)      718 2021-09-19 15:17:43.000000 joker-superuser-0.2.6/joker/superuser/asset/gitignore.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)     2536 2021-07-03 06:34:49.000000 joker-superuser-0.2.6/joker/superuser/asset/setup.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)      287 2019-07-30 02:44:18.000000 joker-superuser-0.2.6/joker/superuser/asset/simple.yml
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.778522 joker-superuser-0.2.6/joker/superuser/cli/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2022-05-17 14:47:03.000000 joker-superuser-0.2.6/joker/superuser/cli/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1299 2022-05-22 05:26:23.000000 joker-superuser-0.2.6/joker/superuser/cli/chksums.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      485 2022-05-18 12:05:24.000000 joker-superuser-0.2.6/joker/superuser/cli/locators.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      842 2022-05-22 05:21:09.000000 joker-superuser-0.2.6/joker/superuser/cli/uuidgen.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.778973 joker-superuser-0.2.6/joker/superuser/desktop/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-09-21 05:03:33.000000 joker-superuser-0.2.6/joker/superuser/desktop/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1312 2021-09-21 14:42:45.000000 joker-superuser-0.2.6/joker/superuser/desktop/chrome.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      290 2022-02-05 13:31:57.000000 joker-superuser-0.2.6/joker/superuser/environ.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.779944 joker-superuser-0.2.6/joker/superuser/experimental/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2022-01-23 01:15:56.000000 joker-superuser-0.2.6/joker/superuser/experimental/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1547 2022-01-23 01:26:30.000000 joker-superuser-0.2.6/joker/superuser/experimental/deploy.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      156 2022-01-23 00:47:23.000000 joker-superuser-0.2.6/joker/superuser/experimental/firefox.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      405 2021-08-04 03:01:05.000000 joker-superuser-0.2.6/joker/superuser/experimental/hexify.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      260 2020-02-05 15:57:33.000000 joker-superuser-0.2.6/joker/superuser/extern.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.783735 joker-superuser-0.2.6/joker/superuser/tools/
+-rw-r--r--   0 Hailong    (502) staff       (20)       39 2021-07-03 04:37:50.000000 joker-superuser-0.2.6/joker/superuser/tools/__init__.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2927 2021-01-28 06:33:27.000000 joker-superuser-0.2.6/joker/superuser/tools/apt.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1515 2020-01-11 14:29:32.000000 joker-superuser-0.2.6/joker/superuser/tools/cases.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     5384 2020-02-24 02:21:05.000000 joker-superuser-0.2.6/joker/superuser/tools/dedup.py
+-rw-r--r--   0 Hailong    (502) staff       (20)       97 2022-01-23 01:19:13.000000 joker-superuser-0.2.6/joker/superuser/tools/experimental.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      697 2021-07-03 06:31:51.000000 joker-superuser-0.2.6/joker/superuser/tools/power.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     7457 2022-02-09 13:17:20.000000 joker-superuser-0.2.6/joker/superuser/tools/pydir.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2285 2019-08-07 11:23:42.000000 joker-superuser-0.2.6/joker/superuser/tools/pyentry.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2965 2021-07-11 15:13:22.000000 joker-superuser-0.2.6/joker/superuser/tools/remove.py
+-rw-r--r--   0 Hailong    (502) staff       (20)      294 2020-03-18 03:34:34.000000 joker-superuser-0.2.6/joker/superuser/tools/setop.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     2810 2022-02-09 13:15:53.000000 joker-superuser-0.2.6/joker/superuser/tools/unsource.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1542 2022-05-22 09:55:37.000000 joker-superuser-0.2.6/joker/superuser/tools/urls.py
+-rw-r--r--   0 Hailong    (502) staff       (20)     1613 2022-05-17 14:40:53.000000 joker-superuser-0.2.6/joker/superuser/utils.py
+drwxr-xr-x   0 Hailong    (502) staff       (20)        0 2023-07-31 08:29:27.786598 joker-superuser-0.2.6/joker_superuser.egg-info/
+-rw-r--r--   0 Hailong    (502) staff       (20)     1658 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/PKG-INFO
+-rw-r--r--   0 Hailong    (502) staff       (20)     1344 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/SOURCES.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/dependency_links.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       58 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/entry_points.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/namespace_packages.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        1 2022-08-31 05:10:14.000000 joker-superuser-0.2.6/joker_superuser.egg-info/not-zip-safe
+-rw-r--r--   0 Hailong    (502) staff       (20)      173 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/requires.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)        6 2023-07-31 08:29:27.000000 joker-superuser-0.2.6/joker_superuser.egg-info/top_level.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)      172 2023-07-31 08:26:39.000000 joker-superuser-0.2.6/requirements.txt
+-rw-r--r--   0 Hailong    (502) staff       (20)       38 2023-07-31 08:29:27.787289 joker-superuser-0.2.6/setup.cfg
+-rw-r--r--   0 Hailong    (502) staff       (20)     2235 2022-05-17 14:51:55.000000 joker-superuser-0.2.6/setup.py
```

### Comparing `joker-superuser-0.2.5/joker/superuser/__main__.py` & `joker-superuser-0.2.6/joker/superuser/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import volkanic
 
 cmddef = """
-l           joker.superuser.cli.locators:main
-chksumdirs  joker.superuser.cli.checksumdirs:main
-pydir       joker.superuser.tools.pydir
-pyentry     joker.superuser.tools.pyentry
-unsource    joker.superuser.tools.unsource
-cases       joker.superuser.tools.cases
-dup         joker.superuser.tools.dedup
-setop       joker.superuser.tools.setop
-rmdir       joker.superuser.tools.remove
-apt         joker.superuser.tools.apt
-url         joker.superuser.tools.urls
-urls        joker.superuser.tools.urls:runloop
+l               joker.superuser.cli.locators:main
+sha1b32         joker.superuser.cli.chksums:sha1b32
+sha384b64       joker.superuser.cli.chksums:sha384b64
+chksum-rename   joker.superuser.cli.chksums:main
+uuid            joker.superuser.cli.uuidgen:main
+pydir           joker.superuser.tools.pydir
+pyentry         joker.superuser.tools.pyentry
+unsource        joker.superuser.tools.unsource
+cases           joker.superuser.tools.cases
+dup             joker.superuser.tools.dedup
+setop           joker.superuser.tools.setop
+rmdir           joker.superuser.tools.remove
+apt             joker.superuser.tools.apt
+url             joker.superuser.tools.urls
+urls            joker.superuser.tools.urls:runloop
+urlquote        joker.superuser.tools.urls:urlquote
+htmlesc         joker.superuser.tools.urls:htmlescape
 """
 
 _prog = 'python3 -m joker.superuser'
 registry = volkanic.CommandRegistry.from_cmddef(cmddef, _prog)
 
 if __name__ == '__main__':
     registry()
```

### Comparing `joker-superuser-0.2.5/joker/superuser/asset/gitignore.txt` & `joker-superuser-0.2.6/joker/superuser/asset/gitignore.txt`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/asset/setup.txt` & `joker-superuser-0.2.6/joker/superuser/asset/setup.txt`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/desktop/chrome.py` & `joker-superuser-0.2.6/joker/superuser/desktop/chrome.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/experimental/deploy.py` & `joker-superuser-0.2.6/joker/superuser/experimental/deploy.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/apt.py` & `joker-superuser-0.2.6/joker/superuser/tools/apt.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/cases.py` & `joker-superuser-0.2.6/joker/superuser/tools/cases.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/dedup.py` & `joker-superuser-0.2.6/joker/superuser/tools/dedup.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/power.py` & `joker-superuser-0.2.6/joker/superuser/tools/power.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/pydir.py` & `joker-superuser-0.2.6/joker/superuser/tools/pydir.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/pyentry.py` & `joker-superuser-0.2.6/joker/superuser/tools/pyentry.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/remove.py` & `joker-superuser-0.2.6/joker/superuser/tools/remove.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/unsource.py` & `joker-superuser-0.2.6/joker/superuser/tools/unsource.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker/superuser/tools/urls.py` & `joker-superuser-0.2.6/joker/superuser/tools/urls.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import argparse
 import shlex
 import sys
+from html import escape
+from urllib.parse import quote_plus
 
 import pyperclip
+from joker.superuser.environ import JokerInterface
 from joker.textmanip.url import url_simplify
 from volkanic.utils import ignore_arguments
 
-from joker.superuser.environ import JokerInterface
-
 ji = JokerInterface()
 
 
+def urlquote(_prog: str, args):
+    for s in args:
+        print(quote_plus(s))
+
+
+def htmlescape(_prog: str, args):
+    for s in args:
+        print(escape(s))
+
+
 def smart_url_simplify(url, queries):
     config = ji.conf['urls']
     for pattern, _queries in config.items():
         if pattern in url:
             queries = _queries
             break
     return str(url_simplify(url, queries))
```

### Comparing `joker-superuser-0.2.5/joker/superuser/utils.py` & `joker-superuser-0.2.6/joker/superuser/utils.py`

 * *Files identical despite different names*

### Comparing `joker-superuser-0.2.5/joker_superuser.egg-info/SOURCES.txt` & `joker-superuser-0.2.6/joker_superuser.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 joker/superuser/environ.py
 joker/superuser/extern.py
 joker/superuser/utils.py
 joker/superuser/asset/gitignore.txt
 joker/superuser/asset/setup.txt
 joker/superuser/asset/simple.yml
 joker/superuser/cli/__init__.py
-joker/superuser/cli/chksumdirs.py
+joker/superuser/cli/chksums.py
 joker/superuser/cli/locators.py
+joker/superuser/cli/uuidgen.py
 joker/superuser/desktop/__init__.py
 joker/superuser/desktop/chrome.py
 joker/superuser/experimental/__init__.py
 joker/superuser/experimental/deploy.py
 joker/superuser/experimental/firefox.py
 joker/superuser/experimental/hexify.py
 joker/superuser/tools/__init__.py
```

### Comparing `joker-superuser-0.2.5/setup.py` & `joker-superuser-0.2.6/setup.py`

 * *Files identical despite different names*

