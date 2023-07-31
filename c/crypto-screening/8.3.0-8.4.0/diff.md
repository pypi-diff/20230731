# Comparing `tmp/crypto-screening-8.3.0.tar.gz` & `tmp/crypto-screening-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.3.0.tar", last modified: Mon Jul 31 04:42:36 2023, max compression
+gzip compressed data, was "crypto-screening-8.4.0.tar", last modified: Mon Jul 31 04:59:50 2023, max compression
```

## Comparing `crypto-screening-8.3.0.tar` & `crypto-screening-8.4.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/
--rw-rw-rw-   0        0        0      196 2023-07-31 04:42:34.000000 crypto-screening-8.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.3.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.3.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.811425 crypto-screening-8.3.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.837430 crypto-screening-8.3.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.3.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.3.0/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.864736 crypto-screening-8.3.0/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.3.0/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.3.0/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.886737 crypto-screening-8.3.0/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    21234 2023-07-31 04:41:38.000000 crypto-screening-8.3.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    21503 2023-07-31 04:41:38.000000 crypto-screening-8.3.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.3.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.3.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.3.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.954345 crypto-screening-8.3.0/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.3.0/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23844 2023-07-29 11:01:44.000000 crypto-screening-8.3.0/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.977342 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.997343 crypto-screening-8.3.0/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.3.0/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.3.0/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.3.0/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.018342 crypto-screening-8.3.0/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.3.0/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.3.0/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.3.0/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.3.0/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.3.0/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.3.0/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.777336 crypto-screening-8.3.0/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.023343 crypto-screening-8.3.0/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.3.0/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10390 2023-07-29 10:33:38.000000 crypto-screening-8.3.0/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.035498 crypto-screening-8.3.0/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.3.0/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.3.0/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.3.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.825462 crypto-screening-8.3.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-31 04:42:34.000000 crypto-screening-8.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.3.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-31 04:42:30.000000 crypto-screening-8.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.492114 crypto-screening-8.4.0/
+-rw-rw-rw-   0        0        0      196 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-31 04:59:50.492114 crypto-screening-8.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.4.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.4.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.446585 crypto-screening-8.4.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.463605 crypto-screening-8.4.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.4.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.4.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.468112 crypto-screening-8.4.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.4.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.4.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.471119 crypto-screening-8.4.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.4.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21265 2023-07-31 04:59:22.000000 crypto-screening-8.4.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21473 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.4.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.4.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.4.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.480126 crypto-screening-8.4.0/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.4.0/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    24218 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.483112 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.486143 crypto-screening-8.4.0/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.4.0/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.4.0/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.4.0/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.489114 crypto-screening-8.4.0/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.4.0/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.4.0/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.4.0/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.4.0/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.4.0/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.4.0/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.4.0/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.4.0/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.437615 crypto-screening-8.4.0/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.490113 crypto-screening-8.4.0/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.4.0/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10453 2023-07-31 04:58:29.000000 crypto-screening-8.4.0/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.491113 crypto-screening-8.4.0/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.4.0/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.4.0/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.4.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:59:50.460642 crypto-screening-8.4.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-31 04:59:50.000000 crypto-screening-8.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.4.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:59:50.493112 crypto-screening-8.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-31 04:59:48.000000 crypto-screening-8.4.0/setup.py
```

### Comparing `crypto-screening-8.3.0/PKG-INFO` & `crypto-screening-8.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.3.0
+Version: 8.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.3.0/README.md` & `crypto-screening-8.4.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/build.py` & `crypto-screening-8.4.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/assets.py` & `crypto-screening-8.4.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/exchanges.py` & `crypto-screening-8.4.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/orders.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/state/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/state/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/state/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/market/trades.py` & `crypto-screening-8.4.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/screeners.py` & `crypto-screening-8.4.0/crypto_screening/collect/screeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,16 @@
 
     return set(pairs)
 # end matching_screener_pairs
 
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
+    __slots__ = "screener",
+
     def __init__(
             self,
             exchange: str,
             base: str,
             quote: str,
             screener: Optional[BaseScreener] = None,
             separator: Optional[str] = None
```

### Comparing `crypto-screening-8.3.0/crypto_screening/collect/symbols.py` & `crypto-screening-8.4.0/crypto_screening/collect/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # symbols.py
 
 import warnings
 from typing import (
-    Optional, Dict, Iterable, Set, Union, Tuple, Any
+    Optional, Dict, Iterable, Set, Union, Tuple, Any, Self
 )
 
 from represent import represent
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.utils.process import (
     find_string_value, upper_string_values,
     mutual_string_values, string_in_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
-    symbol_to_parts, adjust_symbol, Separator, parts_to_symbol
+    symbol_to_parts, adjust_symbol, Separator, Pair
 )
 from crypto_screening.validate import validate_exchange
 from crypto_screening.collect.exchanges import exchanges_data
 
 __all__ = [
     "exchanges_symbols",
     "mutual_exchanges_symbols",
@@ -576,49 +576,40 @@
         # end for
     # end for
 
     return set(pairs)
 # end matching_symbol_pairs
 
 @represent
-class MarketSymbolSignature:
+class MarketSymbolSignature(Pair):
     """A class to represent the data for the execution of a trade."""
 
+    __slots__ = "_exchange",
+
     def __init__(
             self,
             exchange: str,
             base: str,
             quote: str,
             separator: Optional[str] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param exchange: The exchange name.
         :param base: The base asset.
         :param quote: The quote asset.
+        :param separator: The symbol separator.
         """
 
-        self._exchange = exchange
-        self._base = base
-        self._quote = quote
+        super().__init__(base=base, quote=quote, separator=separator)
 
-        self.separator = separator
+        self._exchange = exchange
     # end __init__
 
-    def __hash__(self) -> int:
-        """
-        Returns the hash of the object.
-
-        :return: The hash.
-        """
-
-        return id(self)
-    # end __hash__
-
     def __eq__(self, other: Any) -> bool:
         """
         Checks if the signatures are equal.
 
         :param other: The signature to compare.
 
         :return: The equality value.
@@ -644,48 +635,45 @@
 
         :return: The exchange name.
         """
 
         return self._exchange
     # end exchange
 
-    @property
-    def symbol(self) -> str:
-        """
-        Returns the property value.
-
-        :return: The symbol.
+    @classmethod
+    def load(cls, data: Dict[str, str]) -> Self:
         """
+        Creates a pair of assets from the data.
 
-        return parts_to_symbol(
-            self._base, self._quote, separator=self.separator
-        )
-    # end symbol
-
-    @property
-    def base(self) -> str:
-        """
-        Returns the property value.
+        :param data: The pair data.
 
-        :return: The base name.
+        :return: The pair object.
         """
 
-        return self._base
-    # end base
+        return cls(
+            exchange=data['exchange'],
+            base=data['base'],
+            quote=data['quote'],
+            separator=data.get('separator', None)
+        )
+    # end load
 
-    @property
-    def quote(self) -> str:
+    def json(self) -> Dict[str, str]:
         """
-        Returns the property value.
+        Converts the data into a json format.
 
-        :return: The base name.
+        :return: The chain of assets.
         """
 
-        return self._quote
-    # end quote
+        return {
+            'exchange': self.exchange,
+            'base': self.base,
+            'quote': self.quote
+        }
+    # end json
 # end MarketPairSignature
 
 def matching_symbol_signatures(
         pairs: Optional[ExchangeSymbolPairs] = None,
         data: Optional[Dict[str, Iterable[str]]] = None,
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
```

### Comparing `crypto-screening-8.3.0/crypto_screening/dataset.py` & `crypto-screening-8.4.0/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/exchanges.py` & `crypto-screening-8.4.0/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/interval.py` & `crypto-screening-8.4.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/base.py` & `crypto-screening-8.4.0/crypto_screening/screeners/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,26 +56,25 @@
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data.
     """
 
-    __modifiers__ = Modifiers()
-    __modifiers__.hidden.append("market")
+    __modifiers__ = Modifiers(hidden=["market"])
 
     MINIMUM_DELAY = 1
 
     NAME: Optional[str] = "BASE"
     COLUMNS: Iterable[str] = []
 
     SCREENER_NAME_TYPE_MATCHES: Dict[str, Any] = {}
     SCREENER_TYPE_NAME_MATCHES: Dict[Any, str] = {}
 
-    __slots__ = "symbol", "exchange", "market"
+    __slots__ = "_symbol", "_exchange", "market"
 
     def __init__(
             self,
             symbol: str,
             exchange: str,
             location: Optional[str] = None,
             cancel: Optional[Union[float, dt.timedelta]] = None,
@@ -101,24 +100,46 @@
         # end if
 
         super().__init__(location=location, cancel=cancel, delay=delay)
 
         self.SCREENER_NAME_TYPE_MATCHES.setdefault(self.NAME, type(self))
         self.SCREENER_TYPE_NAME_MATCHES.setdefault(type(self), self.NAME)
 
-        self.exchange = self.validate_exchange(exchange=exchange)
-        self.symbol = self.validate_symbol(exchange=self.exchange, symbol=symbol)
+        self._exchange = self.validate_exchange(exchange=exchange)
+        self._symbol = self.validate_symbol(exchange=self._exchange, symbol=symbol)
 
         if market is None:
             market = create_dataset(self.COLUMNS)
         # end if
 
         self.market = market
     # end __init__
 
+    @property
+    def symbol(self) -> str:
+        """
+        Returns the property value.
+
+        :return: The symbol.
+        """
+
+        return self._symbol
+    # end symbol
+
+    @property
+    def exchange(self) -> str:
+        """
+        Returns the property value.
+
+        :return: The exchange name.
+        """
+
+        return self._exchange
+    # end exchange
+
     def await_initialization(
             self,
             stop: Optional[Union[bool, int]] = False,
             delay: Optional[Union[float, dt.timedelta]] = None,
             cancel: Optional[Union[float, dt.timedelta, dt.datetime]] = None
     ) -> WaitingState[BaseScreenerProtocol]:
         """
```

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.4.0/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.4.0/crypto_screening/screeners/collectors/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.4.0/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.4.0/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/combined.py` & `crypto-screening-8.4.0/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/container.py` & `crypto-screening-8.4.0/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/database.py` & `crypto-screening-8.4.0/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.4.0/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.4.0/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.4.0/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.4.0/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/market.py` & `crypto-screening-8.4.0/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.4.0/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.4.0/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/orders.py` & `crypto-screening-8.4.0/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/recorder.py` & `crypto-screening-8.4.0/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/trades.py` & `crypto-screening-8.4.0/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/screeners/waiting.py` & `crypto-screening-8.4.0/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.4.0/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/symbols.py` & `crypto-screening-8.4.0/crypto_screening/symbols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # symbols.py
 
 from typing import (
-    Optional, Tuple, Dict, Any, Iterable, Union, Set, Self
+    Optional, Tuple, Dict, Any, Iterable, Set, Self
 )
 
 from attrs import define
 
-from represent import represent, Modifiers
+from represent import represent
 
 __all__ = [
     "Pair",
     "symbol_to_pair",
     "symbol_to_parts",
     "pair_to_symbol",
     "parts_to_symbol",
@@ -29,15 +29,15 @@
 
 class Separator:
     """A class to contain the separator value."""
 
     value = "/"
 # end Separator
 
-@define(slots=False, init=False, repr=False)
+@define(slots=False, init=False, repr=False, eq=False, unsafe_hash=True)
 @represent
 class Pair:
     """
     A class to represent a trading pair.
 
     This object represents a pair of assets that can be traded.
 
@@ -50,112 +50,123 @@
         The asset to use to buy or sell.
 
     >>> from crypto_screening.symbols import Pair
     >>>
     >>> pair = Pair("BTC", "USD")
     """
 
-    __slots__ = "base", "quote", "parts"
+    __slots__ = "_base", "_quote", "separator"
 
-    __modifiers__ = Modifiers(excluded=["parts"])
-
-    def __init__(self, base: str, quote: str) -> None:
+    def __init__(self, base: str, quote: str, separator: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param base: The base asset of the trading pair.
         :param quote: The target asset of the trading pair.
+        :param separator: The symbol separator.
         """
 
-        self.base = base
-        self.quote = quote
+        self._base = base
+        self._quote = quote
 
-        self.parts = (self.base, self.quote)
+        self.separator = separator
     # end __init__
 
-    def __getitem__(self, item: Union[slice, int]) -> Union[str, Tuple[str, str]]:
+    def __eq__(self, other: Any) -> bool:
         """
-        Returns the items.
+        Checks if the signatures are equal.
 
-        :param item: The slice item.
+        :param other: The signature to compare.
 
-        :return: The items in the object to get with the slice.
+        :return: The equality value.
         """
 
-        data = self.parts[item]
-
-        if isinstance(data, list):
-            # noinspection PyTypeChecker
-            return type(self)(*data)
+        if type(other) is not type(self):
+            return NotImplemented
         # end if
 
-        return data
-    # end __getitem__
+        other: Pair
+
+        return (
+            (self.base == other.base) and
+            (self.quote == other.quote)
+        )
+    # end __eq__
 
-    def __len__(self) -> int:
+    @classmethod
+    def load(cls, data: Dict[str, str]) -> Self:
         """
-        The length of the assets.
+        Creates a pair of assets from the data.
 
-        :return: The length of the assets.
+        :param data: The pair data.
+
+        :return: The pair object.
         """
 
-        return len(self.parts)
-    # end __len__
+        return cls(
+            base=data['base'],
+            quote=data['quote'],
+            separator=data.get('separator', None)
+        )
+    # end load
 
-    def __iter__(self) -> Tuple[str, str]:
+    @property
+    def parts(self) -> Tuple[str, str]:
         """
-        Returns the object as an iterable.
+        Returns the property value.
 
-        :return: The iterable object.
+        :return: The symbol.
         """
 
-        yield from self.parts
-    # end __iter__
+        return self._base, self._quote
+    # end parts
 
-    @classmethod
-    def load(cls, data: Dict[str, str]) -> Self:
+    @property
+    def symbol(self) -> str:
         """
-        Creates a pair of assets from the data.
+        Returns the property value.
 
-        :param data: The pair data.
+        :return: The symbol.
+        """
 
-        :return: The pair object.
+        return parts_to_symbol(
+            self._base, self._quote, separator=self.separator
+        )
+    # end symbol
+
+    @property
+    def base(self) -> str:
         """
+        Returns the property value.
 
-        if not (
-            set(data.keys()) == {'base', 'quote'} and
-            all(isinstance(part, str) for part in data.values())
-        ):
-            raise ValueError(
-                f"Pair data must be a dictionary of 'base' and "
-                f"'quote' as keys, and asset names as values, not: {data}"
-            )
-        # end if
+        :return: The base name.
+        """
 
-        return cls(**data)
-    # end load
+        return self._base
+    # end base
 
-    def symbol(self) -> str:
+    @property
+    def quote(self) -> str:
         """
-        Gets the symbols of the chain.
+        Returns the property value.
 
-        :return: The symbols of the trading chain.
+        :return: The base name.
         """
 
-        return pair_to_symbol(self)
-    # end symbols
+        return self._quote
+    # end quote
 
-    def json(self) -> Tuple[str, str]:
+    def json(self) -> Dict[str, str]:
         """
         Converts the data into a json format.
 
         :return: The chain of assets.
         """
 
-        return pair_to_parts(self)
+        return {'base': self.base, 'quote': self.quote}
     # end json
 # end Pair
 
 def pair_to_symbol(pair: Pair, separator: Optional[str] = None) -> str:
     """
     Converts a pair of assets into a symbol.
```

### Comparing `crypto-screening-8.3.0/crypto_screening/utils/base.py` & `crypto-screening-8.4.0/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/utils/process.py` & `crypto-screening-8.4.0/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening/validate.py` & `crypto-screening-8.4.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.4.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.3.0
+Version: 8.4.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.3.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.4.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.3.0/pyproject.toml` & `crypto-screening-8.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.3.0'
+version = '8.4.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.3.0/setup.py` & `crypto-screening-8.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.3.0',
+        version='8.4.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

