# Comparing `tmp/basana-1.3.1.tar.gz` & `tmp/basana-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basana-1.3.1.tar", max compression
+gzip compressed data, was "basana-1.3.2.tar", max compression
```

## Comparing `basana-1.3.1.tar` & `basana-1.3.2.tar`

### file list

```diff
@@ -1,70 +1,73 @@
--rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.3.1/LICENSE
--rw-r--r--   0        0        0     1263 2023-04-13 16:56:31.180127 basana-1.3.1/basana/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.3.1/basana/backtesting/__init__.py
--rw-r--r--   0        0        0     3922 2023-04-25 19:59:42.240369 basana-1.3.1/basana/backtesting/account_balances.py
--rw-r--r--   0        0        0    13477 2023-05-22 18:02:28.536545 basana-1.3.1/basana/backtesting/charts.py
--rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.3.1/basana/backtesting/errors.py
--rw-r--r--   0        0        0    22695 2023-04-28 03:07:23.323961 basana-1.3.1/basana/backtesting/exchange.py
--rw-r--r--   0        0        0     2547 2023-04-28 03:07:23.324848 basana-1.3.1/basana/backtesting/fees.py
--rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.3.1/basana/backtesting/helpers.py
--rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.3.1/basana/backtesting/liquidity.py
--rw-r--r--   0        0        0    16012 2023-04-28 03:07:23.326054 basana-1.3.1/basana/backtesting/orders.py
--rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.3.1/basana/backtesting/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.3.1/basana/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.3.1/basana/core/bar.py
--rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.3.1/basana/core/config.py
--rw-r--r--   0        0        0     9620 2023-04-28 03:07:23.327710 basana-1.3.1/basana/core/dispatcher.py
--rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.3.1/basana/core/dt.py
--rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.3.1/basana/core/enums.py
--rw-r--r--   0        0        0     3456 2023-04-28 03:07:23.328623 basana-1.3.1/basana/core/event.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.3.1/basana/core/event_sources/__init__.py
--rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.3.1/basana/core/event_sources/csv.py
--rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.3.1/basana/core/event_sources/trading_signal.py
--rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.3.1/basana/core/helpers.py
--rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.3.1/basana/core/logs.py
--rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.3.1/basana/core/pair.py
--rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.3.1/basana/core/token_bucket.py
--rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.3.1/basana/core/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.3.1/basana/external/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.3.1/basana/external/binance/__init__.py
--rw-r--r--   0        0        0    20702 2023-04-28 03:07:23.330411 basana-1.3.1/basana/external/binance/client.py
--rw-r--r--   0        0        0    10335 2023-04-13 16:56:31.184239 basana-1.3.1/basana/external/binance/common.py
--rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.3.1/basana/external/binance/config.py
--rw-r--r--   0        0        0     2111 2023-04-13 16:56:31.184643 basana-1.3.1/basana/external/binance/cross_margin.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.3.1/basana/external/binance/csv/__init__.py
--rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.3.1/basana/external/binance/csv/bars.py
--rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.3.1/basana/external/binance/exchange.py
--rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.3.1/basana/external/binance/helpers.py
--rw-r--r--   0        0        0     3187 2023-04-13 16:56:31.186035 basana-1.3.1/basana/external/binance/isolated_margin.py
--rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.3.1/basana/external/binance/klines.py
--rw-r--r--   0        0        0    12082 2023-04-28 03:07:23.331079 basana-1.3.1/basana/external/binance/margin.py
--rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.3.1/basana/external/binance/margin_requests.py
--rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.3.1/basana/external/binance/order_book.py
--rw-r--r--   0        0        0    12177 2023-04-13 16:56:31.188619 basana-1.3.1/basana/external/binance/spot.py
--rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.3.1/basana/external/binance/spot_requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.3.1/basana/external/binance/tools/__init__.py
--rw-r--r--   0        0        0     4373 2023-03-29 02:43:04.772398 basana-1.3.1/basana/external/binance/tools/download_bars.py
--rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.3.1/basana/external/binance/trades.py
--rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.3.1/basana/external/binance/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.3.1/basana/external/bitstamp/__init__.py
--rw-r--r--   0        0        0     8684 2023-03-29 02:43:04.773512 basana-1.3.1/basana/external/bitstamp/client.py
--rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.3.1/basana/external/bitstamp/config.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.3.1/basana/external/bitstamp/csv/__init__.py
--rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.3.1/basana/external/bitstamp/csv/bars.py
--rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.3.1/basana/external/bitstamp/exchange.py
--rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.3.1/basana/external/bitstamp/helpers.py
--rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.3.1/basana/external/bitstamp/order_book.py
--rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.3.1/basana/external/bitstamp/orders.py
--rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.3.1/basana/external/bitstamp/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.3.1/basana/external/bitstamp/tools/__init__.py
--rw-r--r--   0        0        0     4069 2023-03-29 02:43:04.777227 basana-1.3.1/basana/external/bitstamp/tools/download_bars.py
--rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.3.1/basana/external/bitstamp/trades.py
--rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.3.1/basana/external/bitstamp/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.3.1/basana/external/common/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.3.1/basana/external/common/csv/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.3.1/basana/external/common/csv/bars.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.3.1/basana/external/yahoo/__init__.py
--rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.3.1/basana/external/yahoo/bars.py
--rw-r--r--   0        0        0     1189 2023-05-22 18:55:08.883336 basana-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 basana-1.3.1/setup.py
--rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1263 2023-04-13 16:56:31.180127 basana-1.3.2/basana/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.3.2/basana/backtesting/__init__.py
+-rw-r--r--   0        0        0     3922 2023-07-14 16:10:28.128588 basana-1.3.2/basana/backtesting/account_balances.py
+-rw-r--r--   0        0        0    13477 2023-07-14 16:10:28.129043 basana-1.3.2/basana/backtesting/charts.py
+-rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.3.2/basana/backtesting/errors.py
+-rw-r--r--   0        0        0    22695 2023-07-14 16:10:28.129542 basana-1.3.2/basana/backtesting/exchange.py
+-rw-r--r--   0        0        0     2547 2023-07-14 16:10:28.129930 basana-1.3.2/basana/backtesting/fees.py
+-rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.3.2/basana/backtesting/helpers.py
+-rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.3.2/basana/backtesting/liquidity.py
+-rw-r--r--   0        0        0    16012 2023-04-28 03:07:23.326054 basana-1.3.2/basana/backtesting/orders.py
+-rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.3.2/basana/backtesting/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.3.2/basana/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.3.2/basana/core/bar.py
+-rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.3.2/basana/core/config.py
+-rw-r--r--   0        0        0     9620 2023-07-30 23:19:27.287155 basana-1.3.2/basana/core/dispatcher.py
+-rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.3.2/basana/core/dt.py
+-rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.3.2/basana/core/enums.py
+-rw-r--r--   0        0        0     3456 2023-07-15 22:07:34.279552 basana-1.3.2/basana/core/event.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.3.2/basana/core/event_sources/__init__.py
+-rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.3.2/basana/core/event_sources/csv.py
+-rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.3.2/basana/core/event_sources/trading_signal.py
+-rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.3.2/basana/core/helpers.py
+-rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.3.2/basana/core/logs.py
+-rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.3.2/basana/core/pair.py
+-rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.3.2/basana/core/token_bucket.py
+-rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.3.2/basana/core/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.3.2/basana/external/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.3.2/basana/external/binance/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-04 19:35:09.136123 basana-1.3.2/basana/external/binance/client/__init__.py
+-rw-r--r--   0        0        0     4971 2023-07-04 19:35:09.136332 basana-1.3.2/basana/external/binance/client/base.py
+-rw-r--r--   0        0        0     8900 2023-07-04 19:35:09.136544 basana-1.3.2/basana/external/binance/client/margin.py
+-rw-r--r--   0        0        0     6166 2023-07-04 19:35:09.136766 basana-1.3.2/basana/external/binance/client/spot.py
+-rw-r--r--   0        0        0    10335 2023-04-13 16:56:31.184239 basana-1.3.2/basana/external/binance/common.py
+-rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.3.2/basana/external/binance/config.py
+-rw-r--r--   0        0        0     2161 2023-07-04 19:35:09.137470 basana-1.3.2/basana/external/binance/cross_margin.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.3.2/basana/external/binance/csv/__init__.py
+-rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.3.2/basana/external/binance/csv/bars.py
+-rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.3.2/basana/external/binance/exchange.py
+-rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.3.2/basana/external/binance/helpers.py
+-rw-r--r--   0        0        0     3237 2023-07-04 19:35:09.138017 basana-1.3.2/basana/external/binance/isolated_margin.py
+-rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.3.2/basana/external/binance/klines.py
+-rw-r--r--   0        0        0    12125 2023-07-04 19:35:09.138533 basana-1.3.2/basana/external/binance/margin.py
+-rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.3.2/basana/external/binance/margin_requests.py
+-rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.3.2/basana/external/binance/order_book.py
+-rw-r--r--   0        0        0    12214 2023-07-04 19:35:09.139462 basana-1.3.2/basana/external/binance/spot.py
+-rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.3.2/basana/external/binance/spot_requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.3.2/basana/external/binance/tools/__init__.py
+-rw-r--r--   0        0        0     4521 2023-06-12 21:54:52.853855 basana-1.3.2/basana/external/binance/tools/download_bars.py
+-rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.3.2/basana/external/binance/trades.py
+-rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.3.2/basana/external/binance/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.3.2/basana/external/bitstamp/__init__.py
+-rw-r--r--   0        0        0     9077 2023-07-04 19:35:09.140072 basana-1.3.2/basana/external/bitstamp/client.py
+-rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.3.2/basana/external/bitstamp/config.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.3.2/basana/external/bitstamp/csv/__init__.py
+-rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.3.2/basana/external/bitstamp/csv/bars.py
+-rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.3.2/basana/external/bitstamp/exchange.py
+-rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.3.2/basana/external/bitstamp/helpers.py
+-rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.3.2/basana/external/bitstamp/order_book.py
+-rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.3.2/basana/external/bitstamp/orders.py
+-rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.3.2/basana/external/bitstamp/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.3.2/basana/external/bitstamp/tools/__init__.py
+-rw-r--r--   0        0        0     4098 2023-06-12 21:54:52.854666 basana-1.3.2/basana/external/bitstamp/tools/download_bars.py
+-rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.3.2/basana/external/bitstamp/trades.py
+-rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.3.2/basana/external/bitstamp/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.3.2/basana/external/common/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.3.2/basana/external/common/csv/__init__.py
+-rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.3.2/basana/external/common/csv/bars.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.3.2/basana/external/yahoo/__init__.py
+-rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.3.2/basana/external/yahoo/bars.py
+-rw-r--r--   0        0        0     1189 2023-07-31 00:51:37.170951 basana-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1294 1970-01-01 00:00:00.000000 basana-1.3.2/setup.py
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.3.2/PKG-INFO
```

### Comparing `basana-1.3.1/LICENSE` & `basana-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/__init__.py` & `basana-1.3.2/basana/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/__init__.py` & `basana-1.3.2/basana/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/account_balances.py` & `basana-1.3.2/basana/backtesting/account_balances.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/charts.py` & `basana-1.3.2/basana/backtesting/charts.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/errors.py` & `basana-1.3.2/basana/backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/exchange.py` & `basana-1.3.2/basana/backtesting/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/fees.py` & `basana-1.3.2/basana/backtesting/fees.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/helpers.py` & `basana-1.3.2/basana/backtesting/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/liquidity.py` & `basana-1.3.2/basana/backtesting/liquidity.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/orders.py` & `basana-1.3.2/basana/backtesting/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/backtesting/requests.py` & `basana-1.3.2/basana/backtesting/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/__init__.py` & `basana-1.3.2/basana/core/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/bar.py` & `basana-1.3.2/basana/core/bar.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/config.py` & `basana-1.3.2/basana/core/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/dispatcher.py` & `basana-1.3.2/basana/core/dispatcher.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/dt.py` & `basana-1.3.2/basana/core/dt.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/enums.py` & `basana-1.3.2/basana/core/enums.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/event.py` & `basana-1.3.2/basana/core/event.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/event_sources/__init__.py` & `basana-1.3.2/basana/core/event_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/event_sources/csv.py` & `basana-1.3.2/basana/core/event_sources/csv.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/event_sources/trading_signal.py` & `basana-1.3.2/basana/core/event_sources/trading_signal.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/helpers.py` & `basana-1.3.2/basana/core/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/logs.py` & `basana-1.3.2/basana/core/logs.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/pair.py` & `basana-1.3.2/basana/core/pair.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/token_bucket.py` & `basana-1.3.2/basana/core/token_bucket.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/core/websockets.py` & `basana-1.3.2/basana/core/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/__init__.py` & `basana-1.3.2/basana/external/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/__init__.py` & `basana-1.3.2/basana/external/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/common.py` & `basana-1.3.2/basana/external/binance/common.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/config.py` & `basana-1.3.2/basana/external/binance/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/cross_margin.py` & `basana-1.3.2/basana/external/binance/cross_margin.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
 from typing import Dict
 
-from . import client, margin
+from . import margin
+from .client import margin as margin_client
 
 
 class Account(margin.Account):
     """Cross margin account."""
-    def __init__(self, cli: client.CrossMarginAccount):
+    def __init__(self, cli: margin_client.CrossMarginAccount):
         self._cli = cli
 
     @property
-    def client(self) -> client.CrossMarginAccount:
+    def client(self) -> margin_client.CrossMarginAccount:
         return self._cli
 
     async def get_balances(self) -> Dict[str, margin.Balance]:
         """Returns all balances."""
         account_info = await self.client.get_account_information()
         return {balance["asset"].upper(): margin.Balance(balance) for balance in account_info["userAssets"]}
```

### Comparing `basana-1.3.1/basana/external/binance/csv/__init__.py` & `basana-1.3.2/basana/external/binance/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/csv/bars.py` & `basana-1.3.2/basana/external/binance/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/exchange.py` & `basana-1.3.2/basana/external/binance/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/helpers.py` & `basana-1.3.2/basana/external/binance/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/isolated_margin.py` & `basana-1.3.2/basana/external/binance/isolated_margin.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
 from typing import Dict
 
-from . import client, helpers, margin
+from . import helpers, margin
+from .client import margin as margin_client
 from basana.core.pair import Pair
 
 
 class IsolatedBalance:
     def __init__(self, json: dict):
         self.json = json
 
@@ -44,19 +45,19 @@
     def quote_asset_balance(self) -> margin.Balance:
         """The quote asset balance."""
         return margin.Balance(self.json["quoteAsset"])
 
 
 class Account(margin.Account):
     """Isolated margin account."""
-    def __init__(self, cli: client.IsolatedMarginAccount):
+    def __init__(self, cli: margin_client.IsolatedMarginAccount):
         self._cli = cli
 
     @property
-    def client(self) -> client.IsolatedMarginAccount:
+    def client(self) -> margin_client.IsolatedMarginAccount:
         return self._cli
 
     async def get_balances(self) -> Dict[Pair, IsolatedBalance]:
         """Returns all balances."""
         account_info = await self.client.get_account_information()
         ret = {}
         for isolated_balance in account_info["assets"]:
```

### Comparing `basana-1.3.1/basana/external/binance/klines.py` & `basana-1.3.2/basana/external/binance/klines.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/margin.py` & `basana-1.3.2/basana/external/binance/margin.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
 from typing import Any, Dict, List, Optional
 import abc
 
-from . import client, common, helpers, margin_requests
+from . import common, helpers, margin_requests
+from .client import margin as margin_client
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
 
 
 class CanceledOCOOrder(common.CanceledOCOOrder):
     pass
 
@@ -73,15 +74,15 @@
         """
         return [Fill(fill) for fill in self.json.get("fills", [])]
 
 
 class Account(metaclass=abc.ABCMeta):
     @property
     @abc.abstractmethod
-    def client(self) -> client.MarginAccount:
+    def client(self) -> margin_client.MarginAccount:
         raise NotImplementedError()
 
     async def create_order(self, order_request: margin_requests.ExchangeOrder) -> CreatedOrder:
         created_order = await order_request.create_order(self.client)
         return CreatedOrder(created_order)
 
     async def create_market_order(
```

### Comparing `basana-1.3.1/basana/external/binance/margin_requests.py` & `basana-1.3.2/basana/external/binance/margin_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/order_book.py` & `basana-1.3.2/basana/external/binance/order_book.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/spot.py` & `basana-1.3.2/basana/external/binance/spot.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
 from typing import Any, Dict, List, Optional
 
-from . import client, common, helpers, spot_requests
+from . import common, helpers, spot_requests
+from .client import spot as spot_client
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
 
 
 Balance = common.Balance
 CanceledOCOOrder = common.CanceledOCOOrder
 CanceledOrder = common.CanceledOrder
@@ -73,15 +74,15 @@
     def quote_amount(self) -> Optional[Decimal]:
         """The order amount in quote units."""
         return helpers.get_optional_decimal(self.json, "origQuoteOrderQty", True)
 
 
 class Account:
     """Spot account."""
-    def __init__(self, cli: client.SpotAccount):
+    def __init__(self, cli: spot_client.SpotAccount):
         self._cli = cli
 
     async def get_balances(self) -> Dict[str, Balance]:
         """Returns all balances."""
         account_info = await self._cli.get_account_information()
         return {balance["asset"].upper(): Balance(balance) for balance in account_info["balances"]}
```

### Comparing `basana-1.3.1/basana/external/binance/spot_requests.py` & `basana-1.3.2/basana/external/binance/spot_requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/tools/__init__.py` & `basana-1.3.2/basana/external/binance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/tools/download_bars.py` & `basana-1.3.2/basana/external/binance/tools/download_bars.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import List, Optional
 import argparse
 import datetime
 
 import aiohttp
 import asyncio
 
-from basana.core import token_bucket
+from basana.core import dt, token_bucket
 from basana.external.binance import client, helpers
 
 
 period_to_step = {
     "1s": 1,
     "1m": 60,
     "3m": 3 * 60,
@@ -55,14 +55,15 @@
     def __init__(self, candlestick: list):
         self.open_timestamp = candlestick[0]
         self.open = candlestick[1]
         self.high = candlestick[2]
         self.low = candlestick[3]
         self.close = candlestick[4]
         self.volume = candlestick[5]
+        self.close_timestamp = candlestick[6]
 
 
 def to_binance_currency_pair(currency_pair: str):
     parts = currency_pair.upper().split("/")
     return "".join(parts)
 
 
@@ -102,29 +103,30 @@
     past_the_end = end + datetime.timedelta(seconds=max(period_to_step["1d"], step))
 
     start_ts = helpers.datetime_to_timestamp(start)
     past_the_end_ts = helpers.datetime_to_timestamp(past_the_end)
     step = step * 1000
 
     tb = token_bucket.TokenBucketLimiter(10, 1)
+    now_ts = helpers.datetime_to_timestamp(dt.utc_now())
     writer = CSVWriter()
     async with aiohttp.ClientSession() as session:
         cli = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
         eof = False
         currency_pair = to_binance_currency_pair(args.currency_pair)
         while not eof:
             response = await cli.get_candlestick_data(
                 currency_pair, args.period, start_time=start_ts, end_time=past_the_end_ts, limit=1000
             )
             eof = True
             for candlestick in response:
                 eof = False
                 candlestick = Candlestick(candlestick)
                 start_ts = max(start_ts, candlestick.open_timestamp)
-                if candlestick.open_timestamp >= past_the_end_ts:
+                if candlestick.open_timestamp >= past_the_end_ts or candlestick.close_timestamp >= now_ts:
                     continue
                 writer.write_candlestick(candlestick)
             if not eof:
                 start_ts += step
                 eof = start_ts >= past_the_end_ts
```

### Comparing `basana-1.3.1/basana/external/binance/trades.py` & `basana-1.3.2/basana/external/binance/trades.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/binance/websockets.py` & `basana-1.3.2/basana/external/binance/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/__init__.py` & `basana-1.3.2/basana/external/bitstamp/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/client.py` & `basana-1.3.2/basana/external/bitstamp/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Sequence, Tuple, Union
 from urllib.parse import urlparse, urljoin
 import asyncio
 
 import aiohttp
 
 from basana.core import token_bucket, helpers as core_helpers
 from basana.core.config import get_config_value
@@ -110,26 +110,29 @@
             params = {"group": group}
         return await self._make_request("GET", f"/api/v2/order_book/{currency_pair}/", False, qs_params=params)
 
     async def get_ticker(self, currency_pair: str) -> dict:
         return await self._make_request("GET", f"/api/v2/ticker/{currency_pair}/", False)
 
     async def get_ohlc_data(
-            self, currency_pair: str, step: int, limit: int, start: Optional[int] = None, end: Optional[int] = None
+            self, currency_pair: str, step: int, limit: int, start: Optional[int] = None, end: Optional[int] = None,
+            exclude_current_candle: bool = False
     ) -> dict:
         assert start is None or end is None, "both start and end should not be set"
 
-        params = {
+        params: Dict[str, Any] = {
             "step": step,
             "limit": limit,
         }
-        if start:
-            params["start"] = start
-        if end:
-            params["end"] = end
+        set_optional_params(params, (
+            ("start", start),
+            ("end", end),
+        ))
+        if exclude_current_candle:
+            params["exclude_current_candle"] = "true"
         return await self._make_request("GET", f"/api/v2/ohlc/{currency_pair}/", False, qs_params=params)
 
     async def get_websocket_auth_token(self) -> dict:
         return await self._make_request("POST", "/api/v2/websockets_token/", True)
 
     async def get_account_balances(self) -> List[dict]:
         return await self._make_request("POST", "/api/v2/account_balances/", True)
@@ -190,13 +193,22 @@
     ) -> dict:
         assert action in ["buy", "sell"], "Invalid action"
         assert amount_in_counter is False or action == "sell", "amount_in_counter only supported for sell orders"
 
         data: Dict[str, Any] = {
             "amount": str(amount),
         }
-        if client_order_id:
-            data["client_order_id"] = client_order_id
-        if amount_in_counter:
-            data["amount_in_counter"] = amount_in_counter
+        set_optional_params(data, (
+            ("client_order_id", client_order_id),
+            ("amount_in_counter", amount_in_counter),
+        ))
         data.update(kwargs)
         return await self._make_request("POST", f"/api/v2/{action}/instant/{currency_pair}/", True, data=data)
+
+
+def set_optional_params(params: Dict[str, Any], tuples: Sequence[Tuple[str, Any]]):
+    for k, v in tuples:
+        if v is None:
+            continue
+        # if isinstance(v, Decimal):
+        #     v = str(v)
+        params[k] = v
```

### Comparing `basana-1.3.1/basana/external/bitstamp/config.py` & `basana-1.3.2/basana/external/bitstamp/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/csv/__init__.py` & `basana-1.3.2/basana/external/bitstamp/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/csv/bars.py` & `basana-1.3.2/basana/external/bitstamp/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/exchange.py` & `basana-1.3.2/basana/external/bitstamp/exchange.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/helpers.py` & `basana-1.3.2/basana/external/bitstamp/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/order_book.py` & `basana-1.3.2/basana/external/bitstamp/order_book.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/orders.py` & `basana-1.3.2/basana/external/bitstamp/orders.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/requests.py` & `basana-1.3.2/basana/external/bitstamp/requests.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/tools/__init__.py` & `basana-1.3.2/basana/external/bitstamp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/tools/download_bars.py` & `basana-1.3.2/basana/external/bitstamp/tools/download_bars.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     tb = token_bucket.TokenBucketLimiter(10, 1)
     writer = CSVWriter()
     async with aiohttp.ClientSession() as session:
         cli = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
         eof = False
         currency_pair = to_bitstamp_currency_pair(args.currency_pair)
         while not eof:
-            response = await cli.get_ohlc_data(currency_pair, step, 1000, start=start_ts)
+            response = await cli.get_ohlc_data(currency_pair, step, 1000, start=start_ts, exclude_current_candle=True)
             eof = True
             for ohlc in response["data"]["ohlc"]:
                 eof = False
                 ohlc = OHLC(ohlc)
                 start_ts = max(start_ts, ohlc.open_timestamp)
                 if ohlc.open_timestamp >= past_the_end_ts:
                     continue
```

### Comparing `basana-1.3.1/basana/external/bitstamp/trades.py` & `basana-1.3.2/basana/external/bitstamp/trades.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/bitstamp/websockets.py` & `basana-1.3.2/basana/external/bitstamp/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/common/__init__.py` & `basana-1.3.2/basana/external/common/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/common/csv/__init__.py` & `basana-1.3.2/basana/external/common/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/common/csv/bars.py` & `basana-1.3.2/basana/external/common/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/yahoo/__init__.py` & `basana-1.3.2/basana/external/yahoo/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/basana/external/yahoo/bars.py` & `basana-1.3.2/basana/external/yahoo/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.3.1/pyproject.toml` & `basana-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "basana"
-version = "1.3.1"
+version = "1.3.2"
 homepage = "https://github.com/gbeced/basana"
 repository = "https://github.com/gbeced/basana"
 documentation = "https://basana.readthedocs.io/en/latest/"
 description = "A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies."
 authors = ["Gabriel Becedillas <gabriel.becedillas@gmail.com>"]
 license = "Apache-2.0"
 packages = [{include = "basana"}]
```

### Comparing `basana-1.3.1/setup.py` & `basana-1.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 packages = \
 ['basana',
  'basana.backtesting',
  'basana.core',
  'basana.core.event_sources',
  'basana.external',
  'basana.external.binance',
+ 'basana.external.binance.client',
  'basana.external.binance.csv',
  'basana.external.binance.tools',
  'basana.external.bitstamp',
  'basana.external.bitstamp.csv',
  'basana.external.bitstamp.tools',
  'basana.external.common',
  'basana.external.common.csv',
@@ -24,15 +25,15 @@
 ['aiohttp[speedups]>=3.8.4,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 extras_require = \
 {'charts': ['plotly>=5.14.1,<6.0.0', 'kaleido==0.2.1']}
 
 setup_kwargs = {
     'name': 'basana',
-    'version': '1.3.1',
+    'version': '1.3.2',
     'description': 'A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.',
     'long_description': 'None',
     'author': 'Gabriel Becedillas',
     'author_email': 'gabriel.becedillas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gbeced/basana',
```

### Comparing `basana-1.3.1/PKG-INFO` & `basana-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basana
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.
 Home-page: https://github.com/gbeced/basana
 License: Apache-2.0
 Author: Gabriel Becedillas
 Author-email: gabriel.becedillas@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

