# Comparing `tmp/prismstudio-dev-1.1.7b0.tar.gz` & `tmp/prismstudio-dev-1.1.7rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismstudio-dev-1.1.7b0.tar", last modified: Mon Jul 31 08:10:11 2023, max compression
+gzip compressed data, was "prismstudio-dev-1.1.7rc0.tar", last modified: Mon Jul 31 08:16:24 2023, max compression
```

## Comparing `prismstudio-dev-1.1.7b0.tar` & `prismstudio-dev-1.1.7rc0.tar`

### file list

```diff
@@ -1,98 +1,101 @@
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.130908 prismstudio-dev-1.1.7b0/
--rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/LICENSE.txt
--rw-r--r--   0 prism      (501) staff       (20)      446 2023-07-31 08:10:11.130767 prismstudio-dev-1.1.7b0/PKG-INFO
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.119454 prismstudio-dev-1.1.7b0/prism/
--rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 08:09:55.000000 prismstudio-dev-1.1.7b0/prism/__init__.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.119916 prismstudio-dev-1.1.7b0/prism/_common/
--rw-r--r--   0 prism      (501) staff       (20)       29 2023-07-31 08:10:04.000000 prismstudio-dev-1.1.7b0/prism/_common/.env
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_common/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     3472 2023-07-31 05:54:47.000000 prismstudio-dev-1.1.7b0/prism/_common/config.py
--rw-r--r--   0 prism      (501) staff       (20)    11029 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_common/const.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.120332 prismstudio-dev-1.1.7b0/prism/_core/
--rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/__init__.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.122115 prismstudio-dev-1.1.7b0/prism/_core/_data/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/esg.py
--rw-r--r--   0 prism      (501) staff       (20)    41180 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/estimate.py
--rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/event.py
--rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/financial.py
--rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/index.py
--rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/industry.py
--rw-r--r--   0 prism      (501) staff       (20)    43804 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/market.py
--rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/precalculated.py
--rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_data/securitymaster.py
--rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_fn.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.123890 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/
--rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_auth.py
--rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dataquery.py
--rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dbinfo.py
--rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_exportdata.py
--rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_gui.py
--rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_job.py
--rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_list.py
--rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_portfolio.py
--rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_securitymaster.py
--rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_task.py
--rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_taskquery.py
--rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_universe.py
--rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/_req_builder/preference.py
--rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_core/ols.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.124608 prismstudio-dev-1.1.7b0/prism/_prismcomponent/
--rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/abstract_prismcomponent.py
--rw-r--r--   0 prism      (501) staff       (20)    12663 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/datacomponent.py
--rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/prismcomponent.py
--rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_prismcomponent/taskcomponent.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.126146 prismstudio-dev-1.1.7b0/prism/_utils/
--rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/auth_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/exceptions.py
--rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/loader.py
--rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/prismcomponent_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/req_builder_utils.py
--rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/validate_utils.py
--rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/prism/_utils/validate_utils_refactored.py
--rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-dev-1.1.7b0/prism/_utils/version.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127037 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/
--rw-r--r--   0 prism      (501) staff       (20)      446 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/PKG-INFO
--rw-r--r--   0 prism      (501) staff       (20)     3097 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/SOURCES.txt
--rw-r--r--   0 prism      (501) staff       (20)        1 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/dependency_links.txt
--rw-r--r--   0 prism      (501) staff       (20)      242 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/requires.txt
--rw-r--r--   0 prism      (501) staff       (20)       12 2023-07-31 08:10:11.000000 prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/top_level.txt
--rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/pyproject.toml
--rw-r--r--   0 prism      (501) staff       (20)       38 2023-07-31 08:10:11.130950 prismstudio-dev-1.1.7b0/setup.cfg
--rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/setup.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127535 prismstudio-dev-1.1.7b0/tests/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/tests/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/conftest.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.127869 prismstudio-dev-1.1.7b0/tests/test__validate_args/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_common_functions.py
--rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_fillna.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.129688 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_01_frequency.py
--rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_02_datetype.py
--rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_03_periodtype.py
--rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_04_adjustment.py
--rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_05_shownid.py
--rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_06_rank_method.py
--rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_07_method.py
--rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
--rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_09_contains_universename.py
--rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
--rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_11_base.py
--rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_12_preliminary.py
--rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_13_setting.py
--rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_14_settings.py
--rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_factors.py
-drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:10:11.130559 prismstudio-dev-1.1.7b0/tests/test_util/
--rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7b0/tests/test_util/__init__.py
--rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/db_fixtures.py
--rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/dq_model.py
--rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/dq_table.py
--rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/factor_fixtures.py
--rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/update_factor.py
--rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_util/utils.py
--rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7b0/tests/test_version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.818335 prismstudio-dev-1.1.7rc0/
+-rw-r--r--   0 prism      (501) staff       (20)    23016 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/LICENSE.txt
+-rw-r--r--   0 prism      (501) staff       (20)      447 2023-07-31 08:16:24.818192 prismstudio-dev-1.1.7rc0/PKG-INFO
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.807000 prismstudio-dev-1.1.7rc0/prism/
+-rw-r--r--   0 prism      (501) staff       (20)     1290 2023-07-31 08:09:55.000000 prismstudio-dev-1.1.7rc0/prism/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.807493 prismstudio-dev-1.1.7rc0/prism/_common/
+-rw-r--r--   0 prism      (501) staff       (20)       29 2023-07-31 08:16:21.000000 prismstudio-dev-1.1.7rc0/prism/_common/.env
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_common/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     3472 2023-07-31 05:54:47.000000 prismstudio-dev-1.1.7rc0/prism/_common/config.py
+-rw-r--r--   0 prism      (501) staff       (20)    11029 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/prism/_common/const.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.807825 prismstudio-dev-1.1.7rc0/prism/_core/
+-rw-r--r--   0 prism      (501) staff       (20)      288 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/prism/_core/__init__.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.809189 prismstudio-dev-1.1.7rc0/prism/_core/_data/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)    17869 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/esg.py
+-rw-r--r--   0 prism      (501) staff       (20)    41180 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/estimate.py
+-rw-r--r--   0 prism      (501) staff       (20)     7950 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/event.py
+-rw-r--r--   0 prism      (501) staff       (20)    70894 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/financial.py
+-rw-r--r--   0 prism      (501) staff       (20)    12927 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/index.py
+-rw-r--r--   0 prism      (501) staff       (20)   121051 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/industry.py
+-rw-r--r--   0 prism      (501) staff       (20)    43804 2023-07-31 05:53:59.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/market.py
+-rw-r--r--   0 prism      (501) staff       (20)     6446 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/precalculated.py
+-rw-r--r--   0 prism      (501) staff       (20)     3840 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_data/securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    15625 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_fn.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.809447 prismstudio-dev-1.1.7rc0/prism/_core/_model/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 08:14:33.000000 prismstudio-dev-1.1.7rc0/prism/_core/_model/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5246 2023-07-31 08:09:55.000000 prismstudio-dev-1.1.7rc0/prism/_core/_model/tcmodel.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.811468 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/
+-rw-r--r--   0 prism      (501) staff       (20)     1458 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2074 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_auth.py
+-rw-r--r--   0 prism      (501) staff       (20)    22677 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_dataquery.py
+-rw-r--r--   0 prism      (501) staff       (20)     2058 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_dbinfo.py
+-rw-r--r--   0 prism      (501) staff       (20)     7633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_exportdata.py
+-rw-r--r--   0 prism      (501) staff       (20)     3633 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_gui.py
+-rw-r--r--   0 prism      (501) staff       (20)    15003 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_job.py
+-rw-r--r--   0 prism      (501) staff       (20)     4828 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_list.py
+-rw-r--r--   0 prism      (501) staff       (20)    15321 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_portfolio.py
+-rw-r--r--   0 prism      (501) staff       (20)     4295 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_securitymaster.py
+-rw-r--r--   0 prism      (501) staff       (20)    25699 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_task.py
+-rw-r--r--   0 prism      (501) staff       (20)    10877 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_taskquery.py
+-rw-r--r--   0 prism      (501) staff       (20)    24533 2023-07-24 00:59:28.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_universe.py
+-rw-r--r--   0 prism      (501) staff       (20)     8696 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/preference.py
+-rw-r--r--   0 prism      (501) staff       (20)     9606 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_core/ols.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.812457 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/
+-rw-r--r--   0 prism      (501) staff       (20)      353 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     7644 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/abstract_prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    12663 2023-07-24 01:11:04.000000 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/datacomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)   186982 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/prismcomponent.py
+-rw-r--r--   0 prism      (501) staff       (20)    21567 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_prismcomponent/taskcomponent.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.813571 prismstudio-dev-1.1.7rc0/prism/_utils/
+-rw-r--r--   0 prism      (501) staff       (20)      480 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2248 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/auth_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     3629 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/exceptions.py
+-rw-r--r--   0 prism      (501) staff       (20)     2028 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/loader.py
+-rw-r--r--   0 prism      (501) staff       (20)     3706 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/prismcomponent_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     5532 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/req_builder_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)    14289 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/validate_utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     7232 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/prism/_utils/validate_utils_refactored.py
+-rw-r--r--   0 prism      (501) staff       (20)     1438 2023-07-24 00:59:23.000000 prismstudio-dev-1.1.7rc0/prism/_utils/version.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.814193 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/
+-rw-r--r--   0 prism      (501) staff       (20)      447 2023-07-31 08:16:24.000000 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/PKG-INFO
+-rw-r--r--   0 prism      (501) staff       (20)     3158 2023-07-31 08:16:24.000000 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 prism      (501) staff       (20)        1 2023-07-31 08:16:24.000000 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 prism      (501) staff       (20)      242 2023-07-31 08:16:24.000000 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/requires.txt
+-rw-r--r--   0 prism      (501) staff       (20)       12 2023-07-31 08:16:24.000000 prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/top_level.txt
+-rw-r--r--   0 prism      (501) staff       (20)      137 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/pyproject.toml
+-rw-r--r--   0 prism      (501) staff       (20)       38 2023-07-31 08:16:24.818396 prismstudio-dev-1.1.7rc0/setup.cfg
+-rw-r--r--   0 prism      (501) staff       (20)     1316 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/setup.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.814625 prismstudio-dev-1.1.7rc0/tests/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/tests/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)       94 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/conftest.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.814977 prismstudio-dev-1.1.7rc0/tests/test__validate_args/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     2200 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_common_functions.py
+-rw-r--r--   0 prism      (501) staff       (20)     1539 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_fillna.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.816864 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)     5990 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_01_frequency.py
+-rw-r--r--   0 prism      (501) staff       (20)     2004 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_02_datetype.py
+-rw-r--r--   0 prism      (501) staff       (20)     2719 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_03_periodtype.py
+-rw-r--r--   0 prism      (501) staff       (20)     1615 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_04_adjustment.py
+-rw-r--r--   0 prism      (501) staff       (20)     2304 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_05_shownid.py
+-rw-r--r--   0 prism      (501) staff       (20)     1946 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_06_rank_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     2302 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_07_method.py
+-rw-r--r--   0 prism      (501) staff       (20)     6448 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py
+-rw-r--r--   0 prism      (501) staff       (20)     3854 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_09_contains_universename.py
+-rw-r--r--   0 prism      (501) staff       (20)     1717 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py
+-rw-r--r--   0 prism      (501) staff       (20)     1118 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_11_base.py
+-rw-r--r--   0 prism      (501) staff       (20)     1792 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_12_preliminary.py
+-rw-r--r--   0 prism      (501) staff       (20)      889 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_13_setting.py
+-rw-r--r--   0 prism      (501) staff       (20)      956 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_14_settings.py
+-rw-r--r--   0 prism      (501) staff       (20)     2441 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_factors.py
+drwxr-xr-x   0 prism      (501) staff       (20)        0 2023-07-31 08:16:24.817972 prismstudio-dev-1.1.7rc0/tests/test_util/
+-rw-r--r--   0 prism      (501) staff       (20)        0 2023-07-19 13:45:53.000000 prismstudio-dev-1.1.7rc0/tests/test_util/__init__.py
+-rw-r--r--   0 prism      (501) staff       (20)      603 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/db_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     1264 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/dq_model.py
+-rw-r--r--   0 prism      (501) staff       (20)     1753 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/dq_table.py
+-rw-r--r--   0 prism      (501) staff       (20)    15617 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/factor_fixtures.py
+-rw-r--r--   0 prism      (501) staff       (20)     2738 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/update_factor.py
+-rw-r--r--   0 prism      (501) staff       (20)     1259 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_util/utils.py
+-rw-r--r--   0 prism      (501) staff       (20)     1770 2023-07-31 05:53:38.000000 prismstudio-dev-1.1.7rc0/tests/test_version.py
```

### Comparing `prismstudio-dev-1.1.7b0/LICENSE.txt` & `prismstudio-dev-1.1.7rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/__init__.py` & `prismstudio-dev-1.1.7rc0/prism/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_common/config.py` & `prismstudio-dev-1.1.7rc0/prism/_common/config.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_common/const.py` & `prismstudio-dev-1.1.7rc0/prism/_common/const.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/esg.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/esg.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/estimate.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/estimate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/event.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/event.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/financial.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/financial.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/index.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/index.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/industry.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/industry.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/market.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/market.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/precalculated.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/precalculated.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_data/securitymaster.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_data/securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_fn.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_fn.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/__init__.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_auth.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_auth.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dataquery.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_dataquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_dbinfo.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_dbinfo.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_exportdata.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_exportdata.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_gui.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_gui.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_job.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_job.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_list.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_list.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_portfolio.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_portfolio.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_securitymaster.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_securitymaster.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_task.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_task.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_taskquery.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_taskquery.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/_universe.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/_universe.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/_req_builder/preference.py` & `prismstudio-dev-1.1.7rc0/prism/_core/_req_builder/preference.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_core/ols.py` & `prismstudio-dev-1.1.7rc0/prism/_core/ols.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_prismcomponent/abstract_prismcomponent.py` & `prismstudio-dev-1.1.7rc0/prism/_prismcomponent/abstract_prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_prismcomponent/datacomponent.py` & `prismstudio-dev-1.1.7rc0/prism/_prismcomponent/datacomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_prismcomponent/prismcomponent.py` & `prismstudio-dev-1.1.7rc0/prism/_prismcomponent/prismcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_prismcomponent/taskcomponent.py` & `prismstudio-dev-1.1.7rc0/prism/_prismcomponent/taskcomponent.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/auth_utils.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/auth_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/exceptions.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/loader.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/loader.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/prismcomponent_utils.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/prismcomponent_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/req_builder_utils.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/req_builder_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/validate_utils.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/validate_utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/validate_utils_refactored.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/validate_utils_refactored.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prism/_utils/version.py` & `prismstudio-dev-1.1.7rc0/prism/_utils/version.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/prismstudio_dev.egg-info/SOURCES.txt` & `prismstudio-dev-1.1.7rc0/prismstudio_dev.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
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
```

### Comparing `prismstudio-dev-1.1.7b0/setup.py` & `prismstudio-dev-1.1.7rc0/setup.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_common_functions.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_common_functions.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_fillna.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_fillna.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_01_frequency.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_01_frequency.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_02_datetype.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_02_datetype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_03_periodtype.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_03_periodtype.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_04_adjustment.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_04_adjustment.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_05_shownid.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_05_shownid.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_06_rank_method.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_06_rank_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_07_method.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_07_method.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_08_in_startdate_or_enddate.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_09_contains_universename.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_09_contains_universename.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_10_contains_min_periods.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_11_base.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_11_base.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_12_preliminary.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_12_preliminary.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_13_setting.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_13_setting.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test__validate_args/test_params/test_param_14_settings.py` & `prismstudio-dev-1.1.7rc0/tests/test__validate_args/test_params/test_param_14_settings.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_factors.py` & `prismstudio-dev-1.1.7rc0/tests/test_factors.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/db_fixtures.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/db_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/dq_model.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/dq_model.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/dq_table.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/dq_table.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/factor_fixtures.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/factor_fixtures.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/update_factor.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/update_factor.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_util/utils.py` & `prismstudio-dev-1.1.7rc0/tests/test_util/utils.py`

 * *Files identical despite different names*

### Comparing `prismstudio-dev-1.1.7b0/tests/test_version.py` & `prismstudio-dev-1.1.7rc0/tests/test_version.py`

 * *Files identical despite different names*

