# Comparing `tmp/cmem_plugin_pyshacl-4.2.0rc3.tar.gz` & `tmp/cmem_plugin_pyshacl-4.2.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_pyshacl-4.2.0rc3.tar", max compression
+gzip compressed data, was "cmem_plugin_pyshacl-4.2.0rc4.tar", max compression
```

## Comparing `cmem_plugin_pyshacl-4.2.0rc3.tar` & `cmem_plugin_pyshacl-4.2.0rc4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11334 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/LICENSE
--rw-r--r--   0        0        0     4312 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/README-public.md
--rwxr-xr-x   0        0        0       46 2023-05-31 19:23:30.688567 cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/__init__.py
--rw-r--r--   0        0        0    26844 2023-05-31 19:23:02.012192 cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/plugin_pyshacl.py
--rw-r--r--   0        0        0     1875 2023-05-31 19:23:30.680567 cmem_plugin_pyshacl-4.2.0rc3/pyproject.toml
--rw-r--r--   0        0        0     5684 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.2.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-07-31 13:28:54.173660 cmem_plugin_pyshacl-4.2.0rc4/LICENSE
+-rw-r--r--   0        0        0     4312 2023-07-31 13:28:54.173660 cmem_plugin_pyshacl-4.2.0rc4/README-public.md
+-rwxr-xr-x   0        0        0       46 2023-07-31 13:29:20.498129 cmem_plugin_pyshacl-4.2.0rc4/cmem_plugin_pyshacl/__init__.py
+-rw-r--r--   0        0        0    26747 2023-07-31 13:28:54.177660 cmem_plugin_pyshacl-4.2.0rc4/cmem_plugin_pyshacl/plugin_pyshacl.py
+-rw-r--r--   0        0        0     1892 2023-07-31 13:29:20.494129 cmem_plugin_pyshacl-4.2.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     5717 1970-01-01 00:00:00.000000 cmem_plugin_pyshacl-4.2.0rc4/PKG-INFO
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc3/LICENSE` & `cmem_plugin_pyshacl-4.2.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.2.0rc3/README-public.md` & `cmem_plugin_pyshacl-4.2.0rc4/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_pyshacl-4.2.0rc3/cmem_plugin_pyshacl/plugin_pyshacl.py` & `cmem_plugin_pyshacl-4.2.0rc4/cmem_plugin_pyshacl/plugin_pyshacl.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,19 +363,15 @@
         focus_nodes = []
         validation_report_uri = validation_graph.value(
             predicate=RDF.type, object=SH.ValidationReport
         )
         conforms = validation_graph.value(
             subject=validation_report_uri, predicate=SH.conforms
         )
-        label = (
-            "SHACL validation report, conforms"
-            if conforms == "true"
-            else "SHACL validation report, nonconforms"
-        )
+        label = f"SHACL validation report, conforms={str(conforms)}"
         validation_graph.add((validation_report_uri, RDFS.label, Literal(label)))
         for validation_result_uri in validation_result_uris:
             message = str(
                 validation_graph.value(
                     subject=validation_result_uri, predicate=SH.resultMessage
                 )
             )
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc3/pyproject.toml` & `cmem_plugin_pyshacl-4.2.0rc4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-pyshacl"
-version = "4.2.0rc3"
+version = "4.2.0rc4"
 license = "Apache-2.0"
 description = "Validate your Knowledge Graphs based on tests generated from SHACL shapes."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules"
@@ -13,26 +13,27 @@
 keywords = [
     "eccenca Corporate Memory", "plugin", "SHACL"
 ]
 homepage = "https://github.com/eccenca/cmem-plugin-pyshacl"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-cmem-plugin-base = ">3.0.0,<4.0.0"
+cmem-plugin-base = ">=3.1.0,<5.0.0"
 pyshacl = "^0.22.2"
 validators = "^0.20.0"
 requests-toolbelt = "^0.10.1"
 rdflib = "^6.2.0"
 cmem-cmempy = "^23.1"
 types-setuptools = "^65.5.0.3"
 distutils-strtobool = "^0.1.0"
 ruamel-yaml = "^0.17.21"
 PyYAML = "^6.0"
 charset-normalizer = "^3.1.0"
 packaging = "^23.0"
+pillow = "9.5.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = "^23.3.0"
 coverage = "^7.2.3"
 defusedxml = "^0.7.1"
 flake8-formatter-junit-xml = "^0.0.6"
@@ -72,8 +73,7 @@
 
 [tool.mypy]
 warn_return_any = true
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = ""
-
```

### Comparing `cmem_plugin_pyshacl-4.2.0rc3/PKG-INFO` & `cmem_plugin_pyshacl-4.2.0rc4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-pyshacl
-Version: 4.2.0rc3
+Version: 4.2.0rc4
 Summary: Validate your Knowledge Graphs based on tests generated from SHACL shapes.
 Home-page: https://github.com/eccenca/cmem-plugin-pyshacl
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,SHACL
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -15,17 +15,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: cmem-cmempy (>=23.1,<24.0)
-Requires-Dist: cmem-plugin-base (>3.0.0,<4.0.0)
+Requires-Dist: cmem-plugin-base (>=3.1.0,<5.0.0)
 Requires-Dist: distutils-strtobool (>=0.1.0,<0.2.0)
 Requires-Dist: packaging (>=23.0,<24.0)
+Requires-Dist: pillow (==9.5.0)
 Requires-Dist: pyshacl (>=0.22.2,<0.23.0)
 Requires-Dist: rdflib (>=6.2.0,<7.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: types-setuptools (>=65.5.0.3,<66.0.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
```

