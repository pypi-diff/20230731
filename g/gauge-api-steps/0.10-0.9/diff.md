# Comparing `tmp/gauge-api-steps-0.10.tar.gz` & `tmp/gauge-api-steps-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauge-api-steps-0.10.tar", last modified: Mon Jul 31 15:53:04 2023, max compression
+gzip compressed data, was "gauge-api-steps-0.9.tar", last modified: Mon Jul 31 14:43:38 2023, max compression
```

## Comparing `gauge-api-steps-0.10.tar` & `gauge-api-steps-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 15:53:04.736470 gauge-api-steps-0.10/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1088 2023-07-24 11:28:58.000000 gauge-api-steps-0.10/LICENCE
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4136 2023-07-31 15:53:04.736327 gauge-api-steps-0.10/PKG-INFO
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3672 2023-07-31 15:15:49.000000 gauge-api-steps-0.10/README.md
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 15:53:04.735093 gauge-api-steps-0.10/gauge_api_steps/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 14:20:52.000000 gauge-api-steps-0.10/gauge_api_steps/__init__.py
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)    12713 2023-07-31 15:15:49.000000 gauge-api-steps-0.10/gauge_api_steps/api_steps.py
-drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 15:53:04.736132 gauge-api-steps-0.10/gauge_api_steps.egg-info/
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)     4136 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/PKG-INFO
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      330 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/SOURCES.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/dependency_links.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/not-zip-safe
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       48 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/requires.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       16 2023-07-31 15:53:04.000000 gauge-api-steps-0.10/gauge_api_steps.egg-info/top_level.txt
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       48 2023-07-31 15:15:49.000000 gauge-api-steps-0.10/pyproject.toml
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)       38 2023-07-31 15:53:04.736510 gauge-api-steps-0.10/setup.cfg
--rw-r--r--   0 tobias.lehmann   (502) staff       (20)      857 2023-07-31 15:19:01.000000 gauge-api-steps-0.10/setup.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 14:43:38.822471 gauge-api-steps-0.9/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     1088 2023-07-24 11:28:58.000000 gauge-api-steps-0.9/LICENCE
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3988 2023-07-31 14:43:38.822358 gauge-api-steps-0.9/PKG-INFO
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3672 2023-07-31 14:25:01.000000 gauge-api-steps-0.9/README.md
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 14:43:38.821459 gauge-api-steps-0.9/gauge_api_steps/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       63 2023-07-28 14:20:52.000000 gauge-api-steps-0.9/gauge_api_steps/__init__.py
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)    12713 2023-07-31 09:16:08.000000 gauge-api-steps-0.9/gauge_api_steps/api_steps.py
+drwxr-xr-x   0 tobias.lehmann   (502) staff       (20)        0 2023-07-31 14:43:38.822185 gauge-api-steps-0.9/gauge_api_steps.egg-info/
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)     3988 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/PKG-INFO
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      330 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)        1 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/not-zip-safe
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       48 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/requires.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       16 2023-07-31 14:43:38.000000 gauge-api-steps-0.9/gauge_api_steps.egg-info/top_level.txt
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       48 2023-07-31 08:52:06.000000 gauge-api-steps-0.9/pyproject.toml
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)       38 2023-07-31 14:43:38.822506 gauge-api-steps-0.9/setup.cfg
+-rw-r--r--   0 tobias.lehmann   (502) staff       (20)      737 2023-07-31 14:31:22.000000 gauge-api-steps-0.9/setup.py
```

### Comparing `gauge-api-steps-0.10/LICENCE` & `gauge-api-steps-0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `gauge-api-steps-0.10/PKG-INFO` & `gauge-api-steps-0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: gauge-api-steps
-Version: 0.10
-Summary: Provides steps for a Gauge project, that runs tests against APIs
-Home-page: https://github.com/IBM/gauge-api-steps
-Author: Tobias Lehmann
-Author-email: derdualist1@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # Gauge API Steps
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENCE)
 [![Python 3.10](https://img.shields.io/badge/Python-3.10-blue.svg?logo=python&logoColor=white)](https://www.python.org/downloads/release/python-31012/)
 [![Gauge](https://img.shields.io/badge/Framework-Gauge-blue)](https://github.com/getgauge)
 [![XPath](https://img.shields.io/badge/XPath-blue)](https://www.w3schools.com/xml/xpath_syntax.asp)
 [![JSONPath](https://img.shields.io/badge/JSONPath-blue)](https://github.com/h2non/jsonpath-ng)
@@ -23,15 +12,15 @@
 
 This is an extensible and flexible test-automation library for [Gauge](https://gauge.org). It enables users with and without programming knowledge to create end-to-end test scenarios in [Markdown](https://www.markdownguide.org/) syntax. Developers can still easily extend their test scenarios with custom code. Python's `urllib` is used to make requests against APIs. XML and JSON are supported and API responses can be validated with XPath and JSONPath.
 
 ## Gauge Step Overview
 
 Find the documentation on all Gauge steps of this project in the overview:
 
-[Gauge Step Overview](https://github.com/IBM/gauge-api-steps/tree/master/docs/STEPS.md)
+[Gauge Step Overview](./docs/STEPS.md)
 
 ## Quick Start
 
 This is a library for the Gauge framework, so Gauge+Python must be installed first.
 
 * Install Python >= 3.10 on your platform and make it available in the \$PATH
 * Install [Gauge](https://docs.gauge.org/getting_started/installing-gauge.html?language=python&ide=vscode) and [create a test projekt with Python](https://docs.gauge.org/getting_started/create-test-project.html?os=macos&language=python&ide=vscode)
@@ -64,15 +53,15 @@
 
 ```shell
 pip install gauge-api-steps --user --upgrade
 ```
 
 ## Development
 
-[Contributions are welcome](https://github.com/IBM/gauge-api-steps/tree/master/docs/CONTRIBUTING.md).
+[Contributions are welcome](./docs/CONTRIBUTING.md).
 
 ## Placeholders and Expressions
 
 Step parameters allow the use of placeholders, that can be defined in the environment properties files. Some steps also allow to set a placeholder value manually. Property keys act as placeholders, they are defined like "\${key}" and they will be replaced by its value if such a property key/value pair exists in any _env/\*/\*.properties_ file or within the execution scope.
 Some steps include parameters, that allow **expressions**, that will be evaluated.
 Examples of allowed expressions include: `=1` , `>1` , `<1` , `>=1` , `<=1`.
 
@@ -88,8 +77,8 @@
 * \_response
 * \_headers
 
 It is possible to access and manipulate them with certain steps.
 
 ## Maintainers
 
-[Maintainers](https://github.com/IBM/gauge-api-steps/tree/master/docs/MAINTAINERS.md)
+[Maintainers](./docs/MAINTAINERS.md)
```

### Comparing `gauge-api-steps-0.10/README.md` & `gauge-api-steps-0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: gauge-api-steps
+Version: 0.9
+Summary: Provides steps for a Gauge project, that runs tests against APIs
+Home-page: https://github.com/IBM/gauge-api-steps
+Author: Tobias Lehmann
+Author-email: derdualist1@gmail.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # Gauge API Steps
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENCE)
 [![Python 3.10](https://img.shields.io/badge/Python-3.10-blue.svg?logo=python&logoColor=white)](https://www.python.org/downloads/release/python-31012/)
 [![Gauge](https://img.shields.io/badge/Framework-Gauge-blue)](https://github.com/getgauge)
 [![XPath](https://img.shields.io/badge/XPath-blue)](https://www.w3schools.com/xml/xpath_syntax.asp)
 [![JSONPath](https://img.shields.io/badge/JSONPath-blue)](https://github.com/h2non/jsonpath-ng)
```

### Comparing `gauge-api-steps-0.10/gauge_api_steps/api_steps.py` & `gauge-api-steps-0.9/gauge_api_steps/api_steps.py`

 * *Files identical despite different names*

### Comparing `gauge-api-steps-0.10/gauge_api_steps.egg-info/PKG-INFO` & `gauge-api-steps-0.9/gauge_api_steps.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gauge-api-steps
-Version: 0.10
+Version: 0.9
 Summary: Provides steps for a Gauge project, that runs tests against APIs
 Home-page: https://github.com/IBM/gauge-api-steps
 Author: Tobias Lehmann
 Author-email: derdualist1@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENCE
@@ -23,15 +23,15 @@
 
 This is an extensible and flexible test-automation library for [Gauge](https://gauge.org). It enables users with and without programming knowledge to create end-to-end test scenarios in [Markdown](https://www.markdownguide.org/) syntax. Developers can still easily extend their test scenarios with custom code. Python's `urllib` is used to make requests against APIs. XML and JSON are supported and API responses can be validated with XPath and JSONPath.
 
 ## Gauge Step Overview
 
 Find the documentation on all Gauge steps of this project in the overview:
 
-[Gauge Step Overview](https://github.com/IBM/gauge-api-steps/tree/master/docs/STEPS.md)
+[Gauge Step Overview](./docs/STEPS.md)
 
 ## Quick Start
 
 This is a library for the Gauge framework, so Gauge+Python must be installed first.
 
 * Install Python >= 3.10 on your platform and make it available in the \$PATH
 * Install [Gauge](https://docs.gauge.org/getting_started/installing-gauge.html?language=python&ide=vscode) and [create a test projekt with Python](https://docs.gauge.org/getting_started/create-test-project.html?os=macos&language=python&ide=vscode)
@@ -64,15 +64,15 @@
 
 ```shell
 pip install gauge-api-steps --user --upgrade
 ```
 
 ## Development
 
-[Contributions are welcome](https://github.com/IBM/gauge-api-steps/tree/master/docs/CONTRIBUTING.md).
+[Contributions are welcome](./docs/CONTRIBUTING.md).
 
 ## Placeholders and Expressions
 
 Step parameters allow the use of placeholders, that can be defined in the environment properties files. Some steps also allow to set a placeholder value manually. Property keys act as placeholders, they are defined like "\${key}" and they will be replaced by its value if such a property key/value pair exists in any _env/\*/\*.properties_ file or within the execution scope.
 Some steps include parameters, that allow **expressions**, that will be evaluated.
 Examples of allowed expressions include: `=1` , `>1` , `<1` , `>=1` , `<=1`.
 
@@ -88,8 +88,8 @@
 * \_response
 * \_headers
 
 It is possible to access and manipulate them with certain steps.
 
 ## Maintainers
 
-[Maintainers](https://github.com/IBM/gauge-api-steps/tree/master/docs/MAINTAINERS.md)
+[Maintainers](./docs/MAINTAINERS.md)
```

### Comparing `gauge-api-steps-0.10/setup.py` & `gauge-api-steps-0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from os import path
 from setuptools import setup
 
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
-    long_description = long_description.replace('./docs/', 'https://github.com/IBM/gauge-api-steps/tree/master/docs/')
 
 setup(
     name='gauge-api-steps',
-    version='0.10',
+    version='0.9',
     description='Provides steps for a Gauge project, that runs tests against APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/IBM/gauge-api-steps',
     author='Tobias Lehmann',
     author_email='derdualist1@gmail.com',
     license='MIT',
```

