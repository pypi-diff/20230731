# Comparing `tmp/fastapi-sa-manager-0.1.1.tar.gz` & `tmp/fastapi-sa-manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-sa-manager-0.1.1.tar", last modified: Mon Jul 31 08:13:09 2023, max compression
+gzip compressed data, was "fastapi-sa-manager-0.1.2.tar", last modified: Mon Jul 31 08:23:04 2023, max compression
```

## Comparing `fastapi-sa-manager-0.1.1.tar` & `fastapi-sa-manager-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-07-31 08:13:09.934584 fastapi-sa-manager-0.1.1/
--rw-r--r--   0 james     (1000) james     (1000)     1049 2023-07-31 08:09:17.000000 fastapi-sa-manager-0.1.1/LICENSE.md
--rw-r--r--   0 james     (1000) james     (1000)      409 2023-07-31 08:13:09.934584 fastapi-sa-manager-0.1.1/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      191 2023-07-31 08:09:51.000000 fastapi-sa-manager-0.1.1/README.md
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-07-31 08:13:09.934584 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)      409 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      279 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/SOURCES.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/dependency_links.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/not-zip-safe
--rw-r--r--   0 james     (1000) james     (1000)       19 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/requires.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.1/fastapi_sa_manager.egg-info/top_level.txt
--rw-r--r--   0 james     (1000) james     (1000)       38 2023-07-31 08:13:09.934584 fastapi-sa-manager-0.1.1/setup.cfg
--rw-r--r--   0 james     (1000) james     (1000)      620 2023-07-31 08:07:03.000000 fastapi-sa-manager-0.1.1/setup.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-07-31 08:23:04.335647 fastapi-sa-manager-0.1.2/
+-rw-r--r--   0 james     (1000) james     (1000)     1049 2023-07-31 08:09:17.000000 fastapi-sa-manager-0.1.2/LICENSE.md
+-rw-r--r--   0 james     (1000) james     (1000)      409 2023-07-31 08:23:04.335647 fastapi-sa-manager-0.1.2/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)      191 2023-07-31 08:09:51.000000 fastapi-sa-manager-0.1.2/README.md
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-07-31 08:23:04.335647 fastapi-sa-manager-0.1.2/fastapi_sa_manager/
+-rw-r--r--   0 james     (1000) james     (1000)        0 2023-07-31 08:19:47.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager/__init__.py
+-rw-r--r--   0 james     (1000) james     (1000)      316 2023-07-17 02:24:24.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager/schemas.py
+-rw-r--r--   0 james     (1000) james     (1000)     4722 2023-07-27 07:35:22.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager/services.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-07-31 08:23:04.335647 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/
+-rw-r--r--   0 james     (1000) james     (1000)      409 2023-07-31 08:23:04.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)      371 2023-07-31 08:23:04.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2023-07-31 08:23:04.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2023-07-31 08:13:09.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/not-zip-safe
+-rw-r--r--   0 james     (1000) james     (1000)       19 2023-07-31 08:23:04.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/requires.txt
+-rw-r--r--   0 james     (1000) james     (1000)       19 2023-07-31 08:23:04.000000 fastapi-sa-manager-0.1.2/fastapi_sa_manager.egg-info/top_level.txt
+-rw-r--r--   0 james     (1000) james     (1000)       38 2023-07-31 08:23:04.335647 fastapi-sa-manager-0.1.2/setup.cfg
+-rw-r--r--   0 james     (1000) james     (1000)      620 2023-07-31 08:22:15.000000 fastapi-sa-manager-0.1.2/setup.py
```

### Comparing `fastapi-sa-manager-0.1.1/LICENSE.md` & `fastapi-sa-manager-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi-sa-manager-0.1.1/setup.py` & `fastapi-sa-manager-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="fastapi-sa-manager",
-    version="0.1.1",
+    version="0.1.2",
     description="FastAPI-sa-manager is an SQLAlchemy ORM extension for FastAPI helping you to build CRUD APIs fast and easy.",
     author="esanzy87",
     author_email="esanzy87@gmail.com",
     install_requires=["fastapi", "sqlalchemy"],
     packages=find_packages(exclude=[]),
     keywords=["fastapi", "sqlalchemy"],
     python_requires=">=3.10",
```

