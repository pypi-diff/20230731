# Comparing `tmp/prismstudio-dev-1.1.7a0.tar.gz` & `tmp/prismstudio-dev-1.1.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-dev-1.1.7a0.tar", last modified: Tue Jul 25 13:58:11 2023, max compression
+gzip compressed data, was "prismstudio-dev-1.1.7b0.tar", last modified: Mon Jul 31 08:10:11 2023, max compression
```

## Comparing `prismstudio-dev-1.1.7a0.tar` & `prismstudio-dev-1.1.7b0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/
--rw-rw-r--   0 prism     (1000) prism     (1000)    23016 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7a0/LICENSE.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      446 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/PKG-INFO
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1177 2023-07-07 08:39:02.000000 prismstudio-dev-1.1.7a0/prism/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/_common/
--rw-rw-r--   0 prism     (1000) prism     (1000)       29 2023-07-25 13:58:08.000000 prismstudio-dev-1.1.7a0/prism/_common/.env
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_common/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3472 2023-07-09 08:26:49.000000 prismstudio-dev-1.1.7a0/prism/_common/config.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    11029 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_common/const.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.250202 prismstudio-dev-1.1.7a0/prism/_core/
--rw-rw-r--   0 prism     (1000) prism     (1000)      288 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/__init__.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_core/_data/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10231 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/esg.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    41180 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/estimate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7950 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/event.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    70894 2023-07-09 08:09:32.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/financial.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    12927 2023-07-15 00:59:57.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/index.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   121051 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/industry.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    37342 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/market.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6446 2023-06-16 00:01:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/precalculated.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3840 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_data/securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15625 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_fn.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/
--rw-rw-r--   0 prism     (1000) prism     (1000)     1458 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2074 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_auth.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    22677 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dataquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2058 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dbinfo.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7633 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_exportdata.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3633 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_gui.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15003 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_job.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4828 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_list.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15321 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_portfolio.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     4295 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_securitymaster.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    25699 2023-06-15 23:39:09.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_task.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    10877 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_taskquery.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    24533 2023-06-14 16:37:45.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_universe.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     8696 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/_req_builder/preference.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     9606 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_core/ols.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_prismcomponent/
--rw-rw-r--   0 prism     (1000) prism     (1000)      353 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7644 2023-07-15 01:00:00.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/abstract_prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    12663 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/datacomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)   186982 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/prismcomponent.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    21567 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7a0/prism/_prismcomponent/taskcomponent.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prism/_utils/
--rw-rw-r--   0 prism     (1000) prism     (1000)      480 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2248 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/auth_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3629 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/exceptions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2028 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/loader.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3706 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/prismcomponent_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5532 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/req_builder_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    14289 2023-07-18 01:25:58.000000 prismstudio-dev-1.1.7a0/prism/_utils/validate_utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     7232 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/prism/_utils/validate_utils_refactored.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1438 2023-07-07 02:42:51.000000 prismstudio-dev-1.1.7a0/prism/_utils/version.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/
--rw-rw-r--   0 prism     (1000) prism     (1000)      446 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/PKG-INFO
--rw-rw-r--   0 prism     (1000) prism     (1000)     3097 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)        1 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      242 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/requires.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)       12 2023-07-25 13:58:11.000000 prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/top_level.txt
--rw-rw-r--   0 prism     (1000) prism     (1000)      137 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/pyproject.toml
--rw-rw-r--   0 prism     (1000) prism     (1000)       38 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/setup.cfg
--rw-rw-r--   0 prism     (1000) prism     (1000)     1316 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/setup.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/tests/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)       94 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/conftest.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test__validate_args/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2200 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_common_functions.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1539 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_fillna.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     5990 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_01_frequency.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2004 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_02_datetype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2719 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_03_periodtype.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1615 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_04_adjustment.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2304 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_05_shownid.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1946 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_06_rank_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2302 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_07_method.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     6448 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     3854 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1717 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1118 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_11_base.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1792 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_12_preliminary.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      889 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_13_setting.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      956 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_14_settings.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2441 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_factors.py
-drwxrwxr-x   0 prism     (1000) prism     (1000)        0 2023-07-25 13:58:11.254202 prismstudio-dev-1.1.7a0/tests/test_util/
--rw-rw-r--   0 prism     (1000) prism     (1000)        0 2023-06-12 06:52:36.000000 prismstudio-dev-1.1.7a0/tests/test_util/__init__.py
--rw-rw-r--   0 prism     (1000) prism     (1000)      603 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/db_fixtures.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1264 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/dq_model.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1753 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/dq_table.py
--rw-rw-r--   0 prism     (1000) prism     (1000)    15617 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/factor_fixtures.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     2738 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/update_factor.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1259 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_util/utils.py
--rw-rw-r--   0 prism     (1000) prism     (1000)     1770 2023-07-25 13:56:42.000000 prismstudio-dev-1.1.7a0/tests/test_version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.130908 prismstudio-dev-1.1.7b0/
+-rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/LICENSE.txt
+-rw-r--r--   0 prism      (501) staff       (20)      446 2023-07-31 08:10:11.130767 prismstudio-dev-1.1.7b0/PKG-INFO
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.119454 prismstudio-dev-1.1.7b0/prism/
+-rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 08:09:55.000000 prismstudio-dev-1.1.7b0/prism/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.119916 prismstudio-dev-1.1.7b0/prism/_common/
+-rw-r--r--   0 prism      (501) staff       (20)       29 2023-07-31 08:10:04.000000 prismstudio-dev-1.1.7b0/prism/_common/.env
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_common/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     3472 2023-07-31 05:54:47.000000 prismstudio-dev-1.1.7b0/prism/_common/config.py
+-rw-r--r--   0 prism      (501) staff       (20)    11029 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_common/const.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.120332 prismstudio-dev-1.1.7b0/prism/_core/
+-rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.122115 prismstudio-dev-1.1.7b0/prism/_core/_data/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/esg.py
+-rw-r--r--   0 prism      (501) staff       (20)    41180 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/estimate.py
+-rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/event.py
+-rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/financial.py
+-rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/index.py
+-rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/industry.py
+-rw-r--r--   0 prism      (501) staff       (20)    43804 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/market.py
+-rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/precalculated.py
+-rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_fn.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.123890 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/
+-rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_auth.py
+-rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dataquery.py
+-rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dbinfo.py
+-rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_exportdata.py
+-rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_gui.py
+-rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_job.py
+-rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_list.py
+-rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_portfolio.py
+-rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_task.py
+-rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_taskquery.py
+-rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_universe.py
+-rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/preference.py
+-rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/ols.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.124608 prismstudio-dev-1.1.7b0/prism/_prismcomponent/
+-rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    12663 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/datacomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/taskcomponent.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.126146 prismstudio-dev-1.1.7b0/prism/_utils/
+-rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/auth_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/exceptions.py
+-rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/loader.py
+-rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/prismcomponent_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/req_builder_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/validate_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/validate_utils_refactored.py
+-rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-dev-1.1.7b0/prism/_utils/version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127037 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/
+-rw-r--r--   0 prism      (501) staff       (20)      446 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/PKG-INFO
+-rw-r--r--   0 prism      (501) staff       (20)     3097 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 prism      (501) staff       (20)        1 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 prism      (501) staff       (20)      242 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/requires.txt
+-rw-r--r--   0 prism      (501) staff       (20)       12 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/top_level.txt
+-rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/pyproject.toml
+-rw-r--r--   0 prism      (501) staff       (20)       38 2023-07-31 08:10:11.130950 prismstudio-dev-1.1.7b0/setup.cfg
+-rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/setup.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127535 prismstudio-dev-1.1.7b0/tests/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/tests/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/conftest.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127869 prismstudio-dev-1.1.7b0/tests/test__validate_args/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_common_functions.py
+-rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_fillna.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.129688 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_01_frequency.py
+-rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_02_datetype.py
+-rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_05_shownid.py
+-rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_07_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_11_base.py
+-rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_13_setting.py
+-rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_14_settings.py
+-rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_factors.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.130559 prismstudio-dev-1.1.7b0/tests/test_util/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/tests/test_util/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/db_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/dq_model.py
+-rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/dq_table.py
+-rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/factor_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/update_factor.py
+-rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_version.py
```

### Comparing `prismstudio-dev-1.1.7a0/LICENSE.txt` & `prismstudio-dev-1.1.7b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/__init__.py` & `prismstudio-dev-1.1.7b0/prism/__init__.py`

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

### Comparing `prismstudio-dev-1.1.7a0/prism/_common/config.py` & `prismstudio-dev-1.1.7b0/prism/_common/config.py`

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

### Comparing `prismstudio-dev-1.1.7a0/prism/_common/const.py` & `prismstudio-dev-1.1.7b0/prism/_common/const.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/estimate.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/estimate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/event.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/financial.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/index.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/index.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/industry.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/market.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     'volume',
     'dividend',
     'exchange_rate',
     'short_interest',
     'split',
     'split_adjustment_factor',
     'dividend_adjustment_factor',
-    'dataitems',
-    'short_interest_dataitems',
     'shares_outstanding',
     'enterprise_value',
-    'implied_market_cap'
+    'implied_market_cap',
+    'dataitems',
+    'short_interest_dataitems'
 ]
 
 
 @_validate_args
 def _build_price(
     datacomponentclass,
     adjustment: Union[str, bool] = None,
@@ -844,17 +844,136 @@
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
@@ -888,15 +1007,15 @@
 
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
@@ -925,22 +1044,7 @@
         4     1100058          Short Interest as % Of Free Float  ...        None  IHS Markit Short Interest
         5     1100059  Short Interest as % Of Shares Outstanding  ...        None  IHS Markit Short Interest
         6     1100060                                Short Score  ...        None  IHS Markit Short Interest
         7     1100063           Supply Side Short Interest Value  ...        None  IHS Markit Short Interest
     """
 
     return _list_dataitem_market(_MarketDataComponentType.SHORT_INTEREST, search, package)
-
-
-@_validate_args
-def shares_outstanding(adjustment: Union[str, bool] = True):
-    return _SharesOutstanding(adjustment=adjustment)
-
-
-@_validate_args
-def enterprise_value(currency: str = 'trade'):
-    return _TotalEnterpriseValue(currency=currency)
-
-
-@_validate_args
-def implied_market_cap(include: str = 'all', currency: str = 'trade'):
-    return _ImpliedMarketCapitalization(include=include, currency=currency)
```

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/precalculated.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_data/securitymaster.py` & `prismstudio-dev-1.1.7b0/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_fn.py` & `prismstudio-dev-1.1.7b0/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/__init__.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_auth.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_auth.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dataquery.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dataquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_exportdata.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_gui.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_job.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_list.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_list.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_portfolio.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_task.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_taskquery.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/_universe.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/_req_builder/preference.py` & `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_core/ols.py` & `prismstudio-dev-1.1.7b0/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-dev-1.1.7b0/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_prismcomponent/datacomponent.py` & `prismstudio-dev-1.1.7b0/prism/_prismcomponent/datacomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_prismcomponent/prismcomponent.py` & `prismstudio-dev-1.1.7b0/prism/_prismcomponent/prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_prismcomponent/taskcomponent.py` & `prismstudio-dev-1.1.7b0/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/auth_utils.py` & `prismstudio-dev-1.1.7b0/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/exceptions.py` & `prismstudio-dev-1.1.7b0/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/loader.py` & `prismstudio-dev-1.1.7b0/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/prismcomponent_utils.py` & `prismstudio-dev-1.1.7b0/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/req_builder_utils.py` & `prismstudio-dev-1.1.7b0/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/validate_utils.py` & `prismstudio-dev-1.1.7b0/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/validate_utils_refactored.py` & `prismstudio-dev-1.1.7b0/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prism/_utils/version.py` & `prismstudio-dev-1.1.7b0/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/prismstudio_dev.egg-info/SOURCES.txt` & `prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/setup.py` & `prismstudio-dev-1.1.7b0/setup.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_common_functions.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_fillna.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_factors.py` & `prismstudio-dev-1.1.7b0/tests/test_factors.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/db_fixtures.py` & `prismstudio-dev-1.1.7b0/tests/test_util/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/dq_model.py` & `prismstudio-dev-1.1.7b0/tests/test_util/dq_model.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/dq_table.py` & `prismstudio-dev-1.1.7b0/tests/test_util/dq_table.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/factor_fixtures.py` & `prismstudio-dev-1.1.7b0/tests/test_util/factor_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/update_factor.py` & `prismstudio-dev-1.1.7b0/tests/test_util/update_factor.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_util/utils.py` & `prismstudio-dev-1.1.7b0/tests/test_util/utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7a0/tests/test_version.py` & `prismstudio-dev-1.1.7b0/tests/test_version.py`

 * *Files identical despite different names*

