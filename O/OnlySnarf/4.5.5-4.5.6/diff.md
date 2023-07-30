# Comparing `tmp/OnlySnarf-4.5.5.tar.gz` & `tmp/OnlySnarf-4.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.5.tar", last modified: Sun Jul 30 23:35:15 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.6.tar", last modified: Sun Jul 30 23:53:20 2023, max compression
```

## Comparing `OnlySnarf-4.5.5.tar` & `OnlySnarf-4.5.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.197844 OnlySnarf-4.5.5/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32003 2023-07-30 23:35:09.000000 OnlySnarf-4.5.5/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.5/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/__main__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2287 2023-07-30 23:34:59.000000 OnlySnarf-4.5.5/OnlySnarf/api.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.5/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.5/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.5/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.5/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.5/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.5/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2334 2023-07-18 04:55:01.000000 OnlySnarf-4.5.5/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   166384 2023-07-27 02:13:20.000000 OnlySnarf-4.5.5/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.5/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.5/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.197844 OnlySnarf-4.5.5/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.5/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.5/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.5/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.5/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20476 2023-07-18 04:40:14.000000 OnlySnarf-4.5.5/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.5/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.193843 OnlySnarf-4.5.5/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-30 23:35:15.000000 OnlySnarf-4.5.5/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 23:35:15.197844 OnlySnarf-4.5.5/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.5/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-30 23:35:15.197844 OnlySnarf-4.5.5/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-07-30 23:35:07.000000 OnlySnarf-4.5.5/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:35:15.197844 OnlySnarf-4.5.5/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.5/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    32005 2023-07-30 23:46:11.000000 OnlySnarf-4.5.6/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.6/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/__main__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2225 2023-07-30 23:53:10.000000 OnlySnarf-4.5.6/OnlySnarf/api.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.6/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.6/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.6/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.6/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.6/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.6/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2334 2023-07-18 04:55:01.000000 OnlySnarf-4.5.6/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   166494 2023-07-30 23:52:59.000000 OnlySnarf-4.5.6/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.6/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.6/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.6/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.6/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.6/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.6/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20476 2023-07-18 04:40:14.000000 OnlySnarf-4.5.6/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.6/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-30 23:53:20.000000 OnlySnarf-4.5.6/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.6/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-07-30 23:53:12.000000 OnlySnarf-4.5.6/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 23:53:20.881336 OnlySnarf-4.5.6/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.6/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.5/CHANGELOG.md` & `OnlySnarf-4.5.6/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -709,15 +709,15 @@
   - continued debugging message tests
   - fixed random user functionality
   - updated driver.poll
   - fixed new message tests
   - added flask to package reqs
   - updated install script
   - updated api scripts to route through snarf
-  **4.5.3,4,5 : 7/30/2023**
+  **4.5.3,4,5,6 : 7/30/2023**
   - api debugging
 
 ------------------------------------------------------------------------------------
 
 ## TODO
 
 - look into Marshmellow package for class / object cleanup
```

### Comparing `OnlySnarf-4.5.5/LICENSE.txt` & `OnlySnarf-4.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/api.py` & `OnlySnarf-4.5.6/OnlySnarf/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,19 +9,16 @@
     app = Flask(__name__)
 
     @app.route('/message', methods=['POST'])
     def message():
         try:
             return "", 200
         finally:
-            Settings.dev_print(request.data)
-            print(request.data)
             args = json.loads(request.data)
             Settings.dev_print(args)
-            print(args)
             config["text"] = args["text"]
             config["user"] = args["user"]
             try: config["files"] = args["input"].split(",")
             except Exception as e: pass
             try: config["price"] = args["price"] or 0
             except Exception as e: pass
             try: config["schedule"] = args["schedule"]
@@ -33,44 +30,42 @@
                 config["verbose"] = 3
             print("messaging")
             Snarf.message()
             Snarf.close()
 
     @app.route('/post', methods=['POST'])
     def post():
-        print(request.data)
-        Settings.dev_print(request.data)
-        args = json.loads(request.data)
-        Settings.dev_print(args)
-        print(args)
-        config["text"] = args["text"]
-        try: config["files"] = args["input"].split(",")
-        except Exception as e: pass
-        try: config["performers"] = args["performers"]
-        except Exception as e: pass
-        try: config["schedule"] = args["schedule"]
-        except Exception as e: pass
-        try: config["questions"] = args["questions"]
-        except Exception as e: pass
-        try: config["duration"] = args["duration"]
-        except Exception as e: pass
-        try: config["expires"] = args["expires"]
-        except Exception as e: pass
-        if app.testing:
-            config["debug"] = True
-            config["verbose"] = 3
-        print("posting")
-        Snarf.post()
-        Snarf.close()
-
-        return "", 200
+        try:
+            return "", 200
+        finally:
+            args = json.loads(request.data)
+            Settings.dev_print(args)
+            config["text"] = args["text"]
+            try: config["files"] = args["input"].split(",")
+            except Exception as e: pass
+            try: config["performers"] = args["performers"]
+            except Exception as e: pass
+            try: config["schedule"] = args["schedule"]
+            except Exception as e: pass
+            try: config["questions"] = args["questions"]
+            except Exception as e: pass
+            try: config["duration"] = args["duration"]
+            except Exception as e: pass
+            try: config["expires"] = args["expires"]
+            except Exception as e: pass
+            if app.testing:
+                config["debug"] = True
+                config["verbose"] = 3
+            print("posting")
+            Snarf.post()
+            Snarf.close()
 
     return app
 
 def main():
     app = create_app()
     app.debug = True
     app.testing = True
-    app.run(host="0.0.0.0")
+    app.run(host="0.0.0.0", port=5000)
 
 if __name__ == "__main__":
     main()
```

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/message.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/poll.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.6/OnlySnarf/classes/user.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.6/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.6/OnlySnarf/conf/test-config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.6/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.6/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.6/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.6/OnlySnarf/lib/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -2973,14 +2973,17 @@
             if str(Settings.is_show_window()) == "False":
                 options.add_argument('--headless')
             options.add_argument("--no-sandbox") # Bypass OS security model
             options.add_argument("--disable-gpu")
             options.add_argument("--disable-extensions")
             options.add_argument("--disable-dev-shm-usage")
 
+            options.add_argument("enable-automation")
+            options.add_argument("--disable-infobars")
+
             # if os.name == 'nt':
                 # options.add_argument(r"--user-data-dir=C:\Users\brain\AppData\Local\Google\Chrome\User Data")
             # else:
             options.add_argument("--user-data-dir="+os.path.join(Settings.get_base_directory(),"tmp","selenium")) # do not disable, required for cookies to work 
             # options.add_argument(r'--profile-directory=Alex D') #e.g. Profile 3
             
             # options.add_argument("--allow-insecure-localhost")
```

### Comparing `OnlySnarf-4.5.5/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.6/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/menu.py` & `OnlySnarf-4.5.6/OnlySnarf/menu.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/snarf.py` & `OnlySnarf-4.5.6/OnlySnarf/snarf.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/args.py` & `OnlySnarf-4.5.6/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.6/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/config.py` & `OnlySnarf-4.5.6/OnlySnarf/util/config.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.6/OnlySnarf/util/defaults.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.6/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.6/OnlySnarf/util/optional_args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.6/OnlySnarf/util/settings.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.6/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.5.6/OnlySnarf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.5
+Version: 4.5.6
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.5 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.6 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.5/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.6/OnlySnarf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/PKG-INFO` & `OnlySnarf-4.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.5
+Version: 4.5.6
 Summary: OnlyFans Content Distribution Tool
 Home-page: https://github.com/skeetzo/onlysnarf
 Author: Skeetzo
 Author-email: WebmasterSkeetzo@gmail.com
 Keywords: OnlyFans,OnlySnarf,selenium,snarf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.5 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.6 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.5/README.md` & `OnlySnarf-4.5.6/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/setup.py` & `OnlySnarf-4.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.5",
+    version="4.5.6",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `OnlySnarf-4.5.5/tests/test_profile.py` & `OnlySnarf-4.5.6/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.5/tests/test_promotion.py` & `OnlySnarf-4.5.6/tests/test_promotion.py`

 * *Files identical despite different names*

