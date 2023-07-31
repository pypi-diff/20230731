# Comparing `tmp/tabb-0.3.1.tar.gz` & `tmp/tabb-0.3.2.tar.gz`

## Comparing `tabb-0.3.1.tar` & `tabb-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.1/.DS_Store
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.3.1/config.json
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.3.1/test.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.3.1/todo.md
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.3.1/font/config.toml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.1/src/.DS_Store
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/__about__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/__init__.py
--rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/base.py
--rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/callback.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/command.py
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/config.py
--rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/context.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/decorators.py
--rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/exceptions.py
--rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/formatter.py
--rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/group.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/missing.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/nargs.py
--rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/py.typed
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/types.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/utils.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/__init__.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/base.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/depends.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/group.py
--rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/parser.py
--rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/resolve.py
--rw-r--r--   0        0        0    32051 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/types.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.3.1/src/tabb/parameter/utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.3.1/tests/__init__.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.3.1/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.3.1/LICENSE.txt
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.3.1/README.md
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.2/.DS_Store
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 tabb-0.3.2/config.json
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 tabb-0.3.2/test.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 tabb-0.3.2/todo.md
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 tabb-0.3.2/font/config.toml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tabb-0.3.2/src/.DS_Store
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/__about__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/__init__.py
+-rw-r--r--   0        0        0    10873 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/base.py
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/callback.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/command.py
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/config.py
+-rw-r--r--   0        0        0     4997 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/context.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/decorators.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/exceptions.py
+-rw-r--r--   0        0        0    11282 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/formatter.py
+-rw-r--r--   0        0        0     7792 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/group.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/missing.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/nargs.py
+-rw-r--r--   0        0        0    16407 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/py.typed
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/types.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/utils.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/__init__.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/base.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/depends.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/group.py
+-rw-r--r--   0        0        0    10284 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/parser.py
+-rw-r--r--   0        0        0    11424 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/resolve.py
+-rw-r--r--   0        0        0    32224 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/types.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 tabb-0.3.2/src/tabb/parameter/utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tabb-0.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 tabb-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 tabb-0.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 tabb-0.3.2/README.md
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 tabb-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 tabb-0.3.2/PKG-INFO
```

### Comparing `tabb-0.3.1/.DS_Store` & `tabb-0.3.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/test.py` & `tabb-0.3.2/test.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/.DS_Store` & `tabb-0.3.2/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/__init__.py` & `tabb-0.3.2/src/tabb/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/base.py` & `tabb-0.3.2/src/tabb/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/callback.py` & `tabb-0.3.2/src/tabb/callback.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/command.py` & `tabb-0.3.2/src/tabb/command.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/config.py` & `tabb-0.3.2/src/tabb/config.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/context.py` & `tabb-0.3.2/src/tabb/context.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/decorators.py` & `tabb-0.3.2/src/tabb/decorators.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/exceptions.py` & `tabb-0.3.2/src/tabb/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/formatter.py` & `tabb-0.3.2/src/tabb/formatter.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/group.py` & `tabb-0.3.2/src/tabb/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/nargs.py` & `tabb-0.3.2/src/tabb/nargs.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parser.py` & `tabb-0.3.2/src/tabb/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/types.py` & `tabb-0.3.2/src/tabb/types.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/utils.py` & `tabb-0.3.2/src/tabb/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/__init__.py` & `tabb-0.3.2/src/tabb/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/base.py` & `tabb-0.3.2/src/tabb/parameter/base.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/depends.py` & `tabb-0.3.2/src/tabb/parameter/depends.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/group.py` & `tabb-0.3.2/src/tabb/parameter/group.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/parser.py` & `tabb-0.3.2/src/tabb/parameter/parser.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/resolve.py` & `tabb-0.3.2/src/tabb/parameter/resolve.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/src/tabb/parameter/types.py` & `tabb-0.3.2/src/tabb/parameter/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,19 @@
             return MISSING
 
         if len(args) != 1 and not self.allow_overwrite:
             self.fail("Parameter already set.")
 
         return self.process_arg(args[-1])
 
+    def process_config(self, value: object) -> object:
+        if isinstance(value, str):
+            return self.parse(value)
+        return super().process_config(value)
+
     def parse_envvar(self, value: str) -> ValueType:
         return self.parse(value)
 
     def validate(self, value: Any) -> TypeGuard[ValueType]:
         if isinstance(self.type, type) and not isinstance(value, self.type):
             self.fail(f"Expected {self.name} value")
         return True
```

### Comparing `tabb-0.3.1/src/tabb/parameter/utils.py` & `tabb-0.3.2/src/tabb/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/.gitignore` & `tabb-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/LICENSE.txt` & `tabb-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/README.md` & `tabb-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/pyproject.toml` & `tabb-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tabb-0.3.1/PKG-INFO` & `tabb-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabb
-Version: 0.3.1
+Version: 0.3.2
 Summary: Trevor's argparse but better.
 Project-URL: Documentation, https://github.com/wtolson/tabb#readme
 Project-URL: Issues, https://github.com/wtolson/tabb/issues
 Project-URL: Source, https://github.com/wtolson/tabb
 Author-email: Trevor Olson <trevor@heytrevor.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

