# Comparing `tmp/litellm-0.1.2.tar.gz` & `tmp/litellm-0.1.201.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.2.tar", last modified: Sat Jul 29 18:52:17 2023, max compression
+gzip compressed data, was "litellm-0.1.201.tar", last modified: Mon Jul 31 14:33:00 2023, max compression
```

## Comparing `litellm-0.1.2.tar` & `litellm-0.1.201.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-29 18:52:17.812054 litellm-0.1.2/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.2/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      149 2023-07-29 18:52:17.811942 litellm-0.1.2/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1366 2023-07-29 14:29:32.000000 litellm-0.1.2/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-29 18:52:17.810837 litellm-0.1.2/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       58 2023-07-29 14:29:33.000000 litellm-0.1.2/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    16887 2023-07-29 18:25:34.000000 litellm-0.1.2/litellm/main.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-07-29 18:52:17.811754 litellm-0.1.2/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      149 2023-07-29 18:52:17.000000 litellm-0.1.2/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      216 2023-07-29 18:52:17.000000 litellm-0.1.2/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-07-29 18:52:17.000000 litellm-0.1.2/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       14 2023-07-29 18:52:17.000000 litellm-0.1.2/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-07-29 18:52:17.000000 litellm-0.1.2/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-07-29 18:52:17.812104 litellm-0.1.2/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      292 2023-07-29 18:52:10.000000 litellm-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 14:32:46.000000 litellm-0.1.201/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:33:00.181347 litellm-0.1.201/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-31 14:32:46.000000 litellm-0.1.201/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 14:32:46.000000 litellm-0.1.201/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-31 14:32:46.000000 litellm-0.1.201/litellm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:33:00.181347 litellm-0.1.201/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 14:32:46.000000 litellm-0.1.201/setup.py
```

### Comparing `litellm-0.1.2/LICENSE` & `litellm-0.1.201/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.2/README.md` & `litellm-0.1.201/README.md`

 * *Files identical despite different names*

