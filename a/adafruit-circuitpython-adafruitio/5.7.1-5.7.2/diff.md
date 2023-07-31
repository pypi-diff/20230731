# Comparing `tmp/adafruit-circuitpython-adafruitio-5.7.1.tar.gz` & `tmp/adafruit-circuitpython-adafruitio-5.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-adafruitio-5.7.1.tar", last modified: Fri May 26 16:22:36 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-adafruitio-5.7.2.tar", last modified: Mon Jul 31 15:50:17 2023, max compression
```

## Comparing `adafruit-circuitpython-adafruitio-5.7.1.tar` & `adafruit-circuitpython-adafruitio-5.7.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.158931 adafruit-circuitpython-adafruitio-5.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 16:22:36.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.162931 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27829 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.166931 adafruit-circuitpython-adafruitio-5.7.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_analog_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_digital_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_randomizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4105 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4134 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4627 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-26 16:22:25.000000 adafruit-circuitpython-adafruitio-5.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 16:22:13.000000 adafruit-circuitpython-adafruitio-5.7.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:36.170931 adafruit-circuitpython-adafruitio-5.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.090404 adafruit-circuitpython-adafruitio-5.7.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.082404 adafruit-circuitpython-adafruitio-5.7.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-31 15:50:17.090404 adafruit-circuitpython-adafruitio-5.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-31 15:50:17.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-31 15:50:17.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 15:50:17.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-31 15:50:17.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-31 15:50:17.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28617 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/adafruit_io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/adafruit_io_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.086404 adafruit-circuitpython-adafruitio-5.7.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.090404 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_digital_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_randomizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:17.090404 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4105 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4134 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3508 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4404 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4627 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-31 15:50:09.000000 adafruit-circuitpython-adafruitio-5.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-31 15:50:01.000000 adafruit-circuitpython-adafruitio-5.7.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-31 15:50:17.090404 adafruit-circuitpython-adafruitio-5.7.2/setup.cfg
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-adafruitio-5.7.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/.gitignore` & `adafruit-circuitpython-adafruitio-5.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/.pre-commit-config.yaml` & `adafruit-circuitpython-adafruitio-5.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/.pylintrc` & `adafruit-circuitpython-adafruitio-5.7.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-adafruitio-5.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/LICENSE` & `adafruit-circuitpython-adafruitio-5.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-adafruitio-5.7.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/MIT.txt` & `adafruit-circuitpython-adafruitio-5.7.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-adafruitio-5.7.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.7.1
+Version: 5.7.2
 Summary: Adafruit IO for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Keywords: adafruit,blinka,circuitpython,micropython,adafruit_io,adafruit-io,rest,api,iot,wifi
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/README.rst` & `adafruit-circuitpython-adafruitio-5.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO` & `adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adafruitio
-Version: 5.7.1
+Version: 5.7.2
 Summary: Adafruit IO for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO
 Keywords: adafruit,blinka,circuitpython,micropython,adafruit_io,adafruit-io,rest,api,iot,wifi
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt` & `adafruit-circuitpython-adafruitio-5.7.2/adafruit_circuitpython_adafruitio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io.py` & `adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/adafruit_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,28 +18,33 @@
 * Adafruit CircuitPython firmware for the supported boards:
     https://github.com/adafruit/circuitpython/releases
 """
 import time
 import json
 import re
 
+try:
+    from typing import List, Any, Callable, Optional
+except ImportError:
+    pass
+
 from adafruit_minimqtt.adafruit_minimqtt import MMQTTException
 from adafruit_io.adafruit_io_errors import (
     AdafruitIO_RequestError,
     AdafruitIO_ThrottleError,
     AdafruitIO_MQTTError,
 )
 
-__version__ = "5.7.1"
+__version__ = "5.7.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO.git"
 
 CLIENT_HEADERS = {"User-Agent": "AIO-CircuitPython/{0}".format(__version__)}
 
 
-def validate_feed_key(feed_key):
+def validate_feed_key(feed_key: str):
     """Validates a provided feed key against Adafruit IO's system rules.
     https://learn.adafruit.com/naming-things-in-adafruit-io/the-two-feed-identifiers
     """
     if len(feed_key) > 128:  # validate feed key length
         raise ValueError("Feed key must be less than 128 characters.")
     if not bool(
         re.match(r"^[a-zA-Z0-9-]+((\/|\.)[a-zA-Z0-9-]+)?$", feed_key)
@@ -139,15 +144,15 @@
         """Runs when the client calls on_disconnect."""
         self._connected = False
         # Call the user-defined on_disconnect callblack if defined
         if self.on_disconnect is not None:
             self.on_disconnect(self)
 
     # pylint: disable=not-callable
-    def _on_message_mqtt(self, client, topic, payload):
+    def _on_message_mqtt(self, client, topic: str, payload: str):
         """Runs when the client calls on_message. Parses and returns
         incoming data from Adafruit IO feeds.
 
         :param MQTT client: A MQTT Client Instance.
         :param str topic: MQTT topic response from Adafruit IO.
         :param str payload: MQTT payload data response from Adafruit IO.
         """
@@ -191,15 +196,15 @@
 
     # pylint: disable=not-callable
     def _on_unsubscribe_mqtt(self, client, user_data, topic, pid):
         """Runs when the client calls on_unsubscribe."""
         if self.on_unsubscribe is not None:
             self.on_unsubscribe(self, user_data, topic, pid)
 
-    def add_feed_callback(self, feed_key, callback_method):
+    def add_feed_callback(self, feed_key: str, callback_method: Callable):
         """Attaches a callback_method to an Adafruit IO feed.
         The callback_method function is called when a
         new value is written to the feed.
 
         NOTE: The callback_method registered to this method
         will only execute during loop().
 
@@ -207,15 +212,15 @@
         :param str callback_method: Name of callback method.
         """
         validate_feed_key(feed_key)
         self._client.add_topic_callback(
             "{0}/f/{1}".format(self._user, feed_key), callback_method
         )
 
-    def remove_feed_callback(self, feed_key):
+    def remove_feed_callback(self, feed_key: str):
         """Removes a previously registered callback method
         from executing whenever feed_key receives new data.
 
         After this method is called, incoming messages
         call the shared on_message.
 
         :param str feed_key: Adafruit IO feed key.
@@ -235,15 +240,20 @@
 
             while True:
                 io.loop()
         """
         self._client.loop(timeout)
 
     # Subscriptions
-    def subscribe(self, feed_key=None, group_key=None, shared_user=None):
+    def subscribe(
+        self,
+        feed_key: str = None,
+        group_key: str = None,
+        shared_user: Optional[str] = None,
+    ):
         """Subscribes to your Adafruit IO feed or group.
         Can also subscribe to someone else's feed.
 
         :param str feed_key: Adafruit IO Feed key.
         :param str group_key: Adafruit IO Group key.
         :param str shared_user: Owner of the Adafruit IO feed, required for shared feeds.
 
@@ -273,50 +283,55 @@
 
     def subscribe_to_errors(self):
         """Subscribes to your personal Adafruit IO /errors topic.
         Notifies you of errors relating to publish/subscribe calls.
         """
         self._client.subscribe("%s/errors" % self._user)
 
-    def subscribe_to_randomizer(self, randomizer_id):
+    def subscribe_to_randomizer(self, randomizer_id: int):
         """Subscribes to a random data stream created by the Adafruit IO Words service.
 
         :param int randomizer_id: Random word record you want data for.
         """
         self._client.subscribe(
             "{0}/integration/words/{1}".format(self._user, randomizer_id)
         )
 
-    def subscribe_to_weather(self, weather_record, forecast):
+    def subscribe_to_weather(self, weather_record: int, forecast: str):
         """Subscribes to a weather forecast using the Adafruit IO PLUS weather
         service. This feature is only avaliable to Adafruit IO PLUS subscribers.
 
         :param int weather_record: Weather record you want data for.
         :param str forecast: Forecast data you'd like to recieve.
         """
         self._client.subscribe(
             "{0}/integration/weather/{1}/{2}".format(
                 self._user, weather_record, forecast
             )
         )
 
-    def subscribe_to_time(self, time_type):
+    def subscribe_to_time(self, time_type: str):
         """Adafruit IO provides some built-in MQTT topics for getting the current server time.
 
         :param str time_type: Current Adafruit IO server time. Can be 'seconds', 'millis', or 'iso'.
 
         Information about these topics can be found on the Adafruit IO MQTT API Docs.:
         https://io.adafruit.com/api/docs/mqtt.html#time-topics
         """
         if time_type == "iso":
             self._client.subscribe("time/ISO-8601")
         else:
             self._client.subscribe("time/" + time_type)
 
-    def unsubscribe(self, feed_key=None, group_key=None, shared_user=None):
+    def unsubscribe(
+        self,
+        feed_key: str = None,
+        group_key: str = None,
+        shared_user: Optional[str] = None,
+    ):
         """Unsubscribes from an Adafruit IO feed or group.
         Can also subscribe to someone else's feed.
 
         :param str feed_key: Adafruit IO Feed key.
         :param str group_key: Adafruit IO Group key.
         :param str shared_user: Owner of the Adafruit IO feed, required for shared feeds.
 
@@ -341,19 +356,21 @@
         elif feed_key is not None:
             validate_feed_key(feed_key)
             self._client.unsubscribe("{0}/f/{1}".format(self._user, feed_key))
         else:
             raise AdafruitIO_MQTTError("Must provide a feed_key or group_key.")
 
     # Publishing
-    def publish_multiple(self, feeds_and_data, timeout=3, is_group=False):
+    def publish_multiple(
+        self, feeds_and_data: List, timeout: int = 3, is_group: bool = False
+    ):
         """Publishes multiple data points to multiple feeds or groups with a variable
         timeout.
 
-        :param str feeds_and_data: List of tuples containing topic strings and data values.
+        :param list feeds_and_data: List of tuples containing topic strings and data values.
         :param int timeout: Delay between publishing data points to Adafruit IO, in seconds.
         :param bool is_group: Set to True if you're publishing to a group.
 
         Example of publishing multiple data points on different feeds to Adafruit IO:
 
         .. code-block:: python
 
@@ -369,16 +386,23 @@
             if is_group:
                 self.publish(topic, data, is_group=True)
             else:
                 self.publish(topic, data)
             time.sleep(timeout)
 
     # pylint: disable=too-many-arguments
-    def publish(self, feed_key, data, metadata=None, shared_user=None, is_group=False):
-        """Publishes to an An Adafruit IO Feed.
+    def publish(
+        self,
+        feed_key: str,
+        data: str,
+        metadata: str = None,
+        shared_user: str = None,
+        is_group: bool = False,
+    ):
+        """Publishes to an Adafruit IO Feed.
 
         :param str feed_key: Adafruit IO Feed key.
         :param str data: Data to publish to the feed or group.
         :param int data: Data to publish to the feed or group.
         :param float data: Data to publish to the feed or group.
         :param str metadata: Optional metadata associated with the data.
         :param str shared_user: Owner of the Adafruit IO feed, required for
@@ -435,15 +459,15 @@
             csv_string = data + "," + metadata
             self._client.publish(
                 "{0}/f/{1}/csv".format(self._user, feed_key), csv_string
             )
         else:
             self._client.publish("{0}/f/{1}".format(self._user, feed_key), data)
 
-    def get(self, feed_key):
+    def get(self, feed_key: str):
         """Calling this method will make Adafruit IO publish the most recent
         value on feed_key.
         https://io.adafruit.com/api/docs/mqtt.html#retained-values
 
         :param str feed_key: Adafruit IO Feed key.
 
         Example of obtaining a recently published value on a feed:
@@ -480,15 +504,15 @@
     def _create_headers(io_headers):
         """Creates http request headers."""
         headers = CLIENT_HEADERS.copy()
         headers.update(io_headers)
         return headers
 
     @staticmethod
-    def _create_data(data, metadata):
+    def _create_data(data, metadata: dict):
         """Returns a data payload as expected by the Adafruit IO HTTP API
 
         :param data: Payload value.
         :param dict metadata: Payload metadata.
         """
         payload = {"value": data}
         if metadata:  # metadata is expected as a dict, append key/vals
@@ -504,66 +528,72 @@
         if response.status_code == 429:
             raise AdafruitIO_ThrottleError
         if response.status_code == 400:
             raise AdafruitIO_RequestError(response)
         if response.status_code >= 400:
             raise AdafruitIO_RequestError(response)
 
-    def _compose_path(self, path):
+    def _compose_path(self, path: str):
         """Composes a valid API request path.
 
         :param str path: Adafruit IO API URL path.
         """
         return "https://io.adafruit.com/api/v2/{0}/{1}".format(self.username, path)
 
     # HTTP Requests
-    def _post(self, path, payload):
+    def _post(self, path: str, payload: Any):
         """
         POST data to Adafruit IO
 
         :param str path: Formatted Adafruit IO URL from _compose_path
         :param json payload: JSON data to send to Adafruit IO
         """
         with self._http.post(
             path, json=payload, headers=self._create_headers(self._aio_headers[0])
         ) as response:
             self._handle_error(response)
             json_data = response.json()
 
         return json_data
 
-    def _get(self, path):
+    def _get(self, path: str):
         """
         GET data from Adafruit IO
 
         :param str path: Formatted Adafruit IO URL from _compose_path
         """
         with self._http.get(
             path, headers=self._create_headers(self._aio_headers[1])
         ) as response:
             self._handle_error(response)
             json_data = response.json()
         return json_data
 
-    def _delete(self, path):
+    def _delete(self, path: str):
         """
         DELETE data from Adafruit IO.
 
         :param str path: Formatted Adafruit IO URL from _compose_path
         """
         with self._http.delete(
             path, headers=self._create_headers(self._aio_headers[0])
         ) as response:
             self._handle_error(response)
             json_data = response.json()
 
         return json_data
 
     # Data
-    def send_data(self, feed_key, data, metadata=None, precision=None):
+    def send_data(
+        self,
+        feed_key: str,
+        data: str,
+        metadata: Optional[dict] = None,
+        precision: Optional[int] = None,
+    ):
         """
         Sends value data to a specified Adafruit IO feed.
 
         :param str feed_key: Adafruit IO feed key
         :param str data: Data to send to the Adafruit IO feed
         :param dict metadata: Optional metadata associated with the data
         :param int precision: Optional amount of precision points to send with floating point data
@@ -576,140 +606,149 @@
             except NotImplementedError as err:  # received a non-float value
                 raise NotImplementedError(
                     "Precision requires a floating point value"
                 ) from err
         payload = self._create_data(data, metadata)
         self._post(path, payload)
 
-    def send_batch_data(self, feed_key, data_list):
+    def send_batch_data(self, feed_key: str, data_list: list):
         """
         Sends a batch array of data to a specified Adafruit IO feed
 
         :param str feed_key: Adafruit IO feed key
         :param list Data: Data list to send
         """
         validate_feed_key(feed_key)
         path = "feeds/{0}/data/batch".format(feed_key)
         data_dict = type(data_list)((data._asdict() for data in data_list))
         self._post(path, {"data": data_dict})
 
-    def receive_all_data(self, feed_key):
+    def receive_all_data(self, feed_key: str):
         """
         Get all data values from a specified Adafruit IO feed. Data is
         returned in reverse order.
 
         :param str feed_key: Adafruit IO feed key
         """
         validate_feed_key(feed_key)
         path = self._compose_path("feeds/{0}/data".format(feed_key))
         return self._get(path)
 
-    def receive_data(self, feed_key):
+    def receive_data(self, feed_key: str):
         """
         Return the most recent value for the specified feed.
 
         :param string feed_key: Adafruit IO feed key
         """
         validate_feed_key(feed_key)
         path = self._compose_path("feeds/{0}/data/last".format(feed_key))
         return self._get(path)
 
-    def delete_data(self, feed_key, data_id):
+    def delete_data(self, feed_key: str, data_id: str):
         """
         Deletes an existing Data point from a feed.
 
         :param string feed: Adafruit IO feed key
         :param string data_id: Data point to delete from the feed
         """
         validate_feed_key(feed_key)
         path = self._compose_path("feeds/{0}/data/{1}".format(feed_key, data_id))
         return self._delete(path)
 
     # Groups
-    def create_new_group(self, group_key, group_description):
+    def create_new_group(self, group_key: str, group_description: str):
         """
         Creates a new Adafruit IO Group.
 
         :param str group_key: Adafruit IO Group Key
         :param str group_description: Brief summary about the group
         """
         path = self._compose_path("groups")
         payload = {"name": group_key, "description": group_description}
         return self._post(path, payload)
 
-    def delete_group(self, group_key):
+    def delete_group(self, group_key: str):
         """
         Deletes an existing group.
 
         :param str group_key: Adafruit IO Group Key
         """
         path = self._compose_path("groups/{0}".format(group_key))
         return self._delete(path)
 
-    def get_group(self, group_key):
+    def get_group(self, group_key: str):
         """
         Returns Group based on Group Key
 
         :param str group_key: Adafruit IO Group Key
         """
         path = self._compose_path("groups/{0}".format(group_key))
         return self._get(path)
 
-    def create_feed_in_group(self, group_key, feed_name):
+    def create_feed_in_group(self, group_key: str, feed_name: str):
         """Creates a new feed in an existing group.
 
         :param str group_key: Group name.
         :param str feed_name: Name of new feed.
         """
         path = self._compose_path("groups/{0}/feeds".format(group_key))
         payload = {"feed": {"name": feed_name}}
         return self._post(path, payload)
 
-    def add_feed_to_group(self, group_key, feed_key):
+    def add_feed_to_group(self, group_key: str, feed_key: str):
         """
         Adds an existing feed to a group
 
         :param str group_key: Group
         :param str feed_key: Feed to add to the group
         """
         validate_feed_key(feed_key)
         path = self._compose_path("groups/{0}/add".format(group_key))
         payload = {"feed_key": feed_key}
         return self._post(path, payload)
 
     # Feeds
-    def get_feed(self, feed_key, detailed=False):
+    def get_feed(self, feed_key: str, detailed: bool = False):
         """
         Returns an Adafruit IO feed based on the feed key
 
         :param str feed_key: Adafruit IO Feed Key
         :param bool detailed: Returns a more verbose feed record
         """
         validate_feed_key(feed_key)
         if detailed:
             path = self._compose_path("feeds/{0}/details".format(feed_key))
         else:
             path = self._compose_path("feeds/{0}".format(feed_key))
         return self._get(path)
 
-    def create_new_feed(self, feed_key, feed_desc=None, feed_license=None):
+    def create_new_feed(
+        self,
+        feed_key: str,
+        feed_desc: Optional[str] = None,
+        feed_license: Optional[str] = None,
+    ):
         """
         Creates a new Adafruit IO feed.
 
         :param str feed_key: Adafruit IO Feed Key
         :param str feed_desc: Optional description of feed
         :param str feed_license: Optional feed license
         """
         validate_feed_key(feed_key)
         path = self._compose_path("feeds")
         payload = {"name": feed_key, "description": feed_desc, "license": feed_license}
         return self._post(path, payload)
 
     def create_and_get_feed(
-        self, feed_key, detailed=False, feed_desc=None, feed_license=None
+        self,
+        feed_key: str,
+        detailed: bool = False,
+        feed_desc: Optional[str] = None,
+        feed_license: Optional[str] = None,
     ):
         """
         Attempts to return a feed; if the feed does not exist, it is created, and then returned.
 
         :param str feed_key: Adafruit IO Feed Key
         :param bool detailed: Returns a more verbose existing feed record
         :param str feed_desc: Optional description of feed to be created
@@ -719,36 +758,36 @@
             return self.get_feed(feed_key, detailed=detailed)
         except AdafruitIO_RequestError:
             self.create_new_feed(
                 feed_key, feed_desc=feed_desc, feed_license=feed_license
             )
             return self.get_feed(feed_key, detailed=detailed)
 
-    def delete_feed(self, feed_key):
+    def delete_feed(self, feed_key: str):
         """
         Deletes an existing feed.
 
         :param str feed_key: Valid feed key
         """
         validate_feed_key(feed_key)
         path = self._compose_path("feeds/{0}".format(feed_key))
         return self._delete(path)
 
     # Adafruit IO Connected Services
-    def receive_weather(self, weather_id):
+    def receive_weather(self, weather_id: int):
         """
         Get data from the Adafruit IO Weather Forecast Service
         NOTE: This service is avaliable to Adafruit IO Plus subscribers only.
 
         :param int weather_id: ID for retrieving a specified weather record.
         """
         path = self._compose_path("integrations/weather/{0}".format(weather_id))
         return self._get(path)
 
-    def receive_random_data(self, generator_id):
+    def receive_random_data(self, generator_id: int):
         """
         Get data from the Adafruit IO Random Data Stream Service
 
         :param int generator_id: Specified randomizer record
         """
         path = self._compose_path("integrations/words/{0}".format(generator_id))
         return self._get(path)
```

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/adafruit_io/adafruit_io_errors.py` & `adafruit-circuitpython-adafruitio-5.7.2/adafruit_io/adafruit_io_errors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/docs/_static/favicon.ico` & `adafruit-circuitpython-adafruitio-5.7.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/docs/conf.py` & `adafruit-circuitpython-adafruitio-5.7.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/docs/index.rst` & `adafruit-circuitpython-adafruitio-5.7.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_analog_in.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_create_and_get_feed.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_digital_out.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_digital_out.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_feeds.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_feeds.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_metadata.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_metadata.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_randomizer.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_randomizer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_temperature.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_temperature.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_http/adafruit_io_weather.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_http/adafruit_io_weather.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_feed_callback.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_groups.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_groups.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_location.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_location.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_pubsub_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_esp32s2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_mqtt/adafruit_io_time.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_mqtt/adafruit_io_time.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/examples/adafruit_io_simpletest.py` & `adafruit-circuitpython-adafruitio-5.7.2/examples/adafruit_io_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adafruitio-5.7.1/pyproject.toml` & `adafruit-circuitpython-adafruitio-5.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-adafruitio"
 description = "Adafruit IO for CircuitPython"
-version = "5.7.1"
+version = "5.7.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AdafruitIO"}
 keywords = [
     "adafruit",
```

