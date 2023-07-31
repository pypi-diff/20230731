# Comparing `tmp/pynose-1.4.6.tar.gz` & `tmp/pynose-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynose-1.4.6.tar", last modified: Sat Jul  8 03:29:15 2023, max compression
+gzip compressed data, was "pynose-1.4.7.tar", last modified: Mon Jul 31 02:20:42 2023, max compression
```

## Comparing `pynose-1.4.6.tar` & `pynose-1.4.7.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554846 pynose-1.4.6/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.546500 pynose-1.4.6/.github/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.548050 pynose-1.4.6/.github/workflows/
--rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.6/.github/workflows/python-package-legacy.yml
--rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.6/.github/workflows/python-package.yml
--rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.6/.gitignore
--rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.6/LICENSE
--rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.6/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-08 03:29:15.554941 pynose-1.4.6/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)    17086 2023-07-08 03:28:10.000000 pynose-1.4.6/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.548629 pynose-1.4.6/bin/
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.6/bin/nosetests
--rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.6/bin/pynose
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.551184 pynose-1.4.6/nose/
--rw-r--r--   0 michael    (501) staff       (20)      643 2023-07-07 23:53:47.000000 pynose-1.4.6/nose/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)      144 2023-07-07 23:40:25.000000 pynose-1.4.6/nose/__main__.py
--rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-07-08 03:28:10.000000 pynose-1.4.6/nose/__version__.py
--rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/case.py
--rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.6/nose/commands.py
--rw-r--r--   0 michael    (501) staff       (20)    24529 2023-03-02 15:02:07.000000 pynose-1.4.6/nose/config.py
--rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.6/nose/core.py
--rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.6/nose/exc.py
--rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.6/nose/failure.py
--rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/importer.py
--rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.6/nose/inspector.py
--rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.6/nose/loader.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.553593 pynose-1.4.6/nose/plugins/
--rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.6/nose/plugins/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.6/nose/plugins/allmodules.py
--rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.6/nose/plugins/attrib.py
--rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.6/nose/plugins/base.py
--rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.6/nose/plugins/builtin.py
--rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.6/nose/plugins/capture.py
--rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.6/nose/plugins/collect.py
--rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.6/nose/plugins/cover.py
--rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.6/nose/plugins/debug.py
--rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.6/nose/plugins/deprecated.py
--rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.6/nose/plugins/doctests.py
--rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.6/nose/plugins/errorclass.py
--rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.6/nose/plugins/failuredetail.py
--rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.6/nose/plugins/isolate.py
--rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.6/nose/plugins/logcapture.py
--rw-r--r--   0 michael    (501) staff       (20)    15004 2023-07-08 03:28:10.000000 pynose-1.4.6/nose/plugins/manager.py
--rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.6/nose/plugins/multiprocess.py
--rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.6/nose/plugins/plugintest.py
--rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.6/nose/plugins/skip.py
--rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.6/nose/plugins/testid.py
--rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.6/nose/plugins/xunit.py
--rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.6/nose/proxy.py
--rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.6/nose/pyversion.py
--rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.6/nose/result.py
--rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.6/nose/selector.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.553828 pynose-1.4.6/nose/sphinx/
--rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.6/nose/sphinx/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.6/nose/sphinx/pluginopts.py
--rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.6/nose/suite.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554164 pynose-1.4.6/nose/tools/
--rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.6/nose/tools/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.6/nose/tools/nontrivial.py
--rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.6/nose/tools/trivial.py
--rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.6/nose/twistedtools.py
--rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.6/nose/usage.txt
--rw-r--r--   0 michael    (501) staff       (20)    18927 2023-05-24 22:14:10.000000 pynose-1.4.6/nose/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-08 03:29:15.554739 pynose-1.4.6/pynose.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1273 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       77 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-08 03:29:15.000000 pynose-1.4.6/pynose.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       86 2023-07-08 03:29:15.555207 pynose-1.4.6/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     4838 2023-07-08 03:28:10.000000 pynose-1.4.6/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.451276 pynose-1.4.7/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.442920 pynose-1.4.7/.github/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.444496 pynose-1.4.7/.github/workflows/
+-rw-r--r--   0 michael    (501) staff       (20)     1332 2023-03-01 21:40:49.000000 pynose-1.4.7/.github/workflows/python-package-legacy.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1357 2023-03-01 21:40:46.000000 pynose-1.4.7/.github/workflows/python-package.yml
+-rw-r--r--   0 michael    (501) staff       (20)     1799 2023-02-28 01:46:25.000000 pynose-1.4.7/.gitignore
+-rw-r--r--   0 michael    (501) staff       (20)     1070 2023-02-28 01:46:25.000000 pynose-1.4.7/LICENSE
+-rw-r--r--   0 michael    (501) staff       (20)      135 2023-02-28 03:14:47.000000 pynose-1.4.7/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-31 02:20:42.451355 pynose-1.4.7/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)    17086 2023-07-08 03:28:10.000000 pynose-1.4.7/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.444932 pynose-1.4.7/bin/
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.7/bin/nosetests
+-rwxr-xr-x   0 michael    (501) staff       (20)       84 2012-09-29 08:18:54.000000 pynose-1.4.7/bin/pynose
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.447395 pynose-1.4.7/nose/
+-rw-r--r--   0 michael    (501) staff       (20)      643 2023-07-07 23:53:47.000000 pynose-1.4.7/nose/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)      144 2023-07-07 23:40:25.000000 pynose-1.4.7/nose/__main__.py
+-rwxr-xr-x   0 michael    (501) staff       (20)       44 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/__version__.py
+-rw-r--r--   0 michael    (501) staff       (20)    11881 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/case.py
+-rw-r--r--   0 michael    (501) staff       (20)     5538 2023-03-02 14:29:59.000000 pynose-1.4.7/nose/commands.py
+-rw-r--r--   0 michael    (501) staff       (20)    24529 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/config.py
+-rw-r--r--   0 michael    (501) staff       (20)    12087 2023-03-02 13:46:19.000000 pynose-1.4.7/nose/core.py
+-rw-r--r--   0 michael    (501) staff       (20)      390 2023-02-26 21:55:15.000000 pynose-1.4.7/nose/exc.py
+-rw-r--r--   0 michael    (501) staff       (20)     1258 2023-02-26 21:54:35.000000 pynose-1.4.7/nose/failure.py
+-rw-r--r--   0 michael    (501) staff       (20)     9007 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/importer.py
+-rw-r--r--   0 michael    (501) staff       (20)     5535 2023-03-02 04:00:31.000000 pynose-1.4.7/nose/inspector.py
+-rw-r--r--   0 michael    (501) staff       (20)    21758 2023-03-02 14:53:46.000000 pynose-1.4.7/nose/loader.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.449999 pynose-1.4.7/nose/plugins/
+-rw-r--r--   0 michael    (501) staff       (20)     5421 2023-03-02 16:20:15.000000 pynose-1.4.7/nose/plugins/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     1007 2023-03-02 15:57:56.000000 pynose-1.4.7/nose/plugins/allmodules.py
+-rw-r--r--   0 michael    (501) staff       (20)     8189 2023-03-02 16:10:06.000000 pynose-1.4.7/nose/plugins/attrib.py
+-rw-r--r--   0 michael    (501) staff       (20)    23205 2023-04-30 16:29:19.000000 pynose-1.4.7/nose/plugins/base.py
+-rw-r--r--   0 michael    (501) staff       (20)     1024 2023-02-26 20:00:18.000000 pynose-1.4.7/nose/plugins/builtin.py
+-rw-r--r--   0 michael    (501) staff       (20)     3280 2023-05-03 01:50:30.000000 pynose-1.4.7/nose/plugins/capture.py
+-rw-r--r--   0 michael    (501) staff       (20)     2739 2023-03-02 15:58:25.000000 pynose-1.4.7/nose/plugins/collect.py
+-rw-r--r--   0 michael    (501) staff       (20)    10668 2023-03-02 16:16:16.000000 pynose-1.4.7/nose/plugins/cover.py
+-rw-r--r--   0 michael    (501) staff       (20)     2163 2023-03-02 15:14:11.000000 pynose-1.4.7/nose/plugins/debug.py
+-rw-r--r--   0 michael    (501) staff       (20)     1435 2023-03-02 15:57:16.000000 pynose-1.4.7/nose/plugins/deprecated.py
+-rw-r--r--   0 michael    (501) staff       (20)    16001 2023-03-02 16:44:33.000000 pynose-1.4.7/nose/plugins/doctests.py
+-rw-r--r--   0 michael    (501) staff       (20)     6390 2023-03-02 15:59:48.000000 pynose-1.4.7/nose/plugins/errorclass.py
+-rw-r--r--   0 michael    (501) staff       (20)     1495 2023-03-02 15:59:22.000000 pynose-1.4.7/nose/plugins/failuredetail.py
+-rw-r--r--   0 michael    (501) staff       (20)     3401 2023-02-28 06:09:15.000000 pynose-1.4.7/nose/plugins/isolate.py
+-rw-r--r--   0 michael    (501) staff       (20)     8666 2023-03-02 15:25:15.000000 pynose-1.4.7/nose/plugins/logcapture.py
+-rw-r--r--   0 michael    (501) staff       (20)    15004 2023-07-08 03:28:10.000000 pynose-1.4.7/nose/plugins/manager.py
+-rw-r--r--   0 michael    (501) staff       (20)    31375 2023-03-02 19:07:14.000000 pynose-1.4.7/nose/plugins/multiprocess.py
+-rw-r--r--   0 michael    (501) staff       (20)    13083 2023-03-02 15:51:36.000000 pynose-1.4.7/nose/plugins/plugintest.py
+-rw-r--r--   0 michael    (501) staff       (20)     1487 2023-03-02 16:00:21.000000 pynose-1.4.7/nose/plugins/skip.py
+-rw-r--r--   0 michael    (501) staff       (20)     9318 2023-03-02 16:04:30.000000 pynose-1.4.7/nose/plugins/testid.py
+-rw-r--r--   0 michael    (501) staff       (20)    11044 2023-03-02 15:37:08.000000 pynose-1.4.7/nose/plugins/xunit.py
+-rw-r--r--   0 michael    (501) staff       (20)     5964 2023-02-28 05:29:54.000000 pynose-1.4.7/nose/proxy.py
+-rw-r--r--   0 michael    (501) staff       (20)     3665 2023-03-02 14:54:42.000000 pynose-1.4.7/nose/pyversion.py
+-rw-r--r--   0 michael    (501) staff       (20)     5808 2023-05-02 02:01:52.000000 pynose-1.4.7/nose/result.py
+-rw-r--r--   0 michael    (501) staff       (20)     9081 2023-03-02 14:46:58.000000 pynose-1.4.7/nose/selector.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.450242 pynose-1.4.7/nose/sphinx/
+-rw-r--r--   0 michael    (501) staff       (20)        5 2022-11-25 20:24:40.000000 pynose-1.4.7/nose/sphinx/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     5348 2023-03-02 17:41:29.000000 pynose-1.4.7/nose/sphinx/pluginopts.py
+-rw-r--r--   0 michael    (501) staff       (20)    18253 2023-03-02 15:00:20.000000 pynose-1.4.7/nose/suite.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.450595 pynose-1.4.7/nose/tools/
+-rw-r--r--   0 michael    (501) staff       (20)      465 2023-02-26 23:14:39.000000 pynose-1.4.7/nose/tools/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4080 2023-02-28 03:39:28.000000 pynose-1.4.7/nose/tools/nontrivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     1083 2023-02-28 03:40:01.000000 pynose-1.4.7/nose/tools/trivial.py
+-rw-r--r--   0 michael    (501) staff       (20)     4981 2023-03-02 14:56:46.000000 pynose-1.4.7/nose/twistedtools.py
+-rw-r--r--   0 michael    (501) staff       (20)     3698 2023-02-28 06:39:10.000000 pynose-1.4.7/nose/usage.txt
+-rw-r--r--   0 michael    (501) staff       (20)    18927 2023-07-31 02:19:59.000000 pynose-1.4.7/nose/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-07-31 02:20:42.451176 pynose-1.4.7/pynose.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    18543 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1273 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       77 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)        5 2023-07-31 02:20:42.000000 pynose-1.4.7/pynose.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       86 2023-07-31 02:20:42.451605 pynose-1.4.7/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     5413 2023-07-31 02:19:59.000000 pynose-1.4.7/setup.py
```

### Comparing `pynose-1.4.6/.github/workflows/python-package-legacy.yml` & `pynose-1.4.7/.github/workflows/python-package-legacy.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/.github/workflows/python-package.yml` & `pynose-1.4.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/.gitignore` & `pynose-1.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/LICENSE` & `pynose-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/PKG-INFO` & `pynose-1.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.6
+Version: 1.4.7
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynose Version: 1.4.6 Summary: pynose fixes nose to
+Metadata-Version: 2.1 Name: pynose Version: 1.4.7 Summary: pynose fixes nose to
 extend unittest and make testing easier Home-page: https://github.com/mdmintz/
 pynose Author: Michael Mintz Author-email: mdmintz@gmail.com License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files Project-URL:
 PyPI, https://pypi.org/project/pynose/ Project-URL: Source, https://github.com/
 mdmintz/pynose Project-URL: Documentation, https://nose.readthedocs.io/en/
 latest/ Keywords: test unittest doctest automatic discovery Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
```

### Comparing `pynose-1.4.6/README.md` & `pynose-1.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/__init__.py` & `pynose-1.4.7/nose/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/case.py` & `pynose-1.4.7/nose/case.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/commands.py` & `pynose-1.4.7/nose/commands.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/config.py` & `pynose-1.4.7/nose/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,22 +335,22 @@
         logger = logging.getLogger('nose')
         logger.propagate = 0
         found = False
         if self.debugLog:
             debugLogAbsPath = os.path.abspath(self.debugLog)
             for h in logger.handlers:
                 if (
-                    type(h) == logging.FileHandler
+                    type(h) is logging.FileHandler
                     and h.baseFilename == debugLogAbsPath
                 ):
                     found = True
         else:
             for h in logger.handlers:
                 if (
-                    type(h) == logging.StreamHandler
+                    type(h) is logging.StreamHandler
                     and h.stream == self.logStream
                 ):
                     found = True
         if not found:
             logger.addHandler(handler)
         lvl = logging.WARNING
         if self.verbosity >= 5:
```

### Comparing `pynose-1.4.6/nose/core.py` & `pynose-1.4.7/nose/core.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/failure.py` & `pynose-1.4.7/nose/failure.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/importer.py` & `pynose-1.4.7/nose/importer.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/inspector.py` & `pynose-1.4.7/nose/inspector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/loader.py` & `pynose-1.4.7/nose/loader.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/__init__.py` & `pynose-1.4.7/nose/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/allmodules.py` & `pynose-1.4.7/nose/plugins/allmodules.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/attrib.py` & `pynose-1.4.7/nose/plugins/attrib.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/base.py` & `pynose-1.4.7/nose/plugins/base.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/builtin.py` & `pynose-1.4.7/nose/plugins/builtin.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/capture.py` & `pynose-1.4.7/nose/plugins/capture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/collect.py` & `pynose-1.4.7/nose/plugins/collect.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/cover.py` & `pynose-1.4.7/nose/plugins/cover.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/debug.py` & `pynose-1.4.7/nose/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/deprecated.py` & `pynose-1.4.7/nose/plugins/deprecated.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/doctests.py` & `pynose-1.4.7/nose/plugins/doctests.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/errorclass.py` & `pynose-1.4.7/nose/plugins/errorclass.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/failuredetail.py` & `pynose-1.4.7/nose/plugins/failuredetail.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/isolate.py` & `pynose-1.4.7/nose/plugins/isolate.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/logcapture.py` & `pynose-1.4.7/nose/plugins/logcapture.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/manager.py` & `pynose-1.4.7/nose/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/multiprocess.py` & `pynose-1.4.7/nose/plugins/multiprocess.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/plugintest.py` & `pynose-1.4.7/nose/plugins/plugintest.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/skip.py` & `pynose-1.4.7/nose/plugins/skip.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/testid.py` & `pynose-1.4.7/nose/plugins/testid.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/plugins/xunit.py` & `pynose-1.4.7/nose/plugins/xunit.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/proxy.py` & `pynose-1.4.7/nose/proxy.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/pyversion.py` & `pynose-1.4.7/nose/pyversion.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/result.py` & `pynose-1.4.7/nose/result.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/selector.py` & `pynose-1.4.7/nose/selector.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/sphinx/pluginopts.py` & `pynose-1.4.7/nose/sphinx/pluginopts.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/suite.py` & `pynose-1.4.7/nose/suite.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/tools/nontrivial.py` & `pynose-1.4.7/nose/tools/nontrivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/tools/trivial.py` & `pynose-1.4.7/nose/tools/trivial.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/twistedtools.py` & `pynose-1.4.7/nose/twistedtools.py`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/usage.txt` & `pynose-1.4.7/nose/usage.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/nose/util.py` & `pynose-1.4.7/nose/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     ...     def get(self):
     ...         return 1
     ...     get = property(get)
     >>> isproperty(Foo.got)
     False
     >>> isproperty(Foo.get)
     True """
-    return type(obj) == property
+    return type(obj) is property
 
 
 def getfilename(package, relativeTo=None):
     """Find the python source file for a package, relative to a
     particular directory (defaults to current working directory if not
     given)."""
     if relativeTo is None:
```

### Comparing `pynose-1.4.6/pynose.egg-info/PKG-INFO` & `pynose-1.4.7/pynose.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynose
-Version: 1.4.6
+Version: 1.4.7
 Summary: pynose fixes nose to extend unittest and make testing easier
 Home-page: https://github.com/mdmintz/pynose
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files
 Project-URL: PyPI, https://pypi.org/project/pynose/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynose Version: 1.4.6 Summary: pynose fixes nose to
+Metadata-Version: 2.1 Name: pynose Version: 1.4.7 Summary: pynose fixes nose to
 extend unittest and make testing easier Home-page: https://github.com/mdmintz/
 pynose Author: Michael Mintz Author-email: mdmintz@gmail.com License: MIT
 Project-URL: Download, https://pypi.org/project/pynose/#files Project-URL:
 PyPI, https://pypi.org/project/pynose/ Project-URL: Source, https://github.com/
 mdmintz/pynose Project-URL: Documentation, https://nose.readthedocs.io/en/
 latest/ Keywords: test unittest doctest automatic discovery Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
```

### Comparing `pynose-1.4.6/pynose.egg-info/SOURCES.txt` & `pynose-1.4.7/pynose.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynose-1.4.6/setup.py` & `pynose-1.4.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -41,23 +41,31 @@
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'build>=0.10.0'")
+        os.system("python -m pip install --upgrade 'build'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        os.system("python -m pip install --upgrade 'pkginfo'")
         print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
+        os.system("python -m pip install --upgrade 'readme-renderer'")
+        print("\n*** Installing jaraco.classes: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'jaraco.classes'")
+        print("\n*** Installing more-itertools: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'more-itertools'")
+        print("\n*** Installing zipp: *** (Required for PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'zipp'")
+        print("\n*** Installing importlib-metadata: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'importlib-metadata'")
+        print("\n*** Installing keyring, requests-toolbelt: *** (For PyPI)\n")
+        os.system("python -m pip install --upgrade keyring requests-toolbelt")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade 'twine>=4.0.2'")
-        print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
-        os.system("python -m pip install --upgrade tqdm")
+        os.system("python -m pip install --upgrade 'twine'")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
         os.system("python -m twine upload dist/*")  # Requires ~/.pypirc Keys
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
```

