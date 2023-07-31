# Comparing `tmp/betfairdatabase-0.1.0.tar.gz` & `tmp/betfairdatabase-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfairdatabase-0.1.0.tar", last modified: Fri Jul 28 18:24:21 2023, max compression
+gzip compressed data, was "betfairdatabase-0.1.1.tar", last modified: Mon Jul 31 12:52:42 2023, max compression
```

## Comparing `betfairdatabase-0.1.0.tar` & `betfairdatabase-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.225482 betfairdatabase-0.1.0/
--rw-rw-rw-   0        0        0     1067 2023-07-26 17:11:33.000000 betfairdatabase-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     4687 2023-07-28 18:24:21.225482 betfairdatabase-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3900 2023-07-28 18:17:23.000000 betfairdatabase-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.214837 betfairdatabase-0.1.0/betfairdatabase/
--rw-rw-rw-   0        0        0       48 2023-07-28 15:32:44.000000 betfairdatabase-0.1.0/betfairdatabase/__init__.py
--rw-rw-rw-   0        0        0     2369 2023-07-28 16:03:10.000000 betfairdatabase-0.1.0/betfairdatabase/api.py
--rw-rw-rw-   0        0        0     6714 2023-07-28 15:23:05.000000 betfairdatabase-0.1.0/betfairdatabase/core.py
--rw-rw-rw-   0        0        0      709 2023-07-27 22:17:23.000000 betfairdatabase-0.1.0/betfairdatabase/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.221492 betfairdatabase-0.1.0/betfairdatabase.egg-info/
--rw-rw-rw-   0        0        0     4687 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 18:24:21.000000 betfairdatabase-0.1.0/betfairdatabase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      853 2023-07-28 18:08:09.000000 betfairdatabase-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-28 18:24:21.226479 betfairdatabase-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-28 18:24:21.223486 betfairdatabase-0.1.0/tests/
--rw-rw-rw-   0        0        0    12295 2023-07-28 17:32:13.000000 betfairdatabase-0.1.0/tests/test_integration.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:52:42.151370 betfairdatabase-0.1.1/
+-rw-rw-rw-   0        0        0     1067 2023-07-26 17:11:33.000000 betfairdatabase-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4687 2023-07-31 12:52:42.150956 betfairdatabase-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3900 2023-07-28 18:17:23.000000 betfairdatabase-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-31 12:52:42.138987 betfairdatabase-0.1.1/betfairdatabase/
+-rw-rw-rw-   0        0        0       48 2023-07-28 15:32:44.000000 betfairdatabase-0.1.1/betfairdatabase/__init__.py
+-rw-rw-rw-   0        0        0     2369 2023-07-28 16:03:10.000000 betfairdatabase-0.1.1/betfairdatabase/api.py
+-rw-rw-rw-   0        0        0     6732 2023-07-31 12:51:47.000000 betfairdatabase-0.1.1/betfairdatabase/core.py
+-rw-rw-rw-   0        0        0      709 2023-07-27 22:17:23.000000 betfairdatabase-0.1.1/betfairdatabase/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-31 12:52:42.145968 betfairdatabase-0.1.1/betfairdatabase.egg-info/
+-rw-rw-rw-   0        0        0     4687 2023-07-31 12:52:42.000000 betfairdatabase-0.1.1/betfairdatabase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-07-31 12:52:42.000000 betfairdatabase-0.1.1/betfairdatabase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 12:52:42.000000 betfairdatabase-0.1.1/betfairdatabase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-31 12:52:42.000000 betfairdatabase-0.1.1/betfairdatabase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      853 2023-07-31 12:25:55.000000 betfairdatabase-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-31 12:52:42.151370 betfairdatabase-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-31 12:52:42.148960 betfairdatabase-0.1.1/tests/
+-rw-rw-rw-   0        0        0      617 2023-07-31 12:51:40.000000 betfairdatabase-0.1.1/tests/test_core.py
+-rw-rw-rw-   0        0        0    12295 2023-07-28 17:32:13.000000 betfairdatabase-0.1.1/tests/test_integration.py
```

### Comparing `betfairdatabase-0.1.0/LICENSE` & `betfairdatabase-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `betfairdatabase-0.1.0/PKG-INFO` & `betfairdatabase-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairdatabase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Turns a collection of historical Betfair data into a queryable SQL database.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/mzaja/betfair-database
 Project-URL: Bug Tracker, https://github.com/mzaja/betfair-database/issues
 Keywords: betfair,trading,betting,database
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `betfairdatabase-0.1.0/README.md` & `betfairdatabase-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `betfairdatabase-0.1.0/betfairdatabase/api.py` & `betfairdatabase-0.1.1/betfairdatabase/api.py`

 * *Files identical despite different names*

### Comparing `betfairdatabase-0.1.0/betfairdatabase/core.py` & `betfairdatabase-0.1.1/betfairdatabase/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     database directory.
     """
     return Path(database_dir).rglob("1.*.json")
 
 
 def parse_market_catalogue(market_catalogue_file: str | Path) -> dict:
     """Parses the market catalogue and"""
-    with open(market_catalogue_file) as f:
+    with open(market_catalogue_file, encoding="utf-8") as f:
         return json.load(f)
 
 
 def flatten_subdict(parent_dict: dict[str, object], child_key: str) -> None:
     """
     Modifies the dictionary in place.
     """
```

### Comparing `betfairdatabase-0.1.0/betfairdatabase/exceptions.py` & `betfairdatabase-0.1.1/betfairdatabase/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfairdatabase-0.1.0/betfairdatabase.egg-info/PKG-INFO` & `betfairdatabase-0.1.1/betfairdatabase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfairdatabase
-Version: 0.1.0
+Version: 0.1.1
 Summary: Turns a collection of historical Betfair data into a queryable SQL database.
 Author-email: Mario Zaja <mzaja0@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/mzaja/betfair-database
 Project-URL: Bug Tracker, https://github.com/mzaja/betfair-database/issues
 Keywords: betfair,trading,betting,database
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `betfairdatabase-0.1.0/pyproject.toml` & `betfairdatabase-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages=["betfairdatabase"]
 
 [project]
 name = "betfairdatabase"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mario Zaja", email="mzaja0@gmail.com" },
 ]
 description = "Turns a collection of historical Betfair data into a queryable SQL database."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
```

### Comparing `betfairdatabase-0.1.0/tests/test_integration.py` & `betfairdatabase-0.1.1/tests/test_integration.py`

 * *Files identical despite different names*

