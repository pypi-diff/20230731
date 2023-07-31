# Comparing `tmp/bsc_utils-1.0.2.tar.gz` & `tmp/bsc_utils-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsc_utils-1.0.2.tar", last modified: Thu Jul  6 08:54:12 2023, max compression
+gzip compressed data, was "bsc_utils-1.0.2b0.tar", last modified: Tue Jul 18 06:40:05 2023, max compression
```

## Comparing `bsc_utils-1.0.2.tar` & `bsc_utils-1.0.2b0.tar`

### file list

```diff
@@ -1,23 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.517596 bsc_utils-1.0.2/
--rw-rw-rw-   0        0        0       26 2023-05-15 03:09:29.000000 bsc_utils-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      547 2023-07-06 08:54:12.516593 bsc_utils-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-05-15 02:48:57.000000 bsc_utils-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.503723 bsc_utils-1.0.2/bsc_utils/
--rw-rw-rw-   0        0        0       21 2023-07-06 08:51:57.000000 bsc_utils-1.0.2/bsc_utils/__init__.py
--rw-rw-rw-   0        0        0      544 2023-07-06 08:42:23.000000 bsc_utils-1.0.2/bsc_utils/_config.py
--rw-rw-rw-   0        0        0      505 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/_helpers.py
--rw-rw-rw-   0        0        0      788 2023-06-21 09:27:42.000000 bsc_utils-1.0.2/bsc_utils/chat.py
--rw-rw-rw-   0        0        0     1097 2023-07-06 08:42:23.000000 bsc_utils-1.0.2/bsc_utils/crawl.py
--rw-rw-rw-   0        0        0     2688 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/database.py
--rw-rw-rw-   0        0        0      231 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/exceptions.py
--rw-rw-rw-   0        0        0     2073 2023-06-21 09:22:44.000000 bsc_utils-1.0.2/bsc_utils/time.py
--rw-rw-rw-   0        0        0     2700 2023-06-08 01:45:46.000000 bsc_utils-1.0.2/bsc_utils/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:54:12.513586 bsc_utils-1.0.2/bsc_utils.egg-info/
--rw-rw-rw-   0        0        0      547 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-06 08:54:12.000000 bsc_utils-1.0.2/bsc_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      160 2023-06-21 09:27:42.000000 bsc_utils-1.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 08:54:12.519602 bsc_utils-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1083 2023-05-15 03:04:43.000000 bsc_utils-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:40:05.046096 bsc_utils-1.0.2b0/
+-rw-rw-rw-   0        0        0       26 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/MANIFEST.in
+-rw-rw-rw-   0        0        0      549 2023-07-18 06:40:05.042094 bsc_utils-1.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 06:40:04.915090 bsc_utils-1.0.2b0/bsc_utils/
+-rw-rw-rw-   0        0        0       22 2023-07-18 06:39:59.000000 bsc_utils-1.0.2b0/bsc_utils/__init__.py
+-rw-rw-rw-   0        0        0      544 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/_config.py
+-rw-rw-rw-   0        0        0      505 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/_helpers.py
+-rw-rw-rw-   0        0        0      788 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/chat.py
+-rw-rw-rw-   0        0        0     1097 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/crawl.py
+-rw-rw-rw-   0        0        0     2728 2023-07-18 04:13:02.000000 bsc_utils-1.0.2b0/bsc_utils/database.py
+-rw-rw-rw-   0        0        0      231 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/exceptions.py
+-rw-rw-rw-   0        0        0     2073 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/time.py
+-rw-rw-rw-   0        0        0     2700 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/bsc_utils/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:40:04.984098 bsc_utils-1.0.2b0/bsc_utils.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-07-18 06:40:04.000000 bsc_utils-1.0.2b0/bsc_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2023-07-18 06:40:04.000000 bsc_utils-1.0.2b0/bsc_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 06:40:04.000000 bsc_utils-1.0.2b0/bsc_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-07-18 06:40:04.000000 bsc_utils-1.0.2b0/bsc_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 06:40:04.000000 bsc_utils-1.0.2b0/bsc_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      176 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 06:40:05.047101 bsc_utils-1.0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     1083 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 06:40:05.034102 bsc_utils-1.0.2b0/tests/
+-rw-rw-rw-   0        0        0      591 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/tests/test_chat.py
+-rw-rw-rw-   0        0        0      445 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/tests/test_crawl.py
+-rw-rw-rw-   0        0        0     1566 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/tests/test_database.py
+-rw-rw-rw-   0        0        0     2264 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/tests/test_time.py
+-rw-rw-rw-   0        0        0     2322 2023-07-18 04:25:01.000000 bsc_utils-1.0.2b0/tests/test_visual.py
```

### Comparing `bsc_utils-1.0.2/PKG-INFO` & `bsc_utils-1.0.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc_utils
-Version: 1.0.2
+Version: 1.0.2b0
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.2/bsc_utils/_config.py` & `bsc_utils-1.0.2b0/bsc_utils/_config.py`

 * *Files identical despite different names*

### Comparing `bsc_utils-1.0.2/bsc_utils/chat.py` & `bsc_utils-1.0.2b0/bsc_utils/chat.py`

 * *Files identical despite different names*

### Comparing `bsc_utils-1.0.2/bsc_utils/crawl.py` & `bsc_utils-1.0.2b0/bsc_utils/crawl.py`

 * *Files identical despite different names*

### Comparing `bsc_utils-1.0.2/bsc_utils/database.py` & `bsc_utils-1.0.2b0/bsc_utils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,18 +27,19 @@
         return pymssql.connect(
             server=config.mssql_server,
             user=config.mssql_user,
             password=config.mssql_password,
             database=config.mssql_database,
         )
     elif database == Database.ORACLE:
+        oracledb.init_oracle_client()
         return oracledb.connect(
             user=config.oracle_user,
             password=config.oracle_password,
-            dsn=config.oracle_dsn
+            dsn=config.oracle_dsn,
         )
     elif database == Database.SQLITE:
         return sqlite3.connect(database=config.sqlite_path)
 
     elif database == Database.ACCESS:
         return pyodbc.connect(
             f'''
```

### Comparing `bsc_utils-1.0.2/bsc_utils/time.py` & `bsc_utils-1.0.2b0/bsc_utils/time.py`

 * *Files identical despite different names*

### Comparing `bsc_utils-1.0.2/bsc_utils/visual.py` & `bsc_utils-1.0.2b0/bsc_utils/visual.py`

 * *Files identical despite different names*

### Comparing `bsc_utils-1.0.2/bsc_utils.egg-info/PKG-INFO` & `bsc_utils-1.0.2b0/bsc_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsc-utils
-Version: 1.0.2
+Version: 1.0.2b0
 Summary: Util Functions for BSC Quants
 Home-page: https://github.com/dang-trung/bsc-utils
 Author: Trung Dang
 Author-email: trungd@bsc.com.vn
 Maintainer: Trung Dang
 Maintainer-email: trungd@bsc.com.vn
 License: MIT
```

### Comparing `bsc_utils-1.0.2/setup.py` & `bsc_utils-1.0.2b0/setup.py`

 * *Files identical despite different names*

