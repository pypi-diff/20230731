# Comparing `tmp/pyupgrade-3.8.0.tar.gz` & `tmp/pyupgrade-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyupgrade-3.8.0.tar", last modified: Sat Jul  1 18:38:44 2023, max compression
+gzip compressed data, was "pyupgrade-3.9.0.tar", last modified: Sat Jul  8 16:47:10 2023, max compression
```

## Comparing `pyupgrade-3.8.0.tar` & `pyupgrade-3.9.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:38:44.972534 pyupgrade-3.8.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-07-01 18:38:44.972534 pyupgrade-3.8.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)    12902 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/README.md
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:38:44.968534 pyupgrade-3.8.0/pyupgrade/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/__main__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_ast_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3237 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_data.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    11830 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_main.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:38:44.972534 pyupgrade-3.8.0/pyupgrade/_plugins/
--rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/__init__.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/collections_abc.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/datetime_utc_alias.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/default_encoding.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/dict_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/format_locals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/fstrings.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/identity_equality.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    20218 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/imports.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/io_open.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/legacy.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/lru_cache.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/metaclass_type.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/mock.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2438 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/native_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/new_style_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/open_mode.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/oserror_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/percent_format.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/set_literals.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/six_base_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/six_calls.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/six_metaclasses.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/six_remove_decorators.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/six_simple.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/subprocess_run.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/type_of_primitive.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_classes.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5653 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep563.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep585.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep604.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep646_unpack.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/typing_text.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/unittest_aliases.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/unpack_list_comprehension.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     6490 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_plugins/versioned_branches.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_string_helpers.py
--rw-r--r--   0 asottile  (1000) asottile  (1000)    14591 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/pyupgrade/_token_helpers.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-01 18:38:44.968534 pyupgrade-3.8.0/pyupgrade.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)    13524 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1711 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/requires.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-07-01 18:38:44.000000 pyupgrade-3.8.0/pyupgrade.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1200 2023-07-01 18:38:44.972534 pyupgrade-3.8.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-01 18:10:42.000000 pyupgrade-3.8.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-08 16:47:10.966192 pyupgrade-3.9.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13675 2023-07-08 16:47:10.966192 pyupgrade-3.9.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13051 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/README.md
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-08 16:47:10.962192 pyupgrade-3.9.0/pyupgrade/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      126 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/__main__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1445 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_ast_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3153 2023-07-03 16:19:54.000000 pyupgrade-3.9.0/pyupgrade/_data.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    11830 2023-06-18 20:35:59.000000 pyupgrade-3.9.0/pyupgrade/_main.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-08 16:47:10.966192 pyupgrade-3.9.0/pyupgrade/_plugins/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        0 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_plugins/__init__.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      985 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/collections_abc.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      970 2022-12-02 18:20:28.000000 pyupgrade-3.9.0/pyupgrade/_plugins/datetime_utc_alias.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1465 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/default_encoding.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2185 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_plugins/dict_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1769 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/format_locals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4398 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/fstrings.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1543 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/identity_equality.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    20218 2023-06-18 20:41:39.000000 pyupgrade-3.9.0/pyupgrade/_plugins/imports.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      919 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/io_open.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7781 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/legacy.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2447 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/lru_cache.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      967 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/metaclass_type.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      870 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/mock.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2438 2023-06-18 20:35:59.000000 pyupgrade-3.9.0/pyupgrade/_plugins/native_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      631 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/new_style_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4031 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/open_mode.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4213 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/oserror_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     9476 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/percent_format.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2303 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/set_literals.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2386 2023-07-03 17:31:33.000000 pyupgrade-3.9.0/pyupgrade/_plugins/shlex_join.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      692 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/six_base_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     6522 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/six_calls.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3340 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/six_metaclasses.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      808 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/six_remove_decorators.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3634 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/six_simple.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3617 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_plugins/subprocess_run.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1413 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/type_of_primitive.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     8320 2023-06-18 20:35:59.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_classes.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5637 2023-07-03 16:19:54.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep563.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1695 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep585.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5787 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep604.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1208 2022-11-10 15:10:00.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep646_unpack.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1083 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/typing_text.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     2182 2022-10-29 19:34:22.000000 pyupgrade-3.9.0/pyupgrade/_plugins/unittest_aliases.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1073 2023-06-02 22:05:16.000000 pyupgrade-3.9.0/pyupgrade/_plugins/unpack_list_comprehension.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     7272 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade/_plugins/versioned_branches.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1949 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/pyupgrade/_string_helpers.py
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    14324 2023-07-03 18:18:38.000000 pyupgrade-3.9.0/pyupgrade/_token_helpers.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-08 16:47:10.962192 pyupgrade-3.9.0/pyupgrade.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)    13675 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1744 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       51 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       19 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/requires.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       10 2023-07-08 16:47:10.000000 pyupgrade-3.9.0/pyupgrade.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1202 2023-07-08 16:47:10.966192 pyupgrade-3.9.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2022-04-30 16:59:39.000000 pyupgrade-3.9.0/setup.py
```

### Comparing `pyupgrade-3.8.0/LICENSE` & `pyupgrade-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/PKG-INFO` & `pyupgrade-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.8.0
+Version: 3.9.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.8.0
+    rev: v3.9.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
@@ -647,14 +647,23 @@
 
 -@functools.lru_cache()
 +@functools.lru_cache
  def expensive():
      ...
 ```
 
+### shlex.join
+
+Availability:
+- `--py38-plus` is passed on the commandline.
+
+```diff
+-' '.join(shlex.quote(arg) for arg in cmd)
++shlex.join(cmd)
+```
 
 ### replace `@functools.lru_cache(maxsize=None)` with shorthand
 
 Availability:
 - `--py39-plus` is passed on the commandline.
 
 ```diff
```

### Comparing `pyupgrade-3.8.0/README.md` & `pyupgrade-3.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.8.0
+    rev: v3.9.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
@@ -630,14 +630,23 @@
 
 -@functools.lru_cache()
 +@functools.lru_cache
  def expensive():
      ...
 ```
 
+### shlex.join
+
+Availability:
+- `--py38-plus` is passed on the commandline.
+
+```diff
+-' '.join(shlex.quote(arg) for arg in cmd)
++shlex.join(cmd)
+```
 
 ### replace `@functools.lru_cache(maxsize=None)` with shorthand
 
 Availability:
 - `--py39-plus` is passed on the commandline.
 
 ```diff
```

### Comparing `pyupgrade-3.8.0/pyupgrade/_ast_helpers.py` & `pyupgrade-3.9.0/pyupgrade/_ast_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_data.py` & `pyupgrade-3.9.0/pyupgrade/_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,23 @@
 import ast
 import collections
 import pkgutil
 from typing import Callable
 from typing import Iterable
 from typing import List
 from typing import NamedTuple
+from typing import Protocol
 from typing import Tuple
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 from tokenize_rt import Offset
 from tokenize_rt import Token
 
 from pyupgrade import _plugins
 
-if TYPE_CHECKING:
-    from typing import Protocol
-else:
-    Protocol = object
-
 Version = Tuple[int, ...]
 
 
 class Settings(NamedTuple):
     min_version: Version = (3,)
     keep_percent_format: bool = False
     keep_mock: bool = False
```

### Comparing `pyupgrade-3.8.0/pyupgrade/_main.py` & `pyupgrade-3.9.0/pyupgrade/_main.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/collections_abc.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/collections_abc.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/datetime_utc_alias.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/datetime_utc_alias.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/default_encoding.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/default_encoding.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/dict_literals.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/dict_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/format_locals.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/format_locals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/fstrings.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/fstrings.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/identity_equality.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/identity_equality.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/imports.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/imports.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/io_open.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/io_open.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/legacy.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/legacy.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/lru_cache.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/lru_cache.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/metaclass_type.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/metaclass_type.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/mock.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/mock.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/native_literals.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/native_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/new_style_classes.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/new_style_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/open_mode.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/open_mode.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/oserror_aliases.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/oserror_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/percent_format.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/percent_format.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/set_literals.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/set_literals.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/six_base_classes.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/six_base_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/six_calls.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/six_calls.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/six_metaclasses.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/six_metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/six_remove_decorators.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/six_remove_decorators.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/six_simple.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/six_simple.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/subprocess_run.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/subprocess_run.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/type_of_primitive.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/type_of_primitive.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_classes.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_classes.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep563.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep563.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 ) -> Iterable[tuple[Offset, TokenFunc]]:
     if not _supported_version(state):
         return
 
     yield from _process_args([node.args.vararg, node.args.kwarg])
     yield from _process_args(node.args.args)
     yield from _process_args(node.args.kwonlyargs)
-    yield from _process_args(getattr(node.args, 'posonlyargs', []))
+    yield from _process_args(node.args.posonlyargs)
     if node.returns is not None:
         yield from _replace_string_literal(node.returns)
 
 
 @register(ast.AsyncFunctionDef)
 def visit_AsyncFunctionDef(
         state: State,
```

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep585.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep585.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep604.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep604.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_pep646_unpack.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_pep646_unpack.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/typing_text.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/typing_text.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/unittest_aliases.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/unittest_aliases.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/unpack_list_comprehension.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/unpack_list_comprehension.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_plugins/versioned_branches.py` & `pyupgrade-3.9.0/pyupgrade/_plugins/versioned_branches.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,54 +21,70 @@
     i = if_block.end
     while tokens[i].src != 'else':
         i += 1
     else_block = Block.find(tokens, i, trim_end=True)
     return if_block, else_block
 
 
-def _find_elif(tokens: list[Token], i: int) -> int:
-    while tokens[i].src != 'elif':  # pragma: no cover (only for <3.8.1)
-        i -= 1
-    return i
-
-
 def _fix_py3_block(i: int, tokens: list[Token]) -> None:
     if tokens[i].src == 'if':
         if_block = Block.find(tokens, i)
         if_block.dedent(tokens)
         del tokens[if_block.start:if_block.block]
     else:
-        if_block = Block.find(tokens, _find_elif(tokens, i))
+        if_block = Block.find(tokens, i)
         if_block.replace_condition(tokens, [Token('NAME', 'else')])
 
 
 def _fix_py2_block(i: int, tokens: list[Token]) -> None:
     if tokens[i].src == 'if':
         if_block, else_block = _find_if_else_block(tokens, i)
         else_block.dedent(tokens)
         del tokens[if_block.start:else_block.block]
     else:
-        j = _find_elif(tokens, i)
-        if_block, else_block = _find_if_else_block(tokens, j)
+        if_block, else_block = _find_if_else_block(tokens, i)
         del tokens[if_block.start:else_block.start]
 
 
+def _fix_remove_block(i: int, tokens: list[Token]) -> None:
+    block = Block.find(tokens, i)
+    del tokens[block.start:block.end]
+
+
+def _fix_py2_convert_elif(i: int, tokens: list[Token]) -> None:
+    if_block = Block.find(tokens, i)
+    # wasn't actually followed by an `elif`
+    if tokens[if_block.end].src != 'elif':
+        return
+    tokens[if_block.end] = Token('CODE', tokens[i].src)
+    _fix_remove_block(i, tokens)
+
+
 def _fix_py3_block_else(i: int, tokens: list[Token]) -> None:
     if tokens[i].src == 'if':
         if_block, else_block = _find_if_else_block(tokens, i)
         if_block.dedent(tokens)
         del tokens[if_block.end:else_block.end]
         del tokens[if_block.start:if_block.block]
     else:
-        j = _find_elif(tokens, i)
-        if_block, else_block = _find_if_else_block(tokens, j)
+        if_block, else_block = _find_if_else_block(tokens, i)
         del tokens[if_block.end:else_block.end]
         if_block.replace_condition(tokens, [Token('NAME', 'else')])
 
 
+def _fix_py3_convert_elif(i: int, tokens: list[Token]) -> None:
+    if_block = Block.find(tokens, i)
+    # wasn't actually followed by an `elif`
+    if tokens[if_block.end].src != 'elif':
+        return
+    tokens[if_block.end] = Token('CODE', tokens[i].src)
+    if_block.dedent(tokens)
+    del tokens[if_block.start:if_block.block]
+
+
 def _eq(test: ast.Compare, n: int) -> bool:
     return (
         isinstance(test.ops[0], ast.Eq) and
         isinstance(test.comparators[0], ast.Constant) and
         test.comparators[0].value == n
     )
 
@@ -146,16 +162,20 @@
                     any(
                         _compare_to_3(node.test, (ast.Lt, ast.LtE), minor)
                         for minor in range(min_version[1])
                     )
                 )
             )
     ):
-        if node.orelse and not isinstance(node.orelse[0], ast.If):
+        if len(node.orelse) == 1 and isinstance(node.orelse[0], ast.If):
+            yield ast_to_offset(node), _fix_py2_convert_elif
+        elif node.orelse:
             yield ast_to_offset(node), _fix_py2_block
+        elif node.col_offset == 0:
+            yield ast_to_offset(node), _fix_remove_block
     elif (
             # if six.PY3:
             is_name_attr(
                 node.test,
                 state.from_imports,
                 ('six',),
                 ('PY3',),
@@ -189,11 +209,13 @@
                     any(
                         _compare_to_3(node.test, (ast.Gt, ast.GtE), minor)
                         for minor in range(min_version[1])
                     )
                 )
             )
     ):
-        if node.orelse and not isinstance(node.orelse[0], ast.If):
+        if len(node.orelse) == 1 and isinstance(node.orelse[0], ast.If):
+            yield ast_to_offset(node), _fix_py3_convert_elif
+        elif node.orelse:
             yield ast_to_offset(node), _fix_py3_block_else
-        elif not node.orelse:
+        else:
             yield ast_to_offset(node), _fix_py3_block
```

### Comparing `pyupgrade-3.8.0/pyupgrade/_string_helpers.py` & `pyupgrade-3.9.0/pyupgrade/_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyupgrade-3.8.0/pyupgrade/_token_helpers.py` & `pyupgrade-3.9.0/pyupgrade/_token_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,25 +45,18 @@
 
 
 def find_open_paren(tokens: list[Token], i: int) -> int:
     return find_token(tokens, i, '(')
 
 
 def find_end(tokens: list[Token], i: int) -> int:
-    while tokens[i].name not in {'NEWLINE', 'ENDMARKER'}:
-        i += 1
-
-    # depending on the version of python, some will not emit
-    # NEWLINE('') at the end of a file which does not end with a
-    # newline (for example 3.7.0)
-    if tokens[i].name == 'ENDMARKER':  # pragma: no cover
-        i -= 1
-    else:
+    while tokens[i].name != 'NEWLINE':
         i += 1
 
+    i += 1
     return i
 
 
 def _arg_token_index(tokens: list[Token], i: int, arg: ast.expr) -> int:
     idx = _search_until(tokens, i, arg) + 1
     while idx < len(tokens) and tokens[idx].name in NON_CODING_TOKENS:
         idx += 1
```

### Comparing `pyupgrade-3.8.0/pyupgrade.egg-info/PKG-INFO` & `pyupgrade-3.9.0/pyupgrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pyupgrade
-Version: 3.8.0
+Version: 3.9.0
 Summary: A tool to automatically upgrade syntax for newer versions.
 Home-page: https://github.com/asottile/pyupgrade
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
+Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![build status](https://github.com/asottile/pyupgrade/actions/workflows/main.yml/badge.svg)](https://github.com/asottile/pyupgrade/actions/workflows/main.yml)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/asottile/pyupgrade/main.svg)](https://results.pre-commit.ci/latest/github/asottile/pyupgrade/main)
 
 pyupgrade
@@ -34,15 +34,15 @@
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`:
 
 ```yaml
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.8.0
+    rev: v3.9.0
     hooks:
     -   id: pyupgrade
 ```
 
 ## Implemented features
 
 ### Set literals
@@ -647,14 +647,23 @@
 
 -@functools.lru_cache()
 +@functools.lru_cache
  def expensive():
      ...
 ```
 
+### shlex.join
+
+Availability:
+- `--py38-plus` is passed on the commandline.
+
+```diff
+-' '.join(shlex.quote(arg) for arg in cmd)
++shlex.join(cmd)
+```
 
 ### replace `@functools.lru_cache(maxsize=None)` with shorthand
 
 Availability:
 - `--py39-plus` is passed on the commandline.
 
 ```diff
```

### Comparing `pyupgrade-3.8.0/pyupgrade.egg-info/SOURCES.txt` & `pyupgrade-3.9.0/pyupgrade.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 pyupgrade/_plugins/mock.py
 pyupgrade/_plugins/native_literals.py
 pyupgrade/_plugins/new_style_classes.py
 pyupgrade/_plugins/open_mode.py
 pyupgrade/_plugins/oserror_aliases.py
 pyupgrade/_plugins/percent_format.py
 pyupgrade/_plugins/set_literals.py
+pyupgrade/_plugins/shlex_join.py
 pyupgrade/_plugins/six_base_classes.py
 pyupgrade/_plugins/six_calls.py
 pyupgrade/_plugins/six_metaclasses.py
 pyupgrade/_plugins/six_remove_decorators.py
 pyupgrade/_plugins/six_simple.py
 pyupgrade/_plugins/subprocess_run.py
 pyupgrade/_plugins/type_of_primitive.py
```

### Comparing `pyupgrade-3.8.0/setup.cfg` & `pyupgrade-3.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyupgrade
-version = 3.8.0
+version = 3.9.0
 description = A tool to automatically upgrade syntax for newer versions.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/pyupgrade
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
@@ -16,15 +16,15 @@
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 
 [options]
 packages = find:
 install_requires = 
 	tokenize-rt>=3.2.0
-python_requires = >=3.8
+python_requires = >=3.8.1
 
 [options.packages.find]
 exclude = 
 	tests*
 	testing*
 
 [options.entry_points]
```

