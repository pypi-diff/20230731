# Comparing `tmp/st-supabase-connection-0.0.0.tar.gz` & `tmp/st-supabase-connection-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-supabase-connection-0.0.0.tar", last modified: Sat Jul 29 12:36:26 2023, max compression
+gzip compressed data, was "st-supabase-connection-0.0.1.tar", last modified: Mon Jul 31 19:39:52 2023, max compression
```

## Comparing `st-supabase-connection-0.0.0.tar` & `st-supabase-connection-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:36:26.874393 st-supabase-connection-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-29 12:36:11.000000 st-supabase-connection-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-29 12:36:11.000000 st-supabase-connection-0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-29 12:36:26.870393 st-supabase-connection-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-29 12:36:11.000000 st-supabase-connection-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 12:36:26.874393 st-supabase-connection-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-29 12:36:11.000000 st-supabase-connection-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:36:26.866393 st-supabase-connection-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:36:26.870393 st-supabase-connection-0.0.0/src/st_supabase_connection/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-29 12:36:11.000000 st-supabase-connection-0.0.0/src/st_supabase_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 12:36:26.870393 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-29 12:36:26.000000 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-29 12:36:26.000000 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 12:36:26.000000 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-29 12:36:26.000000 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-29 12:36:26.000000 st-supabase-connection-0.0.0/src/st_supabase_connection.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.419790 st-supabase-connection-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.419790 st-supabase-connection-0.0.1/src/st_supabase_connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-31 19:39:43.000000 st-supabase-connection-0.0.1/src/st_supabase_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 19:39:52.423790 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-31 19:39:52.000000 st-supabase-connection-0.0.1/src/st_supabase_connection.egg-info/top_level.txt
```

### Comparing `st-supabase-connection-0.0.0/LICENSE` & `st-supabase-connection-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `st-supabase-connection-0.0.0/setup.py` & `st-supabase-connection-0.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     author_email="siddhant.sadangi@gmail.com",
     description="A Streamlit connection component for Supabase.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     project_urls={
         "Homepage": "https://github.com/SiddhantSadangi/st_supabase_connection",
         "Documentation": "https://github.com/SiddhantSadangi/st_supabase_connection/blob/main/README.md",
-        "Support": "https://www.buymeacoffee.com/siddhantsadangi",
+        "Funding": "https://www.buymeacoffee.com/siddhantsadangi",
     },
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     classifiers=[
         "Environment :: Plugins",
         "Environment :: Web Environment",
```

