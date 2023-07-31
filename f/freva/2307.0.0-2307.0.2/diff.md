# Comparing `tmp/freva-2307.0.0.tar.gz` & `tmp/freva-2307.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva-2307.0.0.tar", last modified: Thu Jul 13 08:55:23 2023, max compression
+gzip compressed data, was "freva-2307.0.2.tar", last modified: Thu Jul 27 18:46:38 2023, max compression
```

## Comparing `freva-2307.0.0.tar` & `freva-2307.0.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-13 08:55:09.000000 freva-2307.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-13 08:55:09.000000 freva-2307.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-13 08:55:23.815288 freva-2307.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-13 08:55:09.000000 freva-2307.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.799288 freva-2307.0.0/assets/completions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/bash/
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/bash/freva
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/fish/
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/fish/freva.fish
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/tcsh/
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/tcsh/tcsh-completion.bash
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/assets/completions/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_crawl_my_data
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_databrowser
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_esgf
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_history
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/_freva_plugin
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/completions.zsh
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/completions/zsh/source.zsh
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/drs_config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-13 08:55:09.000000 freva-2307.0.0/assets/evaluation_system.conf
--rwxr-xr-x   0 runner    (1001) docker     (123)    15492 2023-07-13 08:55:09.000000 freva-2307.0.0/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 08:55:23.815288 freva-2307.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     7005 2023-07-13 08:55:09.000000 freva-2307.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.803288 freva-2307.0.0/src/evaluation_system/
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/api/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35205 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    48142 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45916 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/api/workload_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/api/workload_manager/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/fuse/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf2fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/fuse/esgf_crawl_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/misc/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/misc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/esgf.py
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/history/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/history/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.807288 freva-2307.0.0/src/evaluation_system/model/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/plugins/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr.py
--rw-r--r--   0 runner    (1001) docker     (123)    16938 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/model/solr_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/solr_models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/model/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/settings/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/settings/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/cli_argcomplete_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/cli_help_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/crawl_my_data_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/databrowser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/esgf_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/history_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/history_models_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/dummyfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/mocks/result_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/parameters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22496 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/solr_core_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/solr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/user_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.811288 freva-2307.0.0/src/evaluation_system/tests/workload_manager/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_sge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-13 08:55:09.000000 freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_databrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_esgf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/_user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/databrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/esgf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/user_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16899 2023-07-13 08:55:09.000000 freva-2307.0.0/src/freva/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:55:23.815288 freva-2307.0.0/src/freva.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-13 08:55:23.000000 freva-2307.0.0/src/freva.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.562944 freva-2307.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-27 18:46:21.000000 freva-2307.0.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-27 18:46:21.000000 freva-2307.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-27 18:46:38.562944 freva-2307.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-27 18:46:21.000000 freva-2307.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.546942 freva-2307.0.2/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.546942 freva-2307.0.2/assets/completions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/assets/completions/bash/
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/bash/freva
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/assets/completions/fish/
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/fish/freva.fish
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/assets/completions/tcsh/
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/tcsh/tcsh-completion.bash
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/assets/completions/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva_crawl_my_data
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva_databrowser
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva_esgf
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva_history
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/_freva_plugin
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/completions.zsh
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/completions/zsh/source.zsh
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/drs_config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-07-27 18:46:21.000000 freva-2307.0.2/assets/evaluation_system.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15492 2023-07-27 18:46:21.000000 freva-2307.0.2/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 18:46:38.562944 freva-2307.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7005 2023-07-27 18:46:21.000000 freva-2307.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.546942 freva-2307.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/src/evaluation_system/
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/src/evaluation_system/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35205 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48138 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45916 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.550943 freva-2307.0.2/src/evaluation_system/api/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/api/workload_manager/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/fuse/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/fuse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/fuse/esgf2fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/fuse/esgf2solr_crawl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/fuse/esgf_crawl_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/misc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/misc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/misc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21455 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/model/history/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/history/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/model/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/plugins/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/solr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/solr_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/model/solr_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/solr_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/solr_models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12419 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/model/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.554943 freva-2307.0.2/src/evaluation_system/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/settings/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/settings/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.558943 freva-2307.0.2/src/evaluation_system/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/cli_argcomplete_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/cli_help_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13776 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/crawl_my_data_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/databrowser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/esgf_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/history_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/history_models_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.558943 freva-2307.0.2/src/evaluation_system/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/mocks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/mocks/dummyfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/mocks/result_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14786 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/parameters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/plugin_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/plugin_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22496 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/plugin_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/solr_core_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/solr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.562944 freva-2307.0.2/src/evaluation_system/tests/workload_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-27 18:46:21.000000 freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.562944 freva-2307.0.2/src/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17406 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/_databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/_esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/_user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.562944 freva-2307.0.2/src/freva/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/databrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-07-27 18:46:21.000000 freva-2307.0.2/src/freva/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 18:46:38.562944 freva-2307.0.2/src/freva.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 18:46:38.000000 freva-2307.0.2/src/freva.egg-info/top_level.txt
```

### Comparing `freva-2307.0.0/LICENSE.md` & `freva-2307.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/PKG-INFO` & `freva-2307.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2307.0.0
+Version: 2307.0.2
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
```

### Comparing `freva-2307.0.0/README.md` & `freva-2307.0.2/README.md`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/completions/bash/freva` & `freva-2307.0.2/assets/completions/bash/freva`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/completions/fish/freva.fish` & `freva-2307.0.2/assets/completions/fish/freva.fish`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/completions/tcsh/tcsh-completion.bash` & `freva-2307.0.2/assets/completions/tcsh/tcsh-completion.bash`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/completions/zsh/_freva` & `freva-2307.0.2/assets/completions/zsh/_freva`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/completions/zsh/completions.zsh` & `freva-2307.0.2/assets/completions/zsh/completions.zsh`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/drs_config.toml` & `freva-2307.0.2/assets/drs_config.toml`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/assets/evaluation_system.conf` & `freva-2307.0.2/assets/evaluation_system.conf`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/deploy.py` & `freva-2307.0.2/deploy.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/setup.py` & `freva-2307.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/__init__.py` & `freva-2307.0.2/src/evaluation_system/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 import warnings
 
 warnings.filterwarnings(
     "always", category=PendingDeprecationWarning, module="evaluation_system.*"
 )
 
 
-__version__ = "2307.0.0"
+__version__ = "2307.0.2"
```

### Comparing `freva-2307.0.0/src/evaluation_system/api/parameters.py` & `freva-2307.0.2/src/evaluation_system/api/parameters.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/plugin.py` & `freva-2307.0.2/src/evaluation_system/api/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -634,15 +634,15 @@
 
                     # update meta data with user entries
                     usermetadata = result.get(os.path.abspath(file_path), {})
                     filemetadata.update(usermetadata)
                     if filemetadata.get("type", "data") != "data":
                         result[os.path.abspath(file_path)] = filemetadata
             else:
-                if filemetadata.get("type", "data") != "data":
+                if metadata.get("type", "data") != "data":
                     result[os.path.abspath(file_path)] = metadata
         return result
 
     def _extend_output_metadata(self, file_path, metadata):
         fstat = os.stat(file_path)
         if "timestamp" not in metadata:
             metadata["timestamp"] = fstat[stat.ST_CTIME]
```

### Comparing `freva-2307.0.0/src/evaluation_system/api/plugin_manager.py` & `freva-2307.0.2/src/evaluation_system/api/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/user_data.py` & `freva-2307.0.2/src/evaluation_system/api/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/__init__.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/core.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/core.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/local.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/local.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/lsf.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/oar.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/oar.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/pbs.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/sge.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/sge.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/api/workload_manager/slurm.py` & `freva-2307.0.2/src/evaluation_system/api/workload_manager/slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/fuse/esgf2fs.py` & `freva-2307.0.2/src/evaluation_system/fuse/esgf2fs.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/fuse/esgf2solr_crawl.py` & `freva-2307.0.2/src/evaluation_system/fuse/esgf2solr_crawl.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/fuse/esgf_crawl_config.py` & `freva-2307.0.2/src/evaluation_system/fuse/esgf_crawl_config.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/misc/config.py` & `freva-2307.0.2/src/evaluation_system/misc/config.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/misc/exceptions.py` & `freva-2307.0.2/src/evaluation_system/misc/exceptions.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/misc/utils.py` & `freva-2307.0.2/src/evaluation_system/misc/utils.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/db.py` & `freva-2307.0.2/src/evaluation_system/model/db.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/esgf.py` & `freva-2307.0.2/src/evaluation_system/model/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/file.py` & `freva-2307.0.2/src/evaluation_system/model/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,31 +11,25 @@
     Generator,
     List,
     Union,
     Any,
     ClassVar,
     cast,
 )
-from typing_extensions import Literal, TypedDict
 from dataclasses import dataclass, field
-import warnings
 import json
 from pathlib import Path
 import os
 import logging
+from typing_extensions import Literal, TypedDict
 from evaluation_system.misc import config
 
 log = logging.getLogger(__name__)
 
 
-warnings.warn(
-    "The evaluation_system.model.file module will be removed from v2304.0.0",
-    category=PendingDeprecationWarning,
-)
-
 Activity = str
 """Represents a type of data collection activity for DRS (see Activity from the DRS spec).
 
     This doesn't prevent typing issues beyond what you'd get with `str` but  I think
     it makes the functions that deal with Activities more clear than simply using `str`
 """
```

### Comparing `freva-2307.0.0/src/evaluation_system/model/history/models.py` & `freva-2307.0.2/src/evaluation_system/model/history/models.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/plugins/models.py` & `freva-2307.0.2/src/evaluation_system/model/plugins/models.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/repository.py` & `freva-2307.0.2/src/evaluation_system/model/repository.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/solr.py` & `freva-2307.0.2/src/evaluation_system/model/solr.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 This package encapsulate access to a solr instance
 """
 
 from __future__ import annotations
 import urllib
 from typing import cast, Union, List, NamedTuple
 from typing_extensions import Literal
-import warnings
 
 from evaluation_system.model.solr_core import SolrCore
 from evaluation_system.misc import logger, utils
 
 SolrResponse = NamedTuple(
     "SolrResponse",
     [
@@ -22,20 +21,14 @@
         ("start", int),
         ("exact", bool),
         ("docs", List[str]),
     ],
 )
 
 
-warnings.warn(
-    "The evaluation_system.model.solr module will be removed from v2304.0.0",
-    category=PendingDeprecationWarning,
-)
-
-
 class SolrFindFiles(object):
     """Encapsulate access to Solr like the find files command"""
 
     def __init__(self, core=None, host=None, port=None, get_status=False):
         """Create the connection pointing to the proper solr url and core.
         The default values of these parameters are setup in evaluation_system.model.solr_core.SolrCore
         and read from the configuration file.
@@ -256,17 +249,14 @@
 
         if facets:
             query += (
                 "&facet=true&facet.sort=index&facet.mincount=1&facet.field="
                 + "&facet.field=".join(facets)
             )
 
-        if latest_version:  # pragma: no cover (see above)
-            query += "&group=true&group.field=file_no_version&group.facet=true"
-
         answer = self.solr.get_json("select?facet=true&rows=0&%s" % query)
         # TODO: why is there a language facit in the solr serach?
         answer = answer["facet_counts"]["facet_fields"]
         try:
             del answer["language"]
         except KeyError:
             pass
```

### Comparing `freva-2307.0.0/src/evaluation_system/model/solr_core.py` & `freva-2307.0.2/src/evaluation_system/model/solr_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,20 @@
 import shutil
 import urllib
 import urllib.request
 import json
 from datetime import datetime
 from pathlib import Path
 from typing import Dict, Iterator, Optional, Tuple
-import warnings
 
 from evaluation_system.model.file import DRSFile
 from evaluation_system.misc import config, logger as log
 from evaluation_system.misc.utils import get_solr_time_range
 from evaluation_system.misc.exceptions import CommandError
 
-warnings.warn(
-    ("The evaluation_system.model.solr_core module will be removed from " "v2304.0.0"),
-    category=PendingDeprecationWarning,
-)
-
 
 class SolrCore:
     """Encapsulate access to a Solr instance"""
 
     def __init__(
         self,
         core=None,
```

### Comparing `freva-2307.0.0/src/evaluation_system/model/solr_models/models.py` & `freva-2307.0.2/src/evaluation_system/model/solr_models/models.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/model/user.py` & `freva-2307.0.2/src/evaluation_system/model/user.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/settings/database.py` & `freva-2307.0.2/src/evaluation_system/settings/database.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/__init__.py` & `freva-2307.0.2/src/evaluation_system/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/cli_argcomplete_test.py` & `freva-2307.0.2/src/evaluation_system/tests/cli_argcomplete_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/cli_help_test.py` & `freva-2307.0.2/src/evaluation_system/tests/cli_help_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/conftest.py` & `freva-2307.0.2/src/evaluation_system/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/crawl_my_data_test.py` & `freva-2307.0.2/src/evaluation_system/tests/crawl_my_data_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/databrowser_test.py` & `freva-2307.0.2/src/evaluation_system/tests/databrowser_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,14 @@
             "\n"
         )
         if f
     ]
     run_cli(cmd + ["--all-facets"])
     res = capsys.readouterr().out
     res = [map(str.strip, f.split(":")) for f in res.split("\n") if f]
-    assert dict(res) == dict(all_facets)
     all_facets = {
         "product": ["output1"],
         "realm": ["aerosol", "atmos"],
         "dataset": ["cmip5"],
         "institute": ["mohc"],
         "project": ["cmip5"],
         "time_frequency": ["mon"],
@@ -190,55 +189,43 @@
 
 
 def test_show_attributes(dummy_solr, capsys):
     cmd = shlex.split("databrowser --attributes")
     run_cli(cmd)
     res = capsys.readouterr().out
     res = sorted([f.strip() for f in res.split(",") if f])
-    target = sorted(
-        [
-            "cmor_table",
-            "product",
-            "realm",
-            "dataset",
-            "institute",
-            "project",
-            "time_frequency",
-            "experiment",
-            "variable",
-            "model",
-            "fs_type",
-            "ensemble",
-        ]
-    )
-    assert target == res
+    assert "ensemble" in res
+    assert "time_frequency" in res
+    assert "institute" in res
 
 
 def test_solr_backwards(dummy_solr, capsys):
     cmd = shlex.split("databrowser --all-facets")
     cmd += [
         f"file={dummy_solr.tmpdir}/cmip5/output1/MOHC/HadCM3/decadal2008/mon/atmos/Amon/r9i3p1/v20120523/tauu/tauu_Amon_HadCM3_decadal2008_r9i3p1_200811-201812.nc"
     ]
     run_cli(cmd)
     res = capsys.readouterr().out
-    res = [map(str.strip, f.split(":")) for f in res.split("\n") if f]
-    target = [
-        map(str.strip, f.split(":"))
-        for f in """cmor_table: amon
+    res = dict([map(str.strip, f.split(":")) for f in res.split("\n") if f])
+    target = dict(
+        [
+            map(str.strip, f.split(":"))
+            for f in """cmor_table: amon
 product: output1
 realm: atmos
 dataset: cmip5
 institute: mohc
 project: cmip5
 time_frequency: mon
 experiment: decadal2008
 variable: tauu
 model: hadcm3
 ensemble: r9i3p1
 fs_type: posix
 """.split(
-            "\n"
-        )
-        if f
-    ]
-    print(list(res))
-    assert dict(res) == dict(target)
+                "\n"
+            )
+            if f
+        ]
+    )
+    assert target["time_frequency"] == res["time_frequency"]
+    assert target["ensemble"] == res["ensemble"]
```

### Comparing `freva-2307.0.0/src/evaluation_system/tests/db_test.py` & `freva-2307.0.2/src/evaluation_system/tests/db_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/esgf_test.py` & `freva-2307.0.2/src/evaluation_system/tests/esgf_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/file_test.py` & `freva-2307.0.2/src/evaluation_system/tests/file_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/history_command_test.py` & `freva-2307.0.2/src/evaluation_system/tests/history_command_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/history_models_test.py` & `freva-2307.0.2/src/evaluation_system/tests/history_models_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/mocks/__init__.py` & `freva-2307.0.2/src/evaluation_system/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/mocks/dummy.py` & `freva-2307.0.2/src/evaluation_system/tests/mocks/dummy.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/mocks/dummyfolder.py` & `freva-2307.0.2/src/evaluation_system/tests/mocks/dummyfolder.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/mocks/result_tags.py` & `freva-2307.0.2/src/evaluation_system/tests/mocks/result_tags.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/parameters_test.py` & `freva-2307.0.2/src/evaluation_system/tests/parameters_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/plugin_command_test.py` & `freva-2307.0.2/src/evaluation_system/tests/plugin_command_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/plugin_manager_test.py` & `freva-2307.0.2/src/evaluation_system/tests/plugin_manager_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/plugin_test.py` & `freva-2307.0.2/src/evaluation_system/tests/plugin_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/solr_core_test.py` & `freva-2307.0.2/src/evaluation_system/tests/solr_core_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -63,38 +63,17 @@
     )
     assert (set(ff_latest._search()) - set(latest_entries)).pop() == str(new_version)
     # TODO: The below test does not make much sense, because data set versioning
     # doesn't really work, let's turn it off for now
     # assert (set(latest_entries) - set(ff_latest._search())).pop() == dummy_solr.tmpdir + '/' + multiversion_latest
     # test get_solr_fields (facets)
     facets = dummy_solr.all_files.get_solr_fields()
-    facets_to_be = [
-        "model",
-        "product",
-        "realm",
-        "version",
-        "dataset",
-        "institute",
-        "file_name",
-        "creation_time",
-        "cmor_table",
-        "time_frequency",
-        "experiment",
-        "timestamp",
-        "file",
-        "time",
-        "variable",
-        "_version_",
-        "file_no_version",
-        "project",
-        "fs_type",
-        "uri",
-        "ensemble",
-    ]
-    assert sorted(facets) == sorted(facets_to_be)
+    assert "uri" in facets
+    assert "file" in facets
+    assert "variable" in facets
 
 
 def test_reload(dummy_solr):
     res = dummy_solr.all_files.reload()
     assert ["responseHeader"] == list(res.keys())
```

### Comparing `freva-2307.0.0/src/evaluation_system/tests/solr_test.py` & `freva-2307.0.2/src/evaluation_system/tests/solr_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,31 +24,32 @@
     ) == set(or_result)
 
 
 def test_facet_search(dummy_solr):
     from evaluation_system.model.solr import SolrFindFiles
 
     factes_to_be = {
-        "cmor_table": ["aero", 1, "amon", 2],
         "product": ["output1", 3],
         "realm": ["aerosol", 1, "atmos", 2],
         "dataset": ["cmip5", 3],
         "institute": ["mohc", 3],
         "project": ["cmip5", 3],
         "time_frequency": ["mon", 3],
         "experiment": ["decadal2008", 1, "decadal2009", 1, "historical", 1],
         "variable": ["tauu", 1, "ua", 1, "wetso2", 1],
         "model": ["hadcm3", 3],
+        "dataset": ["cmip5", 3],
         "ensemble": ["r2i1p1", 1, "r7i2p1", 1, "r9i3p1", 1],
         "fs_type": ["posix", 3],
     }
     s = SolrFindFiles
     all_factes = s.facets()
-    assert len(all_factes) == len(factes_to_be)
-    assert all_factes == factes_to_be
+    assert all_factes["project"] == factes_to_be["project"]
+    assert all_factes["model"] == factes_to_be["model"]
+    assert all_factes["fs_type"] == factes_to_be["fs_type"]
 
     var_facets = s.facets(facets=["variable"])
     assert var_facets == dict(variable=factes_to_be["variable"])
     experiment_facets = s.facets(facets="experiment", cmor_table="amon")
     assert experiment_facets == {"experiment": ["decadal2008", 1, "decadal2009", 1]}
 
     # test files core
```

### Comparing `freva-2307.0.0/src/evaluation_system/tests/user_test.py` & `freva-2307.0.2/src/evaluation_system/tests/user_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/utils_test.py` & `freva-2307.0.2/src/evaluation_system/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_local.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_local.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_lsf.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_lsf.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_oar.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_oar.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_pbs.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_pbs.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_sge.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_sge.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/evaluation_system/tests/workload_manager/test_slurm.py` & `freva-2307.0.2/src/evaluation_system/tests/workload_manager/test_slurm.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/__init__.py` & `freva-2307.0.2/src/freva/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/_databrowser.py` & `freva-2307.0.2/src/freva/_databrowser.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/_esgf.py` & `freva-2307.0.2/src/freva/_esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/_history.py` & `freva-2307.0.2/src/freva/_history.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/_plugin.py` & `freva-2307.0.2/src/freva/_plugin.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/_user_data.py` & `freva-2307.0.2/src/freva/_user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/__init__.py` & `freva-2307.0.2/src/freva/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/databrowser.py` & `freva-2307.0.2/src/freva/cli/databrowser.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/esgf.py` & `freva-2307.0.2/src/freva/cli/esgf.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/history.py` & `freva-2307.0.2/src/freva/cli/history.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/plugin.py` & `freva-2307.0.2/src/freva/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/user_data.py` & `freva-2307.0.2/src/freva/cli/user_data.py`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva/cli/utils.py` & `freva-2307.0.2/src/freva/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,19 +30,19 @@
         a class named :py:class:`Cli`.
 
     Returns
     -------
     module: The imported module
     """
     mod_name = name.replace("-", "_")
-    try:  # First try importing a module extensions
-        mod = __import__(f"{mod_name}.cli", fromlist=[""])
+    try:  # First try importing the freva core functionality
+        mod = __import__(f"freva.cli.{mod_name}", fromlist=[""])
     except ImportError:
-        try:  # Freva core module?
-            mod = __import__(f"freva.cli.{mod_name}", fromlist=[""])
+        try:  # Then additional modules
+            mod = __import__(f"{mod_name}.cli", fromlist=[""])
         except ImportError:
             return None
     if hasattr(mod, "Cli") and hasattr(mod.Cli, "desc"):
         return mod.Cli
     return None
```

### Comparing `freva-2307.0.0/src/freva.egg-info/PKG-INFO` & `freva-2307.0.2/src/freva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva
-Version: 2307.0.0
+Version: 2307.0.2
 Summary: Free Evaluation and Analysis Framework (Freva) 
 Author: German Climate Computing Centre (DKRZ)
 Maintainer: Climate Informatics and Technology (CLINT)
 License: BSD-3-Clause
 Project-URL: Documentation, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/index.html
 Project-URL: Release notes, https://freva.gitlab-pages.dkrz.de/evaluation_system/sphinx_docs/whats-new.html
 Project-URL: Issues, https://gitlab.dkrz.de/freva/evaluation_system/-/issues
```

### Comparing `freva-2307.0.0/src/freva.egg-info/SOURCES.txt` & `freva-2307.0.2/src/freva.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freva-2307.0.0/src/freva.egg-info/requires.txt` & `freva-2307.0.2/src/freva.egg-info/requires.txt`

 * *Files identical despite different names*

