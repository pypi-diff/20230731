# Comparing `tmp/MySchedule.py-1.0.4.tar.gz` & `tmp/MySchedule.py-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySchedule.py-1.0.4.tar", last modified: Mon Feb  6 09:13:40 2023, max compression
+gzip compressed data, was "MySchedule.py-1.0.5.tar", last modified: Mon Jul 31 09:26:23 2023, max compression
```

## Comparing `MySchedule.py-1.0.4.tar` & `MySchedule.py-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 09:13:40.656664 MySchedule.py-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 09:13:40.656664 MySchedule.py-1.0.4/MySchedule.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-02-06 09:13:40.000000 MySchedule.py-1.0.4/MySchedule.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      270 2023-02-06 09:13:40.000000 MySchedule.py-1.0.4/MySchedule.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-06 09:13:40.000000 MySchedule.py-1.0.4/MySchedule.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-02-06 09:13:40.000000 MySchedule.py-1.0.4/MySchedule.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-02-06 09:13:40.000000 MySchedule.py-1.0.4/MySchedule.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      700 2023-02-06 09:13:40.656664 MySchedule.py-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      421 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 09:13:40.656664 MySchedule.py-1.0.4/schedule/
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5969 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/schedule/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      948 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/schedule/structures.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-02-06 09:13:40.656664 MySchedule.py-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-02-06 09:13:15.000000 MySchedule.py-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/MySchedule.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      270 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-31 09:26:23.000000 MySchedule.py-1.0.5/MySchedule.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/schedule/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11523 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1975 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/schedule/structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-31 09:26:23.942053 MySchedule.py-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-07-31 09:26:11.000000 MySchedule.py-1.0.5/setup.py
```

### Comparing `MySchedule.py-1.0.4/LICENSE` & `MySchedule.py-1.0.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Olijeffers0n
+Copyright (c) 2023 Olijeffers0n
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `MySchedule.py-1.0.4/setup.py` & `MySchedule.py-1.0.5/setup.py`

 * *Files identical despite different names*

