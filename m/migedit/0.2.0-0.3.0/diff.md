# Comparing `tmp/migedit-0.2.0.tar.gz` & `tmp/migedit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migedit-0.2.0.tar", last modified: Thu Apr 27 13:35:02 2023, max compression
+gzip compressed data, was "migedit-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `migedit-0.2.0.tar` & `migedit-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1079 2022-11-21 15:55:21.696838 migedit-0.2.0/LICENSE
--rw-r--r--   0        0        0      396 2023-04-27 13:29:00.000478 migedit-0.2.0/README.md
--rw-r--r--   0        0        0     5717 2023-04-27 13:26:45.655787 migedit-0.2.0/migedit.py
--rw-r--r--   0        0        0      429 2023-04-27 13:26:38.491750 migedit-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 migedit-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1799 2023-07-27 10:46:05.001162 migedit-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1079 2023-07-27 10:46:05.001162 migedit-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1236 2023-07-31 12:11:36.103634 migedit-0.3.0/README.md
+-rw-r--r--   0        0        0     8722 2023-07-31 12:08:09.846163 migedit-0.3.0/migedit.py
+-rw-r--r--   0        0        0      459 2023-07-31 12:28:47.251569 migedit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 migedit-0.3.0/PKG-INFO
```

### Comparing `migedit-0.2.0/LICENSE` & `migedit-0.3.0/LICENSE`

 * *Files identical despite different names*

