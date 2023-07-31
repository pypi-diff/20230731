# Comparing `tmp/database-without-orm-local-0.0.18.tar.gz` & `tmp/database-without-orm-local-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database-without-orm-local-0.0.18.tar", last modified: Sun Jul 23 16:46:23 2023, max compression
+gzip compressed data, was "database-without-orm-local-0.0.19.tar", last modified: Mon Jul 31 19:33:58 2023, max compression
```

## Comparing `database-without-orm-local-0.0.18.tar` & `database-without-orm-local-0.0.19.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:46:23.390596 database-without-orm-local-0.0.18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 16:46:01.000000 database-without-orm-local-0.0.18/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-23 16:46:23.390596 database-without-orm-local-0.0.18/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:46:23.390596 database-without-orm-local-0.0.18/circles_local_database_python/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-23 16:46:01.000000 database-without-orm-local-0.0.18/circles_local_database_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-23 16:46:01.000000 database-without-orm-local-0.0.18/circles_local_database_python/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-23 16:46:23.390596 database-without-orm-local-0.0.18/database_without_orm_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-23 16:46:23.000000 database-without-orm-local-0.0.18/database_without_orm_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-23 16:46:23.000000 database-without-orm-local-0.0.18/database_without_orm_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-23 16:46:23.000000 database-without-orm-local-0.0.18/database_without_orm_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-23 16:46:23.000000 database-without-orm-local-0.0.18/database_without_orm_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-23 16:46:01.000000 database-without-orm-local-0.0.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-23 16:46:23.390596 database-without-orm-local-0.0.18/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-23 16:46:01.000000 database-without-orm-local-0.0.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:33:58.557717 database-without-orm-local-0.0.19/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 19:33:58.557717 database-without-orm-local-0.0.19/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:33:58.557717 database-without-orm-local-0.0.19/circles_local_database_python/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/circles_local_database_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/circles_local_database_python/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/circles_local_database_python/connection_cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:33:58.557717 database-without-orm-local-0.0.19/database_without_orm_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-31 19:33:58.000000 database-without-orm-local-0.0.19/database_without_orm_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-31 19:33:58.000000 database-without-orm-local-0.0.19/database_without_orm_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:33:58.000000 database-without-orm-local-0.0.19/database_without_orm_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 19:33:58.000000 database-without-orm-local-0.0.19/database_without_orm_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:33:58.557717 database-without-orm-local-0.0.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-31 19:33:33.000000 database-without-orm-local-0.0.19/setup.py
```

### Comparing `database-without-orm-local-0.0.18/setup.py` & `database-without-orm-local-0.0.19/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import setuptools
 # used by python -m build
 setuptools.setup(
     name='database-without-orm-local',
-    version='0.0.18',  # https://pypi.org/project/database-without-orm-local/
+    version='0.0.19',  # https://pypi.org/project/database-without-orm-local/
     author="Circles",
     author_email="info@circles.life",
     description="Circles Local Database without ORM Python PyPI Package",
     long_description="This is a package for sharing common Database methods",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
          "License :: Other/Proprietary License",
          "Operating System :: OS Independent",
     ],
 )
+
+
+
```

