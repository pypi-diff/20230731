# Comparing `tmp/tokenize_rt-5.1.0.tar.gz` & `tmp/tokenize_rt-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokenize_rt-5.1.0.tar", last modified: Sat Jun 10 20:35:48 2023, max compression
+gzip compressed data, was "tokenize_rt-5.2.0.tar", last modified: Sun Jul 30 22:45:24 2023, max compression
```

## Comparing `tokenize_rt-5.1.0.tar` & `tokenize_rt-5.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/LICENSE
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)     3438 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/README.md
--rw-r--r--   0 asottile  (1000) asottile  (1000)     1114 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/setup.cfg
--rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-06-10 20:12:24.000000 tokenize_rt-5.1.0/setup.py
-drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-06-10 20:35:48.292503 tokenize_rt-5.1.0/tokenize_rt.egg-info/
--rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/PKG-INFO
--rw-r--r--   0 asottile  (1000) asottile  (1000)      229 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/SOURCES.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/dependency_links.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       49 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/entry_points.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-06-10 20:35:48.000000 tokenize_rt-5.1.0/tokenize_rt.egg-info/top_level.txt
--rw-r--r--   0 asottile  (1000) asottile  (1000)     5702 2023-06-10 20:31:42.000000 tokenize_rt-5.1.0/tokenize_rt.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 22:45:24.533376 tokenize_rt-5.2.0/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1059 2023-07-30 22:41:25.000000 tokenize_rt-5.2.0/LICENSE
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-07-30 22:45:24.533376 tokenize_rt-5.2.0/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     3438 2023-07-30 22:41:25.000000 tokenize_rt-5.2.0/README.md
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     1114 2023-07-30 22:45:24.533376 tokenize_rt-5.2.0/setup.cfg
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       73 2023-07-30 22:41:25.000000 tokenize_rt-5.2.0/setup.py
+drwxr-xr-x   0 asottile  (1000) asottile  (1000)        0 2023-07-30 22:45:24.533376 tokenize_rt-5.2.0/tokenize_rt.egg-info/
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     4062 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.egg-info/PKG-INFO
+-rw-r--r--   0 asottile  (1000) asottile  (1000)      229 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)        1 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       49 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.egg-info/entry_points.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)       12 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.egg-info/top_level.txt
+-rw-r--r--   0 asottile  (1000) asottile  (1000)     5809 2023-07-30 22:45:24.000000 tokenize_rt-5.2.0/tokenize_rt.py
```

### Comparing `tokenize_rt-5.1.0/LICENSE` & `tokenize_rt-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokenize_rt-5.1.0/PKG-INFO` & `tokenize_rt-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenize_rt
-Version: 5.1.0
+Version: 5.2.0
 Summary: A wrapper around the stdlib `tokenize` which roundtrips.
 Home-page: https://github.com/asottile/tokenize-rt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tokenize_rt-5.1.0/README.md` & `tokenize_rt-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tokenize_rt-5.1.0/setup.cfg` & `tokenize_rt-5.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tokenize_rt
-version = 5.1.0
+version = 5.2.0
 description = A wrapper around the stdlib `tokenize` which roundtrips.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/asottile/tokenize-rt
 author = Anthony Sottile
 author_email = asottile@umich.edu
 license = MIT
```

### Comparing `tokenize_rt-5.1.0/tokenize_rt.egg-info/PKG-INFO` & `tokenize_rt-5.2.0/tokenize_rt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokenize-rt
-Version: 5.1.0
+Version: 5.2.0
 Summary: A wrapper around the stdlib `tokenize` which roundtrips.
 Home-page: https://github.com/asottile/tokenize-rt
 Author: Anthony Sottile
 Author-email: asottile@umich.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tokenize_rt-5.1.0/tokenize_rt.py` & `tokenize_rt-5.2.0/tokenize_rt.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # this is a performance hack.  see https://bugs.python.org/issue43014
 if (  # pragma: no branch
         sys.version_info < (3, 10) and
         callable(getattr(tokenize, '_compile', None))
 ):  # pragma: <3.10 cover
     from functools import lru_cache
-    tokenize._compile = lru_cache()(tokenize._compile)
+    tokenize._compile = lru_cache(tokenize._compile)
 
 ESCAPED_NL = 'ESCAPED_NL'
 UNIMPORTANT_WS = 'UNIMPORTANT_WS'
 NON_CODING_TOKENS = frozenset(('COMMENT', ESCAPED_NL, 'NL', UNIMPORTANT_WS))
 
 
 class Offset(NamedTuple):
@@ -36,14 +36,17 @@
     line: int | None = None
     utf8_byte_offset: int | None = None
 
     @property
     def offset(self) -> Offset:
         return Offset(self.line, self.utf8_byte_offset)
 
+    def matches(self, *, name: str, src: str) -> bool:
+        return self.name == name and self.src == src
+
 
 _string_re = re.compile('^([^\'"]*)(.*)$', re.DOTALL)
 _escaped_nl_re = re.compile(r'\\(\n|\r\n|\r)')
 
 
 def _re_partition(regex: Pattern[str], s: str) -> tuple[str, str, str]:
     match = regex.search(s)
```

