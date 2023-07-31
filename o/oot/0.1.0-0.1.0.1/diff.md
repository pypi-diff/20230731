# Comparing `tmp/oot-0.1.0.tar.gz` & `tmp/oot-0.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oot-0.1.0.tar", max compression
+gzip compressed data, was "oot-0.1.0.1.tar", max compression
```

## Comparing `oot-0.1.0.tar` & `oot-0.1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-07-31 10:41:29.043929 oot-0.1.0/LICENSE
--rw-r--r--   0        0        0     2891 2023-07-31 10:41:29.043929 oot-0.1.0/README.md
--rw-r--r--   0        0        0       32 2023-07-31 10:41:29.043929 oot-0.1.0/oot/__init__.py
--rw-r--r--   0        0        0     2636 2023-07-31 10:41:29.043929 oot-0.1.0/oot/loaders.py
--rw-r--r--   0        0        0     1316 2023-07-31 10:41:29.043929 oot-0.1.0/oot/m_exceptions.py
--rw-r--r--   0        0        0     1423 2023-07-31 10:41:29.043929 oot-0.1.0/oot/main.py
--rw-r--r--   0        0        0     1225 2023-07-31 10:41:29.043929 oot-0.1.0/oot/parser.py
--rw-r--r--   0        0        0     1897 2023-07-31 10:41:29.043929 oot-0.1.0/oot/schema_validator.py
--rw-r--r--   0        0        0      584 2023-07-31 10:41:29.043929 oot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 oot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 10:53:47.602093 oot-0.1.0.1/LICENSE
+-rw-r--r--   0        0        0     3050 2023-07-31 10:53:47.602093 oot-0.1.0.1/README.md
+-rw-r--r--   0        0        0       32 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/__init__.py
+-rw-r--r--   0        0        0     2636 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/loaders.py
+-rw-r--r--   0        0        0     1316 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/m_exceptions.py
+-rw-r--r--   0        0        0     1423 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/main.py
+-rw-r--r--   0        0        0     1225 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/parser.py
+-rw-r--r--   0        0        0     1897 2023-07-31 10:53:47.602093 oot-0.1.0.1/oot/schema_validator.py
+-rw-r--r--   0        0        0      586 2023-07-31 10:53:47.602093 oot-0.1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 oot-0.1.0.1/PKG-INFO
```

### Comparing `oot-0.1.0/LICENSE` & `oot-0.1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/README.md` & `oot-0.1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Order of the Template (OOT)
 
-In the sacred halls of software development, the Order of the Template (OOT) stands as a bastion of structure and order amidst the chaos. The order, founded by the ancients, carries the mission of maintaining harmony between variables and templates, ensuring every template adheres to its rightful structure, and bringing light to the shadowy corners of Jinja and YAML.
+In the sacred halls of Dev, the Order of the Template (OOT) stands as a bastion of structure and order amidst the chaos. The order, founded by the ancients, carries the mission of maintaining harmony between variables and templates, ensuring every template adheres to its rightful structure, and bringing light to the shadowy corners of Jinja and YAML.
 
-The Order of the Template provides a noble toolkit for Python developers, aiding them in their quests to parse YAML files and Jinja templates, resolve environment variables, and validate JSON schemas.
+The Order of the Template provides a noble toolkit for Python developers, aiding them in their quests to parse YAML files and Jinja templates, resolve environment variables, and validate schemas.
 
 ## The Code of the Order
 ### A Noble Quest
 
 The Templars are trained not only in the ancient art of parsing Jinja templates but also in the mastery of environments, skillfully resolving environment variables. They are the keepers of schemas, using their wisdom to ensure that data structures adhere to their rightful schemas.
 
 Consider a quest where a Templar must decode an ancient manuscript, a YAML file filled with Jinja templates and environment variables:
 
 ```yaml
+# manuscript.yaml
 Templar: {{ TEMPLAR_NAME|default('Unknown Templar') }}
 HallOfHonor: ${HALL_OF_HONOR:"Hall of the Wicked"}
 ```
 The Templar starts his task. He replaces the `TEMPLAR_NAME` variable with the name of a famous Templar. He then resolves the `HALL_OF_HONOR` environment variable, revealing the name of the sacred hall. Once the manuscript has been decoded, he validates it, ensuring it adheres to the ancient schema:
 
 ```python
 from oot import parse_file
@@ -45,23 +46,22 @@
         "HallOfHonor": {"type": "string"}
     }
 }
 ```
 
 ## Joining the Order
 
-The Order welcomes all who seek order in their templates and harmony in their variables. To install the Order's toolkit, use pip:
+The Order welcomes all who seek order in their templates and harmony in their variables. To install the Order's toolkit, simple run:
 
 ```bash
 pip install oot
 ```
 
 May the Order guide you in your quests. 
 
 
-
 ## Closing Words
 
-Jinja2 is parse-able. There are some packages that help with env substitution in YAML/tpl files. 
-In my work I usually make use of both. So instead of creating the functions and tests for each project, I decided to just create a package that provides me this functionality.
-
-The name was my idea, the readme is ChatGPT's. I love it. 
+- OOT was born out of the re-occuring necessity to parse Jinja templates and resolve environment variables across multiple projects.
+- To separate concerns, enhance productivity and spare myself the need to setup code and tests within each project, I encapsulated the functionality.
+- OOT's primary objective is to painlessly handle the resolution of environmental variables and/or templating in your YAML files. 
+- I came up with the name and theme, the README is a glorious work of `ChatGPT`.
```

### Comparing `oot-0.1.0/oot/loaders.py` & `oot-0.1.0.1/oot/loaders.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/oot/m_exceptions.py` & `oot-0.1.0.1/oot/m_exceptions.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/oot/main.py` & `oot-0.1.0.1/oot/main.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/oot/parser.py` & `oot-0.1.0.1/oot/parser.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/oot/schema_validator.py` & `oot-0.1.0.1/oot/schema_validator.py`

 * *Files identical despite different names*

### Comparing `oot-0.1.0/pyproject.toml` & `oot-0.1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oot"
-version = "0.1.0"
+version = "0.1.0.1"
 description = "Order of the Template: A Python package for parsing Jinja templates and YAML files with environment variables."
 authors = ["Elsayed91 <elsayed.is@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `oot-0.1.0/PKG-INFO` & `oot-0.1.0.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oot
-Version: 0.1.0
+Version: 0.1.0.1
 Summary: Order of the Template: A Python package for parsing Jinja templates and YAML files with environment variables.
 License: MIT
 Author: Elsayed91
 Author-email: elsayed.is@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,26 +15,27 @@
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # Order of the Template (OOT)
 
-In the sacred halls of software development, the Order of the Template (OOT) stands as a bastion of structure and order amidst the chaos. The order, founded by the ancients, carries the mission of maintaining harmony between variables and templates, ensuring every template adheres to its rightful structure, and bringing light to the shadowy corners of Jinja and YAML.
+In the sacred halls of Dev, the Order of the Template (OOT) stands as a bastion of structure and order amidst the chaos. The order, founded by the ancients, carries the mission of maintaining harmony between variables and templates, ensuring every template adheres to its rightful structure, and bringing light to the shadowy corners of Jinja and YAML.
 
-The Order of the Template provides a noble toolkit for Python developers, aiding them in their quests to parse YAML files and Jinja templates, resolve environment variables, and validate JSON schemas.
+The Order of the Template provides a noble toolkit for Python developers, aiding them in their quests to parse YAML files and Jinja templates, resolve environment variables, and validate schemas.
 
 ## The Code of the Order
 ### A Noble Quest
 
 The Templars are trained not only in the ancient art of parsing Jinja templates but also in the mastery of environments, skillfully resolving environment variables. They are the keepers of schemas, using their wisdom to ensure that data structures adhere to their rightful schemas.
 
 Consider a quest where a Templar must decode an ancient manuscript, a YAML file filled with Jinja templates and environment variables:
 
 ```yaml
+# manuscript.yaml
 Templar: {{ TEMPLAR_NAME|default('Unknown Templar') }}
 HallOfHonor: ${HALL_OF_HONOR:"Hall of the Wicked"}
 ```
 The Templar starts his task. He replaces the `TEMPLAR_NAME` variable with the name of a famous Templar. He then resolves the `HALL_OF_HONOR` environment variable, revealing the name of the sacred hall. Once the manuscript has been decoded, he validates it, ensuring it adheres to the ancient schema:
 
 ```python
 from oot import parse_file
@@ -64,23 +65,22 @@
         "HallOfHonor": {"type": "string"}
     }
 }
 ```
 
 ## Joining the Order
 
-The Order welcomes all who seek order in their templates and harmony in their variables. To install the Order's toolkit, use pip:
+The Order welcomes all who seek order in their templates and harmony in their variables. To install the Order's toolkit, simple run:
 
 ```bash
 pip install oot
 ```
 
 May the Order guide you in your quests. 
 
 
-
 ## Closing Words
 
-Jinja2 is parse-able. There are some packages that help with env substitution in YAML/tpl files. 
-In my work I usually make use of both. So instead of creating the functions and tests for each project, I decided to just create a package that provides me this functionality.
-
-The name was my idea, the readme is ChatGPT's. I love it. 
+- OOT was born out of the re-occuring necessity to parse Jinja templates and resolve environment variables across multiple projects.
+- To separate concerns, enhance productivity and spare myself the need to setup code and tests within each project, I encapsulated the functionality.
+- OOT's primary objective is to painlessly handle the resolution of environmental variables and/or templating in your YAML files. 
+- I came up with the name and theme, the README is a glorious work of `ChatGPT`.
```

