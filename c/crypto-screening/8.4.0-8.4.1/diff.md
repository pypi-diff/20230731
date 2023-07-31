# Comparing `tmp/crypto-screening-8.4.0.tar.gz` & `tmp/crypto-screening-8.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.4.0.tar", last modified: Mon Jul 31 04:59:50 2023, max compression
+gzip compressed data, was "crypto-screening-8.4.1.tar", last modified: Mon Jul 31 05:20:16 2023, max compression
```

## Comparing `crypto-screening-8.4.0.tar` & `crypto-screening-8.4.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.492114 crypto-screening-8.4.0/
--rw-rw-rw-   0        0        0      196 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-31 04:59:50.492114 crypto-screening-8.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.446585 crypto-screening-8.4.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.463605 crypto-screening-8.4.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.4.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.4.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.468112 crypto-screening-8.4.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.471119 crypto-screening-8.4.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    21265 2023-07-31 04:59:22.000000 crypto-screening-8.4.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    21473 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.480126 crypto-screening-8.4.0/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.0/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.483112 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.486143 crypto-screening-8.4.0/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.0/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.0/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.4.0/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.489114 crypto-screening-8.4.0/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.0/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.0/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.0/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.4.0/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.0/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.0/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.437615 crypto-screening-8.4.0/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.490113 crypto-screening-8.4.0/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.0/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10453 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.491113 crypto-screening-8.4.0/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.0/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.0/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.4.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.460642 crypto-screening-8.4.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 04:59:50.493112 crypto-screening-8.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-31 04:59:48.000000 crypto-screening-8.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.779783 crypto-screening-8.4.1/
+-rw-rw-rw-   0        0        0      196 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-31 05:20:16.778782 crypto-screening-8.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.736783 crypto-screening-8.4.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.753783 crypto-screening-8.4.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.4.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.4.1/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.757784 crypto-screening-8.4.1/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.1/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.1/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.759783 crypto-screening-8.4.1/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.1/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21356 2023-07-31 05:18:32.000000 crypto-screening-8.4.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21667 2023-07-31 05:19:43.000000 crypto-screening-8.4.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.768782 crypto-screening-8.4.1/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.1/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.1/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.770784 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.773782 crypto-screening-8.4.1/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.1/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.1/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.4.1/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.775782 crypto-screening-8.4.1/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.1/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.1/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.1/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.1/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.1/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.4.1/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.1/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.1/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.728858 crypto-screening-8.4.1/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.776783 crypto-screening-8.4.1/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.1/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10527 2023-07-31 05:20:01.000000 crypto-screening-8.4.1/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.777783 crypto-screening-8.4.1/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.1/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.1/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.4.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-31 05:20:16.750783 crypto-screening-8.4.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-31 05:20:16.000000 crypto-screening-8.4.1/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 05:20:16.779783 crypto-screening-8.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-31 05:20:12.000000 crypto-screening-8.4.1/setup.py
```

### Comparing `crypto-screening-8.4.0/PKG-INFO` & `crypto-screening-8.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.0
+Version: 8.4.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.0/README.md` & `crypto-screening-8.4.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/build.py` & `crypto-screening-8.4.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/assets.py` & `crypto-screening-8.4.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/exchanges.py` & `crypto-screening-8.4.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/orders.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/market/trades.py` & `crypto-screening-8.4.1/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/screeners.py` & `crypto-screening-8.4.1/crypto_screening/collect/screeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # screeners.py
 
 from typing import (
     Optional, Dict, Iterable, TypeVar,
     Set, Union, Tuple, Type, List
 )
 
+from attrs import define
+
 import pandas as pd
 
-from crypto_screening.symbols import symbol_to_pair, symbol_to_parts
+from crypto_screening.symbols import symbol_to_parts
 from crypto_screening.utils.process import string_in_values
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
 from crypto_screening.screeners import (
     BaseScreener, BaseMarketScreener, OHLCVScreener
 )
@@ -114,14 +116,15 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_screener_pairs
 
+@define(init=False, repr=False, slots=False, eq=False, unsafe_hash=True)
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
     __slots__ = "screener",
 
     def __init__(
             self,
@@ -183,15 +186,15 @@
     data = data or matching_screener_pairs(
         screeners=screeners, matches=matches,
         separator=separator, empty=empty
     )
 
     for screener1, screener2 in data:
         asset1, currency1 = symbol_to_parts(screener1.symbol)
-        asset2, currency2 = symbol_to_pair(screener2.symbol)
+        asset2, currency2 = symbol_to_parts(screener2.symbol)
 
         pairs.add(
             (
                 MarketScreenerSignature(
                     base=asset1, quote=currency1,
                     exchange=screener1.exchange,
                     screener=screener1
@@ -258,15 +261,15 @@
                 isinstance(screener, BaseScreener)
             )
         )
     }
 # end running_nonempty_screeners
 
 def running_screeners(
-    screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
+        screeners: Iterable[Union[BaseScreener, BaseMarketScreener]]
 ) -> Set[Union[BaseScreener, BaseMarketScreener]]:
     """
     Returns a list of all the live create_screeners.
 
     :param screeners: The create_screeners to search from.
 
     :return: A list the live create_screeners.
```

### Comparing `crypto-screening-8.4.0/crypto_screening/collect/symbols.py` & `crypto-screening-8.4.1/crypto_screening/collect/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # symbols.py
 
 import warnings
 from typing import (
     Optional, Dict, Iterable, Set, Union, Tuple, Any, Self
 )
 
-from represent import represent
+from attrs import define
+
+from represent import Modifiers
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.utils.process import (
     find_string_value, upper_string_values,
     mutual_string_values, string_in_values
 )
@@ -575,20 +577,23 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_symbol_pairs
 
-@represent
+@define(slots=False, init=False, repr=False, eq=False, unsafe_hash=True)
 class MarketSymbolSignature(Pair):
     """A class to represent the data for the execution of a trade."""
 
     __slots__ = "_exchange",
 
+    __modifiers__ = Modifiers(**Pair.__modifiers__)
+    __modifiers__.properties.append('exchange')
+
     def __init__(
             self,
             exchange: str,
             base: str,
             quote: str,
             separator: Optional[str] = None
     ) -> None:
```

### Comparing `crypto-screening-8.4.0/crypto_screening/dataset.py` & `crypto-screening-8.4.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/exchanges.py` & `crypto-screening-8.4.1/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/interval.py` & `crypto-screening-8.4.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/base.py` & `crypto-screening-8.4.1/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.4.1/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.4.1/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.4.1/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.4.1/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/combined.py` & `crypto-screening-8.4.1/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/container.py` & `crypto-screening-8.4.1/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/database.py` & `crypto-screening-8.4.1/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.4.1/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.4.1/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.4.1/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.4.1/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/market.py` & `crypto-screening-8.4.1/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.4.1/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.4.1/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/orders.py` & `crypto-screening-8.4.1/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/recorder.py` & `crypto-screening-8.4.1/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/trades.py` & `crypto-screening-8.4.1/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/screeners/waiting.py` & `crypto-screening-8.4.1/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.4.1/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/symbols.py` & `crypto-screening-8.4.1/crypto_screening/symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import (
     Optional, Tuple, Dict, Any, Iterable, Set, Self
 )
 
 from attrs import define
 
-from represent import represent
+from represent import represent, Modifiers
 
 __all__ = [
     "Pair",
     "symbol_to_pair",
     "symbol_to_parts",
     "pair_to_symbol",
     "parts_to_symbol",
@@ -50,14 +50,16 @@
         The asset to use to buy or sell.
 
     >>> from crypto_screening.symbols import Pair
     >>>
     >>> pair = Pair("BTC", "USD")
     """
 
+    __modifiers__ = Modifiers(properties=['base', 'quote'])
+
     __slots__ = "_base", "_quote", "separator"
 
     def __init__(self, base: str, quote: str, separator: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param base: The base asset of the trading pair.
```

### Comparing `crypto-screening-8.4.0/crypto_screening/utils/base.py` & `crypto-screening-8.4.1/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/utils/process.py` & `crypto-screening-8.4.1/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening/validate.py` & `crypto-screening-8.4.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.4.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.4.0
+Version: 8.4.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.4.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.4.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.4.0/pyproject.toml` & `crypto-screening-8.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.4.0'
+version = '8.4.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.4.0/setup.py` & `crypto-screening-8.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.4.0',
+        version='8.4.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

