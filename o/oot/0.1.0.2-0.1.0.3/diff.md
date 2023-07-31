# Comparing `tmp/oot-0.1.0.2.tar.gz` & `tmp/oot-0.1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oot-0.1.0.2.tar", max compression
+gzip compressed data, was "oot-0.1.0.3.tar", max compression
```

## Comparing `oot-0.1.0.2.tar` & `oot-0.1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-07-31 10:57:36.588541 oot-0.1.0.2/LICENSE
--rw-r--r--   0        0        0     3050 2023-07-31 10:57:36.588541 oot-0.1.0.2/README.md
--rw-r--r--   0        0        0       32 2023-07-31 10:57:36.588541 oot-0.1.0.2/oot/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-31 10:57:36.592541 oot-0.1.0.2/oot/loaders.py
--rw-r--r--   0        0        0     1316 2023-07-31 10:57:36.592541 oot-0.1.0.2/oot/m_exceptions.py
--rw-r--r--   0        0        0     1423 2023-07-31 10:57:36.592541 oot-0.1.0.2/oot/main.py
--rw-r--r--   0        0        0     1225 2023-07-31 10:57:36.592541 oot-0.1.0.2/oot/parser.py
--rw-r--r--   0        0        0     1897 2023-07-31 10:57:36.592541 oot-0.1.0.2/oot/schema_validator.py
--rw-r--r--   0        0        0      586 2023-07-31 10:57:36.592541 oot-0.1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 oot-0.1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 11:15:57.816553 oot-0.1.0.3/LICENSE
+-rw-r--r--   0        0        0     3110 2023-07-31 11:15:57.816553 oot-0.1.0.3/README.md
+-rw-r--r--   0        0        0       32 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/loaders.py
+-rw-r--r--   0        0        0     1316 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/m_exceptions.py
+-rw-r--r--   0        0        0     1423 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/main.py
+-rw-r--r--   0        0        0     1225 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/parser.py
+-rw-r--r--   0        0        0     1897 2023-07-31 11:15:57.816553 oot-0.1.0.3/oot/schema_validator.py
+-rw-r--r--   0        0        0      586 2023-07-31 11:15:57.820553 oot-0.1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 oot-0.1.0.3/PKG-INFO
```

### Comparing `oot-0.1.0.2/LICENSE` & `oot-0.1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/README.md` & `oot-0.1.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 The Templar starts his task. He replaces the `TEMPLAR_NAME` variable with the name of a famous Templar. He then resolves the `HALL_OF_HONOR` environment variable, revealing the name of the sacred hall. Once the manuscript has been decoded, he validates it, ensuring it adheres to the ancient schema:
 
 ```python
 from oot import parse_file
 
 file_path = "manuscript.yaml"
 variables = {"TEMPLAR_NAME": "Jacques de Molay"}
-os.environ["HALL_OF_HONOR"] = "Hall of the Brave"
+os.environ["HALL_OF_HONOR"] = "Hall of the Brave" # Environmental variables will be automatically substituted
 
 # The Templar decodes the manuscript
 manuscript = parse_file(file_path, context=variables)
 
 # The manuscript is decoded:
 assert manuscript == {"Templar": "Jacques de Molay", "HallOfHonor": "Hall of the Brave"}
```

### Comparing `oot-0.1.0.2/oot/loaders.py` & `oot-0.1.0.3/oot/loaders.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/oot/m_exceptions.py` & `oot-0.1.0.3/oot/m_exceptions.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/oot/main.py` & `oot-0.1.0.3/oot/main.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/oot/parser.py` & `oot-0.1.0.3/oot/parser.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/oot/schema_validator.py` & `oot-0.1.0.3/oot/schema_validator.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0.2/pyproject.toml` & `oot-0.1.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oot"
-version = "0.1.0.2"
+version = "0.1.0.3"
 description = "Order of the Template: A Python package for parsing Jinja templates and YAML files with environment variables."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `oot-0.1.0.2/PKG-INFO` & `oot-0.1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oot
-Version: 0.1.0.2
+Version: 0.1.0.3
 Summary: Order of the Template: A Python package for parsing Jinja templates and YAML files with environment variables.
 License: MIT
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -38,15 +38,15 @@
 The Templar starts his task. He replaces the `TEMPLAR_NAME` variable with the name of a famous Templar. He then resolves the `HALL_OF_HONOR` environment variable, revealing the name of the sacred hall. Once the manuscript has been decoded, he validates it, ensuring it adheres to the ancient schema:
 
 ```python
 from oot import parse_file
 
 file_path = "manuscript.yaml"
 variables = {"TEMPLAR_NAME": "Jacques de Molay"}
-os.environ["HALL_OF_HONOR"] = "Hall of the Brave"
+os.environ["HALL_OF_HONOR"] = "Hall of the Brave" # Environmental variables will be automatically substituted
 
 # The Templar decodes the manuscript
 manuscript = parse_file(file_path, context=variables)
 
 # The manuscript is decoded:
 assert manuscript == {"Templar": "Jacques de Molay", "HallOfHonor": "Hall of the Brave"}
```

