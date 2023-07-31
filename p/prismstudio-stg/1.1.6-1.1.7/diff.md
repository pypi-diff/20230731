# Comparing `tmp/prismstudio-stg-1.1.6.tar.gz` & `tmp/prismstudio-stg-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-stg-1.1.6.tar", last modified: Sun Jul  9 09:14:11 2023, max compression
+gzip compressed data, was "prismstudio-stg-1.1.7.tar", last modified: Mon Jul 31 09:21:13 2023, max compression
```

## Comparing `prismstudio-stg-1.1.6.tar` & `prismstudio-stg-1.1.7.tar`

### file list

```diff
@@ -1,89 +1,101 @@
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/
--rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-09 08:09:32.000000 prismstudio-stg-1.1.6/LICENSE.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/PKG-INFO
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.165009 prismstudio-stg-1.1.6/prism/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-stg-1.1.6/prism/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.165009 prismstudio-stg-1.1.6/prism/_common/
--rw-rw-r--   0 prism     (1000) prism     (1000)       28 2023-07-09 09:14:08.000000 prismstudio-stg-1.1.6/prism/_common/.env
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_common/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3472 2023-07-09 08:26:49.000000 prismstudio-stg-1.1.6/prism/_common/config.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10161 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_common/const.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.165009 prismstudio-stg-1.1.6/prism/_core/
--rw-rw-r--   0 prism     (1000) prism     (1000)      251 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.165009 prismstudio-stg-1.1.6/prism/_core/_data/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_data/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    41177 2023-06-16 00:01:45.000000 prismstudio-stg-1.1.6/prism/_core/_data/estimate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-stg-1.1.6/prism/_core/_data/event.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-09 08:09:32.000000 prismstudio-stg-1.1.6/prism/_core/_data/financial.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    12859 2023-06-27 09:00:21.000000 prismstudio-stg-1.1.6/prism/_core/_data/index.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-stg-1.1.6/prism/_core/_data/industry.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    36768 2023-07-07 02:42:51.000000 prismstudio-stg-1.1.6/prism/_core/_data/market.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-stg-1.1.6/prism/_core/_data/precalculated.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_core/_data/securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-stg-1.1.6/prism/_core/_fn.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/prism/_core/_req_builder/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2074 2023-07-09 08:16:15.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_auth.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    22657 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_dataquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_dbinfo.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_exportdata.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_gui.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_job.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4582 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_list.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_portfolio.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_task.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_taskquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/_universe.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/_req_builder/preference.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_core/ols.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/prism/_prismcomponent/
--rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_prismcomponent/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7323 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_prismcomponent/abstract_prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14370 2023-06-14 16:37:45.000000 prismstudio-stg-1.1.6/prism/_prismcomponent/datacomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   185597 2023-06-15 23:39:09.000000 prismstudio-stg-1.1.6/prism/_prismcomponent/prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-stg-1.1.6/prism/_prismcomponent/taskcomponent.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/prism/_utils/
--rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/auth_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/exceptions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/loader.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/prismcomponent_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/req_builder_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/validate_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/prism/_utils/validate_utils_refactored.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-stg-1.1.6/prism/_utils/version.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/
--rw-rw-r--   0 prism     (1000) prism     (1000)      444 2023-07-09 09:14:11.000000 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/PKG-INFO
--rw-rw-r--   0 prism     (1000) prism     (1000)     3042 2023-07-09 09:14:11.000000 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/SOURCES.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-09 09:14:11.000000 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/dependency_links.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      256 2023-07-09 09:14:11.000000 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/requires.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-09 09:14:11.000000 prismstudio-stg-1.1.6/prismstudio_stg.egg-info/top_level.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       91 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/pyproject.toml
--rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/setup.cfg
--rw-rw-r--   0 prism     (1000) prism     (1000)     1341 2023-07-09 08:09:32.000000 prismstudio-stg-1.1.6/setup.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/tests/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/tests/test_util/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_common_functions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_fillna.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-09 09:14:11.169010 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_07_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_11_base.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_13_setting.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-06-12 06:52:36.000000 prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_14_settings.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-07 02:42:51.000000 prismstudio-stg-1.1.6/tests/test_util/test_version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.127843 prismstudio-stg-1.1.7/
+-rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/LICENSE.txt
+-rw-r--r--   0 prism      (501) staff       (20)      444 2023-07-31 09:21:13.127713 prismstudio-stg-1.1.7/PKG-INFO
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.116936 prismstudio-stg-1.1.7/prism/
+-rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 08:09:55.000000 prismstudio-stg-1.1.7/prism/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.117384 prismstudio-stg-1.1.7/prism/_common/
+-rw-r--r--   0 prism      (501) staff       (20)       28 2023-07-31 09:21:09.000000 prismstudio-stg-1.1.7/prism/_common/.env
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_common/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     3472 2023-07-31 05:54:47.000000 prismstudio-stg-1.1.7/prism/_common/config.py
+-rw-r--r--   0 prism      (501) staff       (20)    11029 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/prism/_common/const.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.117858 prismstudio-stg-1.1.7/prism/_core/
+-rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/prism/_core/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.119544 prismstudio-stg-1.1.7/prism/_core/_data/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 05:53:59.000000 prismstudio-stg-1.1.7/prism/_core/_data/esg.py
+-rw-r--r--   0 prism      (501) staff       (20)    41180 2023-07-24 01:11:04.000000 prismstudio-stg-1.1.7/prism/_core/_data/estimate.py
+-rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/event.py
+-rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/financial.py
+-rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-24 01:11:04.000000 prismstudio-stg-1.1.7/prism/_core/_data/index.py
+-rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/industry.py
+-rw-r--r--   0 prism      (501) staff       (20)    43804 2023-07-31 05:53:59.000000 prismstudio-stg-1.1.7/prism/_core/_data/market.py
+-rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/precalculated.py
+-rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_data/securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_fn.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.119820 prismstudio-stg-1.1.7/prism/_core/_model/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 08:14:33.000000 prismstudio-stg-1.1.7/prism/_core/_model/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5246 2023-07-31 08:09:55.000000 prismstudio-stg-1.1.7/prism/_core/_model/tcmodel.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.121878 prismstudio-stg-1.1.7/prism/_core/_req_builder/
+-rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_auth.py
+-rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_dataquery.py
+-rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_dbinfo.py
+-rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_exportdata.py
+-rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_gui.py
+-rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_job.py
+-rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-24 01:11:04.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_list.py
+-rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_portfolio.py
+-rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_task.py
+-rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_taskquery.py
+-rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/_universe.py
+-rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/_req_builder/preference.py
+-rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_core/ols.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.122587 prismstudio-stg-1.1.7/prism/_prismcomponent/
+-rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_prismcomponent/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-24 01:11:04.000000 prismstudio-stg-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    12663 2023-07-24 01:11:04.000000 prismstudio-stg-1.1.7/prism/_prismcomponent/datacomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/prism/_prismcomponent/prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_prismcomponent/taskcomponent.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.123636 prismstudio-stg-1.1.7/prism/_utils/
+-rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/auth_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/exceptions.py
+-rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/loader.py
+-rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/prismcomponent_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/req_builder_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/validate_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/prism/_utils/validate_utils_refactored.py
+-rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-stg-1.1.7/prism/_utils/version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.124207 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/
+-rw-r--r--   0 prism      (501) staff       (20)      444 2023-07-31 09:21:13.000000 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/PKG-INFO
+-rw-r--r--   0 prism      (501) staff       (20)     3158 2023-07-31 09:21:13.000000 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/SOURCES.txt
+-rw-r--r--   0 prism      (501) staff       (20)        1 2023-07-31 09:21:13.000000 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/dependency_links.txt
+-rw-r--r--   0 prism      (501) staff       (20)      242 2023-07-31 09:21:13.000000 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/requires.txt
+-rw-r--r--   0 prism      (501) staff       (20)       12 2023-07-31 09:21:13.000000 prismstudio-stg-1.1.7/prismstudio_stg.egg-info/top_level.txt
+-rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/pyproject.toml
+-rw-r--r--   0 prism      (501) staff       (20)       38 2023-07-31 09:21:13.127879 prismstudio-stg-1.1.7/setup.cfg
+-rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/setup.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.124649 prismstudio-stg-1.1.7/tests/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/tests/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/conftest.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.124977 prismstudio-stg-1.1.7/tests/test__validate_args/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_common_functions.py
+-rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_fillna.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.126700 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_01_frequency.py
+-rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_02_datetype.py
+-rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_05_shownid.py
+-rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_07_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_11_base.py
+-rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_13_setting.py
+-rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_14_settings.py
+-rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_factors.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 09:21:13.127524 prismstudio-stg-1.1.7/tests/test_util/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-stg-1.1.7/tests/test_util/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/db_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/dq_model.py
+-rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/dq_table.py
+-rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/factor_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/update_factor.py
+-rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_util/utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 05:53:38.000000 prismstudio-stg-1.1.7/tests/test_version.py
```

### Comparing `prismstudio-stg-1.1.6/LICENSE.txt` & `prismstudio-stg-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/__init__.py` & `prismstudio-stg-1.1.7/prism/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 import inspect
 import IPython
 from ._core import *
-from ._core import _data, ols
+from ._core import _data, ols, _model
 from ._core._req_builder import preference
 from ._utils.version import __version__
 from ._utils.validate_utils import handle_sys_exception, handle_jupyter_exception
 from ._prismcomponent import (
     _AbstractPrismComponent,
     _PrismComponent,
     _PrismFinancialComponent,
@@ -20,14 +20,16 @@
 _username = ''
 quiet_mode = False
 
 IPython.core.interactiveshell.InteractiveShell.showtraceback = handle_jupyter_exception(IPython.core.interactiveshell.InteractiveShell.showtraceback)
 sys.excepthook = handle_sys_exception
 
 _data_pkg_list = inspect.getmembers(_data, inspect.ismodule)
+_model_list = inspect.getmembers(_model, inspect.ismodule)
+_data_pkg_list = _data_pkg_list + _model_list
 for pkg_name, pkg in _data_pkg_list:
     new_pkg_name = f"{__name__}.{pkg_name}"
     if new_pkg_name not in sys.modules.keys():
         pkg.__name__ = new_pkg_name  # Will have no effect; see below
         sys.modules[new_pkg_name] = pkg
 
 # ols module
```

### Comparing `prismstudio-stg-1.1.6/prism/_common/config.py` & `prismstudio-stg-1.1.7/prism/_common/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     STAGING = "stg"
     PRODUCTION = "production"
     DEMO = "demo"
 
 
 class StateSettings(BaseSettings):
     ENV_STATE: EnvironmentState = 'production'
-    VERSION: str = '1.1.6'
+    VERSION: str = '1.1.7'
     URL_STABLE: str = 'https://api.prism39.com'
     URL_DEV: str = 'https://ops.prism39.com'
     dev: str = ':30495'
     stg: str = ':30496'
     demo: str = ':40452'
 
     class Config:
```

### Comparing `prismstudio-stg-1.1.6/prism/_common/const.py` & `prismstudio-stg-1.1.7/prism/_common/const.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,24 +29,31 @@
     'BeyondType',
     'COMPONENT2CATEGORY',
     'FUNCTIONS',
     'FILEEXTENSION',
     'AggregateComponents',
     'PACKAGE_NAME',
     'SPECIALVALUEMAP',
+    'DataCategoryType',
 ]
 
 BEGINNING_DATE = pd.to_datetime('1700-01-01')
 ACTIVE_DATE = pd.to_datetime('2199-12-31')
 
 
 class PrismComponentType(str, Enum):
     FUNCTION_COMPONENT = 'functioncomponent'
     DATA_COMPONENT = 'datacomponent'
     TASK_COMPONENT = 'taskcomponent'
+    MODEL_COMPONENT = 'modelcomponent'
+
+
+class TCModelComponentType(str, Enum):
+    ALMGREN = "Almgren"
+    BIDASKSPREAD = "Bid-Ask Spread"
 
 
 SMValues = None
 PreferenceType = None
 
 
 class AdjustmentType(Enum):
@@ -127,14 +134,38 @@
 
 class TaskComponentType(str, Enum):
     SCREEN = 'screen'
     FACTOR_BACKTEST = 'factor_backtest'
     STRATEGY_BACKTEST = 'strategy_backtest'
     EXPORT_DATA = 'export_data'
 
+
+class PrismModelCategoryType(str, Enum):
+    TC = "Transaction Cost"
+
+class DataCategoryType(str, Enum):
+    FINANCIAL = "Financial"
+    PRECALCAULATED = "Precalculated"
+    EVENT = "Event"
+    SM = "Securitymaster"
+    MARKET = "Market"
+    ESTIMATE = "Estimate"
+    INDEX = "Index"
+    INDUSTRY_ESTIMATE = "Industry Estimate"
+    INDUSTRY_FINANCIAL = "Industry"
+    ESG = "ESG"
+
+
+class ESGDataComponentType(str, Enum):
+    ENVIRONMENTAL = 'Environmental'
+    SOCIAL = 'Social'
+    GOVERNANCE = 'Governance'
+    SUMMARY = 'Summary'
+
+
 class FinancialDataComponentType(str, Enum):
     BALANCE_SHEET = 'Balance Sheet'
     CASH_FLOW = 'Cash Flow'
     DPS = 'DPS'
     EPS = 'EPS'
     FINANCIAL_DATE = 'Financial Date'
     INCOME_STATEMENT = 'Income Statement'
@@ -166,14 +197,17 @@
     VOLUME = 'Volume'
     DIVIDEND = 'Dividend'
     DIVIDEND_ADJ_FACTOR = 'Dividend Adjustment Factor'
     EXCHANGERATE = 'Exchange Rate'
     SHORT_INTEREST = 'Short Interest'
     SPLIT = 'Split'
     SPLIT_ADJ_FACTOR = 'Split Adjustment Factor'
+    SHARES_OUTSTANDING = 'Shares Outstanding'
+    TOTAL_ENTERPRISE_VALUE = 'Total Enterprise Value'
+    IMPLIED_MARKET_CAPITALIZATION = 'Implied Market Capitalization'
 
 
 class PrecalculatedDataComponentType(str, Enum):
     AFL = 'Alpha Factor Library'
 
 
 class IndexDataComponentType(str, Enum):
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/estimate.py` & `prismstudio-stg-1.1.7/prism/_core/_data/estimate.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
     -------
         prism._PrismComponent
 
     Examples
     --------
         >>> di = prism.estimate.surprise_dataitems('revenue')
         >>> di[['dataitemid', 'dataitemname']]
-        dataitemid                   dataitemname
+           dataitemid                   dataitemname
         0      200618  Revenue - Surpise, Difference
         1      200619     Revenue - Surpise, Percent
 
         >>> rev = prism.estimate.surprise(dataitemid=200618, periodtype='Q')
         >>> rev_df = rev.get_data(universe='S&P 500', startdate='2010-01-01', enddate='2015-12-31', shownid=['ticker'])
         >>> rev_df
                listingid      period        date  EPS Normalized - Surpise, Difference  Ticker
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/event.py` & `prismstudio-stg-1.1.7/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/financial.py` & `prismstudio-stg-1.1.7/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/index.py` & `prismstudio-stg-1.1.7/prism/_core/_data/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     | Default frequency is business daily.
 
     Parameters
     ----------
         dataitemid : int
             | Unique identifier for the different data item. This identifies the type of the balance sheet value (Revenue, Expense, etc.)
 
-        leveltype : str, {'Price Return', 'Total Return Gross'}
+        leveltype : str, default None, {'Price Return', 'Total Return Gross'}
+            | Default value None gives all leveltype.
 
     Returns
     -------
         prism._PrismComponent
 
     Examples
     --------
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/industry.py` & `prismstudio-stg-1.1.7/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/market.py` & `prismstudio-stg-1.1.7/prism/_core/_data/market.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     _Volume,
     _Dividend,
     _DividendAdjustmentFactor,
     _Split,
     _SplitAdjustmentFactor,
     _ExchangeRate,
     _ShortInterest,
+    _SharesOutstanding,
+    _TotalEnterpriseValue,
+    _ImpliedMarketCapitalization
 )
 from ..._utils.validate_utils import _validate_args
 
 
 __all__ = [
     'open',
     'close',
@@ -34,16 +37,19 @@
     'volume',
     'dividend',
     'exchange_rate',
     'short_interest',
     'split',
     'split_adjustment_factor',
     'dividend_adjustment_factor',
+    'shares_outstanding',
+    'enterprise_value',
+    'implied_market_cap',
     'dataitems',
-    'short_interest_dataitems',
+    'short_interest_dataitems'
 ]
 
 
 @_validate_args
 def _build_price(
     datacomponentclass,
     adjustment: Union[str, bool] = None,
@@ -838,17 +844,136 @@
         305530  278631846  2015-12-30        6.464626e+10  A028260
         305531  278631846  2015-12-31        6.800626e+10  A028260
     """
     return _ShortInterest(dataitemid=dataitemid, package=package)
 
 
 @_validate_args
+def shares_outstanding(adjustment: bool = True):
+    """
+    | The total number of shares of a security that are currently held by all its shareholders and are available for trading on a specific stock exchange.
+    | Default frequency is daily.
+
+    Parameters
+    ----------
+    adjustment : bool, default True
+        | Adjustment for Shares outstanding
+
+    Returns
+    -------
+        prism._PrismComponent
+
+    Examples
+    --------
+        >>> shares_out = prism.market.shares_outstanding()
+        >>> shares_out.get_data("Semiconductor", "2020-01-01", shownid=['Company Name'])
+                  listingid        date      shares                                       Company Name
+        0           2586491  2020-01-01    39521782                                          AXT, Inc.
+        1           2587243  2020-01-01    22740986                                  Aehr Test Systems
+        2           2587303  2020-01-01  1138599272                       Advanced Micro Devices, Inc.
+        3           2587347  2020-01-01    38308569                   Advanced Energy Industries, Inc.
+        4           2589783  2020-01-01   239783075                             Amkor Technology, Inc.
+        ...             ...         ...         ...                                                ...
+        1168126  1831385562  2023-07-26     7501500                                        SEALSQ Corp
+        1168127  1833187092  2023-07-26    12675758                                  GigaVis Co., Ltd.
+        1168128  1833609849  2023-07-26  7021800000  Semiconductor Manufacturing Electronics (Shaox...
+        1168129  1834641950  2023-07-26   452506348     Smarter Microelectronics (Guangzhou) Co., Ltd.
+        1168130  1838168164  2023-07-26    37844925              Integrated Solutions Technology, Inc.
+    """
+    return _SharesOutstanding(adjustment=adjustment)
+
+
+@_validate_args
+def enterprise_value(currency: str = None):
+    """
+    | Represents the total value of a company, taking into account its market capitalization, outstanding debt, cash, and other financial assets.
+    | It is used to determine the true cost of acquiring a company and is calculated as market capitalization plus total debt minus cash and cash equivalents.
+    | Default frequency is daily.
+
+    Parameters
+    ----------
+    currency : str, {'trade', 'report', ISO3 currency}, default None
+            | Desired currency for the enterprise value data.
+
+            - trade : trading currency for a given listing (i.e for Apple - USD, Tencent - HKD)
+            - report : financial reporting currency for a given listing (i.e for Apple - USD, Tencent - CNY)
+            - ISO3 currency : desired currency in ISO 4217 format (i.e USD, EUR, JPY, KRW, etc.)
+            - None : dividend payment currency
+
+    Returns
+    -------
+        prism._PrismComponent
+
+    Examples
+    --------
+        >>> ent_val = prism.market.enterprise_value(currency='trade')
+        >>> ent_val.get_data("Semi", "2020-01-01", shownid=['Company Name'])
+                  listingid        date           tev  currency                                       Company Name
+        0           2586491  2020-01-01  1.546798e+08       USD                                          AXT, Inc.
+        1           2587243  2020-01-01  4.288797e+07       USD                                  Aehr Test Systems
+        2           2587303  2020-01-01  5.211816e+10       USD                       Advanced Micro Devices, Inc.
+        3           2587347  2020-01-01  2.842980e+09       USD                   Advanced Energy Industries, Inc.
+        4           2589783  2020-01-01  3.988825e+09       USD                             Amkor Technology, Inc.
+        ...             ...         ...           ...       ...                                                ...
+        1167719  1831385562  2023-07-25  1.645610e+08       USD                                        SEALSQ Corp
+        1167720  1833187092  2023-07-25           NaN       KRW                                  GigaVis Co., Ltd.
+        1167721  1833609849  2023-07-25  5.481000e+10       CNY  Semiconductor Manufacturing Electronics (Shaox...
+        1167722  1834641950  2023-07-25  9.114210e+09       CNY     Smarter Microelectronics (Guangzhou) Co., Ltd.
+        1167723  1838168164  2023-07-25           NaN       TWD              Integrated Solutions Technology, Inc.
+    """
+    return _TotalEnterpriseValue(currency=currency)
+
+
+@_validate_args
+def implied_market_cap(dilution: str = 'all', currency: str = None):
+    """
+    | Theoretical total value of a company's outstanding shares, including potential dilution from stock options and other equity-based compensation plans.
+    | Default frequency is daily.
+
+    Parameters
+    ----------
+    dilution : str, {'all', 'partner', 'exercisable'}, default 'all'
+            | Options whether to include which potential dilution from stock options and other equity-based compensation plans.
+
+    currency : str, {'trade', 'report', ISO3 currency}, default None
+            | Desired currency for the pricing data.
+
+            - trade : trading currency for a given listing (i.e for Apple - USD, Tencent - HKD)
+            - report : financial reporting currency for a given listing (i.e for Apple - USD, Tencent - CNY)
+            - ISO3 currency : desired currency in ISO 4217 format (i.e USD, EUR, JPY, KRW, etc.)
+            - None : dividend payment currency
+
+    Returns
+    -------
+        prism._PrismComponent
+
+    Examples
+    --------
+             listingid        date    implieddilutedmarketcapout  currency               Company Name
+        0    707934944  2021-06-24                  1.317918e+09       USD  indie Semiconductor, Inc.
+        1    707934944  2021-06-25                  1.335508e+09       USD  indie Semiconductor, Inc.
+        2    707934944  2021-06-26                  1.335508e+09       USD  indie Semiconductor, Inc.
+        3    707934944  2021-06-27                  1.335508e+09       USD  indie Semiconductor, Inc.
+        4    707934944  2021-06-28                  1.332802e+09       USD  indie Semiconductor, Inc.
+        ...        ...         ...                           ...       ...                        ...
+        762  707934944  2023-07-26                  1.485848e+09       USD  indie Semiconductor, Inc.
+        763  707934944  2023-07-27                  1.464184e+09       USD  indie Semiconductor, Inc.
+        764  707934944  2023-07-28                  1.502095e+09       USD  indie Semiconductor, Inc.
+        765  707934944  2023-07-29                  1.502095e+09       USD  indie Semiconductor, Inc.
+        766  707934944  2023-07-30                  1.502095e+09       USD  indie Semiconductor, Inc.
+
+
+    """
+    return _ImpliedMarketCapitalization(dilution=dilution, currency=currency)
+
+
+@_validate_args
 def dataitems(search : str = None, package : str = None):
     """
-    Usable dataitems for the market data categories.
+    | Usable dataitems for the market data categories.
 
     Parameters
     ----------
         search : str, default None
             | Search word for Data Items name, the search is case-insensitive.
         package : str, default None
             | Search word for package name, the search is case-insensitive.
@@ -882,15 +1007,15 @@
 
     return _list_dataitem_market(None, search, package)
 
 
 @_validate_args
 def short_interest_dataitems(search : str = None, package : str = None):
     """
-    Usable data items for the short_interest data component.
+    | Usable data items for the short_interest data component.
 
     Parameters
     ----------
         search : str, default None
             | Search word for data items name, the search is case-insensitive.
         package : str, default None
             | Search word for package name, the search is case-insensitive.
@@ -907,15 +1032,15 @@
             - *datamodule : str*
             - *datacomponent : str*
             - *packagename : str*
 
     Examples
     --------
         >>> prism.market.short_interest_dataitems(search='short')
-           dataitemid                               dataitemname  ...  datamodule                packagename
+           dataitemid         ;                      dataitemname  ...  datamodule                packagename
         0     1100035                Broker Short Interest Value  ...        None  IHS Markit Short Interest
         1     1100055        Short Interest Ratio (Day to Cover)  ...        None  IHS Markit Short Interest
         2     1100056                      Short Interest Tenure  ...        None  IHS Markit Short Interest
         3     1100057                       Short Interest Value  ...        None  IHS Markit Short Interest
         4     1100058          Short Interest as % Of Free Float  ...        None  IHS Markit Short Interest
         5     1100059  Short Interest as % Of Shares Outstanding  ...        None  IHS Markit Short Interest
         6     1100060                                Short Score  ...        None  IHS Markit Short Interest
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/precalculated.py` & `prismstudio-stg-1.1.7/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_data/securitymaster.py` & `prismstudio-stg-1.1.7/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_fn.py` & `prismstudio-stg-1.1.7/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/__init__.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_auth.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_auth.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_dataquery.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_dataquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,15 +403,15 @@
     cmpts = set()
     if isinstance(name, list) & (name is not None):
         if any([not isinstance(n, str) for n in name]):
             raise PrismTypeError('Names shoud be string')
 
     def add_cmpts(o):
         cmpts = set()
-        if o["component_type"] == "datacomponent":
+        if o["component_type"] in ["datacomponent", "modelcomponent"]:
             cmpts.add(o["component_name"])
         else:
             for c in o["children"]:
                 cmpts = cmpts | add_cmpts(c)
         return cmpts
 
     if not isinstance(component, list):
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_exportdata.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_gui.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_job.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_list.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,20 +92,26 @@
 @_validate_args
 def _list_dataitem_estimate(datacomponent, search : str = None, package : str = None):
     param = {'datacategory': 'Estimate', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
-def _list_dataitem_market(datacomponent: str, search : str = None, package : str = None):
+def _list_dataitem_market(datacomponent: str, search : str = None, package: str = None):
     param = {'datacategory': 'Market', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
+def _list_dataitems_esg(datacomponent: str, search: str = None, package: str = None):
+    param = {'datacategory': 'ESG', 'datacomponent': datacomponent, 'search': search, 'package': package}
+    return get(URL_DATAITEMS, param)
+
+
+@_validate_args
 def _list_dataitem_precalculated(datacomponent: str, search : str = None, package : str = None):
     param = {'datacategory': 'Precalculated', 'datacomponent': datacomponent, 'search': search, 'package': package}
     return get(URL_DATAITEMS, param)
 
 
 @_validate_args
 def _list_dataitem_index(datacomponent: str, search : str = None, package : str = None):
```

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_portfolio.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_task.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_taskquery.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/_universe.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/_req_builder/preference.py` & `prismstudio-stg-1.1.7/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_core/ols.py` & `prismstudio-stg-1.1.7/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-stg-1.1.7/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,23 +22,27 @@
     def __init__(
         self,
         *,
         component_type: str,
         component_name: str,
         component_args: dict = {},
         children: list,
+        component_category: str = None,
         nodeid: UUID = None,
         query_name: str = None,
     ):
         # if not hasattr(self, '_func_name'): self._func_name = func_name
         if component_type == PrismComponentType.FUNCTION_COMPONENT:
             if not hasattr(self, "_component_name"):
                 self._component_name = component_name
+            if not hasattr(self, "_component_category"):
+                self._component_category = component_category
         self._query = {
             "component_type": component_type,
+            "component_category": component_category,
             "component_name": component_name,
             "component_args": component_args,
             "children": children,
             "nodeid": nodeid,
         }
         try:
             json.dumps(self._query)
@@ -59,15 +63,15 @@
             except:
                 pass
         else:
             try:
                 print(
                     "\t" * depth,
                     "====",
-                    query["component_name"],
+                    query["component_category"] + "/" + query["component_name"] if query["component_category"] is not None else query["component_name"],
                 )
                 if len(query["component_args"]) > 0:
                     print(
                         "\t" * (depth + 1),
                         "parameters: {",
                     )
                     for k, v in query["component_args"].items():
```

### Comparing `prismstudio-stg-1.1.6/prism/_prismcomponent/prismcomponent.py` & `prismstudio-stg-1.1.7/prism/_prismcomponent/prismcomponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             755975  344286611  2011-10-31   45.6     ITT
         """
         ...
 
     @operation
     def floor(self):
         """
-        The floor value of each element. The floor of x i.e., the largest integer not greater than x. 
+        The floor value of each element. The floor of x i.e., the largest integer not greater than x.
 
         Returns
         -------
             prism._PrismComponent
                 The floor of each element, with ``float`` dtype. This is a scalar if element is a scalar.
 
         Examples
@@ -4168,14 +4168,15 @@
 
     _component_type = PrismComponentType.DATA_COMPONENT
 
     def __init__(self, **kwargs):
         component_args = dict(kwargs)
         query = {
             "component_type": self._component_type,
+            "component_category": self._component_category,
             "component_name": self._component_name,
             "component_args": component_args,
             "children": [],
             "nodeid": str(uuid.uuid4()),
         }
         val_res = requests.post(url=URL_DATAQUERIES + "/validate", json=query, headers=_authentication())
         if val_res.status_code >= 400:
@@ -4193,18 +4194,29 @@
 
     @property
     @classmethod
     @abstractmethod
     def _component_name():
         raise NotImplementedError()
 
+
+    @property
+    @classmethod
+    @abstractmethod
+    def _component_category():
+        raise NotImplementedError()
+
+
     def __setattr__(self, name, value):
         if name == "_component_name":
             raise AttributeError("Can't modify {}".format(name))
 
+        if name == "_component_category":
+            raise AttributeError("Can't modify {}".format(name))
+
         super().__setattr__(name, value)
 
 
 class _PrismTaskComponent(_AbstractPrismComponent, ABC):
     _component_type = PrismComponentType.TASK_COMPONENT
 
     def __init__(self, **kwargs):
@@ -4241,16 +4253,14 @@
             "component_args": component_args,
             "children": [],
         }
         super().__init__(**query)
 
 
 class _PrismFinancialComponent(_PrismComponent):
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
 
     @_validate_args
     @n_period_operation
     @operation
     def n_fiscal_quarters_max(self, n: int, weights: list = None):
         """
         Return the maximum of the values over given fiscal quarter n.
@@ -4538,7 +4548,36 @@
         Returns
         -------
             prism._PrismFinancialComponent
                 n fiscal quarters sum timeseries of the PrismFinancialComponent.
         """
         if (weights is not None) and (len(weights) != n):
             raise PrismValueError("Number of weights should equal to n")
+
+
+class _PrismModelComponent(_PrismComponent):
+    _component_type = PrismComponentType.MODEL_COMPONENT
+
+    def __init__(self, **kwargs):
+        component_args = dict(kwargs)
+        children = [] if "children" not in component_args else component_args.pop("children")
+        query = {
+            "component_type": self._component_type,
+            "component_category": self._component_category,
+            "component_name": self._component_name,
+            "component_args": component_args,
+            "children": children,
+            "nodeid": str(uuid.uuid4()),
+        }
+        val_res = requests.post(url=URL_DATAQUERIES + "/validate", json=query, headers=_authentication())
+        if val_res.status_code >= 400:
+            if val_res.status_code == 401:
+                raise PrismAuthError(f"Please Login First")
+            else:
+                try:
+                    err_msg = val_res.json()["message"]
+                except:
+                    err_msg = val_res.content
+                raise PrismResponseError(err_msg)
+        query = val_res.json()["rescontent"]["data"]
+        query.pop("query_name")
+        super().__init__(**query)
```

### Comparing `prismstudio-stg-1.1.6/prism/_prismcomponent/taskcomponent.py` & `prismstudio-stg-1.1.7/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/auth_utils.py` & `prismstudio-stg-1.1.7/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/exceptions.py` & `prismstudio-stg-1.1.7/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/loader.py` & `prismstudio-stg-1.1.7/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/prismcomponent_utils.py` & `prismstudio-stg-1.1.7/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/req_builder_utils.py` & `prismstudio-stg-1.1.7/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/validate_utils.py` & `prismstudio-stg-1.1.7/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/validate_utils_refactored.py` & `prismstudio-stg-1.1.7/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prism/_utils/version.py` & `prismstudio-stg-1.1.7/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/prismstudio_stg.egg-info/SOURCES.txt` & `prismstudio-stg-1.1.7/prismstudio_stg.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 prism/_common/__init__.py
 prism/_common/config.py
 prism/_common/const.py
 prism/_core/__init__.py
 prism/_core/_fn.py
 prism/_core/ols.py
 prism/_core/_data/__init__.py
+prism/_core/_data/esg.py
 prism/_core/_data/estimate.py
 prism/_core/_data/event.py
 prism/_core/_data/financial.py
 prism/_core/_data/index.py
 prism/_core/_data/industry.py
 prism/_core/_data/market.py
 prism/_core/_data/precalculated.py
 prism/_core/_data/securitymaster.py
+prism/_core/_model/__init__.py
+prism/_core/_model/tcmodel.py
 prism/_core/_req_builder/__init__.py
 prism/_core/_req_builder/_auth.py
 prism/_core/_req_builder/_dataquery.py
 prism/_core/_req_builder/_dbinfo.py
 prism/_core/_req_builder/_exportdata.py
 prism/_core/_req_builder/_gui.py
 prism/_core/_req_builder/_job.py
@@ -48,27 +51,35 @@
 prism/_utils/version.py
 prismstudio_stg.egg-info/PKG-INFO
 prismstudio_stg.egg-info/SOURCES.txt
 prismstudio_stg.egg-info/dependency_links.txt
 prismstudio_stg.egg-info/requires.txt
 prismstudio_stg.egg-info/top_level.txt
 tests/__init__.py
+tests/conftest.py
+tests/test_factors.py
+tests/test_version.py
+tests/test__validate_args/__init__.py
+tests/test__validate_args/test_common_functions.py
+tests/test__validate_args/test_fillna.py
+tests/test__validate_args/test_params/__init__.py
+tests/test__validate_args/test_params/test_param_01_frequency.py
+tests/test__validate_args/test_params/test_param_02_datetype.py
+tests/test__validate_args/test_params/test_param_03_periodtype.py
+tests/test__validate_args/test_params/test_param_04_adjustment.py
+tests/test__validate_args/test_params/test_param_05_shownid.py
+tests/test__validate_args/test_params/test_param_06_rank_method.py
+tests/test__validate_args/test_params/test_param_07_method.py
+tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+tests/test__validate_args/test_params/test_param_09_contains_universename.py
+tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+tests/test__validate_args/test_params/test_param_11_base.py
+tests/test__validate_args/test_params/test_param_12_preliminary.py
+tests/test__validate_args/test_params/test_param_13_setting.py
+tests/test__validate_args/test_params/test_param_14_settings.py
 tests/test_util/__init__.py
-tests/test_util/test_version.py
-tests/test_util/test__validate_args/__init__.py
-tests/test_util/test__validate_args/test_common_functions.py
-tests/test_util/test__validate_args/test_fillna.py
-tests/test_util/test__validate_args/test_params/__init__.py
-tests/test_util/test__validate_args/test_params/test_param_01_frequency.py
-tests/test_util/test__validate_args/test_params/test_param_02_datetype.py
-tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py
-tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py
-tests/test_util/test__validate_args/test_params/test_param_05_shownid.py
-tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py
-tests/test_util/test__validate_args/test_params/test_param_07_method.py
-tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
-tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py
-tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py
-tests/test_util/test__validate_args/test_params/test_param_11_base.py
-tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py
-tests/test_util/test__validate_args/test_params/test_param_13_setting.py
-tests/test_util/test__validate_args/test_params/test_param_14_settings.py
+tests/test_util/db_fixtures.py
+tests/test_util/dq_model.py
+tests/test_util/dq_table.py
+tests/test_util/factor_fixtures.py
+tests/test_util/update_factor.py
+tests/test_util/utils.py
```

### Comparing `prismstudio-stg-1.1.6/setup.py` & `prismstudio-stg-1.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     data_files=datafiles,
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     install_requires=[
-        "pandas==1.4.1",
-        "pytest==7.1.1",
+        "pandas==2.0.3",
         "mypy==0.941",
         "pyarrow==8.0.0",
         "multivolumefile==0.2.3",
         "urllib3==1.26.9",
         "tqdm==4.64.0",
         "orjson==3.7.3",
         "ipywidgets==7.7.1",
```

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_common_functions.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_fillna.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-stg-1.1.7/tests/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-stg-1.1.6/tests/test_util/test_version.py` & `prismstudio-stg-1.1.7/tests/test_version.py`

 * *Files identical despite different names*

