# Comparing `tmp/wf_postgres_client-0.1.1.tar.gz` & `tmp/wf_postgres_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_postgres_client-0.1.1.tar", max compression
+gzip compressed data, was "wf_postgres_client-0.1.2.tar", max compression
```

## Comparing `wf_postgres_client-0.1.1.tar` & `wf_postgres_client-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1088 2023-05-27 00:02:23.477415 wf_postgres_client-0.1.1/LICENSE
--rw-r--r--   0        0        0      533 2023-05-27 00:13:58.563639 wf_postgres_client-0.1.1/README.md
--rw-r--r--   0        0        0      576 2023-06-26 23:12:51.174886 wf_postgres_client-0.1.1/postgres_client/__init__.py
--rw-r--r--   0        0        0     3200 2023-06-26 19:15:33.404097 wf_postgres_client-0.1.1/postgres_client/core.py
--rw-r--r--   0        0        0     5672 2023-06-26 19:15:43.395910 wf_postgres_client-0.1.1/postgres_client/utils.py
--rw-r--r--   0        0        0     1048 2023-06-26 23:14:17.245124 wf_postgres_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.1/setup.py
--rw-r--r--   0        0        0     1580 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-05-27 00:02:23.477415 wf_postgres_client-0.1.2/LICENSE
+-rw-r--r--   0        0        0      533 2023-05-27 00:13:58.563639 wf_postgres_client-0.1.2/README.md
+-rw-r--r--   0        0        0      576 2023-06-26 23:12:51.174886 wf_postgres_client-0.1.2/postgres_client/__init__.py
+-rw-r--r--   0        0        0     3200 2023-06-26 19:15:33.404097 wf_postgres_client-0.1.2/postgres_client/core.py
+-rw-r--r--   0        0        0     5672 2023-06-26 19:15:43.395910 wf_postgres_client-0.1.2/postgres_client/utils.py
+-rw-r--r--   0        0        0     1050 2023-07-30 22:27:54.104815 wf_postgres_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.2/setup.py
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 wf_postgres_client-0.1.2/PKG-INFO
```

### Comparing `wf_postgres_client-0.1.1/LICENSE` & `wf_postgres_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.1/README.md` & `wf_postgres_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.1/postgres_client/__init__.py` & `wf_postgres_client-0.1.2/postgres_client/__init__.py`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.1/postgres_client/core.py` & `wf_postgres_client-0.1.2/postgres_client/core.py`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.1/postgres_client/utils.py` & `wf_postgres_client-0.1.2/postgres_client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_postgres_client-0.1.1/pyproject.toml` & `wf_postgres_client-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-postgres-client"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-postgres-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "A client for communicating with PostgreSQL databases"
 authors = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 readme = "README.md"
 keywords = []
 repository = "https://github.com/WildflowerSchools/wf-postgres-client"
 license = "MIT"
@@ -19,16 +19,16 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 toml = "^0.10.2"
-psycopg2 = "^2.9"
-pandas = "^1.5"
+psycopg2 = ">=2.9"
+pandas = ">=1.5"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 pylint = "^2.15.0"
 pytest = "^7.2.0"
 
 [tool.black]
```

### Comparing `wf_postgres_client-0.1.1/setup.py` & `wf_postgres_client-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['postgres_client']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['pandas>=1.5,<2.0', 'psycopg2>=2.9,<3.0', 'toml>=0.10.2,<0.11.0']
+['pandas>=1.5', 'psycopg2>=2.9', 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'wf-postgres-client',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A client for communicating with PostgreSQL databases',
     'long_description': '# postgres_client\n\nA client for communicating with PostgreSQL databases\n\n## Installation\n\n`pip install wf-postgres-client`\n\n## Development\n\n### Requirements\n\n* [Poetry](https://python-poetry.org/)\n* [just](https://github.com/casey/just)\n\n### Install\n\n`poetry install`\n\n\n#### Install w/ Python Version from PyEnv\n\n```\n# Specify pyenv python version\npyenv shell --unset\npyenv local <<VERSION>>\n\n# Set poetry python to pyenv version\npoetry env use $(pyenv which python)\npoetry cache clear . --all\npoetry install\n```\n\n## Task list\n* TBD\n',
     'author': 'Theodore Quinn',
     'author_email': 'ted.quinn@wildflowerschools.org',
     'maintainer': 'Theodore Quinn',
     'maintainer_email': 'ted.quinn@wildflowerschools.org',
     'url': 'https://github.com/WildflowerSchools/wf-postgres-client',
```

### Comparing `wf_postgres_client-0.1.1/PKG-INFO` & `wf_postgres_client-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-postgres-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A client for communicating with PostgreSQL databases
 Home-page: https://github.com/WildflowerSchools/wf-postgres-client
 License: MIT
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 Maintainer: Theodore Quinn
 Maintainer-email: ted.quinn@wildflowerschools.org
@@ -14,16 +14,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.5,<2.0)
-Requires-Dist: psycopg2 (>=2.9,<3.0)
+Requires-Dist: pandas (>=1.5)
+Requires-Dist: psycopg2 (>=2.9)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/WildflowerSchools/wf-postgres-client
 Description-Content-Type: text/markdown
 
 # postgres_client
 
 A client for communicating with PostgreSQL databases
```

