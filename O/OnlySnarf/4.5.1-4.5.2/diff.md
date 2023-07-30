# Comparing `tmp/OnlySnarf-4.5.1.tar.gz` & `tmp/OnlySnarf-4.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OnlySnarf-4.5.1.tar", last modified: Wed Jul 12 22:44:07 2023, max compression
+gzip compressed data, was "OnlySnarf-4.5.2.tar", last modified: Sun Jul 30 22:58:23 2023, max compression
```

## Comparing `OnlySnarf-4.5.1.tar` & `OnlySnarf-4.5.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    31578 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/CHANGELOG.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/LICENSE.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/MANIFEST.in
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       47 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/__main__.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/classes/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/discount.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/element.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.1/OnlySnarf/classes/file.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12549 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/message.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1974 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/poll.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/classes/profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/classes/promotion.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/schedule.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    18262 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/classes/user.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/conf/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/conf/config.conf
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2263 2023-07-11 19:44:50.000000 OnlySnarf-4.5.1/OnlySnarf/conf/test-config.conf
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf/elements/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/login.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/elements/profile.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/OnlySnarf/lib/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/lib/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   163926 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/lib/driver.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/lib/ffmpeg.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5130 2023-07-06 00:06:23.000000 OnlySnarf-4.5.1/OnlySnarf/menu.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5069 2023-07-11 22:15:14.000000 OnlySnarf-4.5.1/OnlySnarf/snarf.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/OnlySnarf/util/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/__init__.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/colorize.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1483 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/config.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3183 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/util/defaults.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/OnlySnarf/util/logger.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.1/OnlySnarf/util/optional_args.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20018 2023-07-12 22:40:17.000000 OnlySnarf-4.5.1/OnlySnarf/util/settings.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.1/OnlySnarf/util/validators.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.620244 OnlySnarf-4.5.1/OnlySnarf.egg-info/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1171 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/SOURCES.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/dependency_links.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/entry_points.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       73 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/requires.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-12 22:44:07.000000 OnlySnarf-4.5.1/OnlySnarf.egg-info/top_level.txt
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/PKG-INFO
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.1/README.md
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/setup.cfg
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1373 2023-07-12 22:43:39.000000 OnlySnarf-4.5.1/setup.py
-drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-12 22:44:07.624244 OnlySnarf-4.5.1/tests/
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/tests/test_profile.py
--rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.1/tests/test_promotion.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    31991 2023-07-30 22:57:47.000000 OnlySnarf-4.5.2/CHANGELOG.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1064 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/LICENSE.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      141 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/MANIFEST.in
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       75 2023-07-26 00:57:38.000000 OnlySnarf-4.5.2/OnlySnarf/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      387 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/__main__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1978 2023-07-25 19:00:57.000000 OnlySnarf-4.5.2/OnlySnarf/api.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/classes/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/classes/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4388 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/classes/discount.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1892 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/classes/element.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    16142 2023-07-11 22:15:12.000000 OnlySnarf-4.5.2/OnlySnarf/classes/file.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12611 2023-07-17 20:29:42.000000 OnlySnarf-4.5.2/OnlySnarf/classes/message.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1986 2023-07-17 07:19:23.000000 OnlySnarf-4.5.2/OnlySnarf/classes/poll.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    14542 2023-05-29 23:06:57.000000 OnlySnarf-4.5.2/OnlySnarf/classes/profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    10171 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/classes/promotion.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4891 2023-07-12 22:40:17.000000 OnlySnarf-4.5.2/OnlySnarf/classes/schedule.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20341 2023-07-17 21:30:18.000000 OnlySnarf-4.5.2/OnlySnarf/classes/user.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/conf/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2240 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/conf/config.conf
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2334 2023-07-18 04:55:01.000000 OnlySnarf-4.5.2/OnlySnarf/conf/test-config.conf
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/elements/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/elements/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    15689 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/elements/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1401 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/elements/login.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    11335 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/elements/profile.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/lib/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/lib/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)   166384 2023-07-27 02:13:20.000000 OnlySnarf-4.5.2/OnlySnarf/lib/driver.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     9500 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/lib/ffmpeg.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5076 2023-07-17 07:19:23.000000 OnlySnarf-4.5.2/OnlySnarf/menu.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     5006 2023-07-17 07:19:23.000000 OnlySnarf-4.5.2/OnlySnarf/snarf.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf/util/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        0 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/util/__init__.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1327 2023-07-17 03:26:29.000000 OnlySnarf-4.5.2/OnlySnarf/util/args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1062 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/util/colorize.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1591 2023-07-26 01:01:08.000000 OnlySnarf-4.5.2/OnlySnarf/util/config.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3274 2023-07-17 19:07:11.000000 OnlySnarf-4.5.2/OnlySnarf/util/defaults.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     2025 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/OnlySnarf/util/logger.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    12269 2023-05-29 23:06:57.000000 OnlySnarf-4.5.2/OnlySnarf/util/optional_args.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)    20476 2023-07-18 04:40:14.000000 OnlySnarf-4.5.2/OnlySnarf/util/settings.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     3934 2023-07-11 19:44:50.000000 OnlySnarf-4.5.2/OnlySnarf/util/validators.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/OnlySnarf.egg-info/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1188 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/SOURCES.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)        1 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/dependency_links.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)      109 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/entry_points.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       94 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/requires.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       91 2023-07-30 22:58:23.000000 OnlySnarf-4.5.2/OnlySnarf.egg-info/top_level.txt
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4679 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/PKG-INFO
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     4049 2023-07-06 00:40:42.000000 OnlySnarf-4.5.2/README.md
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)       79 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/setup.cfg
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1465 2023-07-30 22:57:31.000000 OnlySnarf-4.5.2/setup.py
+drwxrwxr-x   0 skeetzo   (1000) skeetzo   (1000)        0 2023-07-30 22:58:23.296884 OnlySnarf-4.5.2/tests/
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1209 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/tests/test_profile.py
+-rw-rw-r--   0 skeetzo   (1000) skeetzo   (1000)     1451 2023-04-16 06:45:34.000000 OnlySnarf-4.5.2/tests/test_promotion.py
```

### Comparing `OnlySnarf-4.5.1/CHANGELOG.md` & `OnlySnarf-4.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -696,25 +696,36 @@
   - cleaned up bin/test scripts
   - added basic api setup
   - added test scripts for flask & api
   - beginning modifications for receiving api calls
 **4.5.1 : 7/12/2023**
   - fixed package req: validators
   - added modifications for running via api
-
+**4.5.2 : 7/16/2023**
+  - relocated api structure for testing
+  - added tests for flask api
+  - updates to tests, code flow for missing config / args values
+  - added individual message funcationality tests 
+  **7/17/2023**
+  - continued debugging message tests
+  - fixed random user functionality
+  - updated driver.poll
+  - fixed new message tests
+  - added flask to package reqs
+  - updated install script
+  - updated api scripts to route through snarf
+  **7/30/2023**
+  - api debugging
 
 ------------------------------------------------------------------------------------
 
 ## TODO
 
-
 - look into Marshmellow package for class / object cleanup
-- reconfigure how args & config values are passed through into Settings --> to fix when setting a variable like post.schedule = "text" is referenced after the args check step
 
-- fix how tabs open and scroll and then the process opens another tab to find the same elements and scroll again ala: find users then discount user
 
 - add smart idea for getting statement information
 - add better version notes to readme's list of "works on"
 - re-add stuff for testing on multiple platforms ala mac ;) 
 
 - double check how tags & performers are implemented in config and text config and then re-add to docs
 
@@ -777,14 +788,16 @@
 - fix any new cli menu errors made while updating major processes
 - re-enable prompting for discount amount&months in Settings or somewhere else (at some point)
 - re-add removed user select code in notes/selectstuff.py (for menu prompts)
 - re-enable menu command
 
 ## Fix / Debug
 
+- fix how tabs open and scroll and then the process opens another tab to find the same elements and scroll again ala: find users then discount user
+
 (unlikely to be fixed soon, if ever)
 - google login: unsafe browser warning --> possibly end of usability --> should I just remove this? form login works, twitter login works (i think)
 -- maybe just cut out / leave as is until can debug "unsafe browser" issue?
 
 - debug: discover the cause of the super slow web scraping
 -- probably not: debug_delay
 ---- possibly improved via recent updated coding? (4.3.10)
@@ -835,16 +848,20 @@
   - boolean checks from "Settings.is_" functions are failing: replaced with redundant string checks for if == "True"
 **4.3.12**
   - message: drag&drop has decided to occasionally stop working; maybe a selenium version issue?
 **4.4.0**
   - discount: amount&months still require 2 passes on average to update values correctly
 **4.4.6**
   - followed instructions here for enabled firefox on ubuntu 22.04: https://www.reddit.com/r/learnpython/comments/umft75/selenium_your_firefox_profile_cannot_be_loaded_it/ -> https://support.mozilla.org/en-US/kb/install-firefox-linux#w_install-firefox-from-mozilla-builds-for-advanced-users
-**4.4.9:**
+**4.4.9**
   - when running pytest, the final arg is mistakenly picked up as an input (and passes validation, because it's a file) and tests therefore have multiple repeat file uploads    
+**4.5.2**
+  - [fixed] message tests come up negative when they're all passing basic functionality
+
+
 
 # Web Browser Versions
 (no longer as relevant as of 4.4.7ish updates)
 
 Version Check:
 stable => Google Chrome 106.0.5249.40 beta
 beta => Google Chrome 106.0.5249.40 beta
```

### Comparing `OnlySnarf-4.5.1/LICENSE.txt` & `OnlySnarf-4.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/discount.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/discount.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/element.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/element.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/file.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/file.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/message.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/message.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,23 @@
         """
 
         # universal message variables
         self.text = ""
         self.files = []
         self.performers = []
         self.price = 0 # $3 - $100
-        self.tags = []
+        self.keywords = []
         self.__initialized__ = False
 
     def init(self):
         """Initialize."""
 
         if self.__initialized__: return
         self.get_text()
-        self.get_tags()
+        self.get_keywords()
         self.get_price()
         self.get_files()
         self.get_performers()
         self.__initialized__ = True
 
     @staticmethod
     def format_keywords(keywords):
@@ -89,15 +89,15 @@
         -------
         str
             The generated text into a string. Example:
             "This is the text. @name, @name, and @name #keyword0 #keyword1"
 
         """
 
-        return "{}{}{}".format(self.get_text(), Message.format_performers(self.get_performers()), Message.format_keywords(self.get_tags())).strip()
+        return "{}{}{}".format(self.get_text(), Message.format_performers(self.get_performers()), Message.format_keywords(self.get_keywords())).strip()
 
     @staticmethod
     def is_tip(text):
         """
         Checks if the text contains a tip amount.
 
         Parameters
@@ -189,15 +189,15 @@
         """
 
         return dict({
             "text": self.format_text(),
             "files": self.get_files(),
             "performers": self.get_performers(),
             "price": self.get_price(),
-            "tags": self.get_tags()
+            "keywords": self.get_keywords()
         })
 
     def get_performers(self):
         """
         Gets the performers for the text.
 
         Returns
@@ -237,28 +237,28 @@
         elif Decimal(sub(r'[^\d.]', '', str(price))) > Decimal(priceMax):
             Settings.warn_print("price too high: {} < {}".format(price, priceMax))
             Settings.maybe_print("adjusting price to maximum...")
             price = priceMax    
         self.price = price
         return self.price
 
-    def get_tags(self):
+    def get_keywords(self):
         """
-        Gets the tags for the text.
+        Gets the keywords for the text.
 
         Returns
         -------
         list
-            The tags
+            The keywords
 
         """
 
-        if len(self.tags) > 0: return self.tags
-        self.tags = Settings.get_tags()
-        return self.tags
+        if len(self.keywords) > 0: return self.keywords
+        self.keywords = Settings.get_keywords()
+        return self.keywords
 
     def get_text(self, again=True):
         """
         Gets the text value if not none else sets it from args or prompts.
 
 
         Parameters
@@ -302,15 +302,15 @@
                     text = self.files[0].get_parent()["title"]
             except Exception as e:
                 # not a simple int
                 # do nothing cause probably set already
                 pass
         text = text.replace("_", " ")
         # redo keyword parsing (unsure if necessary call)
-        text = self.update_tags(text)
+        text = self.update_keywords(text)
         return text
 
     def send(self, username, user_id=None):
         """
         Sends a message.
 
 
@@ -418,30 +418,30 @@
             "text": self.format_text(),
             "files": self.get_files(),
             "performers": self.get_performers(),
             "price": self.get_price(),
             "expiration": self.get_expiration(),
             "schedule": self.get_schedule(),
             "poll": self.get_poll(),
-            "tags": self.get_tags()
+            "keywords": self.get_keywords()
         })
 
     def get_schedule(self):
         """
         Gets the schedule value if not none else sets it from args or prompts.
 
         Returns
         -------
         Schedule
             Schedule object with proper values.
 
         """
 
         if self.schedule: return self.schedule
-        # self.schedule = Schedule()
+        self.schedule = Schedule()
         return self.schedule
 
     def send(self):
         """
         Sends a post.
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/poll.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/poll.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,12 +74,12 @@
         -------
         bool
             Whether or not the poll is valid
 
         """
 
         Settings.dev_print("validating poll...")
-        if len(self.get_questions()) > 0 and self.get_duration():
+        if len(self.get_questions()) > 0 and str(self.get_duration()) != "0":
             Settings.dev_print("valid poll!")
             return True
         Settings.dev_print("invalid poll!")
         return False
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/profile.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/promotion.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/promotion.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/schedule.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/schedule.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/classes/user.py` & `OnlySnarf-4.5.2/OnlySnarf/classes/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import json
 import time
 import os
+import random
 import threading
 from datetime import datetime, timedelta
 ##
 from ..util.colorize import colorize
 from ..lib.driver import Driver
 from ..util.settings import Settings
 
+ALREADY_RANDOMIZED_USERS = []
+
 class User:
     """OnlyFans users."""
 
     def __init__(self, data):
         """User object"""
 
         data = json.loads(json.dumps(data))
@@ -56,15 +59,15 @@
 
         Parameters
         ----------
         classes.User
             The user to compare another user object against
         """
 
-        if str(user.username) == str(self.username) or str(user.id) == str(self.id): return True
+        if (str(user.username) != "None" and str(user.username) == str(self.username)) or (str(user.id) != "None" and str(user.id) == str(self.id)): return True
         return False
 
     def get_id(self):
         """
         Get the provided ID of the User. Searches via username if necessary.
 
         Returns
@@ -164,14 +167,15 @@
                     #     continue
                     # self.sent_files.append(file_name)
                 return driver.upload_files(files)
             if all([enter_text(message["text"]), enter_price(message["price"]), enter_files(message["files"])]): return confirm_message()
         except Exception as e:
             Settings.err_print("message failed!")
             Settings.dev_print(e)
+        Settings.err_print("message somehow failed!")
         return False
 
     def update(self, user):
         for key, value in json.loads(user.toJSON()).items():
             # Settings.print("updating: {} = {}".format(key, value))
             setattr(self, str(key), value)
 
@@ -326,18 +330,71 @@
         -------
         classes.User
             A random user
 
         """
 
         Settings.dev_print("getting random user...")
-        import random
-        randomUser = random.choice(User.get_all_users())
-        Settings.dev_print("random user: {}".format(randomUser.username))
-        return randomUser
+
+        users = User.get_all_users_usernames()
+
+        randomUser = None
+        randomizedUsers = User.get_already_randomized_users()
+
+        while randomUser not in randomizedUsers:
+            randomUser = random.choice(users)
+            if randomUser not in randomizedUsers:
+                User.add_to_randomized_users(randomUser, users=randomizedUsers)
+                randomizedUsers.append(randomUser)
+
+        Settings.dev_print("random user: {}".format(randomUser))
+
+        users = User.get_all_users()
+        for user in users:
+            if str(user.username) == str(randomUser):
+                return user
+        return User({"username":randomUser})
+
+    @staticmethod
+    def get_all_users_usernames():
+        users = User.get_all_users()
+        usernames = []
+        for user in users:
+            usernames.append(user.username)
+        return usernames
+
+    # return from json file 
+    @staticmethod
+    def get_already_randomized_users():
+        Settings.dev_print("getting already randomized users...")
+        users = []
+        try:
+            with open(str(Settings.get_users_path().replace("users.json","random_users.json"))) as json_file:  
+                for user in json.load(json_file)['randomized_users']:
+                    users.append(user)
+            Settings.maybe_print("loaded randomized users")
+        except Exception as e:
+            Settings.dev_print(e)
+        return users
+
+    # add to json file
+    @staticmethod
+    def add_to_randomized_users(newUser, users=[]):
+        data = {}
+        data['randomized_users'] = []
+        for user in users:
+            data['randomized_users'].append(user)
+        data['randomized_users'].append(newUser)
+        try:
+            with open(str(Settings.get_users_path().replace("users.json","random_users.json")), 'w') as outfile:  
+                json.dump(data, outfile, indent=4, sort_keys=True)
+        except FileNotFoundError:
+            Settings.err_print("missing random users!")
+        except OSError:
+            Settings.err_print("missing random users path!")
 
     @staticmethod
     def get_recent_messagers():
         """
         Get users that have recently sent messages.
 
         Returns
@@ -443,17 +500,17 @@
         Parameters
         ----------
         message : Object
             The message to send as a serialized Message object from get_message.
         """
 
         if str(username).lower() == "random":
-            User.get_random_user().message(message)
+            return User.get_random_user().message(message)
         else:
-            User({"username":username,"id":user_id}).message(message)
+            return User({"username":username,"id":user_id}).message(message)
 
     @staticmethod
     def read_following_local():
         """
         Read the locally saved following file.
 
         Returns
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/conf/config.conf` & `OnlySnarf-4.5.2/OnlySnarf/conf/config.conf`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/conf/test-config.conf` & `OnlySnarf-4.5.2/OnlySnarf/conf/test-config.conf`

 * *Files 13% similar despite different names*

```diff
@@ -1,67 +1,69 @@
 [ARGS]
 
 ## General ##
 # auto, onlyfans, or twitter
-#login = auto
-#prefer_local = True
-#save_users = False
-#upload_max = 10
-#upload_max_duration = 60 
+login = auto
+prefer_local = True
+save_users = False
+upload_max = 10
+upload_max_duration = 60 
 
 ## OnlySnarf ##
-#amount = 0
-#months = 0
-#price = 
-#date = 
-#duration = 0
-#expiration = 0 
-#questions = 
-#schedule = 
-#tags = 
-#text = 
-#time = 
-#tweeting = False
-#user =  
-#users =  
+amount = 0
+months = 0
+price = 0
+date = None
+duration = 0
+expiration = 0 
+questions = []
+schedule = None
+tags = []
+text = None
+time = None
+tweeting = False
+user = None
+users = None
 ## fetches credentials from user config with provided username
 username = alexdicksdown
 
 ## Selenium ##
 # auto, brave, chrome, chromium, firefox, ie, edge, opera; reconnect[-firefox, chrome, etc], remote[-firefox, chrome, etc]
-#browser = auto
-#cookies = True
-#keep = False
-#session_id = 
-#session_url = 
+browser = auto
+cookies = True
+keep = True
+session_id = None
+session_url = None
 ## show browser window
-show = False
+show = True
 
 ## Debugging ##
 debug = True
-#debug_cookies = False
+debug_cookies = False
 debug_delay = True
-#debug_firefox = False
-#debug_google = False
-#debug_selenium = False
-#force_upload = False
-#recent_users_count = 10
-#skip_upload = False
-#skipped_users = 
-#users_read = 10
-#reduce = False
+debug_firefox = False
+debug_google = False
+debug_selenium = False
+force_upload = False
+recent_users_count = 10
+skip_download = False
+skip_upload = False
+skipped_users = 
+users_read = 10
+reduce = False
 verbose = 3
 
 [PATH]
 #mount = $HOME/onlysnarf
 #download = $HOME/onlysnarf/downloads 
 #profile = $HOME/onlysnarf/profiles/$username
 #users = $HOME/.onlysnarf/users.json
 
 [POSTS]
+## these were all ideas that were never used, fyi
 #welcome = "Welcome to my OnlyFans!"
 #ask = "What would you like to see me post more of? Comment below!"
 #content_request = "Are there any specific content requests?"
 #giggle = "teehee"
 #no_customs = "I don\'t do customs, sorry!"
 #social_media = "Be sure to check out my social medias!"
 #thank_you = "Thank you all for your support!"
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/elements/driver.py` & `OnlySnarf-4.5.2/OnlySnarf/elements/driver.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/elements/login.py` & `OnlySnarf-4.5.2/OnlySnarf/elements/login.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/elements/profile.py` & `OnlySnarf-4.5.2/OnlySnarf/elements/profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/lib/driver.py` & `OnlySnarf-4.5.2/OnlySnarf/lib/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -391,14 +391,15 @@
         Settings.print("downloading content...")
         def scroll_to_bottom():
             try:
                 # go to profile page and scroll to bottom
                 self.go_to_profile()
                 # count number of content elements to scroll to bottom
                 num = self.browser.find_element(By.CLASS_NAME, "b-profile__sections__count").get_attribute("innerHTML")
+                num = num.replace("K","00").replace(".","")
                 Settings.maybe_print("content count: {}".format(num))
                 for n in range(int(int(int(num)/5)+1)):
                     Settings.print_same_line("({}/{}) scrolling...".format(n,int(int(int(num)/5)+1)))
                     self.browser.execute_script("window.scrollTo(0, document.body.scrollHeight);")
                     time.sleep(1)
                 Settings.print("")
             except Exception as e:
@@ -412,49 +413,76 @@
 
     def download_images(self, destination=None):
         """Downloads all images on the page"""
 
         downloaded = []
         downloadMe = []
         try:
-            images = self.browser.find_elements(By.TAG_NAME, "img")
+            images_ = self.browser.find_elements(By.TAG_NAME, "img")
+            images = []
+
+            for image in images_:
+                # print(image)
+                # print(image.get_attribute("src"))
+                if "thumbs.onlyfans.com" not in str(image.get_attribute("src")):
+                    # print(image.get_attribute("src"))
+                    images.append(image)
+
             end = len(images)
             if len(images) == 0:
                 Settings.warn_print("no images found!")
                 return downloaded
             if not destination: destination = os.path.join(Settings.get_download_path(), "images")
             Path(destination).mkdir(parents=True, exist_ok=True)
             i=0
             for j in range(end):
                 try:
-                    images = self.browser.find_elements(By.TAG_NAME, "img")
+                    images_ = self.browser.find_elements(By.TAG_NAME, "img")
+                    images = []
+
+                    for image in images_:
+                        if "thumbs.onlyfans.com" not in str(image.get_attribute("src")):
+                            # print(image.get_attribute("src"))
+                            images.append(image)
+
                     # click on each image
                     # download each image via class "pswp__img"
-                    self.move_to_then_click_element(images[i])
+                    successful = self.move_to_then_click_element(images[j])
+
+                    while not successful:
+                        driver.browser.execute_script("window.scrollTo(0, document.body.scrollHeight);")
+                        time.sleep(1)
+                        successful = self.move_to_then_click_element(images[j])
+
                     time.sleep(1)
                     hdImages = self.browser.find_elements(By.CLASS_NAME, "pswp__img")
-                    downloadMe.extend(hdImages)
+                    for image in hdImages:
+                        downloadMe.append(image.get_attribute("src"))
+                    # print(len(downloadMe))
                 except Exception as err:
                     Settings.print("")            
                     Settings.warn_print(err)
                 finally:
                     ActionChains(self.browser).send_keys(Keys.ESCAPE).perform()
                     i+=1
             Settings.print("")
         except Exception as err:
             Settings.err_print(err)
 
+        # print(downloadMe)
         downloadMe = list(set(downloadMe)) # remove duplicates
+        # print(downloadMe)
 
         i=1
-        for image in downloadMe:
-            src = ""
+        for src in downloadMe:
+            # src = ""
             try:
                 # if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_IMAGES: break
-                src = str(image.get_attribute("src"))
+                # src = str(image.get_attribute("src"))
+                # print(src)
                 if not src or src == "" or src == "None" or "/thumbs/" in src or "_frame_" in src or "http" not in src: continue
                 Settings.print_same_line("downloading image: {}/{}".format(i, len(images)))
                 # Settings.print("Image: {}".format(src[:src.find(".jpg")+4]))
                 # Settings.dev_print("image src: {}".format(src))
                     # while os.path.isfile("{}/{}.jpg".format(destination, i)):
                         # i+=1
 
@@ -536,34 +564,47 @@
                 src = ""
                 playButtons = self.browser.find_elements(By.CLASS_NAME, "b-photos__item__play-btn")
 
                 try:
                     # click on play button
                     # find new and only video ele on page
                     self.move_to_then_click_element(playButtons[i])
-                    time.sleep(3)
-                    video = self.browser.find_element(By.TAG_NAME, "video")
+
+                    time.sleep(2)
+
+                    video = self.browser.find_element(By.CLASS_NAME, "vjs-tech")
+                    # try:
+                    # except Exception as e:
+                        # pass
+                        # try:
+                            # video = self.browser.find_element(By.TAG_NAME, "video")
+                        # except Exception as e:
+                            # pass
+
+                    # if not video: continue
+
                     # if Driver.DOWNLOADING_MAX and i > Driver.DOWNLOAD_MAX_VIDEOS: break
                     src = str(video.get_attribute("src"))
                     if not src or src == "" or src == "None" or "http" not in src: continue
                     downloadMe.append(src)
                 except Exception as e:
                     Settings.warn_print(e)
                 finally:
+                    # self.browser.switch_to.default_content()
                     ActionChains(self.browser).send_keys(Keys.ESCAPE).perform()
                     i+=1
 
             downloadMe = list(set(downloadMe)) # remove duplicates
 
             i=1
             for src in downloadMe:
                 try:
                     Settings.print_same_line("downloading video: {}/{}".format(i, end))
                     # Settings.print("Video: {}".format(src[:src.find(".mp4")+4]))
-                    Settings.dev_print("video src: {}".format(src))
+                    # Settings.dev_print("video src: {}".format(src))
                     # while os.path.isfile("{}/{}.mp4".format(destination, i)):
                         # i+=1
                     wget.download(src, "{}/{}.mp4".format(destination, i), False)
                     downloaded.append(i)
                 except Exception as e:
                     Settings.print("")            
                     Settings.err_print(e)
@@ -742,54 +783,46 @@
         Returns
         -------
         bool
             Whether or not entering the expiration was successful
 
         """
 
-        if not expiration: return True
+        if str(expiration) == "0" or not expiration: return True
         try:
             Settings.print("Expiration:")
             Settings.print("- Period: {}".format(expiration))
             # if expiration is 'no limit', then there's no expiration and hence no point here
             if expiration == 999: return True
-            self.open_more_options()
-            # open expires window
-            Settings.dev_print("adding expiration")
-            self.find_element_to_click("expiresAdd").click()
-            # select duration
-            Settings.dev_print("entering expiration")
 
-            # leave in case needed again
-            # nums = self.find_elements_by_name("expiresPeriods")
-            # for num in nums:
-            #     inner = num.get_attribute("innerHTML")
-            #     if int(expiration) == 1  and ">1<" in str(inner): num.click()
-            #     if int(expiration) == 3  and ">3<" in str(inner): num.click()
-            #     if int(expiration) == 7  and ">7<" in str(inner): num.click()
-            #     if int(expiration) == 30 and ">30<" in str(inner): num.click()
-            #     if int(expiration) == 99 and ">o limit<" in str(inner): num.click()
-
-            # expiration can now have any int, so update for entering any int less than 30
-            self.find_element_by_name("periodValue").send_keys(expiration)
+            def enter_expiration(expires):
+                # enter duration
+                Settings.dev_print("entering expiration")
+                action = ActionChains(self.browser)
+                action.click(on_element=self.find_element_to_click("expiresAdd"))
+                action.pause(int(1))
+                action.send_keys(Keys.TAB)
+                action.send_keys(str(expires))
+                action.pause(int(1))
+                action.key_down(Keys.SHIFT).send_keys(Keys.TAB).key_up(Keys.SHIFT)
+                action.pause(int(1))
+                action.send_keys(Keys.ENTER)
+                action.perform()
+                Settings.dev_print("successfully entered expiration")
+
+            # not really necessary with 'Clear' button
+            def cancel_expiration():
+                #icon-close
+                elements = self.browser.find_elements(By.TAG_NAME, "use")
+                element = [elem for elem in elements if '#icon-close' in str(elem.get_attribute('href'))][0]
+                ActionChains(self.browser).move_to_element(element).click().perform()
 
-            Settings.dev_print("successfully selected expiration")
+            enter_expiration(expiration)
             Settings.debug_delay_check()
-            # save
-            if str(Settings.is_debug()) == "True":
-                Settings.maybe_print("skipping expiration (debug)")
-                Settings.dev_print("skipping expiration")
-                self.find_element_to_click("expiresCancel").click()
-                Settings.dev_print("successfully canceled expires")
-                Settings.dev_print("### Expiration Successfully Canceled ###")
-            else:
-                Settings.dev_print("saving expiration")
-                self.find_element_to_click("expiresSave").click()
-                Settings.dev_print("successfully saved expires")
-                Settings.dev_print("### Expiration Successful ###")
+            Settings.dev_print("### Expiration Successful ###")
             return True
         except Exception as e:
             Driver.error_checker(e)
             Settings.err_print("failed to enter expiration")
             try:
                 Settings.dev_print("canceling expiration")
                 self.find_element_to_click("expiresCancel").click()
@@ -1104,14 +1137,15 @@
         bool
             Whether or not the tab exists
 
 
         """
 
         original_handle = self.browser.current_window_handle
+        Settings.dev_print("searching for page: {}".format(page))
         Settings.dev_print("tabs: {}".format(self.tabs))
         Settings.dev_print("handles: {}".format(self.browser.window_handles))
         try:
             Settings.dev_print("checking tabs...")
             for page_, handle, value in self.tabs:
                 Settings.dev_print("{} = {}".format(page_, page))
                 if str(page_) in str(page):
@@ -1157,15 +1191,14 @@
         windows_before  = self.browser.current_window_handle
         Settings.dev_print("current window handle is : %s" %windows_before)
         windows = self.browser.window_handles
         self.browser.execute_script('''window.open("{}","_blank");'''.format(url))
         # self.browser.execute_script("window.open('{}')".format(url))
         self.handle_alert()
         self.get_page_load()
-        # self.browser.execute_script("window.open('https://www.yahoo.com')")
         WebDriverWait(self.browser, 10).until(EC.number_of_windows_to_be(len(windows)+1))
         windows_after = self.browser.window_handles
         new_window = [x for x in windows_after if x not in windows][0]
         # self.browser.switch_to.window(new_window) <!---deprecated>
         self.browser.switch_to.window(new_window)
         Settings.dev_print("page title after tab switching is : %s" %self.browser.title)
         Settings.dev_print("new window handle is : %s" %new_window)
@@ -1452,14 +1485,15 @@
 
         if not username and not user_id:
             Settings.err_print("missing user to message")
             return False
         try:
             driver = Driver.get_driver()
             driver.auth()
+            driver.go_to_home(force=True)
             Settings.dev_print("attempting to start message for {}...".format(username))
             type__ = None # default
             # if the username is a key string it will behave differently
             if str(username).lower() == "all": type__ = "messageAll"
             elif str(username).lower() == "recent": type__ = "messageRecent"
             elif str(username).lower() == "favorite": type__ = "messageFavorite"
             elif str(username).lower() == "renew on": type__ = "messageRenewers"
@@ -1494,30 +1528,48 @@
         Returns
         -------
         bool
             Whether or not entering the text was successful
 
         """
 
+        def close_icons():
+            try:
+                #icon-close
+                elements = self.browser.find_elements(By.TAG_NAME, "use")
+                for element in [elem for elem in elements if '#icon-close' in str(elem.get_attribute('href'))]:
+                    ActionChains(self.browser).move_to_element(element).click().perform()
+            except Exception as e:
+                # Settings.err_print(e)
+                Settings.dev_print("unable to click: #icon-close")
+
+        def clear_text():
+            try:
+                ActionChains(self.browser).move_to_element(self.browser.find_element(By.ID, "new_post_text_input")).double_click().click_and_hold().send_keys(Keys.CLEAR).perform()
+            except Exception as e:
+                # Settings.err_print(e)
+                Settings.dev_print("unable to clear text")
+
         try:
             Settings.dev_print("clearing message")
-            clearButton = [ele for ele in self.browser.find_elements(By.TAG_NAME, "button") if "Clear" in ele.get_attribute("innerHTML")]
+            clearButton = [ele for ele in self.browser.find_elements(By.TAG_NAME, "button") if "Clear" in ele.get_attribute("innerHTML") and ele.is_enabled()]
             if len(clearButton) > 0:
                 Settings.dev_print("clicking clear button...")
                 clearButton[0].click()
             else:
                 Settings.dev_print("refreshing page and clearing text...")
                 self.go_to_home(force=True)
-                ActionChains(self.browser).move_to_element(self.browser.find_element(By.ID, "new_post_text_input")).double_click().click_and_hold().send_keys(Keys.CLEAR).perform()
+                clear_text()
+                close_icons()
             Settings.dev_print("successfully cleared message")
-            return True
+            # return True
         except Exception as e:
             Driver.error_checker(e)
-            Settings.err_print("failure to clear message")
-        return False
+            Settings.warn_print("failure to clear message")
+        # return False
 
     def message_confirm(self):
         """
         Wait for the message open on the page's Confirm button to be clickable and click it
 
         Returns
         -------
@@ -1528,16 +1580,16 @@
 
         try:
             Settings.dev_print("waiting for message confirm to be clickable...")
             confirm = WebDriverWait(self.browser, int(Settings.get_upload_max_duration()), poll_frequency=3).until(EC.element_to_be_clickable((By.CLASS_NAME, Element.get_element_by_name("new_message").getClass())))
             Settings.dev_print("message confirm is clickable")
             if str(Settings.is_debug()) == "True":
                 Settings.debug_delay_check()
-                self.go_to_home()
-                Settings.print('skipped message (debug)')
+                Settings.print('skipping message (debug)')
+                self.message_clear()
                 return True
             Settings.dev_print("clicking confirm")
             confirm.click()
             Settings.print('OnlyFans message sent!')
             return True
         except TimeoutException:
             Settings.warn_print("timed out waiting for message confirm!")
@@ -1754,26 +1806,31 @@
             )
             scroll_nav_out_of_way = 'window.scrollBy(0, -120);'
             passed_in_driver.execute_script(scroll_by_coord)
             passed_in_driver.execute_script(scroll_nav_out_of_way)
         #
         try:
             ActionChains(self.browser).move_to_element(element).click().perform()
+            return True
         except Exception as e:
-            Settings.dev_print(e)
-            if 'firefox' in self.browser.capabilities['browserName']:
-                scroll_shim(self.browser, element)
+            # Settings.dev_print(e)
+            # if 'firefox' in self.browser.capabilities['browserName']:
             try:
+                scroll_shim(self.browser, element)
                 ActionChains(self.browser).move_to_element(element).click().perform()
             except Exception as e:
-                Settings.dev_print(e)
-            # self.browser.execute_script("arguments[0].scrollIntoView();", ele)
-                self.browser.find_element(By.TAG_NAME, 'body').send_keys(Keys.CONTROL + Keys.HOME)
-                ActionChains(self.browser).move_to_element(element).click().perform()
-
+                pass
+                # Settings.dev_print(e)
+                self.browser.execute_script("arguments[0].scrollIntoView();", element)
+                # try:
+                #     self.browser.find_element(By.TAG_NAME, 'body').send_keys(Keys.CONTROL + Keys.HOME)
+                #     ActionChains(self.browser).move_to_element(element).click().perform()
+                # except Exception as e:
+                #     Settings.dev_print(e)
+        return False
 
     ####################################################################################################
     ####################################################################################################
     ####################################################################################################
 
     # tries both and throws error for not found element internally
     def open_more_options(self):
@@ -1834,58 +1891,74 @@
             Whether or not entering the poll was successful
 
         """
 
         if str(poll) == "None" or not poll: return True
         try:
             Settings.print("Poll:")
-            Settings.print("- Duration: {}".format(poll["duration"]))
-            Settings.print("- Questions:")
-            # make sure the extra options are shown
-            # self.open_more_options()
-            # add a poll
-            Settings.dev_print("adding poll")
-            self.browser.find_element(By.CLASS_NAME, "b-make-post__actions__btns").find_elements(By.XPATH, "./child::*")[5].click()
-            # open the poll duration
-            Settings.dev_print("adding duration")
-            # self.find_element_to_click("pollDuration").click()
-            self.browser.find_element(By.CLASS_NAME, "b-post-piece__value").click()
-            # click on the correct duration number
-            Settings.dev_print("setting duration")
-            time.sleep(0.5)
-            ActionChains(self.browser).move_to_element(self.browser.find_element(By.NAME, "periodValue")).double_click().click_and_hold().send_keys(Keys.CLEAR).send_keys(str(poll["duration"])).perform()
-            # save the duration
-            Settings.dev_print("saving duration")
-            self.find_element_to_click("pollSave").click()
-            Settings.dev_print("successfully saved duration")
-            questions = self.browser.find_elements(By.CLASS_NAME, "v-text-field__slot")
-            Settings.dev_print("configuring question paths...")
-            # add extra question space
-            OFFSET = 2 # number of preexisting questions
-            if OFFSET + len(poll["questions"]) > len(questions):
-                for i in range(OFFSET + len(poll["questions"])-len(questions)):
-                    Settings.dev_print("adding question")
-                    question_ = self.find_element_to_click("pollQuestionAdd").click()
-                    Settings.dev_print("added question")
-            # find the question inputs
-            # questions_ = self.browser.find_elements(By.XPATH, Element.get_element_by_name("pollInput").getXPath())
-            questions = self.browser.find_elements(By.CLASS_NAME, "v-text-field__slot")
-            Settings.dev_print("question paths: {}".format(len(questions)))
-            # enter the questions
-            i = 0
-            Settings.dev_print("questions: {}".format(poll["questions"]))
-            for question in list(poll["questions"]):
-                Settings.print("> {}".format(question))
-                Settings.dev_print("entering question: {}".format(question))
-                questions[i].find_elements(By.XPATH, "./child::*")[0].send_keys(str(question))
-                Settings.dev_print("entered question")
+
+            # open the poll model
+            def open_model():
+                Settings.dev_print("adding poll")
+                elements = self.browser.find_elements(By.TAG_NAME, "use")
+                element = [elem for elem in elements if '#icon-poll' in str(elem.get_attribute('href'))][0]
+                ActionChains(self.browser).move_to_element(element).click().perform()
                 time.sleep(1)
-                i+=1
-            Settings.dev_print("successfully entered questions")
+
+            # open the poll duration
+            # can click anywhere near the top label
+            # TODO: finish updating any inserted wait times to be more dynamic
+            def add_duration(duration, wait=1):
+                # self.find_element_to_click("pollDuration").click()
+                Settings.print("- Duration: {}".format(duration))
+                Settings.dev_print("setting duration")
+                action = ActionChains(self.browser)
+                action.click(on_element=self.browser.find_element(By.CLASS_NAME, "b-post-piece__value"))
+                action.pause(int(wait))
+                action.send_keys(Keys.TAB)
+                action.send_keys(str(duration))
+                action.perform()
+                # save the duration
+                Settings.dev_print("saving duration")
+                self.find_element_to_click("pollSave").click()
+                Settings.dev_print("successfully saved duration")
+
+            def add_questions(questions):
+                Settings.dev_print("configuring question paths...")
+                questionsElement = self.browser.find_elements(By.CLASS_NAME, "v-text-field__slot")
+                # add extra question space
+                OFFSET = 2 # number of preexisting questionsElement
+                if OFFSET + len(questions) > len(questionsElement):
+                    for i in range(OFFSET + len(questions)-len(questionsElement)):
+                        Settings.dev_print("adding question")
+                        question_ = self.find_element_to_click("pollQuestionAdd").click()
+                        Settings.dev_print("added question")
+                # find the question inputs again
+                questionsElement = self.browser.find_elements(By.CLASS_NAME, "v-text-field__slot")
+                Settings.dev_print("question paths: {}".format(len(questionsElement)))
+                # enter the questions
+                i = 0
+                Settings.dev_print("questions: {}".format(questions))
+                Settings.print("- Questions:")
+                for question in list(questions):
+                    Settings.print("> {}".format(question))
+                    Settings.dev_print("entering question: {}".format(question))
+                    questionsElement[i].find_elements(By.XPATH, "./child::*")[0].send_keys(str(question))
+                    Settings.dev_print("entered question")
+                    time.sleep(1)
+                    i+=1
+                Settings.dev_print("successfully entered questions")
+
+            open_model()
             Settings.debug_delay_check()
+            add_duration(poll["duration"])
+            Settings.debug_delay_check()
+            add_questions(poll["questions"])
+            Settings.debug_delay_check()
+
             if str(Settings.is_debug()) == "True":
                 Settings.maybe_print("skipping poll (debug)")
                 cancel = self.find_element_to_click("pollCancel")
                 cancel.click()
             Settings.dev_print("### Poll Successful ###")
             return True
         except Exception as e:
@@ -1937,15 +2010,15 @@
         #     Settings.dev_print(e)
 
         #################### Formatted Text ####################
         Settings.print("====================")
         Settings.print("Posting:")
         Settings.print("- Files: {}".format(len(message["files"])))
         Settings.print("- Performers: {}".format(message["performers"]))
-        Settings.print("- Tags: {}".format(message["tags"]))
+        Settings.print("- Keywords: {}".format(message["keywords"]))
         Settings.print("- Text: {}".format(message["text"]))
         Settings.print("- Tweeting: {}".format(Settings.is_tweeting()))
         ## Expires, Schedule, Poll ##
         if not driver.expires(message["expiration"]): return False
         if message["schedule"] and message["schedule"].validate() and not driver.schedule(message["schedule"].get()): return False
         if message["poll"].validate() and not driver.poll(message["poll"].get()): return False
         Settings.print("====================")
@@ -2629,19 +2702,19 @@
                 raise Exception("failed to enter minutes!")
             if not self.schedule_suffix(schedule["suffix"]):
                 Settings.debug_delay_check()
                 raise Exception("failed to enter suffix!")
             # save time
             Settings.debug_delay_check()
             Settings.dev_print("saving schedule")
-            if str(Settings.is_debug()) == "True":
-                Settings.print("skipping schedule save (debug)")
-                return self.schedule_cancel()
-            else:
-                return self.schedule_save()
+            # if str(Settings.is_debug()) == "True":
+            #     Settings.print("skipping schedule save (debug)")
+            #     return self.schedule_cancel()
+            # else:
+            return self.schedule_save()
         except Exception as e:
             Driver.error_checker(e)
         # attempt to cancel window
         return self.schedule_cancel()
 
     ####################
     ##### Settings #####
@@ -3277,15 +3350,15 @@
         Settings.debug_delay_check()
         if all(successful):
             if self.error_window_upload(): Settings.dev_print("files uploaded successfully")
             else: Settings.dev_print("files probably uploaded succesfully")
             time.sleep(1) # bug prevention
             return True, False
         Settings.warn_print("a file failed to upload!")
-        return False, True
+        return False, False
 
     #################
     ##### Users #####
     #################
 
     @staticmethod
     def get_username():
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/lib/ffmpeg.py` & `OnlySnarf-4.5.2/OnlySnarf/lib/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/menu.py` & `OnlySnarf-4.5.2/OnlySnarf/menu.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import os
 import time
 import random
 import sys
 import inquirer
 ##
-from OnlySnarf.snarf import Snarf
-from OnlySnarf.lib.driver import Driver
-from OnlySnarf.classes.profile import Profile
-from OnlySnarf.util.colorize import colorize
-from OnlySnarf.util.settings import Settings
+from .snarf import Snarf
+from .lib.driver import Driver
+from .classes.profile import Profile
+from .util.colorize import colorize
+from .util.settings import Settings
 
-# from OnlySnarf.util.args import parser
+# from .util.args import parser
 # print(parser)
 # parser.add_parser('menu', help='> access the cli menu')
 
 ####################
 ##### CLI Menu #####
 ####################
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/snarf.py` & `OnlySnarf-4.5.2/OnlySnarf/snarf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/python3
 
-from OnlySnarf.lib.driver import Driver
-from OnlySnarf.util.settings import Settings
-from OnlySnarf.classes.discount import Discount
-from OnlySnarf.classes.message import Message, Post
-from OnlySnarf.classes.profile import Profile
-from OnlySnarf.classes.promotion import Promotion
-from OnlySnarf.classes.user import User
+from .lib.driver import Driver
+from .util.settings import Settings
+from .classes.discount import Discount
+from .classes.message import Message, Post
+from .classes.profile import Profile
+from .classes.promotion import Promotion
+from .classes.user import User
 
 #################
 ##### Snarf #####
 #################
 
 class Snarf:
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/args.py` & `OnlySnarf-4.5.2/OnlySnarf/util/args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/colorize.py` & `OnlySnarf-4.5.2/OnlySnarf/util/colorize.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/config.py` & `OnlySnarf-4.5.2/OnlySnarf/util/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 ## SAME as Settings.get_base_directory ##
 import getpass
 USER = getpass.getuser()
 # USER = os.getenv('USER')
 if str(os.getenv('SUDO_USER')) != "root" and str(os.getenv('SUDO_USER')) != "None":
     USER = os.getenv('SUDO_USER')
 configFile = "config.conf"
-if os.environ.get('ENV') == "test":
+
+if not os.environ.get('ENV') or os.environ.get('ENV') == "test":
   configFile = os.path.join(os.getcwd(), "OnlySnarf/conf", "test-config.conf")
 elif os.path.isfile(os.path.join("/home/{}/.onlysnarf/conf".format(USER), "config.conf")):
   configFile = os.path.join("/home/{}/.onlysnarf/conf".format(USER), "config.conf")
 else:
   configFile = os.path.join(os.getcwd(), "OnlySnarf/conf", "config.conf")
 
 config_file = configparser.ConfigParser()
@@ -31,18 +32,20 @@
     else:
       configs[section.lower()+"_"+key.lower()] = config_file[section][key].strip("\"")
       # print(key, config[section.lower()+"_"+key.lower()])
 
 config = {}
 
 # continue to overwrite values from config file with args
-from .args import args
 # print(args.items())
-for key, value in args.items():
-  config[key] = value
+# print(os.environ.get('ENV'))
+if str(os.environ.get('ENV')) != "test":
+  from .args import args
+  for key, value in args.items():
+    config[key] = value
 for key, value in configs.items():
   config[key] = value  
 
 ###############
 ## Debugging ##
 # import sys
 # print(config)
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/defaults.py` & `OnlySnarf-4.5.2/OnlySnarf/util/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 DEFAULT_GREETING = "hi! thanks for subscribing :3 do you have any preferences?"
 
 DISCOUNT_MAX_AMOUNT = 55
 DISCOUNT_MIN_AMOUNT = 5
 DISCOUNT_MAX_MONTHS = 12
 DISCOUNT_MIN_MONTHS = 1
 
-DURATION_ALLOWED = [1,3,7,30,99] # in days
+## note: '99' aka 'No Limit' no longer allowed?
+# DURATION_ALLOWED = [1,3,7,30, 99] # in days
+DURATION_ALLOWED = [1,3,7,30] # in days
 DURATION_NONE = 0
 
 EXPIRATION_MIN = 1
 EXPIRATION_MAX = 30
 EXPIRATION_NONE = 0
 
 IMAGE_LIMIT = 15
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/logger.py` & `OnlySnarf-4.5.2/OnlySnarf/util/logger.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/optional_args.py` & `OnlySnarf-4.5.2/OnlySnarf/util/optional_args.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/settings.py` & `OnlySnarf-4.5.2/OnlySnarf/util/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,40 +116,41 @@
         return cats
 
     def get_cookies_path():
         # return os.path.join(Settings.get_base_directory(), Settings.get_username(), "cookies.pkl")
         return os.path.join(Settings.get_base_directory(), "cookies.pkl")
 
     def get_price():
-        price = 0
-        try:
-            price = config["price"]
-        except Exception as e:
-            pass
-        return price
+        try: return config["price"]
+        except Exception as e: pass
+        return 0
 
     def get_price_minimum():
         return DEFAULT.PRICE_MINIMUM
 
     def get_price_maximum():
         return DEFAULT.PRICE_MAXIMUM
 
     def get_date():
-        config["date"] = Settings.format_date(config["date"])
-        if str(config["date"]) == DEFAULT.DATE and str(config["schedule"]) != DEFAULT.SCHEDULE:
-            if isinstance(config["schedule"], str):
-                config["date"] = datetime.strptime(config["schedule"], DEFAULT.SCHEDULE_FORMAT).date().strftime(DEFAULT.DATE_FORMAT)
+        try:
+            config["date"] = Settings.format_date(config["date"])
+            if str(config["date"]) == DEFAULT.DATE and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"] != "None"):
+                if isinstance(config["schedule"], str):
+                    config["date"] = datetime.strptime(config["schedule"], DEFAULT.SCHEDULE_FORMAT).date().strftime(DEFAULT.DATE_FORMAT)
+                else:
+                    config["date"] = config["schedule"].date().strftime(DEFAULT.DATE_FORMAT)
+                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
             else:
-                config["date"] = config["schedule"].date().strftime(DEFAULT.DATE_FORMAT)
-            config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
-        else:
-            config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
-        config["date"] = config["date"].strftime(DEFAULT.DATE_FORMAT)    
-        Settings.maybe_print("date (settings): {}".format(config["date"]))
-        return config["date"]
+                config["date"] = datetime.strptime(str(config["date"]), DEFAULT.DATE_FORMAT)
+            config["date"] = config["date"].strftime(DEFAULT.DATE_FORMAT)    
+            Settings.maybe_print("date (settings): {}".format(config["date"]))
+            return config["date"]
+        except Exception as e:
+            pass
+        return datetime.strptime(DEFAULT.DATE, DEFAULT.DATE_FORMAT)
 
     def get_default_greeting():
         return DEFAULT.GREETING or ""
 
     def get_default_refresher():
         return DEFAULT.REFRESHER or ""
         
@@ -163,39 +164,34 @@
         return DEFAULT.DISCOUNT_MAX_MONTHS or 0
         
     def get_discount_min_months():
         return DEFAULT.DISCOUNT_MIN_MONTHS or 0
 
     def get_download_max():
         return config["download_limit"] or DEFAULT.IMAGE_LIMIT
-        
-    def get_drive_ignore():
-        return config["notkeyword"] or None
-        
-    def get_drive_keyword():
-        return config["bykeyword"] or None
-        
+
     def get_duration():
-        return config["duration"] or None
+        try: return config["duration"]
+        except Exception as e: pass
+        return None
 
     def get_promo_duration():
-        return config["duration_promo"] or None
+        try: return config["duration_promo"]
+        except Exception as e: pass
+        return None
         
     def get_duration_allowed():
         return DEFAULT.DURATION_ALLOWED or []
         
     def get_duration_promo_allowed():
         return DEFAULT.PROMOTION_DURATION_ALLOWED or []
 
     def get_expiration():
-        try:
-            return config["expiration"]
-        except Exception as e:
-            pass
-            # print(e)
+        try: return config["expiration"]
+        except Exception as e: pass
         return DEFAULT.EXPIRATION_NONE
 
     def get_promo_expiration():
         return config["promotion_expiration"]
 
     def get_input():
         # fix pytest bug from 4.4.9
@@ -220,20 +216,15 @@
                 file = File()
                 setattr(file, "path", _input)
                 files.append(file)
         except Exception as e:
             pass
         Settings.FILES = files
         return files
-
-    def get_keywords():
-        keywords = config["keywords"] or []
-        keywords = [n.strip() for n in keywords]
-        return keywords
-
+        
     def get_logs_path(process):
         if process == "firefox":
             path_ = os.path.join(Settings.get_base_directory(), "log")
             Path(path_).mkdir(parents=True, exist_ok=True)
             return os.path.join(path_, "geckodriver.log")
         elif process == "google":
             path_ = os.path.join(Settings.get_base_directory(), "log")
@@ -251,20 +242,21 @@
         return config["sort"] or "random"
 
     def get_performers():
         try:
             performers = config["performers"] or []
             performers = [n.strip() for n in performers]
             return performers
-        except Exception as e:
-            # Settings.dev_print(e)
-            return []
+        except Exception as e: pass
+        return []
 
     def get_profile_path():
-        return config["path_profile"] or DEFAULT.PROFILE_PATH
+        try: return config["path_profile"]
+        except Exception as e: pass
+        return DEFAULT.PROFILE_PATH
 
     def get_recent_user_count():
         return config["recent_users_count"] or 0
     
     def get_promotion_limit():
         return config["promotion_limit"] or None
 
@@ -283,39 +275,36 @@
 
     def get_password_twitter():
         try: return Settings.get_user_config(Settings.get_username())["twitter_password"]
         except Exception as e: Settings.err_print(e)
         return ""
 
     def get_download_path():
-        return config["path_download"]
+        try: return config["path_download"]
+        except Exception as e: pass
+        return DEFAULT.DOWNLOAD_PATH
 
     def get_users_path():
-        return config["path_users"]
+        try: return config["path_users"]
+        except Exception as e: pass
+        return DEFAULT.USERS_PATH
 
     def get_config_path():
-        return config["path_config"]   
+        try: return config["path_config"]   
+        except Exception as e: pass
+        return DEFAULT.CONFIG_PATH
 
     def get_local_path():
         localPath = os.path.join(Settings.get_root_path(), Settings.get_username())
         from pathlib import Path
         Path(localPath).mkdir(parents=True, exist_ok=True)
         for cat in Settings.get_categories():
             Path(os.path.join(localPath, cat)).mkdir(parents=True, exist_ok=True)
         return localPath
 
-    def get_destination():
-        return config["destination"] or ""
-
-    def get_source():
-        return config["source"] or ""
-
-    def get_source_options():
-        return DEFAULT.SOURCES
-
     def get_reconnect_id():
         return config["session_id"] or ""
 
     def get_reconnect_url():
         return config["session_url"] or ""
 
     def get_remote_host():
@@ -336,49 +325,54 @@
     def get_profile_method():
         return config["profile_method"] or None
 
     def get_schedule():
         schedule = ""
         try:
             schedule = config["schedule"]
+            if str(schedule) == "None": schedule = DEFAULT.SCHEDULE
             if str(schedule) == DEFAULT.SCHEDULE:
-                schedule = datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
+                schedule = datetime.strptime(schedule, DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
             elif not isinstance(schedule, str):
                 schedule = schedule.strftime(DEFAULT.SCHEDULE_FORMAT)
             Settings.maybe_print("schedule (settings): {}".format(schedule))
             return schedule
         except Exception as e:
             pass
-        return None
+        return datetime.strptime("{} {}".format(Settings.get_date(), Settings.get_time()), DEFAULT.SCHEDULE_FORMAT).strftime(DEFAULT.SCHEDULE_FORMAT)
 
-    def get_tags():
-        tags = []
+    def get_keywords():
+        keywords = []
         try:
-            tags = config["tags"]
-            tags = [n.strip() for n in tags]
+            keywords = config["keywords"]
+            keywords = [n.strip() for n in keywords]
         except Exception as e:
             pass
             # Settings.err_print(e)
-        return tags
+        return keywords
 
     def get_text():
         return config["text"] or ""
 
     def get_time():
-        config["time"] = Settings.format_time(config["time"])        
-        if (str(config["time"]) == DEFAULT.TIME or str(config["time"]) == DEFAULT.TIME_NONE) and str(config["schedule"]) != DEFAULT.SCHEDULE:
-            Settings.dev_print("time from schedule")
-            date = datetime.strptime(str(config["schedule"]), DEFAULT.SCHEDULE_FORMAT)
-            config["time"] = datetime.strptime(str(date.time().strftime(DEFAULT.TIME_FORMAT)), DEFAULT.TIME_FORMAT)
-        else:
-            Settings.dev_print("time from config")
-            config["time"] = datetime.strptime(str(config["time"]), DEFAULT.TIME_FORMAT)
-        config["time"] = config["time"].strftime(DEFAULT.TIME_FORMAT)
-        Settings.maybe_print("time (settings): {}".format(config["time"]))
-        return config["time"]
+        try:
+            config["time"] = Settings.format_time(config["time"])        
+            if (str(config["time"]) == DEFAULT.TIME or str(config["time"]) == DEFAULT.TIME_NONE) and str(config["schedule"]) != DEFAULT.SCHEDULE and str(config["schedule"]) != "None":
+                Settings.dev_print("time from schedule")
+                date = datetime.strptime(str(config["schedule"]), DEFAULT.SCHEDULE_FORMAT)
+                config["time"] = datetime.strptime(str(date.time().strftime(DEFAULT.TIME_FORMAT)), DEFAULT.TIME_FORMAT)
+            else:
+                Settings.dev_print("time from config")
+                config["time"] = datetime.strptime(str(config["time"]), DEFAULT.TIME_FORMAT)
+            config["time"] = config["time"].strftime(DEFAULT.TIME_FORMAT)
+            Settings.maybe_print("time (settings): {}".format(config["time"]))
+            return config["time"]
+        except Exception as e:
+            pass
+        return datetime.strptime(DEFAULT.TIME, DEFAULT.TIME_FORMAT).strftime(DEFAULT.TIME_FORMAT)
 
     def get_title():
         return config["title"] or ""
         
     def get_skipped_users():
         return config["skipped_users"] or []
         
@@ -396,15 +390,17 @@
             pass
         return DEFAULT.IMAGE_LIMIT
         
     # def get_upload_max_messages():
         # return config["upload_max_messages"] or UPLOAD_MAX_MESSAGES
 
     def get_login_method():
-        return config["login"]
+        try: return config["login"]
+        except Exception as e: pass
+        return "auto"
         
     def get_upload_max_duration():
         return config["upload_max_duration"] or DEFAULT.UPLOAD_MAX_DURATION # 1 hour
 
     # comma separated string of usernames
     def get_users():
         from ..classes.user import User
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf/util/validators.py` & `OnlySnarf-4.5.2/OnlySnarf/util/validators.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/OnlySnarf.egg-info/PKG-INFO` & `OnlySnarf-4.5.2/OnlySnarf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.1
+Version: 4.5.2
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
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.1 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.2 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.1/OnlySnarf.egg-info/SOURCES.txt` & `OnlySnarf-4.5.2/OnlySnarf.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 OnlySnarf/__init__.py
 OnlySnarf/__main__.py
+OnlySnarf/api.py
 OnlySnarf/menu.py
 OnlySnarf/snarf.py
 OnlySnarf.egg-info/PKG-INFO
 OnlySnarf.egg-info/SOURCES.txt
 OnlySnarf.egg-info/dependency_links.txt
 OnlySnarf.egg-info/entry_points.txt
 OnlySnarf.egg-info/requires.txt
```

### Comparing `OnlySnarf-4.5.1/PKG-INFO` & `OnlySnarf-4.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OnlySnarf
-Version: 4.5.1
+Version: 4.5.2
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
-Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.1 Summary: OnlyFans Content
+Metadata-Version: 2.1 Name: OnlySnarf Version: 4.5.2 Summary: OnlyFans Content
 Distribution Tool Home-page: https://github.com/skeetzo/onlysnarf Author:
 Skeetzo Author-email: WebmasterSkeetzo@gmail.com Keywords:
 OnlyFans,OnlySnarf,selenium,snarf Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: System :: Emulators Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
```

### Comparing `OnlySnarf-4.5.1/README.md` & `OnlySnarf-4.5.2/README.md`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/setup.py` & `OnlySnarf-4.5.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="OnlySnarf",
-    version="4.5.1",
+    version="4.5.2",
     author="Skeetzo",
     author_email="WebmasterSkeetzo@gmail.com",
     url = 'https://github.com/skeetzo/onlysnarf',
     keywords = ['OnlyFans', 'OnlySnarf', 'selenium', 'snarf'],
     description="OnlyFans Content Distribution Tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -18,25 +18,28 @@
     include_package_data=True,
     install_requires=[
         'ffmpeg',
         'inquirer',
         'wget',
         'selenium',
         'webdriver_manager',
-        'validators'
+        'validators',
+        'flask'
         ],
     extras_require={
         'dev': [
-            'pytest'
+            'pytest',
+            'flask-unittest'
         ]
     },
     entry_points={
         'console_scripts' : [
             'onlysnarf = OnlySnarf.menu:main',
-            'snarf = OnlySnarf.snarf:main'
+            'snarf = OnlySnarf.snarf:main',
+            'snarfapi = OnlySnarf.api:main'
         ]
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: End Users/Desktop',
         'Topic :: System :: Emulators',
         'License :: OSI Approved :: MIT License',
```

### Comparing `OnlySnarf-4.5.1/tests/test_profile.py` & `OnlySnarf-4.5.2/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `OnlySnarf-4.5.1/tests/test_promotion.py` & `OnlySnarf-4.5.2/tests/test_promotion.py`

 * *Files identical despite different names*

