# Comparing `tmp/digital_multimeter-0.5.2.tar.gz` & `tmp/digital_multimeter-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_multimeter-0.5.2.tar", max compression
+gzip compressed data, was "digital_multimeter-0.5.3.tar", max compression
```

## Comparing `digital_multimeter-0.5.2.tar` & `digital_multimeter-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1273 2023-05-07 01:44:56.429713 digital_multimeter-0.5.2/LICENSE
--rw-r--r--   0        0        0     3380 2023-05-07 13:37:32.685899 digital_multimeter-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2616 2023-05-08 01:31:13.891811 digital_multimeter-0.5.2/readme.md
--rw-r--r--   0        0        0      404 2023-05-07 13:37:32.690899 digital_multimeter-0.5.2/src/digital_multimeter/__init__.py
--rw-r--r--   0        0        0        0 2020-11-08 01:13:49.217434 digital_multimeter-0.5.2/src/digital_multimeter/cli/__init__.py
--rw-r--r--   0        0        0     3582 2023-05-07 01:44:56.510713 digital_multimeter-0.5.2/src/digital_multimeter/cli/click.py
--rw-r--r--   0        0        0     3462 2023-05-07 01:44:56.515714 digital_multimeter-0.5.2/src/digital_multimeter/cli/config.py
--rw-r--r--   0        0        0      442 2023-05-07 01:44:56.519713 digital_multimeter-0.5.2/src/digital_multimeter/cli/entrypoints.py
--rw-r--r--   0        0        0       47 2023-05-07 01:44:56.523714 digital_multimeter-0.5.2/src/digital_multimeter/exceptions.py
--rw-r--r--   0        0        0     2087 2023-05-07 01:44:56.527714 digital_multimeter-0.5.2/src/digital_multimeter/main.py
--rw-r--r--   0        0        0      245 2023-05-07 01:44:56.533714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterBase.py
--rw-r--r--   0        0        0     6727 2023-05-07 01:44:56.538714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterEDI9604.py
--rw-r--r--   0        0        0     8680 2023-05-07 01:44:56.544714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
--rw-r--r--   0        0        0    13947 2023-05-07 13:32:31.491604 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
--rw-r--r--   0        0        0     1076 2023-05-07 01:44:56.554714 digital_multimeter-0.5.2/src/digital_multimeter/multimeters/__init__.py
--rw-r--r--   0        0        0       35 2023-05-07 01:44:56.561714 digital_multimeter-0.5.2/src/digital_multimeter/utils/__init__.py
--rw-r--r--   0        0        0     2323 2023-05-07 01:44:56.566714 digital_multimeter-0.5.2/src/digital_multimeter/utils/cli_output.py
--rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 digital_multimeter-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1273 2023-05-07 01:44:56.429713 digital_multimeter-0.5.3/LICENSE
+-rw-r--r--   0        0        0     3304 2023-07-31 07:52:32.416110 digital_multimeter-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2616 2023-07-31 03:40:16.810950 digital_multimeter-0.5.3/readme.md
+-rw-r--r--   0        0        0      413 2023-07-31 07:52:32.424111 digital_multimeter-0.5.3/src/digital_multimeter/__init__.py
+-rw-r--r--   0        0        0        0 2020-11-08 01:13:49.217434 digital_multimeter-0.5.3/src/digital_multimeter/cli/__init__.py
+-rw-r--r--   0        0        0     3582 2023-05-07 01:44:56.510713 digital_multimeter-0.5.3/src/digital_multimeter/cli/click.py
+-rw-r--r--   0        0        0     3462 2023-05-07 01:44:56.515714 digital_multimeter-0.5.3/src/digital_multimeter/cli/config.py
+-rw-r--r--   0        0        0      442 2023-05-07 01:44:56.519713 digital_multimeter-0.5.3/src/digital_multimeter/cli/entrypoints.py
+-rw-r--r--   0        0        0       47 2023-05-07 01:44:56.523714 digital_multimeter-0.5.3/src/digital_multimeter/exceptions.py
+-rw-r--r--   0        0        0     2087 2023-05-07 01:44:56.527714 digital_multimeter-0.5.3/src/digital_multimeter/main.py
+-rw-r--r--   0        0        0      245 2023-05-07 01:44:56.533714 digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterBase.py
+-rw-r--r--   0        0        0     6727 2023-05-07 01:44:56.538714 digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterEDI9604.py
+-rw-r--r--   0        0        0     8680 2023-05-07 01:44:56.544714 digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py
+-rw-r--r--   0        0        0    13947 2023-05-07 13:32:31.491604 digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py
+-rw-r--r--   0        0        0     1076 2023-05-07 01:44:56.554714 digital_multimeter-0.5.3/src/digital_multimeter/multimeters/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-07 01:44:56.561714 digital_multimeter-0.5.3/src/digital_multimeter/utils/__init__.py
+-rw-r--r--   0        0        0     2323 2023-05-07 01:44:56.566714 digital_multimeter-0.5.3/src/digital_multimeter/utils/cli_output.py
+-rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 digital_multimeter-0.5.3/PKG-INFO
```

### Comparing `digital_multimeter-0.5.2/LICENSE` & `digital_multimeter-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/pyproject.toml` & `digital_multimeter-0.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,91 +1,83 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "digital-multimeter"
-version = "0.5.2"
+version = "0.5.3"
 description = "Digital Multimeter provides both a CLI interface and a Python API interface to receive data from a variety of digital multimeters."
 authors = ["Nicholas de Jong <contact@nicholasdejong.com>"]
 license = "BSD-2-Clause"
 readme = "readme.md"
 packages = [{ include = "digital_multimeter", from = "src" }]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License"
 ]
 keywords = ["multimeter", "digital multimeter", "dmm", "Digitech", "Digitek", "TekPower", "UniTrend", "Voltcraft"]
 
 [tool.poetry.urls]
 Documentation = "https://digital-multimeter.readthedocs.io/en/latest/"
 Homepage = "https://digital-multimeter.readthedocs.io/en/latest/"
 Repository = "https://github.com/ndejong/digital-multimeter.git"
 "Bug Tracker" = "https://github.com/ndejong/digital-multimeter/issues"
 
 [tool.poetry.scripts]
 dmm = "digital_multimeter.cli.entrypoints:dmm"
 
 [tool.poetry.dependencies]
-python = "^3.5"
+python = "^3.8"
 click = ">=7.0.0,<9.0.0"        # https://pypi.org/project/click/#history
 pyserial = ">=3.0.0,<4.0.0"     # https://pypi.org/project/pyserial/#history
 pyusb = ">=1.0.0,<2.0.0"        # https://pypi.org/project/pyusb/#history
 
 [tool.poetry.dev-dependencies]
-black = "^23.3"                 # https://pypi.org/project/black/#history
-flake8 = "^6.0"                 # https://pypi.org/project/flake8/#history
+black = "^23.7"                 # https://pypi.org/project/black/#history
+flake8 = "^6.1"                 # https://pypi.org/project/flake8/#history
 isort = "^5.12"                 # https://pypi.org/project/isort/#history
-pytest = "^7.3"                 # https://pypi.org/project/pytest/#history
-safety = "2.4.0b1"              # https://pypi.org/project/safety/#history
-mkdocs = "^1.4"                 # https://pypi.org/project/mkdocs/#history
-# NB: docs/requirements.txt needs to be kept up-to-date manually
+mypy = "^1.4"                   # https://pypi.org/project/mypy/#history
+pycln = "^2.1"                  # https://pypi.org/project/pycln/#history
+pytest = "^7.4"                 # https://pypi.org/project/pytest/#history
+safety = "^2.4.0b1"             # https://pypi.org/project/safety/#history
+mkdocs = "^1.5"                 # https://pypi.org/project/mkdocs/#history
+# NB: pip installs in .readthedocs.yml need to be kept up-to-date manually
 novella = "^0.2"                # https://pypi.org/project/novella/#history
-pydoc-markdown = "^4.6"         # https://pypi.org/project/pydoc-markdown/#history
+pydoc-markdown = "^4.8"         # https://pypi.org/project/pydoc-markdown/#history
 mkdocs-material = "^9.1"        # https://pypi.org/project/mkdocs-material/#history
 
 [tool.poetry.plugins."slap.plugins.check"]
 changelog = "slap.ext.checks.changelog:ChangelogValidationCheckPlugin"
 general = "slap.ext.checks.general:GeneralChecksPlugin"
 poetry = "slap.ext.checks.poetry:PoetryChecksPlugin"
 release = "slap.ext.checks.release:ReleaseChecksPlugin"
 
 [tool.slap]
 typed = false
 release.branch = "dev"
 
 [tool.slap.test]
-pytest = "pytest tests/ -vv"
 check = "slap check"
-isort = "isort src/ tests/ --check-only"
-black = "black src/ tests/ --check"
+black = "black --check src/ tests/"
 flake8 = "flake8 src/ tests/"
-safety = "pip freeze | safety check --stdin --output=text"
+isort = "isort --check-only src/ tests/"
+# mypy = "dmypy run src/"
+pycln  = "pycln src/ tests/ --check"
+safety = "pip freeze | safety check --stdin --short-report --output text"
+pytest = "pytest tests/ -vv"
 
 [tool.slap.run]
 format = "black src/ tests/ && isort src/ tests/"
 docs-build = "cd docs && novella --base-url digital-multimeter/"
 docs-server = "cd docs && novella --serve"
 
 [tool.isort]
 profile = "black"
 line_length = 120
 combine_as_imports = true
 
 [tool.black]
 line-length = 120
-
-[tool.readthedocs-custom-steps]
-script = """
-cd docs
-novella --base-url /en/latest/
-mkdir -p ../_readthedocs
-mv _site ../_readthedocs/html
-echo "COMMAND-PREVENTED: $@"
-"""
```

### Comparing `digital_multimeter-0.5.2/readme.md` & `digital_multimeter-0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/cli/click.py` & `digital_multimeter-0.5.3/src/digital_multimeter/cli/click.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/cli/config.py` & `digital_multimeter-0.5.3/src/digital_multimeter/cli/config.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/main.py` & `digital_multimeter-0.5.3/src/digital_multimeter/main.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterEDI9604.py` & `digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterEDI9604.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py` & `digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterFortuneFS9721.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py` & `digital_multimeter-0.5.3/src/digital_multimeter/multimeters/MultimeterVC870USBHID.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/multimeters/__init__.py` & `digital_multimeter-0.5.3/src/digital_multimeter/multimeters/__init__.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/src/digital_multimeter/utils/cli_output.py` & `digital_multimeter-0.5.3/src/digital_multimeter/utils/cli_output.py`

 * *Files identical despite different names*

### Comparing `digital_multimeter-0.5.2/PKG-INFO` & `digital_multimeter-0.5.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 Metadata-Version: 2.1
 Name: digital-multimeter
-Version: 0.5.2
+Version: 0.5.3
 Summary: Digital Multimeter provides both a CLI interface and a Python API interface to receive data from a variety of digital multimeters.
 License: BSD-2-Clause
 Keywords: multimeter,digital multimeter,dmm,Digitech,Digitek,TekPower,UniTrend,Voltcraft
 Author: Nicholas de Jong
 Author-email: contact@nicholasdejong.com
-Requires-Python: >=3.5,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=7.0.0,<9.0.0)
 Requires-Dist: pyserial (>=3.0.0,<4.0.0)
 Requires-Dist: pyusb (>=1.0.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/ndejong/digital-multimeter/issues
 Project-URL: Documentation, https://digital-multimeter.readthedocs.io/en/latest/
 Project-URL: Homepage, https://digital-multimeter.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/ndejong/digital-multimeter.git
```

