# Comparing `tmp/cobald-0.9.1.tar.gz` & `tmp/cobald-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cobald-0.9.1.tar", last modified: Tue Oct 23 15:21:26 2018, max compression
+gzip compressed data, was "dist/cobald-0.9.2.tar", last modified: Fri Mar  8 09:47:13 2019, max compression
```

## Comparing `cobald-0.9.1.tar` & `cobald-0.9.2.tar`

### file list

```diff
@@ -1,94 +1,105 @@
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/
--rw-r--r--   0 mfischer   (501) staff       (20)       19 2018-05-15 16:32:17.000000 cobald-0.9.1/MANIFEST.in
--rw-r--r--   0 mfischer   (501) staff       (20)     2146 2018-10-23 15:21:26.000000 cobald-0.9.1/PKG-INFO
--rw-r--r--   0 mfischer   (501) staff       (20)      998 2018-07-16 10:40:16.000000 cobald-0.9.1/README.rst
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/
--rw-r--r--   0 mfischer   (501) staff       (20)      757 2018-10-23 15:19:45.000000 cobald-0.9.1/cobald/__about__.py
--rw-r--r--   0 mfischer   (501) staff       (20)       89 2018-06-15 11:38:45.000000 cobald-0.9.1/cobald/__init__.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/composite/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-05 07:54:46.000000 cobald-0.9.1/cobald/composite/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     4354 2018-08-16 14:04:34.000000 cobald-0.9.1/cobald/composite/factory.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1101 2018-06-27 09:03:27.000000 cobald-0.9.1/cobald/composite/uniform.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1133 2018-06-27 09:03:35.000000 cobald-0.9.1/cobald/composite/weighted.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/controller/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-04-13 12:43:10.000000 cobald-0.9.1/cobald/controller/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1319 2018-08-31 07:55:13.000000 cobald-0.9.1/cobald/controller/linear.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1639 2018-08-20 19:21:17.000000 cobald-0.9.1/cobald/controller/relative_supply.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1948 2018-08-17 16:21:25.000000 cobald-0.9.1/cobald/controller/switch.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/daemon/
--rw-r--r--   0 mfischer   (501) staff       (20)      105 2018-07-27 12:43:05.000000 cobald-0.9.1/cobald/daemon/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)       31 2018-05-30 16:25:00.000000 cobald-0.9.1/cobald/daemon/__main__.py
--rw-r--r--   0 mfischer   (501) staff       (20)      695 2018-05-30 16:25:00.000000 cobald-0.9.1/cobald/daemon/cli.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/daemon/config/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-30 16:25:00.000000 cobald-0.9.1/cobald/daemon/config/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     3022 2018-08-02 13:03:44.000000 cobald-0.9.1/cobald/daemon/config/mapping.py
--rw-r--r--   0 mfischer   (501) staff       (20)       77 2018-08-02 14:57:41.000000 cobald-0.9.1/cobald/daemon/config/python.py
--rw-r--r--   0 mfischer   (501) staff       (20)      748 2018-08-02 13:37:04.000000 cobald-0.9.1/cobald/daemon/config/yaml.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2204 2018-10-23 15:05:55.000000 cobald-0.9.1/cobald/daemon/core.py
--rw-r--r--   0 mfischer   (501) staff       (20)      975 2018-05-30 16:25:00.000000 cobald-0.9.1/cobald/daemon/logger.py
--rw-r--r--   0 mfischer   (501) staff       (20)     4527 2018-10-23 15:07:40.000000 cobald-0.9.1/cobald/daemon/service.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/decorator/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-05 07:54:45.000000 cobald-0.9.1/cobald/decorator/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)      835 2018-07-27 12:10:45.000000 cobald-0.9.1/cobald/decorator/buffer.py
--rw-r--r--   0 mfischer   (501) staff       (20)       50 2018-08-10 09:39:10.000000 cobald-0.9.1/cobald/decorator/coarser.py
--rw-r--r--   0 mfischer   (501) staff       (20)       50 2018-08-10 09:38:24.000000 cobald-0.9.1/cobald/decorator/limiter.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1839 2018-06-27 09:04:22.000000 cobald-0.9.1/cobald/decorator/logger.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2427 2018-08-10 12:08:05.000000 cobald-0.9.1/cobald/decorator/standardiser.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/interfaces/
--rw-r--r--   0 mfischer   (501) staff       (20)     1021 2018-06-29 10:49:43.000000 cobald-0.9.1/cobald/interfaces/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1290 2018-06-27 09:12:59.000000 cobald-0.9.1/cobald/interfaces/_composite.py
--rw-r--r--   0 mfischer   (501) staff       (20)      435 2018-08-17 12:35:19.000000 cobald-0.9.1/cobald/interfaces/_controller.py
--rw-r--r--   0 mfischer   (501) staff       (20)      930 2018-06-05 07:54:46.000000 cobald-0.9.1/cobald/interfaces/_pool.py
--rw-r--r--   0 mfischer   (501) staff       (20)      877 2018-06-27 09:12:59.000000 cobald-0.9.1/cobald/interfaces/_proxy.py
--rw-r--r--   0 mfischer   (501) staff       (20)      656 2018-06-11 17:16:41.000000 cobald-0.9.1/cobald/interfaces/actor.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/monitor/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-15 13:26:29.000000 cobald-0.9.1/cobald/monitor/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2082 2018-10-23 15:05:12.000000 cobald-0.9.1/cobald/monitor/format_json.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2960 2018-08-13 14:33:28.000000 cobald-0.9.1/cobald/monitor/format_line.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/utility/
--rw-r--r--   0 mfischer   (501) staff       (20)      748 2018-08-17 15:45:45.000000 cobald-0.9.1/cobald/utility/__init__.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald/utility/concurrent/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-10 10:28:45.000000 cobald-0.9.1/cobald/utility/concurrent/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1071 2018-07-16 21:36:11.000000 cobald-0.9.1/cobald/utility/concurrent/async_tools.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2243 2018-08-10 17:23:39.000000 cobald-0.9.1/cobald/utility/concurrent/asyncio_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1375 2018-08-10 18:08:53.000000 cobald-0.9.1/cobald/utility/concurrent/asyncio_watcher.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2754 2018-07-25 14:53:21.000000 cobald-0.9.1/cobald/utility/concurrent/base_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)     3575 2018-08-10 18:08:53.000000 cobald-0.9.1/cobald/utility/concurrent/meta_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2537 2018-07-25 14:54:23.000000 cobald-0.9.1/cobald/utility/concurrent/thread_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1215 2018-07-20 14:07:23.000000 cobald-0.9.1/cobald/utility/concurrent/trio_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)      489 2018-06-16 08:28:18.000000 cobald-0.9.1/cobald/utility/debug.py
--rw-r--r--   0 mfischer   (501) staff       (20)       24 2018-06-10 10:23:45.000000 cobald-0.9.1/cobald/utility/primitives.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/
--rw-r--r--   0 mfischer   (501) staff       (20)     2146 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/PKG-INFO
--rw-r--r--   0 mfischer   (501) staff       (20)     2242 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/SOURCES.txt
--rw-r--r--   0 mfischer   (501) staff       (20)        1 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/dependency_links.txt
--rw-r--r--   0 mfischer   (501) staff       (20)       52 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/entry_points.txt
--rw-r--r--   0 mfischer   (501) staff       (20)       85 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/requires.txt
--rw-r--r--   0 mfischer   (501) staff       (20)       20 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald.egg-info/top_level.txt
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.1/cobald_tests/__init__.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/controller/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.1/cobald_tests/controller/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     3602 2018-08-17 14:20:07.000000 cobald-0.9.1/cobald_tests/controller/test_linear.py
--rw-r--r--   0 mfischer   (501) staff       (20)      741 2018-08-17 15:53:04.000000 cobald-0.9.1/cobald_tests/controller/test_switch.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/daemon/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-07-19 09:01:20.000000 cobald-0.9.1/cobald_tests/daemon/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1473 2018-07-25 15:42:26.000000 cobald-0.9.1/cobald_tests/daemon/test_service.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/decorator/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-08-10 09:37:11.000000 cobald-0.9.1/cobald_tests/decorator/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1417 2018-08-31 08:00:45.000000 cobald-0.9.1/cobald_tests/decorator/test_logger.py
--rw-r--r--   0 mfischer   (501) staff       (20)     3335 2018-08-10 11:52:41.000000 cobald-0.9.1/cobald_tests/decorator/test_standardiser.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/mock/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.1/cobald_tests/mock/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     1051 2018-08-10 09:37:10.000000 cobald-0.9.1/cobald_tests/mock/pool.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/monitor/
--rw-r--r--   0 mfischer   (501) staff       (20)     1496 2018-10-23 15:05:12.000000 cobald-0.9.1/cobald_tests/monitor/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     3216 2018-10-23 15:05:12.000000 cobald-0.9.1/cobald_tests/monitor/test_format_json.py
--rw-r--r--   0 mfischer   (501) staff       (20)     2925 2018-08-13 14:32:27.000000 cobald-0.9.1/cobald_tests/monitor/test_format_line.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/utility/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-25 12:02:38.000000 cobald-0.9.1/cobald_tests/utility/__init__.py
-drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2018-10-23 15:21:26.000000 cobald-0.9.1/cobald_tests/utility/concurrent/
--rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-25 12:02:38.000000 cobald-0.9.1/cobald_tests/utility/concurrent/__init__.py
--rw-r--r--   0 mfischer   (501) staff       (20)     5011 2018-07-17 19:57:09.000000 cobald-0.9.1/cobald_tests/utility/concurrent/test_meta_runner.py
--rw-r--r--   0 mfischer   (501) staff       (20)       63 2018-10-23 15:21:26.000000 cobald-0.9.1/setup.cfg
--rw-r--r--   0 mfischer   (501) staff       (20)     2190 2018-08-10 15:52:38.000000 cobald-0.9.1/setup.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/
+-rw-r--r--   0 mfischer   (501) staff       (20)     1082 2018-05-18 11:33:01.000000 cobald-0.9.2/LICENSE
+-rw-r--r--   0 mfischer   (501) staff       (20)       35 2018-12-07 13:21:04.000000 cobald-0.9.2/MANIFEST.in
+-rw-r--r--   0 mfischer   (501) staff       (20)     3620 2019-03-08 09:47:13.000000 cobald-0.9.2/PKG-INFO
+-rw-r--r--   0 mfischer   (501) staff       (20)     2254 2019-03-05 09:42:54.000000 cobald-0.9.2/README.rst
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/
+-rw-r--r--   0 mfischer   (501) staff       (20)      766 2019-03-08 09:40:07.000000 cobald-0.9.2/cobald/__about__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       89 2018-06-15 11:38:45.000000 cobald-0.9.2/cobald/__init__.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/composite/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-05 07:54:46.000000 cobald-0.9.2/cobald/composite/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     4354 2019-01-31 14:13:49.000000 cobald-0.9.2/cobald/composite/factory.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1101 2019-01-31 14:13:49.000000 cobald-0.9.2/cobald/composite/uniform.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1283 2019-01-31 14:13:49.000000 cobald-0.9.2/cobald/composite/weighted.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/controller/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-04-13 12:43:10.000000 cobald-0.9.2/cobald/controller/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1319 2018-08-31 07:55:13.000000 cobald-0.9.2/cobald/controller/linear.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1696 2019-01-30 12:35:47.000000 cobald-0.9.2/cobald/controller/relative_supply.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     6595 2019-03-01 18:09:31.000000 cobald-0.9.2/cobald/controller/stepwise.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1940 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/controller/switch.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/daemon/
+-rw-r--r--   0 mfischer   (501) staff       (20)      153 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       42 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/__main__.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/daemon/config/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-30 16:25:00.000000 cobald-0.9.2/cobald/daemon/config/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3529 2019-03-08 09:34:13.000000 cobald-0.9.2/cobald/daemon/config/mapping.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       77 2018-08-02 14:57:41.000000 cobald-0.9.2/cobald/daemon/config/python.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      748 2018-08-02 13:37:04.000000 cobald-0.9.2/cobald/daemon/config/yaml.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/daemon/core/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/core/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      695 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/core/cli.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2181 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/core/config.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      975 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/core/logger.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1045 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/core/main.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1117 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/debug.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/daemon/runners/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1071 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/async_tools.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2497 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/asyncio_runner.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1377 2019-03-04 08:23:34.000000 cobald-0.9.2/cobald/daemon/runners/asyncio_watcher.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2797 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/base_runner.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      842 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/guard.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3601 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/meta_runner.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     5359 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/service.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2711 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/thread_runner.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1422 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/daemon/runners/trio_runner.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/decorator/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-05 07:54:45.000000 cobald-0.9.2/cobald/decorator/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      835 2018-07-27 12:10:45.000000 cobald-0.9.2/cobald/decorator/buffer.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       50 2018-08-10 09:39:10.000000 cobald-0.9.2/cobald/decorator/coarser.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       50 2018-08-10 09:38:24.000000 cobald-0.9.2/cobald/decorator/limiter.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1839 2018-06-27 09:04:22.000000 cobald-0.9.2/cobald/decorator/logger.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2427 2018-08-10 12:08:05.000000 cobald-0.9.2/cobald/decorator/standardiser.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/interfaces/
+-rw-r--r--   0 mfischer   (501) staff       (20)     1060 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/interfaces/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1290 2018-06-27 09:12:59.000000 cobald-0.9.2/cobald/interfaces/_composite.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      744 2019-03-01 18:09:31.000000 cobald-0.9.2/cobald/interfaces/_controller.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3623 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/interfaces/_partial.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      930 2018-06-05 07:54:46.000000 cobald-0.9.2/cobald/interfaces/_pool.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1401 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald/interfaces/_proxy.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/monitor/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-15 13:26:29.000000 cobald-0.9.2/cobald/monitor/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2082 2018-10-23 15:05:12.000000 cobald-0.9.2/cobald/monitor/format_json.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2960 2018-08-13 14:33:28.000000 cobald-0.9.2/cobald/monitor/format_line.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald/utility/
+-rw-r--r--   0 mfischer   (501) staff       (20)      748 2018-08-17 15:45:45.000000 cobald-0.9.2/cobald/utility/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       24 2018-06-10 10:23:45.000000 cobald-0.9.2/cobald/utility/primitives.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/
+-rw-r--r--   0 mfischer   (501) staff       (20)     3620 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/PKG-INFO
+-rw-r--r--   0 mfischer   (501) staff       (20)     2529 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/SOURCES.txt
+-rw-r--r--   0 mfischer   (501) staff       (20)        1 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/dependency_links.txt
+-rw-r--r--   0 mfischer   (501) staff       (20)       60 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/entry_points.txt
+-rw-r--r--   0 mfischer   (501) staff       (20)       85 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/requires.txt
+-rw-r--r--   0 mfischer   (501) staff       (20)       20 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald.egg-info/top_level.txt
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.2/cobald_tests/__init__.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/controller/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.2/cobald_tests/controller/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3602 2018-08-17 14:20:07.000000 cobald-0.9.2/cobald_tests/controller/test_linear.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1718 2019-01-30 12:35:47.000000 cobald-0.9.2/cobald_tests/controller/test_relative_supply.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1246 2019-03-01 18:09:31.000000 cobald-0.9.2/cobald_tests/controller/test_stepwise.py
+-rw-r--r--   0 mfischer   (501) staff       (20)      741 2019-01-30 12:35:47.000000 cobald-0.9.2/cobald_tests/controller/test_switch.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/daemon/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-07-19 09:01:20.000000 cobald-0.9.2/cobald_tests/daemon/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     4799 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald_tests/daemon/test_service.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/decorator/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-08-10 09:37:11.000000 cobald-0.9.2/cobald_tests/decorator/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1417 2018-08-31 08:00:45.000000 cobald-0.9.2/cobald_tests/decorator/test_logger.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3335 2018-08-10 11:52:41.000000 cobald-0.9.2/cobald_tests/decorator/test_standardiser.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/interfaces/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald_tests/interfaces/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2482 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald_tests/interfaces/test_partial.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/mock/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-05-16 13:20:45.000000 cobald-0.9.2/cobald_tests/mock/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     1051 2018-08-10 09:37:10.000000 cobald-0.9.2/cobald_tests/mock/pool.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/monitor/
+-rw-r--r--   0 mfischer   (501) staff       (20)     1496 2018-10-23 15:05:12.000000 cobald-0.9.2/cobald_tests/monitor/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     3216 2018-10-23 15:05:12.000000 cobald-0.9.2/cobald_tests/monitor/test_format_json.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     2925 2018-08-13 14:32:27.000000 cobald-0.9.2/cobald_tests/monitor/test_format_line.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/utility/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-25 12:02:38.000000 cobald-0.9.2/cobald_tests/utility/__init__.py
+drwxr-xr-x   0 mfischer   (501) staff       (20)        0 2019-03-08 09:47:13.000000 cobald-0.9.2/cobald_tests/utility/concurrent/
+-rw-r--r--   0 mfischer   (501) staff       (20)        0 2018-06-25 12:02:38.000000 cobald-0.9.2/cobald_tests/utility/concurrent/__init__.py
+-rw-r--r--   0 mfischer   (501) staff       (20)     5003 2019-03-01 12:03:50.000000 cobald-0.9.2/cobald_tests/utility/concurrent/test_meta_runner.py
+-rw-r--r--   0 mfischer   (501) staff       (20)       63 2019-03-08 09:47:13.000000 cobald-0.9.2/setup.cfg
+-rw-r--r--   0 mfischer   (501) staff       (20)     2198 2019-03-01 12:03:50.000000 cobald-0.9.2/setup.py
```

### Comparing `cobald-0.9.1/cobald/__about__.py` & `cobald-0.9.2/cobald/__about__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     :target: http://cobald.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
 This is a **draft** for a feedback based balancing system for providing opportunistic resources.
 """
 __title__ = 'cobald'
 __summary__ = 'COBalD - the Opportunistic Balancing Deamon'
-__url__ = 'https://github.com/MaineKuehn/cobald'
+__url__ = 'https://github.com/MatterMiners/cobald'
 
-__version__ = '0.9.1'
+__version__ = '0.9.2'
 __author__ = 'Eileen Kuehn, Max Fischer'
 __email__ = 'mainekuehn@gmail.com'
-__copyright__ = '2018 %s' % __author__
+__copyright__ = '2018 - 2019 %s' % __author__
 __keywords__ = 'opportunistic scheduling scheduler demand feedback-loop cobald'
```

### Comparing `cobald-0.9.1/cobald/composite/factory.py` & `cobald-0.9.2/cobald/composite/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         #: children shutting down
         self._mortuary = weakref.WeakSet()
         self.factory = factory
         self.interval = interval
 
     async def run(self):
         while True:
-            await trio.sleep_until(self.interval)
+            await trio.sleep(self.interval)
             # freeze target demand in case another thread updates us
             supply, demand = self.supply, self.demand
             if supply > demand:
                 self._shrink(target=demand)
             else:
                 self._grow(target=demand)
 
@@ -102,15 +102,15 @@
             new_child = self.factory()
             self._hatchery.add(new_child)
             assert new_child.demand > 0, 'factory must produce children with initial demand'
             missing_demand -= new_child.demand
         self._reap_children()
 
     def _reap_children(self):
-        for child in self._hatchery:
+        for child in list(self._hatchery):
             if child.demand <= 0:
                 self._release_child(child)
 
     def _release_child(self, child: Pool):
         child.demand = 0
         self._hatchery.discard(child)
         self._mortuary.add(child)
```

### Comparing `cobald-0.9.1/cobald/composite/uniform.py` & `cobald-0.9.2/cobald/composite/uniform.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/composite/weighted.py` & `cobald-0.9.2/cobald/composite/weighted.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,20 @@
     def demand(self):
         return self._demand
 
     @demand.setter
     def demand(self, value):
         self._demand = value
         total_supply = self.supply
+        child_count = len(self.children)
         for pool in self.children:
-            pool.demand = value * pool.supply / total_supply
+            try:
+                pool.demand = value * pool.supply / total_supply
+            except ZeroDivisionError:
+                pool.demand = value / child_count
 
     @property
     def supply(self):
         return sum(child.supply for child in self.children)
 
     @property
     def utilisation(self):
```

### Comparing `cobald-0.9.1/cobald/controller/linear.py` & `cobald-0.9.2/cobald/controller/linear.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/controller/relative_supply.py` & `cobald-0.9.2/cobald/controller/relative_supply.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,24 @@
     ):
         super().__init__(target=target)
         self.interval = interval
         assert low_utilisation <= high_allocation
         self.low_utilisation = low_utilisation
         self.high_allocation = high_allocation
         assert low_scale <= high_scale
+        assert low_scale < 1
+        assert high_scale > 1
         self.low_scale = low_scale
         self.high_scale = high_scale
 
     async def run(self):
         while True:
             self.regulate_demand(self.interval)
             await trio.sleep(self.interval)
 
     def regulate(self, interval):
         if self.target.utilisation < self.low_utilisation:
-            self.target.demand -= self.target.supply * self.low_scale
+            self.target.demand = self.target.supply * self.low_scale
         elif self.target.allocation > self.high_allocation:
-            self.target.demand += self.target.supply * self.high_scale
+            self.target.demand = self.target.supply * self.high_scale
         else:
             self.target.demand = self.target.supply
```

### Comparing `cobald-0.9.1/cobald/controller/switch.py` & `cobald-0.9.2/cobald/controller/switch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 import trio
 
 from ..interfaces import Pool, Controller
 from ..utility import enforce, InvariantError, pairwise
-from ..daemon.service import service
+from ..daemon import service
 
 
 @service(flavour=trio)
 class DemandSwitch(Controller):
     """
     Controller that dispatches to slaved controllers based on demand
```

### Comparing `cobald-0.9.1/cobald/daemon/cli.py` & `cobald-0.9.2/cobald/daemon/core/cli.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/daemon/config/mapping.py` & `cobald-0.9.2/cobald/daemon/config/mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import logging
 import logging.config
 import sys
 
+from typing import Any
+
 _logger = logging.getLogger(__package__)
 
 
 class ConfigurationError(Exception):
-    def __init__(self, where: str, what):
+    def __init__(self, what: Any, where: str = None):
         self.where = where
         self.what = what
         super().__init__("invalid configuration element '%s': %s" % (where, what))
 
 
 def configure_logging(logging_mapping):
     _logger.info('Configuring logging')
+    # > takes a default parameter, disable_existing_loggers, which defaults to True
+    # > for reasons of backward compatibility. This may or may not be what you want
+    # Note: this is *not* what we want, since we create several loggers in advance
+    logging_mapping['disable_existing_loggers'] = logging_mapping.get('disable_existing_loggers', False)
     logging.config.dictConfig(logging_mapping)
 
 
 class Translator(object):
     """
     Translator from a mapping to an initialised object hierarchy
     """
@@ -35,15 +41,17 @@
                 # translate bottom up - need those lists to materialize reversed and enumerate iterables
                 return list(reversed([
                     self.translate_hierarchy(item, where='%s[%s]' % (where, index))
                     for index, item in reversed(list(enumerate(structure)))
                 ]))
             else:
                 return structure
-        except ConfigurationError:
+        except ConfigurationError as err:
+            if err.where is None:
+                raise ConfigurationError(what=err.what, where=where)
             raise
         except Exception as err:
             raise ConfigurationError(where=where, what=err)
 
     def construct(self, mapping: dict, **kwargs):
         """
         Construct an object from a mapping
@@ -70,11 +78,11 @@
             except KeyError:
                 raise ModuleNotFoundError('No module named %r' % path[0])
             else:
                 for component in path[1:]:
                     try:
                         obj = getattr(obj, component)
                     except AttributeError as err:
-                        raise ConfigurationError('no such object %r: %s' % (absolute_name, err))
+                        raise ConfigurationError(what='no such object %r: %s' % (absolute_name, err))
                 return obj
         else:  # ImportError is not raised if ``absolute_name`` points to a valid module
             return sys.modules[absolute_name]
```

### Comparing `cobald-0.9.1/cobald/daemon/config/yaml.py` & `cobald-0.9.2/cobald/daemon/config/yaml.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/daemon/logger.py` & `cobald-0.9.2/cobald/daemon/core/logger.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/daemon/service.py` & `cobald-0.9.2/cobald/daemon/runners/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import trio
 import gc
 import functools
 import threading
 
 from types import ModuleType
 
-from ..utility.concurrent.meta_runner import MetaRunner
+from .meta_runner import MetaRunner
+from .guard import exclusive
 
 
 class ServiceUnit(object):
     """
     Definition for running a service
 
     :param service: the service to run
     :param flavour: runner flavour to use for running the service
     """
-    __active_units__ = weakref.WeakSet()
+    __active_units__ = weakref.WeakSet()  # type: weakref.WeakSet[ServiceUnit]
 
     def __init__(self, service, flavour):
         assert hasattr(service, 'run'), "service must implement a 'run' method"
         assert any(flavour == runner.flavour for runner in MetaRunner.runner_types), \
             "service flavour must be one of %s" % ','.join(repr(runner.flavour) for runner in MetaRunner.runner_types)
         self.service = weakref.ref(service)
         self.flavour = flavour
@@ -49,15 +50,15 @@
         return '%s(%r, flavour=%r)' % (self.__class__.__name__, self.service() or '<defunct>', self.flavour)
 
 
 def service(flavour):
     r"""
     Mark a class as implementing a Service
 
-    Each Service class must have a ``run`` method.
+    Each Service class must have a ``run`` method, which does not take any arguments.
     This method is :py:meth:`~.ServiceRunner.adopt`\ ed after the daemon starts, unless
 
     * the Service has been garbage collected, or
     * the ServiceUnit has been :py:meth:`~.ServiceUnit.cancel`\ ed.
 
     For each service instance, its :py:class:`~.ServiceUnit` is available at ``service_instance.__service_unit__``.
     """
@@ -85,49 +86,70 @@
     Runner for coroutines, subroutines and services
     """
     def __init__(self, accept_delay: float = 1):
         self._logger = logging.getLogger('cobald.runtime.daemon.services')
         self._meta_runner = MetaRunner()
         self._must_shutdown = False
         self._is_shutdown = threading.Event()
+        self.running = threading.Event()
         self.accept_delay = accept_delay
 
-    def execute(self, payload, flavour: ModuleType):
-        """Synchronously run ``payload`` and provide its output"""
-        self._meta_runner.run_payload(payload, flavour=flavour)
-
-    def adopt(self, payload, flavour: ModuleType):
-        """Concurrently run ``payload`` in the background"""
+    def execute(self, payload, *args, flavour: ModuleType, **kwargs):
+        """
+        Synchronously run ``payload`` and provide its output
+
+        If ``*args*`` and/or ``**kwargs`` are provided, pass them to ``payload`` upon execution.
+        """
+        if args or kwargs:
+            payload = functools.partial(payload, *args, **kwargs)
+        return self._meta_runner.run_payload(payload, flavour=flavour)
+
+    def adopt(self, payload, *args, flavour: ModuleType, **kwargs):
+        """
+        Concurrently run ``payload`` in the background
+
+        If ``*args*`` and/or ``**kwargs`` are provided, pass them to ``payload`` upon execution.
+        """
+        if args or kwargs:
+            payload = functools.partial(payload, *args, **kwargs)
         self._meta_runner.register_payload(payload, flavour=flavour)
 
+    @exclusive()
     def accept(self):
-        """Start accepting synchronous, asynchronous and service payloads"""
+        """
+        Start accepting synchronous, asynchronous and service payloads
+
+        Since services are globally defined, only one :py:class:`ServiceRunner`
+        may :py:meth:`accept` payloads at any time.
+        """
         if self._meta_runner:
             raise RuntimeError('payloads scheduled for %s before being started' % self)
         self._must_shutdown = False
         self._logger.info('ServiceRunner starting')
         # force collecting objects so that defunct, migrated and overwritten services are destroyed now
         gc.collect()
         self._adopt_services()
-        self.adopt(self.run, flavour=trio)
+        self.adopt(self._accept_services, flavour=trio)
         self._meta_runner.run()
 
     def shutdown(self):
         """Shutdown the accept loop and stop running payloads"""
         self._must_shutdown = True
         self._is_shutdown.wait()
         self._meta_runner.stop()
 
-    async def run(self):
+    async def _accept_services(self):
         delay, max_delay, increase = 0.0, self.accept_delay, self.accept_delay / 10
         self._is_shutdown.clear()
+        self.running.set()
         while not self._must_shutdown:
             self._adopt_services()
             await trio.sleep(delay)
             delay = min(delay + increase, max_delay)
+        self.running.clear()
         self._is_shutdown.set()
 
     def _adopt_services(self):
         for unit in ServiceUnit.units():  # type: ServiceUnit
             if unit.running:
                 continue
             unit.start(self._meta_runner)
```

### Comparing `cobald-0.9.1/cobald/decorator/buffer.py` & `cobald-0.9.2/cobald/decorator/buffer.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/decorator/logger.py` & `cobald-0.9.2/cobald/decorator/logger.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/decorator/standardiser.py` & `cobald-0.9.2/cobald/decorator/standardiser.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/interfaces/__init__.py` & `cobald-0.9.2/cobald/interfaces/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,9 +21,10 @@
     }
 
 """
 from ._composite import CompositePool
 from ._controller import Controller
 from ._pool import Pool
 from ._proxy import PoolDecorator
+from ._partial import Partial
 
-__all__ = [cls.__name__ for cls in (Pool, PoolDecorator, Controller, CompositePool)]
+__all__ = [cls.__name__ for cls in (Pool, PoolDecorator, Controller, CompositePool, Partial)]
```

### Comparing `cobald-0.9.1/cobald/interfaces/_composite.py` & `cobald-0.9.2/cobald/interfaces/_composite.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/interfaces/_pool.py` & `cobald-0.9.2/cobald/interfaces/_pool.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/interfaces/_proxy.py` & `cobald-0.9.2/cobald/interfaces/_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,39 @@
 from ._pool import Pool
+from typing import TypeVar, Type
+
+
+from ._partial import Partial
+
+
+C = TypeVar('C', bound='PoolDecorator')
 
 
 class PoolDecorator(Pool):
     """
     Decorator modifying how a pool provides resources
+
+    :param target: the resource pool for which demand is adjusted
     """
     def __init__(self, target: Pool):
         self.target = target
 
+    @classmethod
+    def s(cls: Type[C], *args, **kwargs) -> Partial[C]:
+        """
+        Create an unbound prototype of this class, partially applying arguments
+
+        .. code:: python
+
+            decorator = Buffer.s(window=20)
+
+            pipeline = controller >> decorator >> pool
+        """
+        return Partial(cls, *args, **kwargs)
+
     @property
     def supply(self):
         """The volume of resources that is provided by this site"""
         return self.target.supply
 
     @property
     def demand(self):
```

### Comparing `cobald-0.9.1/cobald/monitor/format_json.py` & `cobald-0.9.2/cobald/monitor/format_json.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/monitor/format_line.py` & `cobald-0.9.2/cobald/monitor/format_line.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/utility/__init__.py` & `cobald-0.9.2/cobald/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/utility/concurrent/async_tools.py` & `cobald-0.9.2/cobald/daemon/runners/async_tools.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald/utility/concurrent/asyncio_runner.py` & `cobald-0.9.2/cobald/daemon/runners/asyncio_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from functools import partial
 
 from .base_runner import BaseRunner
 from .async_tools import raise_return, AsyncExecution
 
 
 class AsyncioRunner(BaseRunner):
+    """Runner for coroutines with :py:mod:`asyncio`"""
     flavour = asyncio
 
     def __init__(self):
         super().__init__()
         self.event_loop = asyncio.new_event_loop()
         self._tasks = set()
 
@@ -19,51 +20,56 @@
     def run_payload(self, payload):
         execution = AsyncExecution(payload)
         super().register_payload(execution.coroutine)
         return execution.wait()
 
     def _run(self):
         asyncio.set_event_loop(self.event_loop)
-        self.event_loop.run_until_complete(self.await_all())
+        self.event_loop.run_until_complete(self._run_payloads())
 
-    async def await_all(self):
+    async def _run_payloads(self):
+        """Async component of _run"""
         delay = 0.0
         try:
             while self.running.is_set():
-                await self._start_outstanding()
-                await self._manage_running()
+                await self._start_payloads()
+                await self._reap_payloads()
                 await asyncio.sleep(delay)
                 delay = min(delay + 0.1, 1.0)
         except Exception:
-            await self._cancel_running()
+            await self._cancel_payloads()
             raise
 
-    async def _start_outstanding(self):
+    async def _start_payloads(self):
+        """Start all queued payloads"""
         with self._lock:
             for coroutine in self._payloads:
                 task = self.event_loop.create_task(coroutine())
                 self._tasks.add(task)
             self._payloads.clear()
         await asyncio.sleep(0)
 
-    async def _manage_running(self):
+    async def _reap_payloads(self):
+        """Clean up all finished payloads"""
         for task in self._tasks.copy():
             if task.done():
                 self._tasks.remove(task)
                 if task.exception() is not None:
                     raise task.exception()
         await asyncio.sleep(0)
 
-    async def _cancel_running(self):
+    async def _cancel_payloads(self):
+        """Cancel all remaining payloads"""
         for task in self._tasks:
             task.cancel()
             await asyncio.sleep(0)
         for task in self._tasks:
             while not task.done():
                 await asyncio.sleep(0.1)
+                task.cancel()
 
     def stop(self):
         if not self.running.wait(0.2):
             return
         self._logger.debug('runner disabled: %s', self)
         with self._lock:
             self.running.clear()
```

### Comparing `cobald-0.9.1/cobald/utility/concurrent/asyncio_watcher.py` & `cobald-0.9.2/cobald/daemon/runners/asyncio_watcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
     Create an ``asyncio`` event loop running in the main thread and watching runners
 
     Using ``asyncio`` to handle suprocesses requires a specific loop type to run in the main thread.
     This function sets up and runs the correct loop in a portable way.
     In addition, it runs a single :py:class:`~.BaseRunner` until completion or failure.
 
-    .. seealso:: The `issue #8 <https://github.com/MaineKuehn/cobald/issues/8>`_ for details.
+    .. seealso:: The `issue #8 <https://github.com/MatterMiners/cobald/issues/8>`_ for details.
     """
     assert threading.current_thread() == threading.main_thread(), 'only main thread can accept asyncio subprocesses'
     if sys.platform == 'win32':
         event_loop = asyncio.ProactorEventLoop()
         asyncio.set_event_loop(event_loop)
     else:
         event_loop = asyncio.get_event_loop()
```

### Comparing `cobald-0.9.1/cobald/utility/concurrent/base_runner.py` & `cobald-0.9.2/cobald/daemon/runners/base_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 import threading
+from typing import Any
 
-from ...utility.debug import NameRepr
+from cobald.daemon.debug import NameRepr
 
 
 class BaseRunner(object):
-    flavour = None
+    flavour = None  # type: Any
 
     def __init__(self):
         self._logger = logging.getLogger('cobald.runtime.runner.%s' % NameRepr(self.flavour))
         self._payloads = []
         self._lock = threading.Lock()
         #: signal that runner should keep in running
         self.running = threading.Event()
@@ -52,15 +53,15 @@
         try:
             with self._lock:
                 assert not self.running.is_set() and self._stopped.is_set(), 'cannot re-run: %s' % self
                 self.running.set()
                 self._stopped.clear()
             self._run()
         except Exception:
-            self._logger.error('runner aborted: %s', self)
+            self._logger.exception('runner aborted: %s', self)
             raise
         else:
             self._logger.info('runner stopped: %s', self)
         finally:
             with self._lock:
                 self.running.clear()
                 self._stopped.set()
```

### Comparing `cobald-0.9.1/cobald/utility/concurrent/meta_runner.py` & `cobald-0.9.2/cobald/daemon/runners/meta_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .base_runner import BaseRunner
 from .trio_runner import TrioRunner
 from .asyncio_runner import AsyncioRunner
 from .thread_runner import ThreadRunner
 from .asyncio_watcher import asyncio_main_run
 
 
-from ...utility.debug import NameRepr
+from cobald.daemon.debug import NameRepr
 
 
 class MetaRunner(object):
     """
     Unified interface to schedule subroutines and coroutines for concurrent execution
     """
     runner_types = (TrioRunner, AsyncioRunner, ThreadRunner)
@@ -39,30 +39,30 @@
             self.runners[flavour].register_payload(payload)
 
     def run_payload(self, payload, *, flavour: ModuleType):
         """Execute one payload after its runner is started and return its output"""
         return self.runners[flavour].run_payload(payload)
 
     def run(self):
-        """Run all runners until completion"""
+        """Run all runners, blocking until completion or error"""
         self._logger.info('starting all runners')
         try:
             with self._lock:
                 assert not self.running.set(), 'cannot re-run: %s' % self
                 self.running.set()
             thread_runner = self.runners[threading]
             for runner in self.runners.values():
                 if runner is not thread_runner:
                     thread_runner.register_payload(runner.run)
             if threading.current_thread() == threading.main_thread():
                 asyncio_main_run(root_runner=thread_runner)
             else:
                 thread_runner.run()
         except Exception as err:
-            self._logger.error('runner terminated: %s', err)
+            self._logger.exception('runner terminated: %s', err)
             raise RuntimeError from err
         finally:
             self._stop_runners()
             self._logger.info('stopped all runners')
             self.running.clear()
 
     def stop(self):
```

### Comparing `cobald-0.9.1/cobald/utility/concurrent/thread_runner.py` & `cobald-0.9.2/cobald/daemon/runners/thread_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,25 +49,31 @@
         # instead of running payload in a thread and blocking this one,
         # we just block this thread by running payload directly
         return payload()
 
     def _run(self):
         delay = 0.0
         while self.running.is_set():
-            self._start_outstanding()
-            for thread in self._threads.copy():
-                if thread.join(timeout=0):
-                    self._threads.remove(thread)
-                    self._logger.debug('reaped thread %s', thread)
+            self._start_payloads()
+            self._reap_payloads()
             time.sleep(delay)
             delay = min(delay + 0.1, 1.0)
 
-    def _start_outstanding(self):
+    def _start_payloads(self):
+        """Start all queued payloads"""
         with self._lock:
             payloads = self._payloads.copy()
             self._payloads.clear()
         for subroutine in payloads:
             thread = CapturingThread(target=subroutine)
             thread.start()
             self._threads.add(thread)
             self._logger.debug('booted thread %s', thread)
         time.sleep(0)
+
+    def _reap_payloads(self):
+        """Clean up all finished payloads"""
+        for thread in self._threads.copy():
+            # CapturingThread.join will throw
+            if thread.join(timeout=0):
+                self._threads.remove(thread)
+                self._logger.debug('reaped thread %s', thread)
```

### Comparing `cobald-0.9.1/cobald/utility/concurrent/trio_runner.py` & `cobald-0.9.2/cobald/daemon/runners/trio_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 from .base_runner import BaseRunner
 from .async_tools import raise_return, AsyncExecution
 
 
 class TrioRunner(BaseRunner):
-    """Runner for coroutines of :py:mod:`trio`"""
+    """Runner for coroutines with :py:mod:`trio`"""
     flavour = trio
 
     def __init__(self):
         self._nursery = None
         super().__init__()
 
     def register_payload(self, payload):
@@ -19,24 +19,28 @@
 
     def run_payload(self, payload):
         execution = AsyncExecution(payload)
         super().register_payload(execution.coroutine)
         return execution.wait()
 
     def _run(self):
-        return trio.run(self.await_all)
+        return trio.run(self._await_all)
 
-    async def await_all(self):
+    async def _await_all(self):
+        """Async component of _run"""
         delay = 0.0
+        # we run a top-level nursery that automatically reaps/cancels for us
         async with trio.open_nursery() as nursery:
             while self.running.is_set():
-                await self._start_outstanding(nursery=nursery)
+                await self._start_payloads(nursery=nursery)
                 await trio.sleep(delay)
                 delay = min(delay + 0.1, 1.0)
+            # cancel the scope to cancel all payloads
             nursery.cancel_scope.cancel()
 
-    async def _start_outstanding(self, nursery):
+    async def _start_payloads(self, nursery):
+        """Start all queued payloads"""
         with self._lock:
             for coroutine in self._payloads:
                 nursery.start_soon(coroutine)
             self._payloads.clear()
         await trio.sleep(0)
```

### Comparing `cobald-0.9.1/cobald.egg-info/SOURCES.txt` & `cobald-0.9.2/cobald.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 cobald/__about__.py
 cobald/__init__.py
 cobald.egg-info/PKG-INFO
@@ -13,60 +14,68 @@
 cobald/composite/__init__.py
 cobald/composite/factory.py
 cobald/composite/uniform.py
 cobald/composite/weighted.py
 cobald/controller/__init__.py
 cobald/controller/linear.py
 cobald/controller/relative_supply.py
+cobald/controller/stepwise.py
 cobald/controller/switch.py
 cobald/daemon/__init__.py
 cobald/daemon/__main__.py
-cobald/daemon/cli.py
-cobald/daemon/core.py
-cobald/daemon/logger.py
-cobald/daemon/service.py
+cobald/daemon/debug.py
 cobald/daemon/config/__init__.py
 cobald/daemon/config/mapping.py
 cobald/daemon/config/python.py
 cobald/daemon/config/yaml.py
+cobald/daemon/core/__init__.py
+cobald/daemon/core/cli.py
+cobald/daemon/core/config.py
+cobald/daemon/core/logger.py
+cobald/daemon/core/main.py
+cobald/daemon/runners/__init__.py
+cobald/daemon/runners/async_tools.py
+cobald/daemon/runners/asyncio_runner.py
+cobald/daemon/runners/asyncio_watcher.py
+cobald/daemon/runners/base_runner.py
+cobald/daemon/runners/guard.py
+cobald/daemon/runners/meta_runner.py
+cobald/daemon/runners/service.py
+cobald/daemon/runners/thread_runner.py
+cobald/daemon/runners/trio_runner.py
 cobald/decorator/__init__.py
 cobald/decorator/buffer.py
 cobald/decorator/coarser.py
 cobald/decorator/limiter.py
 cobald/decorator/logger.py
 cobald/decorator/standardiser.py
 cobald/interfaces/__init__.py
 cobald/interfaces/_composite.py
 cobald/interfaces/_controller.py
+cobald/interfaces/_partial.py
 cobald/interfaces/_pool.py
 cobald/interfaces/_proxy.py
-cobald/interfaces/actor.py
 cobald/monitor/__init__.py
 cobald/monitor/format_json.py
 cobald/monitor/format_line.py
 cobald/utility/__init__.py
-cobald/utility/debug.py
 cobald/utility/primitives.py
-cobald/utility/concurrent/__init__.py
-cobald/utility/concurrent/async_tools.py
-cobald/utility/concurrent/asyncio_runner.py
-cobald/utility/concurrent/asyncio_watcher.py
-cobald/utility/concurrent/base_runner.py
-cobald/utility/concurrent/meta_runner.py
-cobald/utility/concurrent/thread_runner.py
-cobald/utility/concurrent/trio_runner.py
 cobald_tests/__init__.py
 cobald_tests/controller/__init__.py
 cobald_tests/controller/test_linear.py
+cobald_tests/controller/test_relative_supply.py
+cobald_tests/controller/test_stepwise.py
 cobald_tests/controller/test_switch.py
 cobald_tests/daemon/__init__.py
 cobald_tests/daemon/test_service.py
 cobald_tests/decorator/__init__.py
 cobald_tests/decorator/test_logger.py
 cobald_tests/decorator/test_standardiser.py
+cobald_tests/interfaces/__init__.py
+cobald_tests/interfaces/test_partial.py
 cobald_tests/mock/__init__.py
 cobald_tests/mock/pool.py
 cobald_tests/monitor/__init__.py
 cobald_tests/monitor/test_format_json.py
 cobald_tests/monitor/test_format_line.py
 cobald_tests/utility/__init__.py
 cobald_tests/utility/concurrent/__init__.py
```

### Comparing `cobald-0.9.1/cobald_tests/controller/test_linear.py` & `cobald-0.9.2/cobald_tests/controller/test_linear.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/decorator/test_logger.py` & `cobald-0.9.2/cobald_tests/decorator/test_logger.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/decorator/test_standardiser.py` & `cobald-0.9.2/cobald_tests/decorator/test_standardiser.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/mock/pool.py` & `cobald-0.9.2/cobald_tests/mock/pool.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/monitor/__init__.py` & `cobald-0.9.2/cobald_tests/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/monitor/test_format_json.py` & `cobald-0.9.2/cobald_tests/monitor/test_format_json.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/monitor/test_format_line.py` & `cobald-0.9.2/cobald_tests/monitor/test_format_line.py`

 * *Files identical despite different names*

### Comparing `cobald-0.9.1/cobald_tests/utility/concurrent/test_meta_runner.py` & `cobald-0.9.2/cobald_tests/utility/concurrent/test_meta_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import threading
 import pytest
 import time
 import asyncio
 
 import trio
 
-from cobald.utility.concurrent.base_runner import OrphanedReturn
-from cobald.utility.concurrent.meta_runner import MetaRunner
+from cobald.daemon.runners.base_runner import OrphanedReturn
+from cobald.daemon.runners.meta_runner import MetaRunner
 
 
 class TerminateRunner(Exception):
     pass
 
 
 def run_in_thread(payload, name, daemon=True):
```

### Comparing `cobald-0.9.1/setup.py` & `cobald-0.9.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         long_description=long_description.strip(),
         author=package_about['__author__'],
         author_email=package_about['__email__'],
         url=package_about['__url__'],
         packages=find_packages(),
         entry_points={
             'console_scripts': [
-                'cobald = cobald.daemon.core:main',
+                'cobald = cobald.daemon.core.main:cli_run',
             ],
         },
         # dependencies
         install_requires=[
             'typing',
             'pyyaml',
             'trio~=0.4.0',
```

