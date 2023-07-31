# Comparing `tmp/adafruit-circuitpython-httpserver-4.1.0.tar.gz` & `tmp/adafruit-circuitpython-httpserver-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-httpserver-4.1.0.tar", last modified: Mon Jul 17 15:39:17 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-httpserver-4.2.0.tar", last modified: Mon Jul 31 16:49:44 2023, max compression
```

## Comparing `adafruit-circuitpython-httpserver-4.1.0.tar` & `adafruit-circuitpython-httpserver-4.2.0.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.877951 adafruit-circuitpython-httpserver-4.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.877951 adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-17 15:39:17.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.881950 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/mime_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10253 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.885950 adafruit-circuitpython-httpserver-4.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.885950 adafruit-circuitpython-httpserver-4.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13817 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/examples/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_chunked.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_cpu_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_ethernet_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_form_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_handler_serves_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_multiple_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_auto.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_start_and_poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_static_files_serving.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_url_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/examples/settings.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-17 15:39:08.000000 adafruit-circuitpython-httpserver-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 15:38:55.000000 adafruit-circuitpython-httpserver-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:39:17.893951 adafruit-circuitpython-httpserver-4.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.814973 adafruit-circuitpython-httpserver-4.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.778974 adafruit-circuitpython-httpserver-4.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.786974 adafruit-circuitpython-httpserver-4.2.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.790974 adafruit-circuitpython-httpserver-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.790974 adafruit-circuitpython-httpserver-4.2.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-31 16:49:44.814973 adafruit-circuitpython-httpserver-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.794973 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-31 16:49:44.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-31 16:49:44.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 16:49:44.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-31 16:49:44.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-31 16:49:44.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.798973 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/mime_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10331 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25745 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.802974 adafruit-circuitpython-httpserver-4.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.802974 adafruit-circuitpython-httpserver-4.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 16:49:44.814973 adafruit-circuitpython-httpserver-4.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/examples/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_authentication_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_authentication_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_cpu_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_ethernet_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_form_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_handler_serves_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_multiple_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_simpletest_auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_simpletest_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_start_and_poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_static_files_serving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_url_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/examples/settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-31 16:49:33.000000 adafruit-circuitpython-httpserver-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-31 16:49:10.000000 adafruit-circuitpython-httpserver-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 16:49:44.814973 adafruit-circuitpython-httpserver-4.2.0/setup.cfg
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-httpserver-4.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/.gitignore` & `adafruit-circuitpython-httpserver-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/.pre-commit-config.yaml` & `adafruit-circuitpython-httpserver-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/.pylintrc` & `adafruit-circuitpython-httpserver-4.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-httpserver-4.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/LICENSE` & `adafruit-circuitpython-httpserver-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-httpserver-4.2.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/LICENSES/MIT.txt` & `adafruit-circuitpython-httpserver-4.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-httpserver-4.2.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/PKG-INFO` & `adafruit-circuitpython-httpserver-4.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.1.0
+Version: 4.2.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -45,14 +45,15 @@
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
+- Supports Websockets and Server-Sent Events.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/README.rst` & `adafruit-circuitpython-httpserver-4.2.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
+- Supports Websockets and Server-Sent Events.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-httpserver
-Version: 4.1.0
+Version: 4.2.0
 Summary: Simple HTTP Server for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git
 Keywords: adafruit,blinka,circuitpython,micropython,httpserver,web,server,webserver,http
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -45,14 +45,15 @@
 - HTTP 1.1.
 - Serves files from a designated root.
 - Routing for serving computed responses from handlers.
 - Gives access to request headers, query parameters, form data, body and client's address (the one from which the request came).
 - Supports chunked transfer encoding.
 - Supports URL parameters and wildcard URLs.
 - Supports HTTP Basic and Bearer Authentication on both server and route per level.
+- Supports Websockets and Server-Sent Events.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_circuitpython_httpserver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,11 +54,13 @@
 examples/httpserver_mdns.py
 examples/httpserver_methods.py
 examples/httpserver_multiple_servers.py
 examples/httpserver_neopixel.py
 examples/httpserver_redirects.py
 examples/httpserver_simpletest_auto.py
 examples/httpserver_simpletest_manual.py
+examples/httpserver_sse.py
 examples/httpserver_start_and_poll.py
 examples/httpserver_static_files_serving.py
 examples/httpserver_url_parameters.py
+examples/httpserver_websocket.py
 examples/settings.toml
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/__init__.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries, Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver`
 ================================================================================
 
 Socket based HTTP Server for CircuitPython
@@ -15,15 +15,15 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 
-__version__ = "4.1.0"
+__version__ = "4.2.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"
 
 
 from .authentication import (
     Basic,
     Bearer,
     check_authentication,
@@ -54,24 +54,28 @@
 from .request import QueryParams, FormData, Request
 from .response import (
     Response,
     FileResponse,
     ChunkedResponse,
     JSONResponse,
     Redirect,
+    SSEResponse,
+    Websocket,
 )
+from .route import Route, as_route
 from .server import (
     Server,
     NO_REQUEST,
     CONNECTION_TIMED_OUT,
     REQUEST_HANDLED_NO_RESPONSE,
     REQUEST_HANDLED_RESPONSE_SENT,
 )
 from .status import (
     Status,
+    SWITCHING_PROTOCOLS_101,
     OK_200,
     CREATED_201,
     ACCEPTED_202,
     NO_CONTENT_204,
     PARTIAL_CONTENT_206,
     TEMPORARY_REDIRECT_307,
     PERMANENT_REDIRECT_308,
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/authentication.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.authentication`
 ====================================================
 * Author(s): Michał Pokusa
 """
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/exceptions.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.exceptions`
 ====================================================
 * Author(s): Michał Pokusa
 """
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/headers.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.headers`
 ====================================================
 * Author(s): Michał Pokusa
 """
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/mime_types.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/mime_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries, Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.mime_types`
 ====================================================
 * Author(s): Michał Pokusa
 """
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/request.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries, Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.request`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
@@ -298,16 +298,16 @@
             request.form_data.get_list("baz")  # ["qux"]
         """
         if self._form_data is None and self.method == "POST":
             self._form_data = FormData(self.body, self.headers["Content-Type"])
         return self._form_data
 
     def json(self) -> Union[dict, None]:
-        """Body of the request, as a JSON-decoded dictionary."""
-        return json.loads(self.body) if self.body else None
+        """Body of the request, as a JSON-decoded dictionary. Only available for POST requests."""
+        return json.loads(self.body) if (self.body and self.method == "POST") else None
 
     @property
     def _raw_header_bytes(self) -> bytes:
         """Returns headers bytes."""
         empty_line_index = self.raw_request.find(b"\r\n\r\n")
 
         return self.raw_request[:empty_line_index]
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/server.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries, Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.server`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
@@ -25,15 +25,15 @@
     InvalidPathError,
     ServingFilesDisabledError,
 )
 from .headers import Headers
 from .methods import GET, HEAD
 from .request import Request
 from .response import Response, FileResponse
-from .route import _Routes, _Route
+from .route import _Routes, Route
 from .status import BAD_REQUEST_400, UNAUTHORIZED_401, FORBIDDEN_403, NOT_FOUND_404
 
 
 NO_REQUEST = "no_request"
 CONNECTION_TIMED_OUT = "connection_timed_out"
 REQUEST_HANDLED_NO_RESPONSE = "request_handled_no_response"
 REQUEST_HANDLED_RESPONSE_SENT = "request_handled_response_sent"
@@ -125,25 +125,44 @@
 
             # It is possible to use wildcard that can match any number of path segments
             @server.route("/example/.../something", GET) # e.g. /example/123/something
             @server.route("/example/..../something", GET) # e.g. /example/123/456/something
             def route_func(request):
                 ...
         """
-        if path.endswith("/") and append_slash:
-            raise ValueError("Cannot use append_slash=True when path ends with /")
-
-        methods = set(methods) if isinstance(methods, (set, list)) else set([methods])
 
         def route_decorator(func: Callable) -> Callable:
-            self._routes.add(_Route(path, methods, append_slash), func)
+            self._routes.add(Route(path, methods, func, append_slash=append_slash))
             return func
 
         return route_decorator
 
+    def add_routes(self, routes: List[Route]) -> None:
+        """
+        Add multiple routes at once.
+
+        :param List[Route] routes: List of routes to add to the server
+
+        Example::
+
+            from separate_file import external_route1, external_route2
+
+            ...
+
+            server.add_routes([
+                Route("/example", GET, route_func1, append_slash=True),
+                Route("/example/<my_parameter>", GET, route_func2),
+                Route("/example/..../something", [GET, POST], route_func3),
+                external_route1,
+                external_route2,
+            ]}
+        """
+        for route in routes:
+            self._routes.add(route)
+
     def _verify_can_start(self, host: str, port: int) -> None:
         """Check if the server can be successfully started. Raises RuntimeError if not."""
 
         if host is None or port is None:
             raise RuntimeError("Host and port cannot be None")
 
         try:
@@ -333,54 +352,54 @@
         e.g. ``NO_REQUEST`` or ``REQUEST_HANDLED_RESPONSE_SENT``.
         """
         if self.stopped:
             raise ServerStoppedError
 
         try:
             conn, client_address = self._sock.accept()
-            with conn:
-                conn.settimeout(self._timeout)
+            conn.settimeout(self._timeout)
 
-                # Receive the whole request
-                if (request := self._receive_request(conn, client_address)) is None:
-                    return CONNECTION_TIMED_OUT
-
-                # Find a handler for the route
-                handler = self._routes.find_handler(
-                    _Route(request.path, request.method)
-                )
+            # Receive the whole request
+            if (request := self._receive_request(conn, client_address)) is None:
+                conn.close()
+                return CONNECTION_TIMED_OUT
+
+            # Find a handler for the route
+            handler = self._routes.find_handler(Route(request.path, request.method))
 
-                # Handle the request
-                response = self._handle_request(request, handler)
+            # Handle the request
+            response = self._handle_request(request, handler)
 
-                if response is None:
-                    return REQUEST_HANDLED_NO_RESPONSE
+            if response is None:
+                conn.close()
+                return REQUEST_HANDLED_NO_RESPONSE
 
-                self._set_default_server_headers(response)
+            self._set_default_server_headers(response)
 
-                # Send the response
-                response._send()  # pylint: disable=protected-access
+            # Send the response
+            response._send()  # pylint: disable=protected-access
 
-                if self.debug:
-                    _debug_response_sent(response)
+            if self.debug:
+                _debug_response_sent(response)
 
-                return REQUEST_HANDLED_RESPONSE_SENT
+            return REQUEST_HANDLED_RESPONSE_SENT
 
         except Exception as error:  # pylint: disable=broad-except
             if isinstance(error, OSError):
                 # There is no data available right now, try again later.
                 if error.errno == EAGAIN:
                     return NO_REQUEST
                 # Connection reset by peer, try again later.
                 if error.errno == ECONNRESET:
                     return NO_REQUEST
 
             if self.debug:
                 _debug_exception_in_handler(error)
 
+            conn.close()
             raise error  # Raise the exception again to be handled by the user.
 
     def require_authentication(self, auths: List[Union[Basic, Bearer]]) -> None:
         """
         Requires authentication for all routes and files in ``root_path``.
         Any non-authenticated request will be rejected with a 401 status code.
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/adafruit_httpserver/status.py` & `adafruit-circuitpython-httpserver-4.2.0/adafruit_httpserver/status.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: Copyright (c) 2022 Dan Halbert for Adafruit Industries, Michał Pokusa
 #
 # SPDX-License-Identifier: MIT
 """
 `adafruit_httpserver.status`
 ====================================================
 * Author(s): Dan Halbert, Michał Pokusa
 """
@@ -27,14 +27,16 @@
     def __str__(self):
         return f"{self.code} {self.text}"
 
     def __eq__(self, other: "Status"):
         return self.code == other.code and self.text == other.text
 
 
+SWITCHING_PROTOCOLS_101 = Status(101, "Switching Protocols")
+
 OK_200 = Status(200, "OK")
 
 CREATED_201 = Status(201, "Created")
 
 ACCEPTED_202 = Status(202, "Accepted")
 
 NO_CONTENT_204 = Status(204, "No Content")
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/docs/_static/favicon.ico` & `adafruit-circuitpython-httpserver-4.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/docs/api.rst` & `adafruit-circuitpython-httpserver-4.2.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/docs/conf.py` & `adafruit-circuitpython-httpserver-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/docs/examples.rst` & `adafruit-circuitpython-httpserver-4.2.0/docs/examples.rst`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 It also manually connects to the WiFi network.
 
 .. literalinclude:: ../examples/httpserver_simpletest_manual.py
     :caption: examples/httpserver_simpletest_manual.py
     :emphasize-lines: 12-17
     :linenos:
 
+It is also possible to use Ethernet instead of WiFi.
+The only difference in usage is related to configuring the ``socket_source`` differently.
+
+.. literalinclude:: ../examples/httpserver_ethernet_simpletest.py
+    :caption: examples/httpserver_ethernet_simpletest.py
+    :emphasize-lines: 13-23
+    :linenos:
+
 Although there is nothing wrong with this approach, from the version 8.0.0 of CircuitPython,
 `it is possible to use the environment variables <https://docs.circuitpython.org/en/latest/docs/environment.html#circuitpython-behavior>`_
 defined in ``settings.toml`` file to store secrets and configure the WiFi network.
 
 This is the same example as above, but it uses the ``settings.toml`` file to configure the WiFi network.
 
 **From now on, all the examples will use the** ``settings.toml`` **file to configure the WiFi network.**
@@ -28,14 +36,15 @@
     :lines: 5-
     :linenos:
 
 Note that we still need to import ``socketpool`` and ``wifi`` modules.
 
 .. literalinclude:: ../examples/httpserver_simpletest_auto.py
     :caption: examples/httpserver_simpletest_auto.py
+    :emphasize-lines: 11
     :linenos:
 
 Serving static files
 --------------------
 
 It is possible to serve static files from the filesystem.
 In this example we are serving files from the ``/static`` directory.
@@ -72,15 +81,15 @@
 for example read a sensor and capture an average or
 a running total of the last 10 samples.
 
 ``.poll()`` return value can be used to check if there was a request and if it was handled.
 
 .. literalinclude:: ../examples/httpserver_start_and_poll.py
     :caption: examples/httpserver_start_and_poll.py
-    :emphasize-lines: 24,33
+    :emphasize-lines: 29,38
     :linenos:
 
 Server with MDNS
 ----------------
 
 It is possible to use the MDNS protocol to make the server accessible via a hostname in addition
 to an IP address. It is worth noting that it takes a bit longer to get the response from the server
@@ -141,15 +150,15 @@
 
 For example by going to ``/change-neopixel-color?r=255&g=0&b=0`` or ``/change-neopixel-color/255/0/0``
 you can change the color of the NeoPixel to red.
 Tested on ESP32-S2 Feather.
 
 .. literalinclude:: ../examples/httpserver_neopixel.py
     :caption: examples/httpserver_neopixel.py
-    :emphasize-lines: 25-27,39,51,60,66
+    :emphasize-lines: 26-28,41,52,68,74
     :linenos:
 
 Form data parsing
 ---------------------
 
 Another way to pass data to the handler function is to use form data.
 Remember that it is only possible to use it with ``POST`` method.
@@ -255,14 +264,51 @@
 You can specify wheter the redirect is permanent or temporary by passing ``permanent=...``  to ``Redirect``.
 
 .. literalinclude:: ../examples/httpserver_redirects.py
     :caption: examples/httpserver_redirects.py
     :emphasize-lines: 14-18,26,38
     :linenos:
 
+Server-Sent Events
+------------------
+
+All types of responses until now were synchronous, meaning that the response was sent immediately after the handler function returned.
+However, sometimes you might want to send data to the client at a later time, e.g. when some event occurs.
+This can be overcomed by periodically polling the server, but it is not an elegant solution. Instead, you can use Server-Sent Events (SSE).
+
+Response is initialized on ``return``, events can be sent using ``.send_event()`` method. Due to the nature of SSE, it is necessary to store the
+response object somewhere, so that it can be accessed later.
+
+**Because of the limited number of concurrently open sockets, it is not possible to process more than one SSE response at the same time.
+This might change in the future, but for now, it is recommended to use SSE only with one client at a time.**
+
+.. literalinclude:: ../examples/httpserver_sse.py
+    :caption: examples/httpserver_sse.py
+    :emphasize-lines: 10,17,46-53,63
+    :linenos:
+
+Websockets
+----------
+
+Although SSE provide a simple way to send data from the server to the client, they are not suitable for sending data the other way around.
+
+For that purpose, you can use Websockets. They are more complex than SSE, but they provide a persistent two-way communication channel between
+the client and the server.
+
+Remember, that because Websockets also receive data, you have to explicitly call ``.receive()`` on the ``Websocket`` object to get the message.
+This is anologous to calling ``.poll()`` on the ``Server`` object.
+
+**Because of the limited number of concurrently open sockets, it is not possible to process more than one Websocket response at the same time.
+This might change in the future, but for now, it is recommended to use Websocket only with one client at a time.**
+
+.. literalinclude:: ../examples/httpserver_websocket.py
+    :caption: examples/httpserver_websocket.py
+    :emphasize-lines: 12,21,67-73,83,90
+    :linenos:
+
 Multiple servers
 ----------------
 
 Although it is not the primary use case, it is possible to run multiple servers at the same time.
 In order to do that, you need to create multiple ``Server`` instances and call ``.start()`` and ``.poll()`` on each of them.
 Using ``.serve_forever()`` for this is not possible because of it's blocking behaviour.
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/docs/index.rst` & `adafruit-circuitpython-httpserver-4.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_handlers.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_authentication_handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response, UNATUHORIZED_401
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_authentication_server.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_authentication_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response, Basic, Bearer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_chunked.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_chunked.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2022 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, ChunkedResponse
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_cpu_information.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_cpu_information.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_ethernet_simpletest.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_ethernet_simpletest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2023 Tim C for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import board
 import digitalio
+
 from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 import adafruit_wiznet5k.adafruit_wiznet5k_socket as socket
 from adafruit_httpserver import Server, Request, Response
 
 print("Wiznet5k HTTPServer Test")
 
 # For Adafruit Ethernet FeatherWing
@@ -14,18 +15,18 @@
 # For Particle Ethernet FeatherWing
 # cs = digitalio.DigitalInOut(board.D5)
 spi_bus = board.SPI()
 
 # Initialize ethernet interface with DHCP
 eth = WIZNET5K(spi_bus, cs)
 
-# set the interface on the socket source
+# Set the interface on the socket source
 socket.set_interface(eth)
 
-# initialize the server
+# Initialize the server
 server = Server(socket, "/static", debug=True)
 
 
 @server.route("/")
 def base(request: Request):
     """
     Serve a default static plain text message.
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_form_data.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_form_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response, GET, POST
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries # # SPDX-
-License-Identifier: Unlicense import socketpool import wifi from
-adafruit_httpserver import Server, Request, Response, GET, POST pool =
-socketpool.SocketPool(wifi.radio) server = Server(pool, debug=True)
-FORM_HTML_TEMPLATE = """
+# SPDX-FileCopyrightText: 2023 MichaÅ Pokusa # # SPDX-License-Identifier:
+Unlicense import socketpool import wifi from adafruit_httpserver import Server,
+Request, Response, GET, POST pool = socketpool.SocketPool(wifi.radio) server =
+Server(pool, debug=True) FORM_HTML_TEMPLATE = """
 Load_application/x-www-form-urlencoded_form
 Load_multipart/form-data_form
 Load_text/plain_form
 ***** Form with {enctype} enctype *****
 [something           ] [Submit]
 {submitted_value}
 """ @server.route("/form", [GET, POST]) def form(request: Request): """ Serve a
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_mdns.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_mdns.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2022 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import mdns
 import socketpool
 import wifi
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_methods.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, JSONResponse, GET, POST, PUT, DELETE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_multiple_servers.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_multiple_servers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_neopixel.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_neopixel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2022 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import board
 import neopixel
 import socketpool
 import wifi
 
-from adafruit_httpserver import Server, Request, Response, GET, POST
+from adafruit_httpserver import Server, Route, as_route, Request, Response, GET, POST
 
 
 pool = socketpool.SocketPool(wifi.radio)
 server = Server(pool, "/static", debug=True)
 
 pixel = neopixel.NeoPixel(board.NEOPIXEL, 1)
 
 
+# This is the simplest way to register a route. It uses the Server object in current scope.
 @server.route("/change-neopixel-color", GET)
 def change_neopixel_color_handler_query_params(request: Request):
     """Changes the color of the built-in NeoPixel using query/GET params."""
 
     # e.g. /change-neopixel-color?r=255&g=0&b=0
 
     r = request.query_params.get("r") or 0
@@ -27,57 +28,67 @@
     b = request.query_params.get("b") or 0
 
     pixel.fill((int(r), int(g), int(b)))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
-@server.route("/change-neopixel-color/body", POST)
-def change_neopixel_color_handler_post_body(request: Request):
-    """Changes the color of the built-in NeoPixel using POST body."""
-
-    data = request.body  # e.g b"255,0,0"
-    r, g, b = data.decode().split(",")  # ["255", "0", "0"]
-
-    pixel.fill((int(r), int(g), int(b)))
-
-    return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
-
-
-@server.route("/change-neopixel-color/form-data", POST)
+# This is another way to register a route. It uses the decorator that converts the function into
+# a Route object that can be imported and registered later.
+@as_route("/change-neopixel-color/form-data", POST)
 def change_neopixel_color_handler_post_form_data(request: Request):
     """Changes the color of the built-in NeoPixel using POST form data."""
 
     data = request.form_data  # e.g. r=255&g=0&b=0 or r=255\r\nb=0\r\ng=0
     r, g, b = data.get("r", 0), data.get("g", 0), data.get("b", 0)
 
     pixel.fill((int(r), int(g), int(b)))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
-@server.route("/change-neopixel-color/json", POST)
 def change_neopixel_color_handler_post_json(request: Request):
     """Changes the color of the built-in NeoPixel using JSON POST body."""
 
     data = request.json()  # e.g {"r": 255, "g": 0, "b": 0}
     r, g, b = data.get("r", 0), data.get("g", 0), data.get("b", 0)
 
     pixel.fill((r, g, b))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
-@server.route("/change-neopixel-color/<r>/<g>/<b>", GET)
+# You can always manually create a Route object and import or register it later.
+# Using this approach you can also use the same handler for multiple routes.
+post_json_route = Route(
+    "/change-neopixel-color/json", POST, change_neopixel_color_handler_post_json
+)
+
+
 def change_neopixel_color_handler_url_params(
     request: Request, r: str = "0", g: str = "0", b: str = "0"
 ):
     """Changes the color of the built-in NeoPixel using URL params."""
 
     # e.g. /change-neopixel-color/255/0/0
 
     pixel.fill((int(r), int(g), int(b)))
 
     return Response(request, f"Changed NeoPixel to color ({r}, {g}, {b})")
 
 
+# Registering Route objects
+server.add_routes(
+    [
+        change_neopixel_color_handler_post_form_data,
+        post_json_route,
+        # You can also register a inline created Route object
+        Route(
+            path="/change-neopixel-color/<r>/<g>/<b>",
+            methods=GET,
+            handler=change_neopixel_color_handler_url_params,
+        ),
+    ]
+)
+
+
 server.serve_forever(str(wifi.radio.ipv4_address))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_redirects.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_redirects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response, Redirect, NOT_FOUND_404
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_auto.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_simpletest_auto.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_simpletest_manual.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_simpletest_manual.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_start_and_poll.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_start_and_poll.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_static_files_serving.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_static_files_serving.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 
 import socketpool
 import wifi
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/examples/httpserver_url_parameters.py` & `adafruit-circuitpython-httpserver-4.2.0/examples/httpserver_url_parameters.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2022 Dan Halbert for Adafruit Industries
+# SPDX-FileCopyrightText: 2023 Michał Pokusa
 #
 # SPDX-License-Identifier: Unlicense
 
 import socketpool
 import wifi
 
 from adafruit_httpserver import Server, Request, Response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `adafruit-circuitpython-httpserver-4.1.0/pyproject.toml` & `adafruit-circuitpython-httpserver-4.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-httpserver"
 description = "Simple HTTP Server for CircuitPython"
-version = "4.1.0"
+version = "4.2.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTTPServer.git"}
 keywords = [
     "adafruit",
```

