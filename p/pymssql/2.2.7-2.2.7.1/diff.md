# Comparing `tmp/pymssql-2.2.7.tar.gz` & `tmp/pymssql-2.2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymssql-2.2.7.tar", last modified: Wed Nov 16 05:00:11 2022, max compression
+gzip compressed data, was "pymssql-2.2.7.1.tar", last modified: Sun Jul 30 22:27:09 2023, max compression
```

## Comparing `pymssql-2.2.7.tar` & `pymssql-2.2.7.1.tar`

### file list

```diff
@@ -1,112 +1,113 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:11.004713 pymssql-2.2.7/
--rw-r--r--   0 root         (0) root         (0)       40 2022-11-16 04:56:48.000000 pymssql-2.2.7/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.988713 pymssql-2.2.7/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.988713 pymssql-2.2.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      724 2022-11-16 04:56:48.000000 pymssql-2.2.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      238 2022-11-16 04:56:48.000000 pymssql-2.2.7/.github/dependabot.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.988713 pymssql-2.2.7/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     3185 2022-11-16 04:56:48.000000 pymssql-2.2.7/.github/workflows/test_linux.yml
--rw-r--r--   0 root         (0) root         (0)     2507 2022-11-16 04:56:48.000000 pymssql-2.2.7/.github/workflows/test_macos.yml
--rw-r--r--   0 root         (0) root         (0)     2317 2022-11-16 04:56:48.000000 pymssql-2.2.7/.github/workflows/test_windows.yml
--rw-r--r--   0 root         (0) root         (0)      224 2022-11-16 04:56:48.000000 pymssql-2.2.7/.gitignore
--rw-r--r--   0 root         (0) root         (0)      223 2022-11-16 04:56:48.000000 pymssql-2.2.7/.pypirc
--rw-r--r--   0 root         (0) root         (0)      505 2022-11-16 04:56:48.000000 pymssql-2.2.7/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)    38518 2022-11-16 04:56:48.000000 pymssql-2.2.7/ChangeLog.old
--rw-r--r--   0 root         (0) root         (0)    17337 2022-11-16 04:56:48.000000 pymssql-2.2.7/ChangeLog.rst
--rw-r--r--   0 root         (0) root         (0)      964 2022-11-16 04:56:48.000000 pymssql-2.2.7/Dockerfile
--rw-r--r--   0 root         (0) root         (0)    26436 2022-11-16 04:56:48.000000 pymssql-2.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2022-11-16 04:56:48.000000 pymssql-2.2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4542 2022-11-16 05:00:11.004713 pymssql-2.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2448 2022-11-16 04:56:48.000000 pymssql-2.2.7/README.rst
--rw-r--r--   0 root         (0) root         (0)     8473 2022-11-16 04:56:48.000000 pymssql-2.2.7/appveyor.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.992713 pymssql-2.2.7/dev/
--rw-r--r--   0 root         (0) root         (0)       55 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.992713 pymssql-2.2.7/dev/appveyor/
--rw-r--r--   0 root         (0) root         (0)     2270 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/install-win-iconv.ps1
--rw-r--r--   0 root         (0) root         (0)     7195 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/install.ps1
--rw-r--r--   0 root         (0) root         (0)      223 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/pypirc
--rw-r--r--   0 root         (0) root         (0)     4130 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/run_with_env.cmd
--rw-r--r--   0 root         (0) root         (0)     1362 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1
--rw-r--r--   0 root         (0) root         (0)      658 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/appveyor/tests.cfg
--rw-r--r--   0 root         (0) root         (0)     8222 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/build.py
--rwxr-xr-x   0 root         (0) root         (0)     1128 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/build_freetds.sh
--rwxr-xr-x   0 root         (0) root         (0)     3393 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/build_manylinux_wheels.sh
--rw-r--r--   0 root         (0) root         (0)     2533 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/ccompiler.py
--rw-r--r--   0 root         (0) root         (0)       53 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/dev-requirements.pip
--rwxr-xr-x   0 root         (0) root         (0)     2033 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/hudson.sh
--rwxr-xr-x   0 root         (0) root         (0)      920 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/memmonitor.py
--rwxr-xr-x   0 root         (0) root         (0)      464 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/memtest.py
--rwxr-xr-x   0 root         (0) root         (0)       73 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/memtest.sh
--rw-r--r--   0 root         (0) root         (0)      155 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/requirements-dev.txt
--rwxr-xr-x   0 root         (0) root         (0)     1305 2022-11-16 04:56:48.000000 pymssql-2.2.7/dev/test_manylinux_wheels.sh
--rw-r--r--   0 root         (0) root         (0)      811 2022-11-16 04:56:48.000000 pymssql-2.2.7/docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.996713 pymssql-2.2.7/docs/
--rw-r--r--   0 root         (0) root         (0)     6766 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     4952 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/_mssql_examples.rst
--rw-r--r--   0 root         (0) root         (0)     1010 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/azure.rst
--rw-r--r--   0 root         (0) root         (0)     6130 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/building_and_developing.rst
--rw-r--r--   0 root         (0) root         (0)      160 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     9287 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)     1726 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/docker.rst
--rw-r--r--   0 root         (0) root         (0)    10196 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/faq.rst
--rw-r--r--   0 root         (0) root         (0)     6000 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/freetds.rst
--rw-r--r--   0 root         (0) root         (0)     2213 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/freetds_and_dates.rst
--rw-r--r--   0 root         (0) root         (0)     1738 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.996713 pymssql-2.2.7/docs/images/
--rw-r--r--   0 root         (0) root         (0)    15267 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/images/pymssql-stack.graphml
--rw-r--r--   0 root         (0) root         (0)    25535 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/images/pymssql-stack.png
--rw-r--r--   0 root         (0) root         (0)     2133 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     4106 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/intro.rst
--rw-r--r--   0 root         (0) root         (0)     6703 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)     5513 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/migrate_1_x_to_2_x.rst
--rw-r--r--   0 root         (0) root         (0)     8452 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/pymssql_examples.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.996713 pymssql-2.2.7/docs/ref/
--rw-r--r--   0 root         (0) root         (0)    17465 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/ref/_mssql.rst
--rw-r--r--   0 root         (0) root         (0)    17748 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/ref/pymssql.rst
--rw-r--r--   0 root         (0) root         (0)     3943 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/release_notes.rst
--rw-r--r--   0 root         (0) root         (0)       93 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-11-16 04:56:48.000000 pymssql-2.2.7/docs/todo.rst
--rw-r--r--   0 root         (0) root         (0)      292 2022-11-16 04:56:48.000000 pymssql-2.2.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      447 2022-11-16 04:56:48.000000 pymssql-2.2.7/pytest.ini
--rw-r--r--   0 root         (0) root         (0)      149 2022-11-16 05:00:11.008713 pymssql-2.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    11908 2022-11-16 04:56:48.000000 pymssql-2.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:10.984713 pymssql-2.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:11.000713 pymssql-2.2.7/src/pymssql/
--rw-r--r--   0 root         (0) root         (0)      101 2022-11-16 04:56:48.000000 pymssql-2.2.7/src/pymssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2082 2022-11-16 04:56:48.000000 pymssql-2.2.7/src/pymssql/_mssql.pxd
--rw-r--r--   0 root         (0) root         (0)    74966 2022-11-16 04:56:48.000000 pymssql-2.2.7/src/pymssql/_mssql.pyx
--rw-r--r--   0 root         (0) root         (0)    23234 2022-11-16 04:56:48.000000 pymssql-2.2.7/src/pymssql/_pymssql.pyx
--rw-r--r--   0 root         (0) root         (0)    25047 2022-11-16 04:56:48.000000 pymssql-2.2.7/src/pymssql/sqlfront.pxd
--rw-r--r--   0 root         (0) root         (0)       31 2022-11-16 05:00:10.000000 pymssql-2.2.7/src/pymssql/version.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:11.000713 pymssql-2.2.7/src/pymssql.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4542 2022-11-16 05:00:10.000000 pymssql-2.2.7/src/pymssql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2146 2022-11-16 05:00:10.000000 pymssql-2.2.7/src/pymssql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 05:00:10.000000 pymssql-2.2.7/src/pymssql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-16 04:58:20.000000 pymssql-2.2.7/src/pymssql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2022-11-16 05:00:10.000000 pymssql-2.2.7/src/pymssql.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-16 05:00:11.004713 pymssql-2.2.7/tests/
--rw-r--r--   0 root         (0) root         (0)       32 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3707 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)    14638 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/helpers.py
--rwxr-xr-x   0 root         (0) root         (0)     1913 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/run_sqlalchemy_tests.py
--rw-r--r--   0 root         (0) root         (0)     5367 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_bulk_copy.py
--rw-r--r--   0 root         (0) root         (0)     3936 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1294 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_connection_as_dict.py
--rw-r--r--   0 root         (0) root         (0)      631 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_connection_timeout.py
--rw-r--r--   0 root         (0) root         (0)     5939 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_connections.py
--rw-r--r--   0 root         (0) root         (0)     1340 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_context_managers.py
--rw-r--r--   0 root         (0) root         (0)     1052 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_debug_queries.py
--rw-r--r--   0 root         (0) root         (0)     2481 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_err_handle.py
--rw-r--r--   0 root         (0) root         (0)     4469 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_green.py
--rw-r--r--   0 root         (0) root         (0)     1059 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_memory.py
--rw-r--r--   0 root         (0) root         (0)     7321 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_pymssql.py
--rw-r--r--   0 root         (0) root         (0)     3772 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_queries.py
--rw-r--r--   0 root         (0) root         (0)    19782 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_sprocs.py
--rw-r--r--   0 root         (0) root         (0)     1924 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_sqlalchemy.py
--rw-r--r--   0 root         (0) root         (0)     3260 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_threaded.py
--rw-r--r--   0 root         (0) root         (0)    12173 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_types.py
--rw-r--r--   0 root         (0) root         (0)      756 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_unicode.py
--rw-r--r--   0 root         (0) root         (0)     5215 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_user_msghandler.py
--rw-r--r--   0 root         (0) root         (0)     6119 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)      679 2022-11-16 04:56:48.000000 pymssql-2.2.7/tests/tests.cfg.tpl
--rw-r--r--   0 root         (0) root         (0)      617 2022-11-16 04:56:48.000000 pymssql-2.2.7/tox.ini
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.086188 pymssql-2.2.7.1/
+-rw-r--r--   0 termim    (1000) sambashare   (430)       40 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/.dockerignore
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.059188 pymssql-2.2.7.1/.github/
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.059188 pymssql-2.2.7.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 termim    (1000) sambashare   (430)      724 2022-10-10 21:37:05.000000 pymssql-2.2.7.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 termim    (1000) sambashare   (430)      238 2022-11-13 19:35:39.000000 pymssql-2.2.7.1/.github/dependabot.yml
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.060188 pymssql-2.2.7.1/.github/workflows/
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3185 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/.github/workflows/test_linux.yml
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2507 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/.github/workflows/test_macos.yml
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2317 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/.github/workflows/test_windows.yml
+-rw-r--r--   0 termim    (1000) sambashare   (430)      224 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/.gitignore
+-rw-r--r--   0 termim    (1000) sambashare   (430)      223 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/.pypirc
+-rw-r--r--   0 termim    (1000) sambashare   (430)      505 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/.readthedocs.yaml
+-rw-r--r--   0 termim    (1000) sambashare   (430)    38518 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/ChangeLog.old
+-rw-r--r--   0 termim    (1000) sambashare   (430)    17337 2023-02-19 23:28:40.000000 pymssql-2.2.7.1/ChangeLog.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)      964 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/Dockerfile
+-rw-r--r--   0 termim    (1000) sambashare   (430)    26436 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/LICENSE
+-rw-r--r--   0 termim    (1000) sambashare   (430)       52 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/MANIFEST.in
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4544 2023-07-30 22:27:09.086188 pymssql-2.2.7.1/PKG-INFO
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2448 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/README.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     8473 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/appveyor.yml
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.065188 pymssql-2.2.7.1/dev/
+-rw-r--r--   0 termim    (1000) sambashare   (430)       55 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/__init__.py
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.066188 pymssql-2.2.7.1/dev/appveyor/
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2270 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/install-win-iconv.ps1
+-rw-r--r--   0 termim    (1000) sambashare   (430)     7195 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/install.ps1
+-rw-r--r--   0 termim    (1000) sambashare   (430)      223 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/pypirc
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4130 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/run_with_env.cmd
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1362 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1
+-rw-r--r--   0 termim    (1000) sambashare   (430)      658 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/appveyor/tests.cfg
+-rw-r--r--   0 termim    (1000) sambashare   (430)     8222 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/dev/build.py
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)     1128 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/build_freetds.sh
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)     3393 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/dev/build_manylinux_wheels.sh
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2533 2023-02-19 23:28:19.000000 pymssql-2.2.7.1/dev/ccompiler.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)       53 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/dev-requirements.pip
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)     2033 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/hudson.sh
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)      920 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/memmonitor.py
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)      464 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/memtest.py
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)       73 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/memtest.sh
+-rw-r--r--   0 termim    (1000) sambashare   (430)      155 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/dev/requirements-dev.txt
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)     1305 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/dev/test_manylinux_wheels.sh
+-rw-r--r--   0 termim    (1000) sambashare   (430)      811 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docker-compose.yml
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.072188 pymssql-2.2.7.1/docs/
+-rw-r--r--   0 termim    (1000) sambashare   (430)     6766 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/Makefile
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4952 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docs/_mssql_examples.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1010 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docs/azure.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     6130 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/docs/building_and_developing.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)      160 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docs/changelog.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     9287 2023-02-25 19:07:29.000000 pymssql-2.2.7.1/docs/conf.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1726 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/docs/docker.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)    10196 2022-11-06 14:42:24.000000 pymssql-2.2.7.1/docs/faq.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     6000 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docs/freetds.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2213 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/freetds_and_dates.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1738 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/history.rst
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.073188 pymssql-2.2.7.1/docs/images/
+-rw-r--r--   0 termim    (1000) sambashare   (430)    15267 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/images/pymssql-stack.graphml
+-rw-r--r--   0 termim    (1000) sambashare   (430)    25535 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/images/pymssql-stack.png
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2133 2023-02-25 19:07:29.000000 pymssql-2.2.7.1/docs/index.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4106 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/docs/intro.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     6703 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/make.bat
+-rw-r--r--   0 termim    (1000) sambashare   (430)     5513 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/migrate_1_x_to_2_x.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     8452 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/docs/pymssql_examples.rst
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.074188 pymssql-2.2.7.1/docs/ref/
+-rw-r--r--   0 termim    (1000) sambashare   (430)    17390 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/docs/ref/_mssql.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)    17748 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/docs/ref/pymssql.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3943 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/release_notes.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)       93 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/docs/requirements.txt
+-rw-r--r--   0 termim    (1000) sambashare   (430)       59 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/docs/todo.rst
+-rw-r--r--   0 termim    (1000) sambashare   (430)      292 2023-07-30 22:22:24.000000 pymssql-2.2.7.1/pyproject.toml
+-rw-r--r--   0 termim    (1000) sambashare   (430)      447 2020-09-17 21:08:01.000000 pymssql-2.2.7.1/pytest.ini
+-rw-r--r--   0 termim    (1000) sambashare   (430)      149 2023-07-30 22:27:09.087188 pymssql-2.2.7.1/setup.cfg
+-rw-r--r--   0 termim    (1000) sambashare   (430)    11908 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/setup.py
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.052188 pymssql-2.2.7.1/src/
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.075188 pymssql-2.2.7.1/src/pymssql/
+-rw-r--r--   0 termim    (1000) sambashare   (430)      101 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/src/pymssql/__init__.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2082 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/src/pymssql/_mssql.pxd
+-rw-r--r--   0 termim    (1000) sambashare   (430)    74984 2023-07-30 22:22:24.000000 pymssql-2.2.7.1/src/pymssql/_mssql.pyx
+-rw-r--r--   0 termim    (1000) sambashare   (430)    23234 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/src/pymssql/_pymssql.pyx
+-rw-r--r--   0 termim    (1000) sambashare   (430)    25047 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/src/pymssql/sqlfront.pxd
+-rw-r--r--   0 termim    (1000) sambashare   (430)       33 2023-07-30 22:27:08.000000 pymssql-2.2.7.1/src/pymssql/version.h
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.077188 pymssql-2.2.7.1/src/pymssql.egg-info/
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4544 2023-07-30 22:27:08.000000 pymssql-2.2.7.1/src/pymssql.egg-info/PKG-INFO
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2177 2023-07-30 22:27:08.000000 pymssql-2.2.7.1/src/pymssql.egg-info/SOURCES.txt
+-rw-r--r--   0 termim    (1000) sambashare   (430)        1 2023-07-30 22:27:08.000000 pymssql-2.2.7.1/src/pymssql.egg-info/dependency_links.txt
+-rw-r--r--   0 termim    (1000) sambashare   (430)        1 2023-02-23 21:54:50.000000 pymssql-2.2.7.1/src/pymssql.egg-info/not-zip-safe
+-rw-r--r--   0 termim    (1000) sambashare   (430)        8 2023-07-30 22:27:08.000000 pymssql-2.2.7.1/src/pymssql.egg-info/top_level.txt
+drwxr-xr-x   0 termim    (1000) sambashare   (430)        0 2023-07-30 22:27:09.085188 pymssql-2.2.7.1/tests/
+-rw-r--r--   0 termim    (1000) sambashare   (430)       32 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/tests/__init__.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3707 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tests/conftest.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)    14638 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tests/helpers.py
+-rwxr-xr-x   0 termim    (1000) sambashare   (430)     1913 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/tests/run_sqlalchemy_tests.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     5367 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_bulk_copy.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3936 2022-11-14 01:13:32.000000 pymssql-2.2.7.1/tests/test_config.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1294 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_connection_as_dict.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)      631 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_connection_timeout.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     5939 2023-03-19 23:14:17.000000 pymssql-2.2.7.1/tests/test_connections.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1340 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_context_managers.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1052 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_debug_queries.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     2481 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_err_handle.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     4469 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_green.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1059 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_memory.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     7321 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_pymssql.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3772 2023-02-19 23:23:57.000000 pymssql-2.2.7.1/tests/test_queries.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1270 2023-02-23 21:45:52.000000 pymssql-2.2.7.1/tests/test_query_parameters.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)    19782 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tests/test_sprocs.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     1924 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tests/test_sqlalchemy.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     3260 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_threaded.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)    12173 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tests/test_types.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)      756 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_unicode.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     5215 2022-11-13 23:14:43.000000 pymssql-2.2.7.1/tests/test_user_msghandler.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)     6119 2022-11-06 14:42:24.000000 pymssql-2.2.7.1/tests/test_utils.py
+-rw-r--r--   0 termim    (1000) sambashare   (430)      679 2022-10-10 21:37:06.000000 pymssql-2.2.7.1/tests/tests.cfg.tpl
+-rw-r--r--   0 termim    (1000) sambashare   (430)      617 2023-07-30 22:21:30.000000 pymssql-2.2.7.1/tox.ini
```

### Comparing `pymssql-2.2.7/.github/ISSUE_TEMPLATE/bug_report.md` & `pymssql-2.2.7.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/.github/workflows/test_linux.yml` & `pymssql-2.2.7.1/.github/workflows/test_linux.yml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/.github/workflows/test_macos.yml` & `pymssql-2.2.7.1/.github/workflows/test_macos.yml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/.github/workflows/test_windows.yml` & `pymssql-2.2.7.1/.github/workflows/test_windows.yml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/ChangeLog.old` & `pymssql-2.2.7.1/ChangeLog.old`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/ChangeLog.rst` & `pymssql-2.2.7.1/ChangeLog.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/Dockerfile` & `pymssql-2.2.7.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/LICENSE` & `pymssql-2.2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/PKG-INFO` & `pymssql-2.2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymssql
-Version: 2.2.7
+Version: 2.2.7.1
 Summary: DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)
 Author: Damien Churchill
 Author-email: damoxc@gmail.com
 Maintainer: Mikhail Terekhov
 Maintainer-email: termim@gmail.com
 License: LGPL
 Project-URL: Documentation, http://pymssql.readthedocs.io
```

### Comparing `pymssql-2.2.7/README.rst` & `pymssql-2.2.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/appveyor.yml` & `pymssql-2.2.7.1/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/appveyor/install-win-iconv.ps1` & `pymssql-2.2.7.1/dev/appveyor/install-win-iconv.ps1`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/appveyor/install.ps1` & `pymssql-2.2.7.1/dev/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/appveyor/run_with_env.cmd` & `pymssql-2.2.7.1/dev/appveyor/run_with_env.cmd`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1` & `pymssql-2.2.7.1/dev/appveyor/sql-server-activate-tcp-fixed-port.ps1`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/appveyor/tests.cfg` & `pymssql-2.2.7.1/dev/appveyor/tests.cfg`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/build.py` & `pymssql-2.2.7.1/dev/build.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/build_freetds.sh` & `pymssql-2.2.7.1/dev/build_freetds.sh`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/build_manylinux_wheels.sh` & `pymssql-2.2.7.1/dev/build_manylinux_wheels.sh`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/ccompiler.py` & `pymssql-2.2.7.1/dev/ccompiler.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/hudson.sh` & `pymssql-2.2.7.1/dev/hudson.sh`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/memmonitor.py` & `pymssql-2.2.7.1/dev/memmonitor.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/dev/test_manylinux_wheels.sh` & `pymssql-2.2.7.1/dev/test_manylinux_wheels.sh`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docker-compose.yml` & `pymssql-2.2.7.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/Makefile` & `pymssql-2.2.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/_mssql_examples.rst` & `pymssql-2.2.7.1/docs/_mssql_examples.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/azure.rst` & `pymssql-2.2.7.1/docs/azure.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/building_and_developing.rst` & `pymssql-2.2.7.1/docs/building_and_developing.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/conf.py` & `pymssql-2.2.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/docker.rst` & `pymssql-2.2.7.1/docs/docker.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/faq.rst` & `pymssql-2.2.7.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/freetds.rst` & `pymssql-2.2.7.1/docs/freetds.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/freetds_and_dates.rst` & `pymssql-2.2.7.1/docs/freetds_and_dates.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/history.rst` & `pymssql-2.2.7.1/docs/history.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/images/pymssql-stack.graphml` & `pymssql-2.2.7.1/docs/images/pymssql-stack.graphml`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/images/pymssql-stack.png` & `pymssql-2.2.7.1/docs/images/pymssql-stack.png`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/index.rst` & `pymssql-2.2.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/intro.rst` & `pymssql-2.2.7.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/make.bat` & `pymssql-2.2.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/migrate_1_x_to_2_x.rst` & `pymssql-2.2.7.1/docs/migrate_1_x_to_2_x.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/pymssql_examples.rst` & `pymssql-2.2.7.1/docs/pymssql_examples.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/ref/_mssql.rst` & `pymssql-2.2.7.1/docs/ref/_mssql.rst`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,14 @@
    .. versionadded:: 2.2.0
 
    The TDS version used by this connection in tuple form which is more easily
    handled (parse, compare) programmatically. Can be one of ``(4, 2)``,
    ``(5, 0)``, ``(7, 0)``, ``(7, 1)``, ``(7, 2)``, ``(7, 3)`` or ``None`` if no
    TDS version could be detected.
 
-   .. versionchanged:: 2.1.3
-      ``7.3`` was added as a possible value.
-
 ``MSSQLConnection`` object methods
 ----------------------------------
 
 .. method:: MSSQLConnection.cancel()
 
    Cancel all pending results from the last SQL operation. It can be called more
    than one time in a row. No exception is raised in this case.
```

### Comparing `pymssql-2.2.7/docs/ref/pymssql.rst` & `pymssql-2.2.7.1/docs/ref/pymssql.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/docs/release_notes.rst` & `pymssql-2.2.7.1/docs/release_notes.rst`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/setup.py` & `pymssql-2.2.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/src/pymssql/_mssql.pxd` & `pymssql-2.2.7.1/src/pymssql/_mssql.pxd`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/src/pymssql/_mssql.pyx` & `pymssql-2.2.7.1/src/pymssql/_mssql.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -241,15 +241,15 @@
         fprintf(stderr, "+++ %s\n", message)
 
 
 ###################
 ## Error Handler ##
 ###################
 cdef int err_handler(DBPROCESS *dbproc, int severity, int dberr, int oserr,
-        char *dberrstr, char *oserrstr) with gil:
+        char *dberrstr, char *oserrstr) noexcept with gil:
     cdef char *mssql_lastmsgstr
     cdef int *mssql_lastmsgno
     cdef int *mssql_lastmsgseverity
     cdef int *mssql_lastmsgstate
     cdef int _min_error_severity = min_error_severity
     cdef char mssql_message[PYMSSQL_MSGSIZE]
 
@@ -314,15 +314,15 @@
     return INT_CANCEL
 
 #####################
 ## Message Handler ##
 #####################
 cdef int msg_handler(DBPROCESS *dbproc, DBINT msgno, int msgstate,
         int severity, char *msgtext, char *srvname, char *procname,
-        LINE_T line) with gil:
+        LINE_T line) noexcept with gil:
 
     cdef int *mssql_lastmsgno
     cdef int *mssql_lastmsgseverity
     cdef int *mssql_lastmsgstate
     cdef int *mssql_lastmsgline
     cdef char *mssql_lastmsgstr
     cdef char *mssql_lastmsgsrv
```

### Comparing `pymssql-2.2.7/src/pymssql/_pymssql.pyx` & `pymssql-2.2.7.1/src/pymssql/_pymssql.pyx`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/src/pymssql/sqlfront.pxd` & `pymssql-2.2.7.1/src/pymssql/sqlfront.pxd`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/src/pymssql.egg-info/PKG-INFO` & `pymssql-2.2.7.1/src/pymssql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymssql
-Version: 2.2.7
+Version: 2.2.7.1
 Summary: DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)
 Author: Damien Churchill
 Author-email: damoxc@gmail.com
 Maintainer: Mikhail Terekhov
 Maintainer-email: termim@gmail.com
 License: LGPL
 Project-URL: Documentation, http://pymssql.readthedocs.io
```

### Comparing `pymssql-2.2.7/src/pymssql.egg-info/SOURCES.txt` & `pymssql-2.2.7.1/src/pymssql.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 tests/test_context_managers.py
 tests/test_debug_queries.py
 tests/test_err_handle.py
 tests/test_green.py
 tests/test_memory.py
 tests/test_pymssql.py
 tests/test_queries.py
+tests/test_query_parameters.py
 tests/test_sprocs.py
 tests/test_sqlalchemy.py
 tests/test_threaded.py
 tests/test_types.py
 tests/test_unicode.py
 tests/test_user_msghandler.py
 tests/test_utils.py
```

### Comparing `pymssql-2.2.7/tests/conftest.py` & `pymssql-2.2.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/helpers.py` & `pymssql-2.2.7.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/run_sqlalchemy_tests.py` & `pymssql-2.2.7.1/tests/run_sqlalchemy_tests.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_bulk_copy.py` & `pymssql-2.2.7.1/tests/test_bulk_copy.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_config.py` & `pymssql-2.2.7.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_connection_as_dict.py` & `pymssql-2.2.7.1/tests/test_connection_as_dict.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_connection_timeout.py` & `pymssql-2.2.7.1/tests/test_connection_timeout.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_connections.py` & `pymssql-2.2.7.1/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_context_managers.py` & `pymssql-2.2.7.1/tests/test_context_managers.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_debug_queries.py` & `pymssql-2.2.7.1/tests/test_debug_queries.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_err_handle.py` & `pymssql-2.2.7.1/tests/test_err_handle.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_green.py` & `pymssql-2.2.7.1/tests/test_green.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_memory.py` & `pymssql-2.2.7.1/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_pymssql.py` & `pymssql-2.2.7.1/tests/test_pymssql.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_queries.py` & `pymssql-2.2.7.1/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_sprocs.py` & `pymssql-2.2.7.1/tests/test_sprocs.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_sqlalchemy.py` & `pymssql-2.2.7.1/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_threaded.py` & `pymssql-2.2.7.1/tests/test_threaded.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_types.py` & `pymssql-2.2.7.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_unicode.py` & `pymssql-2.2.7.1/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_user_msghandler.py` & `pymssql-2.2.7.1/tests/test_user_msghandler.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/test_utils.py` & `pymssql-2.2.7.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tests/tests.cfg.tpl` & `pymssql-2.2.7.1/tests/tests.cfg.tpl`

 * *Files identical despite different names*

### Comparing `pymssql-2.2.7/tox.ini` & `pymssql-2.2.7.1/tox.ini`

 * *Files identical despite different names*

