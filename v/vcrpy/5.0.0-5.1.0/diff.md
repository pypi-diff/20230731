# Comparing `tmp/vcrpy-5.0.0.tar.gz` & `tmp/vcrpy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcrpy-5.0.0.tar", last modified: Mon Jun 26 21:26:54 2023, max compression
+gzip compressed data, was "vcrpy-5.1.0.tar", last modified: Mon Jul 31 03:18:47 2023, max compression
```

## Comparing `vcrpy-5.0.0.tar` & `vcrpy-5.1.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1063 2023-06-26 14:02:48.000000 vcrpy-5.0.0/LICENSE.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)      142 2023-06-26 14:02:48.000000 vcrpy-5.0.0/MANIFEST.in
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3875 2023-06-26 21:26:54.761739 vcrpy-5.0.0/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2767 2023-06-26 14:02:48.000000 vcrpy-5.0.0/README.rst
--rw-r--r--   0 kevin     (1000) kevin     (1000)      325 2023-06-26 14:02:48.000000 vcrpy-5.0.0/pyproject.toml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       67 2023-06-26 21:26:54.761739 vcrpy-5.0.0/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3503 2023-06-26 17:41:10.000000 vcrpy-5.0.0/setup.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      385 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/assertions.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/migration/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1115 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/new_cassette.json
--rw-r--r--   0 kevin     (1000) kevin     (1000)      599 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/new_cassette.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)       23 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/not_cassette.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1031 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/old_cassette.json
--rw-r--r--   0 kevin     (1000) kevin     (1000)      869 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/migration/old_cassette.yaml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/fixtures/wild/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9705 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/fixtures/wild/domain_redirect.yaml
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/integration/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1214 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/aiohttp_utils.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/integration/cassettes/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1017 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
--rw-r--r--   0 kevin     (1000) kevin     (1000)      781 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/conftest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    16808 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_aiohttp.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2742 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_basic.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2951 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_boto.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3559 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_boto3.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2626 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_config.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1594 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_disksaver.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6426 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_filter.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1030 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_http
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4922 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_httplib2.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10635 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_httpx.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2541 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_ignore.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4000 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      878 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_multiple.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1755 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_proxy.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5170 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_record_mode.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1222 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_register_matcher.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2825 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_register_persister.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      962 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_register_serializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      739 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12531 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_requests.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5052 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12593 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_tornado.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1387 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_tornado_exception_can_be_caught.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1566 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5085 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_urllib2.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6402 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/integration/test_urllib3.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3538 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/integration/test_wild.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/tests/unit/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13542 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_cassettes.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2669 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_errors.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12401 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_filters.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      611 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_json_serializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9990 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1568 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_migration.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1067 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_persist.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2471 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3613 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_response.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3992 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tests/unit/test_serialize.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      840 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5580 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_unittest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    12082 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_vcr.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      395 2023-06-26 14:02:48.000000 vcrpy-5.0.0/tests/unit/test_vcr_import.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3115 2023-06-26 17:41:10.000000 vcrpy-5.0.0/tox.ini
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      296 2023-06-26 17:44:58.000000 vcrpy-5.0.0/vcr/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      125 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/_handle_coroutine.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13958 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/cassette.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    10818 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/config.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1976 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/errors.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6911 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/filters.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4267 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/matchers.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     4639 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/migration.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)    17916 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/patch.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/persisters/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/persisters/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1203 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/persisters/filesystem.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      630 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/record_mode.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3772 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/request.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2124 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serialize.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/serializers/
--rw-r--r--   0 kevin     (1000) kevin     (1000)        0 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2513 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/compat.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      778 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/jsonserializer.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      363 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/serializers/yamlserializer.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcr/stubs/
--rw-r--r--   0 kevin     (1000) kevin     (1000)    13616 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/stubs/__init__.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     9946 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/stubs/aiohttp_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1202 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/boto3_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      235 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/boto_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      578 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/compat.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2166 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/httplib2_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     5579 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/httpx_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      558 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/requests_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3407 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/tornado_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)      504 2023-06-26 14:02:48.000000 vcrpy-5.0.0/vcr/stubs/urllib3_stubs.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1074 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/unittest.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3800 2023-06-26 17:41:10.000000 vcrpy-5.0.0/vcr/util.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-06-26 21:26:54.761739 vcrpy-5.0.0/vcrpy.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3875 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2694 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       65 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/requires.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        4 2023-06-26 21:26:54.000000 vcrpy-5.0.0/vcrpy.egg-info/top_level.txt
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.829178 vcrpy-5.1.0/
+-rw-r--r--   0 kevin      (501) staff       (20)     1063 2022-08-31 19:12:36.000000 vcrpy-5.1.0/LICENSE.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      142 2022-08-31 19:12:36.000000 vcrpy-5.1.0/MANIFEST.in
+-rw-r--r--   0 kevin      (501) staff       (20)     3875 2023-07-31 03:18:47.829253 vcrpy-5.1.0/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2767 2022-08-31 19:12:36.000000 vcrpy-5.1.0/README.rst
+-rw-r--r--   0 kevin      (501) staff       (20)      622 2023-06-28 22:11:37.000000 vcrpy-5.1.0/pyproject.toml
+-rw-r--r--   0 kevin      (501) staff       (20)       67 2023-07-31 03:18:47.829467 vcrpy-5.1.0/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     3495 2023-07-31 03:04:00.000000 vcrpy-5.1.0/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.811968 vcrpy-5.1.0/tests/
+-rw-r--r--   0 kevin      (501) staff       (20)      401 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/assertions.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.810499 vcrpy-5.1.0/tests/fixtures/
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.812559 vcrpy-5.1.0/tests/fixtures/migration/
+-rw-r--r--   0 kevin      (501) staff       (20)     1115 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/migration/new_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      599 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/migration/new_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)       23 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/migration/not_cassette.txt
+-rw-r--r--   0 kevin      (501) staff       (20)     1031 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/migration/old_cassette.json
+-rw-r--r--   0 kevin      (501) staff       (20)      869 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/migration/old_cassette.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.812687 vcrpy-5.1.0/tests/fixtures/wild/
+-rw-r--r--   0 kevin      (501) staff       (20)     9705 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/fixtures/wild/domain_redirect.yaml
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.816138 vcrpy-5.1.0/tests/integration/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/integration/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1214 2023-05-24 18:36:09.000000 vcrpy-5.1.0/tests/integration/aiohttp_utils.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.816272 vcrpy-5.1.0/tests/integration/cassettes/
+-rw-r--r--   0 kevin      (501) staff       (20)     1017 2023-05-24 18:36:09.000000 vcrpy-5.1.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml
+-rw-r--r--   0 kevin      (501) staff       (20)      781 2023-05-26 15:56:05.000000 vcrpy-5.1.0/tests/integration/conftest.py
+-rw-r--r--   0 kevin      (501) staff       (20)    17402 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/integration/test_aiohttp.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2742 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_basic.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2935 2023-07-31 03:03:51.000000 vcrpy-5.1.0/tests/integration/test_boto.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3530 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_boto3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2626 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1594 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_disksaver.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6666 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/integration/test_filter.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1030 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/integration/test_http
+-rw-r--r--   0 kevin      (501) staff       (20)     4922 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_httplib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10568 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_httpx.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2541 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_ignore.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4036 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)      973 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_multiple.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1755 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_proxy.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5358 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1222 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_register_matcher.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2825 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_register_persister.py
+-rw-r--r--   0 kevin      (501) staff       (20)      962 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/integration/test_register_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      739 2023-05-24 18:36:09.000000 vcrpy-5.1.0/tests/integration/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12479 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_requests.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5004 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/integration/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12646 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_tornado.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1387 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/integration/test_tornado_exception_can_be_caught.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     1566 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml
+-rw-r--r--   0 kevin      (501) staff       (20)     5085 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_urllib2.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6411 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_urllib3.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3530 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/integration/test_wild.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.818674 vcrpy-5.1.0/tests/unit/
+-rw-r--r--   0 kevin      (501) staff       (20)    13618 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_cassettes.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2688 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12353 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/unit/test_filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)      611 2023-05-24 18:36:09.000000 vcrpy-5.1.0/tests/unit/test_json_serializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)    11785 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tests/unit/test_matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1568 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1067 2022-08-31 19:12:36.000000 vcrpy-5.1.0/tests/unit/test_persist.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2471 2023-05-24 18:36:09.000000 vcrpy-5.1.0/tests/unit/test_request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3601 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_response.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3992 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_serialize.py
+-rw-r--r--   0 kevin      (501) staff       (20)      840 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5578 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_unittest.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12136 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_vcr.py
+-rw-r--r--   0 kevin      (501) staff       (20)      248 2023-06-28 22:11:37.000000 vcrpy-5.1.0/tests/unit/test_vcr_import.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2127 2023-07-31 03:04:00.000000 vcrpy-5.1.0/tox.ini
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.826780 vcrpy-5.1.0/vcr/
+-rw-r--r--   0 kevin      (501) staff       (20)      270 2023-07-31 03:04:57.000000 vcrpy-5.1.0/vcr/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)       97 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/_handle_coroutine.py
+-rw-r--r--   0 kevin      (501) staff       (20)    13856 2023-07-31 03:04:00.000000 vcrpy-5.1.0/vcr/cassette.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10822 2023-07-31 03:04:00.000000 vcrpy-5.1.0/vcr/config.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1963 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/errors.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6895 2023-07-31 03:04:00.000000 vcrpy-5.1.0/vcr/filters.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6104 2023-07-31 03:04:00.000000 vcrpy-5.1.0/vcr/matchers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4609 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)    17944 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/patch.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.826989 vcrpy-5.1.0/vcr/persisters/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-5.1.0/vcr/persisters/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1203 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/persisters/filesystem.py
+-rw-r--r--   0 kevin      (501) staff       (20)      630 2022-08-31 19:12:36.000000 vcrpy-5.1.0/vcr/record_mode.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3795 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/request.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2125 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/serialize.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.827421 vcrpy-5.1.0/vcr/serializers/
+-rw-r--r--   0 kevin      (501) staff       (20)        0 2022-08-31 19:12:36.000000 vcrpy-5.1.0/vcr/serializers/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2513 2022-08-31 19:12:36.000000 vcrpy-5.1.0/vcr/serializers/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)      504 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/serializers/jsonserializer.py
+-rw-r--r--   0 kevin      (501) staff       (20)      363 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/serializers/yamlserializer.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.828527 vcrpy-5.1.0/vcr/stubs/
+-rw-r--r--   0 kevin      (501) staff       (20)    13637 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/stubs/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     9862 2023-07-31 03:04:00.000000 vcrpy-5.1.0/vcr/stubs/aiohttp_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1202 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/stubs/boto3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      235 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/stubs/boto_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      578 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/stubs/compat.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2166 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/stubs/httplib2_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5579 2023-05-24 18:36:09.000000 vcrpy-5.1.0/vcr/stubs/httpx_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      558 2023-05-26 15:56:05.000000 vcrpy-5.1.0/vcr/stubs/requests_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3427 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/stubs/tornado_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)      504 2023-05-26 15:56:05.000000 vcrpy-5.1.0/vcr/stubs/urllib3_stubs.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1074 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/unittest.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3796 2023-06-28 22:11:37.000000 vcrpy-5.1.0/vcr/util.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-31 03:18:47.829068 vcrpy-5.1.0/vcrpy.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)     3875 2023-07-31 03:18:47.000000 vcrpy-5.1.0/vcrpy.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     2694 2023-07-31 03:18:47.000000 vcrpy-5.1.0/vcrpy.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-07-31 03:18:47.000000 vcrpy-5.1.0/vcrpy.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       56 2023-07-31 03:18:47.000000 vcrpy-5.1.0/vcrpy.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        4 2023-07-31 03:18:47.000000 vcrpy-5.1.0/vcrpy.egg-info/top_level.txt
```

### Comparing `vcrpy-5.0.0/LICENSE.txt` & `vcrpy-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/PKG-INFO` & `vcrpy-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 5.0.0
+Version: 5.1.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-5.0.0/README.rst` & `vcrpy-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/setup.py` & `vcrpy-5.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 install_requires = [
     "PyYAML",
     "wrapt",
-    "six>=1.5",
     "yarl",
     # Support for urllib3 >=2 needs Python >=3.10
     # so we need to block urllib3 >=2 for Python <3.10 for now.
     # Note that vcrpy would work fine without any urllib3 around,
     # so this block and the dependency can be dropped at some point
     # in the future. For more Details:
     # https://github.com/kevin1024/vcrpy/pull/699#issuecomment-1551439663
@@ -60,15 +59,15 @@
     "aiohttp",
     "boto3",
     "httplib2",
     "httpx",
     "pytest",
     "pytest-aiohttp",
     "pytest-httpbin",
-    "requests",
+    "requests>=2.16.2",
     "tornado",
     # Needed to un-break httpbin 0.7.0. For httpbin >=0.7.1 and after,
     # this pin and the dependency itself can be removed, provided
     # that the related bug in httpbin has been fixed:
     # https://github.com/kevin1024/vcrpy/issues/645#issuecomment-1562489489
     # https://github.com/postmanlabs/httpbin/issues/673
     # https://github.com/postmanlabs/httpbin/pull/674
```

### Comparing `vcrpy-5.0.0/tests/fixtures/migration/new_cassette.json` & `vcrpy-5.1.0/tests/fixtures/migration/new_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/fixtures/migration/new_cassette.yaml` & `vcrpy-5.1.0/tests/fixtures/migration/new_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/fixtures/migration/old_cassette.json` & `vcrpy-5.1.0/tests/fixtures/migration/old_cassette.json`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/fixtures/migration/old_cassette.yaml` & `vcrpy-5.1.0/tests/fixtures/migration/old_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/fixtures/wild/domain_redirect.yaml` & `vcrpy-5.1.0/tests/fixtures/wild/domain_redirect.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/aiohttp_utils.py` & `vcrpy-5.1.0/tests/integration/aiohttp_utils.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml` & `vcrpy-5.1.0/tests/integration/cassettes/test_httpx_test_test_behind_proxy.yml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/conftest.py` & `vcrpy-5.1.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_aiohttp.py` & `vcrpy-5.1.0/tests/integration/test_aiohttp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import contextlib
 import logging
 import urllib.parse
 
 import pytest
 
+import vcr
+
 asyncio = pytest.importorskip("asyncio")
 aiohttp = pytest.importorskip("aiohttp")
 
-import vcr  # noqa: E402
 
 from .aiohttp_utils import aiohttp_app, aiohttp_request  # noqa: E402
 
 
 def run_in_loop(fn):
     with contextlib.closing(asyncio.new_event_loop()) as loop:
         asyncio.set_event_loop(loop)
@@ -55,15 +56,15 @@
         response, _ = get(url, auth=auth)
 
     with vcr.use_cassette(str(tmpdir.join("headers.yaml"))) as cassette:
         if auth is not None:
             request = cassette.requests[0]
             assert "AUTHORIZATION" in request.headers
         cassette_response, _ = get(url, auth=auth)
-        assert dict(cassette_response.headers) == dict(response.headers)
+        assert cassette_response.headers.items() == response.headers.items()
         assert cassette.play_count == 1
         assert "istr" not in cassette.data[0]
         assert "yarl.URL" not in cassette.data[0]
 
 
 @pytest.mark.online
 def test_case_insensitive_headers(tmpdir, mockbin_request_url):
@@ -274,17 +275,15 @@
         assert len(cassette) == 3
         assert cassette.play_count == 3
 
     # Assert that the real response and the cassette response have a similar
     # looking request_info.
     assert cassette_response.request_info.url == response.request_info.url
     assert cassette_response.request_info.method == response.request_info.method
-    assert {k: v for k, v in cassette_response.request_info.headers.items()} == {
-        k: v for k, v in response.request_info.headers.items()
-    }
+    assert cassette_response.request_info.headers.items() == response.request_info.headers.items()
     assert cassette_response.request_info.real_url == response.request_info.real_url
 
 
 @pytest.mark.online
 def test_not_modified(tmpdir, mockbin):
     """It doesn't try to redirect on 304"""
     url = mockbin + "/status/304"
@@ -347,25 +346,31 @@
         req_headers = {"Cookie": "Cookie_4=Val_4"}
 
         # ------------------------- Record -------------------------- #
         with vcr.use_cassette(tmp) as cassette:
             async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
                 cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 home_resp = await session.get(
-                    home_url, cookies=req_cookies, headers=req_headers, ssl=httpbin_ssl_context
+                    home_url,
+                    cookies=req_cookies,
+                    headers=req_headers,
+                    ssl=httpbin_ssl_context,
                 )
                 assert cassette.play_count == 0
         assert_responses(cookies_resp, home_resp)
 
         # -------------------------- Play --------------------------- #
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
             async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
                 cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 home_resp = await session.get(
-                    home_url, cookies=req_cookies, headers=req_headers, ssl=httpbin_ssl_context
+                    home_url,
+                    cookies=req_cookies,
+                    headers=req_headers,
+                    ssl=httpbin_ssl_context,
                 )
                 assert cassette.play_count == 2
         assert_responses(cookies_resp, home_resp)
 
     def assert_responses(cookies_resp, home_resp):
         assert cookies_resp.cookies.get("cookie_1").value == "val_1"
         assert cookies_resp.cookies.get("Cookie_2").value == "Val_2"
@@ -388,30 +393,32 @@
         with vcr.use_cassette(tmp) as cassette:
             async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
                 cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
                 assert cassette.play_count == 0
-            cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
+
+            assert cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
 
         # -------------------------- Play --------------------------- #
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
             async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
                 cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
                 assert cassette.play_count == 2
-            cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
+
+            assert cassette.requests[1].headers["Cookie"] == "Cookie_1=Val_1"
 
         # Assert that it's ignoring expiration date
         with vcr.use_cassette(tmp, record_mode=vcr.mode.NONE) as cassette:
             cassette.responses[0]["headers"]["set-cookie"] = [
-                "Cookie_1=Val_1; Expires=Wed, 21 Oct 2015 07:28:00 GMT"
+                "Cookie_1=Val_1; Expires=Wed, 21 Oct 2015 07:28:00 GMT",
             ]
             async with aiohttp.ClientSession(loop=loop, cookie_jar=aiohttp.CookieJar(unsafe=True)) as session:
                 cookies_resp = await session.get(cookies_url, ssl=httpbin_ssl_context)
                 assert not cookies_resp.cookies
                 cookies = session.cookie_jar.filter_cookies(cookies_url)
                 assert cookies["Cookie_1"].value == "Val_1"
 
@@ -429,7 +436,23 @@
         assert response.status == 308
 
     with vcr.use_cassette(path) as cassette:
         response, _ = get(url, allow_redirects=False)
         assert response.url.path == "/redirect/308/5"
         assert response.status == 308
         assert cassette.play_count == 1
+
+
+def test_filter_query_parameters(tmpdir, httpbin):
+    url = httpbin + "?password=secret"
+    path = str(tmpdir.join("query_param_filter.yaml"))
+
+    with vcr.use_cassette(path, filter_query_parameters=["password"]) as cassette:
+        get(url)
+
+    assert "password" not in cassette.requests[0].url
+    assert "secret" not in cassette.requests[0].url
+
+    with open(path) as f:
+        cassette_content = f.read()
+        assert "password" not in cassette_content
+        assert "secret" not in cassette_content
```

### Comparing `vcrpy-5.0.0/tests/integration/test_basic.py` & `vcrpy-5.1.0/tests/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_boto.py` & `vcrpy-5.1.0/tests/integration/test_boto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import pytest
+from configparser import DuplicateSectionError
 
-boto = pytest.importorskip("boto")
+import pytest
 
-from configparser import DuplicateSectionError  # NOQA
+import vcr
 
-import boto  # NOQA
-import boto.iam  # NOQA
-from boto.s3.connection import S3Connection  # NOQA
-from boto.s3.key import Key  # NOQA
+boto = pytest.importorskip("boto")
 
-import vcr  # NOQA
+import boto  # noqa
+import boto.iam  # noqa
+from boto.s3.connection import S3Connection  # noqa
+from boto.s3.key import Key  # noqa
 
 
 def test_boto_stubs(tmpdir):
     with vcr.use_cassette(str(tmpdir.join("boto-stubs.yml"))):
         # Perform the imports within the patched context so that
         # CertValidatingHTTPSConnection refers to the patched version.
         from boto.https_connection import CertValidatingHTTPSConnection
```

### Comparing `vcrpy-5.0.0/tests/integration/test_boto3.py` & `vcrpy-5.1.0/tests/integration/test_boto3.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import os
 
 import pytest
 
-boto3 = pytest.importorskip("boto3")
+import vcr
 
-import boto3  # NOQA
-import botocore  # NOQA
+boto3 = pytest.importorskip("boto3")
 
-import vcr  # NOQA
+import botocore  # noqa
 
 try:
-    from botocore import awsrequest  # NOQA
+    from botocore import awsrequest  # noqa
 
     botocore_awsrequest = True
 except ImportError:
     botocore_awsrequest = False
 
 # skip tests if boto does not use vendored requests anymore
 # https://github.com/boto/botocore/pull/1495
```

### Comparing `vcrpy-5.0.0/tests/integration/test_config.py` & `vcrpy-5.1.0/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_disksaver.py` & `vcrpy-5.1.0/tests/integration/test_disksaver.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_filter.py` & `vcrpy-5.1.0/tests/integration/test_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,21 +41,26 @@
         assert resp.getcode() == 200
         # authorization header should not have been recorded
         assert not _find_header(cass, "authorization")
         assert len(cass) == 2
 
 
 def test_filter_querystring(tmpdir, httpbin):
-    url = httpbin.url + "/?foo=bar"
+    url = httpbin.url + "/?password=secret"
     cass_file = str(tmpdir.join("filter_qs.yaml"))
-    with vcr.use_cassette(cass_file, filter_query_parameters=["foo"]):
+    with vcr.use_cassette(cass_file, filter_query_parameters=["password"]):
         urlopen(url)
-    with vcr.use_cassette(cass_file, filter_query_parameters=["foo"]) as cass:
+    with vcr.use_cassette(cass_file, filter_query_parameters=["password"]) as cass:
         urlopen(url)
-        assert "foo" not in cass.requests[0].url
+        assert "password" not in cass.requests[0].url
+        assert "secret" not in cass.requests[0].url
+    with open(cass_file) as f:
+        cassette_content = f.read()
+        assert "password" not in cassette_content
+        assert "secret" not in cassette_content
 
 
 def test_filter_post_data(tmpdir, httpbin):
     url = httpbin.url + "/post"
     data = urlencode({"id": "secret", "foo": "bar"}).encode("utf-8")
     cass_file = str(tmpdir.join("filter_pd.yaml"))
     with vcr.use_cassette(cass_file, filter_post_data_parameters=["id"]):
```

### Comparing `vcrpy-5.0.0/tests/integration/test_http` & `vcrpy-5.1.0/tests/integration/test_http`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_httplib2.py` & `vcrpy-5.1.0/tests/integration/test_httplib2.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_httpx.py` & `vcrpy-5.1.0/tests/integration/test_httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 import pytest
 
+import vcr
+
 asyncio = pytest.importorskip("asyncio")
 httpx = pytest.importorskip("httpx")
 
-import vcr  # noqa: E402
 from vcr.stubs.httpx_stubs import HTTPX_REDIRECT_PARAM  # noqa: E402
 
 
 class BaseDoRequest:
     _client_class = None
 
     def __init__(self, *args, **kwargs):
@@ -61,16 +62,16 @@
             self._loop.close()
             del self._loop
 
     @property
     def client(self):
         try:
             return self._client
-        except AttributeError:
-            raise ValueError('To access async client, use "with do_request() as client"')
+        except AttributeError as e:
+            raise ValueError('To access async client, use "with do_request() as client"') from e
 
     def __call__(self, *args, **kwargs):
         if hasattr(self, "_loop"):
             return self._loop.run_until_complete(self.client.request(*args, **kwargs))
 
         # Use one-time context and dispose of the loop/client afterwards
         with self:
@@ -181,17 +182,15 @@
         assert len(cassette) == 3
         assert cassette.play_count == 3
 
     # Assert that the real response and the cassette response have a similar
     # looking request_info.
     assert cassette_response.request.url == response.request.url
     assert cassette_response.request.method == response.request.method
-    assert {k: v for k, v in cassette_response.request.headers.items()} == {
-        k: v for k, v in response.request.headers.items()
-    }
+    assert cassette_response.request.headers.items() == response.request.headers.items()
 
 
 @pytest.mark.online
 def test_work_with_gzipped_data(mockbin, do_request, yml):
     url = mockbin + "/gzip?foo=bar"
     headers = {"accept-encoding": "deflate, gzip"}
 
@@ -238,18 +237,18 @@
         assert cassette_response.headers["Via"] == "my_own_proxy", str(cassette_response.headers)
         assert cassette_response.request.url == response.request.url
 
 
 @pytest.mark.online
 def test_cookies(tmpdir, mockbin, do_request):
     def client_cookies(client):
-        return [c for c in client.client.cookies]
+        return list(client.client.cookies)
 
     def response_cookies(response):
-        return [c for c in response.cookies]
+        return list(response.cookies)
 
     url = mockbin + "/bin/26148652-fe25-4f21-aaf5-689b5b4bf65f"
     headers = {"cookie": "k1=v1;k2=v2"}
 
     with do_request(headers=headers) as client:
         assert client_cookies(client) == []
```

### Comparing `vcrpy-5.0.0/tests/integration/test_ignore.py` & `vcrpy-5.1.0/tests/integration/test_ignore.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_matchers.py` & `vcrpy-5.1.0/tests/integration/test_matchers.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,20 @@
     with pytest.raises(vcr.errors.CannotOverwriteExistingCassetteException):
         with vcr.use_cassette(cassette, match_on=["method"]) as cass:
             # is a POST request
             urlopen(default_uri, data=b"")
 
 
 @pytest.mark.parametrize(
-    "uri", [DEFAULT_URI, "http://httpbin.org/get?p2=q2&p1=q1", "http://httpbin.org/get?p2=q2&p1=q1"]
+    "uri",
+    (
+        DEFAULT_URI,
+        "http://httpbin.org/get?p2=q2&p1=q1",
+        "http://httpbin.org/get?p2=q2&p1=q1",
+    ),
 )
 def test_default_matcher_matches(cassette, uri, httpbin, httpbin_secure):
     uri = _replace_httpbin(uri, httpbin, httpbin_secure)
 
     with vcr.use_cassette(cassette) as cass:
         urlopen(uri)
         assert cass.play_count == 1
```

### Comparing `vcrpy-5.0.0/tests/integration/test_multiple.py` & `vcrpy-5.1.0/tests/integration/test_multiple.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.request import urlopen
 
 import pytest
 
 import vcr
+from vcr.errors import CannotOverwriteExistingCassetteException
 
 
 def test_making_extra_request_raises_exception(tmpdir, httpbin):
     # make two requests in the first request that are considered
     # identical (since the match is based on method)
     with vcr.use_cassette(str(tmpdir.join("test.json")), match_on=["method"]):
         urlopen(httpbin.url + "/status/200")
@@ -14,9 +15,9 @@
 
     # Now, try to make three requests.  The first two should return the
     # correct status codes in order, and the third should raise an
     # exception.
     with vcr.use_cassette(str(tmpdir.join("test.json")), match_on=["method"]):
         assert urlopen(httpbin.url + "/status/200").getcode() == 200
         assert urlopen(httpbin.url + "/status/201").getcode() == 201
-        with pytest.raises(Exception):
+        with pytest.raises(CannotOverwriteExistingCassetteException):
             urlopen(httpbin.url + "/status/200")
```

### Comparing `vcrpy-5.0.0/tests/integration/test_proxy.py` & `vcrpy-5.1.0/tests/integration/test_proxy.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_record_mode.py` & `vcrpy-5.1.0/tests/integration/test_record_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from urllib.request import urlopen
 
 import pytest
 
 import vcr
+from vcr.errors import CannotOverwriteExistingCassetteException
 
 
 def test_once_record_mode(tmpdir, httpbin):
     testfile = str(tmpdir.join("recordmode.yml"))
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ONCE):
         # cassette file doesn't exist, so create.
         urlopen(httpbin.url).read()
@@ -14,15 +15,15 @@
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ONCE):
         # make the same request again
         urlopen(httpbin.url).read()
 
         # the first time, it's played from the cassette.
         # but, try to access something else from the same cassette, and an
         # exception is raised.
-        with pytest.raises(Exception):
+        with pytest.raises(CannotOverwriteExistingCassetteException):
             urlopen(httpbin.url + "/get").read()
 
 
 def test_once_record_mode_two_times(tmpdir, httpbin):
     testfile = str(tmpdir.join("recordmode.yml"))
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ONCE):
         # get two of the same file
@@ -90,15 +91,15 @@
 
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ONCE):
         # make the same request again
         assert urlopen(url).read() == original_first_response
         assert urlopen(url).read() == original_second_response
         # now that we are back in once mode, this should raise
         # an error.
-        with pytest.raises(Exception):
+        with pytest.raises(CannotOverwriteExistingCassetteException):
             urlopen(url).read()
 
 
 def test_all_record_mode(tmpdir, httpbin):
     testfile = str(tmpdir.join("recordmode.yml"))
 
     with vcr.use_cassette(testfile, record_mode=vcr.mode.ALL):
@@ -120,15 +121,15 @@
 
 
 def test_none_record_mode(tmpdir, httpbin):
     # Cassette file doesn't exist, yet we are trying to make a request.
     # raise hell.
     testfile = str(tmpdir.join("recordmode.yml"))
     with vcr.use_cassette(testfile, record_mode=vcr.mode.NONE):
-        with pytest.raises(Exception):
+        with pytest.raises(CannotOverwriteExistingCassetteException):
             urlopen(httpbin.url).read()
 
 
 def test_none_record_mode_with_existing_cassette(tmpdir, httpbin):
     # create a cassette file
     testfile = str(tmpdir.join("recordmode.yml"))
 
@@ -136,9 +137,9 @@
         urlopen(httpbin.url).read()
 
     # play from cassette file
     with vcr.use_cassette(testfile, record_mode=vcr.mode.NONE) as cass:
         urlopen(httpbin.url).read()
         assert cass.play_count == 1
         # but if I try to hit the net, raise an exception.
-        with pytest.raises(Exception):
+        with pytest.raises(CannotOverwriteExistingCassetteException):
             urlopen(httpbin.url + "/get").read()
```

### Comparing `vcrpy-5.0.0/tests/integration/test_register_matcher.py` & `vcrpy-5.1.0/tests/integration/test_register_matcher.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_register_persister.py` & `vcrpy-5.1.0/tests/integration/test_register_persister.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_register_serializer.py` & `vcrpy-5.1.0/tests/integration/test_register_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_request.py` & `vcrpy-5.1.0/tests/integration/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_requests.py` & `vcrpy-5.1.0/tests/integration/test_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Test requests' interaction with vcr"""
 import pytest
 from assertions import assert_cassette_empty, assert_is_json_bytes
 
 import vcr
 
 requests = pytest.importorskip("requests")
-from requests.exceptions import ConnectionError  # noqa E402
 
 
 def test_status_code(httpbin_both, tmpdir):
     """Ensure that we can read the status code"""
     url = httpbin_both.url + "/"
     with vcr.use_cassette(str(tmpdir.join("atts.yaml"))):
         status_code = requests.get(url).status_code
@@ -167,15 +166,16 @@
     url = httpbin_both + "/gzip"
 
     expected_response = requests.get(url)
     expected_content = expected_response.content
     assert expected_response.headers["content-encoding"] == "gzip"  # self-test
 
     with vcr.use_cassette(
-        str(tmpdir.join("decode_compressed.yaml")), decode_compressed_response=True
+        str(tmpdir.join("decode_compressed.yaml")),
+        decode_compressed_response=True,
     ) as cassette:
         r = requests.get(url)
         assert r.headers["content-encoding"] == "gzip"  # i.e. not removed
         assert r.content == expected_content
 
     # Has the cassette body been decompressed?
     cassette_response_body = cassette.responses[0]["body"]["string"]
```

### Comparing `vcrpy-5.0.0/tests/integration/test_stubs.py` & `vcrpy-5.1.0/tests/integration/test_stubs.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,20 +116,20 @@
     with vcr.use_cassette(testfile, before_record_response=callback):
         conn = httplib.HTTPConnection(host, port)
         conn.request("GET", "/get")
         inside = conn.getresponse()
 
         # The scrubbed field should be the same, because no cassette existed.
         # Furthermore, the responses should be identical.
-        inside_body = json.loads(inside.read().decode("utf-8"))
-        outside_body = json.loads(outside.read().decode("utf-8"))
+        inside_body = json.loads(inside.read())
+        outside_body = json.loads(outside.read())
         assert not inside_body[field_to_scrub] == replacement
         assert inside_body[field_to_scrub] == outside_body[field_to_scrub]
 
     # Ensure that when a cassette exists, the scrubbed response is returned.
     with vcr.use_cassette(testfile, before_record_response=callback):
         conn = httplib.HTTPConnection(host, port)
         conn.request("GET", "/get")
         inside = conn.getresponse()
 
-        inside_body = json.loads(inside.read().decode("utf-8"))
+        inside_body = json.loads(inside.read())
         assert inside_body[field_to_scrub] == replacement
```

### Comparing `vcrpy-5.0.0/tests/integration/test_tornado.py` & `vcrpy-5.1.0/tests/integration/test_tornado.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
 @pytest.mark.gen_test
 def test_unsupported_features_raises_in_future(get_client, tmpdir):
     """Ensure that the exception for an AsyncHTTPClient feature not being
     supported is raised inside the future."""
 
     def callback(chunk):
-        assert False, "Did not expect to be called."
+        raise AssertionError("Did not expect to be called.")
 
     with vcr.use_cassette(str(tmpdir.join("invalid.yaml"))):
         future = get(get_client(), "http://httpbin.org", streaming_callback=callback)
 
     with pytest.raises(Exception) as excinfo:
         yield future
 
@@ -234,19 +234,22 @@
 @pytest.mark.skipif(not supports_raise_error, reason="raise_error unavailable in tornado <= 3")
 @pytest.mark.gen_test
 def test_unsupported_features_raise_error_disabled(get_client, tmpdir):
     """Ensure that the exception for an AsyncHTTPClient feature not being
     supported is not raised if raise_error=False."""
 
     def callback(chunk):
-        assert False, "Did not expect to be called."
+        raise AssertionError("Did not expect to be called.")
 
     with vcr.use_cassette(str(tmpdir.join("invalid.yaml"))):
         response = yield get(
-            get_client(), "http://httpbin.org", streaming_callback=callback, raise_error=False
+            get_client(),
+            "http://httpbin.org",
+            streaming_callback=callback,
+            raise_error=False,
         )
 
     assert "not yet supported by VCR" in str(response.error)
 
 
 @pytest.mark.gen_test
 def test_cannot_overwrite_cassette_raises_in_future(get_client, tmpdir):
```

### Comparing `vcrpy-5.0.0/tests/integration/test_tornado_exception_can_be_caught.yaml` & `vcrpy-5.1.0/tests/integration/test_tornado_exception_can_be_caught.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml` & `vcrpy-5.1.0/tests/integration/test_tornado_with_decorator_use_cassette.yaml`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_urllib2.py` & `vcrpy-5.1.0/tests/integration/test_urllib2.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/integration/test_urllib3.py` & `vcrpy-5.1.0/tests/integration/test_urllib3.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 urllib3 = pytest.importorskip("urllib3")
 
 
 @pytest.fixture(scope="module")
 def verify_pool_mgr():
     return urllib3.PoolManager(
-        cert_reqs="CERT_REQUIRED", ca_certs=pytest_httpbin.certs.where()  # Force certificate check.
+        cert_reqs="CERT_REQUIRED",
+        ca_certs=pytest_httpbin.certs.where(),  # Force certificate check.
     )
 
 
 @pytest.fixture(scope="module")
 def pool_mgr():
     return urllib3.PoolManager(cert_reqs="CERT_NONE")
```

### Comparing `vcrpy-5.0.0/tests/integration/test_wild.py` & `vcrpy-5.1.0/tests/integration/test_wild.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import http.client as httplib
 import multiprocessing
 from xmlrpc.client import ServerProxy
 from xmlrpc.server import SimpleXMLRPCServer
 
 import pytest
 
-requests = pytest.importorskip("requests")
+import vcr
 
-import vcr  # NOQA
+requests = pytest.importorskip("requests")
 
 
 def test_domain_redirect():
     """Ensure that redirects across domains are considered unique"""
     # In this example, seomoz.org redirects to moz.com, and if those
     # requests are considered identical, then we'll be stuck in a redirect
     # loop.
```

### Comparing `vcrpy-5.0.0/tests/unit/test_cassettes.py` & `vcrpy-5.1.0/tests/unit/test_cassettes.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,21 @@
 
 def test_cassette_load(tmpdir):
     a_file = tmpdir.join("test_cassette.yml")
     a_file.write(
         yaml.dump(
             {
                 "interactions": [
-                    {"request": {"body": "", "uri": "foo", "method": "GET", "headers": {}}, "response": "bar"}
-                ]
-            }
-        )
+                    {
+                        "request": {"body": "", "uri": "foo", "method": "GET", "headers": {}},
+                        "response": "bar",
+                    },
+                ],
+            },
+        ),
     )
     a_cassette = Cassette.load(path=str(a_file))
     assert len(a_cassette) == 1
 
 
 def test_cassette_load_nonexistent():
     a_cassette = Cassette.load(path="something/nonexistent.yml")
@@ -106,15 +109,15 @@
     "vcr.cassette.FilesystemPersister.load_cassette",
     classmethod(lambda *args, **kwargs: (("foo",), (mock.MagicMock(),))),
 )
 @mock.patch("vcr.cassette.Cassette.can_play_response_for", return_value=True)
 @mock.patch("vcr.stubs.VCRHTTPResponse")
 def test_function_decorated_with_use_cassette_can_be_invoked_multiple_times(*args):
     decorated_function = Cassette.use(path="test")(make_get_request)
-    for i in range(4):
+    for _ in range(4):
         decorated_function()
 
 
 def test_arg_getter_functionality():
     arg_getter = mock.Mock(return_value={"path": "test"})
     context_decorator = Cassette.use_arg_getter(arg_getter)
 
@@ -152,15 +155,15 @@
 
 
 @mock.patch("vcr.cassette.requests_match", _mock_requests_match)
 def test_cassette_allow_playback_repeats():
     a = Cassette("test", allow_playback_repeats=True)
     a.append("foo", "bar")
     a.append("other", "resp")
-    for x in range(10):
+    for _ in range(10):
         assert a.play_response("foo") == "bar"
     assert a.play_count == 10
     assert a.all_played is False
     assert a.play_response("other") == "resp"
     assert a.play_count == 11
     assert a.all_played
 
@@ -214,15 +217,15 @@
 
     second_response = copy.deepcopy(first_response)
     second_response["body"]["string"] = b"second_response"
 
     with contextlib.ExitStack() as exit_stack:
         first_cassette = exit_stack.enter_context(Cassette.use(path="test"))
         exit_stack.enter_context(
-            mock.patch.object(first_cassette, "play_response", return_value=first_response)
+            mock.patch.object(first_cassette, "play_response", return_value=first_response),
         )
         assert_get_response_body_is("first_response")
 
         # Make sure a second cassette can supersede the first
         with Cassette.use(path="test") as second_cassette:
             with mock.patch.object(second_cassette, "play_response", return_value=second_response):
                 assert_get_response_body_is("second_response")
```

### Comparing `vcrpy-5.0.0/tests/unit/test_errors.py` & `vcrpy-5.1.0/tests/unit/test_errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,19 +51,22 @@
             "Matchers failed :\n"
             "query - assertion failure :\n"
             "failed : query 2\n",
         ),
     ],
 )
 def test_CannotOverwriteExistingCassetteException_get_message(
-    mock_find_requests_with_most_matches, most_matches, expected_message
+    mock_find_requests_with_most_matches,
+    most_matches,
+    expected_message,
 ):
     mock_find_requests_with_most_matches.return_value = most_matches
     cassette = Cassette("path")
     failed_request = "request"
     exception_message = errors.CannotOverwriteExistingCassetteException._get_message(cassette, "request")
     expected = (
-        "Can't overwrite existing cassette (%r) in your current record mode (%r).\n"
-        "No match for the request (%r) was found.\n"
-        "%s" % (cassette._path, cassette.record_mode, failed_request, expected_message)
+        f"Can't overwrite existing cassette ({cassette._path!r}) "
+        f"in your current record mode ({cassette.record_mode!r}).\n"
+        f"No match for the request ({failed_request!r}) was found.\n"
+        f"{expected_message}"
     )
     assert exception_message == expected
```

### Comparing `vcrpy-5.0.0/tests/unit/test_filters.py` & `vcrpy-5.1.0/tests/unit/test_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,27 +193,27 @@
             ("two", None),
             ("three", "tada"),
             ("four", lambda key, value, request: value.upper()),
             ("five", lambda key, value, request: None),
             ("six", "doesntexist"),
         ],
     )
-    request_data = json.loads(request.body.decode("utf-8"))
+    request_data = json.loads(request.body)
     expected_data = json.loads('{"one": "keep", "three": "tada", "four": "SHOUT"}')
     assert request_data == expected_data
 
 
 def test_remove_json_post_data_parameters():
     # Test the backward-compatible API wrapper.
     body = b'{"id": "secret", "foo": "bar", "baz": "qux"}'
     request = Request("POST", "http://google.com", body, {})
     request.headers["Content-Type"] = "application/json"
     remove_post_data_parameters(request, ["id"])
-    request_body_json = json.loads(request.body.decode("utf-8"))
-    expected_json = json.loads(b'{"foo": "bar", "baz": "qux"}'.decode("utf-8"))
+    request_body_json = json.loads(request.body)
+    expected_json = json.loads(b'{"foo": "bar", "baz": "qux"}')
     assert request_body_json == expected_json
 
 
 def test_remove_all_json_post_data_parameters():
     body = b'{"id": "secret", "foo": "bar"}'
     request = Request("POST", "http://google.com", body, {})
     request.headers["Content-Type"] = "application/json"
```

### Comparing `vcrpy-5.0.0/tests/unit/test_json_serializer.py` & `vcrpy-5.1.0/tests/unit/test_json_serializer.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_matchers.py` & `vcrpy-5.1.0/tests/unit/test_matchers.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,75 +59,135 @@
     "X-Amz-Date": b"20191102T143910Z",
     "User-Agent": b"Boto3/1.9.102 Python/3.5.3 Linux/4.15.0-54-generic Botocore/1.12.253 Resource",
     "Content-MD5": b"GQqjEXsRqrPyxfTl99nkAg==",
     "Content-Type": b"text/plain",
     "Expect": b"100-continue",
     "Content-Length": "21",
 }
+chunked_headers = {
+    "Transfer-Encoding": "chunked",
+}
 
 
 @pytest.mark.parametrize(
     "r1, r2",
     [
         (
             request.Request("POST", "http://host.com/", "123", {}),
             request.Request("POST", "http://another-host.com/", "123", {"Some-Header": "value"}),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", "a=1&b=2", {"Content-Type": "application/x-www-form-urlencoded"}
+                "POST",
+                "http://host.com/",
+                "a=1&b=2",
+                {"Content-Type": "application/x-www-form-urlencoded"},
             ),
             request.Request(
-                "POST", "http://host.com/", "b=2&a=1", {"Content-Type": "application/x-www-form-urlencoded"}
+                "POST",
+                "http://host.com/",
+                "b=2&a=1",
+                {"Content-Type": "application/x-www-form-urlencoded"},
             ),
         ),
         (
             request.Request("POST", "http://host.com/", "123", {}),
             request.Request("POST", "http://another-host.com/", "123", {"Some-Header": "value"}),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", "a=1&b=2", {"Content-Type": "application/x-www-form-urlencoded"}
+                "POST",
+                "http://host.com/",
+                "a=1&b=2",
+                {"Content-Type": "application/x-www-form-urlencoded"},
             ),
             request.Request(
-                "POST", "http://host.com/", "b=2&a=1", {"Content-Type": "application/x-www-form-urlencoded"}
+                "POST",
+                "http://host.com/",
+                "b=2&a=1",
+                {"Content-Type": "application/x-www-form-urlencoded"},
             ),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", '{"a": 1, "b": 2}', {"Content-Type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"a": 1, "b": 2}',
+                {"Content-Type": "application/json"},
             ),
             request.Request(
-                "POST", "http://host.com/", '{"b": 2, "a": 1}', {"content-type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"b": 2, "a": 1}',
+                {"content-type": "application/json"},
             ),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", req1_body, {"User-Agent": "xmlrpclib", "Content-Type": "text/xml"}
+                "POST",
+                "http://host.com/",
+                req1_body,
+                {"User-Agent": "xmlrpclib", "Content-Type": "text/xml"},
             ),
             request.Request(
                 "POST",
                 "http://host.com/",
                 req2_body,
                 {"user-agent": "somexmlrpc", "content-type": "text/xml"},
             ),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", '{"a": 1, "b": 2}', {"Content-Type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"a": 1, "b": 2}',
+                {"Content-Type": "application/json"},
             ),
             request.Request(
-                "POST", "http://host.com/", '{"b": 2, "a": 1}', {"content-type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"b": 2, "a": 1}',
+                {"content-type": "application/json"},
             ),
         ),
         (
             # special case for boto3 bytes headers
             request.Request("POST", "http://aws.custom.com/", b"123", boto3_bytes_headers),
             request.Request("POST", "http://aws.custom.com/", b"123", boto3_bytes_headers),
         ),
+        (
+            # chunked transfer encoding: decoded bytes versus encoded bytes
+            request.Request("POST", "scheme1://host1.test/", b"123456789_123456", chunked_headers),
+            request.Request(
+                "GET",
+                "scheme2://host2.test/",
+                b"10\r\n123456789_123456\r\n0\r\n\r\n",
+                chunked_headers,
+            ),
+        ),
+        (
+            # chunked transfer encoding: bytes iterator versus string iterator
+            request.Request(
+                "POST",
+                "scheme1://host1.test/",
+                iter([b"123456789_", b"123456"]),
+                chunked_headers,
+            ),
+            request.Request("GET", "scheme2://host2.test/", iter(["123456789_", "123456"]), chunked_headers),
+        ),
+        (
+            # chunked transfer encoding: bytes iterator versus single byte iterator
+            request.Request(
+                "POST",
+                "scheme1://host1.test/",
+                iter([b"123456789_", b"123456"]),
+                chunked_headers,
+            ),
+            request.Request("GET", "scheme2://host2.test/", iter(b"123456789_123456"), chunked_headers),
+        ),
     ],
 )
 def test_body_matcher_does_match(r1, r2):
     assert matchers.body(r1, r2) is None
 
 
 @pytest.mark.parametrize(
@@ -135,18 +195,24 @@
     [
         (
             request.Request("POST", "http://host.com/", '{"a": 1, "b": 2}', {}),
             request.Request("POST", "http://host.com/", '{"b": 2, "a": 1}', {}),
         ),
         (
             request.Request(
-                "POST", "http://host.com/", '{"a": 1, "b": 3}', {"Content-Type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"a": 1, "b": 3}',
+                {"Content-Type": "application/json"},
             ),
             request.Request(
-                "POST", "http://host.com/", '{"b": 2, "a": 1}', {"content-type": "application/json"}
+                "POST",
+                "http://host.com/",
+                '{"b": 2, "a": 1}',
+                {"content-type": "application/json"},
             ),
         ),
         (
             request.Request("POST", "http://host.com/", req1_body, {"Content-Type": "text/xml"}),
             request.Request("POST", "http://host.com/", req2_body, {"content-type": "text/xml"}),
         ),
     ],
```

### Comparing `vcrpy-5.0.0/tests/unit/test_migration.py` & `vcrpy-5.1.0/tests/unit/test_migration.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_persist.py` & `vcrpy-5.1.0/tests/unit/test_persist.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_request.py` & `vcrpy-5.1.0/tests/unit/test_request.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_response.py` & `vcrpy-5.1.0/tests/unit/test_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             b"tested in a wide variety of clinical applications. They are especially\n  "
             b"    effective "
             b"in preclinical models of cancer where they show antiproliferative\n      "
             b"action in many "
             b"different types of cancer cells. Recently, the first HDACi was\n      "
             b"approved for the "
             b"treatment of cutaneous T cell lymphomas. Most HDACi currently in\n      "
-            b"clinical "
+            b"clinical ",
         },
     }
     vcr_response = VCRHTTPResponse(recorded_response)
     handle = io.TextIOWrapper(vcr_response, encoding="utf-8")
     handle = iter(handle)
-    articles = [line for line in handle]
+    articles = list(handle)
     assert len(articles) > 1
```

### Comparing `vcrpy-5.0.0/tests/unit/test_serialize.py` & `vcrpy-5.1.0/tests/unit/test_serialize.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_stubs.py` & `vcrpy-5.1.0/tests/unit/test_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/tests/unit/test_unittest.py` & `vcrpy-5.1.0/tests/unit/test_unittest.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,34 +96,34 @@
     # Test that _get_cassette_library_dir applies if cassette_library_dir
     # is absent from vcr kwargs.
     class MyTest(VCRTestCase):
         def test_foo(self):
             pass
 
         def _get_vcr_kwargs(self):
-            return dict(
-                record_mode="new_episodes",
-            )
+            return {
+                "record_mode": "new_episodes",
+            }
 
         _get_cassette_library_dir = MagicMock(return_value="/testing")
 
     test = run_testcase(MyTest)[0][0]
     assert test.cassette._path.startswith("/testing/")
     assert test._get_cassette_library_dir.call_count == 1
 
     # Test that _get_cassette_library_dir is ignored if cassette_library_dir
     # is present in vcr kwargs.
     class MyTest(VCRTestCase):
         def test_foo(self):
             pass
 
         def _get_vcr_kwargs(self):
-            return dict(
-                cassette_library_dir="/testing",
-            )
+            return {
+                "cassette_library_dir": "/testing",
+            }
 
         _get_cassette_library_dir = MagicMock(return_value="/ignored")
 
     test = run_testcase(MyTest)[0][0]
     assert test.cassette._path.startswith("/testing/")
     assert test._get_cassette_library_dir.call_count == 0
```

### Comparing `vcrpy-5.0.0/tests/unit/test_vcr.py` & `vcrpy-5.1.0/tests/unit/test_vcr.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from vcr.stubs import VCRHTTPSConnection
 
 
 def test_vcr_use_cassette():
     record_mode = mock.Mock()
     test_vcr = VCR(record_mode=record_mode)
     with mock.patch(
-        "vcr.cassette.Cassette.load", return_value=mock.MagicMock(inject=False)
+        "vcr.cassette.Cassette.load",
+        return_value=mock.MagicMock(inject=False),
     ) as mock_cassette_load:
 
         @test_vcr.use_cassette("test")
         def function():
             pass
 
         assert mock_cassette_load.call_count == 0
@@ -67,24 +68,27 @@
         request = Request("GET", base_path + "?foo=bar", "", {})
         assert cassette.filter_request(request).query == []
         request = Request("GET", base_path + "?tom=nobody", "", {})
         assert cassette.filter_request(request).query == [("tom", "jerry")]
 
         # Test filter_headers
         request = Request(
-            "GET", base_path + "?foo=bar", "", {"cookie": "test", "other": "fun", "bert": "nobody"}
+            "GET",
+            base_path + "?foo=bar",
+            "",
+            {"cookie": "test", "other": "fun", "bert": "nobody"},
         )
         assert cassette.filter_request(request).headers == {"other": "fun", "bert": "ernie"}
 
         # Test ignore_hosts
-        request = Request("GET", "http://www.test.com" + "?foo=bar", "", {"cookie": "test", "other": "fun"})
+        request = Request("GET", "http://www.test.com?foo=bar", "", {"cookie": "test", "other": "fun"})
         assert cassette.filter_request(request) is None
 
         # Test ignore_localhost
-        request = Request("GET", "http://localhost:8000" + "?foo=bar", "", {"cookie": "test", "other": "fun"})
+        request = Request("GET", "http://localhost:8000?foo=bar", "", {"cookie": "test", "other": "fun"})
         assert cassette.filter_request(request) is None
 
     with test_vcr.use_cassette("test", before_record_request=None) as cassette:
         # Test that before_record can be overwritten in context manager.
         assert cassette.filter_request(request_get) is not None
 
 
@@ -255,15 +259,17 @@
 
     function_name()
 
 
 def test_cassette_library_dir_with_path_transformer():
     library_dir = "/library_dir"
     vcr = VCR(
-        inject_cassette=True, cassette_library_dir=library_dir, path_transformer=lambda path: path + ".json"
+        inject_cassette=True,
+        cassette_library_dir=library_dir,
+        path_transformer=lambda path: path + ".json",
     )
 
     @vcr.use_cassette()
     def function_name(cassette):
         assert cassette._path == os.path.join(library_dir, "function_name.json")
 
     function_name()
@@ -358,11 +364,11 @@
 
 TestVCRClass.test_dynamically_added = test_dynamically_added
 del test_dynamically_added
 
 
 def test_path_class_as_cassette():
     path = Path(__file__).parent.parent.joinpath(
-        "integration/cassettes/test_httpx_test_test_behind_proxy.yml"
+        "integration/cassettes/test_httpx_test_test_behind_proxy.yml",
     )
     with use_cassette(path):
         pass
```

### Comparing `vcrpy-5.0.0/vcr/cassette.py` & `vcrpy-5.1.0/vcr/cassette.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 import collections
 import contextlib
 import copy
 import inspect
 import logging
 import sys
+from asyncio import iscoroutinefunction
 
 import wrapt
 
 from ._handle_coroutine import handle_coroutine
 from .errors import UnhandledHTTPRequestError
 from .matchers import get_matchers_results, method, requests_match, uri
 from .patch import CassettePatcherBuilder
 from .persisters.filesystem import CassetteDecodeError, CassetteNotFoundError, FilesystemPersister
 from .record_mode import RecordMode
 from .serializers import yamlserializer
 from .util import partition_dict
 
-try:
-    from asyncio import iscoroutinefunction
-except ImportError:
-
-    def iscoroutinefunction(*args, **kwargs):
-        return False
-
-
 log = logging.getLogger(__name__)
 
 
 class CassetteContextDecorator:
     """Context manager/decorator that handles installing the cassette and
     removing cassettes.
 
@@ -77,15 +70,16 @@
         # How might this condition be met? Here is an example:
         # context_decorator = Cassette.use('whatever')
         # with context_decorator:
         #     with context_decorator:
         #         pass
         assert self.__finish is None, "Cassette already open."
         other_kwargs, cassette_kwargs = partition_dict(
-            lambda key, _: key in self._non_cassette_arguments, self._args_getter()
+            lambda key, _: key in self._non_cassette_arguments,
+            self._args_getter(),
         )
         if other_kwargs.get("path_transformer"):
             transformer = other_kwargs["path_transformer"]
             cassette_kwargs["path"] = transformer(cassette_kwargs["path"])
         self.__cassette = self.cls.load(**cassette_kwargs)
         self.__finish = self._patch_generator(self.__cassette)
         return next(self.__finish)
@@ -276,30 +270,30 @@
         """
         for index, response in self._responses(request):
             if self.play_counts[index] == 0 or self.allow_playback_repeats:
                 self.play_counts[index] += 1
                 return response
         # The cassette doesn't contain the request asked for.
         raise UnhandledHTTPRequestError(
-            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for"
+            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for",
         )
 
     def responses_of(self, request):
         """
         Find the responses corresponding to a request.
         This function isn't actually used by VCR internally, but is
         provided as an external API.
         """
         responses = [response for index, response in self._responses(request)]
 
         if responses:
             return responses
         # The cassette doesn't contain the request asked for.
         raise UnhandledHTTPRequestError(
-            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for"
+            f"The cassette ({self._path!r}) doesn't contain the request ({request!r}) asked for",
         )
 
     def rewind(self):
         self.play_counts = collections.Counter()
 
     def find_requests_with_most_matches(self, request):
         """
@@ -310,15 +304,15 @@
         - the failed matchers and the related assertion message with the difference details as strings tuple
 
         This is useful when a request failed to be found,
         we can get the similar request(s) in order to know what have changed in the request parts.
         """
         best_matches = []
         request = self._before_record_request(request)
-        for index, (stored_request, response) in enumerate(self.data):
+        for _, (stored_request, _) in enumerate(self.data):
             successes, fails = get_matchers_results(request, stored_request, self._match_on)
             best_matches.append((len(successes), stored_request, successes, fails))
         best_matches.sort(key=lambda t: t[0], reverse=True)
         # Get the first best matches (multiple if equal matches)
         final_best_matches = []
 
         if not best_matches:
@@ -360,11 +354,11 @@
 
     def __len__(self):
         """Return the number of request,response pairs stored in here"""
         return len(self.data)
 
     def __contains__(self, request):
         """Return whether or not a request has been stored"""
-        for index, response in self._responses(request):
+        for index, _ in self._responses(request):
             if self.play_counts[index] == 0 or self.allow_playback_repeats:
                 return True
         return False
```

### Comparing `vcrpy-5.0.0/vcr/config.py` & `vcrpy-5.1.0/vcr/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 import functools
 import inspect
 import os
 import types
 from collections import abc as collections_abc
 from pathlib import Path
 
-import six
-
 from . import filters, matchers
 from .cassette import Cassette
 from .persisters.filesystem import FilesystemPersister
 from .record_mode import RecordMode
 from .serializers import jsonserializer, yamlserializer
 from .util import auto_decorate, compose
 
@@ -84,24 +82,24 @@
         self.record_on_exception = record_on_exception
         self._custom_patches = tuple(custom_patches)
 
     def _get_serializer(self, serializer_name):
         try:
             serializer = self.serializers[serializer_name]
         except KeyError:
-            raise KeyError(f"Serializer {serializer_name} doesn't exist or isn't registered")
+            raise KeyError(f"Serializer {serializer_name} doesn't exist or isn't registered") from None
         return serializer
 
     def _get_matchers(self, matcher_names):
         matchers = []
         try:
             for m in matcher_names:
                 matchers.append(self.matchers[m])
         except KeyError:
-            raise KeyError(f"Matcher {m} doesn't exist or isn't registered")
+            raise KeyError(f"Matcher {m} doesn't exist or isn't registered") from None
         return matchers
 
     def use_cassette(self, path=None, **kwargs):
         if path is not None and not isinstance(path, (str, Path)):
             function = path
             # Assume this is an attempt to decorate a function
             return self._use_cassette(**kwargs)(function)
@@ -158,15 +156,16 @@
         if path:
             merged_config["path"] = path
         return merged_config
 
     def _build_before_record_response(self, options):
         before_record_response = options.get("before_record_response", self.before_record_response)
         decode_compressed_response = options.get(
-            "decode_compressed_response", self.decode_compressed_response
+            "decode_compressed_response",
+            self.decode_compressed_response,
         )
         filter_functions = []
         if decode_compressed_response:
             filter_functions.append(filters.decode_response)
         if before_record_response:
             if not isinstance(before_record_response, collections_abc.Iterable):
                 before_record_response = (before_record_response,)
@@ -182,33 +181,35 @@
         return before_record_response
 
     def _build_before_record_request(self, options):
         filter_functions = []
         filter_headers = options.get("filter_headers", self.filter_headers)
         filter_query_parameters = options.get("filter_query_parameters", self.filter_query_parameters)
         filter_post_data_parameters = options.get(
-            "filter_post_data_parameters", self.filter_post_data_parameters
+            "filter_post_data_parameters",
+            self.filter_post_data_parameters,
         )
         before_record_request = options.get(
-            "before_record_request", options.get("before_record", self.before_record_request)
+            "before_record_request",
+            options.get("before_record", self.before_record_request),
         )
         ignore_hosts = options.get("ignore_hosts", self.ignore_hosts)
         ignore_localhost = options.get("ignore_localhost", self.ignore_localhost)
         if filter_headers:
             replacements = [h if isinstance(h, tuple) else (h, None) for h in filter_headers]
             filter_functions.append(functools.partial(filters.replace_headers, replacements=replacements))
         if filter_query_parameters:
             replacements = [p if isinstance(p, tuple) else (p, None) for p in filter_query_parameters]
             filter_functions.append(
-                functools.partial(filters.replace_query_parameters, replacements=replacements)
+                functools.partial(filters.replace_query_parameters, replacements=replacements),
             )
         if filter_post_data_parameters:
             replacements = [p if isinstance(p, tuple) else (p, None) for p in filter_post_data_parameters]
             filter_functions.append(
-                functools.partial(filters.replace_post_data_parameters, replacements=replacements)
+                functools.partial(filters.replace_post_data_parameters, replacements=replacements),
             )
 
         hosts_to_ignore = set(ignore_hosts)
         if ignore_localhost:
             hosts_to_ignore.update(("localhost", "0.0.0.0", "127.0.0.1"))
         if hosts_to_ignore:
             filter_functions.append(self._build_ignore_hosts(hosts_to_ignore))
@@ -249,9 +250,9 @@
 
     def register_persister(self, persister):
         # Singleton, no name required
         self.persister = persister
 
     def test_case(self, predicate=None):
         predicate = predicate or self.is_test_method
-        # TODO: Remove this reference to `six` in favor of the Python3 equivalent
-        return six.with_metaclass(auto_decorate(self.use_cassette, predicate))
+        metaclass = auto_decorate(self.use_cassette, predicate)
+        return metaclass("temporary_class", (), {})
```

### Comparing `vcrpy-5.0.0/vcr/errors.py` & `vcrpy-5.1.0/vcr/errors.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,34 +9,33 @@
     def _get_message(cassette, failed_request):
         """Get the final message related to the exception"""
         # Get the similar requests in the cassette that
         # have match the most with the request.
         best_matches = cassette.find_requests_with_most_matches(failed_request)
         if best_matches:
             # Build a comprehensible message to put in the exception.
-            best_matches_msg = "Found {} similar requests with {} different matcher(s) :\n".format(
-                len(best_matches), len(best_matches[0][2])
+            best_matches_msg = (
+                f"Found {len(best_matches)} similar requests "
+                f"with {len(best_matches[0][2])} different matcher(s) :\n"
             )
 
             for idx, best_match in enumerate(best_matches, start=1):
                 request, succeeded_matchers, failed_matchers_assertion_msgs = best_match
                 best_matches_msg += (
-                    "\n%s - (%r).\n"
-                    "Matchers succeeded : %s\n"
-                    "Matchers failed :\n" % (idx, request, succeeded_matchers)
+                    f"\n{idx} - ({request!r}).\n"
+                    f"Matchers succeeded : {succeeded_matchers}\n"
+                    "Matchers failed :\n"
                 )
                 for failed_matcher, assertion_msg in failed_matchers_assertion_msgs:
-                    best_matches_msg += "%s - assertion failure :\n" "%s\n" % (failed_matcher, assertion_msg)
+                    best_matches_msg += f"{failed_matcher} - assertion failure :\n{assertion_msg}\n"
         else:
             best_matches_msg = "No similar requests, that have not been played, found."
         return (
-            "Can't overwrite existing cassette (%r) in "
-            "your current record mode (%r).\n"
-            "No match for the request (%r) was found.\n"
-            "%s" % (cassette._path, cassette.record_mode, failed_request, best_matches_msg)
+            f"Can't overwrite existing cassette ({cassette._path!r}) in "
+            f"your current record mode ({cassette.record_mode!r}).\n"
+            f"No match for the request ({failed_request!r}) was found.\n"
+            f"{best_matches_msg}"
         )
 
 
 class UnhandledHTTPRequestError(KeyError):
     """Raised when a cassette does not contain the request we want."""
-
-    pass
```

### Comparing `vcrpy-5.0.0/vcr/filters.py` & `vcrpy-5.1.0/vcr/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     ov = new_body.pop(k)
                     if callable(rv):
                         rv = rv(key=k, value=ov, request=request)
                     if rv is not None:
                         new_body[k] = rv
             request.body = new_body
         elif request.headers.get("Content-Type") == "application/json":
-            json_data = json.loads(request.body.decode("utf-8"))
+            json_data = json.loads(request.body)
             for k, rv in replacements.items():
                 if k in json_data:
                     ov = json_data.pop(k)
                     if callable(rv):
                         rv = rv(key=k, value=ov, request=request)
                     if rv is not None:
                         json_data[k] = rv
```

### Comparing `vcrpy-5.0.0/vcr/migration.py` & `vcrpy-5.1.0/vcr/migration.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         return False
     interactions = _migrate(data)
     out_fp.write(serialize(interactions, jsonserializer))
     return True
 
 
 def _list_of_tuples_to_dict(fs):
-    return {k: v for k, v in fs[0]}
+    return dict(fs[0])
 
 
 def _already_migrated(data):
     try:
         if data.get("version") == 1:
             return True
     except AttributeError:
@@ -126,23 +126,23 @@
             shutil.copyfileobj(out_fp, in_fp)
         return True
 
 
 def try_migrate(path):
     if path.endswith(".json"):
         return migrate(path, migrate_json)
-    elif path.endswith(".yaml") or path.endswith(".yml"):
+    elif path.endswith((".yaml", ".yml")):
         return migrate(path, migrate_yml)
     return False
 
 
 def main():
     if len(sys.argv) != 2:
         raise SystemExit(
-            "Please provide path to cassettes directory or file. " "Usage: python3 -m vcr.migration PATH"
+            "Please provide path to cassettes directory or file. Usage: python3 -m vcr.migration PATH",
         )
 
     path = sys.argv[1]
     if not os.path.isabs(path):
         path = os.path.abspath(path)
     files = [path]
     if os.path.isdir(path):
```

### Comparing `vcrpy-5.0.0/vcr/patch.py` & `vcrpy-5.1.0/vcr/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     try:
         import botocore.vendored.requests  # noqa: F401
     except ImportError:  # pragma: no cover
         pass
     else:
         raise RuntimeError(
             "vcrpy >=4.2.2 and botocore <1.11.0 are not compatible"
-            "; please upgrade botocore (or downgrade vcrpy)"
+            "; please upgrade botocore (or downgrade vcrpy)",
         ) from e
 else:
     _Boto3VerifiedHTTPSConnection = AWSHTTPSConnection
     _cpoolBoto3HTTPConnection = AWSHTTPConnection
     _cpoolBoto3HTTPSConnection = AWSHTTPSConnection
 
 cpool = None
@@ -49,15 +49,15 @@
     import requests
 except ImportError:  # pragma: no cover
     pass
 else:
     if requests.__build__ < 0x021602:
         raise RuntimeError(
             "vcrpy >=4.2.2 and requests <2.16.2 are not compatible"
-            "; please upgrade requests (or downgrade vcrpy)"
+            "; please upgrade requests (or downgrade vcrpy)",
         )
 
 
 # Try to save the original types for httplib2
 try:
     import httplib2
 except ImportError:  # pragma: no cover
@@ -140,15 +140,17 @@
                 yield patcher
 
     def _build_patcher(self, obj, patched_attribute, replacement_class):
         if not hasattr(obj, patched_attribute):
             return
 
         return mock.patch.object(
-            obj, patched_attribute, self._recursively_apply_get_cassette_subclass(replacement_class)
+            obj,
+            patched_attribute,
+            self._recursively_apply_get_cassette_subclass(replacement_class),
         )
 
     def _recursively_apply_get_cassette_subclass(self, replacement_dict_or_obj):
         """One of the subtleties of this class is that it does not directly
         replace HTTPSConnection with `VCRRequestsHTTPSConnection`, but a
         subclass of the aforementioned class that has the `cassette`
         class attribute assigned to `self._cassette`. This behavior is
@@ -182,15 +184,15 @@
             self._class_to_cassette_subclass[klass] = subclass
         return self._class_to_cassette_subclass[klass]
 
     def _build_cassette_subclass(self, base_class):
         bases = (base_class,)
         if not issubclass(base_class, object):  # Check for old style class
             bases += (object,)
-        return type(f"{base_class.__name__}{self._cassette._path}", bases, dict(cassette=self._cassette))
+        return type(f"{base_class.__name__}{self._cassette._path}", bases, {"cassette": self._cassette})
 
     @_build_patchers_from_mock_triples_decorator
     def _httplib(self):
         yield httplib, "HTTPConnection", VCRHTTPConnection
         yield httplib, "HTTPSConnection", VCRHTTPSConnection
 
     def _requests(self):
@@ -329,18 +331,18 @@
             yield httpx.AsyncClient, "send", new_async_client_send
 
             new_sync_client_send = sync_vcr_send(self._cassette, _HttpxSyncClient_send)
             yield httpx.Client, "send", new_sync_client_send
 
     def _urllib3_patchers(self, cpool, conn, stubs):
         http_connection_remover = ConnectionRemover(
-            self._get_cassette_subclass(stubs.VCRRequestsHTTPConnection)
+            self._get_cassette_subclass(stubs.VCRRequestsHTTPConnection),
         )
         https_connection_remover = ConnectionRemover(
-            self._get_cassette_subclass(stubs.VCRRequestsHTTPSConnection)
+            self._get_cassette_subclass(stubs.VCRRequestsHTTPSConnection),
         )
         mock_triples = (
             (conn, "VerifiedHTTPSConnection", stubs.VCRRequestsHTTPSConnection),
             (conn, "HTTPConnection", stubs.VCRRequestsHTTPConnection),
             (conn, "HTTPSConnection", stubs.VCRRequestsHTTPSConnection),
             (cpool, "is_connection_dropped", mock.Mock(return_value=False)),  # Needed on Windows only
             (cpool.HTTPConnectionPool, "ConnectionCls", stubs.VCRRequestsHTTPConnection),
```

### Comparing `vcrpy-5.0.0/vcr/persisters/filesystem.py` & `vcrpy-5.1.0/vcr/persisters/filesystem.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/record_mode.py` & `vcrpy-5.1.0/vcr/record_mode.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/request.py` & `vcrpy-5.1.0/vcr/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,17 @@
     def body(self, value):
         if isinstance(value, str):
             value = value.encode("utf-8")
         self._body = value
 
     def add_header(self, key, value):
         warnings.warn(
-            "Request.add_header is deprecated. " "Please assign to request.headers instead.",
+            "Request.add_header is deprecated. Please assign to request.headers instead.",
             DeprecationWarning,
+            stacklevel=2,
         )
         self.headers[key] = value
 
     @property
     def scheme(self):
         return urlparse(self.uri).scheme
```

### Comparing `vcrpy-5.0.0/vcr/serialize.py` & `vcrpy-5.1.0/vcr/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return isinstance(data, list) and len(data) and "request" in data[0]
 
 
 def _warn_about_old_cassette_format():
     raise ValueError(
         "Your cassette files were generated in an older version "
         "of VCR. Delete your cassettes or run the migration script."
-        "See http://git.io/mHhLBg for more details."
+        "See http://git.io/mHhLBg for more details.",
     )
 
 
 def deserialize(cassette_string, serializer):
     try:
         data = serializer.deserialize(cassette_string)
     # Old cassettes used to use yaml object thingy so I have to
```

### Comparing `vcrpy-5.0.0/vcr/serializers/compat.py` & `vcrpy-5.1.0/vcr/serializers/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/__init__.py` & `vcrpy-5.1.0/vcr/stubs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,16 @@
         if self.cassette.can_play_response_for(self._vcr_request):
             log.info(f"Playing response for {self._vcr_request} from cassette")
             response = self.cassette.play_response(self._vcr_request)
             return VCRHTTPResponse(response)
         else:
             if self.cassette.write_protected and self.cassette.filter_request(self._vcr_request):
                 raise CannotOverwriteExistingCassetteException(
-                    cassette=self.cassette, failed_request=self._vcr_request
+                    cassette=self.cassette,
+                    failed_request=self._vcr_request,
                 )
 
             # Otherwise, we should send the request, then get the response
             # and return it.
 
             log.info(f"{self._vcr_request} not in cassette, sending to real server")
             # This is imported here to avoid circular import.
```

### Comparing `vcrpy-5.0.0/vcr/stubs/aiohttp_stubs.py` & `vcrpy-5.1.0/vcr/stubs/aiohttp_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             timer=None,
             request_info=request_info,
             traces=None,
             loop=asyncio.get_event_loop(),
             session=None,
         )
 
-    async def json(self, *, encoding="utf-8", loads=json.loads, **kwargs):  # NOQA: E999
+    async def json(self, *, encoding="utf-8", loads=json.loads, **kwargs):
         stripped = self._body.strip()
         if not stripped:
             return None
 
         return loads(stripped.decode(encoding))
 
     async def text(self, encoding="utf-8", errors="strict"):
@@ -62,15 +62,15 @@
 def build_response(vcr_request, vcr_response, history):
     request_info = RequestInfo(
         url=URL(vcr_request.url),
         method=vcr_request.method,
         headers=_deserialize_headers(vcr_request.headers),
         real_url=URL(vcr_request.url),
     )
-    response = MockClientResponse(vcr_request.method, URL(vcr_response.get("url")), request_info=request_info)
+    response = MockClientResponse(vcr_request.method, URL(vcr_request.url), request_info=request_info)
     response.status = vcr_response["status"]["code"]
     response._body = vcr_response["body"].get("string", b"")
     response.reason = vcr_response["status"]["message"]
     response._headers = _deserialize_headers(vcr_response["headers"])
     response._history = tuple(history)
     # cookies
     for hdr in response.headers.getall(hdrs.SET_COOKIE, ()):
@@ -158,16 +158,15 @@
     # there is no body. We can use this to know to not write one.
     except ClientConnectionError:
         body = {}
 
     vcr_response = {
         "status": {"code": response.status, "message": response.reason},
         "headers": _serialize_headers(response.headers),
-        "body": body,  # NOQA: E999
-        "url": str(response.url),
+        "body": body,
     }
 
     cassette.append(vcr_request, vcr_response)
 
 
 async def record_responses(cassette, vcr_request, response):
     """Because aiohttp follows redirects by default, we must support
@@ -269,12 +268,12 @@
             return response
 
         if cassette.write_protected and cassette.filter_request(vcr_request):
             raise CannotOverwriteExistingCassetteException(cassette=cassette, failed_request=vcr_request)
 
         log.info("%s not in cassette, sending to real server", vcr_request)
 
-        response = await real_request(self, method, url, **kwargs)  # NOQA: E999
+        response = await real_request(self, method, url, **kwargs)
         await record_responses(cassette, vcr_request, response)
         return response
 
     return new_request
```

### Comparing `vcrpy-5.0.0/vcr/stubs/boto3_stubs.py` & `vcrpy-5.1.0/vcr/stubs/boto3_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/compat.py` & `vcrpy-5.1.0/vcr/stubs/compat.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/httplib2_stubs.py` & `vcrpy-5.1.0/vcr/stubs/httplib2_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/httpx_stubs.py` & `vcrpy-5.1.0/vcr/stubs/httpx_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/requests_stubs.py` & `vcrpy-5.1.0/vcr/stubs/requests_stubs.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/stubs/tornado_stubs.py` & `vcrpy-5.1.0/vcr/stubs/tornado_stubs.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
             or request.streaming_callback is not None
         )
         if unsupported_call:
             response = HTTPResponse(
                 request,
                 599,
                 error=Exception(
-                    "The request (%s) uses AsyncHTTPClient functionality "
+                    f"The request ({request!r}) uses AsyncHTTPClient functionality "
                     "that is not yet supported by VCR.py. Please make the "
-                    "request outside a VCR.py context." % repr(request)
+                    "request outside a VCR.py context.",
                 ),
                 request_time=self.io_loop.time() - request.start_time,
             )
             return callback(response)
 
         vcr_request = Request(request.method, request.url, request.body, headers)
 
@@ -61,15 +61,16 @@
             return callback(response)
         else:
             if cassette.write_protected and cassette.filter_request(vcr_request):
                 response = HTTPResponse(
                     request,
                     599,
                     error=CannotOverwriteExistingCassetteException(
-                        cassette=cassette, failed_request=vcr_request
+                        cassette=cassette,
+                        failed_request=vcr_request,
                     ),
                     request_time=self.io_loop.time() - request.start_time,
                 )
                 return callback(response)
 
             def new_callback(response):
                 headers = [(k, response.headers.get_list(k)) for k in response.headers.keys()]
```

### Comparing `vcrpy-5.0.0/vcr/unittest.py` & `vcrpy-5.1.0/vcr/unittest.py`

 * *Files identical despite different names*

### Comparing `vcrpy-5.0.0/vcr/util.py` & `vcrpy-5.1.0/vcr/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     of how the header name was originally stored.
     If the constructor, ``.update``, or equality comparison
     operations are given keys that have equal ``.lower()``s, the
     behavior is undefined.
     """
 
     def __init__(self, data=None, **kwargs):
-        self._store = dict()
+        self._store = {}
         if data is None:
             data = {}
         self.update(data, **kwargs)
 
     def __setitem__(self, key, value):
         # Use the lowercased key for lookups, but store the actual
         # key alongside the value.
```

### Comparing `vcrpy-5.0.0/vcrpy.egg-info/PKG-INFO` & `vcrpy-5.1.0/vcrpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcrpy
-Version: 5.0.0
+Version: 5.1.0
 Summary: Automatically mock your HTTP interactions to simplify and speed up testing
 Home-page: https://github.com/kevin1024/vcrpy
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `vcrpy-5.0.0/vcrpy.egg-info/SOURCES.txt` & `vcrpy-5.1.0/vcrpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

