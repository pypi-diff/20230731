# Comparing `tmp/quickbar-0.1.1.tar.gz` & `tmp/quickbar-0.1.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbar-0.1.1.tar", max compression
+gzip compressed data, was "quickbar-0.1.1.post0.tar", max compression
```

## Comparing `quickbar-0.1.1.tar` & `quickbar-0.1.1.post0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      434 2023-07-28 00:37:36.475223 quickbar-0.1.1/README.md
--rw-r--r--   0        0        0      564 2023-07-31 02:21:17.669618 quickbar-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      234 2023-07-28 00:27:29.256852 quickbar-0.1.1/quickbar/README.md
--rw-r--r--   0        0        0       41 2023-07-27 18:42:44.521026 quickbar-0.1.1/quickbar/__init__.py
--rw-r--r--   0        0        0     1962 2023-07-28 00:25:31.648766 quickbar-0.1.1/quickbar/__main__.py
--rw-r--r--   0        0        0     2596 2023-07-31 02:02:48.808892 quickbar-0.1.1/quickbar/core.py
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 quickbar-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-07-28 00:37:36.475223 quickbar-0.1.1.post0/README.md
+-rw-r--r--   0        0        0      570 2023-07-31 02:36:38.279914 quickbar-0.1.1.post0/pyproject.toml
+-rw-r--r--   0        0        0      234 2023-07-28 00:27:29.256852 quickbar-0.1.1.post0/quickbar/README.md
+-rw-r--r--   0        0        0       41 2023-07-27 18:42:44.521026 quickbar-0.1.1.post0/quickbar/__init__.py
+-rw-r--r--   0        0        0     1962 2023-07-28 00:25:31.648766 quickbar-0.1.1.post0/quickbar/__main__.py
+-rw-r--r--   0        0        0     2622 2023-07-31 02:36:25.634044 quickbar-0.1.1.post0/quickbar/core.py
+-rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 quickbar-0.1.1.post0/PKG-INFO
```

### Comparing `quickbar-0.1.1/pyproject.toml` & `quickbar-0.1.1.post0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickbar"
-version = "0.1.1"
+version = "0.1.1-post0"
 description = "A small python package to make rich progress bars as easy as 1,2,3."
 authors = ["volt-france <arno.veletanlic@volteuropa.org>"]
 readme = "README.md"
 homepage="https://github.com/arnos-stuff/quickbar"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `quickbar-0.1.1/quickbar/__main__.py` & `quickbar-0.1.1.post0/quickbar/__main__.py`

 * *Files identical despite different names*

### Comparing `quickbar-0.1.1/quickbar/core.py` & `quickbar-0.1.1.post0/quickbar/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,8 +73,9 @@
                     qbar.bar.advance(task_id=task_id)
                     yield item
                 qbar.bar.stop()
                 qbar.bar.remove_task(task_id=task_id)
             except Exception as err:
                 qbar.bar.stop()
                 qbar.bar.remove_task(task_id=task_id)
+                raise err
         return callback()
```

### Comparing `quickbar-0.1.1/PKG-INFO` & `quickbar-0.1.1.post0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbar
-Version: 0.1.1
+Version: 0.1.1.post0
 Summary: A small python package to make rich progress bars as easy as 1,2,3.
 Home-page: https://github.com/arnos-stuff/quickbar
 Author: volt-france
 Author-email: arno.veletanlic@volteuropa.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

