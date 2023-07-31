# Comparing `tmp/gridworks_cert-0.3.1.tar.gz` & `tmp/gridworks_cert-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_cert-0.3.1.tar", max compression
+gzip compressed data, was "gridworks_cert-0.3.2.tar", max compression
```

## Comparing `gridworks_cert-0.3.1.tar` & `gridworks_cert-0.3.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-29 12:19:16.884257 gridworks_cert-0.3.1/LICENSE
--rw-r--r--   0        0        0     3837 2023-07-29 12:19:16.884257 gridworks_cert-0.3.1/README.md
--rw-r--r--   0        0        0     2132 2023-07-29 12:19:37.828654 gridworks_cert-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      101 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/__init__.py
--rw-r--r--   0        0        0      455 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/__main__.py
--rw-r--r--   0        0        0       99 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/ca/__init__.py
--rw-r--r--   0        0        0     7416 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/ca/__main__.py
--rw-r--r--   0        0        0      172 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/key/__init__.py
--rw-r--r--   0        0        0    21478 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/key/__main__.py
--rw-r--r--   0        0        0      196 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/paths.py
--rw-r--r--   0        0        0        0 2023-07-29 12:19:16.888257 gridworks_cert-0.3.1/src/gwcert/py.typed
--rw-r--r--   0        0        0     4797 1970-01-01 00:00:00.000000 gridworks_cert-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 14:57:45.144558 gridworks_cert-0.3.2/LICENSE
+-rw-r--r--   0        0        0     4088 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/README.md
+-rw-r--r--   0        0        0     2164 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/__init__.py
+-rw-r--r--   0        0        0      658 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/src/gwcert/__main__.py
+-rw-r--r--   0        0        0       99 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/ca/__init__.py
+-rw-r--r--   0        0        0     7416 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/ca/__main__.py
+-rw-r--r--   0        0        0      172 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/key/__init__.py
+-rw-r--r--   0        0        0    21477 2023-07-31 14:58:05.818039 gridworks_cert-0.3.2/src/gwcert/key/__main__.py
+-rw-r--r--   0        0        0      196 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/paths.py
+-rw-r--r--   0        0        0        0 2023-07-31 14:57:45.148558 gridworks_cert-0.3.2/src/gwcert/py.typed
+-rw-r--r--   0        0        0     5087 1970-01-01 00:00:00.000000 gridworks_cert-0.3.2/PKG-INFO
```

### Comparing `gridworks_cert-0.3.1/LICENSE` & `gridworks_cert-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.1/README.md` & `gridworks_cert-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,51 +19,63 @@
 
 This library is a thin wrapper around [ownca], which wraps [pyca/cryptography], which wraps the [OpenSSL] C library.
 See also [tls-gen], a repo from [rabbitmq], which performs a similar task using a stack of make/python/OpenSSL CLI.
 
 ## Features
 
 - Create a local Certificate Authority directory with a self-signed certificate, via `gwcert ca create`.
-- Create named key pairs and sign them with the created CA with, via `gwcert ca add-key`.
+- Create named key pairs, CSRs and certificates with _arbitrary_ input and output paths, via `gwcert key add`.
+- Build cli commands visually with `gwcert tui`.
 
 ## Installation
 
-You can install _gwcert_ via [pip] from [PyPI]:
+The recommended way to install _gwcert_ is with [pipx] from [PyPI]:
 
 ```console
-$ pip install gridworks-cert
+$ pipx install gridworks-cert
 ```
 
 ## Usage
 
 Get help with any of:
 
 ```shell
 gwcert
 gwcert ca
-gwcert ca create --help
-gwcert ca add-key --help
+gwcert key
 ```
 
 Create a Certificate Authority directory with a self-signed certificate via:
 
 ```shell
 gwcert ca create
 ```
 
-Show information about the locally created ca with:
+Show information about the locally created ca and keys with:
 
 ```shell
 gwcert ca info
 ```
 
-Add a named set of keys (public, private, certificate) via:
+Add a named set of keys (public, private, certificate) via, for example:
 
 ```shell
-gwcert ca add-key
+gwcert key add KEY_NAME
+```
+
+Show information about a certificate:
+
+```shell
+gwcert key info KEY_NAME
+```
+
+Build CLI commands visually:
+
+```shell
+gwcert tui
 ```
 
 Please see the [Command-line Reference] for more details.
 
 ## Contributing
 
 Contributions are very welcome.
@@ -97,13 +109,14 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [tls-gen]: https://github.com/rabbitmq/tls-gen
 [ownca]: https://ownca.readthedocs.io/en/latest/
 [pyca/cryptography]: https://cryptography.io/en/latest/
 [openssl]: https://www.openssl.org/
 [rabbitmq]: https://rabbitmq.com/ssl.html#automated-certificate-generation-transcript
+[pipx]: https://pypa.github.io/pipx/
 
 <!-- github-only -->
 
 [license]: https://github.com/thegridelectric/gridworks-cert/blob/main/LICENSE
 [contributor guide]: https://github.com/thegridelectric/gridworks-cert/blob/main/CONTRIBUTING.md
 [command-line reference]: https://gridworks-cert.readthedocs.io/en/latest/usage.html
```

### Comparing `gridworks_cert-0.3.1/pyproject.toml` & `gridworks_cert-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-cert"
-version = "0.3.1"
+version = "0.3.2"
 description = "TLS certificate management tools for GridWorks"
 authors = ["Andrew Schweitzer <schweitz72@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-cert"
 repository = "https://github.com/thegridelectric/gridworks-cert"
 documentation = "https://gridworks-cert.readthedocs.io"
@@ -20,14 +20,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 ownca = ">=0.4.0"
 typer = ">=0.9.0"
 xdg = ">=6.0.0"
 rich = ">=12.0.0"
+trogon = "^0.5.0"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
@@ -80,13 +81,14 @@
 show_column_numbers = true
 show_error_codes = true
 show_error_context = false
 
 [[tool.mypy.overrides]]
 module = [
     "ownca.*",
+    "trogon",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gridworks_cert-0.3.1/src/gwcert/ca/__main__.py` & `gridworks_cert-0.3.2/src/gwcert/ca/__main__.py`

 * *Files identical despite different names*

### Comparing `gridworks_cert-0.3.1/src/gwcert/key/__main__.py` & `gridworks_cert-0.3.2/src/gwcert/key/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             help="""Overwrites existing certificate file.
         [yellow][bold]WARNING: [/yellow][/bold]--force will [red][bold]PERMANENTLY DELETE[/red][/bold]
         the certificate file for this name""",
         ),
     ] = False,
 ) -> None:
     """
-    Sign a CSR, producing a certificate .
+    Sign a CSR, producing a certificate.
 
     Uses input files, by default named:
 
         $HOME/.local/share/gridworks/ca/certs/name/name.csr
 
     Writes a certificate file, by default named:
```

### Comparing `gridworks_cert-0.3.1/PKG-INFO` & `gridworks_cert-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: gridworks-cert
-Version: 0.3.1
+Version: 0.3.2
 Summary: TLS certificate management tools for GridWorks
 Home-page: https://github.com/thegridelectric/gridworks-cert
 License: MIT
 Author: Andrew Schweitzer
 Author-email: schweitz72@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ownca (>=0.4.0)
 Requires-Dist: rich (>=12.0.0)
+Requires-Dist: trogon (>=0.5.0,<0.6.0)
 Requires-Dist: typer (>=0.9.0)
 Requires-Dist: xdg (>=6.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-cert/releases
 Project-URL: Documentation, https://gridworks-cert.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-cert
 Description-Content-Type: text/markdown
 
@@ -43,51 +44,63 @@
 
 This library is a thin wrapper around [ownca], which wraps [pyca/cryptography], which wraps the [OpenSSL] C library.
 See also [tls-gen], a repo from [rabbitmq], which performs a similar task using a stack of make/python/OpenSSL CLI.
 
 ## Features
 
 - Create a local Certificate Authority directory with a self-signed certificate, via `gwcert ca create`.
-- Create named key pairs and sign them with the created CA with, via `gwcert ca add-key`.
+- Create named key pairs, CSRs and certificates with _arbitrary_ input and output paths, via `gwcert key add`.
+- Build cli commands visually with `gwcert tui`.
 
 ## Installation
 
-You can install _gwcert_ via [pip] from [PyPI]:
+The recommended way to install _gwcert_ is with [pipx] from [PyPI]:
 
 ```console
-$ pip install gridworks-cert
+$ pipx install gridworks-cert
 ```
 
 ## Usage
 
 Get help with any of:
 
 ```shell
 gwcert
 gwcert ca
-gwcert ca create --help
-gwcert ca add-key --help
+gwcert key
 ```
 
 Create a Certificate Authority directory with a self-signed certificate via:
 
 ```shell
 gwcert ca create
 ```
 
-Show information about the locally created ca with:
+Show information about the locally created ca and keys with:
 
 ```shell
 gwcert ca info
 ```
 
-Add a named set of keys (public, private, certificate) via:
+Add a named set of keys (public, private, certificate) via, for example:
 
 ```shell
-gwcert ca add-key
+gwcert key add KEY_NAME
+```
+
+Show information about a certificate:
+
+```shell
+gwcert key info KEY_NAME
+```
+
+Build CLI commands visually:
+
+```shell
+gwcert tui
 ```
 
 Please see the [Command-line Reference] for more details.
 
 ## Contributing
 
 Contributions are very welcome.
@@ -121,14 +134,15 @@
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 [tls-gen]: https://github.com/rabbitmq/tls-gen
 [ownca]: https://ownca.readthedocs.io/en/latest/
 [pyca/cryptography]: https://cryptography.io/en/latest/
 [openssl]: https://www.openssl.org/
 [rabbitmq]: https://rabbitmq.com/ssl.html#automated-certificate-generation-transcript
+[pipx]: https://pypa.github.io/pipx/
 
 <!-- github-only -->
 
 [license]: https://github.com/thegridelectric/gridworks-cert/blob/main/LICENSE
 [contributor guide]: https://github.com/thegridelectric/gridworks-cert/blob/main/CONTRIBUTING.md
 [command-line reference]: https://gridworks-cert.readthedocs.io/en/latest/usage.html
```

