# Comparing `tmp/simpy-4.0.1.tar.gz` & `tmp/simpy-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpy-4.0.1.tar", last modified: Wed Apr 15 17:08:56 2020, max compression
+gzip compressed data, was "simpy-4.0.2.tar", last modified: Sun Jul 30 22:54:35 2023, max compression
```

## Comparing `simpy-4.0.1.tar` & `simpy-4.0.2.tar`

### file list

```diff
@@ -1,122 +1,125 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      174 2020-04-15 17:08:49.000000 simpy-4.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1515 2020-04-15 17:08:49.000000 simpy-4.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      496 2020-04-15 17:08:49.000000 simpy-4.0.1/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     6321 2020-04-15 17:08:49.000000 simpy-4.0.1/CHANGES.rst
--rw-rw-rw-   0 root         (0) root         (0)     1125 2020-04-15 17:08:49.000000 simpy-4.0.1/LICENSE.rst
--rw-r--r--   0 root         (0) root         (0)    15404 2020-04-15 17:08:56.000000 simpy-4.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4658 2020-04-15 17:08:49.000000 simpy-4.0.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4595 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/_static/
--rw-rw-rw-   0 root         (0) root         (0)    65385 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/_static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)   132151 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/_static/simpy-logo-quad.png
--rw-rw-rw-   0 root         (0) root         (0)    39939 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/_static/simpy-logo-small.png
--rw-rw-rw-   0 root         (0) root         (0)    77450 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/_static/simpy-logo.png
--rw-rw-rw-   0 root         (0) root         (0)    12364 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/_static/simpy-logo.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/about/
--rw-rw-rw-   0 root         (0) root         (0)      860 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/acknowledgements.rst
--rw-rw-rw-   0 root         (0) root         (0)     8136 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/defense_of_design.rst
--rw-rw-rw-   0 root         (0) root         (0)    16594 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       56 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/license.rst
--rw-rw-rw-   0 root         (0) root         (0)      406 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/ports.rst
--rw-rw-rw-   0 root         (0) root         (0)     4278 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/about/release_process.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/api_reference/
--rw-rw-rw-   0 root         (0) root         (0)      345 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      294 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.core.rst
--rw-rw-rw-   0 root         (0) root         (0)      821 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.events.rst
--rw-rw-rw-   0 root         (0) root         (0)      212 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)     1590 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.resources.rst
--rw-rw-rw-   0 root         (0) root         (0)       53 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.rst
--rw-rw-rw-   0 root         (0) root         (0)     1125 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.rt.rst
--rw-rw-rw-   0 root         (0) root         (0)      217 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/api_reference/simpy.util.rst
--rw-rw-rw-   0 root         (0) root         (0)     8204 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     3849 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/contents.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/examples/
--rw-rw-rw-   0 root         (0) root         (0)      665 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/bank_renege.rst
--rw-rw-rw-   0 root         (0) root         (0)      868 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/carwash.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/examples/code/
--rw-rw-rw-   0 root         (0) root         (0)       77 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/README.txt
--rw-rw-rw-   0 root         (0) root         (0)      455 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/bank_renege.out
--rw-rw-rw-   0 root         (0) root         (0)     1850 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/bank_renege.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/carwash.out
--rw-rw-rw-   0 root         (0) root         (0)     2873 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/carwash.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/gas_station_refuel.out
--rw-rw-rw-   0 root         (0) root         (0)     3535 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/gas_station_refuel.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/latency.out
--rw-rw-rw-   0 root         (0) root         (0)     1585 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/latency.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/machine_shop.out
--rw-rw-rw-   0 root         (0) root         (0)     4471 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/machine_shop.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/movie_renege.out
--rw-rw-rw-   0 root         (0) root         (0)     3398 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/movie_renege.py
--rw-rw-rw-   0 root         (0) root         (0)     2704 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/process_communication.out
--rw-rw-rw-   0 root         (0) root         (0)     4491 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/code/process_communication.py
--rw-rw-rw-   0 root         (0) root         (0)     1021 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/gas_station_refuel.rst
--rw-rw-rw-   0 root         (0) root         (0)     1288 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      568 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/latency.rst
--rw-rw-rw-   0 root         (0) root         (0)     1134 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/machine_shop.rst
--rw-rw-rw-   0 root         (0) root         (0)     1322 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/movie_renege.rst
--rw-rw-rw-   0 root         (0) root         (0)      953 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/examples/process_communication.rst
--rw-rw-rw-   0 root         (0) root         (0)     3315 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4509 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/simpy_intro/
--rw-rw-rw-   0 root         (0) root         (0)     4199 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/basic_concepts.rst
--rw-rw-rw-   0 root         (0) root         (0)      536 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/how_to_proceed.rst
--rw-rw-rw-   0 root         (0) root         (0)      510 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1152 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     5725 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/process_interaction.rst
--rw-rw-rw-   0 root         (0) root         (0)     3712 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/simpy_intro/shared_resources.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/docs/topical_guides/
--rw-rw-rw-   0 root         (0) root         (0)     6345 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/environments.rst
--rw-rw-rw-   0 root         (0) root         (0)    10313 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/events.rst
--rw-rw-rw-   0 root         (0) root         (0)      529 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9924 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/monitoring.rst
--rw-rw-rw-   0 root         (0) root         (0)     9934 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/porting_from_simpy2.rst
--rw-rw-rw-   0 root         (0) root         (0)     4114 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/porting_from_simpy3.rst
--rw-rw-rw-   0 root         (0) root         (0)     7425 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/process_interaction.rst
--rw-rw-rw-   0 root         (0) root         (0)     3111 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/real-time-simulations.rst
--rw-rw-rw-   0 root         (0) root         (0)    19238 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/resources.rst
--rw-rw-rw-   0 root         (0) root         (0)     4463 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/simpy_basics.rst
--rw-rw-rw-   0 root         (0) root         (0)     4033 2020-04-15 17:08:49.000000 simpy-4.0.1/docs/topical_guides/time_and_scheduling.rst
--rw-rw-rw-   0 root         (0) root         (0)      240 2020-04-15 17:08:49.000000 simpy-4.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      102 2020-04-15 17:08:49.000000 simpy-4.0.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)     1567 2020-04-15 17:08:56.000000 simpy-4.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       76 2020-04-15 17:08:49.000000 simpy-4.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy/
--rw-rw-rw-   0 root         (0) root         (0)     2033 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8440 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/core.py
--rw-rw-rw-   0 root         (0) root         (0)    23099 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/events.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy/resources/
--rw-rw-rw-   0 root         (0) root         (0)      390 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9562 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3878 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/resources/container.py
--rw-rw-rw-   0 root         (0) root         (0)     9867 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/resources/resource.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/resources/store.py
--rw-rw-rw-   0 root         (0) root         (0)     3039 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/rt.py
--rw-rw-rw-   0 root         (0) root         (0)     2037 2020-04-15 17:08:49.000000 simpy-4.0.1/src/simpy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15404 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2988 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        6 2020-04-15 17:08:56.000000 simpy-4.0.1/src/simpy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-15 17:08:56.000000 simpy-4.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_benchmark.py
--rw-rw-rw-   0 root         (0) root         (0)     8481 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_condition.py
--rw-rw-rw-   0 root         (0) root         (0)     2049 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     3745 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_event.py
--rw-rw-rw-   0 root         (0) root         (0)     7143 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     5472 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_interrupts.py
--rw-rw-rw-   0 root         (0) root         (0)     4266 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_process.py
--rw-rw-rw-   0 root         (0) root         (0)    21278 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_resources.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_rt.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_timeout.py
--rw-rw-rw-   0 root         (0) root         (0)     8949 2020-04-15 17:08:49.000000 simpy-4.0.1/tests/test_util.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2020-04-15 17:08:49.000000 simpy-4.0.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.492463 simpy-4.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-30 22:54:31.000000 simpy-4.0.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1961 2023-07-30 22:54:31.000000 simpy-4.0.2/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-30 22:54:31.000000 simpy-4.0.2/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-07-30 22:54:31.000000 simpy-4.0.2/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7001 2023-07-30 22:54:31.000000 simpy-4.0.2/CHANGES.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-07-30 22:54:31.000000 simpy-4.0.2/LICENSE.rst
+-rw-r--r--   0 root         (0) root         (0)    13456 2023-07-30 22:54:35.492463 simpy-4.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2023-07-30 22:54:31.000000 simpy-4.0.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.473464 simpy-4.0.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4595 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.475463 simpy-4.0.2/docs/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    65385 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)   132151 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/_static/simpy-logo-quad.png
+-rw-rw-rw-   0 root         (0) root         (0)    39939 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/_static/simpy-logo-small.png
+-rw-rw-rw-   0 root         (0) root         (0)    77450 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/_static/simpy-logo.png
+-rw-rw-rw-   0 root         (0) root         (0)    12364 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/_static/simpy-logo.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.476463 simpy-4.0.2/docs/about/
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/acknowledgements.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8132 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/defense_of_design.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16594 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/license.rst
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/ports.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4279 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/about/release_process.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.478464 simpy-4.0.2/docs/api_reference/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      821 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1125 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.rt.rst
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/api_reference/simpy.util.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8364 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3889 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/contents.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.479463 simpy-4.0.2/docs/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/bank_renege.rst
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/carwash.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.482463 simpy-4.0.2/docs/examples/code/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/README.txt
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/bank_renege.out
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/bank_renege.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/carwash.out
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/carwash.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/gas_station_refuel.out
+-rw-rw-rw-   0 root         (0) root         (0)     3620 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/gas_station_refuel.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/latency.out
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/latency.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/machine_shop.out
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/machine_shop.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/movie_renege.out
+-rw-rw-rw-   0 root         (0) root         (0)     3399 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/movie_renege.py
+-rw-rw-rw-   0 root         (0) root         (0)     2704 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/process_communication.out
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/code/process_communication.py
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/gas_station_refuel.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/latency.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/machine_shop.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/movie_renege.rst
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/examples/process_communication.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3249 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4509 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.484464 simpy-4.0.2/docs/simpy_intro/
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/basic_concepts.rst
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/how_to_proceed.rst
+-rw-rw-rw-   0 root         (0) root         (0)      510 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5725 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/process_interaction.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3712 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/simpy_intro/shared_resources.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.486463 simpy-4.0.2/docs/topical_guides/
+-rw-rw-rw-   0 root         (0) root         (0)     6346 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/environments.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10379 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/events.rst
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9924 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/monitoring.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9935 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/porting_from_simpy2.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4114 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/porting_from_simpy3.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7443 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/process_interaction.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3111 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/real-time-simulations.rst
+-rw-rw-rw-   0 root         (0) root         (0)    19239 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4463 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/simpy_basics.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2023-07-30 22:54:31.000000 simpy-4.0.2/docs/topical_guides/time_and_scheduling.rst
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-07-30 22:54:31.000000 simpy-4.0.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-30 22:54:31.000000 simpy-4.0.2/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2023-07-30 22:54:35.493463 simpy-4.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-30 22:54:31.000000 simpy-4.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.469463 simpy-4.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.487464 simpy-4.0.2/src/simpy/
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8440 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/core.py
+-rw-rw-rw-   0 root         (0) root         (0)    23112 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/events.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.489463 simpy-4.0.2/src/simpy/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9598 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/resources/container.py
+-rw-rw-rw-   0 root         (0) root         (0)     9868 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/resources/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     6312 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/resources/store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/rt.py
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2023-07-30 22:54:31.000000 simpy-4.0.2/src/simpy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.488463 simpy-4.0.2/src/simpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13456 2023-07-30 22:54:35.000000 simpy-4.0.2/src/simpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-30 22:54:35.000000 simpy-4.0.2/src/simpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 22:54:35.000000 simpy-4.0.2/src/simpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-30 22:54:35.000000 simpy-4.0.2/src/simpy.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-30 22:54:35.000000 simpy-4.0.2/src/simpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-30 22:54:35.492463 simpy-4.0.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4145 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_benchmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     8481 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_condition.py
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3746 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     7141 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     5472 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_interrupts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4266 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    21280 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     2878 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_rt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)     8946 2023-07-30 22:54:31.000000 simpy-4.0.2/tests/test_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-07-30 22:54:31.000000 simpy-4.0.2/tox.ini
```

### Comparing `simpy-4.0.1/CHANGES.rst` & `simpy-4.0.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,32 @@
 Changelog for SimPy
 ===================
 
+4.0.2 - 2023-07-30
+------------------
+
+- [CHANGE] Tested with Python 3.9, 3.10, and 3.11
+- [CHANGE] Improved docs w.r.t. triggered and processed events
+- [CHANGE] Improved gas station example
+- [FIX] ClassVar annotations in BaseResource
+- [FIX] Documentation typos
+- [FIX] Help static analyzers find exported symbols
+- [FIX] ``license_file`` deprecation in setup.cfg
+- [FIX] Do not re-annotate type of ``__path__``
+- [FIX] Annotate ``ConditionValue.__init__()`` return value
+- [FIX] Unbreak docs build by updating to Sphinx 6.2.1
+- [FIX] Workaround Sphinx circular import problem
+
+
+4.0.1 - 2020-04-15
+------------------
+
+- [FIX] Typing repair for Get and Put as ContextManagers
+
+
 4.0.0 - 2020-04-06
 ------------------
 
 - [BREAKING] Python 3.6 is the minimum supported version
 - [BREAKING] ``BaseEnvironment`` is eliminated. Inherit ``Environment`` instead.
 - [BREAKING] ``Environment.exit()`` is eliminated. Use ``return`` instead.
 - [NEW] "Porting from SimPy 3 to 4" topical guide in docs
```

### Comparing `simpy-4.0.1/LICENSE.rst` & `simpy-4.0.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/README.rst` & `simpy-4.0.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -126,13 +126,13 @@
 
 Enjoy simulation programming in SimPy!
 
 
 Ports and comparable libraries
 ------------------------------
 
-Reimplementations of SimPy and libraries similar to SimPy are available in the
+Re-implementations of SimPy and libraries similar to SimPy are available in the
 following languages:
 
 - C#: `SimSharp <https://github.com/abeham/SimSharp>`_ (written by Andreas Beham)
 - Julia: `SimJulia <https://github.com/BenLauwens/SimJulia.jl>`_
 - R: `Simmer <https://github.com/r-simmer/simmer>`_
```

### Comparing `simpy-4.0.1/docs/Makefile` & `simpy-4.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/_static/favicon.ico` & `simpy-4.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/_static/simpy-logo-quad.png` & `simpy-4.0.2/docs/_static/simpy-logo-quad.png`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/_static/simpy-logo-small.png` & `simpy-4.0.2/docs/_static/simpy-logo-small.png`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/_static/simpy-logo.png` & `simpy-4.0.2/docs/_static/simpy-logo.png`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/_static/simpy-logo.svg` & `simpy-4.0.2/docs/_static/simpy-logo.svg`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/about/acknowledgements.rst` & `simpy-4.0.2/docs/about/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/about/defense_of_design.rst` & `simpy-4.0.2/docs/about/defense_of_design.rst`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 *process execution method* (or PEM in short). A PEM interacted with the
 simulation by yielding one of several keywords defined in the simulation
 package.
 
 The simulation itself was executed via module level functions. The simulation
 state was stored in the global scope. This made it very easy to implement and
 execute a simulation (despite from having to inherit from *Process* and
-instantianting the processes before starting their PEMs). However, having all
+instantiating the processes before starting their PEMs). However, having all
 simulation state global makes it hard to parallelize multiple simulations.
 
 SimPy 1 also followed the "batteries included" approach, providing shared
 resources, monitoring, plotting, GUIs and multiple types of simulations
 ("normal", real-time, manual stepping, with tracing).
 
 The following code fragment shows how a simple simulation could be implemented
@@ -55,15 +55,15 @@
     sim.activate(proc, proc.pem(3))
     sim.simulate(until=10)
 
 
 Changes in SimPy 2
 ==================
 
-SimPy 2 mostly sticked with SimPy 1's design, but added an object orient API
+SimPy 2 mostly stuck with SimPy 1's design, but added an object orient API
 for the execution of simulations, allowing them to be executed in parallel.
 Since processes and the simulation state were so closely coupled, you now
 needed to pass the ``Simulation`` instance into your process to "bind" them to
 that instance. Additionally, you still had to activate the process. If you
 forgot to pass the simulation instance, the process would use a global instance
 thereby breaking your program. SimPy 2's OO-API looked like this:
 
@@ -218,9 +218,9 @@
 .. code-block:: python
 
     class Environment(object):
         def __init__(self):
             self.event = types.MethodType(Event, self)
 
 It turned out the the class attributes (the ``BoundClass`` instances) were now
-quite useless, so we removed them allthough it was actually the "right" way to
+quite useless, so we removed them although it was actually the "right" way to
 to add classes as methods to another class.
```

### Comparing `simpy-4.0.1/docs/about/history.rst` & `simpy-4.0.2/docs/about/history.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,27 +119,27 @@
 backward compatible.
 
 Documentation format changes
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 SimPy's documentation has been restructured and processed by the Sphinx
 documentation generation tool. This has generated one coherent, well
-structured document which can be easily browsed. A seach capability is included.
+structured document which can be easily browsed. A search capability is included.
 
 
 March 2008: Version 1.9.1
 --------------------------
 
 This is a bug-fix release which cures the following bugs:
 
 - Excessive production of circular garbage, due to a circular reference
   between Process instances and event notices. This led to large memory
   requirements.
 
-- Runtime error for preempts of proceeses holding multiple Resource objects.
+- Runtime error for preempts of processes holding multiple Resource objects.
 
 It also adds a Short Manual, describing only the basic facilities of SimPy.
 
 December 2007: Version 1.9
 --------------------------
 
 This is a major release with added functionality/new user API calls and bug
@@ -267,15 +267,15 @@
   + *yield put* for putting items into a buffer, and
 
   + *yield get* for getting items from a buffer.
 
 - The Manual has undergone a major re-write/edit.
 
 - All scripts have been restructured for compatibility with IronPython 1 beta2.
-  This was doen by moving all *import* statements to the beginning of the
+  This was done by moving all *import* statements to the beginning of the
   scripts. After the removal of the first (shebang) line, all scripts (with the
   exception of plotting and GUI scripts) can run successfully under this new
   Python implementation.
 
 September 2005: Version 1.6.1
 -----------------------------
 
@@ -492,15 +492,15 @@
 
 
 27 September 2002
 -----------------
 
 * Version 0.2 Alpha-release, intended to attract feedback from users
 * Extended list of models
-* Upodated documentation
+* Updated documentation
 
 17 September 2002
 -----------------
 
 * Version 0.1.2 published on SourceForge; fully working, pre-alpha code
 * Implements simulation, shared resources with queuing (FIFO), and monitors
   for data gathering/analysis.
```

### Comparing `simpy-4.0.1/docs/about/release_process.rst` & `simpy-4.0.2/docs/about/release_process.rst`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Preparations
 ============
 
 #. Close all `tickets for the next version
    <https://gitlab.com/team-simpy/simpy/-/issues>`_.
 
-#. Update the *minium* required versions of dependencies in :file:`setup.cfg`.
+#. Update the *minimum* required versions of dependencies in :file:`setup.cfg`.
    Update the development dependencies in :file:`requirements-dev.txt`.
 
 #. Run :command:`tox` from the project root. All tests for all supported
    versions must pass:
 
    .. code-block:: console
```

### Comparing `simpy-4.0.1/docs/api_reference/simpy.events.rst` & `simpy-4.0.2/docs/api_reference/simpy.events.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/api_reference/simpy.resources.rst` & `simpy-4.0.2/docs/api_reference/simpy.resources.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/api_reference/simpy.rt.rst` & `simpy-4.0.2/docs/api_reference/simpy.rt.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/conf.py` & `simpy-4.0.2/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,23 @@
 # serve to show the default.
 
 import datetime
 import os
 import sys
 import typing
 
+# HACK: these imports are a workaround for
+# https://github.com/sphinx-doc/sphinx/issues/9243
+import sphinx.builders.html
+import sphinx.builders.latex
+import sphinx.builders.linkcheck
+import sphinx.builders.texinfo
+import sphinx.builders.text
+import sphinx.ext.autodoc  # noqa
+
 # This is used to allow the type checking stubs for various BoundClass methods
 # to be used in the Sphinx documentation in place of the true BoundClass
 # instance attributes. The 'SPHINX' value is used to distinguish sphinx-time
 # versus real type checking-time so that circular imports may still be avoided.
 typing.TYPE_CHECKING = 'SPHINX'
 
 # If extensions (or modules to document with autodoc) are in another directory,
@@ -38,14 +47,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.doctest',
     'sphinx.ext.intersphinx',
+    'sphinx_rtd_theme',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
@@ -106,20 +116,15 @@
 # modindex_common_prefix = []
 
 
 # -- Options for HTML output --------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-try:
-    import sphinx_rtd_theme
-    html_theme = 'sphinx_rtd_theme'
-    html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
-except ImportError:
-    html_theme = 'default'
+html_theme = 'sphinx_rtd_theme'
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 # html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
@@ -241,13 +246,11 @@
 # (source start file, name, description, authors, manual section).
 man_pages = [
     ('index', 'simpy', 'SimPy Documentation', [', '.join(authors)], 1),
 ]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {
-    'http://docs.python.org/3/': None,
-}
+intersphinx_mapping = {'python': ('https://docs.python.org/3', None)}
 
 # Autodoc
 autodoc_member_order = 'bysource'
```

### Comparing `simpy-4.0.1/docs/conftest.py` & `simpy-4.0.2/docs/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 This module scans all ``*.rst`` files below ``docs/`` for example code.
-Example code is discoved by checking for lines containing the ``..
-literalinclude:: `` directives.
+Example code is discovered by checking for lines containing the ``..
+literals include:: `` directives.
 
-An example consists of two consecutive literalinclude directives. The
+An example consists of two consecutive literals include directives. The
 first must include a ``*.py`` file and the second a ``*.out`` file. The
 ``*.py`` file consists of the example code which is executed in
 a separate process. The output of this process is compared to the
 contents of the ``*.out`` file.
 
 """
+import pathlib
 import subprocess
 import sys
 
 from _pytest.assertion.util import _diff_text
 from py._code.code import TerminalRepr
 import pytest
 
 
 def pytest_collect_file(path, parent):
     """Checks if the file is a rst file and creates an
     :class:`ExampleFile` instance."""
     if path.ext == '.py' and path.dirname.endswith('code'):
-        return ExampleFile.from_parent(parent, fspath=path)
+        return ExampleFile.from_parent(parent, path=pathlib.Path(path.strpath))
 
 
 class ExampleFile(pytest.File):
     """Represents an example ``.py`` and its output ``.out``."""
 
     def collect(self):
         pyfile = self.fspath
@@ -61,15 +62,15 @@
         if exc_info.errisinstance(ValueError):
             # Output is mismatching. Create a nice diff as failure description.
             expected, output = exc_info.value.args
             message = _diff_text(output, expected)
             return ReprFailExample(self.pyfile, self.outfile, message)
 
         elif exc_info.errisinstance(subprocess.CalledProcessError):
-            # Something wrent wrong while executing the example.
+            # Something went wrong while executing the example.
             return ReprErrorExample(self.pyfile, exc_info)
 
         else:
             # Something went terribly wrong :(
             return pytest.Item.repr_failure(self, exc_info)
 
     def reportinfo(self):
```

### Comparing `simpy-4.0.1/docs/examples/bank_renege.rst` & `simpy-4.0.2/docs/examples/bank_renege.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/carwash.rst` & `simpy-4.0.2/docs/examples/carwash.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 limited number of washing machines. It also defines a process for washing
 a car.
 
 When a car arrives at the carwash, it requests a machine. Once it got one, it
 starts the carwash's *wash* processes and waits for it to finish. It finally
 releases the machine and leaves.
 
-The cars are generated by a *setup* process. After creating an intial amount of
+The cars are generated by a *setup* process. After creating an initial amount of
 cars it creates new *car* processes after a random time interval as long as the
 simulation continues.
 
 .. literalinclude:: code/carwash.py
 
 The simulation's output:
```

### Comparing `simpy-4.0.1/docs/examples/code/bank_renege.py` & `simpy-4.0.2/docs/examples/code/bank_renege.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/code/carwash.out` & `simpy-4.0.2/docs/examples/code/carwash.out`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/code/carwash.py` & `simpy-4.0.2/docs/examples/code/carwash.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Scenario:
   A carwash has a limited number of washing machines and defines
   a washing processes that takes some (random) time.
 
   Car processes arrive at the carwash at a random time. If one washing
   machine is available, they start the washing process and wait for it
-  to finish. If not, they wait until they an use one.
+  to finish. If not, they wait until they can use one.
 
 """
 import random
 
 import simpy
 
 
@@ -40,15 +40,15 @@
         self.env = env
         self.machine = simpy.Resource(env, num_machines)
         self.washtime = washtime
 
     def wash(self, car):
         """The washing processes. It takes a ``car`` processes and tries
         to clean it."""
-        yield self.env.timeout(WASHTIME)
+        yield self.env.timeout(self.washtime)
         print("Carwash removed %d%% of %s's dirt." %
               (random.randint(50, 99), car))
 
 
 def car(env, name, cw):
     """The car process (each car has a ``name``) arrives at the carwash
     (``cw``) and requests a cleaning machine.
@@ -83,15 +83,15 @@
         i += 1
         env.process(car(env, 'Car %d' % i, carwash))
 
 
 # Setup and start the simulation
 print('Carwash')
 print('Check out http://youtu.be/fXXmeP9TvBg while simulating ... ;-)')
-random.seed(RANDOM_SEED)  # This helps reproducing the results
+random.seed(RANDOM_SEED)  # This helps to reproduce the results
 
 # Create an environment and start the setup process
 env = simpy.Environment()
 env.process(setup(env, NUM_MACHINES, WASHTIME, T_INTER))
 
 # Execute!
 env.run(until=SIM_TIME)
```

### Comparing `simpy-4.0.1/docs/examples/code/gas_station_refuel.py` & `simpy-4.0.2/docs/examples/code/gas_station_refuel.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,85 +20,84 @@
 import itertools
 import random
 
 import simpy
 
 
 RANDOM_SEED = 42
-GAS_STATION_SIZE = 200     # liters
-THRESHOLD = 10             # Threshold for calling the tank truck (in %)
-FUEL_TANK_SIZE = 50        # liters
-FUEL_TANK_LEVEL = [5, 25]  # Min/max levels of fuel tanks (in liters)
-REFUELING_SPEED = 2        # liters / second
-TANK_TRUCK_TIME = 300      # Seconds it takes the tank truck to arrive
-T_INTER = [30, 300]        # Create a car every [min, max] seconds
-SIM_TIME = 1000            # Simulation time in seconds
+STATION_TANK_SIZE = 200    # Size of the gas station tank (liters)
+THRESHOLD = 25             # Station tank minimum level (% of full)
+CAR_TANK_SIZE = 50         # Size of car fuel tanks (liters)
+CAR_TANK_LEVEL = [5, 25]   # Min/max levels of car fuel tanks (liters)
+REFUELING_SPEED = 2        # Rate of refuelling car fuel tank (liters / second)
+TANK_TRUCK_TIME = 300      # Time it takes tank truck to arrive (seconds)
+T_INTER = [30, 300]        # Interval between car arrivals [min, max] (seconds)
+SIM_TIME = 1000            # Simulation time (seconds)
 
 
-def car(name, env, gas_station, fuel_pump):
+def car(name, env, gas_station, station_tank):
     """A car arrives at the gas station for refueling.
 
     It requests one of the gas station's fuel pumps and tries to get the
-    desired amount of gas from it. If the stations reservoir is
+    desired amount of fuel from it. If the station's fuel tank is
     depleted, the car has to wait for the tank truck to arrive.
 
     """
-    fuel_tank_level = random.randint(*FUEL_TANK_LEVEL)
-    print('%s arriving at gas station at %.1f' % (name, env.now))
+    car_tank_level = random.randint(*CAR_TANK_LEVEL)
+    print('%6.1f s: %s arrived at gas station' % (env.now, name))
     with gas_station.request() as req:
-        start = env.now
         # Request one of the gas pumps
         yield req
 
         # Get the required amount of fuel
-        liters_required = FUEL_TANK_SIZE - fuel_tank_level
-        yield fuel_pump.get(liters_required)
+        fuel_required = CAR_TANK_SIZE - car_tank_level
+        yield station_tank.get(fuel_required)
 
         # The "actual" refueling process takes some time
-        yield env.timeout(liters_required / REFUELING_SPEED)
+        yield env.timeout(fuel_required / REFUELING_SPEED)
 
-        print('%s finished refueling in %.1f seconds.' % (name,
-                                                          env.now - start))
+        print('%6.1f s: %s refueled with %.1f liters'
+              % (env.now, name, fuel_required))
 
 
-def gas_station_control(env, fuel_pump):
-    """Periodically check the level of the *fuel_pump* and call the tank
+def gas_station_control(env, station_tank):
+    """Periodically check the level of the gas station tank and call the tank
     truck if the level falls below a threshold."""
     while True:
-        if fuel_pump.level / fuel_pump.capacity * 100 < THRESHOLD:
+        if station_tank.level / station_tank.capacity * 100 < THRESHOLD:
             # We need to call the tank truck now!
-            print('Calling tank truck at %d' % env.now)
-            # Wait for the tank truck to arrive and refuel the station
-            yield env.process(tank_truck(env, fuel_pump))
+            print('%6.1f s: Calling tank truck' % env.now)
+            # Wait for the tank truck to arrive and refuel the station tank
+            yield env.process(tank_truck(env, station_tank))
 
         yield env.timeout(10)  # Check every 10 seconds
 
 
-def tank_truck(env, fuel_pump):
+def tank_truck(env, station_tank):
     """Arrives at the gas station after a certain delay and refuels it."""
     yield env.timeout(TANK_TRUCK_TIME)
-    print('Tank truck arriving at time %d' % env.now)
-    ammount = fuel_pump.capacity - fuel_pump.level
-    print('Tank truck refuelling %.1f liters.' % ammount)
-    yield fuel_pump.put(ammount)
+    amount = station_tank.capacity - station_tank.level
+    station_tank.put(amount)
+    print('%6.1f s: Tank truck arrived and'
+          ' refuelled station with %.1f liters' % (env.now, amount))
 
 
-def car_generator(env, gas_station, fuel_pump):
+def car_generator(env, gas_station, station_tank):
     """Generate new cars that arrive at the gas station."""
     for i in itertools.count():
         yield env.timeout(random.randint(*T_INTER))
-        env.process(car('Car %d' % i, env, gas_station, fuel_pump))
+        env.process(car('Car %d' % i, env, gas_station, station_tank))
 
 
 # Setup and start the simulation
 print('Gas Station refuelling')
 random.seed(RANDOM_SEED)
 
 # Create environment and start processes
 env = simpy.Environment()
 gas_station = simpy.Resource(env, 2)
-fuel_pump = simpy.Container(env, GAS_STATION_SIZE, init=GAS_STATION_SIZE)
-env.process(gas_station_control(env, fuel_pump))
-env.process(car_generator(env, gas_station, fuel_pump))
+station_tank = simpy.Container(env, STATION_TANK_SIZE, init=STATION_TANK_SIZE)
+env.process(gas_station_control(env, station_tank))
+env.process(car_generator(env, gas_station, station_tank))
 
 # Execute!
 env.run(until=SIM_TIME)
```

### Comparing `simpy-4.0.1/docs/examples/code/latency.out` & `simpy-4.0.2/docs/examples/code/latency.out`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/code/latency.py` & `simpy-4.0.2/docs/examples/code/latency.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/code/machine_shop.py` & `simpy-4.0.2/docs/examples/code/machine_shop.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - Resources: PreemptiveResource
 
 Scenario:
   A workshop has *n* identical machines. A stream of jobs (enough to
   keep the machines busy) arrives. Each machine breaks down
   periodically. Repairs are carried out by one repairman. The repairman
   has other, less important tasks to perform, too. Broken machines
-  preempt theses tasks. The repairman continues them when he is done
+  preempt these tasks. The repairman continues them when he is done
   with the machine repair. The workshop works continuously.
 
 """
 import random
 
 import simpy
 
@@ -44,15 +44,15 @@
 
 class Machine(object):
     """A machine produces parts and my get broken every now and then.
 
     If it breaks, it requests a *repairman* and continues the production
     after the it is repaired.
 
-    A machine has a *name* and a numberof *parts_made* thus far.
+    A machine has a *name* and a number of *parts_made* thus far.
 
     """
     def __init__(self, env, name, repairman):
         self.env = env
         self.name = name
         self.parts_made = 0
         self.broken = False
@@ -104,36 +104,36 @@
 def other_jobs(env, repairman):
     """The repairman's other (unimportant) job."""
     while True:
         # Start a new job
         done_in = JOB_DURATION
         while done_in:
             # Retry the job until it is done.
-            # It's priority is lower than that of machine repairs.
+            # Its priority is lower than that of machine repairs.
             with repairman.request(priority=2) as req:
                 yield req
                 try:
                     start = env.now
                     yield env.timeout(done_in)
                     done_in = 0
                 except simpy.Interrupt:
                     done_in -= env.now - start
 
 
 # Setup and start the simulation
 print('Machine shop')
-random.seed(RANDOM_SEED)  # This helps reproducing the results
+random.seed(RANDOM_SEED)  # This helps to reproduce the results
 
 # Create an environment and start the setup process
 env = simpy.Environment()
 repairman = simpy.PreemptiveResource(env, capacity=1)
 machines = [Machine(env, 'Machine %d' % i, repairman)
             for i in range(NUM_MACHINES)]
 env.process(other_jobs(env, repairman))
 
 # Execute!
 env.run(until=SIM_TIME)
 
-# Analyis/results
+# Analysis/results
 print('Machine shop results after %s weeks' % WEEKS)
 for machine in machines:
     print('%s made %d parts.' % (machine.name, machine.parts_made))
```

### Comparing `simpy-4.0.1/docs/examples/code/movie_renege.py` & `simpy-4.0.2/docs/examples/code/movie_renege.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     If at most one ticket is left after the moviegoer bought her
     tickets, the *sold out* event for this movie is triggered causing
     all remaining moviegoers to leave.
 
     """
     with theater.counter.request() as my_turn:
-        # Wait until its our turn or until the movie is sold out
+        # Wait until it's our turn or until the movie is sold out
         result = yield my_turn | theater.sold_out[movie]
 
         # Check if it's our turn or if movie is sold out
         if my_turn not in result:
             theater.num_renegers[movie] += 1
             return
```

### Comparing `simpy-4.0.1/docs/examples/code/process_communication.out` & `simpy-4.0.2/docs/examples/code/process_communication.out`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/code/process_communication.py` & `simpy-4.0.2/docs/examples/code/process_communication.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/gas_station_refuel.rst` & `simpy-4.0.2/docs/examples/gas_station_refuel.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/index.rst` & `simpy-4.0.2/docs/examples/index.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/latency.rst` & `simpy-4.0.2/docs/examples/latency.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/machine_shop.rst` & `simpy-4.0.2/docs/examples/machine_shop.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/movie_renege.rst` & `simpy-4.0.2/docs/examples/movie_renege.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/examples/process_communication.rst` & `simpy-4.0.2/docs/examples/process_communication.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/index.rst` & `simpy-4.0.2/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 .. only:: html
 
     .. figure:: _static/simpy-logo-small.png
         :align: center
 
         Discrete event simulation for Python
 
-        `News <https://plus.google.com/101634625602509193865>`_ |
         `PyPI <https://pypi.python.org/pypi/simpy>`_ |
         `GitLab <https://gitlab.com/team-simpy/simpy/>`_ |
         `Issues
         <https://gitlab.com/groups/team-simpy/-/issues>`_ |
         `Mailing list <https://groups.google.com/forum/#!forum/python-simpy>`_
 
 ========
```

### Comparing `simpy-4.0.1/docs/make.bat` & `simpy-4.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/simpy_intro/basic_concepts.rst` & `simpy-4.0.2/docs/simpy_intro/basic_concepts.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 processes live in an *environment*. They interact with the environment and with
 each other via *events*.
 
 Processes are described by simple Python `generators
 <http://docs.python.org/3/reference/expressions.html#yieldexpr>`_. You can call
 them *process function* or *process method*, depending on whether it is
 a normal function or method of a class. During their lifetime, they create
-events and ``yield`` them in order to wait for them to be triggered.
+events and ``yield`` them in order to wait for them to occur.
 
 When a process yields an event, the process gets *suspended*. SimPy *resumes*
-the process, when the event occurs (we say that the event is *triggered*).
+the process, when the event occurs (we say that the event is *processed*).
 Multiple processes can wait for the same event. SimPy resumes them in the same
 order in which they yielded that event.
 
 An important event type is the :class:`~simpy.events.Timeout`. Events of this
-type are triggered after a certain amount of (simulated) time has passed. They
-allow a process to sleep (or hold its state) for the given time.
+type occur (are processed) after a certain amount of (simulated) time has
+passed. They allow a process to sleep (or hold its state) for the given time.
 A :class:`~simpy.events.Timeout` and all other events can be created by calling
 the appropriate method of the :class:`Environment` that the process lives in
 (:meth:`Environment.timeout()` for example).
 
 
 Our First Process
 =================
@@ -49,15 +49,15 @@
     ...         trip_duration = 2
     ...         yield env.timeout(trip_duration)
 
 Our *car* process requires a reference to an :class:`Environment` (``env``) in
 order to create new events. The *car*'s behavior is described in an infinite
 loop. Remember, this function is a generator. Though it will never terminate,
 it will pass the control flow back to the simulation once a ``yield`` statement
-is reached. Once the yielded event is triggered ("it occurs"), the simulation
+is reached. Once the yielded event is processed ("it occurs"), the simulation
 will resume the function at this statement.
 
 As I said before, our car switches between the states *parking* and *driving*.
 It announces its new state by printing a message and the current simulation
 time (as returned by the :attr:`Environment.now` property). It then calls the
 :meth:`Environment.timeout()` factory function to create
 a :class:`~simpy.events.Timeout` event. This event describes the point in time
```

### Comparing `simpy-4.0.1/docs/simpy_intro/how_to_proceed.rst` & `simpy-4.0.2/docs/simpy_intro/how_to_proceed.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/simpy_intro/installation.rst` & `simpy-4.0.2/docs/simpy_intro/installation.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/simpy_intro/process_interaction.rst` & `simpy-4.0.2/docs/simpy_intro/process_interaction.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/simpy_intro/shared_resources.rst` & `simpy-4.0.2/docs/simpy_intro/shared_resources.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/topical_guides/environments.rst` & `simpy-4.0.2/docs/topical_guides/environments.rst`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 and is increased via :class:`~simpy.events.Timeout` events.
 
 By default, ``now`` starts at 0, but you can pass an ``initial_time`` to the
 :class:`Environment` to use something else.
 
 .. note::
 
-   Although the simulation time is technically unitless, you can pretend that
+   Although the simulation time is technically unit-less, you can pretend that
    it is, for example, in seconds and use it like a timestamp returned by
    :func:`time.time()` to calculate a date or the day of the week.
 
 The property :attr:`Environment.active_process` is comparable to
 :func:`os.getpid()` and is either ``None`` or pointing at the currently active
 :class:`~simpy.events.Process`. A process is *active* when its process function
 is being executed. It becomes *inactive* (or suspended) when it yields an
```

### Comparing `simpy-4.0.1/docs/topical_guides/events.rst` & `simpy-4.0.2/docs/topical_guides/events.rst`

 * *Files 2% similar despite different names*

```diff
@@ -116,16 +116,18 @@
 and pass an :class:`Exception` instance to it (e.g., the exception you caught
 during your failed computation).
 
 There is also a generic way to trigger an event: ``Event.trigger(event)``.
 This will take the value and outcome (success or failure) of the event passed
 to it.
 
-All three methods return the event instance they are bound to. This allows you
-to do things like ``yield Event(env).succeed()``.
+``Event.succeed()`` and ``Event.fail()`` methods return the event instance they
+are bound to. This allows you to do things like ``yield Event(env).succeed()``.
+
+``Event.trigger()`` returns None.
 
 
 Example usages for ``Event``
 ============================
 
 The simple mechanics outlined above provide a great flexibility in the way
 events (even the basic :class:`Event`) can be used.
```

### Comparing `simpy-4.0.1/docs/topical_guides/index.rst` & `simpy-4.0.2/docs/topical_guides/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,9 +19,9 @@
    resources
    real-time-simulations
    monitoring
    time_and_scheduling
    porting_from_simpy3
    porting_from_simpy2
 
-.. - analyzing results (numpy, matploblib, ...)
+.. - analyzing results (numpy, matplotlib, ...)
 .. - integration with guis
```

### Comparing `simpy-4.0.1/docs/topical_guides/monitoring.rst` & `simpy-4.0.2/docs/topical_guides/monitoring.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/topical_guides/porting_from_simpy2.rst` & `simpy-4.0.2/docs/topical_guides/porting_from_simpy2.rst`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
 .. code-block:: python
 
     yield env.timeout(duration)        # hold: renamed
     yield env.event()                  # passivate: renamed
     yield resource.request()           # Request is now bound to class Resource
     resource.release()                 # Release no longer needs to be yielded
     yield event                        # waitevent: just yield the event
-    yield env.all_of([event_a, event_b, event_c])  # waitvent
+    yield env.all_of([event_a, event_b, event_c])  # waitevent
     yield env.any_of([event_a, event_b, event_c])  # queuevent
     yield container.get(amount)        # Level is now called Container
     yield container.put(amount)
 
     yield event_a | event_b            # Wait for either a or b. This is new.
     yield event_a & event_b            # Wait for a and b. This is new.
     yield env.process(calculation(env))  # Wait for the process calculation to
```

### Comparing `simpy-4.0.1/docs/topical_guides/porting_from_simpy3.rst` & `simpy-4.0.2/docs/topical_guides/porting_from_simpy3.rst`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
    No change is required for generators that do not return a value or that do
    not have control flow that requires returning early. This is the most common
    case for process generators used with SimPy.
 
 Once a SimPy 3 application is ported to run with Python 3, it may then replace
 any uses of ``Environment.exit(value)`` and ``raise StopProcess(value)`` with
-``return value``. Once all occurences are changed, the application will be ready
+``return value``. Once all occurrences are changed, the application will be ready
 to run with SimPy 4.
 
 Example: Return from Generator
 ------------------------------
 
 In the following example, ``Environment.exit()`` is used to return the first the
 first "needle" from a store of items. When using SimPy 3 with Python 2, this is
@@ -85,15 +85,15 @@
            item = yield store.get()
            if is_needle(item):
                env.exit(item)  # Python2 generators cannot use return
 
    def proc(env, store):
        needle = yield env.process(find_first_needle(env, store))
 
-In SimPy 4 or whith SimPy 3 and Python 3, ``find_first_needle()`` can be
+In SimPy 4 or with SimPy 3 and Python 3, ``find_first_needle()`` can be
 rewritten as:
 
 .. code-block:: python
 
    def find_first_needle(env, store):
        while True:
            item = yield store.get()
```

### Comparing `simpy-4.0.1/docs/topical_guides/process_interaction.rst` & `simpy-4.0.2/docs/topical_guides/process_interaction.rst`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 
 .. _waiting-for-another-process-to-terminate:
 
 Waiting for another process to terminate
 ========================================
 
 The example above has a problem: it may happen that the vehicle wants to park
-for a shorter duration than it takes to charge the battery (this is the case if
-both charging and parking would take 60 to 90 minutes).
+for a shorter duration than it takes to charge the battery, since the minimum
+park time of 60 minutes is less than the maximum charge time of 90 minutes.
 
 To fix this problem we have to slightly change our model. A new ``bat_ctrl()``
 will be started every time the EV starts parking. The EV then waits until the
 parking duration is over *and* until the charging has stopped:
 
 .. code-block:: python
```

### Comparing `simpy-4.0.1/docs/topical_guides/real-time-simulations.rst` & `simpy-4.0.2/docs/topical_guides/real-time-simulations.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/topical_guides/resources.rst` & `simpy-4.0.2/docs/topical_guides/resources.rst`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
      Users: []
      Queued events: []
 
 
 PriorityResource
 ----------------
 
-As you may know from the real world, not every one is equally important. To map
+As you may know from the real world, everything is not equally important. To map
 that to SimPy, there's the *PriorityResource*. This subclass of *Resource* lets
 requesting processes provide a priority for each request. More important
 requests will gain access to the resource earlier than less important ones.
 Priority is expressed by integer numbers; smaller numbers mean a higher
 priority.
 
 Apart from that, it works like a normal *Resource*:
```

### Comparing `simpy-4.0.1/docs/topical_guides/simpy_basics.rst` & `simpy-4.0.2/docs/topical_guides/simpy_basics.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/docs/topical_guides/time_and_scheduling.rst` & `simpy-4.0.2/docs/topical_guides/time_and_scheduling.rst`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/setup.cfg` & `simpy-4.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 author = Ontje Lünsdorf, Stefan Scherfke
 author_email = the_com@gmx.de, stefan@sofa-rockers.org
 description = Event discrete, process based simulation for Python.
 long_description = file: README.rst, CHANGES.rst, AUTHORS.rst
 long_description_content_type = text/x-rst
 url = https://simpy.readthedocs.io
 license = MIT License
-license_file = LICENSE.rst
+license_files = LICENSE.rst,
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Education
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Scientific/Engineering
 
 [options]
 include_package_data = True
 zip_safe = False
```

### Comparing `simpy-4.0.1/src/simpy/__init__.py` & `simpy-4.0.2/src/simpy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,53 @@
 """
 The ``simpy`` module aggregates SimPy's most used components into a single
 namespace. This is purely for convenience. You can of course also access
 everything (and more!) via their actual submodules.
 
-The following tables list all of the available components in this module.
+The following tables list all the available components in this module.
 
 {toc}
 
 """
 from pkg_resources import get_distribution
 from pkgutil import extend_path
-from typing import List, Tuple, Type
+from typing import Tuple, Type
 
 from simpy.core import Environment
 from simpy.rt import RealtimeEnvironment
 from simpy.exceptions import SimPyException, Interrupt
 from simpy.events import Event, Timeout, Process, AllOf, AnyOf
 from simpy.resources.resource import (
     Resource, PriorityResource, PreemptiveResource)
 from simpy.resources.container import Container
 from simpy.resources.store import (
     Store, PriorityItem, PriorityStore, FilterStore)
 
+__all__ = [
+    'AllOf',
+    'AnyOf',
+    'Container',
+    'Environment',
+    'Event',
+    'FilterStore',
+    'Interrupt',
+    'PreemptiveResource',
+    'PriorityItem',
+    'PriorityResource',
+    'PriorityStore',
+    'Process',
+    'RealtimeEnvironment',
+    'Resource',
+    'SimPyException',
+    'Store',
+    'Timeout',
+]
 
-def compile_toc(
+
+def _compile_toc(
     entries: Tuple[Tuple[str, Tuple[Type, ...]], ...],
     section_marker: str = '=',
 ) -> str:
     """Compiles a list of sections with objects into sphinx formatted
     autosummary directives."""
     toc = ''
     for section, objs in entries:
@@ -36,15 +56,15 @@
         toc += f'{section_marker * len(section)}\n\n'
         toc += '.. autosummary::\n\n'
         for obj in objs:
             toc += f'    ~{obj.__module__}.{obj.__name__}\n'
     return toc
 
 
-toc = (
+_toc = (
     ('Environments', (
         Environment, RealtimeEnvironment,
     )),
     ('Events', (
         Event, Timeout, Process, AllOf, AnyOf, Interrupt,
     )),
     ('Resources', (
@@ -52,14 +72,14 @@
         PriorityItem, PriorityStore, FilterStore,
     )),
     ('Exceptions', (
         SimPyException, Interrupt
     )),
 )
 
-# Use the toc to keep the documentation and the implementation in sync.
+# Use the _toc to keep the documentation and the implementation in sync.
 if __doc__:
-    __doc__ = __doc__.format(toc=compile_toc(toc))
-__all__ = [obj.__name__ for section, objs in toc for obj in objs]
+    __doc__ = __doc__.format(toc=_compile_toc(_toc))
+    assert set(__all__) == {obj.__name__ for _, objs in _toc for obj in objs}
 
-__path__: List[str] = list(extend_path(__path__, __name__))
+__path__ = list(extend_path(__path__, __name__))
 __version__: str = get_distribution('simpy').version
```

### Comparing `simpy-4.0.1/src/simpy/core.py` & `simpy-4.0.2/src/simpy/core.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/src/simpy/events.py` & `simpy-4.0.2/src/simpy/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
 
 EventCallback = Callable[[Event], None]
 EventCallbacks = List[EventCallback]
 
 
 class Timeout(Event):
-    """A :class:`~simpy.events.Event` that gets triggered after a *delay* has
+    """A :class:`~simpy.events.Event` that gets processed after a *delay* has
     passed.
 
     This event is automatically triggered when it is created.
 
 
     """
 
@@ -255,15 +255,15 @@
         # NOTE: The following initialization code is inlined from
         # Event.__init__() for performance reasons.
         self.env = env
         self.callbacks: EventCallbacks = [process._resume]
         self._value: Any = None
 
         # The initialization events needs to be scheduled as urgent so that it
-        # will be handled before interrupts. Otherwise a process whose
+        # will be handled before interrupts. Otherwise, a process whose
         # generator has not yet been started could be interrupted.
         self._ok = True
         env.schedule(self, URGENT)
 
 
 class Interruption(Event):
     """Immediately schedules an :class:`~simpy.exceptions.Interrupt` exception
@@ -327,15 +327,15 @@
     """
 
     def __init__(self, env: 'Environment', generator: ProcessGenerator):
         if not hasattr(generator, 'throw'):
             # Implementation note: Python implementations differ in the
             # generator types they provide. Cython adds its own generator type
             # in addition to the CPython type, which renders a type check
-            # impractical. To workaround this issue, we check for attribute
+            # impractical. To work around this issue, we check for attribute
             # name instead of type and optimistically assume that all objects
             # with a ``throw`` attribute are generators.
             # Remove this workaround if it causes issues in production!
             raise ValueError(f'{generator} is not a generator.')
 
         # NOTE: The following initialization code is inlined from
         # Event.__init__() for performance reasons.
@@ -352,27 +352,27 @@
         gen_name: str = self._generator.__name__  # type: ignore
         return f'{self.__class__.__name__}({gen_name})'
 
     @property
     def target(self) -> Event:
         """The event that the process is currently waiting for.
 
-        Returns ``None`` if the process is dead or it is currently being
+        Returns ``None`` if the process is dead, or it is currently being
         interrupted.
 
         """
         return self._target
 
     @property
     def is_alive(self) -> bool:
         """``True`` until the process generator exits."""
         return self._value is PENDING
 
     def interrupt(self, cause: Optional[Any] = None) -> None:
-        """Interupt this process optionally providing a *cause*.
+        """Interrupt this process optionally providing a *cause*.
 
         A process cannot be interrupted if it already terminated. A process can
         also not interrupt itself. Raise a :exc:`RuntimeError` in these
         cases.
 
         """
         Interruption(self, cause)
@@ -442,17 +442,17 @@
         self._target = event
         self.env._active_proc = None
 
 
 class ConditionValue:
     """Result of a :class:`~simpy.events.Condition`. It supports convenient
     dict-like access to the triggered events and their values. The events are
-    ordered by their occurences in the condition."""
+    ordered by their occurrences in the condition."""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.events: List[Event] = []
 
     def __getitem__(self, key: Event) -> Any:
         if key not in self.events:
             raise KeyError(str(key))
 
         return key._value
```

### Comparing `simpy-4.0.1/src/simpy/exceptions.py` & `simpy-4.0.2/src/simpy/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-SimPy specific exeptions.
+SimPy specific exceptions.
 
 """
 from typing import Any, Optional
 
 
 class SimPyException(Exception):
     """Base class for all SimPy specific exceptions."""
```

### Comparing `simpy-4.0.1/src/simpy/resources/base.py` & `simpy-4.0.2/src/simpy/resources/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,32 +146,32 @@
     - providing custom :attr:`PutQueue` and :attr:`GetQueue` types,
     - providing custom :class:`Put` respectively :class:`Get` events,
     - and implementing the request processing behaviour through the methods
       ``_do_get()`` and ``_do_put()``.
 
     """
 
-    PutQueue: ClassVar[Type[MutableSequence[PutType]]] = list
+    PutQueue: ClassVar[Type[MutableSequence]] = list
     """The type to be used for the :attr:`put_queue`. It is a plain
     :class:`list` by default. The type must support index access (e.g.
     ``__getitem__()`` and ``__len__()``) as well as provide ``append()`` and
     ``pop()`` operations."""
 
-    GetQueue: ClassVar[Type[MutableSequence[GetType]]] = list
+    GetQueue: ClassVar[Type[MutableSequence]] = list
     """The type to be used for the :attr:`get_queue`. It is a plain
     :class:`list` by default. The type must support index access (e.g.
     ``__getitem__()`` and ``__len__()``) as well as provide ``append()`` and
     ``pop()`` operations."""
 
     def __init__(self, env: Environment, capacity: Union[float, int]):
         self._env = env
         self._capacity = capacity
-        self.put_queue = self.PutQueue()
+        self.put_queue: MutableSequence[PutType] = self.PutQueue()
         """Queue of pending *put* requests."""
-        self.get_queue = self.GetQueue()
+        self.get_queue: MutableSequence[GetType] = self.GetQueue()
         """Queue of pending *get* requests."""
 
         # Bind event constructors as methods
         BoundClass.bind_early(self)
 
     @property
     def capacity(self) -> Union[float, int]:
@@ -197,15 +197,15 @@
         get = BoundClass(Get)
 
     def _do_put(self, event: PutType) -> Optional[bool]:
         """Perform the *put* operation.
 
         This method needs to be implemented by subclasses. If the conditions
         for the put *event* are met, the method must trigger the event (e.g.
-        call :meth:`Event.succeed()` with an apropriate value).
+        call :meth:`Event.succeed()` with an appropriate value).
 
         This method is called by :meth:`_trigger_put` for every event in the
         :attr:`put_queue`, as long as the return value does not evaluate
         ``False``.
         """
         raise NotImplementedError(self)
 
@@ -235,15 +235,15 @@
                 break
 
     def _do_get(self, event: GetType) -> Optional[bool]:
         """Perform the *get* operation.
 
         This method needs to be implemented by subclasses. If the conditions
         for the get *event* are met, the method must trigger the event (e.g.
-        call :meth:`Event.succeed()` with an apropriate value).
+        call :meth:`Event.succeed()` with an appropriate value).
 
         This method is called by :meth:`_trigger_get` for every event in the
         :attr:`get_queue`, as long as the return value does not evaluate
         ``False``.
         """
         raise NotImplementedError(self)
```

### Comparing `simpy-4.0.1/src/simpy/resources/container.py` & `simpy-4.0.2/src/simpy/resources/container.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/src/simpy/resources/resource.py` & `simpy-4.0.2/src/simpy/resources/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Shared resources supporting priorities and preemption.
 
 These resources can be used to limit the number of processes using them
 concurrently. A process needs to *request* the usage right to a resource. Once
-the usage right is not needed anymore it has to be *released*. A gas station
+the usage right is not needed any more it has to be *released*. A gas station
 can be modelled as a resource with a limited amount of fuel-pumps. Vehicles
 arrive at the gas station and request to use a fuel-pump. If all fuel-pumps are
 in use, the vehicle needs to wait until one of the users has finished refueling
 and releases its fuel-pump.
 
 These resources can be used by a limited number of processes at a time.
 Processes *request* these resources to become a user and have to *release* them
@@ -33,15 +33,15 @@
 
 from simpy.core import BoundClass, Environment, SimTime
 from simpy.events import Process
 from simpy.resources import base
 
 
 class Preempted:
-    """Cause of an preemption :class:`~simpy.exceptions.Interrupt` containing
+    """Cause of a preemption :class:`~simpy.exceptions.Interrupt` containing
     information about the preemption.
 
     """
 
     def __init__(
         self,
         by: Optional[Process],
@@ -80,15 +80,15 @@
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> Optional[bool]:
         super().__exit__(exc_type, exc_value, traceback)
         # Don't release the resource on generator cleanups. This seems to
-        # create unclaimable circular references otherwise.
+        # create un-claimable circular references otherwise.
         if exc_type is not GeneratorExit:
             self.resource.release(self)
         return None
 
 
 class Release(base.Get):
     """Releases the usage of *resource* granted by *request*. This event is
```

### Comparing `simpy-4.0.1/src/simpy/resources/store.py` & `simpy-4.0.2/src/simpy/resources/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def _do_get(self, event: StoreGet) -> Optional[bool]:
         if self.items:
             event.succeed(self.items.pop(0))
         return None
 
 
 class PriorityItem(NamedTuple):
-    """Wrap an arbitrary *item* with an orderable *priority*.
+    """Wrap an arbitrary *item* with an order-able *priority*.
 
     Pairs a *priority* with an arbitrary *item*. Comparisons of *PriorityItem*
     instances only consider the *priority* attribute, thus supporting use of
     unorderable items in a :class:`PriorityStore` instance.
 
     """
 
@@ -134,17 +134,17 @@
 
 
 class PriorityStore(Store):
     """Resource with *capacity* slots for storing objects in priority order.
 
     Unlike :class:`Store` which provides first-in first-out discipline,
     :class:`PriorityStore` maintains items in sorted order such that
-    the smallest items value are retreived first from the store.
+    the smallest items value are retrieved first from the store.
 
-    All items in a *PriorityStore* instance must be orderable; which is to say
+    All items in a *PriorityStore* instance must be order-able; which is to say
     that items must implement :meth:`~object.__lt__()`. To use unorderable
     items with *PriorityStore*, use :class:`PriorityItem`.
 
     """
 
     def _do_put(self, event: StorePut) -> Optional[bool]:
         if len(self.items) < self._capacity:
```

### Comparing `simpy-4.0.1/src/simpy/rt.py` & `simpy-4.0.2/src/simpy/rt.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/src/simpy/util.py` & `simpy-4.0.2/src/simpy/util.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/src/simpy.egg-info/SOURCES.txt` & `simpy-4.0.2/src/simpy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .gitignore
 .gitlab-ci.yml
+.readthedocs.yaml
 AUTHORS.rst
 CHANGES.rst
 LICENSE.rst
 README.rst
 pyproject.toml
 requirements-dev.txt
 setup.cfg
@@ -11,14 +12,16 @@
 tox.ini
 docs/Makefile
 docs/conf.py
 docs/conftest.py
 docs/contents.rst
 docs/index.rst
 docs/make.bat
+docs/requirements.in
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/simpy-logo-quad.png
 docs/_static/simpy-logo-small.png
 docs/_static/simpy-logo.png
 docs/_static/simpy-logo.svg
 docs/about/acknowledgements.rst
 docs/about/defense_of_design.rst
```

### Comparing `simpy-4.0.1/tests/test_benchmark.py` & `simpy-4.0.2/tests/test_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     env.process(g(env))
     benchmark(env.step)
 
 
 @pytest.mark.benchmark(group='targeted')
 def test_condition_events(env, benchmark):
     def cond_proc(env):
-        yield (env.timeout(0) & (env.timeout(2) | env.timeout(1)))
+        yield env.timeout(0) & (env.timeout(2) | env.timeout(1))
 
     def sim():
         for _ in range(20):
             env.process(cond_proc(env))
         env.run()
 
     benchmark(sim)
```

### Comparing `simpy-4.0.1/tests/test_condition.py` & `simpy-4.0.2/tests/test_condition.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/tests/test_environment.py` & `simpy-4.0.2/tests/test_environment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-General test for the the `simpy.core.Environment`.
+General test for the `simpy.core.Environment`.
 
 """
 # Pytest gets the parameters "env" and "log" from the *conftest.py* file
 import pytest
 
 
 def test_event_queue_empty(env, log):
```

### Comparing `simpy-4.0.1/tests/test_event.py` & `simpy-4.0.2/tests/test_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     env.run()
 
     assert event.value == 'I am the value'
 
 
 def test_unavailable_value(env):
-    """If an event has not yet been triggered, its value is not availabe and
+    """If an event has not yet been triggered, its value is not available and
     trying to access it will result in a AttributeError."""
     event = env.event()
 
     try:
         event.value
         assert False, 'Expected an exception'
     except AttributeError as e:
```

### Comparing `simpy-4.0.1/tests/test_exceptions.py` & `simpy-4.0.2/tests/test_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     event.fail(RuntimeError())
     assert not event.defused, 'Event has been defused immediately'
     env.run(until=1)
     assert event.defused, 'Event has not been defused'
 
 
 def test_process_exception_handling(env):
-    """Processes can't ignore failed events and auto-handle execeptions."""
+    """Processes can't ignore failed events and auto-handle exceptions."""
     def pem(env, event):
         try:
             yield event
             assert False, 'Hey, the event should fail!'
         except RuntimeError:
             pass
 
@@ -248,10 +248,10 @@
         sys.excepthook(*sys.exc_info())
 
         traceback = sys.stderr.getvalue()
 
         sys.stderr = stderr
 
         # Check if frames of process_a and process_b are visible in the
-        # tracebabck.
+        # traceback.
         assert 'process_a' in traceback
         assert 'process_b' in traceback
```

### Comparing `simpy-4.0.1/tests/test_interrupts.py` & `simpy-4.0.2/tests/test_interrupts.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/tests/test_process.py` & `simpy-4.0.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/tests/test_resources.py` & `simpy-4.0.2/tests/test_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,28 +104,28 @@
     env.process(pem(env, res))
     proc = env.process(victim(env, res))
     env.process(interruptor(env, proc))
     env.run()
 
 
 def test_resource_release_after_interrupt(env):
-    """A process needs to release a resource, even it it was interrupted
+    """A process needs to release a resource, even if it was interrupted
     and does not continue to wait for it."""
     def blocker(env, res):
         with res.request() as req:
             yield req
             yield env.timeout(1)
 
     def victim(env, res):
         try:
             evt = res.request()
             yield evt
             pytest.fail('Should not have gotten the resource.')
         except simpy.Interrupt:
-            # Dont wait for the resource
+            # Don't wait for the resource
             res.release(evt)
             assert env.now == 0
 
     def interruptor(env, proc):
         proc.interrupt()
         return 0
         yield
@@ -389,20 +389,20 @@
 
 #
 # Tests for Container
 #
 
 
 def test_container(env, log):
-    """A *container* is a resource (of optinally limited capacity) where
-    you can put in our take out a discrete or continuous amount of
+    """A *container* is a resource (of optionally limited capacity) where
+    you can put in our take-out a discrete or continuous amount of
     things (e.g., a box of lump sugar or a can of milk).  The *put* and
     *get* operations block if the buffer is to full or to empty. If they
-    return, the process nows that the *put* or *get* operation was
-    successfull.
+    return, the process knows that the *put* or *get* operation was
+    successful.
 
     """
     def putter(env, buf, log):
         yield env.timeout(1)
         while True:
             yield buf.put(2)
             log.append(('p', env.now))
@@ -456,15 +456,15 @@
     pytest.raises(ValueError, container.put, -13)
 
 
 @pytest.mark.parametrize(('error', 'args'), [
     (None, [2, 1]),  # normal case
     (None, [1, 1]),  # init == capacity should be valid
     (None, [1, 0]),  # init == 0 should be valid
-    (ValueError, [1, 2]),  # init > capcity
+    (ValueError, [1, 2]),  # init > capacity
     (ValueError, [0]),  # capacity == 0
     (ValueError, [-1]),  # capacity < 0
     (ValueError, [1, -1]),  # init < 0
 ])
 def test_container_init_capacity(env, error, args):
     args.insert(0, env)
     if error:
@@ -477,15 +477,15 @@
 # Tests fore Store
 #
 
 
 def test_store(env):
     """A store models the production and consumption of concrete python
     objects (in contrast to containers, where you only now if the *put*
-    or *get* operations were successfull but don't get concrete
+    or *get* operations were successful but don't get concrete
     objects).
 
     """
     def putter(env, store, item):
         yield store.put(item)
 
     def getter(env, store, orig_item):
```

### Comparing `simpy-4.0.1/tests/test_rt.py` & `simpy-4.0.2/tests/test_rt.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                               'simulation time.')
 
 
 def test_rt_sync(log):
     """Test resetting the internal wall-clock reference time."""
     env = RealtimeEnvironment(factor=0.05)
     env.process(process(env, log, 0.01))
-    sleep(0.06)  # Simulate massiv workload :-)
+    sleep(0.06)  # Simulate massive workload :-)
     env.sync()
     env.run(3)
 
 
 def test_run_with_untriggered_event(env):
     env = RealtimeEnvironment(factor=0.05)
     excinfo = pytest.raises(RuntimeError, env.run, until=env.event())
```

### Comparing `simpy-4.0.1/tests/test_timeout.py` & `simpy-4.0.2/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `simpy-4.0.1/tests/test_util.py` & `simpy-4.0.2/tests/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             assert env.now == 3
 
     env.process(parent(env))
     env.run()
 
 
 def test_subscribe_terminated_proc(env):
-    """subscribe() proc should send a singal immediatly if
+    """subscribe() proc should send a signal immediately if
     "other" has already terminated.
 
     """
     def child(env):
         yield env.timeout(1)
 
     def parent(env):
@@ -290,25 +290,25 @@
         assert values == ['spam', 'eggs']
 
     env.process(parent(env))
     env.run()
 
 
 def test_empty_any_of(env):
-    """AnyOf will triggered immediately if there are no events."""
+    """AnyOf will trigger immediately if there are no events."""
     def parent(env):
         results = yield env.any_of([])
         assert results == {}
 
     env.process(parent(env))
     env.run()
 
 
 def test_empty_all_of(env):
-    """AllOf will triggered immediately if there are no events."""
+    """AllOf will trigger immediately if there are no events."""
     def parent(env):
         results = yield env.all_of([])
         assert results == {}
 
     env.process(parent(env))
     env.run()
```

