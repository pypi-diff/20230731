# Comparing `tmp/codebot-0.0.4.tar.gz` & `tmp/codebot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codebot-0.0.4.tar", last modified: Mon Jul 31 03:38:24 2023, max compression
+gzip compressed data, was "codebot-0.0.5.tar", last modified: Mon Jul 31 03:41:16 2023, max compression
```

## Comparing `codebot-0.0.4.tar` & `codebot-0.0.5.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.339482 codebot-0.0.4/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.4/MANIFEST.in
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:38:24.339064 codebot-0.0.4/PKG-INFO
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.313538 codebot-0.0.4/codebot.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2183 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      107 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:38:24.000000 codebot-0.0.4/codebot.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:38:24.339683 codebot-0.0.4/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      487 2023-07-31 03:38:22.000000 codebot-0.0.4/setup.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.315818 codebot-0.0.4/src/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.316194 codebot-0.0.4/src/.chainlit/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1204 2023-07-31 02:17:30.000000 codebot-0.0.4/src/.chainlit/config.toml
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.4/src/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.320700 codebot-0.0.4/src/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4741 2023-07-31 03:17:06.000000 codebot-0.0.4/src/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.4/src/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.4/src/__pycache__/app.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.4/src/__pycache__/app.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.4/src/__pycache__/app_cn.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    17324 2023-07-31 03:01:37.000000 codebot-0.0.4/src/__pycache__/app_cn.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.4/src/__pycache__/get_text.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.4/src/__pycache__/get_text.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.4/src/__pycache__/get_text.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.4/src/app.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    12827 2023-07-31 03:25:24.000000 codebot-0.0.4/src/app_cn.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      761 2023-07-31 01:29:27.000000 codebot-0.0.4/src/chainlit.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.321908 codebot-0.0.4/src/functions/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.4/src/functions/FunctionManager.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.4/src/functions/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.324589 codebot-0.0.4/src/functions/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.4/src/functions/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.4/src/functions/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.4/src/functions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.4/src/get_env.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.4/src/get_text.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.325508 codebot-0.0.4/src/language/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.4/src/language/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.4/src/language/en.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.4/src/language/zh_CN.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.325842 codebot-0.0.4/src/plugins/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.4/src/plugins/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.326463 codebot-0.0.4/src/plugins/common/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.327666 codebot-0.0.4/src/plugins/common/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/common/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/common/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.328339 codebot-0.0.4/src/plugins/mysql/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/mysql/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/mysql/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.329298 codebot-0.0.4/src/plugins/python/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.331316 codebot-0.0.4/src/plugins/python/__pycache__/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-310.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-311.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-38.pyc
--rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/python/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/python/executor.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/python/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.332803 codebot-0.0.4/src/plugins/serverplugin_unfinsh/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/serverplugin_unfinsh/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/serverplugin_unfinsh/functions.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/serverplugin_unfinsh/my_apis.json
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.334410 codebot-0.0.4/src/plugins/vue/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/vue/config.json
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.4/src/plugins/vue/functions.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:38:24.338301 codebot-0.0.4/src/tmp/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.4/src/tmp/1690769899.3643498.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.4/src/tmp/1690769912.7088609.png
--rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.4/src/tmp/sin_function.gif
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.4/src/tmp/sin_function.png
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.397329 codebot-0.0.5/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 03:36:24.000000 codebot-0.0.5/MANIFEST.in
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:41:16.396884 codebot-0.0.5/PKG-INFO
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.338219 codebot-0.0.5/codebot.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       51 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2183 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       37 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      115 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-07-31 03:41:16.000000 codebot-0.0.5/codebot.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-31 03:41:16.397502 codebot-0.0.5/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      505 2023-07-31 03:41:13.000000 codebot-0.0.5/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.342728 codebot-0.0.5/src/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.343668 codebot-0.0.5/src/.chainlit/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1204 2023-07-31 02:17:30.000000 codebot-0.0.5/src/.chainlit/config.toml
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3134 2023-07-31 03:17:02.000000 codebot-0.0.5/src/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.352409 codebot-0.0.5/src/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4741 2023-07-31 03:17:06.000000 codebot-0.0.5/src/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1564 2023-07-31 02:11:50.000000 codebot-0.0.5/src/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8807 2023-07-31 02:09:03.000000 codebot-0.0.5/src/__pycache__/app.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8642 2023-07-31 01:42:17.000000 codebot-0.0.5/src/__pycache__/app.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8791 2023-07-31 02:11:52.000000 codebot-0.0.5/src/__pycache__/app_cn.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    17324 2023-07-31 03:01:37.000000 codebot-0.0.5/src/__pycache__/app_cn.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      705 2023-07-31 01:56:52.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1312 2023-07-31 02:17:32.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      681 2023-07-31 01:42:17.000000 codebot-0.0.5/src/__pycache__/get_text.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12727 2023-07-31 02:08:58.000000 codebot-0.0.5/src/app.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    12827 2023-07-31 03:25:24.000000 codebot-0.0.5/src/app_cn.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      761 2023-07-31 01:29:27.000000 codebot-0.0.5/src/chainlit.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.354840 codebot-0.0.5/src/functions/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7099 2023-07-31 01:24:31.000000 codebot-0.0.5/src/functions/FunctionManager.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:24:31.000000 codebot-0.0.5/src/functions/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.361907 codebot-0.0.5/src/functions/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4657 2023-07-31 01:56:52.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7501 2023-07-31 02:17:32.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4616 2023-07-31 01:40:17.000000 codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      169 2023-07-31 01:56:52.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      185 2023-07-31 02:17:32.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      167 2023-07-31 01:40:17.000000 codebot-0.0.5/src/functions/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 01:45:57.000000 codebot-0.0.5/src/get_env.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      757 2023-07-31 01:41:53.000000 codebot-0.0.5/src/get_text.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.364034 codebot-0.0.5/src/language/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:12.000000 codebot-0.0.5/src/language/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      995 2023-07-31 01:24:31.000000 codebot-0.0.5/src/language/en.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      902 2023-07-31 01:24:31.000000 codebot-0.0.5/src/language/zh_CN.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.364903 codebot-0.0.5/src/plugins/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:28:23.000000 codebot-0.0.5/src/plugins/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.366392 codebot-0.0.5/src/plugins/common/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.369367 codebot-0.0.5/src/plugins/common/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      792 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1158 2023-07-31 02:17:34.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      779 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/common/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4122 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/common/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.372013 codebot-0.0.5/src/plugins/mysql/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/mysql/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2241 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/mysql/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.374651 codebot-0.0.5/src/plugins/python/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.379726 codebot-0.0.5/src/plugins/python/__pycache__/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4054 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7647 2023-07-31 02:17:32.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4048 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2823 2023-07-31 01:56:52.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-310.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4361 2023-07-31 02:17:32.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-311.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2815 2023-07-31 01:42:17.000000 codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-38.pyc
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       24 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     5897 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/executor.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/python/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.382179 codebot-0.0.5/src/plugins/serverplugin_unfinsh/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3461 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/functions.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   538405 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/serverplugin_unfinsh/my_apis.json
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.387552 codebot-0.0.5/src/plugins/vue/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       25 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/vue/config.json
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4025 2023-07-31 01:24:31.000000 codebot-0.0.5/src/plugins/vue/functions.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-31 03:41:16.395895 codebot-0.0.5/src/tmp/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    28901 2023-07-31 02:18:19.000000 codebot-0.0.5/src/tmp/1690769899.3643498.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    22971 2023-07-31 02:18:32.000000 codebot-0.0.5/src/tmp/1690769912.7088609.png
+-rw-r--r--   0 luzhipeng   (501) staff       (20)   534693 2023-07-31 02:18:47.000000 codebot-0.0.5/src/tmp/sin_function.gif
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29483 2023-07-31 02:18:19.000000 codebot-0.0.5/src/tmp/sin_function.png
```

### Comparing `codebot-0.0.4/codebot.egg-info/SOURCES.txt` & `codebot-0.0.5/codebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/.chainlit/config.toml` & `codebot-0.0.5/src/.chainlit/config.toml`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__init__.py` & `codebot-0.0.5/src/__init__.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/__init__.cpython-311.pyc` & `codebot-0.0.5/src/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/__init__.cpython-38.pyc` & `codebot-0.0.5/src/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/app.cpython-310.pyc` & `codebot-0.0.5/src/__pycache__/app.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/app.cpython-38.pyc` & `codebot-0.0.5/src/__pycache__/app.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/app_cn.cpython-310.pyc` & `codebot-0.0.5/src/__pycache__/app_cn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/app_cn.cpython-311.pyc` & `codebot-0.0.5/src/__pycache__/app_cn.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/get_text.cpython-310.pyc` & `codebot-0.0.5/src/__pycache__/get_text.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/get_text.cpython-311.pyc` & `codebot-0.0.5/src/__pycache__/get_text.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/__pycache__/get_text.cpython-38.pyc` & `codebot-0.0.5/src/__pycache__/get_text.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/app.py` & `codebot-0.0.5/src/app.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/app_cn.py` & `codebot-0.0.5/src/app_cn.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/chainlit.md` & `codebot-0.0.5/src/chainlit.md`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/functions/FunctionManager.py` & `codebot-0.0.5/src/functions/FunctionManager.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-310.pyc` & `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-311.pyc` & `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/functions/__pycache__/FunctionManager.cpython-38.pyc` & `codebot-0.0.5/src/functions/__pycache__/FunctionManager.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/get_text.py` & `codebot-0.0.5/src/get_text.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/language/en.json` & `codebot-0.0.5/src/language/en.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/language/zh_CN.json` & `codebot-0.0.5/src/language/zh_CN.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/common/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.5/src/plugins/common/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/common/functions.py` & `codebot-0.0.5/src/plugins/common/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/mysql/functions.py` & `codebot-0.0.5/src/plugins/mysql/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-310.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-311.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/executor.cpython-38.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/executor.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-310.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-311.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/__pycache__/functions.cpython-38.pyc` & `codebot-0.0.5/src/plugins/python/__pycache__/functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/executor.py` & `codebot-0.0.5/src/plugins/python/executor.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/python/functions.py` & `codebot-0.0.5/src/plugins/python/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/serverplugin_unfinsh/functions.py` & `codebot-0.0.5/src/plugins/serverplugin_unfinsh/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/serverplugin_unfinsh/my_apis.json` & `codebot-0.0.5/src/plugins/serverplugin_unfinsh/my_apis.json`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/plugins/vue/functions.py` & `codebot-0.0.5/src/plugins/vue/functions.py`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/tmp/1690769899.3643498.png` & `codebot-0.0.5/src/tmp/1690769899.3643498.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/tmp/1690769912.7088609.png` & `codebot-0.0.5/src/tmp/1690769912.7088609.png`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/tmp/sin_function.gif` & `codebot-0.0.5/src/tmp/sin_function.gif`

 * *Files identical despite different names*

### Comparing `codebot-0.0.4/src/tmp/sin_function.png` & `codebot-0.0.5/src/tmp/sin_function.png`

 * *Files identical despite different names*

