# Comparing `tmp/vank-1.0.2.tar.gz` & `tmp/vank-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vank-1.0.2.tar", last modified: Thu Jul 27 09:02:14 2023, max compression
+gzip compressed data, was "vank-1.0.3.tar", last modified: Mon Jul 31 09:07:34 2023, max compression
```

## Comparing `vank-1.0.2.tar` & `vank-1.0.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.043025 vank-1.0.2/
--rw-r--r--   0 vank       (501) staff       (20)     1066 2023-03-08 02:58:20.000000 vank-1.0.2/LICENSE
--rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-27 09:02:14.042399 vank-1.0.2/PKG-INFO
--rw-r--r--   0 vank       (501) staff       (20)      682 2023-07-19 09:53:59.000000 vank-1.0.2/README.md
--rw-r--r--   0 vank       (501) staff       (20)      695 2023-07-19 09:53:59.000000 vank-1.0.2/pyproject.toml
--rw-r--r--   0 vank       (501) staff       (20)       38 2023-07-27 09:02:14.043181 vank-1.0.2/setup.cfg
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.005644 vank-1.0.2/vank/
--rw-r--r--   0 vank       (501) staff       (20)       64 2023-07-19 09:53:59.000000 vank-1.0.2/vank/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     2069 2023-07-27 08:56:56.000000 vank-1.0.2/vank/__main__.py
--rw-r--r--   0 vank       (501) staff       (20)       22 2023-07-19 09:53:59.000000 vank-1.0.2/vank/__version__.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.000704 vank-1.0.2/vank/applications/
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.012358 vank-1.0.2/vank/applications/static/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.2/vank/applications/static/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1291 2023-07-21 09:45:07.000000 vank-1.0.2/vank/applications/static/control.py
--rw-r--r--   0 vank       (501) staff       (20)      238 2023-07-21 11:24:01.000000 vank-1.0.2/vank/applications/static/urls.py
--rw-r--r--   0 vank       (501) staff       (20)      382 2023-07-21 11:25:13.000000 vank-1.0.2/vank/applications/static/views.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.014099 vank-1.0.2/vank/cli/
--rw-r--r--   0 vank       (501) staff       (20)     3518 2023-07-21 11:32:42.000000 vank-1.0.2/vank/cli/init.py
--rw-r--r--   0 vank       (501) staff       (20)     1623 2023-07-24 03:20:51.000000 vank-1.0.2/vank/cli/subapp.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.019435 vank-1.0.2/vank/core/
--rw-r--r--   0 vank       (501) staff       (20)      308 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)    13049 2023-07-24 09:57:03.000000 vank-1.0.2/vank/core/app.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.021094 vank-1.0.2/vank/core/config/
--rw-r--r--   0 vank       (501) staff       (20)     1226 2023-07-21 10:21:42.000000 vank-1.0.2/vank/core/config/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     2600 2023-07-25 02:41:46.000000 vank-1.0.2/vank/core/config/base.py
--rw-r--r--   0 vank       (501) staff       (20)     5245 2023-07-21 10:37:28.000000 vank-1.0.2/vank/core/context.py
--rw-r--r--   0 vank       (501) staff       (20)      875 2023-07-24 10:11:32.000000 vank-1.0.2/vank/core/exceptions.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.022557 vank-1.0.2/vank/core/handlers/
--rw-r--r--   0 vank       (501) staff       (20)       72 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/handlers/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1275 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/handlers/exception.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.026009 vank-1.0.2/vank/core/http/
--rw-r--r--   0 vank       (501) staff       (20)      127 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     7076 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/request.py
--rw-r--r--   0 vank       (501) staff       (20)    10398 2023-07-24 09:57:03.000000 vank-1.0.2/vank/core/http/response.py
--rw-r--r--   0 vank       (501) staff       (20)     3792 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/http/status.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.029031 vank-1.0.2/vank/core/routing/
--rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.2/vank/core/routing/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     2545 2023-07-24 03:20:51.000000 vank-1.0.2/vank/core/routing/converters.py
--rw-r--r--   0 vank       (501) staff       (20)     6925 2023-07-21 10:21:42.000000 vank-1.0.2/vank/core/routing/route.py
--rw-r--r--   0 vank       (501) staff       (20)     3316 2023-07-24 09:59:29.000000 vank-1.0.2/vank/core/routing/router.py
--rw-r--r--   0 vank       (501) staff       (20)     1357 2023-07-21 10:57:22.000000 vank-1.0.2/vank/core/view.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.034292 vank-1.0.2/vank/middleware/
--rw-r--r--   0 vank       (501) staff       (20)       88 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)     1621 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/base.py
--rw-r--r--   0 vank       (501) staff       (20)     3640 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/cors.py
--rw-r--r--   0 vank       (501) staff       (20)     2941 2023-07-19 09:53:59.000000 vank-1.0.2/vank/middleware/session.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.041444 vank-1.0.2/vank/utils/
--rw-r--r--   0 vank       (501) staff       (20)      171 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/__init__.py
--rw-r--r--   0 vank       (501) staff       (20)      640 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/cli.py
--rw-r--r--   0 vank       (501) staff       (20)     6947 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/datastructures.py
--rw-r--r--   0 vank       (501) staff       (20)      996 2023-07-24 03:20:51.000000 vank-1.0.2/vank/utils/load_module.py
--rw-r--r--   0 vank       (501) staff       (20)     1083 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/log.py
--rw-r--r--   0 vank       (501) staff       (20)     2439 2023-07-21 10:37:28.000000 vank-1.0.2/vank/utils/parsers.py
--rw-r--r--   0 vank       (501) staff       (20)     2816 2023-07-21 11:02:28.000000 vank-1.0.2/vank/utils/reloader.py
--rw-r--r--   0 vank       (501) staff       (20)     1113 2023-07-19 09:53:59.000000 vank-1.0.2/vank/utils/signal.py
-drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-27 09:02:14.009480 vank-1.0.2/vank.egg-info/
--rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/PKG-INFO
--rw-r--r--   0 vank       (501) staff       (20)     1156 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/SOURCES.txt
--rw-r--r--   0 vank       (501) staff       (20)        1 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/dependency_links.txt
--rw-r--r--   0 vank       (501) staff       (20)       51 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/entry_points.txt
--rw-r--r--   0 vank       (501) staff       (20)       20 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/requires.txt
--rw-r--r--   0 vank       (501) staff       (20)        5 2023-07-27 09:02:13.000000 vank-1.0.2/vank.egg-info/top_level.txt
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.226153 vank-1.0.3/
+-rw-r--r--   0 vank       (501) staff       (20)     1066 2023-03-08 02:58:20.000000 vank-1.0.3/LICENSE
+-rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-31 09:07:34.225658 vank-1.0.3/PKG-INFO
+-rw-r--r--   0 vank       (501) staff       (20)      682 2023-07-19 09:53:59.000000 vank-1.0.3/README.md
+-rw-r--r--   0 vank       (501) staff       (20)      695 2023-07-31 09:03:26.000000 vank-1.0.3/pyproject.toml
+-rw-r--r--   0 vank       (501) staff       (20)       38 2023-07-31 09:07:34.226296 vank-1.0.3/setup.cfg
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.188510 vank-1.0.3/vank/
+-rw-r--r--   0 vank       (501) staff       (20)       64 2023-07-19 09:53:59.000000 vank-1.0.3/vank/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2069 2023-07-27 08:56:56.000000 vank-1.0.3/vank/__main__.py
+-rw-r--r--   0 vank       (501) staff       (20)       22 2023-07-31 09:03:26.000000 vank-1.0.3/vank/__version__.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.177588 vank-1.0.3/vank/applications/
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.196632 vank-1.0.3/vank/applications/static/
+-rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.3/vank/applications/static/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1291 2023-07-21 09:45:07.000000 vank-1.0.3/vank/applications/static/control.py
+-rw-r--r--   0 vank       (501) staff       (20)      247 2023-07-28 02:14:35.000000 vank-1.0.3/vank/applications/static/urls.py
+-rw-r--r--   0 vank       (501) staff       (20)      382 2023-07-21 11:25:13.000000 vank-1.0.3/vank/applications/static/views.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.198447 vank-1.0.3/vank/cli/
+-rw-r--r--   0 vank       (501) staff       (20)     3518 2023-07-21 11:32:42.000000 vank-1.0.3/vank/cli/init.py
+-rw-r--r--   0 vank       (501) staff       (20)     1631 2023-07-31 09:00:03.000000 vank-1.0.3/vank/cli/subapp.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.202870 vank-1.0.3/vank/core/
+-rw-r--r--   0 vank       (501) staff       (20)      308 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)    13049 2023-07-24 09:57:03.000000 vank-1.0.3/vank/core/app.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.204810 vank-1.0.3/vank/core/config/
+-rw-r--r--   0 vank       (501) staff       (20)     1226 2023-07-21 10:21:42.000000 vank-1.0.3/vank/core/config/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2611 2023-07-28 02:14:35.000000 vank-1.0.3/vank/core/config/base.py
+-rw-r--r--   0 vank       (501) staff       (20)     5245 2023-07-21 10:37:28.000000 vank-1.0.3/vank/core/context.py
+-rw-r--r--   0 vank       (501) staff       (20)      875 2023-07-24 10:11:32.000000 vank-1.0.3/vank/core/exceptions.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.206543 vank-1.0.3/vank/core/handlers/
+-rw-r--r--   0 vank       (501) staff       (20)       72 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/handlers/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1275 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/handlers/exception.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.210169 vank-1.0.3/vank/core/http/
+-rw-r--r--   0 vank       (501) staff       (20)      127 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/http/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     7076 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/http/request.py
+-rw-r--r--   0 vank       (501) staff       (20)    10398 2023-07-24 09:57:03.000000 vank-1.0.3/vank/core/http/response.py
+-rw-r--r--   0 vank       (501) staff       (20)     3792 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/http/status.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.214345 vank-1.0.3/vank/core/routing/
+-rw-r--r--   0 vank       (501) staff       (20)        0 2023-07-19 09:53:59.000000 vank-1.0.3/vank/core/routing/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     2545 2023-07-24 03:20:51.000000 vank-1.0.3/vank/core/routing/converters.py
+-rw-r--r--   0 vank       (501) staff       (20)     6925 2023-07-21 10:21:42.000000 vank-1.0.3/vank/core/routing/route.py
+-rw-r--r--   0 vank       (501) staff       (20)     3316 2023-07-24 09:59:29.000000 vank-1.0.3/vank/core/routing/router.py
+-rw-r--r--   0 vank       (501) staff       (20)     1357 2023-07-21 10:57:22.000000 vank-1.0.3/vank/core/view.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.217380 vank-1.0.3/vank/middleware/
+-rw-r--r--   0 vank       (501) staff       (20)       88 2023-07-19 09:53:59.000000 vank-1.0.3/vank/middleware/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)     1621 2023-07-19 09:53:59.000000 vank-1.0.3/vank/middleware/base.py
+-rw-r--r--   0 vank       (501) staff       (20)     3640 2023-07-19 09:53:59.000000 vank-1.0.3/vank/middleware/cors.py
+-rw-r--r--   0 vank       (501) staff       (20)     2941 2023-07-19 09:53:59.000000 vank-1.0.3/vank/middleware/session.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.224483 vank-1.0.3/vank/utils/
+-rw-r--r--   0 vank       (501) staff       (20)      171 2023-07-19 09:53:59.000000 vank-1.0.3/vank/utils/__init__.py
+-rw-r--r--   0 vank       (501) staff       (20)      640 2023-07-21 10:37:28.000000 vank-1.0.3/vank/utils/cli.py
+-rw-r--r--   0 vank       (501) staff       (20)     6947 2023-07-21 10:37:28.000000 vank-1.0.3/vank/utils/datastructures.py
+-rw-r--r--   0 vank       (501) staff       (20)      996 2023-07-24 03:20:51.000000 vank-1.0.3/vank/utils/load_module.py
+-rw-r--r--   0 vank       (501) staff       (20)     1083 2023-07-19 09:53:59.000000 vank-1.0.3/vank/utils/log.py
+-rw-r--r--   0 vank       (501) staff       (20)     2439 2023-07-21 10:37:28.000000 vank-1.0.3/vank/utils/parsers.py
+-rw-r--r--   0 vank       (501) staff       (20)     2816 2023-07-21 11:02:28.000000 vank-1.0.3/vank/utils/reloader.py
+-rw-r--r--   0 vank       (501) staff       (20)     1113 2023-07-19 09:53:59.000000 vank-1.0.3/vank/utils/signal.py
+drwxr-xr-x   0 vank       (501) staff       (20)        0 2023-07-31 09:07:34.193520 vank-1.0.3/vank.egg-info/
+-rw-r--r--   0 vank       (501) staff       (20)     2392 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/PKG-INFO
+-rw-r--r--   0 vank       (501) staff       (20)     1156 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/SOURCES.txt
+-rw-r--r--   0 vank       (501) staff       (20)        1 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/dependency_links.txt
+-rw-r--r--   0 vank       (501) staff       (20)       51 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/entry_points.txt
+-rw-r--r--   0 vank       (501) staff       (20)       20 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/requires.txt
+-rw-r--r--   0 vank       (501) staff       (20)        5 2023-07-31 09:07:34.000000 vank-1.0.3/vank.egg-info/top_level.txt
```

### Comparing `vank-1.0.2/LICENSE` & `vank-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/PKG-INFO` & `vank-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vank
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python Web Framework
 Author-email: WanKe <852003793@qq.com>
 License: MIT License
         
         Copyright (c) 2022 852003793
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vank-1.0.2/README.md` & `vank-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/pyproject.toml` & `vank-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "vank"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
     { name = "WanKe", email = "852003793@qq.com" },
 ]
 description = "A Python Web Framework"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `vank-1.0.2/vank/__main__.py` & `vank-1.0.3/vank/__main__.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/applications/static/control.py` & `vank-1.0.3/vank/applications/static/control.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/cli/init.py` & `vank-1.0.3/vank/cli/init.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/cli/subapp.py` & `vank-1.0.3/vank/cli/subapp.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from vank.utils.cli import BaseCommand
 
 control_template = """"""
 views_template = """
 from vank.core import SubApplication, request, response
 
-api_sub = SubApplication('api')
+{name}_sub = SubApplication('{name}')
 
 # 在此编写你的视图
 
 """
 init_template = """"""
 subapp_files = {
     'control.py': control_template,
@@ -34,15 +34,15 @@
         if not dir_:
             sub_app_dir = os.path.join(os.getcwd(), name)
         else:
             sub_app_dir = os.path.join(dir_, name)
         try:
             os.makedirs(sub_app_dir)
         except FileExistsError:
-            self.stderr.write(f'The "{name}" sub application already exists and cannot be created')
+            self.stderr.write(f'The "{name}" sub application already exists and cannot be created\n')
             sys.exit()
         for file_name, template in subapp_files.items():
             with open(os.path.join(sub_app_dir, file_name), 'w', encoding='utf-8') as f:
                 f.write(template.lstrip().format(name=name))
 
     def init_arguments(self):
         self.parser.add_argument(
```

### Comparing `vank-1.0.2/vank/core/app.py` & `vank-1.0.3/vank/core/app.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/config/__init__.py` & `vank-1.0.3/vank/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/config/base.py` & `vank-1.0.3/vank/core/config/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,9 +102,9 @@
     """检查静态路径"""
     try:
         url = getattr(sender, "STATIC_URL", None)
     except AttributeError:
         raise Exception('STATIC_URL not found in configuration')
     if not isinstance(url, str):
         raise Exception(f'The STATIC_URL type in the configuration must be str instead of {type(url).__name__}')
-    if not url.startswith('/') and not url.endswith('/'):
-        raise Exception('The start and end of the STATIC_URL must be "/"')
+    if not url.startswith('/') or url.endswith('/'):
+        raise Exception('The start of the STATIC_URL must be "/" and cannot end with "/"')
```

### Comparing `vank-1.0.2/vank/core/context.py` & `vank-1.0.3/vank/core/context.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/exceptions.py` & `vank-1.0.3/vank/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/handlers/exception.py` & `vank-1.0.3/vank/core/handlers/exception.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/http/request.py` & `vank-1.0.3/vank/core/http/request.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/http/response.py` & `vank-1.0.3/vank/core/http/response.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/http/status.py` & `vank-1.0.3/vank/core/http/status.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/routing/converters.py` & `vank-1.0.3/vank/core/routing/converters.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/routing/route.py` & `vank-1.0.3/vank/core/routing/route.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/routing/router.py` & `vank-1.0.3/vank/core/routing/router.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/core/view.py` & `vank-1.0.3/vank/core/view.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/middleware/base.py` & `vank-1.0.3/vank/middleware/base.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/middleware/cors.py` & `vank-1.0.3/vank/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/middleware/session.py` & `vank-1.0.3/vank/middleware/session.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/cli.py` & `vank-1.0.3/vank/utils/cli.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/datastructures.py` & `vank-1.0.3/vank/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/load_module.py` & `vank-1.0.3/vank/utils/load_module.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/log.py` & `vank-1.0.3/vank/utils/log.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/parsers.py` & `vank-1.0.3/vank/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/reloader.py` & `vank-1.0.3/vank/utils/reloader.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank/utils/signal.py` & `vank-1.0.3/vank/utils/signal.py`

 * *Files identical despite different names*

### Comparing `vank-1.0.2/vank.egg-info/PKG-INFO` & `vank-1.0.3/vank.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vank
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python Web Framework
 Author-email: WanKe <852003793@qq.com>
 License: MIT License
         
         Copyright (c) 2022 852003793
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `vank-1.0.2/vank.egg-info/SOURCES.txt` & `vank-1.0.3/vank.egg-info/SOURCES.txt`

 * *Files identical despite different names*

