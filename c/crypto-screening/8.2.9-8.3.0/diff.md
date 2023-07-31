# Comparing `tmp/crypto-screening-8.2.9.tar.gz` & `tmp/crypto-screening-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-8.2.9.tar", last modified: Sat Jul 29 11:22:26 2023, max compression
+gzip compressed data, was "crypto-screening-8.3.0.tar", last modified: Mon Jul 31 04:42:36 2023, max compression
```

## Comparing `crypto-screening-8.2.9.tar` & `crypto-screening-8.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.937955 crypto-screening-8.2.9/
--rw-rw-rw-   0        0        0      196 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-29 11:22:26.936984 crypto-screening-8.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.2.9/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.2.9/build.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.891374 crypto-screening-8.2.9/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.911832 crypto-screening-8.2.9/crypto_screening/collect/
--rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.2.9/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.2.9/crypto_screening/collect/exchanges.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.915832 crypto-screening-8.2.9/crypto_screening/collect/market/
--rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.2.9/crypto_screening/collect/market/__init__.py
--rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/ohlcv.py
--rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.2.9/crypto_screening/collect/market/orderbook.py
--rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/orders.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.918832 crypto-screening-8.2.9/crypto_screening/collect/market/state/
--rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.2.9/crypto_screening/collect/market/state/__init__.py
--rw-rw-rw-   0        0        0    24665 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/state/assets.py
--rw-rw-rw-   0        0        0    16516 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/state/base.py
--rw-rw-rw-   0        0        0    21653 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/state/symbols.py
--rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/collect/market/trades.py
--rw-rw-rw-   0        0        0    20755 2023-07-27 15:10:03.000000 crypto-screening-8.2.9/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    19564 2023-07-27 15:04:24.000000 crypto-screening-8.2.9/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14801 2023-07-29 10:34:53.000000 crypto-screening-8.2.9/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.2.9/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.2.9/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.925955 crypto-screening-8.2.9/crypto_screening/screeners/
--rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.2.9/crypto_screening/screeners/__init__.py
--rw-rw-rw-   0        0        0    23844 2023-07-29 11:01:44.000000 crypto-screening-8.2.9/crypto_screening/screeners/base.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.928985 crypto-screening-8.2.9/crypto_screening/screeners/callbacks/
--rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.2.9/crypto_screening/screeners/callbacks/__init__.py
--rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.2.9/crypto_screening/screeners/callbacks/base.py
--rw-rw-rw-   0        0        0     4400 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/screeners/callbacks/database.py
--rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/screeners/callbacks/sockets.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.931984 crypto-screening-8.2.9/crypto_screening/screeners/collectors/
--rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.2.9/crypto_screening/screeners/collectors/__init__.py
--rw-rw-rw-   0        0        0     6271 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/screeners/collectors/base.py
--rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.2.9/crypto_screening/screeners/collectors/database.py
--rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/screeners/collectors/sockets.py
--rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.2.9/crypto_screening/screeners/combined.py
--rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.2.9/crypto_screening/screeners/container.py
--rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.2.9/crypto_screening/screeners/database.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.933984 crypto-screening-8.2.9/crypto_screening/screeners/foundation/
--rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.2.9/crypto_screening/screeners/foundation/data.py
--rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.2.9/crypto_screening/screeners/foundation/protocols.py
--rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.2.9/crypto_screening/screeners/foundation/state.py
--rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.2.9/crypto_screening/screeners/foundation/waiting.py
--rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.2.9/crypto_screening/screeners/market.py
--rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.2.9/crypto_screening/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.2.9/crypto_screening/screeners/orderbook.py
--rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.2.9/crypto_screening/screeners/orders.py
--rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.2.9/crypto_screening/screeners/recorder.py
--rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.2.9/crypto_screening/screeners/trades.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.2.9/crypto_screening/screeners/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.882243 crypto-screening-8.2.9/crypto_screening/source/
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.934989 crypto-screening-8.2.9/crypto_screening/source/data/
--rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.2.9/crypto_screening/source/data/all_exchanges_symbols.json
--rw-rw-rw-   0        0        0    10390 2023-07-29 10:33:38.000000 crypto-screening-8.2.9/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.936984 crypto-screening-8.2.9/crypto_screening/utils/
--rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.2.9/crypto_screening/utils/base.py
--rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.2.9/crypto_screening/utils/process.py
--rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.2.9/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-29 11:22:26.909824 crypto-screening-8.2.9/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-29 11:22:26.000000 crypto-screening-8.2.9/pyproject.toml
--rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.2.9/requirements-dev.txt
--rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.2.9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 11:22:26.937955 crypto-screening-8.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-29 11:22:19.000000 crypto-screening-8.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/
+-rw-rw-rw-   0        0        0      196 2023-07-31 04:42:34.000000 crypto-screening-8.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-8.3.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-8.3.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.811425 crypto-screening-8.3.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.837430 crypto-screening-8.3.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    16957 2023-07-24 18:32:29.000000 crypto-screening-8.3.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4944 2023-07-29 11:22:09.000000 crypto-screening-8.3.0/crypto_screening/collect/exchanges.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.864736 crypto-screening-8.3.0/crypto_screening/collect/market/
+-rw-rw-rw-   0        0        0      288 2023-07-24 09:23:18.000000 crypto-screening-8.3.0/crypto_screening/collect/market/__init__.py
+-rw-rw-rw-   0        0        0    19611 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/ohlcv.py
+-rw-rw-rw-   0        0        0    17318 2023-07-24 09:53:00.000000 crypto-screening-8.3.0/crypto_screening/collect/market/orderbook.py
+-rw-rw-rw-   0        0        0    12521 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/orders.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.886737 crypto-screening-8.3.0/crypto_screening/collect/market/state/
+-rw-rw-rw-   0        0        0      136 2023-07-24 09:51:18.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/__init__.py
+-rw-rw-rw-   0        0        0    24329 2023-07-30 10:08:09.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/assets.py
+-rw-rw-rw-   0        0        0    15451 2023-07-30 10:04:40.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/base.py
+-rw-rw-rw-   0        0        0    21291 2023-07-30 10:08:09.000000 crypto-screening-8.3.0/crypto_screening/collect/market/state/symbols.py
+-rw-rw-rw-   0        0        0    15121 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/collect/market/trades.py
+-rw-rw-rw-   0        0        0    21234 2023-07-31 04:41:38.000000 crypto-screening-8.3.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    21503 2023-07-31 04:41:38.000000 crypto-screening-8.3.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15804 2023-07-30 10:04:16.000000 crypto-screening-8.3.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0     1055 2023-07-22 15:46:14.000000 crypto-screening-8.3.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-29 10:34:48.000000 crypto-screening-8.3.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.954345 crypto-screening-8.3.0/crypto_screening/screeners/
+-rw-rw-rw-   0        0        0      508 2023-07-24 09:41:28.000000 crypto-screening-8.3.0/crypto_screening/screeners/__init__.py
+-rw-rw-rw-   0        0        0    23844 2023-07-29 11:01:44.000000 crypto-screening-8.3.0/crypto_screening/screeners/base.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.977342 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/
+-rw-rw-rw-   0        0        0      193 2023-07-24 09:32:57.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     6494 2023-07-24 09:18:38.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/base.py
+-rw-rw-rw-   0        0        0     4400 2023-07-30 10:12:51.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/database.py
+-rw-rw-rw-   0        0        0     5605 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/callbacks/sockets.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.997343 crypto-screening-8.3.0/crypto_screening/screeners/collectors/
+-rw-rw-rw-   0        0        0      196 2023-07-24 09:51:10.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/__init__.py
+-rw-rw-rw-   0        0        0     6253 2023-07-30 10:04:48.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/base.py
+-rw-rw-rw-   0        0        0     4190 2023-07-24 09:45:56.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/database.py
+-rw-rw-rw-   0        0        0     6143 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/collectors/sockets.py
+-rw-rw-rw-   0        0        0    12263 2023-07-24 09:38:16.000000 crypto-screening-8.3.0/crypto_screening/screeners/combined.py
+-rw-rw-rw-   0        0        0    10775 2023-07-24 09:29:30.000000 crypto-screening-8.3.0/crypto_screening/screeners/container.py
+-rw-rw-rw-   0        0        0    10976 2023-07-29 10:34:41.000000 crypto-screening-8.3.0/crypto_screening/screeners/database.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.018342 crypto-screening-8.3.0/crypto_screening/screeners/foundation/
+-rw-rw-rw-   0        0        0    10678 2023-07-27 14:21:39.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/data.py
+-rw-rw-rw-   0        0        0      840 2023-07-18 21:26:30.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1203 2023-07-24 09:37:42.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/state.py
+-rw-rw-rw-   0        0        0     6966 2023-07-24 09:37:50.000000 crypto-screening-8.3.0/crypto_screening/screeners/foundation/waiting.py
+-rw-rw-rw-   0        0        0    15098 2023-07-24 09:29:05.000000 crypto-screening-8.3.0/crypto_screening/screeners/market.py
+-rw-rw-rw-   0        0        0    22149 2023-07-27 14:51:51.000000 crypto-screening-8.3.0/crypto_screening/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    11836 2023-07-27 14:51:29.000000 crypto-screening-8.3.0/crypto_screening/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    11432 2023-07-27 14:51:23.000000 crypto-screening-8.3.0/crypto_screening/screeners/orders.py
+-rw-rw-rw-   0        0        0    16982 2023-07-24 18:21:12.000000 crypto-screening-8.3.0/crypto_screening/screeners/recorder.py
+-rw-rw-rw-   0        0        0    11501 2023-07-27 14:51:13.000000 crypto-screening-8.3.0/crypto_screening/screeners/trades.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 09:40:07.000000 crypto-screening-8.3.0/crypto_screening/screeners/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.777336 crypto-screening-8.3.0/crypto_screening/source/
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.023343 crypto-screening-8.3.0/crypto_screening/source/data/
+-rw-rw-rw-   0        0        0   284601 2023-07-21 09:53:03.000000 crypto-screening-8.3.0/crypto_screening/source/data/all_exchanges_symbols.json
+-rw-rw-rw-   0        0        0    10390 2023-07-29 10:33:38.000000 crypto-screening-8.3.0/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:36.035498 crypto-screening-8.3.0/crypto_screening/utils/
+-rw-rw-rw-   0        0        0     1012 2023-07-22 15:52:54.000000 crypto-screening-8.3.0/crypto_screening/utils/base.py
+-rw-rw-rw-   0        0        0     2765 2023-07-24 18:15:45.000000 crypto-screening-8.3.0/crypto_screening/utils/process.py
+-rw-rw-rw-   0        0        0     3485 2023-07-24 18:15:45.000000 crypto-screening-8.3.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-31 04:42:35.825462 crypto-screening-8.3.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2145 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-31 04:42:35.000000 crypto-screening-8.3.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-31 04:42:34.000000 crypto-screening-8.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      120 2023-07-17 22:21:20.000000 crypto-screening-8.3.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       77 2023-07-17 20:19:29.000000 crypto-screening-8.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-31 04:42:36.036507 crypto-screening-8.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-07-31 04:42:30.000000 crypto-screening-8.3.0/setup.py
```

### Comparing `crypto-screening-8.2.9/PKG-INFO` & `crypto-screening-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.9
+Version: 8.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.9/README.md` & `crypto-screening-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/build.py` & `crypto-screening-8.3.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/assets.py` & `crypto-screening-8.3.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/exchanges.py` & `crypto-screening-8.3.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/ohlcv.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/orderbook.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/orders.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/state/assets.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/state/assets.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,24 @@
 from attrs import define
 
 from represent import represent
 
 import numpy as np
 import pandas as pd
 
-from crypto_screening.dataset import create_dataset
-from crypto_screening.screeners import BaseScreener
-from crypto_screening.screeners import OrderbookScreener
-from crypto_screening.screeners.ohlcv import OHLCVScreener
-from crypto_screening.screeners import OrdersScreener
-from crypto_screening.screeners import TradesScreener
+from crypto_screening.screeners.base import BaseScreener
+from crypto_screening.dataset import index_to_datetime, create_dataset
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
 from crypto_screening.collect.screeners import find_screeners
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
     dataset_to_data_rows, add_data_to_screeners, data_from_dataset,
     minimum_common_dataset_length, screener_dataset,
-    add_data_to_symbols_screeners, index_to_datetime,
-    adjusted_screener_dataset_length, sort_data, set_screener_dataset
+    add_data_to_symbols_screeners, adjusted_screener_dataset_length,
+    sort_data, set_screener_dataset
 )
 
 __all__ = [
     "validate_assets_market_state_values_symbol",
     "assets_market_value",
     "is_symbol_in_assets_market_values",
     "assets_market_values",
@@ -418,22 +414,15 @@
                 )
             # end for
     # end for
 
     return symbols_data
 # end assets_to_symbols_market_data
 
-_S = TypeVar(
-    "_S",
-    BaseScreener,
-    OrderbookScreener,
-    OHLCVScreener,
-    OrdersScreener,
-    TradesScreener
-)
+_S = TypeVar("_S")
 
 AssetsScreeners = Dict[str, Dict[str, Dict[str, _S]]]
 
 def assets_market_datasets_to_screeners(
         datasets: AssetsMarketDatasets,
         adjust: Optional[bool] = True,
         base: Optional[Type[_S]] = None,
```

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/state/base.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/state/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,26 +7,24 @@
     Any, ClassVar, List, Tuple, TypeVar
 )
 
 from attrs import define
 
 from represent import represent, Modifiers
 
-import numpy as np
 import pandas as pd
 
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv
 )
-from crypto_screening.screeners import BaseScreener
-from crypto_screening.screeners import OrderbookScreener
-from crypto_screening.screeners.ohlcv import OHLCVScreener
-from crypto_screening.screeners import OrdersScreener
-from crypto_screening.screeners import TradesScreener
-from crypto_screening.dataset import dataset_to_json
+from crypto_screening.screeners import (
+    BaseScreener, TradesScreener, OrderbookScreener,
+    OHLCVScreener, OrdersScreener
+)
+from crypto_screening.dataset import dataset_to_json, index_to_datetime
 from crypto_screening.collect.screeners import find_screeners
 
 __all__ = [
     "is_exchange_in_market_data",
     "dataset_to_data_rows",
     "MarketState",
     "ORDERBOOK_ATTRIBUTES",
@@ -36,15 +34,14 @@
     "set_screener_dataset",
     "is_match",
     "screener_dataset",
     "get_last_value",
     "no_match_error",
     "is_ohlcv_orderbook_match",
     "minimum_common_dataset_length",
-    "index_to_datetime",
     "data_from_dataset",
     "adjusted_screener_dataset_length",
     "sort_data",
     "validate_market_state_attributes",
     "is_valid_state_attributes"
 ]
 
@@ -432,64 +429,30 @@
     :param adjust: The value to adjust with screeners that are not found.
     :param force: The value to force the data into the screeners.
     """
 
     for screener in screeners:
         for index, row in data:
             if is_ohlcv_orderbook_match(screener=screener, columns=row.keys()):
+                screener: OHLCVScreener
+
                 screener.orderbook_market.loc[index] = row
 
             elif not (force or is_match(screener=screener, columns=row.keys())):
                 if not adjust:
                     raise no_match_error(screener=screener, columns=row.keys())
                 # end if
 
             else:
                 screener.market.loc[index] = row
             # end if
         # end for
     # end for
 # end add_data_to_screeners
 
-def index_to_datetime(index: Any, adjust: Optional[bool] = True) -> dt.datetime:
-    """
-    Converts the index into a datetime object.
-
-    :param index: The value to convert.
-    :param adjust: The value to adjust the process for errors.
-
-    :return: The datetime object.
-    """
-
-    try:
-        if isinstance(index, str):
-            index = dt.datetime.fromisoformat(index)
-
-        elif isinstance(index, (int, float)):
-            index = dt.datetime.fromtimestamp(index)
-
-        elif isinstance(index, pd.Timestamp):
-            index = index.to_pydatetime()
-
-        elif isinstance(index, np.datetime64):
-            index = np.datetime64(dt.datetime.utcnow()).astype(dt.datetime)
-        # end if
-
-    except (TypeError, ValueError) as e:
-        if adjust:
-            pass
-
-        else:
-            raise e
-        # end if
-    # end try
-
-    return index
-# end index_to_datetime
-
 def screener_dataset(
         columns: Dict[str, str], screener: BaseScreener
 ) -> pd.DataFrame:
     """
     Finds the minimum common length of all datasets.
 
     :param columns: The columns for the data.
```

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/state/symbols.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/state/symbols.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,23 @@
 from attrs import define
 
 from represent import represent
 
 import numpy as np
 import pandas as pd
 
-from crypto_screening.dataset import create_dataset
-from crypto_screening.screeners import BaseScreener
-from crypto_screening.screeners import OrderbookScreener
-from crypto_screening.screeners.ohlcv import OHLCVScreener
-from crypto_screening.screeners import OrdersScreener
-from crypto_screening.screeners import TradesScreener
+from crypto_screening.screeners.base import BaseScreener
 from crypto_screening.symbols import symbol_to_parts
 from crypto_screening.collect.screeners import find_screeners
+from crypto_screening.dataset import create_dataset, index_to_datetime
 from crypto_screening.collect.market.state.base import (
     is_exchange_in_market_data, get_last_value, MarketState,
     dataset_to_data_rows, add_data_to_screeners, adjusted_dataset_length,
     minimum_common_dataset_length, screener_dataset, set_screener_dataset,
-    add_data_to_symbols_screeners, index_to_datetime, data_from_dataset,
+    add_data_to_symbols_screeners, data_from_dataset,
     adjusted_screener_dataset_length, sort_data
 )
 
 __all__ = [
     "symbols_market_values",
     "symbols_market_value",
     "validate_symbols_market_state_values_symbol",
@@ -56,15 +52,14 @@
     "add_data_to_screeners",
     "adjusted_dataset_length",
     "sort_symbols_market_data",
     "set_screener_dataset",
     "screener_dataset",
     "get_last_value",
     "minimum_common_dataset_length",
-    "index_to_datetime",
     "symbols_market_datasets",
     "screeners_to_symbols_datasets"
 ]
 
 _V = TypeVar("_V")
 
 Data = List[Tuple[dt.datetime, _V]]
@@ -385,22 +380,15 @@
         # end for
     # end for
 
     return assets_data
 # end assets_to_symbols_market_data
 
 
-_S = TypeVar(
-    "_S",
-    BaseScreener,
-    OrderbookScreener,
-    OHLCVScreener,
-    OrdersScreener,
-    TradesScreener
-)
+_S = TypeVar("_S")
 
 SymbolsScreeners = Dict[str, Dict[str, _S]]
 
 def symbols_market_datasets_to_screeners(
         datasets: SymbolsMarketDatasets,
         adjust: Optional[bool] = True,
         base: Optional[Type[_S]] = None,
```

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/market/trades.py` & `crypto-screening-8.3.0/crypto_screening/collect/market/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/screeners.py` & `crypto-screening-8.3.0/crypto_screening/collect/screeners.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 
 from typing import (
     Optional, Dict, Iterable, TypeVar,
     Set, Union, Tuple, Type, List
 )
 
 import pandas as pd
-from attrs import define
 
-from crypto_screening.symbols import (
-    symbol_to_pair, symbol_to_parts, adjust_symbol
-)
+from crypto_screening.symbols import symbol_to_pair, symbol_to_parts
 from crypto_screening.utils.process import string_in_values
 from crypto_screening.collect.symbols import (
     matching_symbol_pair, MarketSymbolSignature, exchanges_symbols
 )
 from crypto_screening.screeners import (
     BaseScreener, BaseMarketScreener, OHLCVScreener
 )
@@ -117,19 +114,41 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_screener_pairs
 
-@define(repr=False, unsafe_hash=True)
 class MarketScreenerSignature(MarketSymbolSignature):
     """A class to represent the data for the execution of a trade."""
 
-    screener: Optional[BaseScreener] = None
+    def __init__(
+            self,
+            exchange: str,
+            base: str,
+            quote: str,
+            screener: Optional[BaseScreener] = None,
+            separator: Optional[str] = None
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param exchange: The exchange name.
+        :param base: The base asset.
+        :param quote: The quote asset.
+        :param screener: The screener object.
+        """
+
+        super().__init__(
+            exchange=exchange, base=base,
+            quote=quote, separator=separator
+        )
+
+        self.screener = screener
+    # end __init__
 # end MarketScreenerSignature
 
 def matching_screener_signatures(
         data: Optional[Set[Tuple[BaseScreener, BaseScreener]]] = None,
         screeners: Optional[Iterable[BaseScreener]] = None,
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None,
@@ -161,26 +180,26 @@
 
     data = data or matching_screener_pairs(
         screeners=screeners, matches=matches,
         separator=separator, empty=empty
     )
 
     for screener1, screener2 in data:
-        asset1, currency1 = symbol_to_parts(adjust_symbol(screener1.symbol))
-        asset2, currency2 = symbol_to_pair(adjust_symbol(screener2.symbol))
+        asset1, currency1 = symbol_to_parts(screener1.symbol)
+        asset2, currency2 = symbol_to_pair(screener2.symbol)
 
         pairs.add(
             (
                 MarketScreenerSignature(
-                    asset=asset1, currency=currency1,
+                    base=asset1, quote=currency1,
                     exchange=screener1.exchange,
                     screener=screener1
                 ),
                 MarketScreenerSignature(
-                    asset=asset2, currency=currency2,
+                    base=asset2, quote=currency2,
                     exchange=screener2.exchange,
                     screener=screener2
                 )
             )
         )
     # end for
```

### Comparing `crypto-screening-8.2.9/crypto_screening/collect/symbols.py` & `crypto-screening-8.3.0/crypto_screening/collect/symbols.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 # symbols.py
 
 import warnings
 from typing import (
-    Optional, Dict, Iterable, Set, Union, Tuple
+    Optional, Dict, Iterable, Set, Union, Tuple, Any
 )
 
-from attrs import define
-
 from represent import represent
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.utils.process import (
     find_string_value, upper_string_values,
     mutual_string_values, string_in_values
 )
 from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
 from crypto_screening.symbols import (
-    symbol_to_parts, adjust_symbol, Separator
+    symbol_to_parts, adjust_symbol, Separator, parts_to_symbol
 )
 from crypto_screening.validate import validate_exchange
 from crypto_screening.collect.exchanges import exchanges_data
 
 __all__ = [
     "exchanges_symbols",
     "mutual_exchanges_symbols",
@@ -577,22 +575,117 @@
             # end if
         # end for
     # end for
 
     return set(pairs)
 # end matching_symbol_pairs
 
-@define(repr=False, unsafe_hash=True)
 @represent
 class MarketSymbolSignature:
     """A class to represent the data for the execution of a trade."""
 
-    asset: str
-    currency: str
-    exchange: str
+    def __init__(
+            self,
+            exchange: str,
+            base: str,
+            quote: str,
+            separator: Optional[str] = None
+    ) -> None:
+        """
+        Defines the class attributes.
+
+        :param exchange: The exchange name.
+        :param base: The base asset.
+        :param quote: The quote asset.
+        """
+
+        self._exchange = exchange
+        self._base = base
+        self._quote = quote
+
+        self.separator = separator
+    # end __init__
+
+    def __hash__(self) -> int:
+        """
+        Returns the hash of the object.
+
+        :return: The hash.
+        """
+
+        return id(self)
+    # end __hash__
+
+    def __eq__(self, other: Any) -> bool:
+        """
+        Checks if the signatures are equal.
+
+        :param other: The signature to compare.
+
+        :return: The equality value.
+        """
+
+        if type(other) is not type(self):
+            return NotImplemented
+        # end if
+
+        other: MarketSymbolSignature
+
+        return (
+            (self.exchange == other.exchange) and
+            (self.base == other.base) and
+            (self.quote == other.quote)
+        )
+    # end __eq__
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
+    @property
+    def symbol(self) -> str:
+        """
+        Returns the property value.
+
+        :return: The symbol.
+        """
+
+        return parts_to_symbol(
+            self._base, self._quote, separator=self.separator
+        )
+    # end symbol
+
+    @property
+    def base(self) -> str:
+        """
+        Returns the property value.
+
+        :return: The base name.
+        """
+
+        return self._base
+    # end base
+
+    @property
+    def quote(self) -> str:
+        """
+        Returns the property value.
+
+        :return: The base name.
+        """
+
+        return self._quote
+    # end quote
 # end MarketPairSignature
 
 def matching_symbol_signatures(
         pairs: Optional[ExchangeSymbolPairs] = None,
         data: Optional[Dict[str, Iterable[str]]] = None,
         matches: Optional[ExchangesAssetMatches] = None,
         separator: Optional[str] = None
@@ -621,25 +714,25 @@
     new_pairs = []
 
     pairs = pairs or matching_symbol_pairs(
         data=data, matches=matches, separator=separator
     )
 
     for (exchange1, symbol1), (exchange2, symbol2) in pairs:
-        asset1, currency1 = symbol_to_parts(adjust_symbol(symbol1))
-        asset2, currency2 = symbol_to_parts(adjust_symbol(symbol2))
+        asset1, currency1 = symbol_to_parts(symbol1)
+        asset2, currency2 = symbol_to_parts(symbol2)
 
         new_pairs.append(
             (
                 MarketSymbolSignature(
-                    asset=asset1, currency=currency1,
+                    base=asset1, quote=currency1,
                     exchange=exchange1
                 ),
                 MarketSymbolSignature(
-                    asset=asset2, currency=currency2,
+                    base=asset2, quote=currency2,
                     exchange=exchange2
                 )
             )
         )
     # end for
 
     return set(new_pairs)
```

### Comparing `crypto-screening-8.2.9/crypto_screening/dataset.py` & `crypto-screening-8.3.0/crypto_screening/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # dataset.py
 
 import os
+import datetime as dt
 import json
 from pathlib import Path
 from typing import (
     Union, Optional, Tuple, Iterable,
     Any, Callable, Dict, List
 )
 
+import numpy as np
 import pandas as pd
 from pandas.core.resample import Resampler
 
 from crypto_screening.interval import interval_to_total_time
 
 __all__ = [
     "row_to_dataset",
@@ -51,15 +53,16 @@
     "ORDERBOOK_COLUMNS",
     "TRADES_COLUMNS",
     "PRICE",
     "SIDE",
     "ORDERS_COLUMNS",
     "AMOUNT",
     "adjust_series",
-    "interval_adjuster"
+    "interval_adjuster",
+    "index_to_datetime"
 ]
 
 DATE_TIME = 'DateTime'
 
 OPEN = "Open"
 CLOSE = "Close"
 HIGH = "High"
@@ -79,14 +82,50 @@
 
 OHLC_COLUMNS = (OPEN, HIGH, LOW, CLOSE)
 OHLCV_COLUMNS = (*OHLC_COLUMNS, VOLUME)
 ORDERBOOK_COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
 TRADES_COLUMNS = (AMOUNT, PRICE, SIDE)
 ORDERS_COLUMNS = (BIDS, ASKS)
 
+def index_to_datetime(index: Any, adjust: Optional[bool] = True) -> dt.datetime:
+    """
+    Converts the index into a datetime object.
+
+    :param index: The value to convert.
+    :param adjust: The value to adjust the process for errors.
+
+    :return: The datetime object.
+    """
+
+    try:
+        if isinstance(index, str):
+            index = dt.datetime.fromisoformat(index)
+
+        elif isinstance(index, (int, float)):
+            index = dt.datetime.fromtimestamp(index)
+
+        elif isinstance(index, pd.Timestamp):
+            index = index.to_pydatetime()
+
+        elif isinstance(index, np.datetime64):
+            index = np.datetime64(dt.datetime.utcnow()).astype(dt.datetime)
+        # end if
+
+    except (TypeError, ValueError) as e:
+        if adjust:
+            pass
+
+        else:
+            raise e
+        # end if
+    # end try
+
+    return index
+# end index_to_datetime
+
 def row_to_dataset(
         dataset: Union[pd.DataFrame, pd.Series],
         index: Optional[int] = None
 ) -> pd.DataFrame:
     """
     Creates a dataframe from the row.
```

### Comparing `crypto-screening-8.2.9/crypto_screening/exchanges.py` & `crypto-screening-8.3.0/crypto_screening/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/interval.py` & `crypto-screening-8.3.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/base.py` & `crypto-screening-8.3.0/crypto_screening/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/callbacks/base.py` & `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/callbacks/database.py` & `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/callbacks/sockets.py` & `crypto-screening-8.3.0/crypto_screening/screeners/callbacks/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/collectors/base.py` & `crypto-screening-8.3.0/crypto_screening/screeners/collectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import threading
 import datetime as dt
 import time
 from typing import List, Tuple, Optional, Iterable, Union, Dict, Any
 
 from crypto_screening.screeners.container import ScreenersContainer
 from crypto_screening.screeners.base import BaseScreener, BaseMarketScreener
-from crypto_screening.collect.market.state.base import index_to_datetime
+from crypto_screening.dataset import index_to_datetime
 
 __all__ = [
     "ScreenersDataCollector"
 ]
 
 Data = List[Tuple[Union[str, float, dt.datetime], Dict[str, Optional[Union[str, float, bool]]]]]
```

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/collectors/database.py` & `crypto-screening-8.3.0/crypto_screening/screeners/collectors/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/collectors/sockets.py` & `crypto-screening-8.3.0/crypto_screening/screeners/collectors/sockets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/combined.py` & `crypto-screening-8.3.0/crypto_screening/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/container.py` & `crypto-screening-8.3.0/crypto_screening/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/database.py` & `crypto-screening-8.3.0/crypto_screening/screeners/database.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/foundation/data.py` & `crypto-screening-8.3.0/crypto_screening/screeners/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/foundation/protocols.py` & `crypto-screening-8.3.0/crypto_screening/screeners/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/foundation/state.py` & `crypto-screening-8.3.0/crypto_screening/screeners/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/foundation/waiting.py` & `crypto-screening-8.3.0/crypto_screening/screeners/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/market.py` & `crypto-screening-8.3.0/crypto_screening/screeners/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/ohlcv.py` & `crypto-screening-8.3.0/crypto_screening/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/orderbook.py` & `crypto-screening-8.3.0/crypto_screening/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/orders.py` & `crypto-screening-8.3.0/crypto_screening/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/recorder.py` & `crypto-screening-8.3.0/crypto_screening/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/trades.py` & `crypto-screening-8.3.0/crypto_screening/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/screeners/waiting.py` & `crypto-screening-8.3.0/crypto_screening/screeners/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/source/data/all_exchanges_symbols.json` & `crypto-screening-8.3.0/crypto_screening/source/data/all_exchanges_symbols.json`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/symbols.py` & `crypto-screening-8.3.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/utils/base.py` & `crypto-screening-8.3.0/crypto_screening/utils/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/utils/process.py` & `crypto-screening-8.3.0/crypto_screening/utils/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening/validate.py` & `crypto-screening-8.3.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-8.3.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 8.2.9
+Version: 8.3.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-8.2.9/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-8.3.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-8.2.9/pyproject.toml` & `crypto-screening-8.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '8.2.9'
+version = '8.3.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-8.2.9/setup.py` & `crypto-screening-8.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "crypto_screening/source"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='8.2.9',
+        version='8.3.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

