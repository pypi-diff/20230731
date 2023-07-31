# Comparing `tmp/jupyterlite-0.1.0rc0.tar.gz` & `tmp/jupyterlite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr  1 06:43:15 2023, max compression
+gzip compressed data, last modified: Mon Jul 31 13:00:28 2023, max compression
```

## Comparing `jupyterlite-0.1.0rc0.tar` & `jupyterlite-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       57 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/jupyterlite/__init__.py
--rw-r--r--   0        0        0       81 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/jupyterlite/__main__.py
--rw-r--r--   0        0        0      354 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/jupyterlite/constants.py
--rw-r--r--   0        0        0      331 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/jupyterlite/addons/base.py
--rw-r--r--   0        0        0     2104 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/.gitignore
--rw-r--r--   0        0        0     5346 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/README.md
--rw-r--r--   0        0        0     2065 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     7536 2023-04-01 06:43:15.000000 jupyterlite-0.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/jupyterlite/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/jupyterlite/__main__.py
+-rw-r--r--   0        0        0      354 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/jupyterlite/constants.py
+-rw-r--r--   0        0        0      331 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/jupyterlite/addons/base.py
+-rw-r--r--   0        0        0     2104 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1524 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5346 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/README.md
+-rw-r--r--   0        0        0     2096 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9312 2023-07-31 13:00:28.000000 jupyterlite-0.1.1/PKG-INFO
```

### Comparing `jupyterlite-0.1.0rc0/.gitignore` & `jupyterlite-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.1.0rc0/README.md` & `jupyterlite-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite-0.1.0rc0/pyproject.toml` & `jupyterlite-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     "js",
     "jupyter",
     "jupyterlab",
     "notebook",
     "pyodide",
     "schema",
 ]
+license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
```

### Comparing `jupyterlite-0.1.0rc0/PKG-INFO` & `jupyterlite-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,42 @@
 Metadata-Version: 2.1
 Name: jupyterlite
-Version: 0.1.0rc0
+Version: 0.1.1
 Project-URL: Source, https://github.com/jupyterlite/jupyterlite
 Author: JupyterLite Contributors
+License: BSD 3-Clause License
+        
+        Copyright (c) 2022, JupyterLite Contributors
+        All rights reserved.
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        * Redistributions of source code must retain the above copyright notice, this
+          list of conditions and the following disclaimer.
+        
+        * Redistributions in binary form must reproduce the above copyright notice,
+          this list of conditions and the following disclaimer in the documentation
+          and/or other materials provided with the distribution.
+        
+        * Neither the name of the copyright holder nor the names of its
+          contributors may be used to endorse or promote products derived from
+          this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+License-File: LICENSE
 Keywords: browser,js,jupyter,jupyterlab,notebook,pyodide,schema
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

