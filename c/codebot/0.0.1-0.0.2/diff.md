# Comparing `tmp/codebot-0.0.1.tar.gz` & `tmp/codebot-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.1.tar", last modified: Mon Jul 31 03:18:36 2023, max compression
+gzip compressed data, was "codebot-0.0.2.tar", last modified: Mon Jul 31 03:22:09 2023, max compression
```

## Comparing `codebot-0.0.1.tar` & `codebot-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.554797 codebot-0.0.1/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:18:36.554394 codebot-0.0.1/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.548959 codebot-0.0.1/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      297 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:18:36.000000 codebot-0.0.1/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:18:36.554966 codebot-0.0.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      225 2023-07-31 03:18:18.000000 codebot-0.0.1/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.552021 codebot-0.0.1/src/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.1/src/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.1/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12714 2023-07-31 02:19:31.000000 codebot-0.0.1/src/app_cn.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:18:36.553813 codebot-0.0.1/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.1/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.1/src/functions/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.1/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.1/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:22:09.631595 codebot-0.0.2/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:22:09.630813 codebot-0.0.2/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:22:09.602944 codebot-0.0.2/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      327 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      107 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:22:09.000000 codebot-0.0.2/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:22:09.631901 codebot-0.0.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      439 2023-07-31 03:21:57.000000 codebot-0.0.2/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:22:09.606133 codebot-0.0.2/src/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.2/src/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.2/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12714 2023-07-31 02:19:31.000000 codebot-0.0.2/src/app_cn.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:22:09.609238 codebot-0.0.2/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.2/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.2/src/functions/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.2/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.2/src/get_text.py
```

### Comparing `codebot-0.0.1/src/__init__.py` & `codebot-0.0.2/src/__init__.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.1/src/app.py` & `codebot-0.0.2/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.1/src/app_cn.py` & `codebot-0.0.2/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.1/src/functions/FunctionManager.py` & `codebot-0.0.2/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.1/src/get_text.py` & `codebot-0.0.2/src/get_text.py`

 * *Files identical despite different names*

