# Comparing `tmp/pytest_ruff-0.1.tar.gz` & `tmp/pytest_ruff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ruff-0.1.tar", max compression
+gzip compressed data, was "pytest_ruff-0.1.1.tar", max compression
```

## Comparing `pytest_ruff-0.1.tar` & `pytest_ruff-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1062 2023-06-08 09:25:34.880817 pytest_ruff-0.1/LICENSE
--rw-r--r--   0        0        0      542 2023-06-08 09:25:34.880817 pytest_ruff-0.1/README.md
--rw-r--r--   0        0        0     1190 2023-06-08 09:26:11.084066 pytest_ruff-0.1/pyproject.toml
--rw-r--r--   0        0        0     2436 2023-06-08 09:25:34.880817 pytest_ruff-0.1/pytest_ruff.py
--rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pytest_ruff-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-07-31 16:40:57.312476 pytest_ruff-0.1.1/LICENSE
+-rw-r--r--   0        0        0      542 2023-07-31 16:40:57.312476 pytest_ruff-0.1.1/README.md
+-rw-r--r--   0        0        0     1192 2023-07-31 16:41:43.769363 pytest_ruff-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2426 2023-07-31 16:40:57.312476 pytest_ruff-0.1.1/pytest_ruff.py
+-rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 pytest_ruff-0.1.1/PKG-INFO
```

### Comparing `pytest_ruff-0.1/LICENSE` & `pytest_ruff-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.1/README.md` & `pytest_ruff-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.1/pyproject.toml` & `pytest_ruff-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-ruff"
-version = "0.1"
+version = "0.1.1"
 description = "pytest plugin to check ruff requirements."
 authors = ["Iuri de Silvio <iurisilvio@gmail.com>"]
 readme = "README.md"
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "Operating System :: OS Independent", "Framework :: Pytest", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 :: Only", "Topic :: Software Development :: Libraries :: Python Modules"]
 
 [tool.poetry.urls]
 Homepage = "https://github.com/businho/pytest-ruff"
```

### Comparing `pytest_ruff-0.1/pytest_ruff.py` & `pytest_ruff-0.1.1/pytest_ruff.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,12 +77,12 @@
 
     def reportinfo(self):
         return (self.fspath, None, "")
 
 
 def check_file(path):
     ruff = find_ruff_bin()
-    command = f"{ruff} {path} --quiet --show-source"
-    child = Popen(command, shell=True, stdout=PIPE, stderr=PIPE)
+    command = [ruff, path, '--quiet', '--show-source']
+    child = Popen(command, stdout=PIPE, stderr=PIPE)
     stdout, _ = child.communicate()
     if stdout:
         raise RuffError(stdout.decode())
```

### Comparing `pytest_ruff-0.1/PKG-INFO` & `pytest_ruff-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-ruff
-Version: 0.1
+Version: 0.1.1
 Summary: pytest plugin to check ruff requirements.
 Author: Iuri de Silvio
 Author-email: iurisilvio@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

