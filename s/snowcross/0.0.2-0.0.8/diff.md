# Comparing `tmp/snowcross-0.0.2.tar.gz` & `tmp/snowcross-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowcross-0.0.2.tar", last modified: Fri Jul 28 00:24:41 2023, max compression
+gzip compressed data, was "snowcross-0.0.8.tar", last modified: Mon Jul 31 08:41:47 2023, max compression
```

## Comparing `snowcross-0.0.2.tar` & `snowcross-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,29 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.277863 snowcross-0.0.2/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.260730 snowcross-0.0.2/.github/
--rw-r--r--   0 mike       (501) staff       (20)      471 2023-07-27 23:52:05.000000 snowcross-0.0.2/.github/CODEOWNERS
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.262038 snowcross-0.0.2/.github/workflows/
--rw-r--r--   0 mike       (501) staff       (20)      757 2023-07-27 23:52:05.000000 snowcross-0.0.2/.github/workflows/master.yml
--rw-r--r--   0 mike       (501) staff       (20)      712 2023-07-27 23:52:05.000000 snowcross-0.0.2/.github/workflows/pull_request.yml
--rw-r--r--   0 mike       (501) staff       (20)      345 2023-07-27 23:52:05.000000 snowcross-0.0.2/.github/workflows/tag.yml
--rw-r--r--   0 mike       (501) staff       (20)     3092 2023-07-27 23:52:05.000000 snowcross-0.0.2/.gitignore
--rw-r--r--   0 mike       (501) staff       (20)    11357 2023-07-27 04:31:28.000000 snowcross-0.0.2/LICENSE
--rw-r--r--   0 mike       (501) staff       (20)       55 2023-07-27 23:52:05.000000 snowcross-0.0.2/MANIFEST.in
--rw-r--r--   0 mike       (501) staff       (20)     1363 2023-07-28 00:23:50.000000 snowcross-0.0.2/Makefile
--rw-r--r--   0 mike       (501) staff       (20)      980 2023-07-27 23:52:05.000000 snowcross-0.0.2/Makehelp.mk
--rw-r--r--   0 mike       (501) staff       (20)     1238 2023-07-28 00:24:41.277531 snowcross-0.0.2/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      717 2023-07-28 00:18:49.000000 snowcross-0.0.2/README.md
--rw-r--r--   0 mike       (501) staff       (20)      411 2023-07-27 23:52:05.000000 snowcross-0.0.2/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)      126 2023-07-27 23:52:05.000000 snowcross-0.0.2/requirements-test.txt
--rw-r--r--   0 mike       (501) staff       (20)       52 2023-07-27 23:52:05.000000 snowcross-0.0.2/requirements.txt
--rw-r--r--   0 mike       (501) staff       (20)       38 2023-07-28 00:24:41.277987 snowcross-0.0.2/setup.cfg
--rw-r--r--   0 mike       (501) staff       (20)     1404 2023-07-28 00:22:14.000000 snowcross-0.0.2/setup.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.264167 snowcross-0.0.2/snowcross/
--rw-r--r--   0 mike       (501) staff       (20)        0 2023-07-27 23:52:05.000000 snowcross-0.0.2/snowcross/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)      160 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross/_version.py
--rw-r--r--   0 mike       (501) staff       (20)     6459 2023-07-27 23:52:05.000000 snowcross-0.0.2/snowcross/aws.py
--rw-r--r--   0 mike       (501) staff       (20)      465 2023-07-27 23:52:05.000000 snowcross-0.0.2/snowcross/errors.py
--rw-r--r--   0 mike       (501) staff       (20)     4255 2023-07-27 23:52:05.000000 snowcross-0.0.2/snowcross/snowflake.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.266378 snowcross-0.0.2/snowcross.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)     1238 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      716 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)      174 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       16 2023-07-28 00:24:41.000000 snowcross-0.0.2/snowcross.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.273274 snowcross-0.0.2/tests/
--rw-r--r--   0 mike       (501) staff       (20)      702 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/__init__.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.274017 snowcross-0.0.2/tests/files/
--rw-r--r--   0 mike       (501) staff       (20)       23 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/files/s3testfile.json
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.275741 snowcross-0.0.2/tests/fixtures/
--rw-r--r--   0 mike       (501) staff       (20)        0 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/fixtures/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     4158 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/fixtures/aws.py
--rw-r--r--   0 mike       (501) staff       (20)     3396 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/fixtures/snowflake.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-07-28 00:24:41.276435 snowcross-0.0.2/tests/helpers/
--rw-r--r--   0 mike       (501) staff       (20)        0 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/helpers/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     1256 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/helpers/docker.py
--rw-r--r--   0 mike       (501) staff       (20)     7422 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/test_aws.py
--rw-r--r--   0 mike       (501) staff       (20)     3872 2023-07-27 23:52:05.000000 snowcross-0.0.2/tests/test_snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-31 08:41:24.000000 snowcross-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-31 08:41:24.000000 snowcross-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 08:41:47.821094 snowcross-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-31 08:41:24.000000 snowcross-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-31 08:41:24.000000 snowcross-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-31 08:41:24.000000 snowcross-0.0.8/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-31 08:41:24.000000 snowcross-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 08:41:47.821094 snowcross-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-31 08:41:24.000000 snowcross-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/snowcross/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-07-31 08:41:24.000000 snowcross-0.0.8/snowcross/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/snowcross.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-31 08:41:47.000000 snowcross-0.0.8/snowcross.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/fixtures/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:47.821094 snowcross-0.0.8/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-31 08:41:24.000000 snowcross-0.0.8/tests/helpers/docker.py
```

### Comparing `snowcross-0.0.2/LICENSE` & `snowcross-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.2/README.md` & `snowcross-0.0.8/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # snowcross-python
 
 Adaptors for tools and services in a Snowflake-centric data platform.
 
-> **WARNING** While this repository is private, releases are published _publicly_ to [PyPI](https://pypi.org/project/snowcross/)!
-> All commits, pull requests and this readme (see [DESCRIPTION.md](./DESCRIPTION.md) are hidden,
-> however the source code is easily extracted from the published artifacts. Refrain from including
-> any references to proprietary code, infrastructure or architecture. This package is for generic
-> utilities for tools and services only.
+> **WARNING** While this repository is private, releases are published _publicly_ to 
+> [PyPI](https://pypi.org/project/snowcross/)! All commits, pull requests and this readme are
+> hidden, however the source code is easily extracted from published artifacts. Refrain from
+> including any references to proprietary code, infrastructure or architecture. This package is
+> for generic utilities for tools and services only.
 
 ## Requirements
 
 Requires Python 3.8 or above.
 
 ## Usage
```

### Comparing `snowcross-0.0.2/snowcross/aws.py` & `snowcross-0.0.8/snowcross/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.2/snowcross/snowflake.py` & `snowcross-0.0.8/snowcross/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.2/tests/fixtures/aws.py` & `snowcross-0.0.8/tests/fixtures/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.2/tests/fixtures/snowflake.py` & `snowcross-0.0.8/tests/fixtures/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.0.2/tests/helpers/docker.py` & `snowcross-0.0.8/tests/helpers/docker.py`

 * *Files identical despite different names*

