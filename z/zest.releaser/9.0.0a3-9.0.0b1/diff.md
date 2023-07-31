# Comparing `tmp/zest.releaser-9.0.0a3.tar.gz` & `tmp/zest.releaser-9.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zest.releaser-9.0.0a3.tar", last modified: Tue Jul 25 15:44:42 2023, max compression
+gzip compressed data, was "zest.releaser-9.0.0b1.tar", last modified: Mon Jul 31 20:35:58 2023, max compression
```

## Comparing `zest.releaser-9.0.0a3.tar` & `zest.releaser-9.0.0b1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.452868 zest.releaser-9.0.0a3/
--rw-r--r--   0 maurits    (501) staff       (20)     5088 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1071 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    15569 2023-07-25 15:44:42.453047 zest.releaser-9.0.0a3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8076 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.429459 zest.releaser-9.0.0a3/doc/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.437101 zest.releaser-9.0.0a3/doc/source/
--rw-r--r--   0 maurits    (501) staff       (20)     2010 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/assumptions.rst
--rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/changelog.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6894 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       32 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/credits.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/developing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8341 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/entrypoints.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/further_reading.rst
--rw-r--r--   0 maurits    (501) staff       (20)      837 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6941 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/options.rst
--rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/project.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/uploading.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3566 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/versions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3378 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      294 2023-07-25 15:44:42.453638 zest.releaser-9.0.0a3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      251 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/tox.ini
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.429855 zest.releaser-9.0.0a3/zest/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.444042 zest.releaser-9.0.0a3/zest/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/addchangelogentry.py
--rw-r--r--   0 maurits    (501) staff       (20)    17830 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/baserelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     6297 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/bumpversion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/choose.py
--rw-r--r--   0 maurits    (501) staff       (20)      962 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/fullrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     4178 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/git.py
--rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/lasttagdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      833 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/lasttaglog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1939 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/longtest.py
--rw-r--r--   0 maurits    (501) staff       (20)     5172 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/postrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/preparedocs.py
--rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/prerelease.py
--rw-r--r--   0 maurits    (501) staff       (20)    24188 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)    13543 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.452609 zest.releaser-9.0.0a3/zest/releaser/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       10 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/addchangelogentry.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4446 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/baserelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/bumpversion.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/choose.txt
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/cmd_error.py
--rw-r--r--   0 maurits    (501) staff       (20)    17408 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/example.tar
--rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/fullrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional-git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4444 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional-with-hooks.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4311 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/postrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/preparedocs.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/prerelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12174 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypi.txt
--rw-r--r--   0 maurits    (501) staff       (20)      203 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_both.txt
--rw-r--r--   0 maurits    (501) staff       (20)      275 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_new.txt
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_no_input.txt
--rw-r--r--   0 maurits    (501) staff       (20)      107 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_no_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)       57 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_old.txt
--rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_simple.txt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_universal_nocreate.txt
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_yes_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4211 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pyproject-toml.txt
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     3118 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2857 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)    22286 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/utils.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/vcs.txt
--rw-r--r--   0 maurits    (501) staff       (20)    33481 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    18085 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/vcs.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.439075 zest.releaser-9.0.0a3/zest.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    15569 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2238 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      951 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      220 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.652631 zest.releaser-9.0.0b1/
+-rw-r--r--   0 maurits    (501) staff       (20)     5586 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1071 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/CREDITS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    16067 2023-07-31 20:35:58.652817 zest.releaser-9.0.0b1/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     8076 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.629720 zest.releaser-9.0.0b1/doc/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.637030 zest.releaser-9.0.0b1/doc/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     2010 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/assumptions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/changelog.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6894 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       32 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/credits.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/developing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8341 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/entrypoints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/further_reading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      837 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6941 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/options.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/project.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/uploading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3566 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/doc/source/versions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3378 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2023-07-31 20:35:58.653350 zest.releaser-9.0.0b1/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      251 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.630107 zest.releaser-9.0.0b1/zest/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.643911 zest.releaser-9.0.0b1/zest/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/addchangelogentry.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17961 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/baserelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6297 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/bumpversion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/choose.py
+-rw-r--r--   0 maurits    (501) staff       (20)      962 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/fullrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4178 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/git.py
+-rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/lasttagdiff.py
+-rw-r--r--   0 maurits    (501) staff       (20)      833 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/lasttaglog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1939 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/longtest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5172 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/postrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/preparedocs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/prerelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)    24188 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13543 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.652387 zest.releaser-9.0.0b1/zest/releaser/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       10 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/addchangelogentry.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4644 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/baserelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/bumpversion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/choose.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/cmd_error.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17408 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/example.tar
+-rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/fullrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/functional-git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4444 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/functional-with-hooks.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4311 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/postrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/preparedocs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/prerelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12174 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypi.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      203 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_both.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_new.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      109 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_no_input.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_no_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       57 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_old.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_simple.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_universal_nocreate.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pypirc_yes_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4211 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pyproject-toml.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     3006 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2857 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22544 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/utils.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/tests/vcs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    34706 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18085 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest/releaser/vcs.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-31 20:35:58.639078 zest.releaser-9.0.0b1/zest.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    16067 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2238 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      951 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      220 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-31 20:35:58.000000 zest.releaser-9.0.0b1/zest.releaser.egg-info/top_level.txt
```

### Comparing `zest.releaser-9.0.0a3/CHANGES.rst` & `zest.releaser-9.0.0b1/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 Changelog for zest.releaser
 ===========================
 
+9.0.0b1 (2023-07-31)
+--------------------
+
+- When a command we call exits with a non-zero exit code, clearly state this in the output.
+  Ask the user if she wants to continue or not.
+  Note that this is tricky to do right.  Some commands like ``git`` seem to print everything to stderr,
+  leading us to think there are errors, but the exit code is zero, so it should be fine.
+  We do not want to ask too many questions, but we do not want to silently swallow important errors either.
+  [maurits]
+
+
 9.0.0a3 (2023-07-25)
 --------------------
 
 - Updated contributors list.
 
 - Documenting ``hook_package_dir`` setting for entry points (which isn't
   needed for most entry points, btw).
```

### Comparing `zest.releaser-9.0.0a3/CONTRIBUTING.rst` & `zest.releaser-9.0.0b1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/CREDITS.rst` & `zest.releaser-9.0.0b1/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/LICENSE.GPL` & `zest.releaser-9.0.0b1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/LICENSE.rst` & `zest.releaser-9.0.0b1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/PKG-INFO` & `zest.releaser-9.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 9.0.0a3
+Version: 9.0.0b1
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
@@ -245,14 +245,25 @@
 
 * `Eli Sallé <https://github.com/elisallenens>`_ added pyproject.toml support
   for zest.releaser's own options. We're modern now!
 
 Changelog for zest.releaser
 ===========================
 
+9.0.0b1 (2023-07-31)
+--------------------
+
+- When a command we call exits with a non-zero exit code, clearly state this in the output.
+  Ask the user if she wants to continue or not.
+  Note that this is tricky to do right.  Some commands like ``git`` seem to print everything to stderr,
+  leading us to think there are errors, but the exit code is zero, so it should be fine.
+  We do not want to ask too many questions, but we do not want to silently swallow important errors either.
+  [maurits]
+
+
 9.0.0a3 (2023-07-25)
 --------------------
 
 - Updated contributors list.
 
 - Documenting ``hook_package_dir`` setting for entry points (which isn't
   needed for most entry points, btw).
```

### Comparing `zest.releaser-9.0.0a3/README.rst` & `zest.releaser-9.0.0b1/README.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/assumptions.rst` & `zest.releaser-9.0.0b1/doc/source/assumptions.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/changelog.rst` & `zest.releaser-9.0.0b1/doc/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/conf.py` & `zest.releaser-9.0.0b1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/developing.rst` & `zest.releaser-9.0.0b1/doc/source/developing.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/entrypoints.rst` & `zest.releaser-9.0.0b1/doc/source/entrypoints.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/further_reading.rst` & `zest.releaser-9.0.0b1/doc/source/further_reading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/index.rst` & `zest.releaser-9.0.0b1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/options.rst` & `zest.releaser-9.0.0b1/doc/source/options.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/project.rst` & `zest.releaser-9.0.0b1/doc/source/project.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/uploading.rst` & `zest.releaser-9.0.0b1/doc/source/uploading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/doc/source/versions.rst` & `zest.releaser-9.0.0b1/doc/source/versions.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/pyproject.toml` & `zest.releaser-9.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # See https://snarky.ca/what-the-heck-is-pyproject-toml/
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zest.releaser"
-version = "9.0.0a3"
+version = "9.0.0b1"
 description = "Software releasing made easy and repeatable"
 license = {text = "GPL"}
 authors = [
     {name = "Reinout van Rees", email = "reinout@vanrees.org"},
     {name = "Maurits van Rees", email = "maurits@vanrees.org"},
 ]
 dependencies = [
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/addchangelogentry.py` & `zest.releaser-9.0.0b1/zest/releaser/addchangelogentry.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/baserelease.py` & `zest.releaser-9.0.0b1/zest/releaser/baserelease.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,14 +404,17 @@
         """Offer to push changes, if needed."""
         push_cmds = self.vcs.push_commands()
         if not push_cmds:
             return
         default_anwer = self.zest_releaser_config.push_changes()
         if utils.ask("OK to push commits to the server?", default=default_anwer):
             for push_cmd in push_cmds:
+                if utils.TESTMODE:
+                    logger.info("MOCK push command: %s", push_cmd)
+                    continue
                 output = execute_command(
                     push_cmd,
                     allow_retry=True,
                     fail_message="Perhaps the main branch is protected?",
                 )
                 logger.info(output)
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/bumpversion.py` & `zest.releaser-9.0.0b1/zest/releaser/bumpversion.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/choose.py` & `zest.releaser-9.0.0b1/zest/releaser/choose.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/fullrelease.py` & `zest.releaser-9.0.0b1/zest/releaser/fullrelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/git.py` & `zest.releaser-9.0.0b1/zest/releaser/git.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/lasttagdiff.py` & `zest.releaser-9.0.0b1/zest/releaser/lasttagdiff.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/lasttaglog.py` & `zest.releaser-9.0.0b1/zest/releaser/lasttaglog.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/longtest.py` & `zest.releaser-9.0.0b1/zest/releaser/longtest.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/postrelease.py` & `zest.releaser-9.0.0b1/zest/releaser/postrelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/preparedocs.py` & `zest.releaser-9.0.0b1/zest/releaser/preparedocs.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/prerelease.py` & `zest.releaser-9.0.0b1/zest/releaser/prerelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/pypi.py` & `zest.releaser-9.0.0b1/zest/releaser/pypi.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/release.py` & `zest.releaser-9.0.0b1/zest/releaser/release.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/addchangelogentry.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/addchangelogentry.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/baserelease.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/baserelease.txt`

 * *Files 3% similar despite different names*

```diff
@@ -151,11 +151,15 @@
 Also, if we have no ``history_format`` setting, but the
 history file ends with ``.md``, we consider it Markdown::
 
     >>> lines = ["[zest.releaser]", ""]
     >>> with open('setup.cfg', 'w') as f:
     ...     _ = f.write('\n'.join(lines))
     >>> rename_changelog("CHANGES.txt", "CHANGES.md")
+    >>> with open('setup.py') as f:
+    ...     setup_py_contents = f.read()
+    >>> with open('setup.py', 'w') as f:
+    ...     _ = f.write(setup_py_contents.replace("CHANGES.txt", "CHANGES.md"))
     >>> base = baserelease.Basereleaser()
     >>> base._grab_history()
     >>> base.history_format
     'md'
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/bumpversion.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/bumpversion.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/choose.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/choose.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/example.tar` & `zest.releaser-9.0.0b1/zest/releaser/tests/example.tar`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/fullrelease.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/fullrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/functional-git.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/functional-git.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/functional-with-hooks.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/functional-with-hooks.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/functional.py` & `zest.releaser-9.0.0b1/zest/releaser/tests/functional.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/git.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/git.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/postrelease.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/postrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/preparedocs.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/preparedocs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/prerelease.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/prerelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/pypi.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/pypi.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/pyproject-toml.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/pyproject-toml.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/release.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/release.txt`

 * *Files 6% similar despite different names*

```diff
@@ -79,19 +79,17 @@
     >>> utils.AUTO_RESPONSE
     False
     >>> releaser._info_if_tag_already_exists()
     Question: There is already a tag 0.1, show if there are differences? (Y/n)?
     Our reply: n
     >>> utils.test_answer_book.set_answers(['y'])
     >>> releaser._info_if_tag_already_exists()
-    Question: There is already a tag 0.1, show if there are differences? (Y/n)?
-    Our reply: y
-    git diff 0.1
-    RED fatal: ambiguous argument '0.1': unknown revision or path not in the working tree.
-    ...
+    Traceback (most recent call last):
+    ...diff_command...
+    RuntimeError: SYSTEM EXIT (code=1)
 
 Note: the diff itself fails as we mocked its existence.
 
 
 Making tags
 -----------
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/test_setup.py` & `zest.releaser-9.0.0b1/zest/releaser/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/utils.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/utils.txt`

 * *Files 2% similar despite different names*

```diff
@@ -409,16 +409,16 @@
 
 Just one line: no problem:
 
     >>> output = "just one line, no newlines"
     >>> utils.show_interesting_lines(output)
     just one line, no newlines
 
-In case of errors, shown in red, we show all and ask what the user
-wants to do.
+In case of errors, shown in red, we show all.
+If there was a non-zero exit code, we ask what the user wants to do.
 
     >>> output = "a\nb\nc\nd\ne\nf\ng\nh\ni\nj\nk\nl\nm\nn"
     >>> utils.show_interesting_lines(output)
     Showing first few lines...
     a
     b
     c
@@ -431,19 +431,36 @@
     l
     m
     n
     >>> from colorama import Fore
     >>> output = Fore.RED + output
     >>> utils.test_answer_book.set_answers([''])
     >>> utils.show_interesting_lines(output)
+    RED a
+    b
+    c
+    d
+    e
+    f
+    g
+    h
+    i
+    j
+    k
+    l
+    m
+    n
+    >>> output = f"{utils.ERROR_EXIT_CODE} 1\n{output}"
+    >>> utils.show_interesting_lines(output)
     Traceback (most recent call last):
     ...
     SystemExit: 1
     >>> utils.test_answer_book.set_answers(['y'])
     >>> utils.show_interesting_lines(output)
+    ERROR: exit code 1
     RED a
     b
     c
     d
     e
     f
     g
@@ -468,17 +485,18 @@
 
 We want to discover errors and show them in red.
 
     >>> Fore.RED
     '\x1b[31m'
     >>> Fore.MAGENTA
     '\x1b[35m'
-    >>> output = utils.execute_command(['ls', 'some-non-existing-file'])
-    >>> output.startswith(Fore.RED)
-    True
+    >>> utils.execute_command(['ls', 'some-non-existing-file'])
+    Traceback (most recent call last):
+    ...
+    SystemExit: 1
 
 Warnings may also end up in the error output.  That may be unwanted.
 We have a script to test this, which passes all input to std error.
 
     >>> import os
     >>> import zest.releaser.tests
     >>> test_dir = os.path.dirname(zest.releaser.tests.__file__)
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/tests/vcs.txt` & `zest.releaser-9.0.0b1/zest/releaser/tests/vcs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest/releaser/utils.py` & `zest.releaser-9.0.0b1/zest/releaser/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -440,26 +440,27 @@
         line_number += 1
     return headings
 
 
 def show_interesting_lines(result):
     """Just print the first and last five lines of (pypi) output.
 
-    But: when there are errors or warnings, print everything and ask
-    the user if she wants to continue.
+    But: when there are errors or warnings, print everything.
+    And if there is a non-zero exit code, ask the user if she wants to continue.
     """
     if Fore.RED in result:
         # warnings/errors, print complete result.
         print(result)
-        if not ask(
-            "There were errors or warnings. Are you sure you want to continue?",
-            default=False,
-        ):
-            sys.exit(1)
-        # User has seen everything and wants to continue.
+        if ERROR_EXIT_CODE in result:
+            if not ask(
+                "There were errors or warnings. Are you sure you want to continue?",
+                default=False,
+            ):
+                sys.exit(1)
+        # User has seen everything and wants to continue, or there was no exit code.
         return
 
     # No errors or warnings.  Show first and last lines.
     lines = [line for line in result.split("\n")]
     if len(lines) < 11:
         for line in lines:
             print(line)
@@ -622,14 +623,16 @@
     # This is from bdist_wheel displaying a warning by setuptools that
     # it will not include the __init__.py of a namespace package.  See
     # issue 108.
     "skipping installation of",
 ]
 # Make them lowercase just to be sure.
 KNOWN_WARNINGS = [w.lower() for w in KNOWN_WARNINGS]
+# If we see a non-zero exit code, we add this in this output:
+ERROR_EXIT_CODE = "ERROR: exit code"
 
 
 def format_command(command):
     """Return command list formatted as string.
 
     THIS IS INSECURE! DO NOT USE except for directly printing the result.
     Do NOT pass this to subprocess.popen/run.
@@ -666,15 +669,23 @@
         "stderr": subprocess.PIPE,
         "cwd": cwd,
         "env": env,
         "text": True,
     }
     process = subprocess.run(command, **process_kwargs)
     if process.returncode or show_stderr or "Traceback" in process.stderr:
-        # Some error occurred
+        # Some error occurred.  Or everything is fine, but the command
+        # prints to stderr anyway.
+        if process.returncode:
+            return (
+                Fore.RED
+                + f"{ERROR_EXIT_CODE} {process.returncode}.\n"
+                + process.stdout
+                + get_errors(process.stderr)
+            )
         return process.stdout + get_errors(process.stderr)
     # Only return the stdout. Stderr only contains possible
     # weird/confusing warnings that might trip up extraction of version
     # numbers and so.
     if process.stderr:
         logger.debug(
             "Stderr of running command '%s':\n%s",
@@ -735,19 +746,34 @@
 
     There is an error when there is a red color in the output.
 
     It might be a warning, but we cannot detect the distinction.
     """
     result = _execute_command(command, cwd=cwd, extra_environ=extra_environ)
     if not allow_retry:
+        if ERROR_EXIT_CODE in result:
+            print(result)
+            if not ask(
+                "There were errors or warnings. Are you sure you want to continue?",
+                default=False,
+            ):
+                sys.exit(1)
+        # Note: whoever calls us could print the result.  This would be double
+        # in case there was an error code but the user continues.  So be it.
         return result
+
+    # At this point, a retry is allowed.  We only do this for very few commands.
     if AUTO_RESPONSE:
-        # Also don't ask for retry, just return the result.
+        # Retry is not possible with auto response, so just return the result.
+        if ERROR_EXIT_CODE in result:
+            # This is a real error, and the user cannot react.  We quit.
+            print(result)
+            sys.exit(1)
         return result
-    if Fore.RED not in result:
+    if Fore.RED not in result or ERROR_EXIT_CODE not in result:
         show_interesting_lines(result)
         return result
     # There are warnings or errors. Print the complete result.
     print(result)
     print(Fore.RED + "There were errors or warnings.")
     if fail_message:
         print(Fore.RED + fail_message)
```

### Comparing `zest.releaser-9.0.0a3/zest/releaser/vcs.py` & `zest.releaser-9.0.0b1/zest/releaser/vcs.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest.releaser.egg-info/PKG-INFO` & `zest.releaser-9.0.0b1/zest.releaser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 9.0.0a3
+Version: 9.0.0b1
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
@@ -245,14 +245,25 @@
 
 * `Eli Sallé <https://github.com/elisallenens>`_ added pyproject.toml support
   for zest.releaser's own options. We're modern now!
 
 Changelog for zest.releaser
 ===========================
 
+9.0.0b1 (2023-07-31)
+--------------------
+
+- When a command we call exits with a non-zero exit code, clearly state this in the output.
+  Ask the user if she wants to continue or not.
+  Note that this is tricky to do right.  Some commands like ``git`` seem to print everything to stderr,
+  leading us to think there are errors, but the exit code is zero, so it should be fine.
+  We do not want to ask too many questions, but we do not want to silently swallow important errors either.
+  [maurits]
+
+
 9.0.0a3 (2023-07-25)
 --------------------
 
 - Updated contributors list.
 
 - Documenting ``hook_package_dir`` setting for entry points (which isn't
   needed for most entry points, btw).
```

### Comparing `zest.releaser-9.0.0a3/zest.releaser.egg-info/SOURCES.txt` & `zest.releaser-9.0.0b1/zest.releaser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a3/zest.releaser.egg-info/entry_points.txt` & `zest.releaser-9.0.0b1/zest.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

