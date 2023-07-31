# Comparing `tmp/wmflib-1.2.2.tar.gz` & `tmp/wmflib-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wmflib-1.2.2.tar", last modified: Thu Apr 27 16:58:20 2023, max compression
+gzip compressed data, was "wmflib-1.2.3.tar", last modified: Mon Jul 31 14:26:27 2023, max compression
```

## Comparing `wmflib-1.2.2.tar` & `wmflib-1.2.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.482677 wmflib-1.2.2/
--rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.2/.coveragerc
--rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.2/.gitignore
--rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.2/.gitreview
--rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.2/.wmfconfig
--rw-r--r--   0 riccardo   (501) staff       (20)    12694 2023-04-27 16:27:56.000000 wmflib-1.2.2/CHANGELOG.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.2/COPYRIGHT
--rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.2/LICENSE
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-04-27 16:58:20.483047 wmflib-1.2.2/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.2/README.rst
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.331493 wmflib-1.2.2/doc/
--rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/Makefile
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.351631 wmflib-1.2.2/doc/source/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.353190 wmflib-1.2.2/doc/source/_static/
--rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/_static/themes_override.css
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.385903 wmflib-1.2.2/doc/source/api/
--rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.2/doc/source/api/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.actions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.config.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.constants.rst
--rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.2/doc/source/api/wmflib.decorators.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/api/wmflib.dns.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/api/wmflib.exceptions.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.2/doc/source/api/wmflib.fileio.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.2/doc/source/api/wmflib.idm.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.interactive.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.2/doc/source/api/wmflib.irc.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.2/doc/source/api/wmflib.phabricator.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.2/doc/source/api/wmflib.prometheus.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.2/doc/source/api/wmflib.requests.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.2/doc/source/conf.py
--rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/index.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.2/doc/source/installation.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/introduction.rst
--rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.2/doc/source/release.rst
--rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.2/prospector.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)      615 2023-04-27 16:58:20.484525 wmflib-1.2.2/setup.cfg
--rw-r--r--   0 riccardo   (501) staff       (20)     2491 2023-04-27 16:27:56.000000 wmflib-1.2.2/setup.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1767 2023-04-27 16:27:56.000000 wmflib-1.2.2/tox.ini
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.422803 wmflib-1.2.2/wmflib/
--rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)     5894 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1796 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      578 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)    11577 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8282 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.2/wmflib/exceptions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2524 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     4482 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2929 2023-03-14 20:01:02.000000 wmflib-1.2.2/wmflib/irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.2/wmflib/py.typed
--rw-r--r--   0 riccardo   (501) staff       (20)     7270 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/requests.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.433593 wmflib-1.2.2/wmflib/tests/
--rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/__init__.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.313361 wmflib-1.2.2/wmflib/tests/fixtures/
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.450248 wmflib-1.2.2/wmflib/tests/fixtures/config/
--rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/config.ini
--rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/empty.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/invalid.ini
--rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/invalid.yaml
--rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/config/valid.yaml
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.452334 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/
--rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/invalid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/fixtures/phabricator/valid.conf
--rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/sphinx_checker.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.481687 wmflib-1.2.2/wmflib/tests/unit/
--rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.2/wmflib/tests/unit/__init__.py
--rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/conftest.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.2/wmflib/tests/unit/test_actions.py
--rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_config.py
--rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_constants.py
--rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_decorators.py
--rw-r--r--   0 riccardo   (501) staff       (20)     8332 2023-04-27 16:27:56.000000 wmflib-1.2.2/wmflib/tests/unit/test_dns.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.2/wmflib/tests/unit/test_fileio.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.2/wmflib/tests/unit/test_idm.py
--rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/unit/test_interactive.py
--rw-r--r--   0 riccardo   (501) staff       (20)     1660 2021-02-18 16:38:06.000000 wmflib-1.2.2/wmflib/tests/unit/test_irc.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.2/wmflib/tests/unit/test_phabricator.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.2/wmflib/tests/unit/test_prometheus.py
--rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/unit/test_requests.py
--rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.2/wmflib/tests/vulture_whitelist.py
-drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-04-27 16:58:20.429893 wmflib-1.2.2/wmflib.egg-info/
--rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/PKG-INFO
--rw-r--r--   0 riccardo   (501) staff       (20)     2083 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/SOURCES.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/dependency_links.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/not-zip-safe
--rw-r--r--   0 riccardo   (501) staff       (20)      384 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/requires.txt
--rw-r--r--   0 riccardo   (501) staff       (20)        7 2023-04-27 16:58:20.000000 wmflib-1.2.2/wmflib.egg-info/top_level.txt
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.372678 wmflib-1.2.3/
+-rw-r--r--   0 riccardo   (501) staff       (20)       42 2020-10-23 09:48:59.000000 wmflib-1.2.3/.coveragerc
+-rw-r--r--   0 riccardo   (501) staff       (20)      153 2021-02-18 16:38:06.000000 wmflib-1.2.3/.gitignore
+-rw-r--r--   0 riccardo   (501) staff       (20)       95 2020-10-23 09:48:59.000000 wmflib-1.2.3/.gitreview
+-rw-r--r--   0 riccardo   (501) staff       (20)      204 2023-02-02 15:29:16.000000 wmflib-1.2.3/.wmfconfig
+-rw-r--r--   0 riccardo   (501) staff       (20)    13063 2023-07-31 13:39:56.000000 wmflib-1.2.3/CHANGELOG.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.3/COPYRIGHT
+-rw-r--r--   0 riccardo   (501) staff       (20)    35148 2020-10-23 09:48:59.000000 wmflib-1.2.3/LICENSE
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-07-31 14:26:27.372949 wmflib-1.2.3/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)      567 2021-01-04 11:44:13.000000 wmflib-1.2.3/README.rst
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.193620 wmflib-1.2.3/doc/
+-rw-r--r--   0 riccardo   (501) staff       (20)      608 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/Makefile
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.224294 wmflib-1.2.3/doc/source/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.227519 wmflib-1.2.3/doc/source/_static/
+-rw-r--r--   0 riccardo   (501) staff       (20)      369 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/_static/themes_override.css
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.282261 wmflib-1.2.3/doc/source/api/
+-rw-r--r--   0 riccardo   (501) staff       (20)      381 2021-11-11 14:12:19.000000 wmflib-1.2.3/doc/source/api/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       48 2020-10-23 09:49:17.000000 wmflib-1.2.3/doc/source/api/wmflib.actions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2020-10-23 09:49:17.000000 wmflib-1.2.3/doc/source/api/wmflib.config.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       53 2020-12-21 17:56:39.000000 wmflib-1.2.3/doc/source/api/wmflib.constants.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)      129 2021-01-04 11:44:13.000000 wmflib-1.2.3/doc/source/api/wmflib.decorators.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/api/wmflib.dns.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/api/wmflib.exceptions.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       45 2021-02-18 16:38:06.000000 wmflib-1.2.3/doc/source/api/wmflib.fileio.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       36 2021-07-14 07:59:46.000000 wmflib-1.2.3/doc/source/api/wmflib.idm.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-12-21 17:56:39.000000 wmflib-1.2.3/doc/source/api/wmflib.interactive.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       77 2021-01-04 11:44:13.000000 wmflib-1.2.3/doc/source/api/wmflib.irc.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       60 2020-10-23 09:49:17.000000 wmflib-1.2.3/doc/source/api/wmflib.phabricator.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       57 2020-12-21 17:56:39.000000 wmflib-1.2.3/doc/source/api/wmflib.prometheus.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       51 2020-11-02 11:43:53.000000 wmflib-1.2.3/doc/source/api/wmflib.requests.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     8012 2023-02-02 15:29:16.000000 wmflib-1.2.3/doc/source/conf.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      328 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/index.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1160 2021-11-11 14:12:19.000000 wmflib-1.2.3/doc/source/installation.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       58 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/introduction.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)       61 2020-10-23 09:48:59.000000 wmflib-1.2.3/doc/source/release.rst
+-rw-r--r--   0 riccardo   (501) staff       (20)     1670 2022-03-09 19:50:10.000000 wmflib-1.2.3/prospector.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)      615 2023-07-31 14:26:27.375238 wmflib-1.2.3/setup.cfg
+-rw-r--r--   0 riccardo   (501) staff       (20)     2491 2023-07-31 13:28:37.000000 wmflib-1.2.3/setup.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1767 2023-07-31 13:28:37.000000 wmflib-1.2.3/tox.ini
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.306758 wmflib-1.2.3/wmflib/
+-rw-r--r--   0 riccardo   (501) staff       (20)      395 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     5894 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1796 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      578 2023-07-31 13:28:08.000000 wmflib-1.2.3/wmflib/constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    11577 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8282 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      532 2020-10-23 09:48:59.000000 wmflib-1.2.3/wmflib/exceptions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2524 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     4482 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    10205 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2879 2023-07-31 13:39:56.000000 wmflib-1.2.3/wmflib/irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3741 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     6563 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)       65 2021-01-04 11:44:13.000000 wmflib-1.2.3/wmflib/py.typed
+-rw-r--r--   0 riccardo   (501) staff       (20)     7270 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/requests.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.316065 wmflib-1.2.3/wmflib/tests/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1062 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/__init__.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.172101 wmflib-1.2.3/wmflib/tests/fixtures/
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.333854 wmflib-1.2.3/wmflib/tests/fixtures/config/
+-rw-r--r--   0 riccardo   (501) staff       (20)       20 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/config/config.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)        0 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/config/empty.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       28 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/config/invalid.ini
+-rw-r--r--   0 riccardo   (501) staff       (20)       41 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/config/invalid.yaml
+-rw-r--r--   0 riccardo   (501) staff       (20)       59 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/config/valid.yaml
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.336108 wmflib-1.2.3/wmflib/tests/fixtures/phabricator/
+-rw-r--r--   0 riccardo   (501) staff       (20)       82 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/phabricator/invalid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)      100 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/fixtures/phabricator/valid.conf
+-rw-r--r--   0 riccardo   (501) staff       (20)     2211 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/sphinx_checker.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.370280 wmflib-1.2.3/wmflib/tests/unit/
+-rw-r--r--   0 riccardo   (501) staff       (20)       37 2020-10-23 09:48:59.000000 wmflib-1.2.3/wmflib/tests/unit/__init__.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      421 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/unit/conftest.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3214 2020-12-21 12:21:13.000000 wmflib-1.2.3/wmflib/tests/unit/test_actions.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     2483 2020-12-21 12:21:19.000000 wmflib-1.2.3/wmflib/tests/unit/test_config.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      443 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/unit/test_constants.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     7464 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/unit/test_decorators.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     8332 2023-07-31 13:28:37.000000 wmflib-1.2.3/wmflib/tests/unit/test_dns.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     1456 2021-11-11 14:12:19.000000 wmflib-1.2.3/wmflib/tests/unit/test_fileio.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3280 2021-08-04 08:43:52.000000 wmflib-1.2.3/wmflib/tests/unit/test_idm.py
+-rw-r--r--   0 riccardo   (501) staff       (20)    12913 2023-02-02 15:29:16.000000 wmflib-1.2.3/wmflib/tests/unit/test_interactive.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3340 2023-07-31 13:39:56.000000 wmflib-1.2.3/wmflib/tests/unit/test_irc.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3362 2020-10-23 09:49:17.000000 wmflib-1.2.3/wmflib/tests/unit/test_phabricator.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3416 2022-04-04 10:17:39.000000 wmflib-1.2.3/wmflib/tests/unit/test_prometheus.py
+-rw-r--r--   0 riccardo   (501) staff       (20)     3964 2023-02-02 15:29:16.000000 wmflib-1.2.3/wmflib/tests/unit/test_requests.py
+-rw-r--r--   0 riccardo   (501) staff       (20)      474 2023-02-02 15:29:16.000000 wmflib-1.2.3/wmflib/tests/vulture_whitelist.py
+drwxr-xr-x   0 riccardo   (501) staff       (20)        0 2023-07-31 14:26:27.312956 wmflib-1.2.3/wmflib.egg-info/
+-rw-r--r--   0 riccardo   (501) staff       (20)     1817 2023-07-31 14:26:26.000000 wmflib-1.2.3/wmflib.egg-info/PKG-INFO
+-rw-r--r--   0 riccardo   (501) staff       (20)     2083 2023-07-31 14:26:27.000000 wmflib-1.2.3/wmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-07-31 14:26:26.000000 wmflib-1.2.3/wmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        1 2023-07-31 14:26:26.000000 wmflib-1.2.3/wmflib.egg-info/not-zip-safe
+-rw-r--r--   0 riccardo   (501) staff       (20)      384 2023-07-31 14:26:26.000000 wmflib-1.2.3/wmflib.egg-info/requires.txt
+-rw-r--r--   0 riccardo   (501) staff       (20)        7 2023-07-31 14:26:26.000000 wmflib-1.2.3/wmflib.egg-info/top_level.txt
```

### Comparing `wmflib-1.2.2/CHANGELOG.rst` & `wmflib-1.2.3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 wmflib Changelog
 ----------------
 
+`v1.2.3`_ (2023-07-31)
+^^^^^^^^^^^^^^^^^^^^^^
+
+Bug fixes
+"""""""""
+
+* irc: handle custom logging formatters, when set allow the message to be formatted according to them.
+
+Miscellanea
+"""""""""""
+
+* irc: refactored code and tests to simplify the code and improve readability.
+
 `v1.2.2`_ (2023-04-27)
 ^^^^^^^^^^^^^^^^^^^^^^
 
 Bug fixes
 """""""""
 
 * dns: clarify the type of the ``nameserver_addresses`` argument of the Dns class to adhere to the dnspython one.
@@ -347,7 +360,8 @@
 .. _`v1.0.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.0.2
 .. _`v1.1.0`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.0
 .. _`v1.1.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.1
 .. _`v1.1.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.1.2
 .. _`v1.2.0`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.0
 .. _`v1.2.1`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.1
 .. _`v1.2.2`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.2
+.. _`v1.2.3`: https://github.com/wikimedia/operations-software-pywmflib/releases/tag/v1.2.3
```

### Comparing `wmflib-1.2.2/LICENSE` & `wmflib-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/PKG-INFO` & `wmflib-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.2
+Version: 1.2.3
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.2/README.rst` & `wmflib-1.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/doc/Makefile` & `wmflib-1.2.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/doc/source/conf.py` & `wmflib-1.2.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/doc/source/installation.rst` & `wmflib-1.2.3/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/prospector.yaml` & `wmflib-1.2.3/prospector.yaml`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/setup.cfg` & `wmflib-1.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/setup.py` & `wmflib-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/tox.ini` & `wmflib-1.2.3/tox.ini`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/actions.py` & `wmflib-1.2.3/wmflib/actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/config.py` & `wmflib-1.2.3/wmflib/config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/constants.py` & `wmflib-1.2.3/wmflib/constants.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/decorators.py` & `wmflib-1.2.3/wmflib/decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/dns.py` & `wmflib-1.2.3/wmflib/dns.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/exceptions.py` & `wmflib-1.2.3/wmflib/exceptions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/fileio.py` & `wmflib-1.2.3/wmflib/fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/idm.py` & `wmflib-1.2.3/wmflib/idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/interactive.py` & `wmflib-1.2.3/wmflib/interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/irc.py` & `wmflib-1.2.3/wmflib/irc.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         The tcpircbot that received the message will then send it to the configured IRC channel::
 
             logmsgbot: user@host1001.domain Message
 
     """
 
-    prefix = '{s.username}@{s.hostname}'
+    command = ''
 
     def __init__(self, host: str, port: int, username: str) -> None:
         """Initialize the IRC socket handler.
 
         Arguments:
             host (str): tcpircbot hostname.
             port (int): tcpircbot listening port.
@@ -66,21 +66,20 @@
                 sock.close()
 
     def emit(self, record: logging.LogRecord) -> None:
         """According to Python logging.Handler interface.
 
         See https://docs.python.org/3/library/logging.html#handler-objects
         """
-        message = self.prefix.format(s=self) + ' ' + record.getMessage()
-        self._send_message(message, record)
+        self._send_message(f'{self.command} {self.username}@{self.hostname} {self.format(record)}'.strip(), record)
 
 
 class SALSocketHandler(SocketHandler):
     """Log handler to !log on a SAL.
 
     See the parent class for usage examples.
     """
 
     # Stashbot expects !log messages relayed by logmsgbot to have the
     # format: "!log <nick> <msg>". The <nick> is parsed out and used as
     # the label of who actually made the SAL entry.
-    prefix = '!log {s.username}@{s.hostname}'
+    command = '!log'
```

### Comparing `wmflib-1.2.2/wmflib/phabricator.py` & `wmflib-1.2.3/wmflib/phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/prometheus.py` & `wmflib-1.2.3/wmflib/prometheus.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/requests.py` & `wmflib-1.2.3/wmflib/requests.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/__init__.py` & `wmflib-1.2.3/wmflib/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/sphinx_checker.py` & `wmflib-1.2.3/wmflib/tests/sphinx_checker.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_actions.py` & `wmflib-1.2.3/wmflib/tests/unit/test_actions.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_config.py` & `wmflib-1.2.3/wmflib/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_decorators.py` & `wmflib-1.2.3/wmflib/tests/unit/test_decorators.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_dns.py` & `wmflib-1.2.3/wmflib/tests/unit/test_dns.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_fileio.py` & `wmflib-1.2.3/wmflib/tests/unit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_idm.py` & `wmflib-1.2.3/wmflib/tests/unit/test_idm.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_interactive.py` & `wmflib-1.2.3/wmflib/tests/unit/test_interactive.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_phabricator.py` & `wmflib-1.2.3/wmflib/tests/unit/test_phabricator.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_prometheus.py` & `wmflib-1.2.3/wmflib/tests/unit/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib/tests/unit/test_requests.py` & `wmflib-1.2.3/wmflib/tests/unit/test_requests.py`

 * *Files identical despite different names*

### Comparing `wmflib-1.2.2/wmflib.egg-info/PKG-INFO` & `wmflib-1.2.3/wmflib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wmflib
-Version: 1.2.2
+Version: 1.2.3
 Summary: Generic library for common tasks in the WMF production infrastructure
 Home-page: https://github.com/wikimedia/operations-software-pywmflib
 Author: Luca Toscano
 Author-email: ltoscano@wikimedia.org
 License: GPLv3+
 Keywords: wmf,automation
 Platform: GNU/Linux
```

### Comparing `wmflib-1.2.2/wmflib.egg-info/SOURCES.txt` & `wmflib-1.2.3/wmflib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

