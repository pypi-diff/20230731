# Comparing `tmp/imandra-0.1.9.tar.gz` & `tmp/imandra-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/imandra-0.1.9.tar", last modified: Wed Aug 28 13:21:06 2019, max compression
+gzip compressed data, was "imandra-1.0.0.tar", last modified: Mon Jul 31 18:17:27 2023, max compression
```

## Comparing `imandra-0.1.9.tar` & `imandra-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,105 @@
-drwxr-xr-x   0 kanishev  (1000) kanishev  (1000)        0 2019-08-28 13:21:06.000000 imandra-0.1.9/
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     2410 2019-08-28 13:21:06.000000 imandra-0.1.9/PKG-INFO
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)      689 2019-08-28 12:10:39.000000 imandra-0.1.9/setup.py
-drwxr-xr-x   0 kanishev  (1000) kanishev  (1000)        0 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra/
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     3723 2019-08-27 21:34:01.000000 imandra-0.1.9/imandra/auth.py
-drwxr-xr-x   0 kanishev  (1000) kanishev  (1000)        0 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra/idf/
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     2071 2019-08-28 11:50:11.000000 imandra-0.1.9/imandra/idf/sampler.py
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     1239 2019-08-27 21:34:01.000000 imandra-0.1.9/imandra/idf/decomposition.py
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)      805 2019-08-28 12:08:23.000000 imandra-0.1.9/imandra/idf/__init__.py
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     1937 2019-08-27 21:34:01.000000 imandra-0.1.9/imandra/idf/exception.py
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)       17 2019-08-27 21:34:01.000000 imandra-0.1.9/imandra/__init__.py
-drwxr-xr-x   0 kanishev  (1000) kanishev  (1000)        0 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)        9 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/requires.txt
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     2410 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/PKG-INFO
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)      309 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/SOURCES.txt
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)        8 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/top_level.txt
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)        1 2019-08-28 13:21:06.000000 imandra-0.1.9/imandra.egg-info/dependency_links.txt
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)     1659 2019-08-27 21:34:01.000000 imandra-0.1.9/README.md
--rw-r--r--   0 kanishev  (1000) kanishev  (1000)       38 2019-08-28 13:21:06.000000 imandra-0.1.9/setup.cfg
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.548035 imandra-1.0.0/
+-rw-r--r--   0 dave       (501) staff       (20)     5003 2023-07-31 18:17:27.547807 imandra-1.0.0/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     4608 2023-07-31 18:15:50.000000 imandra-1.0.0/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.515861 imandra-1.0.0/docs/
+-rw-r--r--   0 dave       (501) staff       (20)     4815 2023-07-31 13:35:13.000000 imandra-1.0.0/docs/README.md
+-rw-r--r--   0 dave       (501) staff       (20)      536 2023-07-31 18:17:22.000000 imandra-1.0.0/pyproject.toml
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-07-31 18:17:27.548120 imandra-1.0.0/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)       92 2023-07-28 16:24:50.000000 imandra-1.0.0/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.513872 imandra-1.0.0/src/
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.520455 imandra-1.0.0/src/imandra/
+-rw-r--r--   0 dave       (501) staff       (20)     7645 2023-07-28 16:24:50.000000 imandra-1.0.0/src/imandra/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)    12146 2023-07-29 09:01:15.000000 imandra-1.0.0/src/imandra/auth.py
+-rw-r--r--   0 dave       (501) staff       (20)     1324 2023-07-21 15:18:58.000000 imandra-1.0.0/src/imandra/cfb.py
+-rw-r--r--   0 dave       (501) staff       (20)      795 2023-07-21 15:18:58.000000 imandra-1.0.0/src/imandra/core.py
+-rw-r--r--   0 dave       (501) staff       (20)     1963 2023-07-28 16:24:50.000000 imandra-1.0.0/src/imandra/instance.py
+-rw-r--r--   0 dave       (501) staff       (20)     5088 2023-07-21 15:18:58.000000 imandra-1.0.0/src/imandra/ipl.py
+-rw-r--r--   0 dave       (501) staff       (20)      902 2023-07-21 15:18:58.000000 imandra-1.0.0/src/imandra/rule_synth.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.524798 imandra-1.0.0/src/imandra.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)     5003 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)     4540 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)       45 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/entry_points.txt
+-rw-r--r--   0 dave       (501) staff       (20)       99 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/requires.txt
+-rw-r--r--   0 dave       (501) staff       (20)       32 2023-07-31 18:17:27.000000 imandra-1.0.0/src/imandra.egg-info/top_level.txt
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.526841 imandra-1.0.0/src/imandra_http_api_client/
+-rw-r--r--   0 dave       (501) staff       (20)     3520 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/__init__.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.527218 imandra-1.0.0/src/imandra_http_api_client/api/
+-rw-r--r--   0 dave       (501) staff       (20)      111 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/api/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)    56187 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/api/default_api.py
+-rw-r--r--   0 dave       (501) staff       (20)    30152 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/api_client.py
+-rw-r--r--   0 dave       (501) staff       (20)      844 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/api_response.py
+-rw-r--r--   0 dave       (501) staff       (20)    14774 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/configuration.py
+-rw-r--r--   0 dave       (501) staff       (20)     5397 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/exceptions.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.536544 imandra-1.0.0/src/imandra_http_api_client/models/
+-rw-r--r--   0 dave       (501) staff       (20)     2832 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     2162 2023-07-31 11:23:33.000000 imandra-1.0.0/src/imandra_http_api_client/models/eval_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     2143 2023-07-31 11:23:33.000000 imandra-1.0.0/src/imandra_http_api_client/models/eval_response.py
+-rw-r--r--   0 dave       (501) staff       (20)     2128 2023-07-31 11:23:33.000000 imandra-1.0.0/src/imandra_http_api_client/models/hints.py
+-rw-r--r--   0 dave       (501) staff       (20)     1983 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/induct_functional_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2199 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/induct_structural_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      863 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/induct_structural_style.py
+-rw-r--r--   0 dave       (501) staff       (20)      828 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/induct_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     2872 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/instance_request_name.py
+-rw-r--r--   0 dave       (501) staff       (20)     3036 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/instance_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     2436 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/instance_response.py
+-rw-r--r--   0 dave       (501) staff       (20)      854 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/instance_result.py
+-rw-r--r--   0 dave       (501) staff       (20)      818 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/instance_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     2311 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method.py
+-rw-r--r--   0 dave       (501) staff       (20)     5985 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1991 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_ext_solver_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2433 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_induct_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     5425 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_induct_body_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      836 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     1971 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/method_unroll_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2395 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/printer_details.py
+-rw-r--r--   0 dave       (501) staff       (20)     2130 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/response_error.py
+-rw-r--r--   0 dave       (501) staff       (20)     2504 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/response_instance.py
+-rw-r--r--   0 dave       (501) staff       (20)     2165 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/response_model.py
+-rw-r--r--   0 dave       (501) staff       (20)      886 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/syntax.py
+-rw-r--r--   0 dave       (501) staff       (20)     1996 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/up_to_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2856 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/verify_request_name.py
+-rw-r--r--   0 dave       (501) staff       (20)     3020 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/verify_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     2414 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/verify_response.py
+-rw-r--r--   0 dave       (501) staff       (20)     5997 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/verify_response_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      856 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/verify_result.py
+-rw-r--r--   0 dave       (501) staff       (20)     2275 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/with_instance_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2023 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/models/with_unknown_reason_body.py
+-rw-r--r--   0 dave       (501) staff       (20)    12976 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/rest.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.546799 imandra-1.0.0/src/imandra_http_api_client/test/
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-07-31 11:23:34.000000 imandra-1.0.0/src/imandra_http_api_client/test/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)     2876 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_default_api.py
+-rw-r--r--   0 dave       (501) staff       (20)     1660 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_eval_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     1673 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_eval_response.py
+-rw-r--r--   0 dave       (501) staff       (20)     1753 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_hints.py
+-rw-r--r--   0 dave       (501) staff       (20)     1705 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_induct_functional_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1874 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_induct_structural_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      937 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_induct_structural_style.py
+-rw-r--r--   0 dave       (501) staff       (20)      859 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_induct_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     2090 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_instance_request_name.py
+-rw-r--r--   0 dave       (501) staff       (20)     2109 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_instance_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     1691 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_instance_response.py
+-rw-r--r--   0 dave       (501) staff       (20)      887 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_instance_result.py
+-rw-r--r--   0 dave       (501) staff       (20)      873 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_instance_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     1571 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method.py
+-rw-r--r--   0 dave       (501) staff       (20)     1713 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1664 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_ext_solver_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1703 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_induct_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1935 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_induct_body_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      859 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_type.py
+-rw-r--r--   0 dave       (501) staff       (20)     1627 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_method_unroll_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1696 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_printer_details.py
+-rw-r--r--   0 dave       (501) staff       (20)     1677 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_response_error.py
+-rw-r--r--   0 dave       (501) staff       (20)     1821 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_response_instance.py
+-rw-r--r--   0 dave       (501) staff       (20)     1620 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_response_model.py
+-rw-r--r--   0 dave       (501) staff       (20)      830 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_syntax.py
+-rw-r--r--   0 dave       (501) staff       (20)     1588 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_up_to_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     2066 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_verify_request_name.py
+-rw-r--r--   0 dave       (501) staff       (20)     2085 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_verify_request_src.py
+-rw-r--r--   0 dave       (501) staff       (20)     1669 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_verify_response.py
+-rw-r--r--   0 dave       (501) staff       (20)     2466 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_verify_response_body.py
+-rw-r--r--   0 dave       (501) staff       (20)      873 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_verify_result.py
+-rw-r--r--   0 dave       (501) staff       (20)     2281 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_with_instance_body.py
+-rw-r--r--   0 dave       (501) staff       (20)     1735 2023-07-30 12:26:26.000000 imandra-1.0.0/src/imandra_http_api_client/test/test_with_unknown_reason_body.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-07-31 18:17:27.547503 imandra-1.0.0/tests/
+-rw-r--r--   0 dave       (501) staff       (20)     2408 2023-07-31 14:17:09.000000 imandra-1.0.0/tests/test_imandra_http_api.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

