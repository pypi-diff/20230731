# Comparing `tmp/bstk_datatables-0.2.2.tar.gz` & `tmp/bstk_datatables-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bstk_datatables-0.2.2.tar", max compression
+gzip compressed data, was "bstk_datatables-0.2.3.tar", max compression
```

## Comparing `bstk_datatables-0.2.2.tar` & `bstk_datatables-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4244 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/README.md
--rw-r--r--   0        0        0     2497 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/__init__.py
--rw-r--r--   0        0        0     2311 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/entry.py
--rw-r--r--   0        0        0      560 2023-07-28 06:43:42.066491 bstk_datatables-0.2.2/bstk_datatables/enum.py
--rw-r--r--   0        0        0     3522 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/merge.py
--rw-r--r--   0        0        0     9807 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/schema.py
--rw-r--r--   0        0        0     1565 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/table.py
--rw-r--r--   0        0        0     1680 2023-07-28 06:43:42.070491 bstk_datatables-0.2.2/bstk_datatables/validators/luhn.py
--rw-r--r--   0        0        0      669 2023-07-28 06:44:08.318630 bstk_datatables-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4244 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/README.md
+-rw-r--r--   0        0        0     2497 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/__init__.py
+-rw-r--r--   0        0        0     2311 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/entry.py
+-rw-r--r--   0        0        0      560 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/enum.py
+-rw-r--r--   0        0        0     3522 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/merge.py
+-rw-r--r--   0        0        0     9807 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/schema.py
+-rw-r--r--   0        0        0     1565 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/table.py
+-rw-r--r--   0        0        0     1690 2023-07-31 09:06:00.747099 bstk_datatables-0.2.3/bstk_datatables/validators/luhn.py
+-rw-r--r--   0        0        0      669 2023-07-31 09:06:21.394755 bstk_datatables-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5009 1970-01-01 00:00:00.000000 bstk_datatables-0.2.3/PKG-INFO
```

### Comparing `bstk_datatables-0.2.2/README.md` & `bstk_datatables-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/__init__.py` & `bstk_datatables-0.2.3/bstk_datatables/__init__.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/entry.py` & `bstk_datatables-0.2.3/bstk_datatables/entry.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/enum.py` & `bstk_datatables-0.2.3/bstk_datatables/enum.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/merge.py` & `bstk_datatables-0.2.3/bstk_datatables/merge.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/schema.py` & `bstk_datatables-0.2.3/bstk_datatables/schema.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/table.py` & `bstk_datatables-0.2.3/bstk_datatables/table.py`

 * *Files identical despite different names*

### Comparing `bstk_datatables-0.2.2/bstk_datatables/validators/luhn.py` & `bstk_datatables-0.2.3/bstk_datatables/validators/luhn.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     _min_length: int = None
     default_message = "Number does not appear to be valid."
 
     def __init__(
         self,
         min_length: typing.Optional[int] = 2,
         *,
-        error: str | None = None,
+        error: typing.Optional[str] = None,
     ):
         self._min_length = min_length
         self.error = error or self.default_message  # type: str
 
     def _repr_args(self) -> str:
         return f"min_length={self._min_length!r}"
```

### Comparing `bstk_datatables-0.2.2/pyproject.toml` & `bstk_datatables-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bstk-datatables"
-version = "0.2.2"
+version = "0.2.3"
 description = "A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!"
 authors = ["colin <colin@broadstack.com.au>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "bstk_datatables" }]
 
 [tool.poetry.dependencies]
```

### Comparing `bstk_datatables-0.2.2/PKG-INFO` & `bstk_datatables-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bstk-datatables
-Version: 0.2.2
+Version: 0.2.3
 Summary: A polymorphic schema managed semi structured crosslinked data dictionary builder.. BINGO!
 License: MIT
 Author: colin
 Author-email: colin@broadstack.com.au
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

