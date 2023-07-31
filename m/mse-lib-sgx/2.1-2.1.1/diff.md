# Comparing `tmp/mse_lib_sgx-2.1.tar.gz` & `tmp/mse-lib-sgx-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_lib_sgx-2.1.tar", last modified: Fri Jul 21 08:22:29 2023, max compression
+gzip compressed data, was "mse-lib-sgx-2.1.1.tar", last modified: Mon Jul 31 08:08:19 2023, max compression
```

## Comparing `mse_lib_sgx-2.1.tar` & `mse-lib-sgx-2.1.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.837664 mse_lib_sgx-2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/base64url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/quote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:22:29.000000 mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:22:29.841664 mse_lib_sgx-2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/tests/test_cert_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-21 08:21:43.000000 mse_lib_sgx-2.1/tests/test_conf_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.442604 mse-lib-sgx-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.442604 mse-lib-sgx-2.1.1/src/mse_lib_sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/base64url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/src/mse_lib_sgx/sgx/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/sgx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/sgx/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx/sgx/quote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 08:08:19.000000 mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 08:08:19.450604 mse-lib-sgx-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/tests/test_cert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-31 08:07:25.000000 mse-lib-sgx-2.1.1/tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.1/PKG-INFO` & `mse-lib-sgx-2.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
-Name: mse_lib_sgx
-Version: 2.1
-Summary: Library for Cosmian MSE to bootstrap Flask application
-Home-page: https://cosmian.com
-Author: Cosmian Tech
-Author-email: tech@cosmian.com
+Name: mse-lib-sgx
+Version: 2.1.1
+Summary: Library to bootstrap WSGI/ASGI application for Gramine
+Author-email: Cosmian Tech <tech@cosmian.com>
 License: MIT
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 6 - Mature
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: deploy
 
 # MicroService Encryption Lib SGX
 
 ## Overview
 
 MSE lib SGX bootstraps the execution of an encrypted ASGI/WSGI Python web application for [Gramine](https://gramine.readthedocs.io/).
 
 The library is responsible for:
 
 - Configuring the SSL certificates with either:
   - *RA-TLS*, a self-signed certificate including the Intel SGX quote in an X.509 v3 extension
   - *Custom*, the private key and full keychain is provided by the application owner
   - *No SSL*, the secure channel may be managed elsewhere by an SSL proxy
-- Decrypting Python modules encrypted with XSala20-Poly1305 AEAD
+- Decrypting Python modules encrypted with XSala20-Poly1305 AE
 - Running the ASGI/WSGI Python web application with [hypercorn](https://pgjones.gitlab.io/hypercorn/)
 
 ## Technical details
 
 The flow to run an encrypted Python web application is the following:
 
 1. A first self-signed HTTPS server using RA-TLS is launched waiting to receive a JSON payload with:
@@ -43,36 +47,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
-                     UUID [--version] [--debug]
-                     (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
+usage: mse-bootstrap [-h] [--host HOST] [--port PORT] [--subject SUBJECT] [--san SAN] --app-dir APP_DIR --id ID [--plaincode]
+                     [--timeout TIMEOUT] [--version] [--debug]
+                     (--ratls EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
   application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           hostname of the configuration server, also the
-                        hostname of the app server if `--self-signed`
+  --host HOST           hostname of the server
   --port PORT           port of the server
+  --subject SUBJECT     Subject as RFC 4514 string for the RA-TLS certificate
+  --san SAN             Subject Alternative Name in the RA-TLS certificate
   --app-dir APP_DIR     path of the python web application
-  --uuid UUID           unique application UUID
+  --id ID               identifier of the application as UUID in RFC 4122
+  --plaincode           unencrypted python web application
+  --timeout TIMEOUT     seconds before closing the configuration server
   --version             show program's version number and exit
   --debug               debug mode with more logging
-  --self-signed EXPIRATION_DATE
-                        generate a self-signed certificate for the web app
-                        with a specific expiration date (Unix time)
+  --ratls EXPIRATION_DATE
+                        generate a self-signed certificate for RA-TLS with a specific expiration date (Unix time)
   --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        custom certificate used for the SSL connection,
-                        private key must be sent through the configuration
-                        server
+                        custom certificate used for the SSL connection, private key must be sent through the configuration server
 
 ```
```

### Comparing `mse_lib_sgx-2.1/README.md` & `mse-lib-sgx-2.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 The library is responsible for:
 
 - Configuring the SSL certificates with either:
   - *RA-TLS*, a self-signed certificate including the Intel SGX quote in an X.509 v3 extension
   - *Custom*, the private key and full keychain is provided by the application owner
   - *No SSL*, the secure channel may be managed elsewhere by an SSL proxy
-- Decrypting Python modules encrypted with XSala20-Poly1305 AEAD
+- Decrypting Python modules encrypted with XSala20-Poly1305 AE
 - Running the ASGI/WSGI Python web application with [hypercorn](https://pgjones.gitlab.io/hypercorn/)
 
 ## Technical details
 
 The flow to run an encrypted Python web application is the following:
 
 1. A first self-signed HTTPS server using RA-TLS is launched waiting to receive a JSON payload with:
@@ -30,36 +30,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
-                     UUID [--version] [--debug]
-                     (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
+usage: mse-bootstrap [-h] [--host HOST] [--port PORT] [--subject SUBJECT] [--san SAN] --app-dir APP_DIR --id ID [--plaincode]
+                     [--timeout TIMEOUT] [--version] [--debug]
+                     (--ratls EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
   application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           hostname of the configuration server, also the
-                        hostname of the app server if `--self-signed`
+  --host HOST           hostname of the server
   --port PORT           port of the server
+  --subject SUBJECT     Subject as RFC 4514 string for the RA-TLS certificate
+  --san SAN             Subject Alternative Name in the RA-TLS certificate
   --app-dir APP_DIR     path of the python web application
-  --uuid UUID           unique application UUID
+  --id ID               identifier of the application as UUID in RFC 4122
+  --plaincode           unencrypted python web application
+  --timeout TIMEOUT     seconds before closing the configuration server
   --version             show program's version number and exit
   --debug               debug mode with more logging
-  --self-signed EXPIRATION_DATE
-                        generate a self-signed certificate for the web app
-                        with a specific expiration date (Unix time)
+  --ratls EXPIRATION_DATE
+                        generate a self-signed certificate for RA-TLS with a specific expiration date (Unix time)
   --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        custom certificate used for the SSL connection,
-                        private key must be sent through the configuration
-                        server
+                        custom certificate used for the SSL connection, private key must be sent through the configuration server
 
 ```
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx/cli.py` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,22 @@
 from mse_lib_sgx.copy import copytree
 from mse_lib_sgx.error import SecurityError
 from mse_lib_sgx.http_server import serve as serve_sgx_secrets
 from mse_lib_sgx.sgx.key import get_mrenclave_key
 
 
 def parse_args() -> argparse.Namespace:
-    """Argument parser."""
+    """Argument parser.
+
+    Returns
+    -------
+    argparse.Namespace
+        Namespace with parsed arguments.
+
+    """
     parser = argparse.ArgumentParser(
         description="Bootstrap ASGI/WSGI Python web application for Gramine"
     )
     parser.add_argument(
         "application",
         type=str,
         help="ASGI application path (as module:app)",
@@ -108,29 +115,27 @@
     NO_SSL = 3  # no SSL, will be done by the SSL proxy
 
 
 # pylint: disable=too-many-statements,too-many-branches
 def run() -> None:
     """Entrypoint of the CLI.
 
-    The program creates a self-signed certificate.
-
-    Then starts a configuration server using HTTPS and this previous cert
-    in order to allow the user to send some secrets params.
-
-    Once all the secrets has been sent, three options:
-    - (--self-signed) If the app owner relies on the enclave certificate,
+    Note
+    ----
+    Once all the secrets sent to the configuration server, three options:
+    - [--self-signed] If the app owner relies on the enclave certificate,
       then start the app server using this same certificate
-    - (--certificate) Start the app server using the certificate
+    - [--certificate] Start the app server using the certificate
       provided by the app owner. In that case, the certificate
       is already present in the workspace of the program
       but the private key is sent by the app owner
       when the configuration server is up.
-    - (--no-ssl) If the app owner and the users trust the operator (cosmian)
+    - [--no-ssl] If the app owner and the users trust the operator (cosmian)
       then don't use https connection.
+
     """
     args: argparse.Namespace = parse_args()
 
     globs.HOME_DIR_PATH.mkdir(exist_ok=True)
     globs.KEY_DIR_PATH.mkdir(exist_ok=True)
 
     logging.basicConfig(
@@ -192,18 +197,14 @@
         root_path=globs.KEY_DIR_PATH,
         expiration_date=expiration_date,
         ratls=enclave_pk,
     )
 
     if not globs.MODULE_DIR_PATH.exists():
         logging.info("Starting the configuration server...")
-        # The app owner will send:
-        # - the uuid of the app (see as an uniq token allowing to query the API)
-        # - the key to decrypt the code
-        # - (optional) the SSL private key if AppConnection.OWNER_CERTFICIATE
         serve_sgx_secrets(
             hostname=args.host,
             port=args.port,
             certificate=cert,
             app_id=args.id,
             need_ssl_private_key=ssl_app_mode == SslAppMode.CUSTOM_CERTIFICATE,
             timeout=globs.TIMEOUT,
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx/copy.py` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx/copy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,17 @@
-"""mse_lib_sgx.copy module."""
+"""mse_lib_sgx.copy module.
+
+Note
+----
+Code from `cpython/Lib/shutil.py`_ but with copystat() removed for Gramine.
+
+.. _cpython/Lib/shutil.py:
+    https://github.com/python/cpython/blob/3.8/Lib/shutil.py#L507
+
+"""
 
 import os
 import stat
 import sys
 from shutil import Error, copy, copy2
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx/globs.py` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx/globs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""mse_lib_sgx.global module."""
+"""mse_lib_sgx.globs module."""
 
 import os
 import threading
 from pathlib import Path
 from typing import Optional
 from uuid import UUID
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx/http_server.py` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx/http_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,29 @@
 from mse_lib_sgx import globs
 from mse_lib_sgx.base64url import base64url_decode
 from mse_lib_sgx.certificate import Certificate
 from mse_lib_sgx.error import CryptoError
 
 
 class SGXHTTPRequestHandler(BaseHTTPRequestHandler):
-    """SGX HTTP server to complete application config with secrets params."""
+    """HTTP server to configure the targeted WSGI/ASGI application.
+
+    Server is killed if it receives correcly the following elements
+    on POST method:
+        - uuid
+        - (optional) ssl_private_key
+        - (optional) app_secrets
+        - (optional) app_sealed_secrets
+        - (optional if plain code) code_secret_key
+
+    Note
+    ----
+    Contains only one endpoint '/' with GET and POST methods.
+
+    """
 
     def do_GET(self) -> None:
         """GET /."""
         msg: bytes = b"Waiting for code secret key and/or ssl private key..."
         self.send_response(200)
         self.send_header("Content-Length", str(len(msg)))
         # We send an extra header to easily know when the configuration server is up
@@ -32,20 +46,20 @@
 
     def do_POST(self) -> None:
         """POST /."""
         logging.info("Processing POST query...")
         content_length: int = int(self.headers.get("Content-Length", 0))
         body = self.rfile.read(content_length)
 
-        # body is a json withthese fields:
+        # body is a JSON with keys:
         # - uuid
         # - (optional) ssl_private_key
         # - (optional) app_secrets
         # - (optional) app_sealed_secrets
-        # - code_secret_key
+        # - (optional if plain code)  code_secret_key
         try:
             data = json.loads(body.decode("utf8"))
 
             if app_secrets := data.get("app_secrets"):
                 globs.SECRETS_PATH.parent.mkdir(parents=True, exist_ok=True)
                 globs.SECRETS_PATH.write_bytes(json.dumps(app_secrets).encode("utf-8"))
 
@@ -93,15 +107,41 @@
     hostname: str,
     port: int,
     certificate: Certificate,
     app_id: UUID,
     need_ssl_private_key: bool,
     timeout: Optional[int],
 ):
-    """Serve simple SGX HTTP server."""
+    """Serve SGXHTTPRequestHandler and run kill event in another thead.
+
+    Server is killed if it receives correctly:
+        - uuid
+        - (optional) ssl_private_key
+        - (optional) app_secrets
+        - (optional) app_sealed_secrets
+        - (optional if plain code) code_secret_key
+    or after `timeout`.
+
+    Parameters
+    ----------
+    hostname : str
+        Hostname of the server.
+    port : int
+        Port of the server.
+    certificate : Certificate
+        Certificate used for SSL.
+    app_id : UUID
+        Unique identifier of the server.
+    need_ssl_private_key : bool
+        Whether you provide a custom private key through
+        configuration server.
+    timeout : Optional[int]
+        Duration in ms before closing the HTTP server.
+
+    """
     globs.NEED_SSL_PRIVATE_KEY = need_ssl_private_key
     globs.ID = app_id
 
     httpd = HTTPServer((hostname, port), SGXHTTPRequestHandler)
 
     ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
     ctx.load_cert_chain(
@@ -119,24 +159,35 @@
     else:
         threading.Thread(target=kill_event, args=(httpd, None)).start()
 
     httpd.serve_forever()
 
 
 def kill_event(httpd: HTTPServer, timer: Optional[threading.Timer]):
-    """Kill HTTP server in a thread if `EXIT_EVENT` is set."""
+    """Event to kill `httpd`.
+
+    Loop exits if `globs.EXIT_EVENT` is set or timer thread finished.
+
+    Parameters
+    ----------
+    httpd : HTTPServer
+        Server to be killed.
+    timer : Optional[threading.Timer]
+        Timer thread to kill `httpd` if provided.
+
+    """
     while True:
         if globs.EXIT_EVENT.is_set():
             logging.info("Stopping the configuration server...")
 
             if timer:
                 timer.cancel()
 
             httpd.shutdown()
             return
 
         time.sleep(1)
 
 
 def kill():
-    """Kill HTTP server by setting `EXIT_EVENT`."""
+    """Set `globs.EXIT_EVENT` to kill HTTPServer with `kill_event`."""
     globs.EXIT_EVENT.set()
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx/sgx/quote.py` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx/sgx/quote.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,36 @@
 
 from mse_lib_sgx.error import SGXError
 
 SGX_QUOTE_MAX_SIZE: int = 8192
 
 
 def get_quote(user_report_data: bytes) -> bytes:
-    """Read the quote if inside Intel SGX enclave."""
+    """Request quote with `user_report_data` in REPORT_DATA field of SGX quote.
+
+    Parameters
+    ----------
+    user_report_data : bytes
+        Bytes to insert in REPORT_DATA field of SGX quote (max 64 bytes).
+
+    Returns
+    -------
+    bytes
+        Bytes of Intel SGX quote.
+
+    """
     if len(user_report_data) > 64:
         raise SGXError("user_report_data must be at most 64 bytes")
 
     attestation_type: str
     try:
         with open("/dev/attestation/attestation_type", "rb") as f:
             attestation_type = f.read(32).decode("utf-8").strip()
 
+        # only DCAP supported
         if attestation_type != "dcap":
             raise SGXError(f"Only DCAP supported, found '{attestation_type}'")
 
         with open("/dev/attestation/user_report_data", "wb") as f:
             f.write(user_report_data)
 
         with open("/dev/attestation/quote", "rb") as f:
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/PKG-INFO` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: mse-lib-sgx
-Version: 2.1
-Summary: Library for Cosmian MSE to bootstrap Flask application
-Home-page: https://cosmian.com
-Author: Cosmian Tech
-Author-email: tech@cosmian.com
+Version: 2.1.1
+Summary: Library to bootstrap WSGI/ASGI application for Gramine
+Author-email: Cosmian Tech <tech@cosmian.com>
 License: MIT
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 6 - Mature
+Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: deploy
 
 # MicroService Encryption Lib SGX
 
 ## Overview
 
 MSE lib SGX bootstraps the execution of an encrypted ASGI/WSGI Python web application for [Gramine](https://gramine.readthedocs.io/).
 
 The library is responsible for:
 
 - Configuring the SSL certificates with either:
   - *RA-TLS*, a self-signed certificate including the Intel SGX quote in an X.509 v3 extension
   - *Custom*, the private key and full keychain is provided by the application owner
   - *No SSL*, the secure channel may be managed elsewhere by an SSL proxy
-- Decrypting Python modules encrypted with XSala20-Poly1305 AEAD
+- Decrypting Python modules encrypted with XSala20-Poly1305 AE
 - Running the ASGI/WSGI Python web application with [hypercorn](https://pgjones.gitlab.io/hypercorn/)
 
 ## Technical details
 
 The flow to run an encrypted Python web application is the following:
 
 1. A first self-signed HTTPS server using RA-TLS is launched waiting to receive a JSON payload with:
@@ -43,36 +47,36 @@
 $ pip install mse-lib-sgx
 ```
 
 ## Usage
 
 ```console
 $ mse-bootstrap --help
-usage: mse-bootstrap [-h] --host HOST --port PORT --app-dir APP_DIR --uuid
-                     UUID [--version] [--debug]
-                     (--self-signed EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
+usage: mse-bootstrap [-h] [--host HOST] [--port PORT] [--subject SUBJECT] [--san SAN] --app-dir APP_DIR --id ID [--plaincode]
+                     [--timeout TIMEOUT] [--version] [--debug]
+                     (--ratls EXPIRATION_DATE | --no-ssl | --certificate CERTIFICATE_PATH)
                      application
 
 Bootstrap ASGI/WSGI Python web application for Gramine
 
 positional arguments:
   application           ASGI application path (as module:app)
 
 optional arguments:
   -h, --help            show this help message and exit
-  --host HOST           hostname of the configuration server, also the
-                        hostname of the app server if `--self-signed`
+  --host HOST           hostname of the server
   --port PORT           port of the server
+  --subject SUBJECT     Subject as RFC 4514 string for the RA-TLS certificate
+  --san SAN             Subject Alternative Name in the RA-TLS certificate
   --app-dir APP_DIR     path of the python web application
-  --uuid UUID           unique application UUID
+  --id ID               identifier of the application as UUID in RFC 4122
+  --plaincode           unencrypted python web application
+  --timeout TIMEOUT     seconds before closing the configuration server
   --version             show program's version number and exit
   --debug               debug mode with more logging
-  --self-signed EXPIRATION_DATE
-                        generate a self-signed certificate for the web app
-                        with a specific expiration date (Unix time)
+  --ratls EXPIRATION_DATE
+                        generate a self-signed certificate for RA-TLS with a specific expiration date (Unix time)
   --no-ssl              use HTTP without SSL
   --certificate CERTIFICATE_PATH
-                        custom certificate used for the SSL connection,
-                        private key must be sent through the configuration
-                        server
+                        custom certificate used for the SSL connection, private key must be sent through the configuration server
 
 ```
```

### Comparing `mse_lib_sgx-2.1/src/mse_lib_sgx.egg-info/SOURCES.txt` & `mse-lib-sgx-2.1.1/src/mse_lib_sgx.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 src/mse_lib_sgx/__init__.py
 src/mse_lib_sgx/base64url.py
 src/mse_lib_sgx/certificate.py
 src/mse_lib_sgx/cli.py
 src/mse_lib_sgx/copy.py
 src/mse_lib_sgx/error.py
 src/mse_lib_sgx/globs.py
 src/mse_lib_sgx/http_server.py
 src/mse_lib_sgx.egg-info/PKG-INFO
 src/mse_lib_sgx.egg-info/SOURCES.txt
 src/mse_lib_sgx.egg-info/dependency_links.txt
 src/mse_lib_sgx.egg-info/entry_points.txt
-src/mse_lib_sgx.egg-info/not-zip-safe
 src/mse_lib_sgx.egg-info/requires.txt
 src/mse_lib_sgx.egg-info/top_level.txt
 src/mse_lib_sgx/sgx/__init__.py
 src/mse_lib_sgx/sgx/key.py
 src/mse_lib_sgx/sgx/quote.py
 tests/test_cert_utils.py
 tests/test_conf_server.py
```

### Comparing `mse_lib_sgx-2.1/tests/test_cert_utils.py` & `mse-lib-sgx-2.1.1/tests/test_cert_utils.py`

 * *Files identical despite different names*

### Comparing `mse_lib_sgx-2.1/tests/test_conf_server.py` & `mse-lib-sgx-2.1.1/tests/test_conf_server.py`

 * *Files identical despite different names*

