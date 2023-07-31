# Comparing `tmp/jupylint-2.2.2.tar.gz` & `tmp/jupylint-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupylint-2.2.2.tar", last modified: Fri Nov 19 01:46:51 2021, max compression
+gzip compressed data, was "jupylint-2.2.3.tar", last modified: Mon Jul 31 17:45:58 2023, max compression
```

## Comparing `jupylint-2.2.2.tar` & `jupylint-2.2.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2021-11-19 01:46:51.555284 jupylint-2.2.2/
--rw-r--r--   0 edjg      (1000) edjg      (1000)     2258 2021-11-19 01:46:51.556285 jupylint-2.2.2/PKG-INFO
--rw-r--r--   0 edjg      (1000) edjg      (1000)     1135 2021-10-30 18:22:43.000000 jupylint-2.2.2/README.md
-drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2021-11-19 01:46:51.462734 jupylint-2.2.2/jupylint/
--rw-r--r--   0 edjg      (1000) edjg      (1000)      109 2021-10-30 13:57:40.000000 jupylint-2.2.2/jupylint/__init__.py
--rw-r--r--   0 edjg      (1000) edjg      (1000)       89 2021-10-30 13:57:40.000000 jupylint-2.2.2/jupylint/__main__.py
--rw-r--r--   0 edjg      (1000) edjg      (1000)     6688 2021-11-19 01:14:56.000000 jupylint-2.2.2/jupylint/_test.py
--rw-r--r--   0 edjg      (1000) edjg      (1000)     2381 2021-11-19 01:15:11.000000 jupylint-2.2.2/jupylint/_test_template.py
--rwxr-xr-x   0 edjg      (1000) edjg      (1000)     5050 2021-11-19 01:44:39.000000 jupylint-2.2.2/jupylint/jupylint.py
-drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2021-11-19 01:46:51.543695 jupylint-2.2.2/jupylint.egg-info/
--rw-r--r--   0 edjg      (1000) edjg      (1000)     2258 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/PKG-INFO
--rw-r--r--   0 edjg      (1000) edjg      (1000)      330 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/SOURCES.txt
--rw-r--r--   0 edjg      (1000) edjg      (1000)        1 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/dependency_links.txt
--rw-r--r--   0 edjg      (1000) edjg      (1000)       53 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/entry_points.txt
--rw-r--r--   0 edjg      (1000) edjg      (1000)        7 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/requires.txt
--rw-r--r--   0 edjg      (1000) edjg      (1000)        9 2021-11-19 01:46:51.000000 jupylint-2.2.2/jupylint.egg-info/top_level.txt
--rw-r--r--   0 edjg      (1000) edjg      (1000)       79 2021-11-19 01:46:51.560905 jupylint-2.2.2/setup.cfg
--rw-r--r--   0 edjg      (1000) edjg      (1000)     1248 2021-11-19 01:44:30.000000 jupylint-2.2.2/setup.py
+drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2023-07-31 17:45:58.160567 jupylint-2.2.3/
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     1071 2023-07-31 17:25:53.000000 jupylint-2.2.3/LICENSE
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     2148 2023-07-31 17:45:58.160567 jupylint-2.2.3/PKG-INFO
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     1323 2023-07-31 17:34:57.000000 jupylint-2.2.3/README.md
+drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2023-07-31 17:45:58.160567 jupylint-2.2.3/jupylint/
+-rw-r--r--   0 edjg      (1000) edjg      (1000)      109 2023-07-31 17:25:53.000000 jupylint-2.2.3/jupylint/__init__.py
+-rw-r--r--   0 edjg      (1000) edjg      (1000)       89 2023-07-31 17:25:53.000000 jupylint-2.2.3/jupylint/__main__.py
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     6688 2023-07-31 17:25:53.000000 jupylint-2.2.3/jupylint/_test.py
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     2381 2023-07-31 17:25:53.000000 jupylint-2.2.3/jupylint/_test_template.py
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)     5341 2023-07-31 17:34:27.000000 jupylint-2.2.3/jupylint/jupylint.py
+drwxr-xr-x   0 edjg      (1000) edjg      (1000)        0 2023-07-31 17:45:58.160567 jupylint-2.2.3/jupylint.egg-info/
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)     2148 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/PKG-INFO
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)      338 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/SOURCES.txt
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)        1 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/dependency_links.txt
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)       52 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/entry_points.txt
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)        7 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/requires.txt
+-rwxr-xr-x   0 edjg      (1000) edjg      (1000)        9 2023-07-31 17:45:58.000000 jupylint-2.2.3/jupylint.egg-info/top_level.txt
+-rw-r--r--   0 edjg      (1000) edjg      (1000)       79 2023-07-31 17:45:58.163901 jupylint-2.2.3/setup.cfg
+-rw-r--r--   0 edjg      (1000) edjg      (1000)     1203 2023-07-31 17:28:57.000000 jupylint-2.2.3/setup.py
```

### Comparing `jupylint-2.2.2/PKG-INFO` & `jupylint-2.2.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: jupylint
-Version: 2.2.2
+Version: 2.2.3
 Summary: A tool to run pylint on Jupyter notebooks
 Home-page: https://github.com/EdmundGoodman/Jupyter_Pylinter
+Download-URL: https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.3.tar.gz
 Author: Edmund Goodman
 Author-email: egoodman3141@gmail.com
 License: MIT
-Download-URL: https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.2.tar.gz
-Description: ![Build status](https://github.com/EdmundGoodman/Jupyter_Pylinter/actions/workflows/python-app.yml/badge.svg)
-        [![Code coverage](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter/branch/main/graph/badge.svg?token=5XL3ZX71OJ)](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter)
-        
-        # Jupyter Pylinter
-        
-        A simple tool to extract python code from a Jupyter notebook, and then run
-        pylint on it for static analysis.
-        
-        If you find this tool useful, please give it a star on GitHub!
-        
-        # Usage
-        
-        The package can be installed via PyPI, then run from the command line, as
-        follows:
-        
-        ```bash
-        pip install jupylint
-        jupylint <input file name>
-        ```
-        
-        Full documentation is available:
-        
-        - [On readthedocs](https://jupylint.readthedocs.io/en/latest/)
-        
-        # Download
-        
-        The tool can be downloaded in the following places:
-        
-        - [As a standalone python file](https://raw.githubusercontent.com/EdmundGoodman/Jupyter_Pylinter/main/jupylint/jupylint.py)
-        - [As a package on PyPI](https://pypi.org/project/jupylint/)
-        
-        ## Contributions and errata
-        
-        If you find a bug in the code, feel free to submit a pull request or an issue
-        through GitHub, and I will endeavour to fix it!
-        
 Keywords: Jupyter,Pylint,linter
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Build status](https://github.com/EdmundGoodman/Jupyter_Pylinter/actions/workflows/python-app.yml/badge.svg)
+[![Code coverage](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter/branch/main/graph/badge.svg?token=5XL3ZX71OJ)](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter)
+
+# Jupyter Pylinter - Archived
+
+***This project is archived, and no longer under active development.***
+
+**Please consider using [https://github.com/nbQA-dev/nbQA](https://github.com/nbQA-dev/nbQA) instead**
+
+A simple tool to extract python code from a Jupyter notebook, and then run
+pylint on it for static analysis.
+
+If you find this tool useful, please give it a star on GitHub!
+
+# Usage
+
+The package can be installed via PyPI, then run from the command line, as
+follows:
+
+```bash
+pip install jupylint
+jupylint <input file name>
+```
+
+Full documentation is available:
+
+- [On readthedocs](https://jupylint.readthedocs.io/en/latest/)
+
+# Download
+
+The tool can be downloaded in the following places:
+
+- [As a standalone python file](https://raw.githubusercontent.com/EdmundGoodman/Jupyter_Pylinter/main/jupylint/jupylint.py)
+- [As a package on PyPI](https://pypi.org/project/jupylint/)
+
+## Contributions and errata
+
+If you find a bug in the code, feel free to submit a pull request or an issue
+through GitHub, and I will endeavour to fix it!
```

### Comparing `jupylint-2.2.2/README.md` & `jupylint-2.2.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 ![Build status](https://github.com/EdmundGoodman/Jupyter_Pylinter/actions/workflows/python-app.yml/badge.svg)
 [![Code coverage](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter/branch/main/graph/badge.svg?token=5XL3ZX71OJ)](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter)
 
-# Jupyter Pylinter
+# Jupyter Pylinter - Archived
+
+***This project is archived, and no longer under active development.***
+
+**Please consider using [https://github.com/nbQA-dev/nbQA](https://github.com/nbQA-dev/nbQA) instead**
 
 A simple tool to extract python code from a Jupyter notebook, and then run
 pylint on it for static analysis.
 
 If you find this tool useful, please give it a star on GitHub!
 
 # Usage
```

### Comparing `jupylint-2.2.2/jupylint/_test.py` & `jupylint-2.2.3/jupylint/_test.py`

 * *Files identical despite different names*

### Comparing `jupylint-2.2.2/jupylint/_test_template.py` & `jupylint-2.2.3/jupylint/_test_template.py`

 * *Files identical despite different names*

### Comparing `jupylint-2.2.2/jupylint/jupylint.py` & `jupylint-2.2.3/jupylint/jupylint.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,57 +10,83 @@
 from os import remove, path
 
 
 __author__ = "Edmund Goodman"
 __copyright__ = "Copyright 2021"
 __credits__ = ["Edmund Goodman"]
 __license__ = "MIT"
-__version__ = "2.2.2"
+__version__ = "2.2.3"
 __maintainer__ = "Edmund Goodman"
 __email__ = "egoodman3141@gmail.com"
 __status__ = "Production"
 
 
 class OldJupyterVersionError(Exception):
     """A custom exception for when the Jupyter version is too old"""
 
 
 class Jupylint:
     """The tool to extract from Jupyter notebooks and run pylint"""
+
     CELL_SEPARATOR = "# " + ("=" * 78) + "\n"
     DEFAULT_OUT_FILE = ".jupylint_tmp_out.py"
 
     @staticmethod
     def get_arguments():
         """Parse keyword arguments for the tool"""
-        parser = ArgumentParser(description="""A simple tool to extract
+        parser = ArgumentParser(
+            description="""A simple tool to extract
         python code from a Jupyter notebook, and then run pylint on it for static
-        analysis.""")
-        parser.add_argument("in_file_name", metavar="input_file_name", type=str,
-            nargs=1, help="the name of the Jupyter notebook file to extract the code from")
-        parser.add_argument("out_file_name", metavar="output_file_name", type=str,
-            nargs="?", default=Jupylint.DEFAULT_OUT_FILE,
-            help="the name of the output file to write the extracted code to")
-        parser.add_argument("-k", "--keep", dest="save_file", action="store_true",
-            help="a boolean specifying whether to keep or delete the extracted python file")
-        parser.add_argument("--rcfile", metavar="rcfile", type=str,
-            nargs=1, help="the pylintrc file to use")
-        parser.add_argument("-v", "--version", action="version",
-            version=f"%(prog)s {__version__}")
+        analysis."""
+        )
+        parser.add_argument(
+            "in_file_name",
+            metavar="input_file_name",
+            type=str,
+            nargs=1,
+            help="the name of the Jupyter notebook file to extract the code from",
+        )
+        parser.add_argument(
+            "out_file_name",
+            metavar="output_file_name",
+            type=str,
+            nargs="?",
+            default=Jupylint.DEFAULT_OUT_FILE,
+            help="the name of the output file to write the extracted code to",
+        )
+        parser.add_argument(
+            "-k",
+            "--keep",
+            dest="save_file",
+            action="store_true",
+            help="a boolean specifying whether to keep or delete the extracted python file",
+        )
+        parser.add_argument(
+            "--rcfile",
+            metavar="rcfile",
+            type=str,
+            nargs=1,
+            help="the pylintrc file to use",
+        )
+        parser.add_argument(
+            "-v", "--version", action="version", version=f"%(prog)s {__version__}"
+        )
         return parser.parse_args()
 
     @staticmethod
     def get_json_content(in_file_name):
         """Extract the json contents from the Jupyter file"""
         json_content = ""
         with open(in_file_name, "r", encoding="utf-8") as in_file:
             json_content = load(in_file)
         if json_content["nbformat"] >= 4:
             return json_content["cells"]
-        raise OldJupyterVersionError(f"The Jupyter version of '{in_file_name}' is too old (<=4.0)")
+        raise OldJupyterVersionError(
+            f"The Jupyter version of '{in_file_name}' is too old (<=4.0)"
+        )
 
     @staticmethod
     def get_code_content(json_content):
         """Extract the code blocks from the json"""
         code_content = ""
         for cell in json_content:
             if cell["cell_type"] == "code":
```

### Comparing `jupylint-2.2.2/jupylint.egg-info/PKG-INFO` & `jupylint-2.2.3/jupylint.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: jupylint
-Version: 2.2.2
+Version: 2.2.3
 Summary: A tool to run pylint on Jupyter notebooks
 Home-page: https://github.com/EdmundGoodman/Jupyter_Pylinter
+Download-URL: https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.3.tar.gz
 Author: Edmund Goodman
 Author-email: egoodman3141@gmail.com
 License: MIT
-Download-URL: https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.2.tar.gz
-Description: ![Build status](https://github.com/EdmundGoodman/Jupyter_Pylinter/actions/workflows/python-app.yml/badge.svg)
-        [![Code coverage](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter/branch/main/graph/badge.svg?token=5XL3ZX71OJ)](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter)
-        
-        # Jupyter Pylinter
-        
-        A simple tool to extract python code from a Jupyter notebook, and then run
-        pylint on it for static analysis.
-        
-        If you find this tool useful, please give it a star on GitHub!
-        
-        # Usage
-        
-        The package can be installed via PyPI, then run from the command line, as
-        follows:
-        
-        ```bash
-        pip install jupylint
-        jupylint <input file name>
-        ```
-        
-        Full documentation is available:
-        
-        - [On readthedocs](https://jupylint.readthedocs.io/en/latest/)
-        
-        # Download
-        
-        The tool can be downloaded in the following places:
-        
-        - [As a standalone python file](https://raw.githubusercontent.com/EdmundGoodman/Jupyter_Pylinter/main/jupylint/jupylint.py)
-        - [As a package on PyPI](https://pypi.org/project/jupylint/)
-        
-        ## Contributions and errata
-        
-        If you find a bug in the code, feel free to submit a pull request or an issue
-        through GitHub, and I will endeavour to fix it!
-        
 Keywords: Jupyter,Pylint,linter
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 7 - Inactive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![Build status](https://github.com/EdmundGoodman/Jupyter_Pylinter/actions/workflows/python-app.yml/badge.svg)
+[![Code coverage](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter/branch/main/graph/badge.svg?token=5XL3ZX71OJ)](https://codecov.io/gh/EdmundGoodman/Jupyter_Pylinter)
+
+# Jupyter Pylinter - Archived
+
+***This project is archived, and no longer under active development.***
+
+**Please consider using [https://github.com/nbQA-dev/nbQA](https://github.com/nbQA-dev/nbQA) instead**
+
+A simple tool to extract python code from a Jupyter notebook, and then run
+pylint on it for static analysis.
+
+If you find this tool useful, please give it a star on GitHub!
+
+# Usage
+
+The package can be installed via PyPI, then run from the command line, as
+follows:
+
+```bash
+pip install jupylint
+jupylint <input file name>
+```
+
+Full documentation is available:
+
+- [On readthedocs](https://jupylint.readthedocs.io/en/latest/)
+
+# Download
+
+The tool can be downloaded in the following places:
+
+- [As a standalone python file](https://raw.githubusercontent.com/EdmundGoodman/Jupyter_Pylinter/main/jupylint/jupylint.py)
+- [As a package on PyPI](https://pypi.org/project/jupylint/)
+
+## Contributions and errata
+
+If you find a bug in the code, feel free to submit a pull request or an issue
+through GitHub, and I will endeavour to fix it!
```

### Comparing `jupylint-2.2.2/setup.py` & `jupylint-2.2.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from setuptools import setup, find_packages
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
-    name = 'jupylint',
-    version = '2.2.2',
-    license='MIT',
-    description = 'A tool to run pylint on Jupyter notebooks',
+    name="jupylint",
+    version="2.2.3",
+    license="MIT",
+    description="A tool to run pylint on Jupyter notebooks",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author = 'Edmund Goodman',
-    author_email = 'egoodman3141@gmail.com',
-    url = 'https://github.com/EdmundGoodman/Jupyter_Pylinter',
-    download_url = 'https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.2.tar.gz',
+    author="Edmund Goodman",
+    author_email="egoodman3141@gmail.com",
+    url="https://github.com/EdmundGoodman/Jupyter_Pylinter",
+    download_url="https://github.com/EdmundGoodman/Jupyter_Pylinter/archive/refs/tags/v2.2.3.tar.gz",
     packages=find_packages(),
-    entry_points = {
-        "console_scripts": ['jupylint = jupylint.jupylint:main']
-    },
-    keywords = ['Jupyter', 'Pylint', 'linter'],
-    install_requires = ['pylint'],
+    entry_points={"console_scripts": ["jupylint = jupylint.jupylint:main"]},
+    keywords=["Jupyter", "Pylint", "linter"],
+    install_requires=["pylint"],
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development :: Build Tools',
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        "Development Status :: 7 - Inactive",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Build Tools",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
     ],
 )
```

