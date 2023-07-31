# Comparing `tmp/padic-0.2.2.tar.gz` & `tmp/padic-0.2.2.1.tar.gz`

## Comparing `padic-0.2.2.tar` & `padic-0.2.2.1.tar`

### file list

```diff
@@ -1,6 +1,10 @@
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 padic-0.2.2/src/padic/__init__.py
--rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 padic-0.2.2/src/padic/padic.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 padic-0.2.2/LICENSE.txt
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 padic-0.2.2/README.md
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 padic-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 padic-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5868 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.1/padic-0.2.1-py3-none-any.whl
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.1/padic-0.2.1.tar.gz
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.2/padic-0.2.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 padic-0.2.2.1/2.2.2/padic-0.2.2.tar.gz
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 padic-0.2.2.1/src/padic/__init__.py
+-rw-r--r--   0        0        0    13882 2020-02-02 00:00:00.000000 padic-0.2.2.1/src/padic/padic.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 padic-0.2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 padic-0.2.2.1/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 padic-0.2.2.1/pyproject.toml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 padic-0.2.2.1/PKG-INFO
```

### Comparing `padic-0.2.2/src/padic/padic.py` & `padic-0.2.2.1/src/padic/padic.py`

 * *Files identical despite different names*

### Comparing `padic-0.2.2/LICENSE.txt` & `padic-0.2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `padic-0.2.2/pyproject.toml` & `padic-0.2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "padic"
-version = "0.2.2"
+version = "0.2.2.1"
 authors = [
   { name="MRaczuk", email="mraczuk@gmail.com" },
 ]
 description = "Package implementing p-adic numbers"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `padic-0.2.2/PKG-INFO` & `padic-0.2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: padic
-Version: 0.2.2
+Version: 0.2.2.1
 Summary: Package implementing p-adic numbers
 Project-URL: Homepage, https://github.com/MRaczuk/padic
 Author-email: MRaczuk <mraczuk@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

