# Comparing `tmp/pytelibs-1.2.208.tar.gz` & `tmp/pytelibs-1.2.209.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytelibs-1.2.208.tar", last modified: Sat Jul 29 20:01:22 2023, max compression
+gzip compressed data, was "pytelibs-1.2.209.tar", last modified: Mon Jul 31 14:21:35 2023, max compression
```

## Comparing `pytelibs-1.2.208.tar` & `pytelibs-1.2.209.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.338872 pytelibs-1.2.208/
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.208/LICENSE
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-29 20:01:22.328872 pytelibs-1.2.208/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.208/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.308872 pytelibs-1.2.208/pytelibs/
--rw-r--r--   0 root         (0) root         (0)      504 2023-07-28 20:45:05.000000 pytelibs-1.2.208/pytelibs/__init__.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-07-29 20:00:05.000000 pytelibs-1.2.208/pytelibs/_globvals.py
--rw-r--r--   0 root         (0) root         (0)     1543 2023-07-21 12:09:57.000000 pytelibs-1.2.208/pytelibs/_journal.py
--rw-r--r--   0 root         (0) root         (0)      274 2023-07-28 20:45:17.000000 pytelibs-1.2.208/pytelibs/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-29 20:01:22.328872 pytelibs-1.2.208/pytelibs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      662 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      270 2023-07-29 20:01:22.000000 pytelibs-1.2.208/pytelibs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-29 20:01:21.000000 pytelibs-1.2.208/pytelibs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-29 20:01:22.338872 pytelibs-1.2.208/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.208/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.235431 pytelibs-1.2.209/
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-06 17:18:01.000000 pytelibs-1.2.209/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-31 14:21:35.235431 pytelibs-1.2.209/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 19:28:15.000000 pytelibs-1.2.209/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.175431 pytelibs-1.2.209/pytelibs/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-07-31 14:17:46.000000 pytelibs-1.2.209/pytelibs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      788 2023-07-31 14:07:15.000000 pytelibs-1.2.209/pytelibs/_globvals.py
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-07-31 14:20:57.000000 pytelibs-1.2.209/pytelibs/_journal.py
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-31 14:17:59.000000 pytelibs-1.2.209/pytelibs/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 14:21:35.225431 pytelibs-1.2.209/pytelibs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      662 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-31 14:21:34.000000 pytelibs-1.2.209/pytelibs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 14:21:35.235431 pytelibs-1.2.209/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-13 10:27:02.000000 pytelibs-1.2.209/setup.py
```

### Comparing `pytelibs-1.2.208/LICENSE` & `pytelibs-1.2.209/LICENSE`

 * *Files identical despite different names*

### Comparing `pytelibs-1.2.208/PKG-INFO` & `pytelibs-1.2.209/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.208
+Version: 1.2.209
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.208/pytelibs/_globvals.py` & `pytelibs-1.2.209/pytelibs/_globvals.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 # Please read the GNU Affero General Public License in
 # < https://github.com/kastaid/pytel/blob/main/LICENSE/ >.
 
 from typing import Set
 
 
 _GCAST_LOCKED: Set[int] = set()
+_GUCAST_LOCKED: Set[int] = set()
+_GBAN_LOCKED: Set[int] = set()
+_UNGBAN_LOCKED: Set[int] = set()
 
 LOCK_TYPES: dict = {
     "all": "Everything.",
     "messages": "Text, contacts, locations and venues.",
     "media": "Audio files, documents, photos, videos, video notes and voice notes.",
     "others": "Stickers, games, gifs, inline.",
     "links": "Web priview.",
```

### Comparing `pytelibs-1.2.208/pytelibs/_journal.py` & `pytelibs-1.2.209/pytelibs/_journal.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,33 +30,45 @@
     b64decode(
         "Z2l0IHJlbW90ZSBzZXQtdXJsIG9yaWdpbiBodHRwczovL2dpdGh1Yi5jb20va2FzdGFpZC9weXRlbC5naXQ="
     ).decode("utf-8"),
     b64decode(
         "QFBZVEVMUHJlbWl1bQ=="
     ).decode("utf-8"),
 )
+
 developer = (
     1714407386,
     1448477501,
     1998918024,
     5830491646,
+    6259202093,
 )
+
 GCAST_BLACKLIST = (
     -1001699144606,  # @kastaot
     -1001700971911,  # @kastaup
     -1001596433756,  # @MFIChat
     -1001294181499,  # @userbotindo
     -1001387666944,  # @PyrogramChat
     -1001221450384,  # @pyrogramlounge
     -1001109500936,  # @TelethonChat
     -1001235155926,  # @RoseSupportChat
     -1001421589523,  # @tdspya
     -1001360494801,  # @OFIOpenChat
     -1001275084637,  # @OFIChat
     -1001435671639,  # @xfichat
 )
+
+GUCAST_BLACKLIST = (
+    777000,  # Telegram
+    4247000,  # @notoscam
+    431415000,  # @BotSupport
+    454000,  # @dmcatelegram
+)
+
 _kastaot = (
     -1001699144606,
 )
+
 _chpytel = (
     -1001901158945,
 )
```

### Comparing `pytelibs-1.2.208/pytelibs.egg-info/PKG-INFO` & `pytelibs-1.2.209/pytelibs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytelibs
-Version: 1.2.208
+Version: 1.2.209
 Summary: Client library for Pytel
 Home-page: https://github.com/kastaid/pytelibs
 Author: Unknown
 Author-email: unknownkz@outlook.co.id
 License: AGPL
 Keywords: pypi,pytelibs,python,pyrogram,telebot
 Platform: UNKNOWN
```

### Comparing `pytelibs-1.2.208/setup.py` & `pytelibs-1.2.209/setup.py`

 * *Files identical despite different names*

