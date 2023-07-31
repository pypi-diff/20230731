# Comparing `tmp/iluxaMod-2.6.tar.gz` & `tmp/iluxaMod-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iluxaMod-2.6.tar", last modified: Fri Aug 12 08:08:46 2022, max compression
+gzip compressed data, was "iluxaMod-2.7.tar", last modified: Mon Jul 31 16:28:41 2023, max compression
```

## Comparing `iluxaMod-2.6.tar` & `iluxaMod-2.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-08-12 08:08:46.670108 iluxaMod-2.6/
--rw-rw-rw-   0        0        0     3610 2022-08-12 08:08:46.671109 iluxaMod-2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-08-12 08:08:46.631488 iluxaMod-2.6/iluxaMod/
--rw-rw-rw-   0        0        0    10229 2022-08-12 08:08:45.000000 iluxaMod-2.6/iluxaMod/__init__.py
--rw-rw-rw-   0        0        0      592 2022-08-05 14:43:55.000000 iluxaMod-2.6/iluxaMod/tools.py
-drwxrwxrwx   0        0        0        0 2022-08-12 08:08:46.668109 iluxaMod-2.6/iluxaMod.egg-info/
--rw-rw-rw-   0        0        0     3610 2022-08-12 08:08:46.000000 iluxaMod-2.6/iluxaMod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2022-08-12 08:08:46.000000 iluxaMod-2.6/iluxaMod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-12 08:08:46.000000 iluxaMod-2.6/iluxaMod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2022-08-12 08:08:46.000000 iluxaMod-2.6/iluxaMod.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-12 08:08:46.000000 iluxaMod-2.6/iluxaMod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-12 08:08:46.678104 iluxaMod-2.6/setup.cfg
--rw-rw-rw-   0        0        0     3891 2022-08-12 08:08:45.000000 iluxaMod-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.225865 iluxaMod-2.7/
+-rw-rw-rw-   0        0        0      876 2023-07-31 16:28:41.224864 iluxaMod-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4466 2023-07-31 16:25:53.000000 iluxaMod-2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.208636 iluxaMod-2.7/iluxaMod/
+-rw-rw-rw-   0        0        0       24 2023-07-31 16:09:15.000000 iluxaMod-2.7/iluxaMod/__init__.py
+-rw-rw-rw-   0        0        0    21458 2023-07-31 16:25:53.000000 iluxaMod-2.7/iluxaMod/tools.py
+drwxrwxrwx   0        0        0        0 2023-07-31 16:28:41.222866 iluxaMod-2.7/iluxaMod.egg-info/
+-rw-rw-rw-   0        0        0      876 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-31 16:28:41.000000 iluxaMod-2.7/iluxaMod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 16:28:41.225865 iluxaMod-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1578 2023-07-31 16:28:38.000000 iluxaMod-2.7/setup.py
```

