# Comparing `tmp/litellm-0.1.201.tar.gz` & `tmp/litellm-0.1.202.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.201.tar", last modified: Mon Jul 31 14:33:00 2023, max compression
+gzip compressed data, was "litellm-0.1.202.tar", last modified: Mon Jul 31 14:41:14 2023, max compression
```

## Comparing `litellm-0.1.201.tar` & `litellm-0.1.202.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 14:32:46.000000 litellm-0.1.201/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:33:00.181347 litellm-0.1.201/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-31 14:32:46.000000 litellm-0.1.201/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/litellm/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 14:32:46.000000 litellm-0.1.201/litellm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-31 14:32:46.000000 litellm-0.1.201/litellm/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:33:00.181347 litellm-0.1.201/litellm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:33:00.000000 litellm-0.1.201/litellm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:33:00.181347 litellm-0.1.201/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 14:32:46.000000 litellm-0.1.201/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:41:14.057739 litellm-0.1.202/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-31 14:40:57.000000 litellm-0.1.202/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:41:14.057739 litellm-0.1.202/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-31 14:40:57.000000 litellm-0.1.202/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:41:14.057739 litellm-0.1.202/litellm/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-31 14:40:57.000000 litellm-0.1.202/litellm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-31 14:40:57.000000 litellm-0.1.202/litellm/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 14:41:14.057739 litellm-0.1.202/litellm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 14:41:14.000000 litellm-0.1.202/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-31 14:41:14.000000 litellm-0.1.202/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 14:41:14.000000 litellm-0.1.202/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-31 14:41:14.000000 litellm-0.1.202/litellm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-31 14:41:14.000000 litellm-0.1.202/litellm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 14:41:14.057739 litellm-0.1.202/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-31 14:40:57.000000 litellm-0.1.202/setup.py
```

### Comparing `litellm-0.1.201/LICENSE` & `litellm-0.1.202/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.201/README.md` & `litellm-0.1.202/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 # *🚅 litellm*
+[![Publish to PyPI](https://github.com/BerriAI/litellm/actions/workflows/publish_pypi.yml/badge.svg?branch=main)](https://github.com/BerriAI/litellm/actions/workflows/publish_pypi.yml) 
+![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)
+
 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light 100 line package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
 - guarantees consistent output, text responses will always be available at `['choices'][0]['message']['content']`
```

### Comparing `litellm-0.1.201/litellm/main.py` & `litellm-0.1.202/litellm/main.py`

 * *Files identical despite different names*

