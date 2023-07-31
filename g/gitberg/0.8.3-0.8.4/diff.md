# Comparing `tmp/gitberg-0.8.3.tar.gz` & `tmp/gitberg-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitberg-0.8.3.tar", last modified: Thu Apr 20 17:16:11 2023, max compression
+gzip compressed data, was "gitberg-0.8.4.tar", last modified: Mon Jul 31 19:52:25 2023, max compression
```

## Comparing `gitberg-0.8.3.tar` & `gitberg-0.8.4.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.591438 gitberg-0.8.3/
--rw-r--r--   0 eric       (501) staff       (20)      413 2016-03-08 17:03:43.000000 gitberg-0.8.3/CONTRIBUTING.rst
--rw-r--r--   0 eric       (501) staff       (20)     6422 2023-04-20 17:13:11.000000 gitberg-0.8.3/HISTORY.rst
--rw-r--r--   0 eric       (501) staff       (20)    35065 2016-02-05 20:21:16.000000 gitberg-0.8.3/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      126 2016-03-12 19:39:51.000000 gitberg-0.8.3/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)    35647 2023-04-20 17:16:11.591550 gitberg-0.8.3/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     2463 2022-09-26 22:28:56.000000 gitberg-0.8.3/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.546415 gitberg-0.8.3/bin/
--rwxr-xr-x   0 eric       (501) staff       (20)     5744 2022-09-26 22:28:56.000000 gitberg-0.8.3/bin/gitberg
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.547324 gitberg-0.8.3/gitberg.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)    35647 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     6739 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)      294 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       10 2023-04-20 17:16:11.000000 gitberg-0.8.3/gitberg.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.553444 gitberg-0.8.3/gitenberg/
--rw-r--r--   0 eric       (501) staff       (20)    10244 2023-04-20 16:15:38.000000 gitberg-0.8.3/gitenberg/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)      418 2023-04-20 16:10:13.000000 gitberg-0.8.3/gitenberg/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      717 2019-08-16 13:25:41.000000 gitberg-0.8.3/gitenberg/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.558570 gitberg-0.8.3/gitenberg/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      591 2020-01-02 18:44:43.000000 gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      599 2022-09-03 19:19:32.000000 gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2496 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/actions.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9466 2020-01-02 18:44:43.000000 gitberg-0.8.3/gitenberg/__pycache__/book.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9620 2022-09-03 19:19:32.000000 gitberg-0.8.3/gitenberg/__pycache__/book.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2510 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2545 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3446 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/config.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3565 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/config.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2388 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2651 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1127 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1153 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1704 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/library.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3812 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3812 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2393 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/make.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2449 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/make.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      260 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/parameters.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      268 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/parameters.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2202 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2339 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5456 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/__pycache__/push.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4585 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/__pycache__/push.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3550 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/__pycache__/workflow.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2608 2018-10-23 16:38:04.000000 gitberg-0.8.3/gitenberg/actions.py
--rw-r--r--   0 eric       (501) staff       (20)     3374 2018-10-23 16:40:03.000000 gitberg-0.8.3/gitenberg/actions.pyc
--rw-r--r--   0 eric       (501) staff       (20)    12687 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/book.py
--rw-r--r--   0 eric       (501) staff       (20)    12013 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/book.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2205 2018-09-15 18:38:44.000000 gitberg-0.8.3/gitenberg/clone.py
--rw-r--r--   0 eric       (501) staff       (20)     3139 2018-09-15 18:38:50.000000 gitberg-0.8.3/gitenberg/clone.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)     3328 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/config.py
--rw-r--r--   0 eric       (501) staff       (20)     4413 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/config.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.568389 gitberg-0.8.3/gitenberg/data/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-10-03 17:58:06.000000 gitberg-0.8.3/gitenberg/data/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)  3876689 2023-04-20 15:58:58.000000 gitberg-0.8.3/gitenberg/data/GITenberg_repo_list.tsv
--rw-r--r--   0 eric       (501) staff       (20)  1815872 2017-03-29 18:11:05.000000 gitberg-0.8.3/gitenberg/data/gutenberg_descriptions.json
--rw-r--r--   0 eric       (501) staff       (20)    57617 2022-09-26 22:31:30.000000 gitberg-0.8.3/gitenberg/data/missing.tsv
--rw-r--r--   0 eric       (501) staff       (20)       17 2020-01-18 01:02:06.000000 gitberg-0.8.3/gitenberg/data/removed.txt
--rw-r--r--   0 eric       (501) staff       (20)     2265 2020-03-24 17:09:28.000000 gitberg-0.8.3/gitenberg/dialog.py
--rw-r--r--   0 eric       (501) staff       (20)     2963 2018-05-14 18:18:37.000000 gitberg-0.8.3/gitenberg/dialog.pyc
--rw-r--r--   0 eric       (501) staff       (20)      681 2018-10-03 19:32:10.000000 gitberg-0.8.3/gitenberg/fetch.py
--rw-r--r--   0 eric       (501) staff       (20)     1365 2018-10-03 21:25:03.000000 gitberg-0.8.3/gitenberg/fetch.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.568939 gitberg-0.8.3/gitenberg/gitenberg/
--rw-r--r--   0 eric       (501) staff       (20)      243 2017-03-29 18:13:43.000000 gitberg-0.8.3/gitenberg/gitenberg/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      373 2017-11-09 21:09:26.000000 gitberg-0.8.3/gitenberg/gitenberg/__init__.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1197 2019-01-01 22:05:08.000000 gitberg-0.8.3/gitenberg/library.py
--rw-r--r--   0 eric       (501) staff       (20)     2062 2019-01-01 23:27:51.000000 gitberg-0.8.3/gitenberg/library.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3093 2020-01-02 22:45:38.000000 gitberg-0.8.3/gitenberg/local_repo.py
--rw-r--r--   0 eric       (501) staff       (20)     4380 2020-01-02 22:46:15.000000 gitberg-0.8.3/gitenberg/local_repo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2243 2018-10-20 18:41:52.000000 gitberg-0.8.3/gitenberg/make.py
--rw-r--r--   0 eric       (501) staff       (20)     2966 2018-10-20 18:42:53.000000 gitberg-0.8.3/gitenberg/make.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.572473 gitberg-0.8.3/gitenberg/metadata/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2017-03-15 21:43:48.000000 gitberg-0.8.3/gitenberg/metadata/.DS_Store
--rwxr-xr-x   0 eric       (501) staff       (20)        0 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/metadata/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      150 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.573590 gitberg-0.8.3/gitenberg/metadata/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      154 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9544 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3813 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/marc.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     7888 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     8948 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1284 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/metadata/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1458 2023-04-20 16:26:42.000000 gitberg-0.8.3/gitenberg/metadata/fileinfo.py
--rw-r--r--   0 eric       (501) staff       (20)     1752 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/fileinfo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     9254 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/licenses.py
--rw-r--r--   0 eric       (501) staff       (20)    11538 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/licenses.pyc
--rw-r--r--   0 eric       (501) staff       (20)     7973 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/metadata/marc.py
--rw-r--r--   0 eric       (501) staff       (20)     5057 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/marc.pyc
--rw-r--r--   0 eric       (501) staff       (20)     8408 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/metadata/pandata.py
--rw-r--r--   0 eric       (501) staff       (20)    10101 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/pandata.pyc
--rw-r--r--   0 eric       (501) staff       (20)       29 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/parameters.py
--rw-r--r--   0 eric       (501) staff       (20)      119 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/parameters.pyc
--rw-r--r--   0 eric       (501) staff       (20)    11568 2023-04-20 16:29:26.000000 gitberg-0.8.3/gitenberg/metadata/pg_rdf.py
--rw-r--r--   0 eric       (501) staff       (20)    11832 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/metadata/pg_rdf.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1019 2016-03-08 17:03:43.000000 gitberg-0.8.3/gitenberg/metadata/utils.py
--rw-r--r--   0 eric       (501) staff       (20)     1703 2016-03-09 21:30:05.000000 gitberg-0.8.3/gitenberg/metadata/utils.pyc
--rw-r--r--   0 eric       (501) staff       (20)      114 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/parameters.py
--rw-r--r--   0 eric       (501) staff       (20)      291 2018-03-06 20:26:11.000000 gitberg-0.8.3/gitenberg/parameters.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2003 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/pg_wikipedia.py
--rw-r--r--   0 eric       (501) staff       (20)     2926 2020-01-02 22:46:15.000000 gitberg-0.8.3/gitenberg/pg_wikipedia.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4658 2022-12-01 17:24:51.000000 gitberg-0.8.3/gitenberg/push.py
--rw-r--r--   0 eric       (501) staff       (20)     6839 2019-01-01 21:04:42.000000 gitberg-0.8.3/gitenberg/push.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.575813 gitberg-0.8.3/gitenberg/templates/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-08-30 21:11:21.000000 gitberg-0.8.3/gitenberg/templates/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)      413 2017-03-29 18:14:25.000000 gitberg-0.8.3/gitenberg/templates/CONTRIBUTING.rst
--rw-r--r--   0 eric       (501) staff       (20)    17504 2017-03-29 18:14:30.000000 gitberg-0.8.3/gitenberg/templates/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)     1986 2018-10-20 00:56:40.000000 gitberg-0.8.3/gitenberg/templates/README.rst.j2
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.580579 gitberg-0.8.3/gitenberg/tests/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2023-04-20 16:14:35.000000 gitberg-0.8.3/gitenberg/tests/.DS_Store
--rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/tests/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      147 2016-03-02 17:13:57.000000 gitberg-0.8.3/gitenberg/tests/__init__.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1324 2018-10-24 05:11:21.000000 gitberg-0.8.3/gitenberg/tests/test_book.py
--rw-r--r--   0 eric       (501) staff       (20)     2450 2018-10-24 05:11:32.000000 gitberg-0.8.3/gitenberg/tests/test_book.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1733 2018-09-05 14:03:00.000000 gitberg-0.8.3/gitenberg/tests/test_config.py
--rw-r--r--   0 eric       (501) staff       (20)     2394 2018-09-05 14:05:51.000000 gitberg-0.8.3/gitenberg/tests/test_config.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)      985 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_cover.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.581014 gitberg-0.8.3/gitenberg/tests/test_data/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2020-01-02 21:21:15.000000 gitberg-0.8.3/gitenberg/tests/test_data/.DS_Store
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.581887 gitberg-0.8.3/gitenberg/tests/test_data/1234/
--rw-r--r--   0 eric       (501) staff       (20)   154730 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_data/1234/1234.txt
--rw-r--r--   0 eric       (501) staff       (20)    10564 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/tests/test_data/1234/pg1234.rdf
--rw-r--r--   0 eric       (501) staff       (20)      176 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_data/config.yaml
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582150 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/
--rw-r--r--   0 eric       (501) staff       (20)     6148 2018-09-24 20:45:43.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/.DS_Store
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582315 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.582911 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/
--rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/HEAD
--rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/config
--rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/description
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584596 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/
--rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/post-update.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample
--rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584798 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/info/
--rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-03 19:26:13.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/info/exclude
--rw-r--r--   0 eric       (501) staff       (20)     9545 2016-08-13 21:57:29.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.584977 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.585459 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/
--rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/HEAD
--rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/config
--rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/description
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.587186 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/
--rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/post-update.sample
--rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample
--rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.587366 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/info/
--rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-15 17:13:08.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/info/exclude
--rw-r--r--   0 eric       (501) staff       (20)    11002 2018-09-24 20:32:21.000000 gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/pg7.rdf
--rw-r--r--   0 eric       (501) staff       (20)      910 2018-08-23 14:55:00.000000 gitberg-0.8.3/gitenberg/tests/test_fetch.py
--rw-r--r--   0 eric       (501) staff       (20)     1449 2018-08-23 15:14:49.000000 gitberg-0.8.3/gitenberg/tests/test_fetch.pyc
--rw-r--r--   0 eric       (501) staff       (20)     2078 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/tests/test_local_repo.py
--rw-r--r--   0 eric       (501) staff       (20)     3406 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/tests/test_local_repo.pyc
--rw-r--r--   0 eric       (501) staff       (20)     1463 2018-09-05 14:03:10.000000 gitberg-0.8.3/gitenberg/tests/test_make.py
--rw-r--r--   0 eric       (501) staff       (20)     2369 2018-09-05 14:05:51.000000 gitberg-0.8.3/gitenberg/tests/test_make.pyc
--rw-r--r--   0 eric       (501) staff       (20)     4614 2020-01-17 23:13:49.000000 gitberg-0.8.3/gitenberg/tests/test_metadata.py
--rw-r--r--   0 eric       (501) staff       (20)     6713 2020-01-02 22:46:16.000000 gitberg-0.8.3/gitenberg/tests/test_metadata.pyc
--rw-r--r--   0 eric       (501) staff       (20)      947 2018-03-06 20:16:12.000000 gitberg-0.8.3/gitenberg/tests/test_old_metadata.py
--rw-r--r--   0 eric       (501) staff       (20)     1645 2018-03-08 16:32:09.000000 gitberg-0.8.3/gitenberg/tests/test_old_metadata.pyc
--rw-r--r--   0 eric       (501) staff       (20)      839 2018-09-26 20:43:13.000000 gitberg-0.8.3/gitenberg/tests/test_push.py
--rw-r--r--   0 eric       (501) staff       (20)     1675 2018-09-26 20:43:45.000000 gitberg-0.8.3/gitenberg/tests/test_push.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.589097 gitberg-0.8.3/gitenberg/util/
--rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.3/gitenberg/util/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)      146 2016-02-05 21:55:38.000000 gitberg-0.8.3/gitenberg/util/__init__.pyc
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-04-20 17:16:11.591032 gitberg-0.8.3/gitenberg/util/__pycache__/
--rw-r--r--   0 eric       (501) staff       (20)      142 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      150 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5787 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)     5970 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      722 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)      668 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)      674 2022-09-03 19:19:34.000000 gitberg-0.8.3/gitenberg/util/__pycache__/pg.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)    18365 2020-01-02 18:44:44.000000 gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc
--rw-r--r--   0 eric       (501) staff       (20)    18375 2022-09-03 19:19:33.000000 gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc
--rw-r--r--   0 eric       (501) staff       (20)     6252 2023-02-17 22:50:16.000000 gitberg-0.8.3/gitenberg/util/catalog.py
--rw-r--r--   0 eric       (501) staff       (20)     7415 2020-01-06 13:39:38.000000 gitberg-0.8.3/gitenberg/util/catalog.pyc
--rw-r--r--   0 eric       (501) staff       (20)      653 2019-01-02 17:21:37.000000 gitberg-0.8.3/gitenberg/util/filetypes.py
--rw-r--r--   0 eric       (501) staff       (20)      986 2019-01-02 17:25:13.000000 gitberg-0.8.3/gitenberg/util/filetypes.pyc
--rw-r--r--   0 eric       (501) staff       (20)      710 2018-10-01 21:31:41.000000 gitberg-0.8.3/gitenberg/util/pg.py
--rw-r--r--   0 eric       (501) staff       (20)      826 2018-10-01 21:31:49.000000 gitberg-0.8.3/gitenberg/util/pg.pyc
--rwxr-xr-x   0 eric       (501) staff       (20)    27391 2018-08-23 14:57:32.000000 gitberg-0.8.3/gitenberg/util/tenprintcover.py
--rw-r--r--   0 eric       (501) staff       (20)    22658 2018-08-23 15:14:49.000000 gitberg-0.8.3/gitenberg/util/tenprintcover.pyc
--rw-r--r--   0 eric       (501) staff       (20)     3988 2022-09-26 22:28:56.000000 gitberg-0.8.3/gitenberg/workflow.py
--rw-r--r--   0 eric       (501) staff       (20)     4453 2019-01-02 00:03:57.000000 gitberg-0.8.3/gitenberg/workflow.pyc
--rw-r--r--   0 eric       (501) staff       (20)      523 2020-11-25 17:33:55.000000 gitberg-0.8.3/requirements.pip
--rw-r--r--   0 eric       (501) staff       (20)       67 2023-04-20 17:16:11.591892 gitberg-0.8.3/setup.cfg
--rwxr-xr-x   0 eric       (501) staff       (20)     2010 2022-12-01 17:10:57.000000 gitberg-0.8.3/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.022457 gitberg-0.8.4/
+-rw-r--r--   0 eric       (501) staff       (20)      413 2016-03-08 17:03:43.000000 gitberg-0.8.4/CONTRIBUTING.rst
+-rw-r--r--   0 eric       (501) staff       (20)     6550 2023-07-31 19:21:36.000000 gitberg-0.8.4/HISTORY.rst
+-rw-r--r--   0 eric       (501) staff       (20)    35065 2016-02-05 20:21:16.000000 gitberg-0.8.4/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      126 2016-03-12 19:39:51.000000 gitberg-0.8.4/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)    35647 2023-07-31 19:52:25.022611 gitberg-0.8.4/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     2463 2022-09-26 22:28:56.000000 gitberg-0.8.4/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.954446 gitberg-0.8.4/bin/
+-rwxr-xr-x   0 eric       (501) staff       (20)     5744 2022-09-26 22:28:56.000000 gitberg-0.8.4/bin/gitberg
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.955343 gitberg-0.8.4/gitberg.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)    35647 2023-07-31 19:52:24.000000 gitberg-0.8.4/gitberg.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     6739 2023-07-31 19:52:24.000000 gitberg-0.8.4/gitberg.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-07-31 19:52:24.000000 gitberg-0.8.4/gitberg.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)      294 2023-07-31 19:52:24.000000 gitberg-0.8.4/gitberg.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       10 2023-07-31 19:52:24.000000 gitberg-0.8.4/gitberg.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.962996 gitberg-0.8.4/gitenberg/
+-rw-r--r--   0 eric       (501) staff       (20)    10244 2023-05-17 16:03:23.000000 gitberg-0.8.4/gitenberg/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)      418 2023-07-31 19:24:08.000000 gitberg-0.8.4/gitenberg/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      717 2019-08-16 13:25:41.000000 gitberg-0.8.4/gitenberg/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.971016 gitberg-0.8.4/gitenberg/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      591 2020-01-02 18:44:43.000000 gitberg-0.8.4/gitenberg/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      599 2022-09-03 19:19:32.000000 gitberg-0.8.4/gitenberg/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2496 2022-09-03 19:19:34.000000 gitberg-0.8.4/gitenberg/__pycache__/actions.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9466 2020-01-02 18:44:43.000000 gitberg-0.8.4/gitenberg/__pycache__/book.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9620 2022-09-03 19:19:32.000000 gitberg-0.8.4/gitenberg/__pycache__/book.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2510 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/clone.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2545 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/clone.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3446 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/config.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3565 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2388 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/dialog.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2651 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/dialog.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1127 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/fetch.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1153 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/fetch.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1704 2022-09-03 19:19:34.000000 gitberg-0.8.4/gitenberg/__pycache__/library.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3812 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/local_repo.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3812 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/local_repo.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2393 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/make.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2449 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/make.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      260 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/parameters.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      268 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/parameters.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2202 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2339 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5456 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/__pycache__/push.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4585 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/__pycache__/push.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3550 2022-09-03 19:19:34.000000 gitberg-0.8.4/gitenberg/__pycache__/workflow.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2608 2018-10-23 16:38:04.000000 gitberg-0.8.4/gitenberg/actions.py
+-rw-r--r--   0 eric       (501) staff       (20)     3374 2018-10-23 16:40:03.000000 gitberg-0.8.4/gitenberg/actions.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    12687 2022-09-26 22:28:56.000000 gitberg-0.8.4/gitenberg/book.py
+-rw-r--r--   0 eric       (501) staff       (20)    12013 2020-01-06 13:39:38.000000 gitberg-0.8.4/gitenberg/book.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2205 2018-09-15 18:38:44.000000 gitberg-0.8.4/gitenberg/clone.py
+-rw-r--r--   0 eric       (501) staff       (20)     3139 2018-09-15 18:38:50.000000 gitberg-0.8.4/gitenberg/clone.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)     3328 2022-09-26 22:28:56.000000 gitberg-0.8.4/gitenberg/config.py
+-rw-r--r--   0 eric       (501) staff       (20)     4413 2020-01-06 13:39:38.000000 gitberg-0.8.4/gitenberg/config.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.982332 gitberg-0.8.4/gitenberg/data/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-10-03 17:58:06.000000 gitberg-0.8.4/gitenberg/data/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)  3921908 2023-07-31 19:21:02.000000 gitberg-0.8.4/gitenberg/data/GITenberg_repo_list.tsv
+-rw-r--r--   0 eric       (501) staff       (20)  1815872 2017-03-29 18:11:05.000000 gitberg-0.8.4/gitenberg/data/gutenberg_descriptions.json
+-rw-r--r--   0 eric       (501) staff       (20)    57617 2022-09-26 22:31:30.000000 gitberg-0.8.4/gitenberg/data/missing.tsv
+-rw-r--r--   0 eric       (501) staff       (20)       17 2020-01-18 01:02:06.000000 gitberg-0.8.4/gitenberg/data/removed.txt
+-rw-r--r--   0 eric       (501) staff       (20)     2265 2020-03-24 17:09:28.000000 gitberg-0.8.4/gitenberg/dialog.py
+-rw-r--r--   0 eric       (501) staff       (20)     2963 2018-05-14 18:18:37.000000 gitberg-0.8.4/gitenberg/dialog.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      681 2018-10-03 19:32:10.000000 gitberg-0.8.4/gitenberg/fetch.py
+-rw-r--r--   0 eric       (501) staff       (20)     1365 2018-10-03 21:25:03.000000 gitberg-0.8.4/gitenberg/fetch.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.983133 gitberg-0.8.4/gitenberg/gitenberg/
+-rw-r--r--   0 eric       (501) staff       (20)      243 2017-03-29 18:13:43.000000 gitberg-0.8.4/gitenberg/gitenberg/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      373 2017-11-09 21:09:26.000000 gitberg-0.8.4/gitenberg/gitenberg/__init__.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1197 2019-01-01 22:05:08.000000 gitberg-0.8.4/gitenberg/library.py
+-rw-r--r--   0 eric       (501) staff       (20)     2062 2019-01-01 23:27:51.000000 gitberg-0.8.4/gitenberg/library.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3093 2020-01-02 22:45:38.000000 gitberg-0.8.4/gitenberg/local_repo.py
+-rw-r--r--   0 eric       (501) staff       (20)     4380 2020-01-02 22:46:15.000000 gitberg-0.8.4/gitenberg/local_repo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2243 2018-10-20 18:41:52.000000 gitberg-0.8.4/gitenberg/make.py
+-rw-r--r--   0 eric       (501) staff       (20)     2966 2018-10-20 18:42:53.000000 gitberg-0.8.4/gitenberg/make.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.994830 gitberg-0.8.4/gitenberg/metadata/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2017-03-15 21:43:48.000000 gitberg-0.8.4/gitenberg/metadata/.DS_Store
+-rwxr-xr-x   0 eric       (501) staff       (20)        0 2020-01-17 23:13:49.000000 gitberg-0.8.4/gitenberg/metadata/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      150 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/metadata/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.997047 gitberg-0.8.4/gitenberg/metadata/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      154 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9544 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3813 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/marc.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     7888 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     8948 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1284 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/metadata/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1458 2023-04-20 16:26:42.000000 gitberg-0.8.4/gitenberg/metadata/fileinfo.py
+-rw-r--r--   0 eric       (501) staff       (20)     1752 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/metadata/fileinfo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     9254 2016-03-08 17:03:43.000000 gitberg-0.8.4/gitenberg/metadata/licenses.py
+-rw-r--r--   0 eric       (501) staff       (20)    11538 2016-03-09 21:30:05.000000 gitberg-0.8.4/gitenberg/metadata/licenses.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     7973 2020-01-17 23:13:49.000000 gitberg-0.8.4/gitenberg/metadata/marc.py
+-rw-r--r--   0 eric       (501) staff       (20)     5057 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/metadata/marc.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     8408 2022-09-26 22:28:56.000000 gitberg-0.8.4/gitenberg/metadata/pandata.py
+-rw-r--r--   0 eric       (501) staff       (20)    10101 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/metadata/pandata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)       29 2016-03-08 17:03:43.000000 gitberg-0.8.4/gitenberg/metadata/parameters.py
+-rw-r--r--   0 eric       (501) staff       (20)      119 2016-03-09 21:30:05.000000 gitberg-0.8.4/gitenberg/metadata/parameters.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    11568 2023-04-20 16:29:26.000000 gitberg-0.8.4/gitenberg/metadata/pg_rdf.py
+-rw-r--r--   0 eric       (501) staff       (20)    11832 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/metadata/pg_rdf.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1019 2016-03-08 17:03:43.000000 gitberg-0.8.4/gitenberg/metadata/utils.py
+-rw-r--r--   0 eric       (501) staff       (20)     1703 2016-03-09 21:30:05.000000 gitberg-0.8.4/gitenberg/metadata/utils.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      114 2018-03-06 20:16:12.000000 gitberg-0.8.4/gitenberg/parameters.py
+-rw-r--r--   0 eric       (501) staff       (20)      291 2018-03-06 20:26:11.000000 gitberg-0.8.4/gitenberg/parameters.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2003 2020-01-17 23:13:49.000000 gitberg-0.8.4/gitenberg/pg_wikipedia.py
+-rw-r--r--   0 eric       (501) staff       (20)     2926 2020-01-02 22:46:15.000000 gitberg-0.8.4/gitenberg/pg_wikipedia.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4783 2023-07-19 20:28:57.000000 gitberg-0.8.4/gitenberg/push.py
+-rw-r--r--   0 eric       (501) staff       (20)     6839 2019-01-01 21:04:42.000000 gitberg-0.8.4/gitenberg/push.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:24.998745 gitberg-0.8.4/gitenberg/templates/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-08-30 21:11:21.000000 gitberg-0.8.4/gitenberg/templates/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)      413 2017-03-29 18:14:25.000000 gitberg-0.8.4/gitenberg/templates/CONTRIBUTING.rst
+-rw-r--r--   0 eric       (501) staff       (20)    17504 2017-03-29 18:14:30.000000 gitberg-0.8.4/gitenberg/templates/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)     1986 2018-10-20 00:56:40.000000 gitberg-0.8.4/gitenberg/templates/README.rst.j2
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.006344 gitberg-0.8.4/gitenberg/tests/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2023-04-20 16:14:35.000000 gitberg-0.8.4/gitenberg/tests/.DS_Store
+-rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.4/gitenberg/tests/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      147 2016-03-02 17:13:57.000000 gitberg-0.8.4/gitenberg/tests/__init__.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1324 2018-10-24 05:11:21.000000 gitberg-0.8.4/gitenberg/tests/test_book.py
+-rw-r--r--   0 eric       (501) staff       (20)     2450 2018-10-24 05:11:32.000000 gitberg-0.8.4/gitenberg/tests/test_book.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1733 2018-09-05 14:03:00.000000 gitberg-0.8.4/gitenberg/tests/test_config.py
+-rw-r--r--   0 eric       (501) staff       (20)     2394 2018-09-05 14:05:51.000000 gitberg-0.8.4/gitenberg/tests/test_config.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)      985 2018-03-06 20:16:12.000000 gitberg-0.8.4/gitenberg/tests/test_cover.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.006777 gitberg-0.8.4/gitenberg/tests/test_data/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2020-01-02 21:21:15.000000 gitberg-0.8.4/gitenberg/tests/test_data/.DS_Store
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.007390 gitberg-0.8.4/gitenberg/tests/test_data/1234/
+-rw-r--r--   0 eric       (501) staff       (20)   154730 2018-03-06 20:16:12.000000 gitberg-0.8.4/gitenberg/tests/test_data/1234/1234.txt
+-rw-r--r--   0 eric       (501) staff       (20)    10564 2016-02-05 20:21:16.000000 gitberg-0.8.4/gitenberg/tests/test_data/1234/pg1234.rdf
+-rw-r--r--   0 eric       (501) staff       (20)      176 2018-03-06 20:16:12.000000 gitberg-0.8.4/gitenberg/tests/test_data/config.yaml
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.007686 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/
+-rw-r--r--   0 eric       (501) staff       (20)     6148 2018-09-24 20:45:43.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/.DS_Store
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.007940 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.008724 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/
+-rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/HEAD
+-rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/config
+-rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/description
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.011352 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/
+-rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/post-update.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample
+-rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.011549 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/info/
+-rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-03 19:26:13.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/info/exclude
+-rw-r--r--   0 eric       (501) staff       (20)     9545 2016-08-13 21:57:29.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.011725 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.012274 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/
+-rw-r--r--   0 eric       (501) staff       (20)       23 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/HEAD
+-rw-r--r--   0 eric       (501) staff       (20)      137 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/config
+-rw-r--r--   0 eric       (501) staff       (20)       73 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/description
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.014257 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/
+-rwxr-xr-x   0 eric       (501) staff       (20)      478 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      896 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      189 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/post-update.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)      424 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1642 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1348 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     4951 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample
+-rw-r--r--   0 eric       (501) staff       (20)      544 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     1239 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 eric       (501) staff       (20)     3610 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.014467 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/info/
+-rw-r--r--   0 eric       (501) staff       (20)      240 2017-03-15 17:13:08.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/info/exclude
+-rw-r--r--   0 eric       (501) staff       (20)    11002 2018-09-24 20:32:21.000000 gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/pg7.rdf
+-rw-r--r--   0 eric       (501) staff       (20)      910 2018-08-23 14:55:00.000000 gitberg-0.8.4/gitenberg/tests/test_fetch.py
+-rw-r--r--   0 eric       (501) staff       (20)     1449 2018-08-23 15:14:49.000000 gitberg-0.8.4/gitenberg/tests/test_fetch.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     2078 2020-01-17 23:13:49.000000 gitberg-0.8.4/gitenberg/tests/test_local_repo.py
+-rw-r--r--   0 eric       (501) staff       (20)     3406 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/tests/test_local_repo.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     1463 2018-09-05 14:03:10.000000 gitberg-0.8.4/gitenberg/tests/test_make.py
+-rw-r--r--   0 eric       (501) staff       (20)     2369 2018-09-05 14:05:51.000000 gitberg-0.8.4/gitenberg/tests/test_make.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     4614 2020-01-17 23:13:49.000000 gitberg-0.8.4/gitenberg/tests/test_metadata.py
+-rw-r--r--   0 eric       (501) staff       (20)     6713 2020-01-02 22:46:16.000000 gitberg-0.8.4/gitenberg/tests/test_metadata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      947 2018-03-06 20:16:12.000000 gitberg-0.8.4/gitenberg/tests/test_old_metadata.py
+-rw-r--r--   0 eric       (501) staff       (20)     1645 2018-03-08 16:32:09.000000 gitberg-0.8.4/gitenberg/tests/test_old_metadata.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      839 2018-09-26 20:43:13.000000 gitberg-0.8.4/gitenberg/tests/test_push.py
+-rw-r--r--   0 eric       (501) staff       (20)     1675 2018-09-26 20:43:45.000000 gitberg-0.8.4/gitenberg/tests/test_push.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.019341 gitberg-0.8.4/gitenberg/util/
+-rw-r--r--   0 eric       (501) staff       (20)        0 2016-02-05 20:21:16.000000 gitberg-0.8.4/gitenberg/util/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)      146 2016-02-05 21:55:38.000000 gitberg-0.8.4/gitenberg/util/__init__.pyc
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-07-31 19:52:25.022010 gitberg-0.8.4/gitenberg/util/__pycache__/
+-rw-r--r--   0 eric       (501) staff       (20)      142 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/util/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      150 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/util/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5787 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/util/__pycache__/catalog.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     5970 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/util/__pycache__/catalog.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      722 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/util/__pycache__/filetypes.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      668 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/util/__pycache__/filetypes.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      674 2022-09-03 19:19:34.000000 gitberg-0.8.4/gitenberg/util/__pycache__/pg.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    18365 2020-01-02 18:44:44.000000 gitberg-0.8.4/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc
+-rw-r--r--   0 eric       (501) staff       (20)    18375 2022-09-03 19:19:33.000000 gitberg-0.8.4/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     6252 2023-02-17 22:50:16.000000 gitberg-0.8.4/gitenberg/util/catalog.py
+-rw-r--r--   0 eric       (501) staff       (20)     7415 2020-01-06 13:39:38.000000 gitberg-0.8.4/gitenberg/util/catalog.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      653 2019-01-02 17:21:37.000000 gitberg-0.8.4/gitenberg/util/filetypes.py
+-rw-r--r--   0 eric       (501) staff       (20)      986 2019-01-02 17:25:13.000000 gitberg-0.8.4/gitenberg/util/filetypes.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      710 2018-10-01 21:31:41.000000 gitberg-0.8.4/gitenberg/util/pg.py
+-rw-r--r--   0 eric       (501) staff       (20)      826 2018-10-01 21:31:49.000000 gitberg-0.8.4/gitenberg/util/pg.pyc
+-rwxr-xr-x   0 eric       (501) staff       (20)    27391 2018-08-23 14:57:32.000000 gitberg-0.8.4/gitenberg/util/tenprintcover.py
+-rw-r--r--   0 eric       (501) staff       (20)    22658 2018-08-23 15:14:49.000000 gitberg-0.8.4/gitenberg/util/tenprintcover.pyc
+-rw-r--r--   0 eric       (501) staff       (20)     3988 2022-09-26 22:28:56.000000 gitberg-0.8.4/gitenberg/workflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     4453 2019-01-02 00:03:57.000000 gitberg-0.8.4/gitenberg/workflow.pyc
+-rw-r--r--   0 eric       (501) staff       (20)      523 2020-11-25 17:33:55.000000 gitberg-0.8.4/requirements.pip
+-rw-r--r--   0 eric       (501) staff       (20)       67 2023-07-31 19:52:25.023018 gitberg-0.8.4/setup.cfg
+-rwxr-xr-x   0 eric       (501) staff       (20)     2010 2022-12-01 17:10:57.000000 gitberg-0.8.4/setup.py
```

### Comparing `gitberg-0.8.3/HISTORY.rst` & `gitberg-0.8.4/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 .. :changelog:
 
 History
 -------
+0.8.4 (2023-07-31)
+==================
+* try to stop making new when ratelimit comes in
+* update repo lists
+  * add 70402-71226
+
 0.8.3 (2023-04-20)
 ==================
 * fix opening rdf files and reading mod date
 * update repo lists
   * add 69347-70401
 
 0.8.2 (2022-12-07)
```

### Comparing `gitberg-0.8.3/LICENSE` & `gitberg-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/PKG-INFO` & `gitberg-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitberg
-Version: 0.8.3
+Version: 0.8.4
 Summary: A library and command for interacting with the GITenberg books project
 Home-page: https://github.com/gitenberg-dev/gitberg
 Author: Seth Woodworth
 Author-email: seth@sethish.com
 License: GPLv3
 Keywords: books ebooks gitenberg gutenberg epub metadata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitberg-0.8.3/README.md` & `gitberg-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/bin/gitberg` & `gitberg-0.8.4/bin/gitberg`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitberg.egg-info/PKG-INFO` & `gitberg-0.8.4/gitberg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitberg
-Version: 0.8.3
+Version: 0.8.4
 Summary: A library and command for interacting with the GITenberg books project
 Home-page: https://github.com/gitenberg-dev/gitberg
 Author: Seth Woodworth
 Author-email: seth@sethish.com
 License: GPLv3
 Keywords: books ebooks gitenberg gutenberg epub metadata
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `gitberg-0.8.3/gitberg.egg-info/SOURCES.txt` & `gitberg-0.8.4/gitberg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/.DS_Store` & `gitberg-0.8.4/gitenberg/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 2000 0000 0800  ....Bud1.. .....
 00000010: 0000 2000 0000 100c 0000 0000 0000 0000  .. .............
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0011  ................
 00000050: 0000 0001 0000 1000 6473 636c 626f 6f6c  ........dsclbool
-00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000060: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -252,15 +252,15 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 0011 0000 0004  ................
 00001010: 0064 0061 0074 0061 6473 636c 626f 6f6c  .d.a.t.adsclbool
-00001020: 0000 0000 0400 6400 6100 7400 6166 6473  ......d.a.t.afds
+00001020: 0100 0000 0400 6400 6100 7400 6166 6473  ......d.a.t.afds
 00001030: 6362 6f6f 6c01 0000 0004 0064 0061 0074  cbool......d.a.t
 00001040: 0061 6c67 3153 636f 6d70 0000 0000 0000  .alg1Scomp......
 00001050: 0000 0000 0004 0064 0061 0074 0061 6d6f  .......d.a.t.amo
 00001060: 4444 6475 7463 0000 d304 e6f7 0000 0000  DDdutc..........
 00001070: 0004 0064 0061 0074 0061 6d6f 6444 6475  ...d.a.t.amodDdu
 00001080: 7463 0000 d304 e6f7 0000 0000 0004 0064  tc.............d
 00001090: 0061 0074 0061 7068 3153 636f 6d70 0000  .a.t.aph1Scomp..
```

### Comparing `gitberg-0.8.3/gitenberg/__init__.pyc` & `gitberg-0.8.4/gitenberg/__init__.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/__init__.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/__init__.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/actions.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/actions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/book.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/book.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/book.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/book.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/clone.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/clone.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/clone.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/config.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/config.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/config.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/dialog.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/dialog.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/dialog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/fetch.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/fetch.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/fetch.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/library.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/library.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/local_repo.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/local_repo.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/local_repo.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/make.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/make.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/make.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/make.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/pg_wikipedia.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/pg_wikipedia.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/push.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/push.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/push.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/push.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/__pycache__/workflow.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/__pycache__/workflow.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/actions.py` & `gitberg-0.8.4/gitenberg/actions.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/actions.pyc` & `gitberg-0.8.4/gitenberg/actions.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/book.py` & `gitberg-0.8.4/gitenberg/book.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/book.pyc` & `gitberg-0.8.4/gitenberg/book.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/clone.py` & `gitberg-0.8.4/gitenberg/clone.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/clone.pyc` & `gitberg-0.8.4/gitenberg/clone.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/config.py` & `gitberg-0.8.4/gitenberg/config.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/config.pyc` & `gitberg-0.8.4/gitenberg/config.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/data/.DS_Store` & `gitberg-0.8.4/gitenberg/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/data/GITenberg_repo_list.tsv` & `gitberg-0.8.4/gitenberg/data/GITenberg_repo_list.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -69880,8 +69880,833 @@
 70394	Travels-in-the-Upper-Egyptian-deserts_70394
 70395	De-zwervers-op-de-grenzen-b-Naar-de-achtste-Fransche-uitgave_70395
 70396	Chroniques-de-J-Froissart-tome-1013_70396
 70397	How-to-swim-b-A-practical-manual-of-swimming-by-a-practical-swimmer-and-a-guide-to-the-novice__70397
 70398	A-bibliography-of-the-writings-of-D-H-Lawrence_70398
 70399	The-clammer_70399
 70400	The-cheerful-blackguard_70400
-70401	By-paths-in-Hebraic-bookland_70401
+70401	By-paths-in-Hebraic-bookland_70401
+70402	Dynasty-of-the-lost_70402
+70403	The-miniature-menace_70403
+70404	The-Negro-as-a-soldier_70404
+70405	Selected-etchings-by-Piranesi-series-1_70405
+70406	Tarasconin-Tartarin_70406
+70407	The-life-savers-of-Cape-Cod_70407
+70408	Napoleon-s-British-visitors-and-captives-1801-1815_70408
+70409	Vacuum-cleaning-systems-b-A-treatise-on-the-principles-and-practice-of-mechanical-cleaning_70409
+70410	A-history-of-commerce_70410
+70411	Godey-s-Lady-s-Book-Vol-48-June-1854_70411
+70412	Scripture-texts-illustrated-by-general-literature_70412
+70413	The-presidential-snapshot-b-or-The-all-seeing-eye_70413
+70414	Training-Infantry_70414
+70415	The-boy-s-book-of-battle-lyrics-b-a-collection-of-verses-illustrating-some-notable-events-in-__70415
+70416	Emmanuel-Burden-merchant-of-Thames-St-in-the-city-of-London-exporter-of-hardware-b-A-record-o__70416
+70417	Tinting-and-toning-of-Eastman-positive-motion-picture-film-b-Second-editionrevised_70417
+70418	Maritime-enterprise-1485-1558_70418
+70419	History-of-Christian-names_70419
+70420	Plymouth-memories-of-an-octogenarian_70420
+70421	Dingaansdag_70421
+70422	Ma-Fille-Bernadette_70422
+70423	L-Ile-d-Enfer_70423
+70424	Old-nurse-s-book-of-rhymes-jingles-and-ditties_70424
+70425	Narrative-of-the-Fenian-invasion-of-Canada_70425
+70426	Men-of-Marlowe-s_70426
+70427	History-for-ready-reference-Volumes-1-to-5_70427
+70428	Maantiede-ja-loytoretket-4-b-Uusin-aika-17-vuosisadan-alusta-nykyaikaan-loppupuoli_70428
+70429	The-Radio-Girls-on-the-program-b-or-Singing-and-reciting-at-the-sending-station_70429
+70430	Studi-sulla-letteratura-contemporanea-b-Prima-serie_70430
+70431	Between-two-thieves_70431
+70432	Clouds-of-witness_70432
+70433	The-floral-symbolism-of-the-great-masters_70433
+70434	Americans-by-adoption-b-Brief-biographies-of-great-citizens-born-in-foreign-lands_70434
+70435	Bingo-und-andere-Tiergeschichten_70435
+70436	Devil-tales_70436
+70437	The-eagle-s-masque_70437
+70438	Women-compositors-b-A-guide-to-the-composing-room_70438
+70439	In-het-land-der-zon-b-Een-kwart-eeuw-tusschen-de-keerkringen_70439
+70440	The-awakening_70440
+70441	The-Anzac-Book_70441
+70442	The-Barnum-Bailey-Greatest-Show-on-Earth-songster_70442
+70443	Governor-Bradford-s-first-dialogue-b-A-dialogue-or-the-sum-of-a-conference-between-some-young__70443
+70444	French-English-b-A-comparison_70444
+70445	Host-and-Guest-b-a-book-about-dinners-dinner-giving-wines-and-desserts_70445
+70446	Olivia-b-or-It-was-for-her-sake_70446
+70447	The-Nantucket-Indians_70447
+70448	Tokology-b-A-book-for-every-woman_70448
+70449	Bluffer-s-luck_70449
+70450	The-boys-in-white-b-The-experience-of-a-hospital-agent-in-and-around-Washington_70450
+70451	Haeckel-b-his-life-and-work_70451
+70452	The-man-eaters-and-other-odd-people-b-A-popular-description-of-singular-races-of-man_70452
+70453	Clerk-Maxwell-s-electromagnetic-theory_70453
+70454	Der-Bruderhof-b-Eine-bauerliche-Liebes-und-Leidens-Geschichte_70454
+70455	Angel-s-Brother_70455
+70456	Tomato-products-pulp-ketchup-and-chili-sauce_70456
+70457	Tumbling-river-range_70457
+70458	Primitive-culture-vol-1-of-2-b-Researches-into-the-development-of-mythology-philosophy-religi__70458
+70459	To-let_70459
+70460	Docas-b-The-Indian-boy-of-Santa-Clara_70460
+70461	An-Egyptian-oasis-b-An-account-of-the-oasis-of-Kharga-in-the-Libyan-desert-with-special-refer__70461
+70462	The-hermit-of-the-forest-b-or-Wandering-infants-a-rural-tale_70462
+70463	The-Pennsylvania-Journal-of-prison-discipline-and-philanthropy-Vol-VIII-No-III-July-1853_70463
+70464	Absolutely-no-paradox_70464
+70465	Opinions_70465
+70466	Reaching-for-the-moon_70466
+70467	The-attache-at-Peking_70467
+70468	Rebilius-Cruso-b-Robinson-Crusoe-in-Latin-a-book-to-lighten-tedium-to-a-learner_70468
+70469	Papa-Bouchard_70469
+70470	The-Bodleian-Library-at-Oxford_70470
+70471	Kabuki-b-The-popular-stage-of-Japan_70471
+70472	Randvar-the-songsmith-b-A-romance-of-Norumbega_70472
+70473	Forrest-House-b-A-novel_70473
+70474	Queenie-Hetherton_70474
+70475	Atomic-bonanza_70475
+70476	India-b-the-pearl-of-Pearl-River_70476
+70477	The-O-S-U-Naturalist-Vol-1-No-2-December-1900_70477
+70478	The-silver-key_70478
+70479	Geoffrey-s-victory-b-or-the-double-deception_70479
+70480	Old-Cape-Cod-b-the-land-the-men-the-sea_70480
+70481	A-man-made-of-money_70481
+70482	Prosperity-s-child_70482
+70483	Children-of-the-lens_70483
+70484	Primitive-culture-vol-2-of-2-b-Researches-into-the-development-of-mythology-philosophy-religi__70484
+70485	The-things-which-belong_70485
+70486	The-lurking-fear_70486
+70487	A-new-name_70487
+70488	The-keeper-of-Red-Horse-Pass_70488
+70489	A-true-exact-history-of-the-island-of-Barbados_70489
+70490	Polite-bunny_70490
+70491	Elfin-Land_70491
+70492	Aspects-of-the-novel_70492
+70493	The-Prince-of-Wales-and-other-famous-Americans_70493
+70494	Second-stage-Lensmen_70494
+70495	The-great-inquiry_70495
+70496	Turn-backward-o-time_70496
+70497	The-Oxford-Methodists-b-Memoirs-of-the-Rev-Messrs-Clayton-Ingham-Gambold-Hervey-and-Broughton__70497
+70498	The-evergreen-tree_70498
+70499	Medium-boiled_70499
+70500	Gentlemen-please-note_70500
+70501	Moon-of-memory_70501
+70502	On-the-red-staircase_70502
+70503	Washington-its-sights-and-insights-1903_70503
+70504	Barnavaux-et-quelques-femmes_70504
+70505	Louise-et-Barnavaux_70505
+70506	The-family-at-Misrule_70506
+70507	The-Cornhill-Magazine-Vol-I-No-5-May-1860_70507
+70508	The-Cornhill-Magazine-Vol-I-No-6-June-1860_70508
+70509	A-caricature-history-of-Canadian-politics-b-events-from-the-union-of-1841-as-illustrated-by-c__70509
+70510	Hiljaisten-metsien-tytto_70510
+70511	De-republiek-van-Plato-b-In-het-Nederduitsch-overgebragt_70511
+70512	The-life-travels-exploits-frauds-and-robberies-of-Charles-Speckman-alias-Brown-who-was-execut__70512
+70513	The-non-stop-stowaway-b-The-story-of-a-long-distance-flight_70513
+70514	The-Survey-volume-30-number-7-May-17-1913_70514
+70515	Yuletide-entertainments-b-Christmas-recitations-monologues-drills-tableaux-motion-songs-exerc__70515
+70516	Now-we-are-six_70516
+70517	The-glue-book-b-How-to-select-prepare-and-use-glue_70517
+70518	Nippon-orszag-naposkertje-b-Japan-nepmesek_70518
+70519	A-csokok-ejszakaja-es-egyeb-elbeszelesek_70519
+70520	Naomi-b-or-the-last-days-of-Jerusalem_70520
+70521	The-hermit-s-Christmas_70521
+70522	For-the-freedom-of-the-seas_70522
+70523	Remarks-on-the-speeches-of-William-Paul-Clerk-and-John-Hall-of-Otterburn-Esq-b-Executed-at-Ty__70523
+70524	Bird-s-nest-a-fantasy-in-one-act_70524
+70525	Sahara_70525
+70526	The-Canterbury-pilgrims-b-A-comedy_70526
+70527	The-Eagle-s-eye_70527
+70528	English-printers-ornaments_70528
+70529	Little-Arthur-s-history-of-England_70529
+70530	Physician-and-patient-b-or-a-practical-view-of-the-mutual-duties-relations-and-interests-of-t__70530
+70531	The-seven-books-of-Paulus-0xc6gineta-volume-1-of-3-b-translated-from-the-Greek-with-a-comment__70531
+70532	The-seven-books-of-Paulus-0xc6gineta-volume-2-of-3-b-translated-from-the-Greek-with-a-comment__70532
+70533	The-seven-books-of-Paulus-0xc6gineta-volume-3-of-3-b-translated-from-the-Greek-with-a-comment__70533
+70534	Les-creux-de-maisons_70534
+70535	The-world-s-navies-in-the-Boxer-rebellion-China-1900_70535
+70536	The-land-of-hidden-men_70536
+70537	The-city-of-Jerusalem_70537
+70538	Job-le-predestine_70538
+70539	Chambers-s-Journal-of-Popular-Literature-Science-and-Art-fifth-series-no-124-vol-III-May-15-1__70539
+70540	Skulls-in-the-stars_70540
+70541	Star-bright_70541
+70542	Comedias-tomo-3-de-3-b-Las-Fiestas-de-Ceres-las-Ranas-las-Junteras-Pluto_70542
+70543	Color_70543
+70544	Parodies-of-the-works-of-English-American-authors-vol-II_70544
+70545	Parodies-of-the-works-of-English-American-authors-vol-III_70545
+70546	Parodies-of-the-works-of-English-American-authors-vol-IV_70546
+70547	Parodies-of-the-works-of-English-American-authors-vol-V_70547
+70548	Parodies-of-the-works-of-English-American-authors-vol-VI_70548
+70549	Fugue_70549
+70550	The-miracle-of-Saint-Anthony_70550
+70551	Peter-Voss-der-Millionendieb-Roman_70551
+70552	Righteous-plague_70552
+70553	Trotwood-s-Monthly-Vol-I-No-3-December-1905_70553
+70554	Sir-Richard-s-grandson-b-or-A-soldier-s-son_70554
+70555	The-feather-symbol-in-ancient-Hopi-designs_70555
+70556	Accounting-theory-and-practice-Volume-2-of-3-b-a-textbook-for-colleges-and-schools-of-busines__70556
+70557	Robert-Merry-s-Museum-Vol-VII-No-1-6_70557
+70558	Sanovat-miehen-sammuneen_70558
+70559	Survival-of-the-fittest_70559
+70560	Wie-es-Licht-geworden-b-Roman_70560
+70561	The-writings-of-Origen-Vol-1-of-2_70561
+70562	Be-young-again_70562
+70563	The-romance-of-my-childhood-and-youth_70563
+70564	Landesverein-Sachsischer-Heimatschutz-Mitteilungen-Band-XII-Heft-7-9-b-Monatsschrift-fur-Heim__70564
+70565	A-thousand-miles-up-the-Nile_70565
+70566	The-Collected-Works-of-Henrik-Ibsen-Vol-07-of-11_70566
+70567	Grundzuge-der-Palaontologie-Palaozoologie-1-Abteilung-Invertebrata_70567
+70568	Debating-for-boys_70568
+70569	Pvcna-porcorvm_70569
+70570	Red-shadows_70570
+70571	Earth-needs-a-killer_70571
+70572	Bomba-the-jungle-boy-b-or-The-old-naturalist-s-secret_70572
+70573	Bucolic-Beatitudes_70573
+70574	Little-Jack-Rabbit-s-big-blue-book_70574
+70575	Marooned-on-Australia-b-being-the-narration-by-Diedrich-Buys-of-his-discoveries-and-exploits-__70575
+70576	Felicidade-pela-Agricultura-Vol-II_70576
+70577	The-Collected-Works-of-Henrik-Ibsen-Vol-08-of-11_70577
+70578	Short-story-classics-Foreign-Vol-2-Italian-and-Scandinavian_70578
+70579	The-philosophy-of-Elbert-Hubbard_70579
+70580	No-war-tomorrow_70580
+70581	Botanical-features-of-the-Algerian-Sahara_70581
+70582	Her-fairy-prince_70582
+70583	Stopwatch-on-the-world_70583
+70584	Chambers-s-journal-of-popular-literature-science-and-art-fifth-series-no-125-vol-III-May-22-1__70584
+70585	Afrikan-viimeinen-kuningas_70585
+70586	Cutting-and-draping-b-a-practical-handbook-for-upholsterers-and-decorators_70586
+70587	Terry_70587
+70588	Richardson-s-New-London-fashionable-gentleman-s-valentine-writer-or-the-lover-s-own-book-for-__70588
+70589	Tarzan-and-the-lost-empire_70589
+70590	Dark-recess_70590
+70591	Elizabeth-Montagu-the-queen-of-the-bluestockings-Volume-1-of-2-b-Her-correspondence-from-1720__70591
+70592	Elizabeth-Montagu-the-queen-of-the-bluestockings-Volume-2-of-2-b-Her-correspondence-from-1720__70592
+70593	Elizabeth-Montagu-the-queen-of-the-bluestockings-Volumes-1-and-2-b-Her-correspondence-from-17__70593
+70594	The-Engadine_70594
+70595	A-visit-to-the-Bazaar_70595
+70596	The-Byzantines_70596
+70597	The-collector-s-whatnot-b-a-compendium-manual-and-syllabus-of-information-and-advice-on-all-s__70597
+70598	A-Pet-Reader_70598
+70599	The-trumpet-in-the-dust_70599
+70600	WantedLeaders-b-A-study-of-Negro-development_70600
+70601	Archeology-of-the-lower-Mimbres-valley-New-Mexico_70601
+70602	Kosinta-b-Yksinaytoksinen-pila_70602
+70603	Maantieta-pitkin_70603
+70604	Sophokles_70604
+70605	The-black-alarm_70605
+70606	The-last-test_70606
+70607	Little-soldiers-all_70607
+70608	Chambers-s-Journal-of-Popular-Literature-Science-and-Art-fifth-series-no-126-vol-III-May-29-1__70608
+70609	Natalie-b-Ein-Beitrag-zur-Geschichte-des-weiblichen-Herzens_70609
+70610	The-grandfathers-war_70610
+70611	US-copyright-renewals-artwork-1965-1977_70611
+70612	Les-moyens-du-bord-b-roman_70612
+70613	A-reply-to-The-affectionate-and-Christian-address-of-many-thousands-of-women-of-Great-Britain__70613
+70614	Tommy-Tiptop-and-his-baseball-nine-b-or-The-boys-of-Riverdale-and-their-good-times_70614
+70615	The-ritual-and-significance-of-the-Winnebago-medicine-dance_70615
+70616	Karhu-b-Pila-yhdessa-naytoksessa_70616
+70617	Laululintunen-b-Laulusekainen-naytelma-yhdessa-naytoksessa_70617
+70618	Lemminkainen-b-Viisinaytoksinen-naytelma_70618
+70619	A-history-of-criticism-and-literary-taste-in-Europe-from-the-earliest-texts-to-the-present-da__70619
+70620	The-logic-of-modern-physics_70620
+70621	Oxford-and-the-Rhodes-Scholarships_70621
+70622	The-stainless-steel-rat_70622
+70623	The-deadly-thinkers_70623
+70624	Sanitation-in-Panama_70624
+70625	Debts-hopeful-and-desperate-b-Financing-the-Plymouth-Colony_70625
+70626	The-tragedy-of-Monomoy-Beach-b-The-graveyard-of-the-Atlantic_70626
+70627	Uncle-Wiggily-s-June-Bug-friends-b-or-How-the-June-Bugs-brought-joy-to-Uncle-Wiggily-and-The-__70627
+70628	A-popular-history-of-the-United-States-of-America-Vol-1-of-2-b-from-the-discovery-of-the-Amer__70628
+70629	A-popular-history-of-the-United-States-of-America-Vol-2-of-2-b-from-the-discovery-of-the-Amer__70629
+70630	Public-opinion-and-the-teaching-of-history-in-the-United-States_70630
+70631	Storia-universale-del-canto-Vol-1-of-2_70631
+70632	Storia-universale-del-canto-Vol-2-of-2_70632
+70633	The-Territorial-Divisions-1914-1918_70633
+70634	The-Benson-murder-case_70634
+70635	Lively-plays-for-live-people_70635
+70636	Dropped-stitches-in-Tennessee-history_70636
+70637	Journal-of-Herbert-Edward-Pretyman-written-during-his-expedition-to-the-Kittar-Mountains-betw__70637
+70638	Ribbon-in-the-sky_70638
+70639	The-life-and-adventures-of-Alexander-Selkirk-the-real-Robinson-Crusoe-b-A-narrative-founded-o__70639
+70640	Third-Base-Thatcher_70640
+70641	Three-little-maids_70641
+70642	Historical-vignettes-1st-series_70642
+70643	Coca-and-Cocaine-b-Their-history-medical-and-economic-uses-and-medicinal-preparations_70643
+70644	Caroline-the-Illustrious-vol-1-of-2-b-Queen-Consort-of-George-II-and-sometime-Queen-Regent-a-__70644
+70645	Sam-Bass_70645
+70646	Ludus-Coventriae_70646
+70647	The-belt_70647
+70648	The-course-of-creation_70648
+70649	Catalogue-of-valuable-paintings-and-water-colors-mostly-of-the-modern-Dutch-school-forming-th__70649
+70650	Les-roses-d-Ispahan-La-Perse-en-automobile-a-travers-la-Russie-et-le-Caucase_70650
+70651	Passion-fruit_70651
+70652	At-the-mountains-of-madness_70652
+70653	Rattle-of-bones_70653
+70654	Submerged-forests_70654
+70655	The-Hermit-s-Cave-b-or-Theodore-and-Jack_70655
+70656	Chronicles-and-characters-of-the-stock-exchange_70656
+70657	Prayer-and-praying-men_70657
+70658	The-life-of-Rev-Henry-Martyn-b-Written-for-the-American-Sunday-School-Union-with-some-account__70658
+70659	Beautiful-end_70659
+70660	Why-do-we-die_70660
+70661	Terre-de-Chanaan-b-roman_70661
+70662	Cultura-e-opulencia-do-Brasil-por-suas-drogas-e-minas-b-com-varias-noticias-curiosas-do-modo-__70662
+70663	Le-idee-di-una-donna_70663
+70664	O-sangue_70664
+70665	On-harelip-and-cleft-palate_70665
+70666	The-ethics-of-Hercules-b-A-study-of-man-s-body-as-the-sole-determinant-of-ethical-values_70666
+70667	The-diagnostics-and-treatment-of-tropical-diseases_70667
+70668	Needler_70668
+70669	Aesthetical-and-philosophical-essays-b-introducing-the-dissertation-on-the-connection-between__70669
+70670	Overtones-a-book-of-temperaments-b-Richard-Strauss-Parsifal-Verdi-Balzac-Flaubert-Nietzsche-a__70670
+70671	Harvard-episodes_70671
+70672	Scenas-do-seculo-18-em-Portugal_70672
+70673	Sisaiset-voimat_70673
+70674	The-glamour-of-prospecting_70674
+70675	Chicago-by-day-and-night-b-The-Pleasure-Seeker-s-Guide-to-the-Paris-of-America_70675
+70676	Lettres-sur-l-histoire-de-France_70676
+70677	An-economic-interpretation-of-the-Constitution-of-the-United-States_70677
+70678	Einstein-the-searcher-b-his-work-explained-from-dialogues-with-Einstein_70678
+70679	The-Irish-ecclesiastical-record-Volume-1-September-1865_70679
+70680	Tirol_70680
+70681	Slavery-Letters-and-Speeches_70681
+70682	Emberi-problemak_70682
+70683	The-doom-trail_70683
+70684	The-Collected-Works-of-Henrik-Ibsen-Vol-9-of-11_70684
+70685	Historical-Vignettes-2nd-Series_70685
+70686	The-Tallants-of-Barton-vol-1-of-3-b-A-tale-of-fortune-and-finance_70686
+70687	Naturgeschichte-einer-Kerze-b-Sechs-Vorlesungen-fur-die-Jugend_70687
+70688	Rajah-Brooke-b-the-englishman-as-ruler-of-an-eastern-state_70688
+70689	Slipstream-the-autobiography-of-an-air-craftsman_70689
+70690	The-trial-of-John-Jasper-for-the-murder-of-Edwin-Drood_70690
+70691	A-fighting-man-of-Mars-b-Hidden-menace-on-the-Red-Planet_70691
+70692	Naturstudien-im-Hause-b-Plaudereien-in-der-Dammerstunde_70692
+70693	The-writings-of-Origen-vol-2-of-2_70693
+70694	Boheemielamaa_70694
+70695	Bakst-b-The-story-of-Leon-Bakst-s-life_70695
+70696	Stella-Rosevelt-b-A-novel_70696
+70697	Mousey-b-or-Cousin-Robert-s-Treasure_70697
+70698	The-lonely-house_70698
+70699	Sea-life-in-Nelson-s-time_70699
+70700	Journal-of-a-tour-in-Marocco-and-the-Great-Atlas_70700
+70701	Fine-prints-b-New-and-enlarged-edition-with-fifteen-illustrations_70701
+70702	The-children-s-book-of-Christmas_70702
+70703	Christmas-builders_70703
+70704	Prayer-for-the-oppressed-b-A-premium-tract_70704
+70705	The-Collected-Works-of-Henrik-Ibsen-Vol-06-of-11_70705
+70706	The-Philistine-a-periodical-of-protest-Vol-II-No-3-February-1896_70706
+70707	The-Philistine-a-periodical-of-protest-Vol-II-No-4-March-1896_70707
+70708	The-atom-and-the-Bohr-theory-of-its-structure_70708
+70709	Victorious-life-studies_70709
+70710	Makers-of-Japan_70710
+70711	The-Philistine-a-periodical-for-curious-persons-Vol-II-No-6-May-1896_70711
+70712	Egy-haditudosito-emlekei-b-1914-november-1915-november_70712
+70713	Colloquia-sive-Confabulationes-tyronum-literatorum_70713
+70714	Demobilization-our-industrial-and-military-demobilization-after-the-armistice-1918-1920_70714
+70715	To-Mesopotamia-and-Kurdistan-in-disguise_70715
+70716	Illustrations-of-Political-Economy-Volume-1-of-9_70716
+70717	Spenser-s-Faerie-Queene-Vol-I-of-II_70717
+70718	The-inter-ocean-curiosity-shop-for-the-year-1883_70718
+70719	Memoirs-of-Arsene-Lupin_70719
+70720	Alexander-s-Magazine-Vol-1-No-1-May-15-1905_70720
+70721	The-Cairn-b-A-gathering-of-precious-stones-from-many-hands_70721
+70722	Storia-degli-Italiani-vol-9-di-15_70722
+70723	Drugs-that-enslave-b-The-opium-morphine-chloral-and-hashisch-habits_70723
+70724	Emberek-a-kovek-kozott-b-Regeny_70724
+70725	The-Republic-of-Costa-Rica_70725
+70726	The-traveller-s-oracle-or-maxims-for-locomotion-part-2-of-2-b-Containing-precepts-for-promoti__70726
+70727	Sweet-Violet-b-or-the-fairest-of-the-fair_70727
+70728	Tafilet-b-the-narrative-of-a-journey-of-exploration-in-the-Atlas-mountains-and-the-oases-of-t__70728
+70729	Vortigern-an-historical-play_70729
+70730	A-history-of-England-principally-in-the-seventeenth-century-Volume-II_70730
+70731	A-History-of-English-literature-b-A-practical-text-book_70731
+70732	The-old-vicarage-b-A-novel_70732
+70733	La-bufera_70733
+70734	The-skeleton-crew-b-or-Wildfire-Ned_70734
+70735	The-dead-towns-of-Georgia_70735
+70736	William-the-outlaw_70736
+70737	Illustrations-of-political-economy-Volume-2-of-9_70737
+70738	Dramatics-in-the-home_70738
+70739	Burning-truths-from-Billy-s-bat-b-A-graphic-description-of-the-remarkable-conversion-of-Rev-B__70739
+70740	The-Dalrymples_70740
+70741	A-decade-of-negro-extension-work-1914-1924-b-US-department-of-agriculture-miscellaneous-circu__70741
+70742	Tollinmaki_70742
+70743	Quer-durch-Afghanistan-nach-Indien_70743
+70744	The-revolt-in-Arabia_70744
+70745	Bouncing-Bet_70745
+70746	Voyage-en-Espagne-du-Chevalier-Saint-Gervais-1-de-2_70746
+70747	Voyage-en-Espagne-du-Chevalier-Saint-Gervais-2-de-2_70747
+70748	The-speaker-s-ideal-entertainments-for-home-church-and-school-b-Consisting-of-recitals-dialog__70748
+70749	Cosmic-symbolism-b-Being-a-discussion-and-exposition-of-some-recondite-and-obscure-points-in-__70749
+70750	The-Review-Vol-1-No-12-December-1911_70750
+70751	Archeological-investigations-in-New-Mexico-Colorado-and-Utah_70751
+70752	Le-goeland_70752
+70753	Le-pot-au-noir_70753
+70754	Au-Sahara-b-Illustre-d-apres-des-photographies-de-l-auteur_70754
+70755	The-Earl-s-promise-Vol-I-of-3-b-A-novel_70755
+70756	The-Earl-s-promise-Vol-II-of-3-b-A-novel_70756
+70757	The-Earl-s-promise-Vol-III-of-3-b-A-novel_70757
+70758	An-account-of-some-kjoekkenmoeddings-or-shell-heaps-in-Maine-and-Massachusetts_70758
+70759	Ye-antient-wrecke1626-b-Loss-of-the-Sparrow-Hawk-in-1626-Remarkable-preservation-and-recent-d__70759
+70760	Corpus-earthling_70760
+70761	Destiny-times-three_70761
+70762	Jesus_70762
+70763	The-poetical-works-of-Edmund-Clarence-Stedman_70763
+70764	Parnaso-portuguez-moderno-b-precedido-de-um-estudo-da-poesia-moderna-portugueza_70764
+70765	The-Kansas-University-Quarterly-b-Vol-I-No-4-April-1893_70765
+70766	A-daughter-of-the-Samurai_70766
+70767	Frederick-Law-Olmsted-b-Landscape-architect_70767
+70768	The-fields-of-France-b-with-twenty-illustrations-in-color_70768
+70769	Old-times-b-A-picture-of-social-life-at-the-end-of-the-eighteenth-century_70769
+70770	Abu-Seif-b-Aventyrsroman-fran-Roda-Havet-och-Mekka_70770
+70771	Oxford-Poetry-b-1918_70771
+70772	Suomesta-pois-b-Kuvaus-kevaalta-1899_70772
+70773	Sywanne-b-Kuvauksia-Chicagon-porssipiireista_70773
+70774	Hochtouren-im-tropischen-Amerika_70774
+70775	Lebensbilder-b-Novellensammlung_70775
+70776	The-curse-of-Clifton-b-or-the-widowed-bride_70776
+70777	Porto-Bello-gold_70777
+70778	Un-pari-de-milliardaires-et-autres-nouvelles_70778
+70779	The-highland-glen-b-Plenty-and-famine_70779
+70780	Big-lake-b-A-tragedy-in-two-parts_70780
+70781	The-saddle-boys-on-the-plains-b-or-after-a-treasure-of-gold_70781
+70782	The-United-States-Marine-Corps-in-the-World-War_70782
+70783	Uncle-Wiggily-s-funny-auto-b-How-the-skillery-skallery-alligator-was-bumped-and-Uncle-Wiggily__70783
+70784	Money-and-trade-considered-b-With-a-proposal-for-supplying-the-nation-with-money_70784
+70785	Falcon-of-Squawtooth-b-A-western-story_70785
+70786	Het-krajczar-b-Elbeszelesek_70786
+70787	Under-the-absolute-Amir_70787
+70788	The-Canary-murder-case_70788
+70789	Le-bol-de-Chine-ou-divagations-sur-les-beaux-arts_70789
+70790	The-spiritual-exercises-of-St-Ignatius-b-adapted-to-an-eight-days-retreat-and-six-triduums-in__70790
+70791	The-highest-aim-of-the-physicist_70791
+70792	Pe-belli-occhi-della-gloria-b-Scene-quasi-vere_70792
+70793	The-foundations-of-Einstein-s-theory-of-gravitation_70793
+70794	In-the-Bad-Lands_70794
+70795	A-forgotten-Prince-of-Wales_70795
+70796	An-account-of-the-manners-and-customs-of-the-modern-Egyptians_70796
+70797	Personal-hygiene-and-physical-training-for-women_70797
+70798	Kansan-keskelta-b-Kuvaus-kevaalta-1899_70798
+70799	Az-ehes-varos_70799
+70800	Novelleja_70800
+70801	L-epopee-blanche_70801
+70802	The-story-of-Eros-Psyche-retold-from-Apuleius-b-together-with-some-early-verses_70802
+70803	Darwin_70803
+70804	Lord-Lister-No-0021-Onder-de-puinhoopen-van-Messina_70804
+70805	Lord-Lister-No-0022-De-goudmaker_70805
+70806	Lord-Lister-No-0023-Het-geheim-van-den-ring_70806
+70807	Lord-Lister-No-0301-Het-einde-van-een-schrikbewind_70807
+70808	Edith-Lyle-b-A-novel_70808
+70809	Jane-Austen-and-her-works_70809
+70810	The-Terriford-mystery_70810
+70811	Gloria-b-A-novel_70811
+70812	The-dramatic-instinct-in-children_70812
+70813	Hand-book-on-cheese-making_70813
+70814	After-world-s-end_70814
+70815	Tarzan-at-the-Earth-s-core_70815
+70816	Lost-on-Venus_70816
+70817	Scream-at-midnight_70817
+70818	A-travers-les-cactus-b-Traversee-de-l-Algerie-a-bicyclette_70818
+70819	Contos_70819
+70820	Blair-of-Balaclava-b-A-hero-of-the-Light-Brigade_70820
+70821	A-Suse-b-Journal-des-fouilles-1884-1886_70821
+70822	The-Tallants-of-Barton-vol-2-of-3-A-tale-of-fortune-and-finance_70822
+70823	Retrospective-exhibition-of-important-works-of-John-Singer-Sargent-February-23rd-to-March-22n__70823
+70824	The-world-mover_70824
+70825	Les-endormies_70825
+70826	Young-Peggy-McQueen_70826
+70827	The-Tallants-of-Barton-vol-3-of-3-b-A-tale-of-fortune-and-finance_70827
+70828	The-early-Plantagenets_70828
+70829	For-the-good-of-the-team_70829
+70830	The-shadow-kingdom_70830
+70831	Great-bands-of-America_70831
+70832	The-valley-of-lost-herds_70832
+70833	A-narrative-of-travels-in-northern-Africa-in-the-years-1818-19-and-20-accompanied-by-geograph__70833
+70834	The-negro-the-southerner-s-problem_70834
+70835	Shakespeare-s-environment_70835
+70836	Too-close-fisted-and-other-stories_70836
+70837	Thrice-wedded-but-only-once-a-wife_70837
+70838	The-journal-of-Montaigne-s-travels-in-Italy-by-way-of-Switzerland-and-Germany-in-1580-and-158__70838
+70839	The-journal-of-Montaigne-s-travels-in-Italy-by-way-of-Switzerland-and-Germany-in-1580-and-158__70839
+70840	The-journal-of-Montaigne-s-travels-in-Italy-by-way-of-Switzerland-and-Germany-in-1580-and-158__70840
+70841	Robinson-Crusoe_70841
+70842	The-Champlain-tercentenary-b-Final-report-of-the-New-York-Lake-Champlain-tercentenary-commiss__70842
+70843	Hurrah-for-Peter-Perry_70843
+70844	Twilight-sleep_70844
+70845	Pilgerreise-zur-seligen-Ewigkeit_70845
+70846	Expedition-des-dix-mille_70846
+70847	The-new-spirit-in-India_70847
+70848	A-godly-medytacyon-of-the-christen-sowle-concerninge-a-loue-towardes-God-and-hys-Christe_70848
+70849	Rodeo_70849
+70850	Ptolemy-s-Tetrabiblos-b-or-Quadripartite-being-four-books-of-the-influence-of-the-stars-with-__70850
+70851	The-heiress-of-Greenhurst-b-An-autobiography_70851
+70852	The-Chinese-lantern-b-A-play_70852
+70853	Old-and-rare-Scottish-tartans-b-with-historical-introduction-and-descriptive-notices_70853
+70854	The-Countess-of-Pembroke-s-Arcadia_70854
+70855	Lilith-b-A-novel_70855
+70856	William-Tyndale_70856
+70857	Accidents-of-an-antiquary-s-life_70857
+70858	History-of-the-United-States-of-America-Volume-1-of-9-b-During-the-first-administration-of-Th__70858
+70859	Legends-of-Texas_70859
+70860	Japanse-Verzen_70860
+70861	The-doings-of-Doris_70861
+70862	Earle-Wayne-s-nobility_70862
+70863	On-the-effect-of-the-motion-of-a-body-upon-the-velocity-with-which-it-is-traversed-by-light_70863
+70864	History-of-Zionism-1600-1918-Vol-1-of-2_70864
+70865	History-of-Zionism-1600-1918-Vol-2-of-2_70865
+70866	Recollections-of-the-eventful-life-of-a-soldier_70866
+70867	Somewhere-south-in-Sonora-b-A-novel_70867
+70868	Memorias-de-un-cortesano-de-1815_70868
+70869	The-Ballantyne-Press-and-its-founders-1796-1908_70869
+70870	Marian-Grey-b-or-The-heiress-of-Redstone-Hall_70870
+70871	Picciola-b-The-prisoner-of-Fenestrella-or-captivity-captive_70871
+70872	Spears-of-destiny-b-A-story-of-the-first-capture-of-Constantinople_70872
+70873	Anthony-Cragg-s-tenant_70873
+70874	Knotting-and-splicing-ropes-and-cordage-b-With-numerous-engravings-and-diagrams_70874
+70875	Arrowsmith_70875
+70876	-n-Jodenstreek_70876
+70877	The-mystery-at-lovers-cave_70877
+70878	Maadith_70878
+70879	The-mirrors-of-Tuzun-Thune_70879
+70880	The-hoe-cake-of-Appomattox-b-Commandery-of-the-District-of-Columbia-War-Paper-93_70880
+70881	How-we-elected-Lincoln-b-personal-recollections-of-Lincoln-and-men-of-his-time_70881
+70882	The-clue-of-the-new-pin_70882
+70883	Doctor-Hathern-s-daughters-b-A-story-of-Virginia-in-four-parts_70883
+70884	French-without-a-master-b-A-farce-in-one-act_70884
+70885	Cape-Cod-b-its-natural-and-cultural-history-a-guide-to-Cape-Cod-National-Seashore-Massachuset__70885
+70886	Introducao-a-archeologia-da-peninsula-Iberica_70886
+70887	The-mothercraft-manual_70887
+70888	On-the-relative-motion-of-the-earth-and-the-luminiferous-aether_70888
+70889	Travels-of-an-Arab-merchant-in-Soudan-the-Black-Kingdoms-of-Central-Africa_70889
+70890	Sininen-silmapari_70890
+70891	0x152uvres-completes-de-Victor-Hugo-Volume-20-b-Notre-Dame-de-Paris-Tome-1_70891
+70892	Rudin_70892
+70893	The-abandoned-farm-and-Connie-s-mistake_70893
+70894	The-life-of-Adoniram-Judson_70894
+70895	Notes-on-witchcraft_70895
+70896	Arizonan-oita_70896
+70897	Avioliittoilmoitus-b-Pilakuvaus-2ssa-kohtauksessa_70897
+70898	Storia-degli-Italiani-vol-10-di-15_70898
+70899	Medusa-s-coil_70899
+70900	Le-monarque_70900
+70901	The-great-fraud-of-Ulster_70901
+70902	Many-happy-returns-of-the-day_70902
+70903	The-history-of-the-1st-Batt-Wilts-volunteers-from-1861-to-1885_70903
+70904	Partant-pour-la-Syrie_70904
+70905	Le-confessioni-di-fra-Gualberto-b-Storia-del-Secolo-XIV_70905
+70906	Sherwood-Anderson-a-bibliography_70906
+70907	Catalogue-of-the-dipterous-insects-collected-at-Singapore-and-Malacca-b-by-Mr-A-R-Wallace-wit__70907
+70908	The-undertakers-manual_70908
+70909	Pan-Germany-b-The-disease-and-cure_70909
+70910	Bruder-Leichtfu0xdf-und-Stein-am-Bein_70910
+70911	The-evolution-of-general-ideas_70911
+70912	The-curse-of-Yig_70912
+70913	Harilek-b-A-romance_70913
+70914	Caroline-the-Illustrious-vol-2-of-2-b-Queen-Consort-of-George-II-and-sometime-Queen-Regent-a-__70914
+70915	Pekan-naimapuuhat-b-Pilakuvaus_70915
+70916	Savua-b-Romaani_70916
+70917	Chercheurs-de-sources_70917
+70918	Lions-n-tigers-n-everything_70918
+70919	Miles-Murchison_70919
+70920	Whilst-father-was-fighting_70920
+70921	The-little-cap-b-Or-The-lost-heir-of-Sternfelden_70921
+70922	A-little-town-mouse_70922
+70923	An-experiment-in-gyro-hats_70923
+70924	The-adventures-of-Dora-Bell-detective_70924
+70925	Candaule_70925
+70926	Unter-Herbststernen_70926
+70927	Wanderings-in-North-Africa_70927
+70928	A-Book-of-Christmas-Verse_70928
+70929	Guatemala-b-The-land-of-the-quetzal_70929
+70930	A-memoir-of-Miss-Hannah-Adams_70930
+70931	Kuusi-pilapuhetta-huvi-iltain-ratoksi_70931
+70932	L-antica-madre_70932
+70933	Pyhan-Klaaran-kaivolla_70933
+70934	Landesverein-Sachsischer-Heimatschutz-Mitteilungen-Band-XII-Heft-10-12-b-Monatsschrift-fur-He__70934
+70935	A-Tale-of-Three-Weeks_70935
+70936	The-Wizard-s-Cave_70936
+70937	The-Photodrama-b-The-philosophy-of-its-principles-the-nature-of-its-plot-its-dramatic-constru__70937
+70938	The-day-will-come-b-A-Novel_70938
+70939	The-Jimmyjohns-and-other-stories_70939
+70940	Juttuja_70940
+70941	Meren-kirja-b-Mainetekoja-ja-suuria-saavutuksia-ulapoilla-ja-rantamilla-piirteita-merenkulun-__70941
+70942	Tish-plays-the-game_70942
+70943	Bismarck-some-secret-pages-of-his-history-Volume-II-of-3_70943
+70944	Knock-three-one-two_70944
+70945	500-Schwanke_70945
+70946	Constantinople-old-and-new_70946
+70947	A-walk-in-the-Grisons-b-Being-a-third-month-in-Switzerland_70947
+70948	Viisi-pilaa_70948
+70949	Kuningas-kivihiili_70949
+70950	In-memoriam_70950
+70951	A-text-book-on-hygiene-and-pediatrics-from-a-chiropractic-standpoint_70951
+70952	La-falce-Punizione-L-enigma_70952
+70953	The-model-prayer-b-A-series-of-expositions-on-The-Lord-s-Prayer_70953
+70954	Trois-femmes_70954
+70955	Daedalus-or-Science-and-the-future_70955
+70956	Clerambault-b-Histoire-d-une-concience-libre-pendant-la-guerre_70956
+70957	The-treasury-of-languages-b-A-rudimentary-dictionary-of-universal-philology_70957
+70958	Joking-apart_70958
+70959	Ikom-folk-stories-from-Southern-Nigeria_70959
+70960	Kuninkaan-miekkamies-b-Historiallinen-seikkailuromaani_70960
+70961	Pilaesitelmia_70961
+70962	The-sentinel-stars_70962
+70963	Heortology-b-A-history-of-the-Christian-festivals-from-their-origin-to-the-present-day_70963
+70964	The-wrong-letter_70964
+70965	The-first-French-Republic-b-A-study-of-the-origin-and-the-contents-of-the-declaration-of-the-__70965
+70966	The-Tracy-diamonds_70966
+70967	The-unhallowed-harvest_70967
+70968	The-Danube_70968
+70969	The-Dardanelles-campaign_70969
+70970	Tragedy-in-Dedham-b-The-story-of-the-Sacco-Venzetti-case_70970
+70971	The-East-I-know_70971
+70972	The-Man-killers_70972
+70973	The-agricultural-and-forest-products-of-British-West-Africa_70973
+70974	Luvattomilla-teilla-b-Matkustukset-ja-seikkailut-Tiibetissa_70974
+70975	Parturi-ja-prinssi_70975
+70976	The-Radiant-City-b-An-Allegory_70976
+70977	Good-For-Evil-b-or-Rose-Cottage_70977
+70978	The-Little-Gentleman_70978
+70979	The-riddle-of-the-rangeland_70979
+70980	Printing-and-bookbinding-for-schools_70980
+70981	The-romance-of-excavation-b-A-record-of-the-amazing-discoveries-in-Egypt-Assyria-Troy-Crete-e__70981
+70982	Vagabonds-of-the-sea-b-The-campaign-of-a-French-cruiser_70982
+70983	The-Ohio-naturalist-Vol-1-No-3-January-1901_70983
+70984	En-las-orillas-del-Sar_70984
+70985	The-life-of-John-Thompson-a-fugitive-slave-b-Containing-his-history-of-25-years-in-bondage-an__70985
+70986	Mildred-b-A-novel_70986
+70987	The-comic-history-of-the-United-States-from-a-period-prior-to-the-discovery-of-America-to-tim__70987
+70988	Neidon-ryosto-b-Kolminaytoksinen-huvinaytelma_70988
+70989	A-vol-de-velo-b-De-Paris-a-Vienne_70989
+70990	Richard-Wagner_70990
+70991	The-book-of-The-Cheese-b-Being-traits-and-stories-of-Ye-Olde-Cheshire-Cheese_70991
+70992	Escape-from-east-Tennessee-to-the-federal-lines-b-The-history-given-as-nearly-as-possible-by-__70992
+70993	L-Uomo-di-Fuoco_70993
+70994	Rogo-d-amore_70994
+70995	Lectures-pour-une-ombre_70995
+70996	The-D-Arblay-mystery_70996
+70997	Amore-ha-cent-occhi_70997
+70998	The-complete-works-of-John-Gower-volume-1-b-The-French-works_70998
+70999	The-human-species_70999
+71000	The-public-and-its-problems_71000
+71001	Mary-of-Lorraine-b-An-historical-romance_71001
+71002	Debits-and-credits_71002
+71003	Tusayan-katcinas_71003
+71004	Between-the-twilights-b-Being-studies-of-Indian-women-by-one-of-themselves_71004
+71005	Metsien-mies-b-Kolminaytoksinen-naytelma_71005
+71006	Idan-aarelta-b-Kuvia-ja-luonnoksia-Japanista_71006
+71007	Kesamatkoilla-kanootissa_71007
+71008	The-poems-of-Winthrop-Mackworth-Praed-selected_71008
+71009	The-Ainu-group-at-the-Saint-Louis-Exposition_71009
+71010	The-British-soldier-b-his-courage-and-humour_71010
+71011	A-voyage-to-Senegal-b-or-Historical-philosophical-and-political-memoirs-relative-to-the-disco__71011
+71012	At-the-Sign-of-the-Golden-Fleece-b-A-Story-of-Reformation-Days_71012
+71013	The-Turk-and-his-lost-provinces-b-Greece-Bulgaria-Servia-Bosnia_71013
+71014	Alexis-Kivi-och-hans-roman-Seitseman-veljesta_71014
+71015	Text-book-of-veterinary-medicine-Volume-1-of-5_71015
+71016	Hollywoodin-tytto_71016
+71017	Das-Gefangnis-zum-Preussischen-Adler-Eine-selbsterlebte-Schildburgerei_71017
+71018	The-natives-of-British-Central-Africa_71018
+71019	The-Summers-readers-second-reader_71019
+71020	Venezuela_71020
+71021	Battling-with-waves-and-lawyers-b-a-genuine-history-of-perils-of-the-deep-and-an-authentic-re__71021
+71022	La-Comedie-humaine-Volume-13-b-Scenes-de-la-vie-militaire-et-Scenes-de-la-vie-de-campagne_71022
+71023	En-croupe-de-Bellone_71023
+71024	The-man-she-hated-b-or-Won-by-strategy_71024
+71025	Kultaa_71025
+71026	An-enquiry-concerning-the-principles-of-natural-knowledge_71026
+71027	Il-costruttore-Solness_71027
+71028	Friendless-Felicia-b-Or-a-little-city-sparrow_71028
+71029	Jasper-s-old-shed-and-how-the-light-shone-in_71029
+71030	The-spokesman-s-secretary-b-Being-the-letters-of-Mame-to-Mom_71030
+71031	Principios-e-questoes-de-philosophia-politica-Vol-1-of-2_71031
+71032	Fanciful-tales_71032
+71033	La-bibliotheque-nationale-b-Son-origine-et-ses-accroissements-jusqu-a-nos-jours_71033
+71034	Tom-Taylor-at-West-Point-b-or-The-old-army-officer-s-secret_71034
+71035	The-Hampstead-mystery-a-novel-Volume-3-of-3_71035
+71036	John-Williams-b-or-The-sailor-boy_71036
+71037	The-gamblers_71037
+71038	Additional-mounds-of-Duval-and-of-Clay-counties-Florida-Mound-investigation-on-the-east-coast__71038
+71039	The-illustrated-story-of-evolution_71039
+71040	Elaman-pelko_71040
+71041	Sorrisi-di-gioventu-b-Ricordi-e-note_71041
+71042	Poster-advertising-b-Being-a-talk-on-the-subject-of-posting-as-an-advertising-medium-with-hel__71042
+71043	Around-the-clock-in-Europe-b-A-travel-sequence_71043
+71044	The-four-Corners-in-camp_71044
+71045	The-interpretation-of-dreams-and-moles-with-other-curious-matters-relating-to-love-and-courts__71045
+71046	Modern-English-biography-volume-2-of-4-I-Q_71046
+71047	Lewis-and-Irene_71047
+71048	Memoirs-of-the-Princesse-de-Ligne-Vol-1-of-2_71048
+71049	The-red-planet-b-a-science-fiction-novel_71049
+71050	My-dear-Cornelia_71050
+71051	Memoirs-of-the-Princesse-de-Ligne-Vol-2-of-2_71051
+71052	The-dream-snake_71052
+71053	Paraboles-et-diversions_71053
+71054	Sous-d-humbles-toits_71054
+71055	La-segunda-casaca_71055
+71056	Kun-silmat-aukenevat_71056
+71057	A-libell-of-Spanish-lies-b-found-at-the-sacke-of-Cales-discoursing-the-fight-in-the-West-Indi__71057
+71058	Holidays-at-Brighton-b-or-sea-side-amusements_71058
+71059	Constantinople_71059
+71060	The-anatomy-of-drunkenness_71060
+71061	A-wilful-ward_71061
+71062	Charmes_71062
+71063	The-Yoga-Vasishtha-Maharamayana-of-Valmiki-Vol-2-of-4-Part-1-of-2_71063
+71064	The-Yoga-Vasishtha-Maharamayana-of-Valmiki-Vol-2-of-4-Part-2-of-2_71064
+71065	The-hyena_71065
+71066	Dig-me-no-grave_71066
+71067	Mary-Rose-b-A-play-in-three-acts_71067
+71068	The-Rambler-Club-on-the-Texas-border_71068
+71069	Mere-mortals-b-Medico-historical-essays_71069
+71070	Natalika_71070
+71071	Satuja-ja-tarinoita-VII_71071
+71072	John-Baskerville-type-founder-and-printer-1706-1775_71072
+71073	The-Starvel-Hollow-tragedy-b-An-Inspector-French-case_71073
+71074	The-legend-of-Perseus-Volume-I-of-3-b-The-supernatural-birth_71074
+71075	Lord-Lister-No-0302-Chesterton-en-Chesterton_71075
+71076	Seetrien-alla-b-Romaani_71076
+71077	Suomen-rahvaan-olo-Pietarissa-b-Lukemisia-Suomen-rahvaalle-I_71077
+71078	Her-country_71078
+71079	Little-maid-Marigold_71079
+71080	The-rag-pickers-b-and-other-stories_71080
+71081	An-account-of-a-useful-discovery-to-distill-double-the-usual-quantity-of-seawater_71081
+71082	Political-and-commercial-geology-and-the-world-s-mineral-resources_71082
+71083	Anna-Hollmannin-havio-b-Kertomus_71083
+71084	Satuja-b-Lukemisia-Suomen-rahvaalle-Pietarista-II_71084
+71085	The-fire-of-Asshurbanipal_71085
+71086	The-outcast_71086
+71087	Home-education-b-Home-Education-Series-Vol-1-of-6_71087
+71088	The-chemical-nature-of-the-alpha-particles-from-radioactive-substances_71088
+71089	Tall-tales-from-Texas_71089
+71090	The-Prisoners-Memoirs-or-Dartmoor-Prison-b-Containing-a-Complete-and-Impartial-History-of-the__71090
+71091	Father-Duffy-s-story_71091
+71092	Gypsy-folk-tales_71092
+71093	Le-supplice-de-Phedre_71093
+71094	Re-creations_71094
+71095	The-Yoga-Vasishtha-Maharamayana-of-Valmiki-Vol-3-of-4-Part-1-of-2_71095
+71096	The-Nightingale_71096
+71097	The-unwelcome-child-b-Or-The-crime-of-an-undesigned-and-undesired-maternity_71097
+71098	Dorothy-Harcourt-s-secret-b-Sequel-to-A-deed-without-a-name_71098
+71099	Maggie-Lee-b-Bad-spelling-Diamonds-The-answered-prayer_71099
+71100	Memoirs-of-a-griffin-b-Or-A-cadet-s-first-year-in-India_71100
+71101	Ensimainen-rakkauteni_71101
+71102	Taiteilijan-avioliitto-b-Pariisilaisia-kuvia_71102
+71103	The-Pillars-of-Hercules-Volume-II-of-2-b-A-Narrative-of-Travels-in-Spain-and-Morocco-in-1848_71103
+71104	English-and-Scottish-Popular-Ballads-Volume-5-of-5_71104
+71105	The-story-of-a-border-city-during-the-Civil-War_71105
+71106	Social-legislation-and-social-activity-b-being-addresses-delivered-at-the-sixth-annual-meetin__71106
+71107	The-legend-of-Perseus-Volume-II-of-3-b-The-life-token_71107
+71108	Meadow-Brook_71108
+71109	Black-hound-of-death_71109
+71110	Eloge-de-la-paresse_71110
+71111	Ahasverus-b-Dramatische-episode-in-een-bedrijf_71111
+71112	Far-above-rubies-Vol-1-of-3-b-A-novel_71112
+71113	Far-above-rubies-Vol-2-of-3-b-A-novel_71113
+71114	Far-above-rubies-Vol-3-of-3-b-A-novel_71114
+71115	Storia-degli-Italiani-vol-11-di-15_71115
+71116	Practical-pathology_71116
+71117	Thunder-on-the-left_71117
+71118	Brownie-s-triumph_71118
+71119	Aunt-Caroline-s-Dixieland-recipes_71119
+71120	Meri-ja-nainen_71120
+71121	Taistelu-paalumajalla_71121
+71122	The-Book-of-Antelopes-Vol-I-of-4_71122
+71123	La-bancale_71123
+71124	The-radium-pool_71124
+71125	How-the-shortage-of-skilled-mechanics-is-being-overcome-by-training-the-unskilled_71125
+71126	Animal-portraiture_71126
+71127	The-lands-of-silence-b-A-history-of-Arctic-and-Antarctic-exploration_71127
+71128	Five-little-Peppers-in-the-Little-Brown-House_71128
+71129	Travels-in-Nubia_71129
+71130	The-life-and-times-of-the-Rev-John-Wesley-Vol-II-of-3-b-Founder-of-the-Methodists_71130
+71131	El-Gibaro-b-Cuadro-de-costumbres-de-la-isla-de-Puerto-Rico_71131
+71132	A-quiet-valley_71132
+71133	Won-at-Last-b-or-Mrs-Briscoe-s-Nephews_71133
+71134	The-book-of-antelopes-v-2-of-4_71134
+71135	An-Englishwoman-s-adventures-in-the-German-lines_71135
+71136	Isien-perinto_71136
+71137	Meren-kasvojen-edessa_71137
+71138	Pioneers-of-space-b-A-trip-to-the-Moon-Mars-and-Venus_71138
+71139	The-fearsome-touch-of-death_71139
+71140	The-Works-of-the-Reverend-George-Whitefield-Vol-II-of-6_71140
+71141	The-legend-of-Perseus-Volume-III-of-3-b-Andromeda-Medusa_71141
+71142	A-Translation-of-Glanville_71142
+71143	La-Maternelle_71143
+71144	Robert-Merry-s-Museum-Vol-VIII-July-to-December-1844_71144
+71145	The-eternal-masculine-b-Stories-of-men-and-boys_71145
+71146	Phronsie-Pepper-b-The-youngest-of-the-Five-Little-Peppers_71146
+71147	Lord-Lister-No-0024-De-heilige-schat-van-de-Siwa_71147
+71148	Lord-Lister-No-0111-De-gestolen-familiejuweelen_71148
+71149	Seikkailumatka_71149
+71150	Schools-of-Gaul-in-the-last-century-of-the-Western-Empire-b-A-study-of-pagan-and-Christian-ed__71150
+71151	Studii-sulla-letteratura-contemporanea-b-Seconda-serie_71151
+71152	A-lady-and-her-husband_71152
+71153	The-sacred-dance-b-A-study-in-comparative-folklore_71153
+71154	Lectures-on-painting-delivered-at-the-Royal-Academy-by-Henry-Fuseli-PP-b-With-additional-obse__71154
+71155	Facing-the-chair-b-Story-of-the-Americanization-of-two-foreignborn-workmen_71155
+71156	Five-years-of-youth-b-or-sense-and-sentiment_71156
+71157	Essays-in-Zen-Buddhism-b-First-series_71157
+71158	Three-textile-raw-materials-and-their-manufacture_71158
+71159	Thomas-Carlyle_71159
+71160	Homemade-candysweet-and-dandy_71160
+71161	Elamani-taipaleelta-b-Muistelmia_71161
+71162	The-complete-works-of-John-Gower-volume-2-b-The-English-works_71162
+71163	The-Parted-Family-and-Other-Poems-b-An-Offering-to-the-Afflicted_71163
+71164	Two-bad-blue-eyes_71164
+71165	Lady-Maclairn-the-Victim-of-Villany-A-Novel-Volume-II-of-4_71165
+71166	Wisdom-while-you-wait-b-Being-a-foretaste-of-the-glories-of-the-Insidecompletuar-Britanniawar__71166
+71167	Through-the-gates-of-the-silver-key_71167
+71168	Black-Canaan_71168
+71169	Illustrations-of-political-economy-Volume-3-of-9_71169
+71170	Modern-daughters-b-Conversations-with-various-American-girls-and-one-man_71170
+71171	The-Negro-in-American-Fiction_71171
+71172	0x152uvres-completes-de-Guy-de-Maupassant-volume-22_71172
+71173	Romanceiro-geral_71173
+71174	The-nugget-finders-b-A-tale-of-the-gold-fields-of-Australia_71174
+71175	Bunny-Brown-and-his-sister-Sue-on-the-rolling-ocean_71175
+71176	Ruth-Fielding-in-Alaska-b-The-girl-miners-of-snow-mountain_71176
+71177	The-trial-of-Sacco-and-Vanzetti-b-A-summary-of-the-outstanding-testimony_71177
+71178	Dora_71178
+71179	The-book-of-antelopes-vol-3-of-4_71179
+71180	The-grisly-horror_71180
+71181	Hitting-the-line_71181
+71182	Travels-in-Kordofan-b-Embracing-a-description-of-that-province-of-Egypt-and-of-some-of-the-bo__71182
+71183	Diderot_71183
+71184	A-reference-hand-book-for-nurses_71184
+71185	The-adventures-of-Uncle-Wiggily-the-bunny-rabbit-gentleman-with-the-twinkling-pink-nose_71185
+71186	The-Magazine-of-History-with-Notes-and-Queries-Vol-I-No-4-April-1905_71186
+71187	Poetry-and-the-Drama-b-Three-Plays-by-Frederic-Hebbel_71187
+71188	Rules-for-compositors-and-readers-at-the-University-Press-Oxford_71188
+71189	Satuja-ja-tarinoita-VIII_71189
+71190	Brought-out-of-peril_71190
+71191	The-celestial-worlds-discover-d-b-or-conjectures-concerning-the-inhabitants-plants-and-produc__71191
+71192	Five-thousand-pounds_71192
+71193	The-doctor-looks-at-biography-b-Psychological-studies-of-life-and-letters_71193
+71194	The-history-of-the-condition-of-women-in-various-ages-and-nations-vol-2-of-2-b-Comprising-the__71194
+71195	Tarzan-the-invincible_71195
+71196	The-book-of-Martha_71196
+71197	The-haunter-of-the-ring_71197
+71198	Il-tramonto-della-schiavitu-nel-mondo-antico_71198
+71199	Les-voix-qui-crient-dans-le-desert_71199
+71200	An-aviator-s-luck-b-or-The-Camp-Knox-plot_71200
+71201	Betty-at-St-Benedick-s-b-A-school-story-for-girls_71201
+71202	Stories-of-grit_71202
+71203	Father-Tom-and-the-Pope-b-Or-a-night-in-the-Vatican_71203
+71204	La-chanson-de-la-croisade-contre-les-Albigeois_71204
+71205	On-the-Wings-of-Fate_71205
+71206	Souvenirs-epars-d-un-ancien-cavalier_71206
+71207	Kamertjeszonde-b-Herinneringen-van-Alfred-Spier_71207
+71208	Trimardeur-roman-b-Termine-et-publie-avec-une-preface-par-Victor-Barrucand_71208
+71209	The-historians-history-of-the-world-in-twenty-five-volumes-volume-09-b-Italy_71209
+71210	Kalastajia-b-Valikoima-kertomuksia-tanskalaisten-kalastajien-elamasta_71210
+71211	Maan-puoleen-b-Runoja_71211
+71212	Hike-and-the-aeroplane_71212
+71213	Adventures-of-the-runaway-rocking-chair_71213
+71214	Your-boy-and-his-training-b-A-practical-treatise-on-boy-training_71214
+71215	Our-Davie-Pepper_71215
+71216	Harhateilla_71216
+71217	Tuokiokuvia-matkan-varrelta_71217
+71218	La-vita-nuova_71218
+71219	The-manufacture-of-earth-colours-b-With-thirty-one-illustrations_71219
+71220	Report-of-the-naval-committee-to-the-House-of-Representatives-August-1850-in-favor-of-the-est__71220
+71221	A-history-of-tithes_71221
+71222	The-crisis-vol-1-no-1-b-A-record-of-the-darker-races_71222
+71223	Religion-and-the-rise-of-capitalism-b-A-historial-study-Holland-Memorial-Lectures-1922_71223
+71224	Twenty-five-years-in-the-West_71224
+71225	Les-angoysses-douloureuses-qui-procedent-damours_71225
+71226	Woman-from-another-planet_71226
```

### Comparing `gitberg-0.8.3/gitenberg/data/gutenberg_descriptions.json` & `gitberg-0.8.4/gitenberg/data/gutenberg_descriptions.json`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/data/missing.tsv` & `gitberg-0.8.4/gitenberg/data/missing.tsv`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/dialog.py` & `gitberg-0.8.4/gitenberg/dialog.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/dialog.pyc` & `gitberg-0.8.4/gitenberg/dialog.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/fetch.py` & `gitberg-0.8.4/gitenberg/fetch.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/fetch.pyc` & `gitberg-0.8.4/gitenberg/fetch.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/library.py` & `gitberg-0.8.4/gitenberg/library.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/library.pyc` & `gitberg-0.8.4/gitenberg/library.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/local_repo.py` & `gitberg-0.8.4/gitenberg/local_repo.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/local_repo.pyc` & `gitberg-0.8.4/gitenberg/local_repo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/make.py` & `gitberg-0.8.4/gitenberg/make.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/make.pyc` & `gitberg-0.8.4/gitenberg/make.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/.DS_Store` & `gitberg-0.8.4/gitenberg/metadata/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/metadata/__pycache__/licenses.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/__pycache__/marc.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/metadata/__pycache__/marc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/metadata/__pycache__/pandata.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/metadata/__pycache__/pg_rdf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/__pycache__/utils.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/metadata/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/fileinfo.py` & `gitberg-0.8.4/gitenberg/metadata/fileinfo.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/fileinfo.pyc` & `gitberg-0.8.4/gitenberg/metadata/fileinfo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/licenses.py` & `gitberg-0.8.4/gitenberg/metadata/licenses.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/licenses.pyc` & `gitberg-0.8.4/gitenberg/metadata/licenses.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/marc.py` & `gitberg-0.8.4/gitenberg/metadata/marc.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/marc.pyc` & `gitberg-0.8.4/gitenberg/metadata/marc.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/pandata.py` & `gitberg-0.8.4/gitenberg/metadata/pandata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/pandata.pyc` & `gitberg-0.8.4/gitenberg/metadata/pandata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/pg_rdf.py` & `gitberg-0.8.4/gitenberg/metadata/pg_rdf.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/pg_rdf.pyc` & `gitberg-0.8.4/gitenberg/metadata/pg_rdf.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/utils.py` & `gitberg-0.8.4/gitenberg/metadata/utils.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/metadata/utils.pyc` & `gitberg-0.8.4/gitenberg/metadata/utils.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/pg_wikipedia.py` & `gitberg-0.8.4/gitenberg/pg_wikipedia.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/pg_wikipedia.pyc` & `gitberg-0.8.4/gitenberg/pg_wikipedia.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/push.py` & `gitberg-0.8.4/gitenberg/push.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 import semver
 
 from . import config
 from .parameters import GITHUB_ORG, ORG_HOMEPAGE
 
 logger = logging.getLogger(__name__)
 
+class RateLimitError(github3.GitHubError):
+    pass
+
 class GithubRepo():
 
     def __init__(self, book):
         self.org_name = GITHUB_ORG
         self.org_homepage = ORG_HOMEPAGE
         self.book = book
         self.repo = None
@@ -103,14 +106,16 @@
                 description=self.format_desc(),
                 homepage=self.org_homepage,
                 private=False,
                 has_issues=True,
                 has_wiki=False
             )
         except github3.GitHubError as e:
+            if '403' in str(e):
+                raise RateLimitError(e)
             logger.warning("repo already created?: %s" % e)
             self.repo = self.github.repository(self.org_name, self.book.repo_name)
 
     def update_repo(self):
         try:
             self.repo = self.github.repository(self.org_name, self.book.repo_name)
             self.repo.edit(
```

### Comparing `gitberg-0.8.3/gitenberg/push.pyc` & `gitberg-0.8.4/gitenberg/push.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/templates/.DS_Store` & `gitberg-0.8.4/gitenberg/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/templates/LICENSE` & `gitberg-0.8.4/gitenberg/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/templates/README.rst.j2` & `gitberg-0.8.4/gitenberg/templates/README.rst.j2`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/.DS_Store` & `gitberg-0.8.4/gitenberg/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_book.py` & `gitberg-0.8.4/gitenberg/tests/test_book.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_book.pyc` & `gitberg-0.8.4/gitenberg/tests/test_book.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_config.py` & `gitberg-0.8.4/gitenberg/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_config.pyc` & `gitberg-0.8.4/gitenberg/tests/test_config.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_cover.py` & `gitberg-0.8.4/gitenberg/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/.DS_Store` & `gitberg-0.8.4/gitenberg/tests/test_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/1234/1234.txt` & `gitberg-0.8.4/gitenberg/tests/test_data/1234/1234.txt`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/1234/pg1234.rdf` & `gitberg-0.8.4/gitenberg/tests/test_data/1234/pg1234.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/.DS_Store` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/.DS_Store`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/1234/pg1234.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_data/rdf_library/7/pg7.rdf` & `gitberg-0.8.4/gitenberg/tests/test_data/rdf_library/7/pg7.rdf`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_fetch.py` & `gitberg-0.8.4/gitenberg/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_fetch.pyc` & `gitberg-0.8.4/gitenberg/tests/test_fetch.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_local_repo.py` & `gitberg-0.8.4/gitenberg/tests/test_local_repo.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_local_repo.pyc` & `gitberg-0.8.4/gitenberg/tests/test_local_repo.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_make.py` & `gitberg-0.8.4/gitenberg/tests/test_make.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_make.pyc` & `gitberg-0.8.4/gitenberg/tests/test_make.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_metadata.py` & `gitberg-0.8.4/gitenberg/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_metadata.pyc` & `gitberg-0.8.4/gitenberg/tests/test_metadata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_old_metadata.py` & `gitberg-0.8.4/gitenberg/tests/test_old_metadata.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_old_metadata.pyc` & `gitberg-0.8.4/gitenberg/tests/test_old_metadata.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_push.py` & `gitberg-0.8.4/gitenberg/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/tests/test_push.pyc` & `gitberg-0.8.4/gitenberg/tests/test_push.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/catalog.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/catalog.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/catalog.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/filetypes.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/filetypes.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/filetypes.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/pg.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/pg.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/tenprintcover.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc` & `gitberg-0.8.4/gitenberg/util/__pycache__/tenprintcover.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/catalog.py` & `gitberg-0.8.4/gitenberg/util/catalog.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/catalog.pyc` & `gitberg-0.8.4/gitenberg/util/catalog.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/filetypes.py` & `gitberg-0.8.4/gitenberg/util/filetypes.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/filetypes.pyc` & `gitberg-0.8.4/gitenberg/util/filetypes.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/pg.py` & `gitberg-0.8.4/gitenberg/util/pg.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/pg.pyc` & `gitberg-0.8.4/gitenberg/util/pg.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/tenprintcover.py` & `gitberg-0.8.4/gitenberg/util/tenprintcover.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/util/tenprintcover.pyc` & `gitberg-0.8.4/gitenberg/util/tenprintcover.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/workflow.py` & `gitberg-0.8.4/gitenberg/workflow.py`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/gitenberg/workflow.pyc` & `gitberg-0.8.4/gitenberg/workflow.pyc`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/requirements.pip` & `gitberg-0.8.4/requirements.pip`

 * *Files identical despite different names*

### Comparing `gitberg-0.8.3/setup.py` & `gitberg-0.8.4/setup.py`

 * *Files identical despite different names*

